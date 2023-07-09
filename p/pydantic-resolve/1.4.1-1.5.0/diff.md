# Comparing `tmp/pydantic_resolve-1.4.1.tar.gz` & `tmp/pydantic_resolve-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_resolve-1.4.1.tar", max compression
+gzip compressed data, was "pydantic_resolve-1.5.0.tar", max compression
```

## Comparing `pydantic_resolve-1.4.1.tar` & `pydantic_resolve-1.5.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-1.4.1/LICENSE
--rw-r--r--   0        0        0      587 2023-07-03 08:03:54.897877 pydantic_resolve-1.4.1/pydantic_resolve/__init__.py
--rw-r--r--   0        0        0      228 2023-07-09 02:37:13.250821 pydantic_resolve-1.4.1/pydantic_resolve/constant.py
--rw-r--r--   0        0        0     3552 2023-07-08 14:14:06.292603 pydantic_resolve-1.4.1/pydantic_resolve/core.py
--rw-r--r--   0        0        0      229 2023-06-01 01:21:44.326847 pydantic_resolve-1.4.1/pydantic_resolve/exceptions.py
--rw-r--r--   0        0        0     6512 2023-07-09 03:16:50.755677 pydantic_resolve-1.4.1/pydantic_resolve/resolver.py
--rw-r--r--   0        0        0     6158 2023-07-09 03:16:50.754667 pydantic_resolve-1.4.1/pydantic_resolve/util.py
--rw-r--r--   0        0        0      814 2023-07-06 14:14:21.541726 pydantic_resolve-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     7660 2023-07-04 04:23:48.147702 pydantic_resolve-1.4.1/README.md
--rw-r--r--   0        0        0     8235 1970-01-01 00:00:00.000000 pydantic_resolve-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-1.5.0/LICENSE
+-rw-r--r--   0        0        0      587 2023-07-03 08:03:54.897877 pydantic_resolve-1.5.0/pydantic_resolve/__init__.py
+-rw-r--r--   0        0        0      228 2023-07-09 02:37:13.250821 pydantic_resolve-1.5.0/pydantic_resolve/constant.py
+-rw-r--r--   0        0        0     3552 2023-07-08 14:14:06.292603 pydantic_resolve-1.5.0/pydantic_resolve/core.py
+-rw-r--r--   0        0        0      229 2023-06-01 01:21:44.326847 pydantic_resolve-1.5.0/pydantic_resolve/exceptions.py
+-rw-r--r--   0        0        0     6512 2023-07-09 03:16:50.755677 pydantic_resolve-1.5.0/pydantic_resolve/resolver.py
+-rw-r--r--   0        0        0     6158 2023-07-09 03:16:50.754667 pydantic_resolve-1.5.0/pydantic_resolve/util.py
+-rw-r--r--   0        0        0      814 2023-07-09 03:31:01.556305 pydantic_resolve-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7660 2023-07-04 04:23:48.147702 pydantic_resolve-1.5.0/README.md
+-rw-r--r--   0        0        0     8235 1970-01-01 00:00:00.000000 pydantic_resolve-1.5.0/PKG-INFO
```

### Comparing `pydantic_resolve-1.4.1/LICENSE` & `pydantic_resolve-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.4.1/pydantic_resolve/__init__.py` & `pydantic_resolve-1.5.0/pydantic_resolve/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.4.1/pydantic_resolve/core.py` & `pydantic_resolve-1.5.0/pydantic_resolve/core.py`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.4.1/pydantic_resolve/resolver.py` & `pydantic_resolve-1.5.0/pydantic_resolve/resolver.py`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.4.1/pydantic_resolve/util.py` & `pydantic_resolve-1.5.0/pydantic_resolve/util.py`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.4.1/pyproject.toml` & `pydantic_resolve-1.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-resolve"
-version = "1.4.1"
+version = "1.5.0"
 description = "Make pydantic have a GraphQL-like assembly experience."
 authors = ["tangkikodo <allmonday@126.com>"]
 readme = "README.md"
 repository = "https://github.com/allmonday/pydantic_resolve"
 keywords = ["pydantic", "fastapi"]
 license = "MIT"
 packages = [{include = "pydantic_resolve"}]
```

### Comparing `pydantic_resolve-1.4.1/README.md` & `pydantic_resolve-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.4.1/PKG-INFO` & `pydantic_resolve-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-resolve
-Version: 1.4.1
+Version: 1.5.0
 Summary: Make pydantic have a GraphQL-like assembly experience.
 Home-page: https://github.com/allmonday/pydantic_resolve
 License: MIT
 Keywords: pydantic,fastapi
 Author: tangkikodo
 Author-email: allmonday@126.com
 Requires-Python: >=3.7,<4.0
```

