# Comparing `tmp/FiveMCipherFinder-2.1.0.tar.gz` & `tmp/FiveMCipherFinder-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FiveMCipherFinder-2.1.0.tar", last modified: Sat Jul  8 22:19:33 2023, max compression
+gzip compressed data, was "FiveMCipherFinder-2.2.0.tar", last modified: Sun Jul  9 07:11:36 2023, max compression
```

## Comparing `FiveMCipherFinder-2.1.0.tar` & `FiveMCipherFinder-2.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:19:33.521449 FiveMCipherFinder-2.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:19:33.521449 FiveMCipherFinder-2.1.0/FiveMCipherFinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-08 22:19:33.000000 FiveMCipherFinder-2.1.0/FiveMCipherFinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-08 22:19:33.000000 FiveMCipherFinder-2.1.0/FiveMCipherFinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 22:19:33.000000 FiveMCipherFinder-2.1.0/FiveMCipherFinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-08 22:19:33.000000 FiveMCipherFinder-2.1.0/FiveMCipherFinder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-08 22:19:33.000000 FiveMCipherFinder-2.1.0/FiveMCipherFinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-08 22:19:33.000000 FiveMCipherFinder-2.1.0/FiveMCipherFinder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-08 22:19:23.000000 FiveMCipherFinder-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-08 22:19:33.521449 FiveMCipherFinder-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-08 22:19:23.000000 FiveMCipherFinder-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:19:33.521449 FiveMCipherFinder-2.1.0/cipherFinder/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-08 22:19:23.000000 FiveMCipherFinder-2.1.0/cipherFinder/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6929 2023-07-08 22:19:23.000000 FiveMCipherFinder-2.1.0/cipherFinder/finder.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-08 22:19:23.000000 FiveMCipherFinder-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-08 22:19:33.521449 FiveMCipherFinder-2.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-07-08 22:19:23.000000 FiveMCipherFinder-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:11:36.193485 FiveMCipherFinder-2.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:11:36.193485 FiveMCipherFinder-2.2.0/FiveMCipherFinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-09 07:11:36.000000 FiveMCipherFinder-2.2.0/FiveMCipherFinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-09 07:11:36.000000 FiveMCipherFinder-2.2.0/FiveMCipherFinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 07:11:36.000000 FiveMCipherFinder-2.2.0/FiveMCipherFinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-09 07:11:36.000000 FiveMCipherFinder-2.2.0/FiveMCipherFinder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-09 07:11:36.000000 FiveMCipherFinder-2.2.0/FiveMCipherFinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-09 07:11:36.000000 FiveMCipherFinder-2.2.0/FiveMCipherFinder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-09 07:11:23.000000 FiveMCipherFinder-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-09 07:11:36.193485 FiveMCipherFinder-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-09 07:11:23.000000 FiveMCipherFinder-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:11:36.193485 FiveMCipherFinder-2.2.0/cipherFinder/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-09 07:11:23.000000 FiveMCipherFinder-2.2.0/cipherFinder/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6929 2023-07-09 07:11:23.000000 FiveMCipherFinder-2.2.0/cipherFinder/finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-09 07:11:23.000000 FiveMCipherFinder-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-09 07:11:36.193485 FiveMCipherFinder-2.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-07-09 07:11:23.000000 FiveMCipherFinder-2.2.0/setup.py
```

### Comparing `FiveMCipherFinder-2.1.0/FiveMCipherFinder.egg-info/PKG-INFO` & `FiveMCipherFinder-2.2.0/FiveMCipherFinder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: FiveMCipherFinder
-Version: 2.1.0
+Version: 2.2.0
 Summary: Finds Cipher in lua scripts.
 Home-page: https://github.com/exersalza/FivemCipherFinder
 Author: exersalza
 License: MIT
 Project-URL: Source, https://github.com/exersalza/FivemCipherFinder
 Project-URL: Issues, https://github.com/exersalza/FivemCipherFinder/issues
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# FivemCipherFinder (v2.1.0)
+# FivemCipherFinder (v2.2.0)
 <div align="center">
   <h2> Visitors </h2>
 <img src="https://profile-counter.glitch.me/FivemCipherFinder/count.svg" />
 </div>
 
 [![Pylint](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml/badge.svg)](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml)
```

### Comparing `FiveMCipherFinder-2.1.0/LICENSE` & `FiveMCipherFinder-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FiveMCipherFinder-2.1.0/PKG-INFO` & `FiveMCipherFinder-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: FiveMCipherFinder
-Version: 2.1.0
+Version: 2.2.0
 Summary: Finds Cipher in lua scripts.
 Home-page: https://github.com/exersalza/FivemCipherFinder
 Author: exersalza
 License: MIT
 Project-URL: Source, https://github.com/exersalza/FivemCipherFinder
 Project-URL: Issues, https://github.com/exersalza/FivemCipherFinder/issues
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# FivemCipherFinder (v2.1.0)
+# FivemCipherFinder (v2.2.0)
 <div align="center">
   <h2> Visitors </h2>
 <img src="https://profile-counter.glitch.me/FivemCipherFinder/count.svg" />
 </div>
 
 [![Pylint](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml/badge.svg)](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml)
```

### Comparing `FiveMCipherFinder-2.1.0/README.md` & `FiveMCipherFinder-2.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# FivemCipherFinder (v2.1.0)
+# FivemCipherFinder (v2.2.0)
 <div align="center">
   <h2> Visitors </h2>
 <img src="https://profile-counter.glitch.me/FivemCipherFinder/count.svg" />
 </div>
 
 [![Pylint](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml/badge.svg)](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml)
```

### Comparing `FiveMCipherFinder-2.1.0/cipherFinder/finder.py` & `FiveMCipherFinder-2.2.0/cipherFinder/finder.py`

 * *Files identical despite different names*

### Comparing `FiveMCipherFinder-2.1.0/setup.cfg` & `FiveMCipherFinder-2.2.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = FiveMCipherFinder
-version = 2.1.0
+version = 2.2.0
 description = Finds Cipher in lua scripts.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 author = exersalza
 url = https://github.com/exersalza/FivemCipherFinder
 project_urls = 
@@ -16,14 +16,15 @@
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Topic :: Software Development
 
 [options]
 install_requires = 
 	gibberish_detector
+	requests
 packages = cipherFinder
 
 [options.entry_points]
 console_scripts = 
 	find-cipher = cipherFinder:main
 
 [egg_info]
```

