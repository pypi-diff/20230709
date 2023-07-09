# Comparing `tmp/web_ext_helper-1.1.9.tar.gz` & `tmp/web_ext_helper-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web_ext_helper-1.1.9.tar", max compression
+gzip compressed data, was "web_ext_helper-1.2.0.tar", max compression
```

## Comparing `web_ext_helper-1.1.9.tar` & `web_ext_helper-1.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35822 2023-06-17 19:16:11.163007 web_ext_helper-1.1.9/LICENSE
--rw-r--r--   0        0        0      659 2023-07-09 21:02:11.518233 web_ext_helper-1.1.9/pyproject.toml
--rw-r--r--   0        0        0     1871 2023-06-19 17:29:34.258602 web_ext_helper-1.1.9/README.md
--rw-r--r--   0        0        0      262 2023-06-18 17:57:02.181036 web_ext_helper-1.1.9/web_ext_helper/classes.py
--rw-r--r--   0        0        0      613 2023-06-18 17:49:15.766872 web_ext_helper-1.1.9/web_ext_helper/functions.py
--rw-r--r--   0        0        0    21295 2023-07-09 21:02:00.258892 web_ext_helper-1.1.9/web_ext_helper/web_ext_helper.py
--rw-r--r--   0        0        0     2441 1970-01-01 00:00:00.000000 web_ext_helper-1.1.9/PKG-INFO
+-rw-r--r--   0        0        0    35822 2023-06-17 19:16:11.163007 web_ext_helper-1.2.0/LICENSE
+-rw-r--r--   0        0        0      659 2023-07-09 21:14:29.386245 web_ext_helper-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1871 2023-06-19 17:29:34.258602 web_ext_helper-1.2.0/README.md
+-rw-r--r--   0        0        0      262 2023-06-18 17:57:02.181036 web_ext_helper-1.2.0/web_ext_helper/classes.py
+-rw-r--r--   0        0        0      613 2023-06-18 17:49:15.766872 web_ext_helper-1.2.0/web_ext_helper/functions.py
+-rw-r--r--   0        0        0    21525 2023-07-09 21:14:12.816226 web_ext_helper-1.2.0/web_ext_helper/web_ext_helper.py
+-rw-r--r--   0        0        0     2441 1970-01-01 00:00:00.000000 web_ext_helper-1.2.0/PKG-INFO
```

### Comparing `web_ext_helper-1.1.9/LICENSE` & `web_ext_helper-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.1.9/pyproject.toml` & `web_ext_helper-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "web-ext-helper"
-version = "1.1.9"
-description = "An awseome CLI for building, publishing and running web extensions."
+version = "1.2.0"
+description = "An awesome CLI for building, publishing and running web extensions."
 authors = ["AppSolves <appsolves@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [{include = "web_ext_helper"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `web_ext_helper-1.1.9/README.md` & `web_ext_helper-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.1.9/web_ext_helper/functions.py` & `web_ext_helper-1.2.0/web_ext_helper/functions.py`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.1.9/web_ext_helper/web_ext_helper.py` & `web_ext_helper-1.2.0/web_ext_helper/web_ext_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__ext_version__ = "1.1.9"
+__ext_version__ = "1.2.0"
 
 import os
 import sys
 import json
 import shutil
 import typer
 import zipfile
@@ -31,15 +31,17 @@
 web_ext_helper_logo = rf"""{bcolors.OKGREEN}
               ___.                              __            .__           .__                       
 __  _  __ ____\_ |__             ____ ___  ____/  |_          |  |__   ____ |  | ______   ___________ 
 \ \/ \/ // __ \| __ \   ______ _/ __ \\  \/  /\   __\  ______ |  |  \_/ __ \|  | \____ \_/ __ \_  __ \
  \     /\  ___/| \_\ \ /_____/ \  ___/ >    <  |  |   /_____/ |   Y  \  ___/|  |_|  |_> >  ___/|  | \/
   \/\_/  \___  >___  /          \___  >__/\_ \ |__|           |___|  /\___  >____/   __/ \___  >__|   
              \/    \/               \/      \/                     \/     \/     |__|        \/       
-{bcolors.ENDC}"""
+
+ Version: {bcolors.PURPLE}{__ext_version__}{bcolors.OKGREEN}
+ An awesome CLI for {bcolors.OKCYAN}building{bcolors.OKGREEN}, {bcolors.OKCYAN}publishing {bcolors.OKGREEN}and {bcolors.OKCYAN}running {bcolors.PURPLE}web extensions.{bcolors.ENDC}"""
 
 load_dotenv(cached_app_data_env_dir)
 
 app = typer.Typer(
     help="An awseome CLI for building, publishing and running web extensions."
 )
```

### Comparing `web_ext_helper-1.1.9/PKG-INFO` & `web_ext_helper-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: web-ext-helper
-Version: 1.1.9
-Summary: An awseome CLI for building, publishing and running web extensions.
+Version: 1.2.0
+Summary: An awesome CLI for building, publishing and running web extensions.
 License: GPL-3.0-or-later
 Author: AppSolves
 Author-email: appsolves@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

