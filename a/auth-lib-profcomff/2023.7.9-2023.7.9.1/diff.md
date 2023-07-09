# Comparing `tmp/auth_lib_profcomff-2023.7.9.tar.gz` & `tmp/auth_lib_profcomff-2023.7.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auth_lib_profcomff-2023.7.9.tar", last modified: Sun Jul  9 05:51:26 2023, max compression
+gzip compressed data, was "auth_lib_profcomff-2023.7.9.1.tar", last modified: Sun Jul  9 06:03:52 2023, max compression
```

## Comparing `auth_lib_profcomff-2023.7.9.tar` & `auth_lib_profcomff-2023.7.9.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 05:51:26.015044 auth_lib_profcomff-2023.7.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-09 05:51:13.000000 auth_lib_profcomff-2023.7.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-07-09 05:51:26.015044 auth_lib_profcomff-2023.7.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-07-09 05:51:13.000000 auth_lib_profcomff-2023.7.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 05:51:26.015044 auth_lib_profcomff-2023.7.9/auth_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 05:51:13.000000 auth_lib_profcomff-2023.7.9/auth_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-09 05:51:13.000000 auth_lib_profcomff-2023.7.9/auth_lib/aiomethods.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-09 05:51:13.000000 auth_lib_profcomff-2023.7.9/auth_lib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-09 05:51:13.000000 auth_lib_profcomff-2023.7.9/auth_lib/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-09 05:51:13.000000 auth_lib_profcomff-2023.7.9/auth_lib/methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 05:51:26.015044 auth_lib_profcomff-2023.7.9/auth_lib/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-09 05:51:13.000000 auth_lib_profcomff-2023.7.9/auth_lib/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-09 05:51:13.000000 auth_lib_profcomff-2023.7.9/auth_lib/testing/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 05:51:26.015044 auth_lib_profcomff-2023.7.9/auth_lib_profcomff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-07-09 05:51:26.000000 auth_lib_profcomff-2023.7.9/auth_lib_profcomff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-09 05:51:26.000000 auth_lib_profcomff-2023.7.9/auth_lib_profcomff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 05:51:26.000000 auth_lib_profcomff-2023.7.9/auth_lib_profcomff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-09 05:51:26.000000 auth_lib_profcomff-2023.7.9/auth_lib_profcomff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-09 05:51:26.000000 auth_lib_profcomff-2023.7.9/auth_lib_profcomff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-09 05:51:26.000000 auth_lib_profcomff-2023.7.9/auth_lib_profcomff.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 05:51:26.015044 auth_lib_profcomff-2023.7.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-09 05:51:13.000000 auth_lib_profcomff-2023.7.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:03:52.776368 auth_lib_profcomff-2023.7.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-09 06:03:41.000000 auth_lib_profcomff-2023.7.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-07-09 06:03:52.776368 auth_lib_profcomff-2023.7.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-07-09 06:03:41.000000 auth_lib_profcomff-2023.7.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:03:52.776368 auth_lib_profcomff-2023.7.9.1/auth_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 06:03:41.000000 auth_lib_profcomff-2023.7.9.1/auth_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-09 06:03:41.000000 auth_lib_profcomff-2023.7.9.1/auth_lib/aiomethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-09 06:03:41.000000 auth_lib_profcomff-2023.7.9.1/auth_lib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-07-09 06:03:41.000000 auth_lib_profcomff-2023.7.9.1/auth_lib/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-09 06:03:41.000000 auth_lib_profcomff-2023.7.9.1/auth_lib/methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:03:52.776368 auth_lib_profcomff-2023.7.9.1/auth_lib/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-09 06:03:41.000000 auth_lib_profcomff-2023.7.9.1/auth_lib/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-09 06:03:41.000000 auth_lib_profcomff-2023.7.9.1/auth_lib/testing/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:03:52.776368 auth_lib_profcomff-2023.7.9.1/auth_lib_profcomff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-07-09 06:03:52.000000 auth_lib_profcomff-2023.7.9.1/auth_lib_profcomff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-09 06:03:52.000000 auth_lib_profcomff-2023.7.9.1/auth_lib_profcomff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 06:03:52.000000 auth_lib_profcomff-2023.7.9.1/auth_lib_profcomff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-09 06:03:52.000000 auth_lib_profcomff-2023.7.9.1/auth_lib_profcomff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-09 06:03:52.000000 auth_lib_profcomff-2023.7.9.1/auth_lib_profcomff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-09 06:03:52.000000 auth_lib_profcomff-2023.7.9.1/auth_lib_profcomff.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 06:03:52.776368 auth_lib_profcomff-2023.7.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-09 06:03:41.000000 auth_lib_profcomff-2023.7.9.1/setup.py
```

### Comparing `auth_lib_profcomff-2023.7.9/LICENSE` & `auth_lib_profcomff-2023.7.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2023.7.9/PKG-INFO` & `auth_lib_profcomff-2023.7.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auth_lib_profcomff
-Version: 2023.7.9
+Version: 2023.7.9.1
 Home-page: https://github.com/profcomff/auth-lib
 Author: Semyon Grigoriev
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: fastapi
 Provides-Extra: testing
 License-File: LICENSE
```

### Comparing `auth_lib_profcomff-2023.7.9/README.md` & `auth_lib_profcomff-2023.7.9.1/README.md`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2023.7.9/auth_lib/aiomethods.py` & `auth_lib_profcomff-2023.7.9.1/auth_lib/aiomethods.py`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2023.7.9/auth_lib/exceptions.py` & `auth_lib_profcomff-2023.7.9.1/auth_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2023.7.9/auth_lib/fastapi.py` & `auth_lib_profcomff-2023.7.9.1/auth_lib/fastapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from auth_lib.aiomethods import AsyncAuthLib
 
 
 class UnionAuthSettings(BaseSettings):
     AUTH_URL: str = "https://api.test.profcomff.com/auth/"
     AUTH_AUTO_ERROR: bool = True
     AUTH_ALLOW_NONE: bool = False
-    model_config = ConfigDict(case_sensitive=True, env_file=".env", extra="allow")
+    model_config = ConfigDict(case_sensitive=True, env_file=".env", extra="ignore")
 
 
 class UnionAuth(SecurityBase):
     model = APIKey.construct(in_=APIKeyIn.header, name="Authorization")
     scheme_name = "token"
     settings = UnionAuthSettings()
```

### Comparing `auth_lib_profcomff-2023.7.9/auth_lib/methods.py` & `auth_lib_profcomff-2023.7.9.1/auth_lib/methods.py`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2023.7.9/auth_lib/testing/testutils.py` & `auth_lib_profcomff-2023.7.9.1/auth_lib/testing/testutils.py`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2023.7.9/auth_lib_profcomff.egg-info/PKG-INFO` & `auth_lib_profcomff-2023.7.9.1/auth_lib_profcomff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auth-lib-profcomff
-Version: 2023.7.9
+Version: 2023.7.9.1
 Home-page: https://github.com/profcomff/auth-lib
 Author: Semyon Grigoriev
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: fastapi
 Provides-Extra: testing
 License-File: LICENSE
```

### Comparing `auth_lib_profcomff-2023.7.9/setup.py` & `auth_lib_profcomff-2023.7.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 setup(
     name="auth_lib_profcomff",
-    version="2023.07.09",
+    version="2023.07.09.1",
     author="Semyon Grigoriev",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/profcomff/auth-lib",
     packages=find_packages(),
     install_requires=["requests", "aiohttp", "setuptools"],
     extras_require={
```

