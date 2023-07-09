# Comparing `tmp/pygmailsorter-0.0.4.tar.gz` & `tmp/pygmailsorter-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmailsorter-0.0.4.tar", last modified: Sat Oct 29 23:35:15 2022, max compression
+gzip compressed data, was "pygmailsorter-0.0.5.tar", last modified: Sun Jul  9 15:12:34 2023, max compression
```

## Comparing `pygmailsorter-0.0.4.tar` & `pygmailsorter-0.0.5.tar`

### file list

```diff
@@ -1,34 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 23:35:15.552299 pygmailsorter-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1511 2022-10-29 23:35:12.000000 pygmailsorter-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-10-29 23:35:12.000000 pygmailsorter-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6437 2022-10-29 23:35:15.552299 pygmailsorter-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6072 2022-10-29 23:35:12.000000 pygmailsorter-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 23:35:15.552299 pygmailsorter-0.0.4/pygmailsorter/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-10-29 23:35:12.000000 pygmailsorter-0.0.4/pygmailsorter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2616 2022-10-29 23:35:12.000000 pygmailsorter-0.0.4/pygmailsorter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      496 2022-10-29 23:35:15.552299 pygmailsorter-0.0.4/pygmailsorter/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 23:35:15.552299 pygmailsorter-0.0.4/pygmailsorter/base/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-10-29 23:35:12.000000 pygmailsorter-0.0.4/pygmailsorter/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15686 2022-10-29 23:35:12.000000 pygmailsorter-0.0.4/pygmailsorter/base/database.py
--rw-r--r--   0 runner    (1001) docker     (121)     1822 2022-10-29 23:35:12.000000 pygmailsorter-0.0.4/pygmailsorter/base/message.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 23:35:15.552299 pygmailsorter-0.0.4/pygmailsorter/google/
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-10-29 23:35:12.000000 pygmailsorter-0.0.4/pygmailsorter/google/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1817 2022-10-29 23:35:12.000000 pygmailsorter-0.0.4/pygmailsorter/google/authentication.py
--rw-r--r--   0 runner    (1001) docker     (121)     1871 2022-10-29 23:35:12.000000 pygmailsorter-0.0.4/pygmailsorter/google/database.py
--rw-r--r--   0 runner    (1001) docker     (121)    14481 2022-10-29 23:35:12.000000 pygmailsorter-0.0.4/pygmailsorter/google/mail.py
--rw-r--r--   0 runner    (1001) docker     (121)     4450 2022-10-29 23:35:12.000000 pygmailsorter-0.0.4/pygmailsorter/google/message.py
--rw-r--r--   0 runner    (1001) docker     (121)     2246 2022-10-29 23:35:12.000000 pygmailsorter-0.0.4/pygmailsorter/local.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 23:35:15.552299 pygmailsorter-0.0.4/pygmailsorter/ml/
--rw-r--r--   0 runner    (1001) docker     (121)      259 2022-10-29 23:35:12.000000 pygmailsorter-0.0.4/pygmailsorter/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4952 2022-10-29 23:35:12.000000 pygmailsorter-0.0.4/pygmailsorter/ml/database.py
--rw-r--r--   0 runner    (1001) docker     (121)     5994 2022-10-29 23:35:12.000000 pygmailsorter-0.0.4/pygmailsorter/ml/encoding.py
--rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-10-29 23:35:12.000000 pygmailsorter-0.0.4/pygmailsorter/ml/model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 23:35:15.552299 pygmailsorter-0.0.4/pygmailsorter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6437 2022-10-29 23:35:15.000000 pygmailsorter-0.0.4/pygmailsorter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      718 2022-10-29 23:35:15.000000 pygmailsorter-0.0.4/pygmailsorter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-29 23:35:15.000000 pygmailsorter-0.0.4/pygmailsorter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-10-29 23:35:15.000000 pygmailsorter-0.0.4/pygmailsorter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-10-29 23:35:15.000000 pygmailsorter-0.0.4/pygmailsorter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-10-29 23:35:15.552299 pygmailsorter-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      944 2022-10-29 23:35:15.000000 pygmailsorter-0.0.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    68611 2022-10-29 23:35:12.000000 pygmailsorter-0.0.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:12:34.536314 pygmailsorter-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-07-09 15:12:34.536314 pygmailsorter-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:12:34.540314 pygmailsorter-0.0.5/pygmailsorter/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-09 15:12:34.540314 pygmailsorter-0.0.5/pygmailsorter/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:12:34.532314 pygmailsorter-0.0.5/pygmailsorter/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15686 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/base/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/base/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:12:34.536314 pygmailsorter-0.0.5/pygmailsorter/daemon/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/daemon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/daemon/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/daemon/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/daemon/shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/daemon/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:12:34.536314 pygmailsorter-0.0.5/pygmailsorter/google/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/google/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/google/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/google/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14634 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/google/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/google/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:12:34.536314 pygmailsorter-0.0.5/pygmailsorter/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/ml/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/ml/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/ml/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:12:34.532314 pygmailsorter-0.0.5/pygmailsorter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-07-09 15:12:34.000000 pygmailsorter-0.0.5/pygmailsorter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-09 15:12:34.000000 pygmailsorter-0.0.5/pygmailsorter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 15:12:34.000000 pygmailsorter-0.0.5/pygmailsorter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-09 15:12:34.000000 pygmailsorter-0.0.5/pygmailsorter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-09 15:12:34.000000 pygmailsorter-0.0.5/pygmailsorter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-09 15:12:34.000000 pygmailsorter-0.0.5/pygmailsorter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-09 15:12:34.536314 pygmailsorter-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-09 15:12:34.000000 pygmailsorter-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:12:34.536314 pygmailsorter-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/tests/test_google_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/versioneer.py
```

### Comparing `pygmailsorter-0.0.4/LICENSE` & `pygmailsorter-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pygmailsorter-0.0.4/PKG-INFO` & `pygmailsorter-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pygmailsorter
-Version: 0.0.4
+Version: 0.0.5
 Summary: Assign labels to emails in Google Mail based on their similarity to other emails assigned to the same label.
-Home-page: https://github.com/jan-janssen/pygmailsorter
+Home-page: https://github.com/mailsort/pygmailsorter
 Author: Jan Janssen
 Author-email: jan.janssen@outlook.com
 License: BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Sort your emails automatically 
-[![Python package](https://github.com/jan-janssen/pygmailsorter/actions/workflows/unittest.yml/badge.svg?branch=main)](https://github.com/jan-janssen/pygmailsorter/actions/workflows/unittest.yml)
-[![Coverage Status](https://coveralls.io/repos/github/jan-janssen/pygmailsorter/badge.svg?branch=main)](https://coveralls.io/github/jan-janssen/pygmailsorter?branch=main)
+[![Python package](https://github.com/mailsort/pygmailsorter/actions/workflows/unittest.yml/badge.svg?branch=main)](https://github.com/mailsort/pygmailsorter/actions/workflows/unittest.yml)
+[![Coverage Status](https://coveralls.io/repos/github/mailsort/pygmailsorter/badge.svg?branch=main)](https://coveralls.io/github/mailsort/pygmailsorter?branch=main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 The `pygmailsorter` is a python module to automate the filtering of emails on the Google mail service using the their API. It assigns 
 labels to emails based on their similarity to other emails assigned to the same label.
 
 # Motivation 
 Many people struggle with the increasing email volume leading to hundreds of unread emails. As the capabilities of even the best search engine are limited when it comes to large numbers of emails, the only way to keep an overview is filing emails into folders. The manual work of filing emails into folders is tedious, still most people are too lazy to create email filters and keep their email filters up to date. Finally, in the age of mobile computing when most people access their emails from their smartphone, the challenge of sorting emails is more relevant than ever.
```

### Comparing `pygmailsorter-0.0.4/README.md` & `pygmailsorter-0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Sort your emails automatically 
-[![Python package](https://github.com/jan-janssen/pygmailsorter/actions/workflows/unittest.yml/badge.svg?branch=main)](https://github.com/jan-janssen/pygmailsorter/actions/workflows/unittest.yml)
-[![Coverage Status](https://coveralls.io/repos/github/jan-janssen/pygmailsorter/badge.svg?branch=main)](https://coveralls.io/github/jan-janssen/pygmailsorter?branch=main)
+[![Python package](https://github.com/mailsort/pygmailsorter/actions/workflows/unittest.yml/badge.svg?branch=main)](https://github.com/mailsort/pygmailsorter/actions/workflows/unittest.yml)
+[![Coverage Status](https://coveralls.io/repos/github/mailsort/pygmailsorter/badge.svg?branch=main)](https://coveralls.io/github/mailsort/pygmailsorter?branch=main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 The `pygmailsorter` is a python module to automate the filtering of emails on the Google mail service using the their API. It assigns 
 labels to emails based on their similarity to other emails assigned to the same label.
 
 # Motivation 
 Many people struggle with the increasing email volume leading to hundreds of unread emails. As the capabilities of even the best search engine are limited when it comes to large numbers of emails, the only way to keep an overview is filing emails into folders. The manual work of filing emails into folders is tedious, still most people are too lazy to create email filters and keep their email filters up to date. Finally, in the age of mobile computing when most people access their emails from their smartphone, the challenge of sorting emails is more relevant than ever.
```

### Comparing `pygmailsorter-0.0.4/pygmailsorter/__main__.py` & `pygmailsorter-0.0.5/pygmailsorter/__main__.py`

 * *Files identical despite different names*

### Comparing `pygmailsorter-0.0.4/pygmailsorter/base/database.py` & `pygmailsorter-0.0.5/pygmailsorter/base/database.py`

 * *Files identical despite different names*

### Comparing `pygmailsorter-0.0.4/pygmailsorter/base/message.py` & `pygmailsorter-0.0.5/pygmailsorter/base/message.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from abc import ABC, abstractmethod
 from datetime import datetime
 
 
 def email_date_converter(email_date):
+    if not isinstance(email_date, str):
+        return None
     if email_date.count(",") >= 2:
         email_date = ", ".join(email_date.split(", ")[-2:])
     if email_date[-3:-2].isalpha():
         email_date = " ".join(email_date.split()[:-1])
     if email_date[-1].isalpha():
         email_date = email_date[:-1]
     if email_date[:3].isalpha() and email_date[-3] != ":":
```

### Comparing `pygmailsorter-0.0.4/pygmailsorter/google/authentication.py` & `pygmailsorter-0.0.5/pygmailsorter/google/authentication.py`

 * *Files identical despite different names*

### Comparing `pygmailsorter-0.0.4/pygmailsorter/google/database.py` & `pygmailsorter-0.0.5/pygmailsorter/google/database.py`

 * *Files identical despite different names*

### Comparing `pygmailsorter-0.0.4/pygmailsorter/google/mail.py` & `pygmailsorter-0.0.5/pygmailsorter/google/mail.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,24 +202,28 @@
             email_format (str): Email format to download - default: "full"
 
         Returns:
             pandas.DataFrame: pandas.DataFrame which contains the rendered emails
         """
         return pandas.DataFrame(
             [
-                get_email_dict(
-                    message=self._get_message_detail(
-                        message_id=message_id,
-                        email_format=email_format,
-                        metadata_headers=[],
+                message
+                for message in [
+                    get_email_dict(
+                        message=self._get_message_detail(
+                            message_id=message_id,
+                            email_format=email_format,
+                            metadata_headers=[],
+                        )
                     )
-                )
-                for message_id in tqdm(
-                    iterable=message_id_lst, desc="Download messagees to DataFrame"
-                )
+                    for message_id in tqdm(
+                        iterable=message_id_lst, desc="Download messages to DataFrame"
+                    )
+                ]
+                if message is not None
             ]
         )
 
     def _get_labels_for_email(self, message_id):
         """
         Get labels for email
```

### Comparing `pygmailsorter-0.0.4/pygmailsorter/google/message.py` & `pygmailsorter-0.0.5/pygmailsorter/google/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,19 @@
         self.text.write(d)
 
     def get_data(self):
         return self.text.getvalue()
 
 
 def get_email_dict(message):
-    return Message(message_dict=message).to_dict()
+    try:
+        return Message(message_dict=message).to_dict()
+    except ValueError as e:
+        print(message, e.message)
+        return None
 
 
 class Message(AbstractMessage):
     def __init__(self, message_dict):
         self._message_dict = message_dict
 
     def get_from(self):
```

### Comparing `pygmailsorter-0.0.4/pygmailsorter/local.py` & `pygmailsorter-0.0.5/pygmailsorter/local.py`

 * *Files identical despite different names*

### Comparing `pygmailsorter-0.0.4/pygmailsorter/ml/database.py` & `pygmailsorter-0.0.5/pygmailsorter/ml/database.py`

 * *Files identical despite different names*

### Comparing `pygmailsorter-0.0.4/pygmailsorter/ml/encoding.py` & `pygmailsorter-0.0.5/pygmailsorter/ml/encoding.py`

 * *Files identical despite different names*

### Comparing `pygmailsorter-0.0.4/pygmailsorter/ml/model.py` & `pygmailsorter-0.0.5/pygmailsorter/ml/model.py`

 * *Files identical despite different names*

### Comparing `pygmailsorter-0.0.4/pygmailsorter.egg-info/PKG-INFO` & `pygmailsorter-0.0.5/pygmailsorter.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pygmailsorter
-Version: 0.0.4
+Version: 0.0.5
 Summary: Assign labels to emails in Google Mail based on their similarity to other emails assigned to the same label.
-Home-page: https://github.com/jan-janssen/pygmailsorter
+Home-page: https://github.com/mailsort/pygmailsorter
 Author: Jan Janssen
 Author-email: jan.janssen@outlook.com
 License: BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Sort your emails automatically 
-[![Python package](https://github.com/jan-janssen/pygmailsorter/actions/workflows/unittest.yml/badge.svg?branch=main)](https://github.com/jan-janssen/pygmailsorter/actions/workflows/unittest.yml)
-[![Coverage Status](https://coveralls.io/repos/github/jan-janssen/pygmailsorter/badge.svg?branch=main)](https://coveralls.io/github/jan-janssen/pygmailsorter?branch=main)
+[![Python package](https://github.com/mailsort/pygmailsorter/actions/workflows/unittest.yml/badge.svg?branch=main)](https://github.com/mailsort/pygmailsorter/actions/workflows/unittest.yml)
+[![Coverage Status](https://coveralls.io/repos/github/mailsort/pygmailsorter/badge.svg?branch=main)](https://coveralls.io/github/mailsort/pygmailsorter?branch=main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 The `pygmailsorter` is a python module to automate the filtering of emails on the Google mail service using the their API. It assigns 
 labels to emails based on their similarity to other emails assigned to the same label.
 
 # Motivation 
 Many people struggle with the increasing email volume leading to hundreds of unread emails. As the capabilities of even the best search engine are limited when it comes to large numbers of emails, the only way to keep an overview is filing emails into folders. The manual work of filing emails into folders is tedious, still most people are too lazy to create email filters and keep their email filters up to date. Finally, in the age of mobile computing when most people access their emails from their smartphone, the challenge of sorting emails is more relevant than ever.
```

### Comparing `pygmailsorter-0.0.4/versioneer.py` & `pygmailsorter-0.0.5/versioneer.py`

 * *Files identical despite different names*

