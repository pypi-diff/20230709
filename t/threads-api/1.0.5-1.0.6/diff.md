# Comparing `tmp/threads-api-1.0.5.tar.gz` & `tmp/threads-api-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threads-api-1.0.5.tar", last modified: Sat Jul  8 20:31:04 2023, max compression
+gzip compressed data, was "threads-api-1.0.6.tar", last modified: Sun Jul  9 20:54:15 2023, max compression
```

## Comparing `threads-api-1.0.5.tar` & `threads-api-1.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-08 20:31:04.895779 threads-api-1.0.5/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1068 2023-07-06 22:22:29.000000 threads-api-1.0.5/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     9508 2023-07-08 20:31:04.895779 threads-api-1.0.5/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     8982 2023-07-08 20:30:17.000000 threads-api-1.0.5/README.md
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      349 2023-07-06 21:24:15.000000 threads-api-1.0.5/pyproject.toml
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-08 20:31:04.895779 threads-api-1.0.5/setup.cfg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      785 2023-07-08 20:29:32.000000 threads-api-1.0.5/setup.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-08 20:31:04.895779 threads-api-1.0.5/threads_api/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 20:59:49.000000 threads-api-1.0.5/threads_api/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-08 20:31:04.895779 threads-api-1.0.5/threads_api/src/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:13:21.000000 threads-api-1.0.5/threads_api/src/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    15315 2023-07-07 21:21:06.000000 threads-api-1.0.5/threads_api/src/threads_api.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-08 20:31:04.895779 threads-api-1.0.5/threads_api/tests/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:19:18.000000 threads-api-1.0.5/threads_api/tests/__init__.py
--rwxrwxr-x   0 daniel    (1000) daniel    (1000)      404 2023-07-07 21:21:06.000000 threads-api-1.0.5/threads_api/tests/get_threads_test.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-08 20:31:04.895779 threads-api-1.0.5/threads_api.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     9508 2023-07-08 20:31:04.000000 threads-api-1.0.5/threads_api.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      366 2023-07-08 20:31:04.000000 threads-api-1.0.5/threads_api.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-08 20:31:04.000000 threads-api-1.0.5/threads_api.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       17 2023-07-08 20:31:04.000000 threads-api-1.0.5/threads_api.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       12 2023-07-08 20:31:04.000000 threads-api-1.0.5/threads_api.egg-info/top_level.txt
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-09 20:54:15.300830 threads-api-1.0.6/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1068 2023-07-06 22:22:29.000000 threads-api-1.0.6/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    10074 2023-07-09 20:54:15.296830 threads-api-1.0.6/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     9548 2023-07-09 20:54:06.000000 threads-api-1.0.6/README.md
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      349 2023-07-06 21:24:15.000000 threads-api-1.0.6/pyproject.toml
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-09 20:54:15.300830 threads-api-1.0.6/setup.cfg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      785 2023-07-09 20:52:30.000000 threads-api-1.0.6/setup.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-09 20:54:15.296830 threads-api-1.0.6/threads_api/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 20:59:49.000000 threads-api-1.0.6/threads_api/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-09 20:54:15.296830 threads-api-1.0.6/threads_api/src/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:13:21.000000 threads-api-1.0.6/threads_api/src/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    18821 2023-07-09 20:45:43.000000 threads-api-1.0.6/threads_api/src/threads_api.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-09 20:54:15.296830 threads-api-1.0.6/threads_api/tests/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:19:18.000000 threads-api-1.0.6/threads_api/tests/__init__.py
+-rwxrwxr-x   0 daniel    (1000) daniel    (1000)      404 2023-07-07 21:21:06.000000 threads-api-1.0.6/threads_api/tests/get_threads_test.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-09 20:54:15.296830 threads-api-1.0.6/threads_api.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    10074 2023-07-09 20:54:15.000000 threads-api-1.0.6/threads_api.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      366 2023-07-09 20:54:15.000000 threads-api-1.0.6/threads_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-09 20:54:15.000000 threads-api-1.0.6/threads_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       17 2023-07-09 20:54:15.000000 threads-api-1.0.6/threads_api.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       12 2023-07-09 20:54:15.000000 threads-api-1.0.6/threads_api.egg-info/top_level.txt
```

### Comparing `threads-api-1.0.5/LICENSE` & `threads-api-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `threads-api-1.0.5/PKG-INFO` & `threads-api-1.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threads-api
-Version: 1.0.5
+Version: 1.0.6
 Summary: Unofficial Python client for Meta Threads API
 Home-page: https://github.com/danie1/threads-api
 Author: Danie1
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -248,24 +248,48 @@
 -
 winchester_757's Reply: {'text': 'If only the meta verse was this good LMAO'} || Likes: 0
 -
 winchester_757's Reply: {'text': 'Only 10 mil more to match the big guy'} || Likes: 0
 ```
 </details>
 
+<details>
+  <summary>"post" Function</summary>
+
+``` python
+async def post():
+    threads_api = ThreadsAPI()
+    # either set USERNAME and PASSWORD as environment variables, or replace these with your actual credentials
+    await threads_api.login(os.environ.get('USERNAME'), os.environ.get('PASSWORD'))
+    result = await threads_api.post("Hello World!")
+
+    if result:
+        print("Post has been successfully posted")
+    else:
+        print("Unable to post.")
+```
+
+Example Output:
+```
+Post has been successfully posted
+```
+</details>
+
 ## 📌 Roadmap
 
+- [x] ✅ Login as User
+- [x] ✅ Write Posts
 - [x] ✅ Read public data\
   - [x] ✅ Fetch UserID(`314216`) via username(`zuck`)
   - [x] ✅ Read user profile info
   - [x] ✅ Read list of user Threads
   - [x] ✅ Read list of user Replies
   - [x] ✅ Read Post and a list of its Replies
-- [ ] 🚧 Read private data
-- [ ] 🚧 Write data (i.e. write automated Threads)
+- [ ]🚧  Upload images and videos
+- [ ]🚧  Reply to Posts
 - [ ]🚧  CI/CD
   - [ ]🚧  Pytest
   - [ ]🚧  GitHub Actions Pipeline
 
 
 # License
 This project is licensed under the MIT license.
```

### Comparing `threads-api-1.0.5/README.md` & `threads-api-1.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -231,24 +231,48 @@
 -
 winchester_757's Reply: {'text': 'If only the meta verse was this good LMAO'} || Likes: 0
 -
 winchester_757's Reply: {'text': 'Only 10 mil more to match the big guy'} || Likes: 0
 ```
 </details>
 
+<details>
+  <summary>"post" Function</summary>
+
+``` python
+async def post():
+    threads_api = ThreadsAPI()
+    # either set USERNAME and PASSWORD as environment variables, or replace these with your actual credentials
+    await threads_api.login(os.environ.get('USERNAME'), os.environ.get('PASSWORD'))
+    result = await threads_api.post("Hello World!")
+
+    if result:
+        print("Post has been successfully posted")
+    else:
+        print("Unable to post.")
+```
+
+Example Output:
+```
+Post has been successfully posted
+```
+</details>
+
 ## 📌 Roadmap
 
+- [x] ✅ Login as User
+- [x] ✅ Write Posts
 - [x] ✅ Read public data\
   - [x] ✅ Fetch UserID(`314216`) via username(`zuck`)
   - [x] ✅ Read user profile info
   - [x] ✅ Read list of user Threads
   - [x] ✅ Read list of user Replies
   - [x] ✅ Read Post and a list of its Replies
-- [ ] 🚧 Read private data
-- [ ] 🚧 Write data (i.e. write automated Threads)
+- [ ]🚧  Upload images and videos
+- [ ]🚧  Reply to Posts
 - [ ]🚧  CI/CD
   - [ ]🚧  Pytest
   - [ ]🚧  GitHub Actions Pipeline
 
 
 # License
 This project is licensed under the MIT license.
```

### Comparing `threads-api-1.0.5/setup.py` & `threads-api-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='threads-api',
-    version='1.0.5',
+    version='1.0.6',
     description='Unofficial Python client for Meta Threads API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Danie1',
     author_email='',
     url='https://github.com/danie1/threads-api',
     packages=find_packages(),
```

### Comparing `threads-api-1.0.5/threads_api/src/threads_api.py` & `threads-api-1.0.6/threads_api/src/threads_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,58 +1,97 @@
 import requests
 from typing import Optional, Dict, Union, List
 import aiohttp
 import re
 import json
-
-class Extensions:
-    # Define the Extensions class if necessary
-    pass
-
-class Thread:
-    # Define the Thread class if necessary
-    pass
-
-class ThreadsUser:
-    # Define the ThreadsUser class if necessary
-    pass
-
-class GetUserProfileResponse:
-    def __init__(self, data: Dict[str, Union[Dict[str, Union[ThreadsUser, Dict[str, Union[str, int]]]], Extensions]]):
-        self.data = data['data']
-        self.extensions = data['extensions']
-
-class GetUserProfileThreadsResponse:
-    def __init__(self, data: Dict[str, Union[Dict[str, List[Thread]] , Extensions]]):
-        self.data = data['data']
-        self.extensions = data['extensions']
+import asyncio
+import json
+import random
+from datetime import datetime
+import urllib.parse
+import random
+import urllib
+import os
+import mimetypes
+import uuid
+import time
 
 class ThreadsAPIOptions:
-    def __init__(self, fbLSDToken: Optional[str] = None):
+    def __init__(self, fbLSDToken: Optional[str] = None, 
+                       token: Optional[str] = None):
         self.fbLSDToken = fbLSDToken
+        self.token = token
 
 class ThreadsAPI:
     def __init__(self, options: Optional[ThreadsAPIOptions] = None):
-        self.fbLSDToken = 'NjppQDEgONsU_1LCzrmp6q'  # FIXME: Remove default value
+        self.fbLSDToken = 'NjppQDEgONsU_1LCzrmp6q'
+        self.token = None
+        self.user_id = None
+
         if options and options.fbLSDToken:
             self.fbLSDToken = options.fbLSDToken
 
-    def _get_default_headers(self, username: str) -> Dict[str, Union[str, int]]:
-        return {
-            'authority': 'www.threads.net',
-            'accept': '*/*',
-            'accept-language': 'ko',
-            'cache-control': 'no-cache',
-            'origin': 'https://www.threads.net',
-            'pragma': 'no-cache',
-            'referer': f'https://www.threads.net/@{username}',
-            'x-asbd-id': '129477',
-            'x-fb-lsd': self.fbLSDToken,
-            'x-ig-app-id': '238260118697367',
-        }
+        if options and options.token:
+            self.token = options.token
+
+    async def login(self, username, password):
+        if username is None or password is None:
+            return None
+        
+        self.username = username
+
+        try:
+            blockVersion = "5f56efad68e1edec7801f630b5c122704ec5378adbee6609a448f105f34a9c73"
+            headers = {
+                "User-Agent": "Barcelona 289.0.0.77.109 Android",
+                "Sec-Fetch-Site": "same-origin",
+                "Content-Type": "application/x-www-form-urlencoded; charset=UTF-8",
+            }
+            params = json.dumps(
+                {
+                    "client_input_params": {
+                        "password": password,
+                        "contact_point": username,
+                        "device_id": f"android-{random.randint(0, 1e24):x}",
+                    },
+                    "server_params": {
+                        "credential_type": "password",
+                        "device_id": f"android-{random.randint(0, 1e24):x}",
+                    },
+                }
+            )
+            bk_client_context = json.dumps(
+                {"bloks_version": blockVersion, "styles_id": "instagram"}
+            )
+
+            LOGIN_URL = "https://i.instagram.com/api/v1/bloks/apps/com.bloks.www.bloks.caa.login.async.send_login_request/"
+            payload = f"params={urllib.parse.quote(params)}&bk_client_context={urllib.parse.quote(bk_client_context)}&bloks_versioning_id={blockVersion}"
+            
+            async with aiohttp.ClientSession() as session:
+                async with session.post(LOGIN_URL, timeout=60 * 1000, headers=headers, data=payload) as response:
+                    data = await response.text()
+            
+            print(data)
+            if data == "Oops, an error occurred.":
+                raise Exception("Failed to login")
+            
+            pos = data.split("Bearer IGT:2:")
+
+            if len(pos) > 1:
+                pos = pos[1]
+                pos = pos.split("==")[0]
+                token = f"{pos}=="
+                self.token = token
+
+                self.user_id = await self.get_user_id_from_username(username)
+                return True
+            return False
+        except Exception as e:
+            print("[ERROR] ", e)
+            raise
 
     async def get_user_id_from_username(self, username: str) -> str:
         url = f"https://www.threads.net/@{username}"
         headers = {
             "authority": "www.threads.net",
             "accept": "*/*",
             "accept-language": "ko",
@@ -67,14 +106,19 @@
 
         async with aiohttp.ClientSession() as session:
             async with session.get(url, headers=headers) as response:
                 text = await response.text()
 
         text = text.replace('\\s', "").replace('\\n', "")
         user_id = re.search(r'"props":{"user_id":"(\d+)"},', text)
+
+        lsd_token_match = re.search('"LSD",\[\],{"token":"(\w+)"},\d+\]', text)
+        lsd_token = lsd_token_match.group(1) if lsd_token_match else None
+        self.fbLSDToken = lsd_token
+
         return user_id.group(1) if user_id else None
 
     async def get_user_profile(self, username: str, user_id: str):
         url = 'https://www.threads.net/api/graphql'
         headers = {
             'authority': 'www.threads.net',
             'accept': '*/*',
@@ -341,8 +385,54 @@
                 try:
                     text = await response.text()
                     data = json.loads(text)
                 except (aiohttp.ContentTypeError, json.JSONDecodeError):
                     raise Exception('Failed to decode response as JSON')
 
         threads = data['data']['data']
-        return threads
+        return threads
+                
+    async def post(self, caption: str) -> bool:
+        if self.user_id is None:
+            raise Exception("Failed to resolve user_id. You must login to post posts")
+
+        if self.token is None:
+            raise Exception("Failed to resolve token. You must login to post posts")
+
+        params = json.dumps(
+            {
+                "publish_mode": "text_post",
+                "text_post_app_info": '{"reply_control":0}',
+                "timezone_offset": "-25200",
+                "source_type": "4",
+                "_uid": self.user_id,
+                "device_id": f"android-{random.randint(0, 1e24):x}",
+                "caption": caption,
+                "upload_id": str(int(datetime.now().timestamp() * 1000)),
+                "device": {
+                    "manufacturer": "OnePlus",
+                    "model": "ONEPLUS+A3010",
+                    "android_version": 25,
+                    "android_release": "7.1.1",
+                },
+            }
+        )
+        POST_HEADERS_DEFAULT = {
+            "User-Agent": "Barcelona 289.0.0.77.109 Android",
+            "Sec-Fetch-Site": "same-origin",
+            "Content-Type": "application/x-www-form-urlencoded; charset=UTF-8",
+        }
+
+        payload = f"signed_body=SIGNATURE.{urllib.parse.quote(params)}"
+        headers = POST_HEADERS_DEFAULT.copy()
+        headers.update({"Authorization": f"Bearer IGT:2:{self.token}"})
+
+        try:
+            async with aiohttp.ClientSession() as session:
+                async with session.post("https://i.instagram.com/api/v1/media/configure_text_only_post/", headers=headers, data=payload) as response:
+                    if response.status == 200:
+                        return True
+                    else:
+                        return False
+        except Exception as e:
+            print("[ERROR] ", e)
+            return False
```

### Comparing `threads-api-1.0.5/threads_api.egg-info/PKG-INFO` & `threads-api-1.0.6/threads_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threads-api
-Version: 1.0.5
+Version: 1.0.6
 Summary: Unofficial Python client for Meta Threads API
 Home-page: https://github.com/danie1/threads-api
 Author: Danie1
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -248,24 +248,48 @@
 -
 winchester_757's Reply: {'text': 'If only the meta verse was this good LMAO'} || Likes: 0
 -
 winchester_757's Reply: {'text': 'Only 10 mil more to match the big guy'} || Likes: 0
 ```
 </details>
 
+<details>
+  <summary>"post" Function</summary>
+
+``` python
+async def post():
+    threads_api = ThreadsAPI()
+    # either set USERNAME and PASSWORD as environment variables, or replace these with your actual credentials
+    await threads_api.login(os.environ.get('USERNAME'), os.environ.get('PASSWORD'))
+    result = await threads_api.post("Hello World!")
+
+    if result:
+        print("Post has been successfully posted")
+    else:
+        print("Unable to post.")
+```
+
+Example Output:
+```
+Post has been successfully posted
+```
+</details>
+
 ## 📌 Roadmap
 
+- [x] ✅ Login as User
+- [x] ✅ Write Posts
 - [x] ✅ Read public data\
   - [x] ✅ Fetch UserID(`314216`) via username(`zuck`)
   - [x] ✅ Read user profile info
   - [x] ✅ Read list of user Threads
   - [x] ✅ Read list of user Replies
   - [x] ✅ Read Post and a list of its Replies
-- [ ] 🚧 Read private data
-- [ ] 🚧 Write data (i.e. write automated Threads)
+- [ ]🚧  Upload images and videos
+- [ ]🚧  Reply to Posts
 - [ ]🚧  CI/CD
   - [ ]🚧  Pytest
   - [ ]🚧  GitHub Actions Pipeline
 
 
 # License
 This project is licensed under the MIT license.
```

