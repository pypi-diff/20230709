# Comparing `tmp/saladpy-1.0.2a2.tar.gz` & `tmp/saladpy-1.0.2a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saladpy-1.0.2a2.tar", last modified: Tue Jun 27 13:11:16 2023, max compression
+gzip compressed data, was "saladpy-1.0.2a3.tar", last modified: Sun Jul  9 13:15:52 2023, max compression
```

## Comparing `saladpy-1.0.2a2.tar` & `saladpy-1.0.2a3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:11:16.932517 saladpy-1.0.2a2/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-27 13:11:05.000000 saladpy-1.0.2a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-27 13:11:05.000000 saladpy-1.0.2a2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-06-27 13:11:16.932517 saladpy-1.0.2a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-27 13:11:05.000000 saladpy-1.0.2a2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-27 13:11:05.000000 saladpy-1.0.2a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-27 13:11:05.000000 saladpy-1.0.2a2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:11:16.932517 saladpy-1.0.2a2/saladpy/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-27 13:11:05.000000 saladpy-1.0.2a2/saladpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-06-27 13:11:05.000000 saladpy-1.0.2a2/saladpy/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-27 13:11:05.000000 saladpy-1.0.2a2/saladpy/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:11:16.932517 saladpy-1.0.2a2/saladpy/methods/
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-06-27 13:11:05.000000 saladpy-1.0.2a2/saladpy/methods/User.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-27 13:11:05.000000 saladpy-1.0.2a2/saladpy/methods/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:11:16.932517 saladpy-1.0.2a2/saladpy/methods/types/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-27 13:11:05.000000 saladpy-1.0.2a2/saladpy/methods/types/BaseClient.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-27 13:11:05.000000 saladpy-1.0.2a2/saladpy/methods/types/UserTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-27 13:11:05.000000 saladpy-1.0.2a2/saladpy/methods/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:11:16.932517 saladpy-1.0.2a2/saladpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-06-27 13:11:16.000000 saladpy-1.0.2a2/saladpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-27 13:11:16.000000 saladpy-1.0.2a2/saladpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:11:16.000000 saladpy-1.0.2a2/saladpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 13:11:16.000000 saladpy-1.0.2a2/saladpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 13:11:16.000000 saladpy-1.0.2a2/saladpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 13:11:16.932517 saladpy-1.0.2a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-27 13:11:05.000000 saladpy-1.0.2a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:15:52.253825 saladpy-1.0.2a3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-09 13:15:40.000000 saladpy-1.0.2a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-09 13:15:40.000000 saladpy-1.0.2a3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-09 13:15:52.253825 saladpy-1.0.2a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-09 13:15:40.000000 saladpy-1.0.2a3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-09 13:15:40.000000 saladpy-1.0.2a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-09 13:15:40.000000 saladpy-1.0.2a3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:15:52.249825 saladpy-1.0.2a3/saladpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-09 13:15:40.000000 saladpy-1.0.2a3/saladpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-07-09 13:15:40.000000 saladpy-1.0.2a3/saladpy/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-09 13:15:40.000000 saladpy-1.0.2a3/saladpy/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:15:52.249825 saladpy-1.0.2a3/saladpy/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-07-09 13:15:40.000000 saladpy-1.0.2a3/saladpy/methods/User.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-09 13:15:40.000000 saladpy-1.0.2a3/saladpy/methods/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:15:52.253825 saladpy-1.0.2a3/saladpy/methods/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-09 13:15:40.000000 saladpy-1.0.2a3/saladpy/methods/types/BaseClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-09 13:15:40.000000 saladpy-1.0.2a3/saladpy/methods/types/UserTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-09 13:15:40.000000 saladpy-1.0.2a3/saladpy/methods/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:15:52.249825 saladpy-1.0.2a3/saladpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-09 13:15:52.000000 saladpy-1.0.2a3/saladpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-09 13:15:52.000000 saladpy-1.0.2a3/saladpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 13:15:52.000000 saladpy-1.0.2a3/saladpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-09 13:15:52.000000 saladpy-1.0.2a3/saladpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-09 13:15:52.000000 saladpy-1.0.2a3/saladpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 13:15:52.253825 saladpy-1.0.2a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-09 13:15:40.000000 saladpy-1.0.2a3/setup.py
```

### Comparing `saladpy-1.0.2a2/LICENSE` & `saladpy-1.0.2a3/LICENSE`

 * *Files identical despite different names*

### Comparing `saladpy-1.0.2a2/PKG-INFO` & `saladpy-1.0.2a3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saladpy
-Version: 1.0.2a2
+Version: 1.0.2a3
 Summary: A Python wrapper for the Salad Web API
 Home-page: https://github.com/Coddo-Python/SaladPy
 Author: Coddo-Python
 Author-email: Coddo <coddobusiness@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2015-present Coddo-Python
@@ -80,12 +80,12 @@
     await client.close()
 
 asyncio.run(main())
 ```
 
 Docs
 --------------
-Docs are available at <https://saladpy.gitbook.io/saladpy-docs/>. 
+The docs are available at <https://saladpy.gitbook.io/saladpy-docs/>.
 
 Contact
 --------------
 You can contact me at `Coddo#3210` on Discord! Ensure to first send me a friend request.
```

### Comparing `saladpy-1.0.2a2/README.md` & `saladpy-1.0.2a3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -43,12 +43,12 @@
     await client.close()
 
 asyncio.run(main())
 ```
 
 Docs
 --------------
-Docs are available at <https://saladpy.gitbook.io/saladpy-docs/>. 
+The docs are available at <https://saladpy.gitbook.io/saladpy-docs/>.
 
 Contact
 --------------
 You can contact me at `Coddo#3210` on Discord! Ensure to first send me a friend request.
```

### Comparing `saladpy-1.0.2a2/pyproject.toml` & `saladpy-1.0.2a3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "saladpy"
-version = "1.0.2-a.2"
+version = "1.0.2-a.3"
 description = "A Python wrapper for the Salad Web API"
 readme = "README.md"
 authors = [{ name = "Coddo", email = "coddobusiness@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `saladpy-1.0.2a2/saladpy/client.py` & `saladpy-1.0.2a3/saladpy/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,32 +6,39 @@
 from types import SimpleNamespace
 
 from .exceptions import *
 from .methods import Methods
 
 
 class SaladClient(Methods):
+    """The main client allowing you to use the rest of the library.
+    
+    NOTE: If using `token`, do not call login or verify
+    """
     V1_API_URL = "https://app-api.salad.com/api/v1/"
     V2_API_URL = "https://app-api.salad.com/api/v2/"
     AUTH_API_URL = "https://app-api.salad.com/auth/"
 
     def __init__(
         self,
         cachePath: Optional[Path] = None,
+        token: Optional[str] = None,
         *args,
         **kwargs,
     ):
         self.cachePath = cachePath
         self.cached = False
+        self.token = token
         self.http = ClientSession(*args, **kwargs)
-        if self.cachePath is not None:
-            if self.cachePath.exists():
-                if self.cachePath.stat().st_size > 0:  # File is not empty
-                    self.http.cookie_jar.load(self.cachePath)
-                    self.cached = True
+        if not token:
+            if self.cachePath is not None:
+                if self.cachePath.exists():
+                    if self.cachePath.stat().st_size > 0:  # File is not empty
+                        self.http.cookie_jar.load(self.cachePath)
+                        self.cached = True
                     
     @property
     def cookies(self):
         return {cookie.key: cookie.value for cookie in list(self.http.cookie_jar) }
                             
     async def close(self):
         """
@@ -108,16 +115,19 @@
                     raise SaladPyException(
                         f"Error {r.status} during OTP verification! {text}"
                     )
                 else:
                     return True
 
     async def _req(self, api_url : str, method: str, endpoint: str, params: Optional[dict] = None):
+        headers = {}
+        if self.token:
+            headers["Authorization"] = f"Bearer {self.token}"
         async with self.http.request(
-            method, f"{api_url}{endpoint}", params=params
+            method, f"{api_url}{endpoint}", params=params, headers=headers
         ) as r:
             text = await r.text()
             try:
                 assert r.status == 200
             except AssertionError:
                 if (
                     "try refresh token" in text
```

### Comparing `saladpy-1.0.2a2/saladpy/methods/User.py` & `saladpy-1.0.2a3/saladpy/methods/User.py`

 * *Files identical despite different names*

### Comparing `saladpy-1.0.2a2/saladpy/methods/types/BaseClient.py` & `saladpy-1.0.2a3/saladpy/methods/types/BaseClient.py`

 * *Files identical despite different names*

### Comparing `saladpy-1.0.2a2/saladpy/methods/types/UserTypes.py` & `saladpy-1.0.2a3/saladpy/methods/types/UserTypes.py`

 * *Files identical despite different names*

### Comparing `saladpy-1.0.2a2/saladpy.egg-info/PKG-INFO` & `saladpy-1.0.2a3/saladpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saladpy
-Version: 1.0.2a2
+Version: 1.0.2a3
 Summary: A Python wrapper for the Salad Web API
 Home-page: https://github.com/Coddo-Python/SaladPy
 Author: Coddo-Python
 Author-email: Coddo <coddobusiness@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2015-present Coddo-Python
@@ -80,12 +80,12 @@
     await client.close()
 
 asyncio.run(main())
 ```
 
 Docs
 --------------
-Docs are available at <https://saladpy.gitbook.io/saladpy-docs/>. 
+The docs are available at <https://saladpy.gitbook.io/saladpy-docs/>.
 
 Contact
 --------------
 You can contact me at `Coddo#3210` on Discord! Ensure to first send me a friend request.
```

### Comparing `saladpy-1.0.2a2/setup.py` & `saladpy-1.0.2a3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     author='Coddo-Python',
     url='https://github.com/Coddo-Python/SaladPy',
     project_urls={
         'Github': 'https://github.com/Coddo-Python/SaladPy',
         'Issue tracker': 'https://github.com/Coddo-Python/SaladPy/issues',
         'Docs': 'https://saladpy.gitbook.io/saladpy-docs/'
     },
-    version="1.0.2-a.2",
+    version="1.0.2-a.3",
     license='MIT',
     description='A Python wrapper for the Salad Web API',
     long_description=readme,
     packages=["saladpy", "saladpy.methods", "saladpy.methods.types"],
     install_requires=requirements,
     python_requires='>=3.8.0',
     classifiers=[
```

