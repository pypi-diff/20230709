# Comparing `tmp/imgk-1.0.4.tar.gz` & `tmp/imgk-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/imgk-1.0.4.tar", last modified: Sun Jul  9 04:56:07 2023, max compression
+gzip compressed data, was "dist/imgk-2.0.0.tar", last modified: Sun Jul  9 04:59:18 2023, max compression
```

## Comparing `imgk-1.0.4.tar` & `imgk-2.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 praveenrathore   (501) staff       (20)        0 2023-07-09 04:56:07.000000 imgk-1.0.4/
--rw-r--r--   0 praveenrathore   (501) staff       (20)     2361 2023-07-09 04:56:07.000000 imgk-1.0.4/PKG-INFO
--rw-r--r--   0 praveenrathore   (501) staff       (20)     1609 2023-07-09 03:55:10.000000 imgk-1.0.4/README.md
--rw-r--r--   0 praveenrathore   (501) staff       (20)      641 2023-07-09 04:55:57.000000 imgk-1.0.4/setup.py
-drwxr-xr-x   0 praveenrathore   (501) staff       (20)        0 2023-07-09 04:56:07.000000 imgk-1.0.4/imgk/
--rw-r--r--   0 praveenrathore   (501) staff       (20)       48 2023-07-09 04:55:24.000000 imgk-1.0.4/imgk/__init__.py
--rw-r--r--   0 praveenrathore   (501) staff       (20)      562 2023-07-09 04:53:57.000000 imgk-1.0.4/imgk/cli.py
--rw-r--r--   0 praveenrathore   (501) staff       (20)      145 2023-07-09 03:09:03.000000 imgk-1.0.4/imgk/utils.py
-drwxr-xr-x   0 praveenrathore   (501) staff       (20)        0 2023-07-09 04:56:07.000000 imgk-1.0.4/imgk/commands/
--rw-r--r--   0 praveenrathore   (501) staff       (20)      436 2023-07-09 03:08:43.000000 imgk-1.0.4/imgk/commands/metadata.py
--rw-r--r--   0 praveenrathore   (501) staff       (20)      632 2023-07-09 04:44:58.000000 imgk-1.0.4/imgk/commands/convert.py
--rw-r--r--   0 praveenrathore   (501) staff       (20)      943 2023-07-09 04:46:08.000000 imgk-1.0.4/imgk/commands/__init__.py
--rw-r--r--   0 praveenrathore   (501) staff       (20)      933 2023-07-09 03:08:23.000000 imgk-1.0.4/imgk/commands/crop.py
--rw-r--r--   0 praveenrathore   (501) staff       (20)      765 2023-07-09 03:08:51.000000 imgk-1.0.4/imgk/commands/resize.py
--rw-r--r--   0 praveenrathore   (501) staff       (20)      693 2023-07-09 03:08:35.000000 imgk-1.0.4/imgk/commands/filter.py
-drwxr-xr-x   0 praveenrathore   (501) staff       (20)        0 2023-07-09 04:56:07.000000 imgk-1.0.4/imgk.egg-info/
--rw-r--r--   0 praveenrathore   (501) staff       (20)     2361 2023-07-09 04:56:07.000000 imgk-1.0.4/imgk.egg-info/PKG-INFO
--rw-r--r--   0 praveenrathore   (501) staff       (20)      378 2023-07-09 04:56:07.000000 imgk-1.0.4/imgk.egg-info/SOURCES.txt
--rw-r--r--   0 praveenrathore   (501) staff       (20)       40 2023-07-09 04:56:07.000000 imgk-1.0.4/imgk.egg-info/entry_points.txt
--rw-r--r--   0 praveenrathore   (501) staff       (20)        7 2023-07-09 04:56:07.000000 imgk-1.0.4/imgk.egg-info/requires.txt
--rw-r--r--   0 praveenrathore   (501) staff       (20)        5 2023-07-09 04:56:07.000000 imgk-1.0.4/imgk.egg-info/top_level.txt
--rw-r--r--   0 praveenrathore   (501) staff       (20)        1 2023-07-09 04:56:07.000000 imgk-1.0.4/imgk.egg-info/dependency_links.txt
--rw-r--r--   0 praveenrathore   (501) staff       (20)       38 2023-07-09 04:56:07.000000 imgk-1.0.4/setup.cfg
+drwxr-xr-x   0 praveenrathore   (501) staff       (20)        0 2023-07-09 04:59:17.000000 imgk-2.0.0/
+-rw-r--r--   0 praveenrathore   (501) staff       (20)     2361 2023-07-09 04:59:17.000000 imgk-2.0.0/PKG-INFO
+-rw-r--r--   0 praveenrathore   (501) staff       (20)     1609 2023-07-09 03:55:10.000000 imgk-2.0.0/README.md
+-rw-r--r--   0 praveenrathore   (501) staff       (20)      641 2023-07-09 04:58:39.000000 imgk-2.0.0/setup.py
+drwxr-xr-x   0 praveenrathore   (501) staff       (20)        0 2023-07-09 04:59:17.000000 imgk-2.0.0/imgk/
+-rw-r--r--   0 praveenrathore   (501) staff       (20)       72 2023-07-09 04:59:11.000000 imgk-2.0.0/imgk/__init__.py
+-rw-r--r--   0 praveenrathore   (501) staff       (20)      562 2023-07-09 04:53:57.000000 imgk-2.0.0/imgk/cli.py
+-rw-r--r--   0 praveenrathore   (501) staff       (20)      145 2023-07-09 03:09:03.000000 imgk-2.0.0/imgk/utils.py
+drwxr-xr-x   0 praveenrathore   (501) staff       (20)        0 2023-07-09 04:59:17.000000 imgk-2.0.0/imgk/commands/
+-rw-r--r--   0 praveenrathore   (501) staff       (20)      436 2023-07-09 03:08:43.000000 imgk-2.0.0/imgk/commands/metadata.py
+-rw-r--r--   0 praveenrathore   (501) staff       (20)      632 2023-07-09 04:44:58.000000 imgk-2.0.0/imgk/commands/convert.py
+-rw-r--r--   0 praveenrathore   (501) staff       (20)      943 2023-07-09 04:46:08.000000 imgk-2.0.0/imgk/commands/__init__.py
+-rw-r--r--   0 praveenrathore   (501) staff       (20)      933 2023-07-09 03:08:23.000000 imgk-2.0.0/imgk/commands/crop.py
+-rw-r--r--   0 praveenrathore   (501) staff       (20)      765 2023-07-09 03:08:51.000000 imgk-2.0.0/imgk/commands/resize.py
+-rw-r--r--   0 praveenrathore   (501) staff       (20)      693 2023-07-09 03:08:35.000000 imgk-2.0.0/imgk/commands/filter.py
+drwxr-xr-x   0 praveenrathore   (501) staff       (20)        0 2023-07-09 04:59:17.000000 imgk-2.0.0/imgk.egg-info/
+-rw-r--r--   0 praveenrathore   (501) staff       (20)     2361 2023-07-09 04:59:17.000000 imgk-2.0.0/imgk.egg-info/PKG-INFO
+-rw-r--r--   0 praveenrathore   (501) staff       (20)      378 2023-07-09 04:59:17.000000 imgk-2.0.0/imgk.egg-info/SOURCES.txt
+-rw-r--r--   0 praveenrathore   (501) staff       (20)       40 2023-07-09 04:59:17.000000 imgk-2.0.0/imgk.egg-info/entry_points.txt
+-rw-r--r--   0 praveenrathore   (501) staff       (20)        7 2023-07-09 04:59:17.000000 imgk-2.0.0/imgk.egg-info/requires.txt
+-rw-r--r--   0 praveenrathore   (501) staff       (20)        5 2023-07-09 04:59:17.000000 imgk-2.0.0/imgk.egg-info/top_level.txt
+-rw-r--r--   0 praveenrathore   (501) staff       (20)        1 2023-07-09 04:59:17.000000 imgk-2.0.0/imgk.egg-info/dependency_links.txt
+-rw-r--r--   0 praveenrathore   (501) staff       (20)       38 2023-07-09 04:59:17.000000 imgk-2.0.0/setup.cfg
```

### Comparing `imgk-1.0.4/PKG-INFO` & `imgk-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imgk
-Version: 1.0.4
+Version: 2.0.0
 Summary: Image Processing Utility
 Home-page: https://github.com/prak132/imgk_cli
 Author: Prakhar Rathore
 License: UNKNOWN
 Description: # Imgk
         * Imgk is an image processing utility that provides various functionalities for manipulating and processing images from the command line.
```

### Comparing `imgk-1.0.4/README.md` & `imgk-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `imgk-1.0.4/setup.py` & `imgk-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'rb') as f:
     long_description = f.read().decode('utf-8')
 
 setup(
     name='imgk',
-    version='1.0.4',
+    version='2.0.0',
     author='Prakhar Rathore',
     description='Image Processing Utility',
     url='https://github.com/prak132/imgk_cli',
     keywords='image-processing utility command-line',
     long_description_content_type='text/markdown',
     long_description=long_description,
     platforms="macOS",
```

### Comparing `imgk-1.0.4/imgk/cli.py` & `imgk-2.0.0/imgk/cli.py`

 * *Files identical despite different names*

### Comparing `imgk-1.0.4/imgk/commands/convert.py` & `imgk-2.0.0/imgk/commands/convert.py`

 * *Files identical despite different names*

### Comparing `imgk-1.0.4/imgk/commands/__init__.py` & `imgk-2.0.0/imgk/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `imgk-1.0.4/imgk/commands/crop.py` & `imgk-2.0.0/imgk/commands/crop.py`

 * *Files identical despite different names*

### Comparing `imgk-1.0.4/imgk/commands/resize.py` & `imgk-2.0.0/imgk/commands/resize.py`

 * *Files identical despite different names*

### Comparing `imgk-1.0.4/imgk/commands/filter.py` & `imgk-2.0.0/imgk/commands/filter.py`

 * *Files identical despite different names*

### Comparing `imgk-1.0.4/imgk.egg-info/PKG-INFO` & `imgk-2.0.0/imgk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imgk
-Version: 1.0.4
+Version: 2.0.0
 Summary: Image Processing Utility
 Home-page: https://github.com/prak132/imgk_cli
 Author: Prakhar Rathore
 License: UNKNOWN
 Description: # Imgk
         * Imgk is an image processing utility that provides various functionalities for manipulating and processing images from the command line.
```

