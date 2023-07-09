# Comparing `tmp/cli_toolkit-2.5.0.tar.gz` & `tmp/cli_toolkit-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli_toolkit-2.5.0.tar", max compression
+gzip compressed data, was "cli_toolkit-2.5.1.tar", max compression
```

## Comparing `cli_toolkit-2.5.0.tar` & `cli_toolkit-2.5.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1497 2023-03-06 18:54:07.842811 cli_toolkit-2.5.0/LICENSE
--rw-r--r--   0        0        0     3376 2022-07-27 08:30:13.204835 cli_toolkit-2.5.0/README.md
--rw-r--r--   0        0        0      288 2023-03-06 17:43:40.864553 cli_toolkit-2.5.0/cli_toolkit/__init__.py
--rw-r--r--   0        0        0     8711 2023-03-06 18:03:38.374239 cli_toolkit-2.5.0/cli_toolkit/base.py
--rw-r--r--   0        0        0     3119 2023-03-06 18:08:14.673174 cli_toolkit-2.5.0/cli_toolkit/command.py
--rw-r--r--   0        0        0      234 2023-03-06 17:43:57.567788 cli_toolkit-2.5.0/cli_toolkit/exceptions.py
--rw-r--r--   0        0        0      431 2023-03-07 03:06:45.389105 cli_toolkit-2.5.0/cli_toolkit/fixtures.py
--rw-r--r--   0        0        0     4003 2023-03-06 18:16:37.076383 cli_toolkit-2.5.0/cli_toolkit/script.py
--rw-r--r--   0        0        0     3472 2023-03-06 18:22:01.357405 cli_toolkit-2.5.0/cli_toolkit/task.py
--rw-r--r--   0        0        0      150 2023-03-06 17:43:23.324926 cli_toolkit-2.5.0/cli_toolkit/tests/__init__.py
--rw-r--r--   0        0        0     2721 2023-03-06 18:02:08.618848 cli_toolkit-2.5.0/cli_toolkit/tests/script.py
--rw-r--r--   0        0        0     1053 2023-03-18 10:03:14.494469 cli_toolkit-2.5.0/pyproject.toml
--rw-r--r--   0        0        0     4289 1970-01-01 00:00:00.000000 cli_toolkit-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1497 2023-03-06 18:54:07.842811 cli_toolkit-2.5.1/LICENSE
+-rw-r--r--   0        0        0     3376 2022-07-27 08:30:13.204835 cli_toolkit-2.5.1/README.md
+-rw-r--r--   0        0        0      288 2023-03-06 17:43:40.864553 cli_toolkit-2.5.1/cli_toolkit/__init__.py
+-rw-r--r--   0        0        0     8711 2023-03-06 18:03:38.374239 cli_toolkit-2.5.1/cli_toolkit/base.py
+-rw-r--r--   0        0        0     3119 2023-03-06 18:08:14.673174 cli_toolkit-2.5.1/cli_toolkit/command.py
+-rw-r--r--   0        0        0      234 2023-03-06 17:43:57.567788 cli_toolkit-2.5.1/cli_toolkit/exceptions.py
+-rw-r--r--   0        0        0      431 2023-03-07 03:06:45.389105 cli_toolkit-2.5.1/cli_toolkit/fixtures.py
+-rw-r--r--   0        0        0     4003 2023-03-06 18:16:37.076383 cli_toolkit-2.5.1/cli_toolkit/script.py
+-rw-r--r--   0        0        0     3472 2023-03-06 18:22:01.357405 cli_toolkit-2.5.1/cli_toolkit/task.py
+-rw-r--r--   0        0        0      150 2023-03-06 17:43:23.324926 cli_toolkit-2.5.1/cli_toolkit/tests/__init__.py
+-rw-r--r--   0        0        0     2721 2023-03-06 18:02:08.618848 cli_toolkit-2.5.1/cli_toolkit/tests/script.py
+-rw-r--r--   0        0        0     1102 2023-07-09 02:50:58.084414 cli_toolkit-2.5.1/pyproject.toml
+-rw-r--r--   0        0        0     4137 1970-01-01 00:00:00.000000 cli_toolkit-2.5.1/PKG-INFO
```

### Comparing `cli_toolkit-2.5.0/LICENSE` & `cli_toolkit-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cli_toolkit-2.5.0/README.md` & `cli_toolkit-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `cli_toolkit-2.5.0/cli_toolkit/base.py` & `cli_toolkit-2.5.1/cli_toolkit/base.py`

 * *Files identical despite different names*

### Comparing `cli_toolkit-2.5.0/cli_toolkit/command.py` & `cli_toolkit-2.5.1/cli_toolkit/command.py`

 * *Files identical despite different names*

### Comparing `cli_toolkit-2.5.0/cli_toolkit/script.py` & `cli_toolkit-2.5.1/cli_toolkit/script.py`

 * *Files identical despite different names*

### Comparing `cli_toolkit-2.5.0/cli_toolkit/task.py` & `cli_toolkit-2.5.1/cli_toolkit/task.py`

 * *Files identical despite different names*

### Comparing `cli_toolkit-2.5.0/cli_toolkit/tests/script.py` & `cli_toolkit-2.5.1/cli_toolkit/tests/script.py`

 * *Files identical despite different names*

### Comparing `cli_toolkit-2.5.0/pyproject.toml` & `cli_toolkit-2.5.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cli-toolkit"
-version = "2.5.0"
+version = "2.5.1"
 description = "Classes to implement CLI commands in python"
 authors = ["Ilkka Tuohela <hile@iki.fi>"]
 homepage = "https://github.com/hile/cli-toolkit"
 readme = "README.md"
 include = [
     "LICENSE",
 ]
@@ -31,14 +31,18 @@
 flake8-bugbear = "^22"
 flake8-quotes = "^3"
 pycodestyle = "^2"
 pyflakes = "^3"
 pylint = "^2"
 pytest = "^7"
 tox = "^4"
+ruff = "^0.0.261"
 
 [tool.poetry.plugins.pytest11]
 cli_toolkit_fixtures = 'cli_toolkit.fixtures'
 
+[tool.ruff]
+line-length = 120
+
 [build-system]
-requires = ["poetry-core>=1.3.2"]
+requires = ["poetry-core>=1.5.2"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cli_toolkit-2.5.0/PKG-INFO` & `cli_toolkit-2.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-toolkit
-Version: 2.5.0
+Version: 2.5.1
 Summary: Classes to implement CLI commands in python
 Home-page: https://github.com/hile/cli-toolkit
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
 Requires-Dist: sys-toolkit (>=2,<3)
 Description-Content-Type: text/markdown
 
 ![Unit Tests](https://github.com/hile/cli-toolkit/actions/workflows/unittest.yml/badge.svg)
 ![Style Checks](https://github.com/hile/cli-toolkit/actions/workflows/lint.yml/badge.svg)
```

