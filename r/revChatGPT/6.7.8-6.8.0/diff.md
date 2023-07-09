# Comparing `tmp/revChatGPT-6.7.8.tar.gz` & `tmp/revChatGPT-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-6.7.8.tar", last modified: Sat Jul  8 11:47:46 2023, max compression
+gzip compressed data, was "revChatGPT-6.8.0.tar", last modified: Sun Jul  9 05:02:17 2023, max compression
```

## Comparing `revChatGPT-6.7.8.tar` & `revChatGPT-6.8.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:46.037971 revChatGPT-6.7.8/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-08 11:47:17.000000 revChatGPT-6.7.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-07-08 11:47:46.041971 revChatGPT-6.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-07-08 11:47:45.000000 revChatGPT-6.7.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-08 11:47:46.041971 revChatGPT-6.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-08 11:47:17.000000 revChatGPT-6.7.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:46.037971 revChatGPT-6.7.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:46.037971 revChatGPT-6.7.8/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    60775 2023-07-08 11:47:17.000000 revChatGPT-6.7.8/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    25069 2023-07-08 11:47:17.000000 revChatGPT-6.7.8/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-08 11:47:17.000000 revChatGPT-6.7.8/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-08 11:47:17.000000 revChatGPT-6.7.8/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:46.037971 revChatGPT-6.7.8/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-08 11:47:17.000000 revChatGPT-6.7.8/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-07-08 11:47:17.000000 revChatGPT-6.7.8/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-08 11:47:17.000000 revChatGPT-6.7.8/src/revChatGPT/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-08 11:47:17.000000 revChatGPT-6.7.8/src/revChatGPT/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:46.037971 revChatGPT-6.7.8/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-07-08 11:47:46.000000 revChatGPT-6.7.8/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-08 11:47:46.000000 revChatGPT-6.7.8/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 11:47:46.000000 revChatGPT-6.7.8/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-08 11:47:46.000000 revChatGPT-6.7.8/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-08 11:47:46.000000 revChatGPT-6.7.8/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:46.037971 revChatGPT-6.7.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-08 11:47:17.000000 revChatGPT-6.7.8/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 05:02:17.384767 revChatGPT-6.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-09 05:01:50.000000 revChatGPT-6.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-07-09 05:02:17.384767 revChatGPT-6.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-07-09 05:02:17.000000 revChatGPT-6.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-09 05:02:17.384767 revChatGPT-6.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-09 05:01:50.000000 revChatGPT-6.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 05:02:17.380767 revChatGPT-6.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 05:02:17.384767 revChatGPT-6.8.0/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    62593 2023-07-09 05:01:50.000000 revChatGPT-6.8.0/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25069 2023-07-09 05:01:50.000000 revChatGPT-6.8.0/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-09 05:01:50.000000 revChatGPT-6.8.0/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-09 05:01:50.000000 revChatGPT-6.8.0/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 05:02:17.384767 revChatGPT-6.8.0/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-09 05:01:50.000000 revChatGPT-6.8.0/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-07-09 05:01:50.000000 revChatGPT-6.8.0/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-09 05:01:50.000000 revChatGPT-6.8.0/src/revChatGPT/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-09 05:01:50.000000 revChatGPT-6.8.0/src/revChatGPT/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 05:02:17.384767 revChatGPT-6.8.0/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-07-09 05:02:17.000000 revChatGPT-6.8.0/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-09 05:02:17.000000 revChatGPT-6.8.0/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 05:02:17.000000 revChatGPT-6.8.0/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-09 05:02:17.000000 revChatGPT-6.8.0/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-09 05:02:17.000000 revChatGPT-6.8.0/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 05:02:17.384767 revChatGPT-6.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-09 05:01:50.000000 revChatGPT-6.8.0/tests/test_recipient.py
```

### Comparing `revChatGPT-6.7.8/LICENSE` & `revChatGPT-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.8/PKG-INFO` & `revChatGPT-6.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.7.8
+Version: 6.8.0
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.7.8/README.md` & `revChatGPT-6.8.0/README.md`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.8/setup.py` & `revChatGPT-6.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.8/src/revChatGPT/V1.py` & `revChatGPT-6.8.0/src/revChatGPT/V1.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 except ImportError:
     pass
 from pathlib import Path
 from typing import AsyncGenerator
 from typing import Generator
 from typing import NoReturn
 import tempfile
+import random
 
 # Import function type
 from typing import Callable as function
 
 import httpx
 import requests
 from httpx import AsyncClient
@@ -152,53 +153,88 @@
 
 CAPTCHA_URL = getenv("CAPTCHA_URL", "https://bypass.churchless.tech/captcha/")
 
 
 def get_arkose_token(
     download_images: bool = True,
     solver: function = captcha_solver,
+    captcha_supported: bool = True,
 ) -> str:
     """
     The solver function should take in a list of images in base64 and a dict of challenge details
     and return the index of the image that matches the challenge details
 
     Challenge details:
         game_type: str - Audio or Image
         instructions: str - Instructions for the captcha
         URLs: list[str] - URLs of the images or audio files
     """
-    resp = requests.get(
-        (CAPTCHA_URL + "start?download_images=true")
-        if download_images
-        else CAPTCHA_URL + "start",
-    )
-    resp_json: dict = resp.json()
-    if resp.status_code == 200:
+    if captcha_supported:
+        resp = requests.get(
+            (CAPTCHA_URL + "start?download_images=true")
+            if download_images
+            else CAPTCHA_URL + "start",
+        )
+        resp_json: dict = resp.json()
+        if resp.status_code == 200:
+            return resp_json.get("token")
+        if resp.status_code != 511:
+            raise Exception(resp_json.get("error", "Unknown error"))
+
+        if resp_json.get("status") != "captcha":
+            raise Exception("unknown error")
+
+        challenge_details: dict = resp_json.get("session", {}).get("concise_challenge")
+        if not challenge_details:
+            raise Exception("missing details")
+
+        images: list[str] = resp_json.get("images")
+
+        index = solver(images, challenge_details)
+
+        resp = requests.post(
+            CAPTCHA_URL + "verify",
+            json={"session": resp_json.get("session"), "index": index},
+        )
+        if resp.status_code != 200:
+            raise Exception("Failed to verify captcha")
         return resp_json.get("token")
-    if resp.status_code != 511:
-        raise Exception(resp_json.get("error", "Unknown error"))
-
-    if resp_json.get("status") != "captcha":
-        raise Exception("unknown error")
-
-    challenge_details: dict = resp_json.get("session", {}).get("concise_challenge")
-    if not challenge_details:
-        raise Exception("missing details")
-
-    images: list[str] = resp_json.get("images")
-
-    index = solver(images, challenge_details)
-
-    resp = requests.post(
-        CAPTCHA_URL + "verify",
-        json={"session": resp_json.get("session"), "index": index},
-    )
-    if resp.status_code != 200:
-        raise Exception("Failed to verify captcha")
-    return resp_json.get("token")
+    else:
+        working_endpoints: list[str] = []
+        # Check uptime for different endpoints via gatus
+        resp: list[dict] = requests.get(
+            "https://stats.churchless.tech/api/v1/endpoints/statuses?page=1"
+        ).json()
+        for endpoint in resp:
+            if endpoint.get("group") != "Arkose Labs":
+                continue
+            # Check the last 5 results
+            results: list[dict] = endpoint.get("results", [])[:5]
+            if not results:
+                continue
+            # Check if all the results are up
+            if all(result.get("success") == True for result in results):
+                working_endpoints.append(endpoint.get("name"))
+        if not working_endpoints:
+            print("No working endpoints found. Please solve the captcha manually.")
+            return get_arkose_token(download_images=True, captcha_supported=True)
+        # Choose a random endpoint
+        endpoint = random.choice(working_endpoints)
+        print(f"Using endpoint {endpoint} for captcha")
+        resp: requests.Response = requests.get(endpoint)
+        if resp.status_code != 200:
+            if resp.status_code != 511:
+                raise Exception("Failed to get captcha token")
+            else:
+                print("Captcha required. Please solve the captcha manually.")
+                return get_arkose_token(download_images=True, captcha_supported=True)
+        try:
+            return resp.json().get("token")
+        except Exception:
+            return resp.text
 
 
 class Chatbot:
     """
     Chatbot class for ChatGPT
     """
 
@@ -482,15 +518,17 @@
             and not self.config.get("SERVER_SIDE_ARKOSE")
             and not getenv("SERVER_SIDE_ARKOSE")
         ):
             try:
                 data["arkose_token"] = get_arkose_token(
                     self.captcha_download_images,
                     self.captcha_solver,
+                    captcha_supported=False,
                 )
+                # print(f"Arkose token obtained: {data['arkose_token']}")
             except Exception as e:
                 print(e)
                 raise e
 
         cid, pid = data["conversation_id"], data["parent_message_id"]
         message = ""
```

### Comparing `revChatGPT-6.7.8/src/revChatGPT/V3.py` & `revChatGPT-6.8.0/src/revChatGPT/V3.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.8/src/revChatGPT/__init__.py` & `revChatGPT-6.8.0/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.8/src/revChatGPT/__main__.py` & `revChatGPT-6.8.0/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.8/src/revChatGPT/config/enable_internet.json` & `revChatGPT-6.8.0/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.8/src/revChatGPT/typings.py` & `revChatGPT-6.8.0/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.8/src/revChatGPT/utils.py` & `revChatGPT-6.8.0/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.8/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-6.8.0/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.7.8
+Version: 6.8.0
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.7.8/tests/test_recipient.py` & `revChatGPT-6.8.0/tests/test_recipient.py`

 * *Files identical despite different names*

