# Comparing `tmp/treesync-1.5.0.tar.gz` & `tmp/treesync-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "treesync-1.5.0.tar", max compression
+gzip compressed data, was "treesync-1.5.1.tar", max compression
```

## Comparing `treesync-1.5.0.tar` & `treesync-1.5.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1497 2023-03-10 15:53:58.794087 treesync-1.5.0/LICENSE
--rw-r--r--   0        0        0     4808 2022-10-02 06:36:08.913659 treesync-1.5.0/README.md
--rw-r--r--   0        0        0     1039 2023-03-10 15:55:37.244319 treesync-1.5.0/pyproject.toml
--rw-r--r--   0        0        0      155 2023-03-10 15:52:50.019142 treesync-1.5.0/treesync/__init__.py
--rw-r--r--   0        0        0      160 2023-03-10 15:52:35.267934 treesync-1.5.0/treesync/bin/__init__.py
--rw-r--r--   0        0        0      134 2023-03-10 15:51:34.234840 treesync-1.5.0/treesync/bin/treesync/__init__.py
--rw-r--r--   0        0        0      142 2023-03-10 15:51:46.679406 treesync-1.5.0/treesync/bin/treesync/commands/__init__.py
--rw-r--r--   0        0        0     1704 2023-03-10 15:52:06.550986 treesync-1.5.0/treesync/bin/treesync/commands/base.py
--rw-r--r--   0        0        0      807 2023-03-10 15:51:44.267684 treesync-1.5.0/treesync/bin/treesync/commands/list.py
--rw-r--r--   0        0        0     1331 2023-03-10 15:51:40.287443 treesync-1.5.0/treesync/bin/treesync/commands/pull.py
--rw-r--r--   0        0        0     1327 2023-03-10 15:52:08.851717 treesync-1.5.0/treesync/bin/treesync/commands/push.py
--rw-r--r--   0        0        0     1374 2023-03-10 15:51:37.139523 treesync-1.5.0/treesync/bin/treesync/commands/show.py
--rw-r--r--   0        0        0      713 2023-03-10 15:52:22.998318 treesync-1.5.0/treesync/bin/treesync/main.py
--rw-r--r--   0        0        0      201 2023-03-10 15:50:37.928188 treesync-1.5.0/treesync/configuration/__init__.py
--rw-r--r--   0        0        0      965 2023-03-10 15:51:31.484259 treesync-1.5.0/treesync/configuration/defaults.py
--rw-r--r--   0        0        0     5450 2023-03-10 15:50:43.428450 treesync-1.5.0/treesync/configuration/hosts.py
--rw-r--r--   0        0        0     3146 2023-03-10 15:51:24.702957 treesync-1.5.0/treesync/configuration/loader.py
--rw-r--r--   0        0        0     1350 2023-03-10 15:51:11.516316 treesync-1.5.0/treesync/configuration/servers.py
--rw-r--r--   0        0        0     1020 2023-03-10 15:51:21.945989 treesync-1.5.0/treesync/configuration/sources.py
--rw-r--r--   0        0        0     3627 2023-03-10 15:50:26.990233 treesync-1.5.0/treesync/configuration/targets.py
--rw-r--r--   0        0        0      937 2023-03-10 15:52:43.343737 treesync-1.5.0/treesync/constants.py
--rw-r--r--   0        0        0      335 2023-03-10 15:52:52.193518 treesync-1.5.0/treesync/exceptions.py
--rw-r--r--   0        0        0     1326 2023-03-10 15:52:37.974993 treesync-1.5.0/treesync/host.py
--rw-r--r--   0        0        0     9213 2023-03-10 15:52:55.587785 treesync-1.5.0/treesync/target.py
--rw-r--r--   0        0        0     5717 1970-01-01 00:00:00.000000 treesync-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1497 2023-03-10 15:53:58.794087 treesync-1.5.1/LICENSE
+-rw-r--r--   0        0        0     4808 2022-10-02 06:36:08.913659 treesync-1.5.1/README.md
+-rw-r--r--   0        0        0     1088 2023-07-09 02:58:06.157057 treesync-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0      155 2023-03-10 15:52:50.019142 treesync-1.5.1/treesync/__init__.py
+-rw-r--r--   0        0        0      160 2023-03-10 15:52:35.267934 treesync-1.5.1/treesync/bin/__init__.py
+-rw-r--r--   0        0        0      134 2023-03-10 15:51:34.234840 treesync-1.5.1/treesync/bin/treesync/__init__.py
+-rw-r--r--   0        0        0      142 2023-03-10 15:51:46.679406 treesync-1.5.1/treesync/bin/treesync/commands/__init__.py
+-rw-r--r--   0        0        0     1704 2023-03-10 15:52:06.550986 treesync-1.5.1/treesync/bin/treesync/commands/base.py
+-rw-r--r--   0        0        0      807 2023-03-10 15:51:44.267684 treesync-1.5.1/treesync/bin/treesync/commands/list.py
+-rw-r--r--   0        0        0     1331 2023-03-10 15:51:40.287443 treesync-1.5.1/treesync/bin/treesync/commands/pull.py
+-rw-r--r--   0        0        0     1327 2023-03-10 15:52:08.851717 treesync-1.5.1/treesync/bin/treesync/commands/push.py
+-rw-r--r--   0        0        0     1374 2023-03-10 15:51:37.139523 treesync-1.5.1/treesync/bin/treesync/commands/show.py
+-rw-r--r--   0        0        0      713 2023-03-10 15:52:22.998318 treesync-1.5.1/treesync/bin/treesync/main.py
+-rw-r--r--   0        0        0      201 2023-03-10 15:50:37.928188 treesync-1.5.1/treesync/configuration/__init__.py
+-rw-r--r--   0        0        0      965 2023-03-10 15:51:31.484259 treesync-1.5.1/treesync/configuration/defaults.py
+-rw-r--r--   0        0        0     5450 2023-03-10 15:50:43.428450 treesync-1.5.1/treesync/configuration/hosts.py
+-rw-r--r--   0        0        0     3146 2023-03-10 15:51:24.702957 treesync-1.5.1/treesync/configuration/loader.py
+-rw-r--r--   0        0        0     1350 2023-03-10 15:51:11.516316 treesync-1.5.1/treesync/configuration/servers.py
+-rw-r--r--   0        0        0     1020 2023-03-10 15:51:21.945989 treesync-1.5.1/treesync/configuration/sources.py
+-rw-r--r--   0        0        0     3627 2023-03-10 15:50:26.990233 treesync-1.5.1/treesync/configuration/targets.py
+-rw-r--r--   0        0        0      937 2023-03-10 15:52:43.343737 treesync-1.5.1/treesync/constants.py
+-rw-r--r--   0        0        0      335 2023-03-10 15:52:52.193518 treesync-1.5.1/treesync/exceptions.py
+-rw-r--r--   0        0        0     1326 2023-03-10 15:52:37.974993 treesync-1.5.1/treesync/host.py
+-rw-r--r--   0        0        0     9213 2023-03-10 15:52:55.587785 treesync-1.5.1/treesync/target.py
+-rw-r--r--   0        0        0     5565 1970-01-01 00:00:00.000000 treesync-1.5.1/PKG-INFO
```

### Comparing `treesync-1.5.0/LICENSE` & `treesync-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `treesync-1.5.0/README.md` & `treesync-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `treesync-1.5.0/pyproject.toml` & `treesync-1.5.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "treesync"
-version = "1.5.0"
+version = "1.5.1"
 description = "Utilitiies to use rsync for multiple targets"
 authors = ["Ilkka Tuohela <hile@iki.fi>"]
 homepage = "https://github.com/hile/treesync"
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
 
 [tool.poetry.scripts]
 treesync = "treesync.bin.treesync.main:main"
 
+[tool.ruff]
+line-length = 120
+
 [build-system]
-requires = ["poetry-core>=1.3.2"]
+requires = ["poetry-core>=1.5.2"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `treesync-1.5.0/treesync/bin/treesync/commands/base.py` & `treesync-1.5.1/treesync/bin/treesync/commands/base.py`

 * *Files identical despite different names*

### Comparing `treesync-1.5.0/treesync/bin/treesync/commands/list.py` & `treesync-1.5.1/treesync/bin/treesync/commands/list.py`

 * *Files identical despite different names*

### Comparing `treesync-1.5.0/treesync/bin/treesync/commands/pull.py` & `treesync-1.5.1/treesync/bin/treesync/commands/pull.py`

 * *Files identical despite different names*

### Comparing `treesync-1.5.0/treesync/bin/treesync/commands/push.py` & `treesync-1.5.1/treesync/bin/treesync/commands/push.py`

 * *Files identical despite different names*

### Comparing `treesync-1.5.0/treesync/bin/treesync/commands/show.py` & `treesync-1.5.1/treesync/bin/treesync/commands/show.py`

 * *Files identical despite different names*

### Comparing `treesync-1.5.0/treesync/bin/treesync/main.py` & `treesync-1.5.1/treesync/bin/treesync/main.py`

 * *Files identical despite different names*

### Comparing `treesync-1.5.0/treesync/configuration/defaults.py` & `treesync-1.5.1/treesync/configuration/defaults.py`

 * *Files identical despite different names*

### Comparing `treesync-1.5.0/treesync/configuration/hosts.py` & `treesync-1.5.1/treesync/configuration/hosts.py`

 * *Files identical despite different names*

### Comparing `treesync-1.5.0/treesync/configuration/loader.py` & `treesync-1.5.1/treesync/configuration/loader.py`

 * *Files identical despite different names*

### Comparing `treesync-1.5.0/treesync/configuration/servers.py` & `treesync-1.5.1/treesync/configuration/servers.py`

 * *Files identical despite different names*

### Comparing `treesync-1.5.0/treesync/configuration/sources.py` & `treesync-1.5.1/treesync/configuration/sources.py`

 * *Files identical despite different names*

### Comparing `treesync-1.5.0/treesync/configuration/targets.py` & `treesync-1.5.1/treesync/configuration/targets.py`

 * *Files identical despite different names*

### Comparing `treesync-1.5.0/treesync/constants.py` & `treesync-1.5.1/treesync/constants.py`

 * *Files identical despite different names*

### Comparing `treesync-1.5.0/treesync/host.py` & `treesync-1.5.1/treesync/host.py`

 * *Files identical despite different names*

### Comparing `treesync-1.5.0/treesync/target.py` & `treesync-1.5.1/treesync/target.py`

 * *Files identical despite different names*

### Comparing `treesync-1.5.0/PKG-INFO` & `treesync-1.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treesync
-Version: 1.5.0
+Version: 1.5.1
 Summary: Utilitiies to use rsync for multiple targets
 Home-page: https://github.com/hile/treesync
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
 Requires-Dist: pathlib-tree (>=2,<3)
 Description-Content-Type: text/markdown
 
 ![Unit Tests](https://github.com/hile/treesync/actions/workflows/unittest.yml/badge.svg)
 ![Style Checks](https://github.com/hile/treesync/actions/workflows/lint.yml/badge.svg)
```

