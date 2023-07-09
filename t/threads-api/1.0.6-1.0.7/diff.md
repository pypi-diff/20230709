# Comparing `tmp/threads-api-1.0.6.tar.gz` & `tmp/threads-api-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threads-api-1.0.6.tar", last modified: Sun Jul  9 20:54:15 2023, max compression
+gzip compressed data, was "threads-api-1.0.7.tar", last modified: Sun Jul  9 21:01:32 2023, max compression
```

## Comparing `threads-api-1.0.6.tar` & `threads-api-1.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-09 20:54:15.300830 threads-api-1.0.6/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1068 2023-07-06 22:22:29.000000 threads-api-1.0.6/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    10074 2023-07-09 20:54:15.296830 threads-api-1.0.6/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     9548 2023-07-09 20:54:06.000000 threads-api-1.0.6/README.md
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      349 2023-07-06 21:24:15.000000 threads-api-1.0.6/pyproject.toml
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-09 20:54:15.300830 threads-api-1.0.6/setup.cfg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      785 2023-07-09 20:52:30.000000 threads-api-1.0.6/setup.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-09 20:54:15.296830 threads-api-1.0.6/threads_api/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 20:59:49.000000 threads-api-1.0.6/threads_api/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-09 20:54:15.296830 threads-api-1.0.6/threads_api/src/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:13:21.000000 threads-api-1.0.6/threads_api/src/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    18821 2023-07-09 20:45:43.000000 threads-api-1.0.6/threads_api/src/threads_api.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-09 20:54:15.296830 threads-api-1.0.6/threads_api/tests/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:19:18.000000 threads-api-1.0.6/threads_api/tests/__init__.py
--rwxrwxr-x   0 daniel    (1000) daniel    (1000)      404 2023-07-07 21:21:06.000000 threads-api-1.0.6/threads_api/tests/get_threads_test.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-09 20:54:15.296830 threads-api-1.0.6/threads_api.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    10074 2023-07-09 20:54:15.000000 threads-api-1.0.6/threads_api.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      366 2023-07-09 20:54:15.000000 threads-api-1.0.6/threads_api.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-09 20:54:15.000000 threads-api-1.0.6/threads_api.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       17 2023-07-09 20:54:15.000000 threads-api-1.0.6/threads_api.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       12 2023-07-09 20:54:15.000000 threads-api-1.0.6/threads_api.egg-info/top_level.txt
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-09 21:01:32.037741 threads-api-1.0.7/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1068 2023-07-06 22:22:29.000000 threads-api-1.0.7/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    10074 2023-07-09 21:01:32.037741 threads-api-1.0.7/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     9548 2023-07-09 20:54:06.000000 threads-api-1.0.7/README.md
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      349 2023-07-06 21:24:15.000000 threads-api-1.0.7/pyproject.toml
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-09 21:01:32.037741 threads-api-1.0.7/setup.cfg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      785 2023-07-09 21:01:29.000000 threads-api-1.0.7/setup.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-09 21:01:32.033741 threads-api-1.0.7/threads_api/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 20:59:49.000000 threads-api-1.0.7/threads_api/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-09 21:01:32.037741 threads-api-1.0.7/threads_api/src/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:13:21.000000 threads-api-1.0.7/threads_api/src/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    18797 2023-07-09 21:00:53.000000 threads-api-1.0.7/threads_api/src/threads_api.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-09 21:01:32.037741 threads-api-1.0.7/threads_api/tests/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:19:18.000000 threads-api-1.0.7/threads_api/tests/__init__.py
+-rwxrwxr-x   0 daniel    (1000) daniel    (1000)      404 2023-07-07 21:21:06.000000 threads-api-1.0.7/threads_api/tests/get_threads_test.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-09 21:01:32.037741 threads-api-1.0.7/threads_api.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    10074 2023-07-09 21:01:32.000000 threads-api-1.0.7/threads_api.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      366 2023-07-09 21:01:32.000000 threads-api-1.0.7/threads_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-09 21:01:32.000000 threads-api-1.0.7/threads_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       17 2023-07-09 21:01:32.000000 threads-api-1.0.7/threads_api.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       12 2023-07-09 21:01:32.000000 threads-api-1.0.7/threads_api.egg-info/top_level.txt
```

### Comparing `threads-api-1.0.6/LICENSE` & `threads-api-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `threads-api-1.0.6/PKG-INFO` & `threads-api-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threads-api
-Version: 1.0.6
+Version: 1.0.7
 Summary: Unofficial Python client for Meta Threads API
 Home-page: https://github.com/danie1/threads-api
 Author: Danie1
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `threads-api-1.0.6/README.md` & `threads-api-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `threads-api-1.0.6/setup.py` & `threads-api-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='threads-api',
-    version='1.0.6',
+    version='1.0.7',
     description='Unofficial Python client for Meta Threads API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Danie1',
     author_email='',
     url='https://github.com/danie1/threads-api',
     packages=find_packages(),
```

### Comparing `threads-api-1.0.6/threads_api/src/threads_api.py` & `threads-api-1.0.7/threads_api/src/threads_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,14 @@
             LOGIN_URL = "https://i.instagram.com/api/v1/bloks/apps/com.bloks.www.bloks.caa.login.async.send_login_request/"
             payload = f"params={urllib.parse.quote(params)}&bk_client_context={urllib.parse.quote(bk_client_context)}&bloks_versioning_id={blockVersion}"
             
             async with aiohttp.ClientSession() as session:
                 async with session.post(LOGIN_URL, timeout=60 * 1000, headers=headers, data=payload) as response:
                     data = await response.text()
             
-            print(data)
             if data == "Oops, an error occurred.":
                 raise Exception("Failed to login")
             
             pos = data.split("Bearer IGT:2:")
 
             if len(pos) > 1:
                 pos = pos[1]
```

### Comparing `threads-api-1.0.6/threads_api.egg-info/PKG-INFO` & `threads-api-1.0.7/threads_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threads-api
-Version: 1.0.6
+Version: 1.0.7
 Summary: Unofficial Python client for Meta Threads API
 Home-page: https://github.com/danie1/threads-api
 Author: Danie1
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

