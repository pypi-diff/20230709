# Comparing `tmp/gmail_draft_creator-1.1.0.tar.gz` & `tmp/gmail_draft_creator-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmail_draft_creator-1.1.0.tar", max compression
+gzip compressed data, was "gmail_draft_creator-1.2.0.tar", max compression
```

## Comparing `gmail_draft_creator-1.1.0.tar` & `gmail_draft_creator-1.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1071 2023-07-04 17:40:55.128486 gmail_draft_creator-1.1.0/LICENSE
--rw-r--r--   0        0        0     3468 2023-07-04 17:40:55.128486 gmail_draft_creator-1.1.0/gmail_draft_creator/__init__.py
--rw-r--r--   0        0        0     1016 2023-07-04 17:41:15.756877 gmail_draft_creator-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1745 2023-07-04 17:40:55.128486 gmail_draft_creator-1.1.0/readme.md
--rw-r--r--   0        0        0     2523 1970-01-01 00:00:00.000000 gmail_draft_creator-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-09 13:14:19.581481 gmail_draft_creator-1.2.0/LICENSE
+-rw-r--r--   0        0        0     4554 2023-07-09 13:14:19.581481 gmail_draft_creator-1.2.0/gmail_draft_creator/__init__.py
+-rw-r--r--   0        0        0     1079 2023-07-09 13:14:41.669720 gmail_draft_creator-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1917 2023-07-09 13:14:19.581481 gmail_draft_creator-1.2.0/readme.md
+-rw-r--r--   0        0        0     2756 1970-01-01 00:00:00.000000 gmail_draft_creator-1.2.0/PKG-INFO
```

### Comparing `gmail_draft_creator-1.1.0/LICENSE` & `gmail_draft_creator-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gmail_draft_creator-1.1.0/gmail_draft_creator/__init__.py` & `gmail_draft_creator-1.2.0/gmail_draft_creator/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,72 +4,103 @@
 import os
 import pickle
 import re
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 from string import Template
 
+import click
 import markdown
 from google.auth.transport.requests import Request
 from google.oauth2.credentials import Credentials
 from google_auth_oauthlib.flow import InstalledAppFlow
 from googleapiclient.discovery import build
 
 SCOPES = [
     "https://www.googleapis.com/auth/gmail.compose",
     "https://www.googleapis.com/auth/gmail.readonly",
     "https://www.googleapis.com/auth/calendar.readonly",
     "https://www.googleapis.com/auth/calendar.events",
 ]
 
-import click
-
 
 @click.command()
 @click.option("--csv", "csv_file_path", type=click.Path(exists=True), help="Path to the CSV file.", required=True)
 @click.option(
     "--template", "template_file_path", type=click.Path(exists=True), help="Path to the template file.", required=True
 )
-@click.option("--subject", "subject", type=str, help="Subject for the email drafts.", required=True)
+@click.option("--subject", "subject", type=str, help="Subject for the email drafts.", required=False)
 @click.option("--dry-run", is_flag=True, default=False, help="Run script without creating drafts.")
 def send_drafts_from_csv_cli(csv_file_path, template_file_path, subject, dry_run):
     send_drafts_from_csv(csv_file_path, template_file_path, subject, dry_run)
 
 
-def send_drafts_from_csv(csv_file_path, template_file_path, subject, dry_run=False):
+def _process_template_string(raw_template_string):
+    # if the first line in the file starts with "Subject: " pull that into a separate variable
+    # and remove it from the template string
+    first_line = raw_template_string.split("\n")[0]
+
+    if first_line.startswith("Subject: "):
+        subject = first_line.replace("Subject: ", "").strip()
+        # remove first line from template string
+        template_string = "\n".join(raw_template_string.split("\n")[1:])
+    else:
+        subject = None
+        template_string = raw_template_string
+
+    template_string = markdown.markdown(template_string.strip())
+
+    return subject, template_string
+
+
+def send_drafts_from_csv(csv_file_path, template_file_path, subject, dry_run):
     with open(template_file_path, "r") as template_file:
-        template_string = markdown.markdown(template_file.read())
+        template_string = template_file.read()
 
     with open(csv_file_path, "r") as file:
         reader = csv.DictReader(file)
         for row in reader:
             email = row.pop("email", None) or row.pop("Email", None)
             template_params = {k.lower(): v for k, v in row.items()}
 
             if email is not None:
-                create_draft(email, subject, template_string, template_params, dry_run)
+                create_draft(email, template_string, template_params, subject, dry_run)
 
 
-def create_draft(email, subject, template_string, template_params, dry_run=False):
+# TODO this should really be much smarter
+def _extract_credentials():
     creds = None
     if os.path.exists("token.pickle"):
         with open("token.pickle", "rb") as token:
             creds = pickle.load(token)
 
     if not creds or not creds.valid:
         if creds and creds.expired and creds.refresh_token:
             creds.refresh(Request())
         else:
             flow = InstalledAppFlow.from_client_secrets_file("credentials.json", SCOPES)
             creds = flow.run_local_server(port=0)
         with open("token.pickle", "wb") as token:
             pickle.dump(creds, token)
 
+    return creds
+
+
+def create_draft(email, template_string, template_params, subject=None, dry_run=False):
+    creds = _extract_credentials()
     service = build("gmail", "v1", credentials=creds)
 
+    template_subject, template_string = _process_template_string(template_string)
+
+    if template_subject and subject:
+        raise ValueError("Subject defined in both template and arguments, pick one")
+
+    subject_template = template_subject or subject
+    subject = Template(subject_template).substitute(template_params)
+
     message_template = Template(template_string)
     message_text = message_template.substitute(template_params)
 
     # remove <p> and </p> tags if they are on the first line
     # this causes weird formatting in gmail
     first_line, remaining_text = message_text.split("\n", 1)
     first_line = re.sub(r"^<p>(.*)</p>$", r"\1", first_line)
```

### Comparing `gmail_draft_creator-1.1.0/pyproject.toml` & `gmail_draft_creator-1.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "gmail_draft_creator"
-version = "1.1.0"
+version = "1.2.0"
 description = "Create draft messages in Gmail"
 authors = ["Michael Bianco <mike@mikebian.co>"]
 license = "MIT"
 readme = "readme.md"
+homepage = "https://github.com/iloveitaly/gmail-draft-creator"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 google-api-python-client = "^2.21.0"
 python-decouple = "^3.5"
 google-auth-httplib2 = "^0.1.0"
 google-auth-oauthlib = "^0.4.6"
```

### Comparing `gmail_draft_creator-1.1.0/readme.md` & `gmail_draft_creator-1.2.0/readme.md`

 * *Files 22% similar despite different names*

```diff
@@ -21,14 +21,24 @@
   --dry-run        Run script without creating drafts.
   --help           Show this message and exit.
 
 ```
 
 You can also import the `create_draft` function and use it in your own scripts.
 
+### Template Files
+
+You can include subject line and variables in the template file:
+
+```text
+Subject: Hello $NAME
+
+Hi, here's another ${REASON} why I'm emailing you.
+```
+
 ## Setup
 
 ### Generating a Gmail API Token
 
 1. Navigate to the Google Cloud Console. https://console.developers.google.com/
 2. Create a new project or select an existing one.
 3. Go to "APIs & Services" -> "Library" and enable the Gmail API.
```

### Comparing `gmail_draft_creator-1.1.0/PKG-INFO` & `gmail_draft_creator-1.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: gmail-draft-creator
-Version: 1.1.0
+Version: 1.2.0
 Summary: Create draft messages in Gmail
+Home-page: https://github.com/iloveitaly/gmail-draft-creator
 License: MIT
 Author: Michael Bianco
 Author-email: mike@mikebian.co
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -42,14 +43,24 @@
   --dry-run        Run script without creating drafts.
   --help           Show this message and exit.
 
 ```
 
 You can also import the `create_draft` function and use it in your own scripts.
 
+### Template Files
+
+You can include subject line and variables in the template file:
+
+```text
+Subject: Hello $NAME
+
+Hi, here's another ${REASON} why I'm emailing you.
+```
+
 ## Setup
 
 ### Generating a Gmail API Token
 
 1. Navigate to the Google Cloud Console. https://console.developers.google.com/
 2. Create a new project or select an existing one.
 3. Go to "APIs & Services" -> "Library" and enable the Gmail API.
```

