# Comparing `tmp/gable-0.0.1a1.tar.gz` & `tmp/gable-0.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gable-0.0.1a1.tar", max compression
+gzip compressed data, was "gable-0.0.1a2.tar", max compression
```

## Comparing `gable-0.0.1a1.tar` & `gable-0.0.1a2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-06-13 23:27:44.590688 gable-0.0.1a1/gable/__init__.py
--rw-r--r--   0        0        0       53 2023-07-09 16:45:03.358691 gable-0.0.1a1/gable/cli.py
--rw-r--r--   0        0        0      652 2023-07-09 16:46:39.761746 gable-0.0.1a1/pyproject.toml
--rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 gable-0.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-13 23:27:44.590688 gable-0.0.1a2/gable/__init__.py
+-rw-r--r--   0        0        0       76 2023-07-09 16:59:25.836461 gable-0.0.1a2/gable/cli.py
+-rw-r--r--   0        0        0      652 2023-07-09 16:59:48.589676 gable-0.0.1a2/pyproject.toml
+-rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 gable-0.0.1a2/PKG-INFO
```

### Comparing `gable-0.0.1a1/pyproject.toml` & `gable-0.0.1a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gable"
-version = "0.0.1a1"
+version = "0.0.1a2"
 description = "Command line interface to interact with Gable API"
 authors = ["Gable.ai <engineers@gable.ai>"]
 packages = [{include = "gable"}]
 
 [tool.poetry.dependencies]
 python = ">=3.0.0,<4.0.0"
```

### Comparing `gable-0.0.1a1/PKG-INFO` & `gable-0.0.1a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gable
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: Command line interface to interact with Gable API
 Author: Gable.ai
 Author-email: engineers@gable.ai
 Requires-Python: >=3.0.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

