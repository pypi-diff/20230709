# Comparing `tmp/sys_toolkit-2.5.0.tar.gz` & `tmp/sys_toolkit-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sys_toolkit-2.5.0.tar", max compression
+gzip compressed data, was "sys_toolkit-2.5.1.tar", max compression
```

## Comparing `sys_toolkit-2.5.0.tar` & `sys_toolkit-2.5.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1497 2023-03-05 17:02:32.837216 sys_toolkit-2.5.0/LICENSE
--rw-r--r--   0        0        0      784 2022-07-27 08:25:26.079239 sys_toolkit-2.5.0/README.md
--rw-r--r--   0        0        0     1065 2023-03-18 10:02:01.585854 sys_toolkit-2.5.0/pyproject.toml
--rw-r--r--   0        0        0      157 2023-03-05 17:43:09.568131 sys_toolkit-2.5.0/sys_toolkit/__init__.py
--rw-r--r--   0        0        0     2217 2023-03-05 17:46:48.611728 sys_toolkit-2.5.0/sys_toolkit/base.py
--rw-r--r--   0        0        0      175 2023-03-05 17:43:21.625943 sys_toolkit-2.5.0/sys_toolkit/clipboard/__init__.py
--rw-r--r--   0        0        0     4321 2023-03-05 17:43:28.434666 sys_toolkit-2.5.0/sys_toolkit/clipboard/base.py
--rw-r--r--   0        0        0     1524 2023-03-05 17:43:37.347119 sys_toolkit-2.5.0/sys_toolkit/clipboard/darwin.py
--rw-r--r--   0        0        0     1610 2023-03-05 17:43:45.661608 sys_toolkit-2.5.0/sys_toolkit/clipboard/wayland.py
--rw-r--r--   0        0        0     2315 2023-03-05 17:43:59.432199 sys_toolkit-2.5.0/sys_toolkit/clipboard/xclip.py
--rw-r--r--   0        0        0     5449 2023-03-05 17:46:53.564044 sys_toolkit-2.5.0/sys_toolkit/collection.py
--rw-r--r--   0        0        0      357 2023-03-05 17:44:08.169410 sys_toolkit-2.5.0/sys_toolkit/configuration/__init__.py
--rw-r--r--   0        0        0    17442 2023-03-05 17:44:12.906674 sys_toolkit-2.5.0/sys_toolkit/configuration/base.py
--rw-r--r--   0        0        0     3015 2023-03-05 17:44:23.429673 sys_toolkit-2.5.0/sys_toolkit/configuration/directory.py
--rw-r--r--   0        0        0     2455 2023-03-05 17:44:31.446979 sys_toolkit-2.5.0/sys_toolkit/configuration/file.py
--rw-r--r--   0        0        0     1820 2023-03-05 17:44:38.444727 sys_toolkit-2.5.0/sys_toolkit/configuration/ini.py
--rw-r--r--   0        0        0     1737 2023-03-05 17:44:45.370060 sys_toolkit-2.5.0/sys_toolkit/configuration/json.py
--rw-r--r--   0        0        0     1236 2023-03-05 17:44:53.226491 sys_toolkit-2.5.0/sys_toolkit/configuration/yaml.py
--rw-r--r--   0        0        0      212 2023-03-05 17:47:02.897435 sys_toolkit-2.5.0/sys_toolkit/constants.py
--rw-r--r--   0        0        0     2655 2023-03-05 17:47:45.152159 sys_toolkit-2.5.0/sys_toolkit/encoders.py
--rw-r--r--   0        0        0      755 2023-03-05 17:47:43.865933 sys_toolkit-2.5.0/sys_toolkit/exceptions.py
--rw-r--r--   0        0        0     1904 2023-03-05 17:47:42.680364 sys_toolkit-2.5.0/sys_toolkit/fixtures.py
--rw-r--r--   0        0        0    13463 2023-03-05 17:47:41.415099 sys_toolkit-2.5.0/sys_toolkit/logger.py
--rw-r--r--   0        0        0      602 2023-03-05 17:47:38.782574 sys_toolkit-2.5.0/sys_toolkit/modules.py
--rw-r--r--   0        0        0     3149 2023-03-05 17:47:35.675892 sys_toolkit-2.5.0/sys_toolkit/path.py
--rw-r--r--   0        0        0     2623 2023-03-18 09:51:23.210806 sys_toolkit-2.5.0/sys_toolkit/platform.py
--rw-r--r--   0        0        0     5490 2023-03-05 17:47:28.305357 sys_toolkit-2.5.0/sys_toolkit/process.py
--rw-r--r--   0        0        0     4706 2023-03-05 17:47:25.125483 sys_toolkit-2.5.0/sys_toolkit/subprocess.py
--rw-r--r--   0        0        0      145 2023-03-05 17:45:17.543432 sys_toolkit-2.5.0/sys_toolkit/system/__init__.py
--rw-r--r--   0        0        0     1589 2023-03-05 17:45:23.941679 sys_toolkit-2.5.0/sys_toolkit/system/darwin.py
--rw-r--r--   0        0        0     1603 2023-03-05 17:45:30.991382 sys_toolkit-2.5.0/sys_toolkit/system/info.py
--rw-r--r--   0        0        0      138 2023-03-05 17:46:01.713161 sys_toolkit-2.5.0/sys_toolkit/tests/__init__.py
--rw-r--r--   0        0        0     6420 2023-03-07 03:08:28.668031 sys_toolkit-2.5.0/sys_toolkit/tests/mock.py
--rw-r--r--   0        0        0      567 2023-03-05 17:46:15.686966 sys_toolkit-2.5.0/sys_toolkit/tests/packaging.py
--rw-r--r--   0        0        0     2333 2023-03-05 17:47:21.811949 sys_toolkit-2.5.0/sys_toolkit/textfile.py
--rw-r--r--   0        0        0      200 2023-03-05 17:46:23.936554 sys_toolkit-2.5.0/sys_toolkit/tmpdir/__init__.py
--rw-r--r--   0        0        0     3474 2023-03-05 17:46:33.609064 sys_toolkit-2.5.0/sys_toolkit/tmpdir/base.py
--rw-r--r--   0        0        0     3835 2023-03-05 17:46:39.179102 sys_toolkit-2.5.0/sys_toolkit/tmpdir/darwin.py
--rw-r--r--   0        0        0     1730 1970-01-01 00:00:00.000000 sys_toolkit-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1497 2023-03-05 17:02:32.837216 sys_toolkit-2.5.1/LICENSE
+-rw-r--r--   0        0        0      784 2022-07-27 08:25:26.079239 sys_toolkit-2.5.1/README.md
+-rw-r--r--   0        0        0     1114 2023-07-09 02:46:45.247813 sys_toolkit-2.5.1/pyproject.toml
+-rw-r--r--   0        0        0      157 2023-03-05 17:43:09.568131 sys_toolkit-2.5.1/sys_toolkit/__init__.py
+-rw-r--r--   0        0        0     2217 2023-05-06 04:53:18.382252 sys_toolkit-2.5.1/sys_toolkit/base.py
+-rw-r--r--   0        0        0      175 2023-05-06 04:53:18.386030 sys_toolkit-2.5.1/sys_toolkit/clipboard/__init__.py
+-rw-r--r--   0        0        0     4321 2023-05-06 04:53:18.390059 sys_toolkit-2.5.1/sys_toolkit/clipboard/base.py
+-rw-r--r--   0        0        0     1524 2023-05-06 04:53:18.394220 sys_toolkit-2.5.1/sys_toolkit/clipboard/darwin.py
+-rw-r--r--   0        0        0     1610 2023-05-06 04:53:18.398217 sys_toolkit-2.5.1/sys_toolkit/clipboard/wayland.py
+-rw-r--r--   0        0        0     2315 2023-05-06 04:53:18.401175 sys_toolkit-2.5.1/sys_toolkit/clipboard/xclip.py
+-rw-r--r--   0        0        0     5449 2023-05-06 04:53:18.406072 sys_toolkit-2.5.1/sys_toolkit/collection.py
+-rw-r--r--   0        0        0      357 2023-03-05 17:44:08.169410 sys_toolkit-2.5.1/sys_toolkit/configuration/__init__.py
+-rw-r--r--   0        0        0    17442 2023-05-06 04:53:18.414226 sys_toolkit-2.5.1/sys_toolkit/configuration/base.py
+-rw-r--r--   0        0        0     3015 2023-03-05 17:44:23.429673 sys_toolkit-2.5.1/sys_toolkit/configuration/directory.py
+-rw-r--r--   0        0        0     2455 2023-03-05 17:44:31.446979 sys_toolkit-2.5.1/sys_toolkit/configuration/file.py
+-rw-r--r--   0        0        0     1820 2023-03-05 17:44:38.444727 sys_toolkit-2.5.1/sys_toolkit/configuration/ini.py
+-rw-r--r--   0        0        0     1737 2023-03-05 17:44:45.370060 sys_toolkit-2.5.1/sys_toolkit/configuration/json.py
+-rw-r--r--   0        0        0     1236 2023-03-05 17:44:53.226491 sys_toolkit-2.5.1/sys_toolkit/configuration/yaml.py
+-rw-r--r--   0        0        0      212 2023-03-05 17:47:02.897435 sys_toolkit-2.5.1/sys_toolkit/constants.py
+-rw-r--r--   0        0        0     2655 2023-05-06 04:53:18.417752 sys_toolkit-2.5.1/sys_toolkit/encoders.py
+-rw-r--r--   0        0        0      755 2023-03-05 17:47:43.865933 sys_toolkit-2.5.1/sys_toolkit/exceptions.py
+-rw-r--r--   0        0        0     1904 2023-03-05 17:47:42.680364 sys_toolkit-2.5.1/sys_toolkit/fixtures.py
+-rw-r--r--   0        0        0    13463 2023-05-06 04:53:18.422005 sys_toolkit-2.5.1/sys_toolkit/logger.py
+-rw-r--r--   0        0        0      602 2023-05-06 04:53:18.426293 sys_toolkit-2.5.1/sys_toolkit/modules.py
+-rw-r--r--   0        0        0     3149 2023-05-06 04:53:18.429747 sys_toolkit-2.5.1/sys_toolkit/path.py
+-rw-r--r--   0        0        0     2623 2023-03-18 09:51:23.210806 sys_toolkit-2.5.1/sys_toolkit/platform.py
+-rw-r--r--   0        0        0     5490 2023-05-06 04:53:18.433203 sys_toolkit-2.5.1/sys_toolkit/process.py
+-rw-r--r--   0        0        0     4706 2023-05-06 04:53:18.437413 sys_toolkit-2.5.1/sys_toolkit/subprocess.py
+-rw-r--r--   0        0        0      145 2023-03-05 17:45:17.543432 sys_toolkit-2.5.1/sys_toolkit/system/__init__.py
+-rw-r--r--   0        0        0     1589 2023-05-06 04:53:18.441050 sys_toolkit-2.5.1/sys_toolkit/system/darwin.py
+-rw-r--r--   0        0        0     1603 2023-05-06 04:53:18.444495 sys_toolkit-2.5.1/sys_toolkit/system/info.py
+-rw-r--r--   0        0        0      138 2023-03-05 17:46:01.713161 sys_toolkit-2.5.1/sys_toolkit/tests/__init__.py
+-rw-r--r--   0        0        0     6420 2023-05-06 04:53:18.448130 sys_toolkit-2.5.1/sys_toolkit/tests/mock.py
+-rw-r--r--   0        0        0      567 2023-05-06 04:53:18.451954 sys_toolkit-2.5.1/sys_toolkit/tests/packaging.py
+-rw-r--r--   0        0        0     2333 2023-05-06 04:53:18.458136 sys_toolkit-2.5.1/sys_toolkit/textfile.py
+-rw-r--r--   0        0        0      200 2023-05-06 04:53:18.462213 sys_toolkit-2.5.1/sys_toolkit/tmpdir/__init__.py
+-rw-r--r--   0        0        0     3474 2023-05-06 04:53:18.471549 sys_toolkit-2.5.1/sys_toolkit/tmpdir/base.py
+-rw-r--r--   0        0        0     3835 2023-05-06 04:53:18.492491 sys_toolkit-2.5.1/sys_toolkit/tmpdir/darwin.py
+-rw-r--r--   0        0        0     1578 1970-01-01 00:00:00.000000 sys_toolkit-2.5.1/PKG-INFO
```

### Comparing `sys_toolkit-2.5.0/LICENSE` & `sys_toolkit-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sys_toolkit-2.5.0/README.md` & `sys_toolkit-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `sys_toolkit-2.5.0/pyproject.toml` & `sys_toolkit-2.5.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sys-toolkit"
-version = "2.5.0"
+version = "2.5.1"
 description = "Classes for operating system utilities"
 authors = ["Ilkka Tuohela <hile@iki.fi>"]
 homepage = "https://github.com/hile/sys-toolkit"
 readme = "README.md"
 include = [
     "LICENSE",
 ]
@@ -32,14 +32,18 @@
 flake8-bugbear = "^22"
 flake8-quotes = "^3"
 pycodestyle = "^2"
 pyflakes = "^3"
 pylint = "^2"
 pytest = "^7"
 tox = "^4"
+ruff = "^0.0.261"
 
 [tool.poetry.plugins.pytest11]
 sys_toolkit_fixtures = 'sys_toolkit.fixtures'
 
+[tool.ruff]
+line-length = 120
+
 [build-system]
-requires = ["poetry-core>=1.3.2"]
+requires = ["poetry-core>=1.5.2"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `sys_toolkit-2.5.0/sys_toolkit/base.py` & `sys_toolkit-2.5.1/sys_toolkit/base.py`

 * *Files identical despite different names*

### Comparing `sys_toolkit-2.5.0/sys_toolkit/clipboard/base.py` & `sys_toolkit-2.5.1/sys_toolkit/clipboard/base.py`

 * *Files identical despite different names*

### Comparing `sys_toolkit-2.5.0/sys_toolkit/clipboard/darwin.py` & `sys_toolkit-2.5.1/sys_toolkit/clipboard/darwin.py`

 * *Files identical despite different names*

### Comparing `sys_toolkit-2.5.0/sys_toolkit/clipboard/wayland.py` & `sys_toolkit-2.5.1/sys_toolkit/clipboard/wayland.py`

 * *Files identical despite different names*

### Comparing `sys_toolkit-2.5.0/sys_toolkit/clipboard/xclip.py` & `sys_toolkit-2.5.1/sys_toolkit/clipboard/xclip.py`

 * *Files identical despite different names*

### Comparing `sys_toolkit-2.5.0/sys_toolkit/collection.py` & `sys_toolkit-2.5.1/sys_toolkit/collection.py`

 * *Files identical despite different names*

### Comparing `sys_toolkit-2.5.0/sys_toolkit/configuration/base.py` & `sys_toolkit-2.5.1/sys_toolkit/configuration/base.py`

 * *Files identical despite different names*

### Comparing `sys_toolkit-2.5.0/sys_toolkit/configuration/directory.py` & `sys_toolkit-2.5.1/sys_toolkit/configuration/directory.py`

 * *Files identical despite different names*

### Comparing `sys_toolkit-2.5.0/sys_toolkit/configuration/file.py` & `sys_toolkit-2.5.1/sys_toolkit/configuration/file.py`

 * *Files identical despite different names*

### Comparing `sys_toolkit-2.5.0/sys_toolkit/configuration/ini.py` & `sys_toolkit-2.5.1/sys_toolkit/configuration/ini.py`

 * *Files identical despite different names*

### Comparing `sys_toolkit-2.5.0/sys_toolkit/configuration/json.py` & `sys_toolkit-2.5.1/sys_toolkit/configuration/json.py`

 * *Files identical despite different names*

### Comparing `sys_toolkit-2.5.0/sys_toolkit/configuration/yaml.py` & `sys_toolkit-2.5.1/sys_toolkit/configuration/yaml.py`

 * *Files identical despite different names*

### Comparing `sys_toolkit-2.5.0/sys_toolkit/encoders.py` & `sys_toolkit-2.5.1/sys_toolkit/encoders.py`

 * *Files identical despite different names*

### Comparing `sys_toolkit-2.5.0/sys_toolkit/exceptions.py` & `sys_toolkit-2.5.1/sys_toolkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `sys_toolkit-2.5.0/sys_toolkit/fixtures.py` & `sys_toolkit-2.5.1/sys_toolkit/fixtures.py`

 * *Files identical despite different names*

### Comparing `sys_toolkit-2.5.0/sys_toolkit/logger.py` & `sys_toolkit-2.5.1/sys_toolkit/logger.py`

 * *Files identical despite different names*

### Comparing `sys_toolkit-2.5.0/sys_toolkit/modules.py` & `sys_toolkit-2.5.1/sys_toolkit/modules.py`

 * *Files identical despite different names*

### Comparing `sys_toolkit-2.5.0/sys_toolkit/path.py` & `sys_toolkit-2.5.1/sys_toolkit/path.py`

 * *Files identical despite different names*

### Comparing `sys_toolkit-2.5.0/sys_toolkit/platform.py` & `sys_toolkit-2.5.1/sys_toolkit/platform.py`

 * *Files identical despite different names*

### Comparing `sys_toolkit-2.5.0/sys_toolkit/process.py` & `sys_toolkit-2.5.1/sys_toolkit/process.py`

 * *Files identical despite different names*

### Comparing `sys_toolkit-2.5.0/sys_toolkit/subprocess.py` & `sys_toolkit-2.5.1/sys_toolkit/subprocess.py`

 * *Files identical despite different names*

### Comparing `sys_toolkit-2.5.0/sys_toolkit/system/darwin.py` & `sys_toolkit-2.5.1/sys_toolkit/system/darwin.py`

 * *Files identical despite different names*

### Comparing `sys_toolkit-2.5.0/sys_toolkit/system/info.py` & `sys_toolkit-2.5.1/sys_toolkit/system/info.py`

 * *Files identical despite different names*

### Comparing `sys_toolkit-2.5.0/sys_toolkit/tests/mock.py` & `sys_toolkit-2.5.1/sys_toolkit/tests/mock.py`

 * *Files identical despite different names*

### Comparing `sys_toolkit-2.5.0/sys_toolkit/tests/packaging.py` & `sys_toolkit-2.5.1/sys_toolkit/tests/packaging.py`

 * *Files identical despite different names*

### Comparing `sys_toolkit-2.5.0/sys_toolkit/textfile.py` & `sys_toolkit-2.5.1/sys_toolkit/textfile.py`

 * *Files identical despite different names*

### Comparing `sys_toolkit-2.5.0/sys_toolkit/tmpdir/base.py` & `sys_toolkit-2.5.1/sys_toolkit/tmpdir/base.py`

 * *Files identical despite different names*

### Comparing `sys_toolkit-2.5.0/sys_toolkit/tmpdir/darwin.py` & `sys_toolkit-2.5.1/sys_toolkit/tmpdir/darwin.py`

 * *Files identical despite different names*

### Comparing `sys_toolkit-2.5.0/PKG-INFO` & `sys_toolkit-2.5.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sys-toolkit
-Version: 2.5.0
+Version: 2.5.1
 Summary: Classes for operating system utilities
 Home-page: https://github.com/hile/sys-toolkit
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
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: inflection (>=0.5,<0.6)
 Description-Content-Type: text/markdown
 
 ![Unit Tests](https://github.com/hile/sys-toolkit/actions/workflows/unittest.yml/badge.svg)
 ![Style Checks](https://github.com/hile/sys-toolkit/actions/workflows/lint.yml/badge.svg)
```

