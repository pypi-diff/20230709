# Comparing `tmp/scriptime-0.1.4.tar.gz` & `tmp/scriptime-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scriptime-0.1.4.tar", last modified: Thu Jul  6 20:17:23 2023, max compression
+gzip compressed data, was "scriptime-0.1.5.tar", last modified: Sun Jul  9 02:59:46 2023, max compression
```

## Comparing `scriptime-0.1.4.tar` & `scriptime-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-06 20:17:23.630296 scriptime-0.1.4/
--rw-r--r--   0 jakestrasler   (501) staff       (20)       45 2023-07-06 20:17:09.000000 scriptime-0.1.4/MANIFEST.in
--rw-r--r--   0 jakestrasler   (501) staff       (20)     5248 2023-07-06 20:17:23.630169 scriptime-0.1.4/PKG-INFO
--rw-r--r--   0 jakestrasler   (501) staff       (20)     4960 2023-07-06 20:16:49.000000 scriptime-0.1.4/README.md
-drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-06 20:17:23.629179 scriptime-0.1.4/scriptime/
--rw-r--r--   0 jakestrasler   (501) staff       (20)       45 2023-07-06 00:08:59.000000 scriptime-0.1.4/scriptime/__init__.py
--rw-r--r--   0 jakestrasler   (501) staff       (20)   701148 2023-07-05 22:10:39.000000 scriptime-0.1.4/scriptime/alert.wav
--rw-r--r--   0 jakestrasler   (501) staff       (20)     9874 2023-07-06 19:55:45.000000 scriptime-0.1.4/scriptime/main.py
-drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-06 20:17:23.629965 scriptime-0.1.4/scriptime.egg-info/
--rw-r--r--   0 jakestrasler   (501) staff       (20)     5248 2023-07-06 20:17:23.000000 scriptime-0.1.4/scriptime.egg-info/PKG-INFO
--rw-r--r--   0 jakestrasler   (501) staff       (20)      254 2023-07-06 20:17:23.000000 scriptime-0.1.4/scriptime.egg-info/SOURCES.txt
--rw-r--r--   0 jakestrasler   (501) staff       (20)        1 2023-07-06 20:17:23.000000 scriptime-0.1.4/scriptime.egg-info/dependency_links.txt
--rw-r--r--   0 jakestrasler   (501) staff       (20)       30 2023-07-06 20:17:23.000000 scriptime-0.1.4/scriptime.egg-info/requires.txt
--rw-r--r--   0 jakestrasler   (501) staff       (20)       10 2023-07-06 20:17:23.000000 scriptime-0.1.4/scriptime.egg-info/top_level.txt
--rw-r--r--   0 jakestrasler   (501) staff       (20)       38 2023-07-06 20:17:23.630333 scriptime-0.1.4/setup.cfg
--rw-r--r--   0 jakestrasler   (501) staff       (20)      694 2023-07-06 20:17:14.000000 scriptime-0.1.4/setup.py
+drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-09 02:59:46.252062 scriptime-0.1.5/
+-rw-r--r--   0 jakestrasler   (501) staff       (20)     1087 2023-07-09 02:56:28.000000 scriptime-0.1.5/LICENSE
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       45 2023-07-06 20:17:09.000000 scriptime-0.1.5/MANIFEST.in
+-rw-r--r--   0 jakestrasler   (501) staff       (20)     5401 2023-07-09 02:59:46.251898 scriptime-0.1.5/PKG-INFO
+-rw-r--r--   0 jakestrasler   (501) staff       (20)     5091 2023-07-09 02:59:26.000000 scriptime-0.1.5/README.md
+drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-09 02:59:46.250315 scriptime-0.1.5/scriptime/
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       45 2023-07-06 00:08:59.000000 scriptime-0.1.5/scriptime/__init__.py
+-rw-r--r--   0 jakestrasler   (501) staff       (20)   701148 2023-07-05 22:10:39.000000 scriptime-0.1.5/scriptime/alert.wav
+-rw-r--r--   0 jakestrasler   (501) staff       (20)     9874 2023-07-06 19:55:45.000000 scriptime-0.1.5/scriptime/main.py
+drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-09 02:59:46.251640 scriptime-0.1.5/scriptime.egg-info/
+-rw-r--r--   0 jakestrasler   (501) staff       (20)     5401 2023-07-09 02:59:46.000000 scriptime-0.1.5/scriptime.egg-info/PKG-INFO
+-rw-r--r--   0 jakestrasler   (501) staff       (20)      262 2023-07-09 02:59:46.000000 scriptime-0.1.5/scriptime.egg-info/SOURCES.txt
+-rw-r--r--   0 jakestrasler   (501) staff       (20)        1 2023-07-09 02:59:46.000000 scriptime-0.1.5/scriptime.egg-info/dependency_links.txt
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       30 2023-07-09 02:59:46.000000 scriptime-0.1.5/scriptime.egg-info/requires.txt
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       10 2023-07-09 02:59:46.000000 scriptime-0.1.5/scriptime.egg-info/top_level.txt
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       38 2023-07-09 02:59:46.252110 scriptime-0.1.5/setup.cfg
+-rw-r--r--   0 jakestrasler   (501) staff       (20)      694 2023-07-09 02:59:44.000000 scriptime-0.1.5/setup.py
```

### Comparing `scriptime-0.1.4/PKG-INFO` & `scriptime-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: scriptime
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python library to notify when a script has finished running and providing insights such as run time, CPU and RAM usage, and more.
 Author: Jake Strasler
 Author-email: jstr36@gmail.com
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # scriptime
 Python library to notify when a script has finished running and providing insights such as run time, CPU and RAM usage, and more.
 
 
 - [scriptime](#scriptime)
   - [About](#about)
   - [Getting Started](#getting-started)
   - [Using scriptimer](#using-scriptimer)
   - [Output](#output)
+  - [Links](#links)
 
 ## About
 
 This project will send you an email or text message notifying you when a script has completed running. Configurable thorugh a config file, environment variables, or hardcoding the email credentials, this project has little overhead to get started.
 
 ## Getting Started
 
@@ -147,7 +149,12 @@
 Python Version: 3.11.4
 
 Packages Used:
 Package: numpy, Version: 1.24.2
 Package: scikit-learn, Version: 1.2.2
 ...
 ```
+
+## Links
+
+ - Source code: https://github.com/straslerj/scriptime
+ - PyPI: https://pypi.org/project/scriptime/
```

### Comparing `scriptime-0.1.4/README.md` & `scriptime-0.1.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 
 - [scriptime](#scriptime)
   - [About](#about)
   - [Getting Started](#getting-started)
   - [Using scriptimer](#using-scriptimer)
   - [Output](#output)
+  - [Links](#links)
 
 ## About
 
 This project will send you an email or text message notifying you when a script has completed running. Configurable thorugh a config file, environment variables, or hardcoding the email credentials, this project has little overhead to get started.
 
 ## Getting Started
 
@@ -139,7 +140,12 @@
 Python Version: 3.11.4
 
 Packages Used:
 Package: numpy, Version: 1.24.2
 Package: scikit-learn, Version: 1.2.2
 ...
 ```
+
+## Links
+
+ - Source code: https://github.com/straslerj/scriptime
+ - PyPI: https://pypi.org/project/scriptime/
```

### Comparing `scriptime-0.1.4/scriptime/alert.wav` & `scriptime-0.1.5/scriptime/alert.wav`

 * *Files identical despite different names*

### Comparing `scriptime-0.1.4/scriptime/main.py` & `scriptime-0.1.5/scriptime/main.py`

 * *Files identical despite different names*

### Comparing `scriptime-0.1.4/scriptime.egg-info/PKG-INFO` & `scriptime-0.1.5/scriptime.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: scriptime
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python library to notify when a script has finished running and providing insights such as run time, CPU and RAM usage, and more.
 Author: Jake Strasler
 Author-email: jstr36@gmail.com
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # scriptime
 Python library to notify when a script has finished running and providing insights such as run time, CPU and RAM usage, and more.
 
 
 - [scriptime](#scriptime)
   - [About](#about)
   - [Getting Started](#getting-started)
   - [Using scriptimer](#using-scriptimer)
   - [Output](#output)
+  - [Links](#links)
 
 ## About
 
 This project will send you an email or text message notifying you when a script has completed running. Configurable thorugh a config file, environment variables, or hardcoding the email credentials, this project has little overhead to get started.
 
 ## Getting Started
 
@@ -147,7 +149,12 @@
 Python Version: 3.11.4
 
 Packages Used:
 Package: numpy, Version: 1.24.2
 Package: scikit-learn, Version: 1.2.2
 ...
 ```
+
+## Links
+
+ - Source code: https://github.com/straslerj/scriptime
+ - PyPI: https://pypi.org/project/scriptime/
```

### Comparing `scriptime-0.1.4/setup.py` & `scriptime-0.1.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="scriptime",
-    version="0.1.4",
+    version="0.1.5",
     author="Jake Strasler",
     author_email="jstr36@gmail.com",
     description="A Python library to notify when a script has finished running and providing insights such as run time, CPU and RAM usage, and more.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["scriptime"],
     package_data={"scriptime": ["scriptime/alert.wav"]},
```

