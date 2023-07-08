# Comparing `tmp/FiveMCipherFinder-2.0.0.tar.gz` & `tmp/FiveMCipherFinder-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FiveMCipherFinder-2.0.0.tar", last modified: Sat Jul  8 12:18:22 2023, max compression
+gzip compressed data, was "FiveMCipherFinder-2.1.0.tar", last modified: Sat Jul  8 22:19:33 2023, max compression
```

## Comparing `FiveMCipherFinder-2.0.0.tar` & `FiveMCipherFinder-2.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:18:22.530048 FiveMCipherFinder-2.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:18:22.530048 FiveMCipherFinder-2.0.0/FiveMCipherFinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-08 12:18:22.000000 FiveMCipherFinder-2.0.0/FiveMCipherFinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-08 12:18:22.000000 FiveMCipherFinder-2.0.0/FiveMCipherFinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 12:18:22.000000 FiveMCipherFinder-2.0.0/FiveMCipherFinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-08 12:18:22.000000 FiveMCipherFinder-2.0.0/FiveMCipherFinder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-08 12:18:22.000000 FiveMCipherFinder-2.0.0/FiveMCipherFinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-08 12:18:22.000000 FiveMCipherFinder-2.0.0/FiveMCipherFinder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-08 12:18:10.000000 FiveMCipherFinder-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-08 12:18:22.530048 FiveMCipherFinder-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-08 12:18:10.000000 FiveMCipherFinder-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:18:22.530048 FiveMCipherFinder-2.0.0/cipherFinder/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-08 12:18:10.000000 FiveMCipherFinder-2.0.0/cipherFinder/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6840 2023-07-08 12:18:10.000000 FiveMCipherFinder-2.0.0/cipherFinder/finder.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-08 12:18:10.000000 FiveMCipherFinder-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-08 12:18:22.530048 FiveMCipherFinder-2.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-07-08 12:18:10.000000 FiveMCipherFinder-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:19:33.521449 FiveMCipherFinder-2.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:19:33.521449 FiveMCipherFinder-2.1.0/FiveMCipherFinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-08 22:19:33.000000 FiveMCipherFinder-2.1.0/FiveMCipherFinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-08 22:19:33.000000 FiveMCipherFinder-2.1.0/FiveMCipherFinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 22:19:33.000000 FiveMCipherFinder-2.1.0/FiveMCipherFinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-08 22:19:33.000000 FiveMCipherFinder-2.1.0/FiveMCipherFinder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-08 22:19:33.000000 FiveMCipherFinder-2.1.0/FiveMCipherFinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-08 22:19:33.000000 FiveMCipherFinder-2.1.0/FiveMCipherFinder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-08 22:19:23.000000 FiveMCipherFinder-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-08 22:19:33.521449 FiveMCipherFinder-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-08 22:19:23.000000 FiveMCipherFinder-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:19:33.521449 FiveMCipherFinder-2.1.0/cipherFinder/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-08 22:19:23.000000 FiveMCipherFinder-2.1.0/cipherFinder/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6929 2023-07-08 22:19:23.000000 FiveMCipherFinder-2.1.0/cipherFinder/finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-08 22:19:23.000000 FiveMCipherFinder-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-08 22:19:33.521449 FiveMCipherFinder-2.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-07-08 22:19:23.000000 FiveMCipherFinder-2.1.0/setup.py
```

### Comparing `FiveMCipherFinder-2.0.0/FiveMCipherFinder.egg-info/PKG-INFO` & `FiveMCipherFinder-2.1.0/FiveMCipherFinder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: FiveMCipherFinder
-Version: 2.0.0
+Version: 2.1.0
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
 
-# FivemCipherFinder (v2.0.0)
+# FivemCipherFinder (v2.1.0)
 <div align="center">
   <h2> Visitors </h2>
 <img src="https://profile-counter.glitch.me/FivemCipherFinder/count.svg" />
 </div>
 
 [![Pylint](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml/badge.svg)](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml)
 
@@ -46,15 +46,15 @@
 `--v2` flag behind the command like `find-cipher . --v2 cars,mlos`.
 
 As you can see in the last example, you can exclude Directories so can prevent false-positives like `\[cars\],\[mlos\],easy-admin` but make sure you add `\` before curly and square brackets, otherwise your terminal will throw an error.
 
 The script logs found Cipher in a file names `CipherLog-HH-MM-SS.txt` so can easily find your log files.
 
 ## Install instructions for Python
-Py-Version: 3.7 and above
+Py-Version: 3.8 and above
 
 run `pip install FivemCipherFinder` or download the latest release and unpack it.
 
 ### Troubleshooting
 
 Should the installation with pip fail with the error code `externally-managed-environment`, add `--break-system-packages`. Pip changed something in their internals in the newer versions.
```

### Comparing `FiveMCipherFinder-2.0.0/LICENSE` & `FiveMCipherFinder-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FiveMCipherFinder-2.0.0/PKG-INFO` & `FiveMCipherFinder-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: FiveMCipherFinder
-Version: 2.0.0
+Version: 2.1.0
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
 
-# FivemCipherFinder (v2.0.0)
+# FivemCipherFinder (v2.1.0)
 <div align="center">
   <h2> Visitors </h2>
 <img src="https://profile-counter.glitch.me/FivemCipherFinder/count.svg" />
 </div>
 
 [![Pylint](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml/badge.svg)](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml)
 
@@ -46,15 +46,15 @@
 `--v2` flag behind the command like `find-cipher . --v2 cars,mlos`.
 
 As you can see in the last example, you can exclude Directories so can prevent false-positives like `\[cars\],\[mlos\],easy-admin` but make sure you add `\` before curly and square brackets, otherwise your terminal will throw an error.
 
 The script logs found Cipher in a file names `CipherLog-HH-MM-SS.txt` so can easily find your log files.
 
 ## Install instructions for Python
-Py-Version: 3.7 and above
+Py-Version: 3.8 and above
 
 run `pip install FivemCipherFinder` or download the latest release and unpack it.
 
 ### Troubleshooting
 
 Should the installation with pip fail with the error code `externally-managed-environment`, add `--break-system-packages`. Pip changed something in their internals in the newer versions.
```

### Comparing `FiveMCipherFinder-2.0.0/README.md` & `FiveMCipherFinder-2.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# FivemCipherFinder (v2.0.0)
+# FivemCipherFinder (v2.1.0)
 <div align="center">
   <h2> Visitors </h2>
 <img src="https://profile-counter.glitch.me/FivemCipherFinder/count.svg" />
 </div>
 
 [![Pylint](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml/badge.svg)](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml)
 
@@ -29,15 +29,15 @@
 `--v2` flag behind the command like `find-cipher . --v2 cars,mlos`.
 
 As you can see in the last example, you can exclude Directories so can prevent false-positives like `\[cars\],\[mlos\],easy-admin` but make sure you add `\` before curly and square brackets, otherwise your terminal will throw an error.
 
 The script logs found Cipher in a file names `CipherLog-HH-MM-SS.txt` so can easily find your log files.
 
 ## Install instructions for Python
-Py-Version: 3.7 and above
+Py-Version: 3.8 and above
 
 run `pip install FivemCipherFinder` or download the latest release and unpack it.
 
 ### Troubleshooting
 
 Should the installation with pip fail with the error code `externally-managed-environment`, add `--break-system-packages`. Pip changed something in their internals in the newer versions.
```

### Comparing `FiveMCipherFinder-2.0.0/cipherFinder/finder.py` & `FiveMCipherFinder-2.1.0/cipherFinder/finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,15 +190,15 @@
         print(main.__doc__)
         return 0
 
     pattern = ''.join([(i.replace(',', ')|(') if '--' not in i else '') for i in sys.argv[2:]])
     local_path = '.'
     count = 0 
 
-    get_big_model_file()  # sure there are other ways, but python is down python stuff.
+    get_big_model_file()  # sure there are other ways, but python is doing python stuff.
 
     if len(sys.argv) > 1 and '--' not in sys.argv[1]:
         local_path = sys.argv[1]
     
     for d, _, files in os.walk(local_path):
         if pattern and re.findall(f'{"(" + pattern + ")"}', 
                                   fr'{d}'.format(d=d), re.MULTILINE and re.IGNORECASE):
@@ -211,14 +211,19 @@
             _, count = check_file(d, file, count)
     # Write log
     
     red = green = white = ''
 
     if 'linux' in platform.platform().lower():
         white, red, green = COLORS
+    
+    try:
+        os.remove('big.model')
+    except FileNotFoundError:
+        pass
 
     if log:
         return write_log_file(white=white, red=red, count=count)
 
     print(f'{green}Nice! There were no Cipher\'s found!{white}')
 
     return 0
```

### Comparing `FiveMCipherFinder-2.0.0/setup.cfg` & `FiveMCipherFinder-2.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = FiveMCipherFinder
-version = 2.0.0
+version = 2.1.0
 description = Finds Cipher in lua scripts.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 author = exersalza
 url = https://github.com/exersalza/FivemCipherFinder
 project_urls =
```

