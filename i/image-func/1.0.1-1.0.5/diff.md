# Comparing `tmp/image_func-1.0.1.tar.gz` & `tmp/image_func-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_func-1.0.1.tar", last modified: Sun Jul  9 10:42:17 2023, max compression
+gzip compressed data, was "image_func-1.0.5.tar", last modified: Sun Jul  9 11:03:52 2023, max compression
```

## Comparing `image_func-1.0.1.tar` & `image_func-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 10:42:17.649225 image_func-1.0.1/
--rw-rw-rw-   0        0        0     1477 2023-07-08 13:23:55.000000 image_func-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      577 2023-07-09 10:42:17.648228 image_func-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-09 10:42:17.634264 image_func-1.0.1/image_func/
--rw-rw-rw-   0        0        0      504 2023-07-08 14:00:53.000000 image_func-1.0.1/image_func/__init__.py
--rw-rw-rw-   0        0        0      504 2023-07-08 13:19:09.000000 image_func-1.0.1/image_func/a.py
-drwxrwxrwx   0        0        0        0 2023-07-09 10:42:17.647237 image_func-1.0.1/image_func.egg-info/
--rw-rw-rw-   0        0        0      577 2023-07-09 10:42:17.000000 image_func-1.0.1/image_func.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-07-09 10:42:17.000000 image_func-1.0.1/image_func.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 10:42:17.000000 image_func-1.0.1/image_func.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-07-09 10:42:17.000000 image_func-1.0.1/image_func.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-09 10:42:17.000000 image_func-1.0.1/image_func.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-09 10:42:17.650221 image_func-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      793 2023-07-09 10:41:42.000000 image_func-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 11:03:52.265298 image_func-1.0.5/
+-rw-rw-rw-   0        0        0     1477 2023-07-08 13:23:55.000000 image_func-1.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      577 2023-07-09 11:03:52.264300 image_func-1.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-09 11:03:52.246350 image_func-1.0.5/image_func/
+-rw-rw-rw-   0        0        0      766 2023-07-09 10:52:26.000000 image_func-1.0.5/image_func/__init__.py
+-rw-rw-rw-   0        0        0      766 2023-07-09 11:00:20.000000 image_func-1.0.5/image_func/a.py
+drwxrwxrwx   0        0        0        0 2023-07-09 11:03:52.263303 image_func-1.0.5/image_func.egg-info/
+-rw-rw-rw-   0        0        0      577 2023-07-09 11:03:52.000000 image_func-1.0.5/image_func.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2023-07-09 11:03:52.000000 image_func-1.0.5/image_func.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 11:03:52.000000 image_func-1.0.5/image_func.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-07-09 11:03:52.000000 image_func-1.0.5/image_func.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-09 11:03:52.000000 image_func-1.0.5/image_func.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-09 11:03:52.265298 image_func-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      793 2023-07-09 11:03:32.000000 image_func-1.0.5/setup.py
```

### Comparing `image_func-1.0.1/LICENSE.txt` & `image_func-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `image_func-1.0.1/PKG-INFO` & `image_func-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image_func
-Version: 1.0.1
+Version: 1.0.5
 Summary: A module for image processing
 Author: Armankhanvsit
 Author-email: armanpconly@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `image_func-1.0.1/image_func.egg-info/PKG-INFO` & `image_func-1.0.5/image_func.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-func
-Version: 1.0.1
+Version: 1.0.5
 Summary: A module for image processing
 Author: Armankhanvsit
 Author-email: armanpconly@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `image_func-1.0.1/setup.py` & `image_func-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='image_func',
-    version='1.0.1',
+    version='1.0.5',
     author='Armankhanvsit',
     author_email='armanpconly@gmail.com',
     description='A module for image processing',
     long_description='A module for image processing using numpy, PIL, scipy, and matplotlib.',
     packages=['image_func'],
     install_requires=[
         'numpy',
```

