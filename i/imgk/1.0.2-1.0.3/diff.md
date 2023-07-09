# Comparing `tmp/imgk-1.0.2.tar.gz` & `tmp/imgk-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/imgk-1.0.2.tar", last modified: Sun Jul  9 04:48:37 2023, max compression
+gzip compressed data, was "dist/imgk-1.0.3.tar", last modified: Sun Jul  9 04:51:22 2023, max compression
```

## Comparing `imgk-1.0.2.tar` & `imgk-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 praveenrathore   (501) staff       (20)        0 2023-07-09 04:48:37.000000 imgk-1.0.2/
--rw-r--r--   0 praveenrathore   (501) staff       (20)     2361 2023-07-09 04:48:37.000000 imgk-1.0.2/PKG-INFO
--rw-r--r--   0 praveenrathore   (501) staff       (20)     1609 2023-07-09 03:55:10.000000 imgk-1.0.2/README.md
--rw-r--r--   0 praveenrathore   (501) staff       (20)      641 2023-07-09 04:48:31.000000 imgk-1.0.2/setup.py
-drwxr-xr-x   0 praveenrathore   (501) staff       (20)        0 2023-07-09 04:48:37.000000 imgk-1.0.2/imgk/
--rw-r--r--   0 praveenrathore   (501) staff       (20)      566 2023-07-09 04:45:58.000000 imgk-1.0.2/imgk/__init__.py
--rw-r--r--   0 praveenrathore   (501) staff       (20)      145 2023-07-09 03:09:03.000000 imgk-1.0.2/imgk/utils.py
-drwxr-xr-x   0 praveenrathore   (501) staff       (20)        0 2023-07-09 04:48:37.000000 imgk-1.0.2/imgk/commands/
--rw-r--r--   0 praveenrathore   (501) staff       (20)      436 2023-07-09 03:08:43.000000 imgk-1.0.2/imgk/commands/metadata.py
--rw-r--r--   0 praveenrathore   (501) staff       (20)      632 2023-07-09 04:44:58.000000 imgk-1.0.2/imgk/commands/convert.py
--rw-r--r--   0 praveenrathore   (501) staff       (20)      943 2023-07-09 04:46:08.000000 imgk-1.0.2/imgk/commands/__init__.py
--rw-r--r--   0 praveenrathore   (501) staff       (20)      933 2023-07-09 03:08:23.000000 imgk-1.0.2/imgk/commands/crop.py
--rw-r--r--   0 praveenrathore   (501) staff       (20)      765 2023-07-09 03:08:51.000000 imgk-1.0.2/imgk/commands/resize.py
--rw-r--r--   0 praveenrathore   (501) staff       (20)      693 2023-07-09 03:08:35.000000 imgk-1.0.2/imgk/commands/filter.py
-drwxr-xr-x   0 praveenrathore   (501) staff       (20)        0 2023-07-09 04:48:37.000000 imgk-1.0.2/imgk.egg-info/
--rw-r--r--   0 praveenrathore   (501) staff       (20)     2361 2023-07-09 04:48:37.000000 imgk-1.0.2/imgk.egg-info/PKG-INFO
--rw-r--r--   0 praveenrathore   (501) staff       (20)      366 2023-07-09 04:48:37.000000 imgk-1.0.2/imgk.egg-info/SOURCES.txt
--rw-r--r--   0 praveenrathore   (501) staff       (20)       40 2023-07-09 04:48:37.000000 imgk-1.0.2/imgk.egg-info/entry_points.txt
--rw-r--r--   0 praveenrathore   (501) staff       (20)        7 2023-07-09 04:48:37.000000 imgk-1.0.2/imgk.egg-info/requires.txt
--rw-r--r--   0 praveenrathore   (501) staff       (20)        5 2023-07-09 04:48:37.000000 imgk-1.0.2/imgk.egg-info/top_level.txt
--rw-r--r--   0 praveenrathore   (501) staff       (20)        1 2023-07-09 04:48:37.000000 imgk-1.0.2/imgk.egg-info/dependency_links.txt
--rw-r--r--   0 praveenrathore   (501) staff       (20)       38 2023-07-09 04:48:37.000000 imgk-1.0.2/setup.cfg
+drwxr-xr-x   0 praveenrathore   (501) staff       (20)        0 2023-07-09 04:51:22.000000 imgk-1.0.3/
+-rw-r--r--   0 praveenrathore   (501) staff       (20)     2361 2023-07-09 04:51:22.000000 imgk-1.0.3/PKG-INFO
+-rw-r--r--   0 praveenrathore   (501) staff       (20)     1609 2023-07-09 03:55:10.000000 imgk-1.0.3/README.md
+-rw-r--r--   0 praveenrathore   (501) staff       (20)      641 2023-07-09 04:51:18.000000 imgk-1.0.3/setup.py
+drwxr-xr-x   0 praveenrathore   (501) staff       (20)        0 2023-07-09 04:51:22.000000 imgk-1.0.3/imgk/
+-rw-r--r--   0 praveenrathore   (501) staff       (20)      605 2023-07-09 04:51:01.000000 imgk-1.0.3/imgk/__init__.py
+-rw-r--r--   0 praveenrathore   (501) staff       (20)      145 2023-07-09 03:09:03.000000 imgk-1.0.3/imgk/utils.py
+drwxr-xr-x   0 praveenrathore   (501) staff       (20)        0 2023-07-09 04:51:22.000000 imgk-1.0.3/imgk/commands/
+-rw-r--r--   0 praveenrathore   (501) staff       (20)      436 2023-07-09 03:08:43.000000 imgk-1.0.3/imgk/commands/metadata.py
+-rw-r--r--   0 praveenrathore   (501) staff       (20)      632 2023-07-09 04:44:58.000000 imgk-1.0.3/imgk/commands/convert.py
+-rw-r--r--   0 praveenrathore   (501) staff       (20)      943 2023-07-09 04:46:08.000000 imgk-1.0.3/imgk/commands/__init__.py
+-rw-r--r--   0 praveenrathore   (501) staff       (20)      933 2023-07-09 03:08:23.000000 imgk-1.0.3/imgk/commands/crop.py
+-rw-r--r--   0 praveenrathore   (501) staff       (20)      765 2023-07-09 03:08:51.000000 imgk-1.0.3/imgk/commands/resize.py
+-rw-r--r--   0 praveenrathore   (501) staff       (20)      693 2023-07-09 03:08:35.000000 imgk-1.0.3/imgk/commands/filter.py
+drwxr-xr-x   0 praveenrathore   (501) staff       (20)        0 2023-07-09 04:51:22.000000 imgk-1.0.3/imgk.egg-info/
+-rw-r--r--   0 praveenrathore   (501) staff       (20)     2361 2023-07-09 04:51:22.000000 imgk-1.0.3/imgk.egg-info/PKG-INFO
+-rw-r--r--   0 praveenrathore   (501) staff       (20)      366 2023-07-09 04:51:22.000000 imgk-1.0.3/imgk.egg-info/SOURCES.txt
+-rw-r--r--   0 praveenrathore   (501) staff       (20)       40 2023-07-09 04:51:22.000000 imgk-1.0.3/imgk.egg-info/entry_points.txt
+-rw-r--r--   0 praveenrathore   (501) staff       (20)        7 2023-07-09 04:51:22.000000 imgk-1.0.3/imgk.egg-info/requires.txt
+-rw-r--r--   0 praveenrathore   (501) staff       (20)        5 2023-07-09 04:51:22.000000 imgk-1.0.3/imgk.egg-info/top_level.txt
+-rw-r--r--   0 praveenrathore   (501) staff       (20)        1 2023-07-09 04:51:22.000000 imgk-1.0.3/imgk.egg-info/dependency_links.txt
+-rw-r--r--   0 praveenrathore   (501) staff       (20)       38 2023-07-09 04:51:22.000000 imgk-1.0.3/setup.cfg
```

### Comparing `imgk-1.0.2/PKG-INFO` & `imgk-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imgk
-Version: 1.0.2
+Version: 1.0.3
 Summary: Image Processing Utility
 Home-page: https://github.com/prak132/imgk_cli
 Author: Prakhar Rathore
 License: UNKNOWN
 Description: # Imgk
         * Imgk is an image processing utility that provides various functionalities for manipulating and processing images from the command line.
```

### Comparing `imgk-1.0.2/README.md` & `imgk-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `imgk-1.0.2/setup.py` & `imgk-1.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'rb') as f:
     long_description = f.read().decode('utf-8')
 
 setup(
     name='imgk',
-    version='1.0.2',
+    version='1.0.3',
     author='Prakhar Rathore',
     description='Image Processing Utility',
     url='https://github.com/prak132/imgk_cli',
     keywords='image-processing utility command-line',
     long_description_content_type='text/markdown',
     long_description=long_description,
     platforms="macOS",
```

### Comparing `imgk-1.0.2/imgk/__init__.py` & `imgk-1.0.3/imgk/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,7 +10,10 @@
     metadata.add_subparser(subparsers)
     resize.add_subparser(subparsers)
     args = parser.parse_args()
     if not args.command:
         parser.print_help()
     else:
         args.func(args)
+
+if __name__ == "__main__":
+    main()
```

### Comparing `imgk-1.0.2/imgk/commands/convert.py` & `imgk-1.0.3/imgk/commands/convert.py`

 * *Files identical despite different names*

### Comparing `imgk-1.0.2/imgk/commands/__init__.py` & `imgk-1.0.3/imgk/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `imgk-1.0.2/imgk/commands/crop.py` & `imgk-1.0.3/imgk/commands/crop.py`

 * *Files identical despite different names*

### Comparing `imgk-1.0.2/imgk/commands/resize.py` & `imgk-1.0.3/imgk/commands/resize.py`

 * *Files identical despite different names*

### Comparing `imgk-1.0.2/imgk/commands/filter.py` & `imgk-1.0.3/imgk/commands/filter.py`

 * *Files identical despite different names*

### Comparing `imgk-1.0.2/imgk.egg-info/PKG-INFO` & `imgk-1.0.3/imgk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imgk
-Version: 1.0.2
+Version: 1.0.3
 Summary: Image Processing Utility
 Home-page: https://github.com/prak132/imgk_cli
 Author: Prakhar Rathore
 License: UNKNOWN
 Description: # Imgk
         * Imgk is an image processing utility that provides various functionalities for manipulating and processing images from the command line.
```

