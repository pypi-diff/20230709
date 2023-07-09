# Comparing `tmp/web_ext_helper-1.1.7.tar.gz` & `tmp/web_ext_helper-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web_ext_helper-1.1.7.tar", max compression
+gzip compressed data, was "web_ext_helper-1.1.8.tar", max compression
```

## Comparing `web_ext_helper-1.1.7.tar` & `web_ext_helper-1.1.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35822 2023-06-17 19:16:11.163007 web_ext_helper-1.1.7/LICENSE
--rw-r--r--   0        0        0      654 2023-07-09 20:23:41.176913 web_ext_helper-1.1.7/pyproject.toml
--rw-r--r--   0        0        0     1871 2023-06-19 17:29:34.258602 web_ext_helper-1.1.7/README.md
--rw-r--r--   0        0        0      262 2023-06-18 17:57:02.181036 web_ext_helper-1.1.7/web_ext_helper/classes.py
--rw-r--r--   0        0        0      613 2023-06-18 17:49:15.766872 web_ext_helper-1.1.7/web_ext_helper/functions.py
--rw-r--r--   0        0        0    20341 2023-07-09 20:23:21.044790 web_ext_helper-1.1.7/web_ext_helper/web_ext_helper.py
--rw-r--r--   0        0        0     2436 1970-01-01 00:00:00.000000 web_ext_helper-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0    35822 2023-06-17 19:16:11.163007 web_ext_helper-1.1.8/LICENSE
+-rw-r--r--   0        0        0      659 2023-07-09 20:57:09.143651 web_ext_helper-1.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1871 2023-06-19 17:29:34.258602 web_ext_helper-1.1.8/README.md
+-rw-r--r--   0        0        0      262 2023-06-18 17:57:02.181036 web_ext_helper-1.1.8/web_ext_helper/classes.py
+-rw-r--r--   0        0        0      613 2023-06-18 17:49:15.766872 web_ext_helper-1.1.8/web_ext_helper/functions.py
+-rw-r--r--   0        0        0    21217 2023-07-09 20:57:16.687103 web_ext_helper-1.1.8/web_ext_helper/web_ext_helper.py
+-rw-r--r--   0        0        0     2441 1970-01-01 00:00:00.000000 web_ext_helper-1.1.8/PKG-INFO
```

### Comparing `web_ext_helper-1.1.7/LICENSE` & `web_ext_helper-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.1.7/pyproject.toml` & `web_ext_helper-1.1.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "web-ext-helper"
-version = "1.1.7"
-description = "A simple cli tool that helps you building your web extensions."
+version = "1.1.8"
+description = "An awseome CLI for building, publishing and running web extensions."
 authors = ["AppSolves <appsolves@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [{include = "web_ext_helper"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `web_ext_helper-1.1.7/README.md` & `web_ext_helper-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.1.7/web_ext_helper/functions.py` & `web_ext_helper-1.1.8/web_ext_helper/functions.py`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.1.7/web_ext_helper/web_ext_helper.py` & `web_ext_helper-1.1.8/web_ext_helper/web_ext_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-__ext_version__ = "1.1.7"
+__ext_version__ = "1.1.8"
 
 import os
+import sys
 import json
 import shutil
 import typer
 import zipfile
 import rich.progress
 import requests as req
 import subprocess as sp
@@ -23,29 +24,43 @@
 cached_app_data_env_dir = os.path.join(
     user_cache_dir("web-ext-helper", False), "data", ".env"
 )
 cached_app_dir = os.path.dirname(os.path.dirname(cached_app_build_dir))
 os.makedirs(cached_app_build_dir, exist_ok=True)
 os.makedirs(os.path.dirname(cached_app_data_env_dir), exist_ok=True)
 
+web_ext_helper_logo = rf"""{bcolors.OKGREEN}
+              ___.                              __            .__           .__                       
+__  _  __ ____\_ |__             ____ ___  ____/  |_          |  |__   ____ |  | ______   ___________ 
+\ \/ \/ // __ \| __ \   ______ _/ __ \\  \/  /\   __\  ______ |  |  \_/ __ \|  | \____ \_/ __ \_  __ \
+ \     /\  ___/| \_\ \ /_____/ \  ___/ >    <  |  |   /_____/ |   Y  \  ___/|  |_|  |_> >  ___/|  | \/
+  \/\_/  \___  >___  /          \___  >__/\_ \ |__|           |___|  /\___  >____/   __/ \___  >__|   
+             \/    \/               \/      \/                     \/     \/     |__|        \/       
+{bcolors.ENDC}"""
+
 load_dotenv(cached_app_data_env_dir)
 
-app = typer.Typer()
+app = typer.Typer(
+    help="An awseome CLI for building, publishing and running web extensions."
+)
 
 try:
     with open("src/manifest.json", "r") as manifest_file:
         manifest_data = json.load(manifest_file)
 
     manifest_name = manifest_data["name"]
     manifest_name_lower = manifest_data["name"].lower()
     manifest_version = manifest_data["version"]
 except FileNotFoundError:
     manifest_name_lower = None
     manifest_version = None
 
+if len(sys.argv) == 2 and sys.argv[1] == "--help":
+    typer.echo(web_ext_helper_logo)
+
 
 @app.command(help="Show the version of the extension", name="version")
 def __version__():
     typer.echo(
         f"{bcolors.OKGREEN}Current {bcolors.OKCYAN}web-ext-helper{bcolors.OKGREEN} version: {bcolors.PURPLE}{__ext_version__}{bcolors.ENDC}"
     )
```

### Comparing `web_ext_helper-1.1.7/PKG-INFO` & `web_ext_helper-1.1.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: web-ext-helper
-Version: 1.1.7
-Summary: A simple cli tool that helps you building your web extensions.
+Version: 1.1.8
+Summary: An awseome CLI for building, publishing and running web extensions.
 License: GPL-3.0-or-later
 Author: AppSolves
 Author-email: appsolves@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

