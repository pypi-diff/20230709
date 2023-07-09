# Comparing `tmp/revChatGPT-6.8.0.tar.gz` & `tmp/revChatGPT-6.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-6.8.0.tar", last modified: Sun Jul  9 05:02:17 2023, max compression
+gzip compressed data, was "revChatGPT-6.8.1.tar", last modified: Sun Jul  9 06:01:53 2023, max compression
```

## Comparing `revChatGPT-6.8.0.tar` & `revChatGPT-6.8.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 05:02:17.384767 revChatGPT-6.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-09 05:01:50.000000 revChatGPT-6.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-07-09 05:02:17.384767 revChatGPT-6.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-07-09 05:02:17.000000 revChatGPT-6.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-09 05:02:17.384767 revChatGPT-6.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-09 05:01:50.000000 revChatGPT-6.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 05:02:17.380767 revChatGPT-6.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 05:02:17.384767 revChatGPT-6.8.0/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    62593 2023-07-09 05:01:50.000000 revChatGPT-6.8.0/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    25069 2023-07-09 05:01:50.000000 revChatGPT-6.8.0/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-09 05:01:50.000000 revChatGPT-6.8.0/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-09 05:01:50.000000 revChatGPT-6.8.0/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 05:02:17.384767 revChatGPT-6.8.0/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-09 05:01:50.000000 revChatGPT-6.8.0/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-07-09 05:01:50.000000 revChatGPT-6.8.0/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-09 05:01:50.000000 revChatGPT-6.8.0/src/revChatGPT/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-09 05:01:50.000000 revChatGPT-6.8.0/src/revChatGPT/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 05:02:17.384767 revChatGPT-6.8.0/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-07-09 05:02:17.000000 revChatGPT-6.8.0/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-09 05:02:17.000000 revChatGPT-6.8.0/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 05:02:17.000000 revChatGPT-6.8.0/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-09 05:02:17.000000 revChatGPT-6.8.0/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-09 05:02:17.000000 revChatGPT-6.8.0/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 05:02:17.384767 revChatGPT-6.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-09 05:01:50.000000 revChatGPT-6.8.0/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:01:53.546250 revChatGPT-6.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-09 06:01:21.000000 revChatGPT-6.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-07-09 06:01:53.546250 revChatGPT-6.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-07-09 06:01:53.000000 revChatGPT-6.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-09 06:01:53.546250 revChatGPT-6.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-09 06:01:21.000000 revChatGPT-6.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:01:53.542250 revChatGPT-6.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:01:53.546250 revChatGPT-6.8.1/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    62781 2023-07-09 06:01:21.000000 revChatGPT-6.8.1/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25069 2023-07-09 06:01:21.000000 revChatGPT-6.8.1/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-09 06:01:21.000000 revChatGPT-6.8.1/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-09 06:01:21.000000 revChatGPT-6.8.1/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:01:53.546250 revChatGPT-6.8.1/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-09 06:01:21.000000 revChatGPT-6.8.1/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-07-09 06:01:21.000000 revChatGPT-6.8.1/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-09 06:01:21.000000 revChatGPT-6.8.1/src/revChatGPT/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-09 06:01:21.000000 revChatGPT-6.8.1/src/revChatGPT/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:01:53.546250 revChatGPT-6.8.1/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-07-09 06:01:53.000000 revChatGPT-6.8.1/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-09 06:01:53.000000 revChatGPT-6.8.1/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 06:01:53.000000 revChatGPT-6.8.1/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-09 06:01:53.000000 revChatGPT-6.8.1/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-09 06:01:53.000000 revChatGPT-6.8.1/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:01:53.546250 revChatGPT-6.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-09 06:01:21.000000 revChatGPT-6.8.1/tests/test_recipient.py
```

### Comparing `revChatGPT-6.8.0/LICENSE` & `revChatGPT-6.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.8.0/PKG-INFO` & `revChatGPT-6.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.8.0
+Version: 6.8.1
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.8.0/README.md` & `revChatGPT-6.8.1/README.md`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.8.0/setup.py` & `revChatGPT-6.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.8.0/src/revChatGPT/V1.py` & `revChatGPT-6.8.1/src/revChatGPT/V1.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,33 +197,37 @@
         )
         if resp.status_code != 200:
             raise Exception("Failed to verify captcha")
         return resp_json.get("token")
     else:
         working_endpoints: list[str] = []
         # Check uptime for different endpoints via gatus
-        resp: list[dict] = requests.get(
+        resp2: list[dict] = requests.get(
             "https://stats.churchless.tech/api/v1/endpoints/statuses?page=1"
         ).json()
-        for endpoint in resp:
+        for endpoint in resp2:
+            # print(endpoint.get("name"))
             if endpoint.get("group") != "Arkose Labs":
                 continue
             # Check the last 5 results
-            results: list[dict] = endpoint.get("results", [])[:5]
+            results: list[dict] = endpoint.get("results", [])[-5:-1]
+            # print(results)
             if not results:
+                print(f"Endpoint {endpoint.get('name')} has no results")
                 continue
             # Check if all the results are up
             if all(result.get("success") == True for result in results):
                 working_endpoints.append(endpoint.get("name"))
         if not working_endpoints:
             print("No working endpoints found. Please solve the captcha manually.")
             return get_arkose_token(download_images=True, captcha_supported=True)
         # Choose a random endpoint
+        # print(working_endpoints)
         endpoint = random.choice(working_endpoints)
-        print(f"Using endpoint {endpoint} for captcha")
+        print(f"Using endpoint {endpoint} for captcha\n\n")
         resp: requests.Response = requests.get(endpoint)
         if resp.status_code != 200:
             if resp.status_code != 511:
                 raise Exception("Failed to get captcha token")
             else:
                 print("Captcha required. Please solve the captcha manually.")
                 return get_arkose_token(download_images=True, captcha_supported=True)
```

### Comparing `revChatGPT-6.8.0/src/revChatGPT/V3.py` & `revChatGPT-6.8.1/src/revChatGPT/V3.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.8.0/src/revChatGPT/__init__.py` & `revChatGPT-6.8.1/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.8.0/src/revChatGPT/__main__.py` & `revChatGPT-6.8.1/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.8.0/src/revChatGPT/config/enable_internet.json` & `revChatGPT-6.8.1/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.8.0/src/revChatGPT/typings.py` & `revChatGPT-6.8.1/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.8.0/src/revChatGPT/utils.py` & `revChatGPT-6.8.1/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.8.0/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-6.8.1/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.8.0
+Version: 6.8.1
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.8.0/tests/test_recipient.py` & `revChatGPT-6.8.1/tests/test_recipient.py`

 * *Files identical despite different names*

