# Comparing `tmp/pwforecast-1.1.1.tar.gz` & `tmp/pwforecast-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwforecast-1.1.1.tar", last modified: Sun Jul  9 03:07:36 2023, max compression
+gzip compressed data, was "pwforecast-1.1.2.tar", last modified: Sun Jul  9 04:42:06 2023, max compression
```

## Comparing `pwforecast-1.1.1.tar` & `pwforecast-1.1.2.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 03:07:36.719890 pwforecast-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-09 03:07:24.000000 pwforecast-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-09 03:07:36.719890 pwforecast-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-07-09 03:07:24.000000 pwforecast-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 03:07:36.719890 pwforecast-1.1.1/pwforecast/
--rw-r--r--   0 runner    (1001) docker     (123)    16609 2023-07-09 03:07:24.000000 pwforecast-1.1.1/pwforecast/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 03:07:36.719890 pwforecast-1.1.1/pwforecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-09 03:07:36.000000 pwforecast-1.1.1/pwforecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-09 03:07:36.000000 pwforecast-1.1.1/pwforecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 03:07:36.000000 pwforecast-1.1.1/pwforecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-09 03:07:36.000000 pwforecast-1.1.1/pwforecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-09 03:07:36.000000 pwforecast-1.1.1/pwforecast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 03:07:36.719890 pwforecast-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-09 03:07:24.000000 pwforecast-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 04:42:06.355281 pwforecast-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-09 04:41:53.000000 pwforecast-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-07-09 04:42:06.351281 pwforecast-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-07-09 04:41:53.000000 pwforecast-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 04:42:06.351281 pwforecast-1.1.2/pwforecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-07-09 04:42:06.000000 pwforecast-1.1.2/pwforecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-09 04:42:06.000000 pwforecast-1.1.2/pwforecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 04:42:06.000000 pwforecast-1.1.2/pwforecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-09 04:42:06.000000 pwforecast-1.1.2/pwforecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-09 04:42:06.000000 pwforecast-1.1.2/pwforecast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16738 2023-07-09 04:41:53.000000 pwforecast-1.1.2/pwforecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 04:42:06.355281 pwforecast-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-09 04:41:53.000000 pwforecast-1.1.2/setup.py
```

### Comparing `pwforecast-1.1.1/LICENSE` & `pwforecast-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pwforecast-1.1.1/PKG-INFO` & `pwforecast-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: pwforecast
-Version: 1.1.1
+Version: 1.1.2
 Summary: A Python module to charge/discharge Powerwall based on solar forecast and peak/off peak tariffs.
 Home-page: https://github.com/timhawker/pwforecast
 Author: Tim Hawker
+License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## PwForecast
 
 A Python module to charge/discharge Powerwall based on solar forecast and peak/off-peak tariffs.
```

### Comparing `pwforecast-1.1.1/README.md` & `pwforecast-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pwforecast-1.1.1/pwforecast/__init__.py` & `pwforecast-1.1.2/pwforecast.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""
+A Python module to charge/discharge Powerwall based on solar forecast and peak/off-peak tariffs.
+
+"""
+
+# Author: Tim Hawker
+
 import time
 import tzlocal
 import datetime
 import requests
 import pprint
 from dateutil import parser
```

### Comparing `pwforecast-1.1.1/pwforecast.egg-info/PKG-INFO` & `pwforecast-1.1.2/pwforecast.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: pwforecast
-Version: 1.1.1
+Version: 1.1.2
 Summary: A Python module to charge/discharge Powerwall based on solar forecast and peak/off peak tariffs.
 Home-page: https://github.com/timhawker/pwforecast
 Author: Tim Hawker
+License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## PwForecast
 
 A Python module to charge/discharge Powerwall based on solar forecast and peak/off-peak tariffs.
```

### Comparing `pwforecast-1.1.1/setup.py` & `pwforecast-1.1.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import setuptools
 from pathlib import Path
 
-this_directory = Path(__file__).parent
-
 # read the contents of README file
+this_directory = Path(__file__).parent
 readme = (this_directory / 'README.md').read_text()
 
 setuptools.setup(
     name='pwforecast',
-    version='1.1.1',
+    version='1.1.2',
     author='Tim Hawker',
-    description='A Python module to charge/discharge Powerwall based on solar forecast and peak/off peak tariffs.',
+    license='MIT',
     url='https://github.com/timhawker/pwforecast',
+    description='A Python module to charge/discharge Powerwall based on solar forecast and peak/off peak tariffs.',
     long_description_content_type='text/markdown',
     long_description=readme,
-    packages=['pwforecast'],
+    py_modules=['pwforecast'],
     install_requires=['tzlocal', 'requests', 'python-dateutil', 'TeslaPy']
 )
```

