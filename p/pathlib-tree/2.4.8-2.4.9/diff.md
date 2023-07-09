# Comparing `tmp/pathlib_tree-2.4.8.tar.gz` & `tmp/pathlib_tree-2.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathlib_tree-2.4.8.tar", max compression
+gzip compressed data, was "pathlib_tree-2.4.9.tar", max compression
```

## Comparing `pathlib_tree-2.4.8.tar` & `pathlib_tree-2.4.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1497 2023-03-06 18:55:05.441919 pathlib_tree-2.4.8/LICENSE
--rw-r--r--   0        0        0      383 2022-07-27 08:37:18.406855 pathlib_tree-2.4.8/README.md
--rw-r--r--   0        0        0      200 2023-03-06 19:00:51.589527 pathlib_tree-2.4.8/pathlib_tree/__init__.py
--rw-r--r--   0        0        0      244 2023-03-06 18:59:10.884845 pathlib_tree-2.4.8/pathlib_tree/exceptions.py
--rw-r--r--   0        0        0     1878 2023-03-06 19:03:36.669688 pathlib_tree-2.4.8/pathlib_tree/patterns.py
--rw-r--r--   0        0        0    15899 2023-03-07 05:49:00.780935 pathlib_tree-2.4.8/pathlib_tree/tree.py
--rw-r--r--   0        0        0      287 2023-03-06 19:22:45.463908 pathlib_tree-2.4.8/pathlib_tree/utils.py
--rw-r--r--   0        0        0     1039 2023-03-07 06:15:47.930268 pathlib_tree-2.4.8/pyproject.toml
--rw-r--r--   0        0        0     1394 1970-01-01 00:00:00.000000 pathlib_tree-2.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1497 2023-03-06 18:55:05.441919 pathlib_tree-2.4.9/LICENSE
+-rw-r--r--   0        0        0      383 2022-07-27 08:37:18.406855 pathlib_tree-2.4.9/README.md
+-rw-r--r--   0        0        0      200 2023-03-06 19:00:51.589527 pathlib_tree-2.4.9/pathlib_tree/__init__.py
+-rw-r--r--   0        0        0      244 2023-03-06 18:59:10.884845 pathlib_tree-2.4.9/pathlib_tree/exceptions.py
+-rw-r--r--   0        0        0     1878 2023-03-06 19:03:36.669688 pathlib_tree-2.4.9/pathlib_tree/patterns.py
+-rw-r--r--   0        0        0    15899 2023-03-07 05:49:00.780935 pathlib_tree-2.4.9/pathlib_tree/tree.py
+-rw-r--r--   0        0        0      287 2023-03-06 19:22:45.463908 pathlib_tree-2.4.9/pathlib_tree/utils.py
+-rw-r--r--   0        0        0     1088 2023-07-09 02:53:05.193350 pathlib_tree-2.4.9/pyproject.toml
+-rw-r--r--   0        0        0     1242 1970-01-01 00:00:00.000000 pathlib_tree-2.4.9/PKG-INFO
```

### Comparing `pathlib_tree-2.4.8/LICENSE` & `pathlib_tree-2.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pathlib_tree-2.4.8/pathlib_tree/patterns.py` & `pathlib_tree-2.4.9/pathlib_tree/patterns.py`

 * *Files identical despite different names*

### Comparing `pathlib_tree-2.4.8/pathlib_tree/tree.py` & `pathlib_tree-2.4.9/pathlib_tree/tree.py`

 * *Files identical despite different names*

### Comparing `pathlib_tree-2.4.8/pyproject.toml` & `pathlib_tree-2.4.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pathlib-tree"
-version = "2.4.8"
+version = "2.4.9"
 description = "Filesystem tree utilities"
 authors = ["Ilkka Tuohela <hile@iki.fi>"]
 readme = "README.md"
 homepage = "https://github.com/hile/pathlib-tree"
 include = [
     "LICENSE",
 ]
@@ -33,11 +33,15 @@
 flake8-bugbear = "^22"
 flake8-quotes = "^3"
 pycodestyle = "^2"
 pyflakes = "^3"
 pylint = "^2"
 pytest = "^7"
 tox = "^4"
+ruff = "^0.0.261"
+
+[tool.ruff]
+line-length = 120
 
 [build-system]
-requires = ["poetry-core>=1.3.2"]
+requires = ["poetry-core>=1.5.2"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pathlib_tree-2.4.8/PKG-INFO` & `pathlib_tree-2.4.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pathlib-tree
-Version: 2.4.8
+Version: 2.4.9
 Summary: Filesystem tree utilities
 Home-page: https://github.com/hile/pathlib-tree
 License: BSD-3-Clause
 Author: Ilkka Tuohela
 Author-email: hile@iki.fi
 Requires-Python: >=3.9,<4.0
 Classifier: Environment :: Console
@@ -12,17 +12,14 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities
 Requires-Dist: cli-toolkit (>=2,<3)
 Requires-Dist: filemagic (>=1.6,<2.0)
 Requires-Dist: python-magic-bin (>=0.4.14,<0.5.0) ; sys_platform == "win32"
 Description-Content-Type: text/markdown
 
 ![Unit Tests](https://github.com/hile/pathlib-tree/actions/workflows/unittest.yml/badge.svg)
```

