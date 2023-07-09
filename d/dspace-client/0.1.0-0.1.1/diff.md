# Comparing `tmp/dspace_client-0.1.0.tar.gz` & `tmp/dspace_client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dspace_client-0.1.0.tar", max compression
+gzip compressed data, was "dspace_client-0.1.1.tar", max compression
```

## Comparing `dspace_client-0.1.0.tar` & `dspace_client-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       84 2023-07-08 00:42:17.474123 dspace_client-0.1.0/dspace/__init__.py
--rw-r--r--   0        0        0     3358 2023-07-08 20:50:03.728160 dspace_client-0.1.0/dspace/dspace_client.py
--rw-r--r--   0        0        0     1539 2023-07-08 20:42:51.878462 dspace_client-0.1.0/dspace/dspace_objects.py
--rw-r--r--   0        0        0     1083 2023-07-08 00:38:07.760248 dspace_client-0.1.0/LICENSE
--rw-r--r--   0        0        0      418 2023-07-09 15:03:15.312468 dspace_client-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      362 2023-07-09 15:01:10.496019 dspace_client-0.1.0/README.md
--rw-r--r--   0        0        0      798 1970-01-01 00:00:00.000000 dspace_client-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       84 2023-07-08 00:42:17.474123 dspace_client-0.1.1/dspace/__init__.py
+-rw-r--r--   0        0        0     3358 2023-07-08 20:50:03.728160 dspace_client-0.1.1/dspace/dspace_client.py
+-rw-r--r--   0        0        0     1539 2023-07-09 18:59:49.776291 dspace_client-0.1.1/dspace/dspace_objects.py
+-rw-r--r--   0        0        0     1083 2023-07-08 00:38:07.760248 dspace_client-0.1.1/LICENSE
+-rw-r--r--   0        0        0      529 2023-07-09 19:22:59.004524 dspace_client-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      613 2023-07-09 19:23:53.495092 dspace_client-0.1.1/README.md
+-rw-r--r--   0        0        0     1251 1970-01-01 00:00:00.000000 dspace_client-0.1.1/PKG-INFO
```

### Comparing `dspace_client-0.1.0/dspace/dspace_client.py` & `dspace_client-0.1.1/dspace/dspace_client.py`

 * *Files identical despite different names*

### Comparing `dspace_client-0.1.0/dspace/dspace_objects.py` & `dspace_client-0.1.1/dspace/dspace_objects.py`

 * *Files identical despite different names*

### Comparing `dspace_client-0.1.0/LICENSE` & `dspace_client-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dspace_client-0.1.0/PKG-INFO` & `dspace_client-0.1.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,47 @@
 Metadata-Version: 2.1
 Name: dspace-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: DSpace Rest Client for Python
+Home-page: https://github.com/vitorsilverio/dspace-client
+License: MIT
+Keywords: dspace,rest
 Author: Vítor
 Author-email: vitor.silverio.rodrigues@gmail.com
 Requires-Python: >=3.11,<4.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: pydantic (>=2.0.2,<3.0.0)
 Requires-Dist: pyjwt (>=2.6.0,<3.0.0)
+Project-URL: Repository, https://github.com/vitorsilverio/dspace-client
 Description-Content-Type: text/markdown
 
 DSpace rest client for v7 or above
 =====================================
 
+## Using
+```
+pip install dspace-client
+```
+on code:
+```python
+from dspace import DSpaceClient
+
+client = DSpaceClient("https://api7.dspace.org/server/")
+client.login("dspacedemo+admin@gmail.com", "dspace")
+print(client.get_items())
+```
+
 ## Goals
 - [ ] Implement all endpoints on DSpace Rest Contract
 - [ ] Configurable by default
 - [ ] All authentication methods
 - [ ] Async support
 
 ## Features
 - Authenticaion using login/password
 - Autorefresh token
 - Auto XSRF token
 - Objects are pydantic friendly not dicts
+
```

