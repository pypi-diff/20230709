# Comparing `tmp/tdir-1.5.0.tar.gz` & `tmp/tdir-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdir-1.5.0.tar", max compression
+gzip compressed data, was "tdir-1.6.0.tar", max compression
```

## Comparing `tdir-1.5.0.tar` & `tdir-1.6.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1067 2023-02-08 17:50:42.050848 tdir-1.5.0/LICENSE
--rw-r--r--   0        0        0     2791 2023-02-23 19:48:11.504186 tdir-1.5.0/README.md
--rw-r--r--   0        0        0      576 2023-02-23 19:57:31.574401 tdir-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     8045 2023-02-16 15:52:23.812084 tdir-1.5.0/tdir.py
--rw-r--r--   0        0        0     3478 1970-01-01 00:00:00.000000 tdir-1.5.0/setup.py
--rw-r--r--   0        0        0     3454 1970-01-01 00:00:00.000000 tdir-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-02-08 17:50:42.050848 tdir-1.6.0/LICENSE
+-rw-r--r--   0        0        0     2791 2023-02-23 19:48:11.504186 tdir-1.6.0/README.md
+-rw-r--r--   0        0        0      548 2023-07-09 14:51:09.520004 tdir-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     8045 2023-02-16 15:52:23.812084 tdir-1.6.0/tdir.py
+-rw-r--r--   0        0        0     3415 1970-01-01 00:00:00.000000 tdir-1.6.0/PKG-INFO
```

### Comparing `tdir-1.5.0/LICENSE` & `tdir-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tdir-1.5.0/README.md` & `tdir-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `tdir-1.5.0/pyproject.toml` & `tdir-1.6.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 target-version = ['py37']
 
 [tool.doks]
 auto = true
 
 [tool.poetry]
 name = "tdir"
-version = "1.5.0"
+version = "1.6.0"
 description = "🗃 Create and fill a temporary directory 🗃"
 authors = ["Tom Ritchford <tom@swirly.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.7"
-dek = "^1.0.2"
-xmod = "^1.3.2"
+python = ">=3.7"
+dek = "*"
+xmod = "*"
 
 [tool.poetry.group.dev.dependencies]
-coverage = "^6.5.0"
-doks = "^1.0.1"
-pytest = "^7.2.0"
-flake8 = "5.0.4"
+coverage = "*"
+doks = "*"
+pytest = "*"
+flake8 = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tdir-1.5.0/tdir.py` & `tdir-1.6.0/tdir.py`

 * *Files identical despite different names*

### Comparing `tdir-1.5.0/PKG-INFO` & `tdir-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: tdir
-Version: 1.5.0
+Version: 1.6.0
 Summary: 🗃 Create and fill a temporary directory 🗃
 License: MIT
 Author: Tom Ritchford
 Author-email: tom@swirly.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: dek (>=1.0.2,<2.0.0)
-Requires-Dist: xmod (>=1.3.2,<2.0.0)
+Requires-Dist: dek
+Requires-Dist: xmod
 Description-Content-Type: text/markdown
 
 # 🗃 tdir - create and fill a temporary directory 🗃
 
 Run code inside a temporary directory filled with zero or more files.
 
 Very convenient for writing tests: you can decorate individual tests or a whole
```

