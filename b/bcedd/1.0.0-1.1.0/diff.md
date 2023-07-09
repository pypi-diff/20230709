# Comparing `tmp/bcedd-1.0.0.tar.gz` & `tmp/bcedd-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcedd-1.0.0.tar", last modified: Thu Apr 13 11:00:08 2023, max compression
+gzip compressed data, was "bcedd-1.1.0.tar", last modified: Sun Jul  9 13:00:59 2023, max compression
```

## Comparing `bcedd-1.0.0.tar` & `bcedd-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-04-13 11:00:08.004487 bcedd-1.0.0/
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1071 2023-04-13 10:23:09.000000 bcedd-1.0.0/LICENSE
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       35 2023-04-13 10:49:04.000000 bcedd-1.0.0/MANIFEST.in
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2672 2023-04-13 11:00:08.004487 bcedd-1.0.0/PKG-INFO
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2301 2023-04-13 10:56:31.000000 bcedd-1.0.0/README.md
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      200 2023-04-13 09:59:09.000000 bcedd-1.0.0/pyproject.toml
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       38 2023-04-13 11:00:08.004487 bcedd-1.0.0/setup.cfg
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      989 2023-04-13 10:20:57.000000 bcedd-1.0.0/setup.py
-drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-04-13 11:00:08.001154 bcedd-1.0.0/src/
-drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-04-13 11:00:08.001154 bcedd-1.0.0/src/bcedd/
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       55 2023-04-13 10:01:54.000000 bcedd-1.0.0/src/bcedd/__init__.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2808 2023-04-13 10:31:10.000000 bcedd-1.0.0/src/bcedd/__main__.py
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     5470 2023-04-13 10:49:42.000000 bcedd-1.0.0/src/bcedd/event_data.py
-drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-04-13 11:00:08.004487 bcedd-1.0.0/src/bcedd/files/
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)        5 2023-04-13 09:59:09.000000 bcedd-1.0.0/src/bcedd/files/version.txt
-drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-04-13 11:00:08.001154 bcedd-1.0.0/src/bcedd.egg-info/
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2672 2023-04-13 11:00:07.000000 bcedd-1.0.0/src/bcedd.egg-info/PKG-INFO
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      313 2023-04-13 11:00:08.000000 bcedd-1.0.0/src/bcedd.egg-info/SOURCES.txt
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)        1 2023-04-13 11:00:07.000000 bcedd-1.0.0/src/bcedd.egg-info/dependency_links.txt
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       38 2023-04-13 11:00:07.000000 bcedd-1.0.0/src/bcedd.egg-info/requires.txt
--rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)        6 2023-04-13 11:00:07.000000 bcedd-1.0.0/src/bcedd.egg-info/top_level.txt
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-07-09 13:00:59.068068 bcedd-1.1.0/
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1071 2023-04-13 10:23:09.000000 bcedd-1.1.0/LICENSE
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       35 2023-04-13 10:49:04.000000 bcedd-1.1.0/MANIFEST.in
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2813 2023-07-09 13:00:59.068068 bcedd-1.1.0/PKG-INFO
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2466 2023-07-09 12:58:33.000000 bcedd-1.1.0/README.md
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      200 2023-04-13 09:59:09.000000 bcedd-1.1.0/pyproject.toml
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       38 2023-07-09 13:00:59.068068 bcedd-1.1.0/setup.cfg
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      844 2023-07-09 12:49:41.000000 bcedd-1.1.0/setup.py
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-07-09 13:00:59.064735 bcedd-1.1.0/src/
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-07-09 13:00:59.064735 bcedd-1.1.0/src/bcedd/
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      204 2023-07-09 12:39:39.000000 bcedd-1.1.0/src/bcedd/__init__.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3128 2023-07-09 12:57:29.000000 bcedd-1.1.0/src/bcedd/__main__.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2614 2023-07-09 12:34:56.000000 bcedd-1.1.0/src/bcedd/country_code.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3576 2023-07-09 12:36:40.000000 bcedd-1.1.0/src/bcedd/crypto.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     9742 2023-07-09 12:55:30.000000 bcedd-1.1.0/src/bcedd/event_data.py
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-07-09 13:00:59.068068 bcedd-1.1.0/src/bcedd/files/
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)        5 2023-07-09 12:53:37.000000 bcedd-1.1.0/src/bcedd/files/version.txt
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     5377 2023-07-09 12:35:45.000000 bcedd-1.1.0/src/bcedd/game_version.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      986 2023-07-09 12:39:26.000000 bcedd-1.1.0/src/bcedd/json_file.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1229 2023-07-09 12:47:00.000000 bcedd-1.1.0/src/bcedd/request.py
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-07-09 13:00:59.068068 bcedd-1.1.0/src/bcedd.egg-info/
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2813 2023-07-09 13:00:59.000000 bcedd-1.1.0/src/bcedd.egg-info/PKG-INFO
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      429 2023-07-09 13:00:59.000000 bcedd-1.1.0/src/bcedd.egg-info/SOURCES.txt
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)        1 2023-07-09 13:00:59.000000 bcedd-1.1.0/src/bcedd.egg-info/dependency_links.txt
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)        9 2023-07-09 13:00:59.000000 bcedd-1.1.0/src/bcedd.egg-info/requires.txt
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)        6 2023-07-09 13:00:59.000000 bcedd-1.1.0/src/bcedd.egg-info/top_level.txt
```

### Comparing `bcedd-1.0.0/LICENSE` & `bcedd-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bcedd-1.0.0/PKG-INFO` & `bcedd-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 Metadata-Version: 2.1
 Name: bcedd
-Version: 1.0.0
+Version: 1.1.0
 Home-page: https://github.com/fieryhenry/bcedd
 Author: fieryhenry
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: testing
 License-File: LICENSE
 
 # Battle Cats Event Data Downloader
 
 The Battle Cats Event Data Downloader (BCEDD) is a tool made for downloading battle cats event data such as gatya data and sale data.
 
 [PyPI](https://pypi.org/project/bcedd)
 
 ## Credits
 
-- The [PackPack Discord Bot](https://github.com/battlecatsultimate/PackPack) for the general cryptography algorithm needed
+- The [PackPack Discord Bot](https://github.com/battlecatsultimate/PackPack) for the old method of downloading data (aws stuff)
 
 ## How To Use
 
 ### Prerequisites
 
 - [Python](https://www.python.org/downloads/) for running and installing the tool
 
 Run the following commands in command prompt or another terminal to install the tool - If you are not using windows you will need to use `python` or `python3` instead of `py`
 
 ### Installation
 
+To install / update the tool run the following command:
+
 ```bash
 py -m pip install -U bcedd
 ```
 
 If you get an error saying `No module named pip` then run
 
 ```bash
@@ -69,14 +70,20 @@
 
 ```bash
 py -m bcedd -o "Event Data"
 ```
 
 This will save all 3 en files to a folder called "Event Data" in the current working directory (use the `cd` command to change that)
 
+If you want to use the old method of downloading data then use `--old`
+
+```bash
+py -m bcedd --old
+```
+
 ## Install From Source
 
 If you want the latest features and don't want to wait for a release then you can install the tool from the github directly.
 
 1. Download [Git](https://git-scm.com/downloads)
 2. Run the following commands: (You may have to replace `py` with `python` or `python3`)
```

### Comparing `bcedd-1.0.0/README.md` & `bcedd-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,26 +2,28 @@
 
 The Battle Cats Event Data Downloader (BCEDD) is a tool made for downloading battle cats event data such as gatya data and sale data.
 
 [PyPI](https://pypi.org/project/bcedd)
 
 ## Credits
 
-- The [PackPack Discord Bot](https://github.com/battlecatsultimate/PackPack) for the general cryptography algorithm needed
+- The [PackPack Discord Bot](https://github.com/battlecatsultimate/PackPack) for the old method of downloading data (aws stuff)
 
 ## How To Use
 
 ### Prerequisites
 
 - [Python](https://www.python.org/downloads/) for running and installing the tool
 
 Run the following commands in command prompt or another terminal to install the tool - If you are not using windows you will need to use `python` or `python3` instead of `py`
 
 ### Installation
 
+To install / update the tool run the following command:
+
 ```bash
 py -m pip install -U bcedd
 ```
 
 If you get an error saying `No module named pip` then run
 
 ```bash
@@ -56,14 +58,20 @@
 
 ```bash
 py -m bcedd -o "Event Data"
 ```
 
 This will save all 3 en files to a folder called "Event Data" in the current working directory (use the `cd` command to change that)
 
+If you want to use the old method of downloading data then use `--old`
+
+```bash
+py -m bcedd --old
+```
+
 ## Install From Source
 
 If you want the latest features and don't want to wait for a release then you can install the tool from the github directly.
 
 1. Download [Git](https://git-scm.com/downloads)
 2. Run the following commands: (You may have to replace `py` with `python` or `python3`)
```

### Comparing `bcedd-1.0.0/src/bcedd/__main__.py` & `bcedd-1.1.0/src/bcedd/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 import os
 import tkinter as tk
 from tkinter import filedialog
 from typing import Optional
 
-from bcedd import event_data
+from bcedd import event_data, game_version, country_code
 
 
 def save_file(name: str, data: bytes):
     """Saves a file to the user's computer using a dialog.
 
     Args:
         name (str): Name of the file.
@@ -33,15 +33,15 @@
     """
     file_path = os.path.join(output, name)
     os.makedirs(os.path.dirname(file_path), exist_ok=True)
     with open(file_path, "wb") as f:
         f.write(data)
 
 
-def load_args() -> tuple[str, list[str], Optional[str]]:
+def load_args() -> tuple[str, list[str], Optional[str], bool]:
     """Loads the arguments from the command line.
 
     Returns:
         tuple[str, list[str], Optional[str]]: Country code, files, and output folder.
     """
     parser = argparse.ArgumentParser()
     parser.add_argument(
@@ -61,43 +61,52 @@
     )
     parser.add_argument(
         "-o",
         "--output",
         help="Output folder",
         default=None,
     )
+    parser.add_argument(
+        "--old",
+        help="Use the old event data domain and method (aws)",
+        action="store_true",
+    )
 
     args = parser.parse_args()
 
-    country_code: str = args.country_code
+    cc: str = args.country_code
     files: list[str] = args.files
     output: Optional[str] = args.output
+    use_old: bool = args.old
 
-    return country_code, files, output
+    return cc, files, output, use_old
 
 
-def download(country_code: str, files: list[str], output: Optional[str]):
+def download(cc: str, files: list[str], output: Optional[str], use_old: bool):
     """Downloads the files.
 
     Args:
         country_code (str): Country code to download the files for.
         files (list[str]): Files to download.
         output (Optional[str]): Output folder.
     """
+    gv = game_version.GameVersion.from_string("12.4.0")  # doesn't matter
     for file in files:
-        file_name = country_code + "_" + file
+        file_name = cc + "_" + file
         print(f"Downloading {file_name}...")
-        ed = event_data.EventData(file, country_code)
+        ed = event_data.EventData(
+            file, country_code.CountryCode.from_code(cc), gv, use_old
+        )
         if output is not None:
             save_file_no_dialog(file_name, ed.make_request().content, output)
         else:
             save_file(file_name, ed.make_request().content)
 
 
 def main():
     """Main function."""
-    country_code, files, output = load_args()
-    download(country_code, files, output)
+    cc, files, output, use_old = load_args()
+    download(cc, files, output, use_old)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `bcedd-1.0.0/src/bcedd.egg-info/PKG-INFO` & `bcedd-1.1.0/src/bcedd.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 Metadata-Version: 2.1
 Name: bcedd
-Version: 1.0.0
+Version: 1.1.0
 Home-page: https://github.com/fieryhenry/bcedd
 Author: fieryhenry
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: testing
 License-File: LICENSE
 
 # Battle Cats Event Data Downloader
 
 The Battle Cats Event Data Downloader (BCEDD) is a tool made for downloading battle cats event data such as gatya data and sale data.
 
 [PyPI](https://pypi.org/project/bcedd)
 
 ## Credits
 
-- The [PackPack Discord Bot](https://github.com/battlecatsultimate/PackPack) for the general cryptography algorithm needed
+- The [PackPack Discord Bot](https://github.com/battlecatsultimate/PackPack) for the old method of downloading data (aws stuff)
 
 ## How To Use
 
 ### Prerequisites
 
 - [Python](https://www.python.org/downloads/) for running and installing the tool
 
 Run the following commands in command prompt or another terminal to install the tool - If you are not using windows you will need to use `python` or `python3` instead of `py`
 
 ### Installation
 
+To install / update the tool run the following command:
+
 ```bash
 py -m pip install -U bcedd
 ```
 
 If you get an error saying `No module named pip` then run
 
 ```bash
@@ -69,14 +70,20 @@
 
 ```bash
 py -m bcedd -o "Event Data"
 ```
 
 This will save all 3 en files to a folder called "Event Data" in the current working directory (use the `cd` command to change that)
 
+If you want to use the old method of downloading data then use `--old`
+
+```bash
+py -m bcedd --old
+```
+
 ## Install From Source
 
 If you want the latest features and don't want to wait for a release then you can install the tool from the github directly.
 
 1. Download [Git](https://git-scm.com/downloads)
 2. Run the following commands: (You may have to replace `py` with `python` or `python3`)
```

