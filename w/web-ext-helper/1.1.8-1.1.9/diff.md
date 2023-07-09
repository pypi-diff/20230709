# Comparing `tmp/web_ext_helper-1.1.8.tar.gz` & `tmp/web_ext_helper-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web_ext_helper-1.1.8.tar", max compression
+gzip compressed data, was "web_ext_helper-1.1.9.tar", max compression
```

## Comparing `web_ext_helper-1.1.8.tar` & `web_ext_helper-1.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35822 2023-06-17 19:16:11.163007 web_ext_helper-1.1.8/LICENSE
--rw-r--r--   0        0        0      659 2023-07-09 20:57:09.143651 web_ext_helper-1.1.8/pyproject.toml
--rw-r--r--   0        0        0     1871 2023-06-19 17:29:34.258602 web_ext_helper-1.1.8/README.md
--rw-r--r--   0        0        0      262 2023-06-18 17:57:02.181036 web_ext_helper-1.1.8/web_ext_helper/classes.py
--rw-r--r--   0        0        0      613 2023-06-18 17:49:15.766872 web_ext_helper-1.1.8/web_ext_helper/functions.py
--rw-r--r--   0        0        0    21217 2023-07-09 20:57:16.687103 web_ext_helper-1.1.8/web_ext_helper/web_ext_helper.py
--rw-r--r--   0        0        0     2441 1970-01-01 00:00:00.000000 web_ext_helper-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0    35822 2023-06-17 19:16:11.163007 web_ext_helper-1.1.9/LICENSE
+-rw-r--r--   0        0        0      659 2023-07-09 21:02:11.518233 web_ext_helper-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1871 2023-06-19 17:29:34.258602 web_ext_helper-1.1.9/README.md
+-rw-r--r--   0        0        0      262 2023-06-18 17:57:02.181036 web_ext_helper-1.1.9/web_ext_helper/classes.py
+-rw-r--r--   0        0        0      613 2023-06-18 17:49:15.766872 web_ext_helper-1.1.9/web_ext_helper/functions.py
+-rw-r--r--   0        0        0    21295 2023-07-09 21:02:00.258892 web_ext_helper-1.1.9/web_ext_helper/web_ext_helper.py
+-rw-r--r--   0        0        0     2441 1970-01-01 00:00:00.000000 web_ext_helper-1.1.9/PKG-INFO
```

### Comparing `web_ext_helper-1.1.8/LICENSE` & `web_ext_helper-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.1.8/pyproject.toml` & `web_ext_helper-1.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "web-ext-helper"
-version = "1.1.8"
+version = "1.1.9"
 description = "An awseome CLI for building, publishing and running web extensions."
 authors = ["AppSolves <appsolves@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [{include = "web_ext_helper"}]
 
 [tool.poetry.dependencies]
```

### Comparing `web_ext_helper-1.1.8/README.md` & `web_ext_helper-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.1.8/web_ext_helper/functions.py` & `web_ext_helper-1.1.9/web_ext_helper/functions.py`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.1.8/web_ext_helper/web_ext_helper.py` & `web_ext_helper-1.1.9/web_ext_helper/web_ext_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__ext_version__ = "1.1.8"
+__ext_version__ = "1.1.9"
 
 import os
 import sys
 import json
 import shutil
 import typer
 import zipfile
@@ -50,14 +50,17 @@
     manifest_name = manifest_data["name"]
     manifest_name_lower = manifest_data["name"].lower()
     manifest_version = manifest_data["version"]
 except FileNotFoundError:
     manifest_name_lower = None
     manifest_version = None
 
+if len(sys.argv) == 2 and sys.argv[1] == "-h":
+    sys.argv[1] = "--help"
+
 if len(sys.argv) == 2 and sys.argv[1] == "--help":
     typer.echo(web_ext_helper_logo)
 
 
 @app.command(help="Show the version of the extension", name="version")
 def __version__():
     typer.echo(
```

### Comparing `web_ext_helper-1.1.8/PKG-INFO` & `web_ext_helper-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-ext-helper
-Version: 1.1.8
+Version: 1.1.9
 Summary: An awseome CLI for building, publishing and running web extensions.
 License: GPL-3.0-or-later
 Author: AppSolves
 Author-email: appsolves@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

