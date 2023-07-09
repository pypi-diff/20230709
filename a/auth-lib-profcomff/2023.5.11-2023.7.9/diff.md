# Comparing `tmp/auth_lib_profcomff-2023.5.11.tar.gz` & `tmp/auth_lib_profcomff-2023.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auth_lib_profcomff-2023.5.11.tar", last modified: Wed May 10 23:53:57 2023, max compression
+gzip compressed data, was "auth_lib_profcomff-2023.7.9.tar", last modified: Sun Jul  9 05:51:26 2023, max compression
```

## Comparing `auth_lib_profcomff-2023.5.11.tar` & `auth_lib_profcomff-2023.7.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:53:57.294563 auth_lib_profcomff-2023.5.11/
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-10 23:53:46.000000 auth_lib_profcomff-2023.5.11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-05-10 23:53:57.294563 auth_lib_profcomff-2023.5.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-05-10 23:53:46.000000 auth_lib_profcomff-2023.5.11/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:53:57.294563 auth_lib_profcomff-2023.5.11/auth_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 23:53:46.000000 auth_lib_profcomff-2023.5.11/auth_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-10 23:53:46.000000 auth_lib_profcomff-2023.5.11/auth_lib/aiomethods.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-10 23:53:46.000000 auth_lib_profcomff-2023.5.11/auth_lib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-10 23:53:46.000000 auth_lib_profcomff-2023.5.11/auth_lib/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-10 23:53:46.000000 auth_lib_profcomff-2023.5.11/auth_lib/methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:53:57.294563 auth_lib_profcomff-2023.5.11/auth_lib/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-10 23:53:46.000000 auth_lib_profcomff-2023.5.11/auth_lib/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-10 23:53:46.000000 auth_lib_profcomff-2023.5.11/auth_lib/testing/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:53:57.294563 auth_lib_profcomff-2023.5.11/auth_lib_profcomff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-05-10 23:53:57.000000 auth_lib_profcomff-2023.5.11/auth_lib_profcomff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-10 23:53:57.000000 auth_lib_profcomff-2023.5.11/auth_lib_profcomff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 23:53:57.000000 auth_lib_profcomff-2023.5.11/auth_lib_profcomff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-10 23:53:57.000000 auth_lib_profcomff-2023.5.11/auth_lib_profcomff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-10 23:53:57.000000 auth_lib_profcomff-2023.5.11/auth_lib_profcomff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-10 23:53:57.000000 auth_lib_profcomff-2023.5.11/auth_lib_profcomff.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 23:53:57.294563 auth_lib_profcomff-2023.5.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-10 23:53:46.000000 auth_lib_profcomff-2023.5.11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 05:51:26.015044 auth_lib_profcomff-2023.7.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-09 05:51:13.000000 auth_lib_profcomff-2023.7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-07-09 05:51:26.015044 auth_lib_profcomff-2023.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-07-09 05:51:13.000000 auth_lib_profcomff-2023.7.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 05:51:26.015044 auth_lib_profcomff-2023.7.9/auth_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 05:51:13.000000 auth_lib_profcomff-2023.7.9/auth_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-09 05:51:13.000000 auth_lib_profcomff-2023.7.9/auth_lib/aiomethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-09 05:51:13.000000 auth_lib_profcomff-2023.7.9/auth_lib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-09 05:51:13.000000 auth_lib_profcomff-2023.7.9/auth_lib/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-09 05:51:13.000000 auth_lib_profcomff-2023.7.9/auth_lib/methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 05:51:26.015044 auth_lib_profcomff-2023.7.9/auth_lib/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-09 05:51:13.000000 auth_lib_profcomff-2023.7.9/auth_lib/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-09 05:51:13.000000 auth_lib_profcomff-2023.7.9/auth_lib/testing/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 05:51:26.015044 auth_lib_profcomff-2023.7.9/auth_lib_profcomff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-07-09 05:51:26.000000 auth_lib_profcomff-2023.7.9/auth_lib_profcomff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-09 05:51:26.000000 auth_lib_profcomff-2023.7.9/auth_lib_profcomff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 05:51:26.000000 auth_lib_profcomff-2023.7.9/auth_lib_profcomff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-09 05:51:26.000000 auth_lib_profcomff-2023.7.9/auth_lib_profcomff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-09 05:51:26.000000 auth_lib_profcomff-2023.7.9/auth_lib_profcomff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-09 05:51:26.000000 auth_lib_profcomff-2023.7.9/auth_lib_profcomff.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 05:51:26.015044 auth_lib_profcomff-2023.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-09 05:51:13.000000 auth_lib_profcomff-2023.7.9/setup.py
```

### Comparing `auth_lib_profcomff-2023.5.11/LICENSE` & `auth_lib_profcomff-2023.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2023.5.11/PKG-INFO` & `auth_lib_profcomff-2023.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auth_lib_profcomff
-Version: 2023.5.11
+Version: 2023.7.9
 Home-page: https://github.com/profcomff/auth-lib
 Author: Semyon Grigoriev
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: fastapi
 Provides-Extra: testing
 License-File: LICENSE
```

### Comparing `auth_lib_profcomff-2023.5.11/README.md` & `auth_lib_profcomff-2023.7.9/README.md`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2023.5.11/auth_lib/aiomethods.py` & `auth_lib_profcomff-2023.7.9/auth_lib/aiomethods.py`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2023.5.11/auth_lib/exceptions.py` & `auth_lib_profcomff-2023.7.9/auth_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2023.5.11/auth_lib/fastapi.py` & `auth_lib_profcomff-2023.7.9/auth_lib/fastapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 from typing import Any
 from warnings import warn
 
 from fastapi.exceptions import HTTPException
 from fastapi.openapi.models import APIKey, APIKeyIn
 from fastapi.security.base import SecurityBase
-from pydantic import BaseSettings
+from pydantic import ConfigDict
+from pydantic_settings import BaseSettings
 from starlette.requests import Request
 from starlette.status import HTTP_403_FORBIDDEN
 
 from auth_lib.aiomethods import AsyncAuthLib
 
 
 class UnionAuthSettings(BaseSettings):
     AUTH_URL: str = "https://api.test.profcomff.com/auth/"
     AUTH_AUTO_ERROR: bool = True
     AUTH_ALLOW_NONE: bool = False
-
-    class Config:
-        """Pydantic BaseSettings config"""
-
-        case_sensitive = True
-        env_file = ".env"
+    model_config = ConfigDict(case_sensitive=True, env_file=".env", extra="allow")
 
 
 class UnionAuth(SecurityBase):
     model = APIKey.construct(in_=APIKeyIn.header, name="Authorization")
     scheme_name = "token"
     settings = UnionAuthSettings()
```

### Comparing `auth_lib_profcomff-2023.5.11/auth_lib/methods.py` & `auth_lib_profcomff-2023.7.9/auth_lib/methods.py`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2023.5.11/auth_lib/testing/testutils.py` & `auth_lib_profcomff-2023.7.9/auth_lib/testing/testutils.py`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2023.5.11/auth_lib_profcomff.egg-info/PKG-INFO` & `auth_lib_profcomff-2023.7.9/auth_lib_profcomff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auth-lib-profcomff
-Version: 2023.5.11
+Version: 2023.7.9
 Home-page: https://github.com/profcomff/auth-lib
 Author: Semyon Grigoriev
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: fastapi
 Provides-Extra: testing
 License-File: LICENSE
```

### Comparing `auth_lib_profcomff-2023.5.11/setup.py` & `auth_lib_profcomff-2023.7.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 setup(
     name="auth_lib_profcomff",
-    version="2023.05.11",
+    version="2023.07.09",
     author="Semyon Grigoriev",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/profcomff/auth-lib",
     packages=find_packages(),
     install_requires=["requests", "aiohttp", "setuptools"],
     extras_require={
-        "fastapi": ["fastapi", "starlette", "pydantic"],
+        "fastapi": ["fastapi", "starlette", "pydantic", "pydantic_settings"],
         "testing": ["pytest"],
     },
     entry_points={"pytest11": ["pytest_auth_lib = auth_lib.testing"]},
     classifiers=[
         "Programming Language :: Python :: 3.11",
     ],
 )
```

