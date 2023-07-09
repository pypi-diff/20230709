# Comparing `tmp/image_func-1.0.6.tar.gz` & `tmp/image_func-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_func-1.0.6.tar", last modified: Sun Jul  9 11:24:33 2023, max compression
+gzip compressed data, was "image_func-1.0.8.tar", last modified: Sun Jul  9 11:29:50 2023, max compression
```

## Comparing `image_func-1.0.6.tar` & `image_func-1.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 11:24:33.612964 image_func-1.0.6/
--rw-rw-rw-   0        0        0     1477 2023-07-08 13:23:55.000000 image_func-1.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0      577 2023-07-09 11:24:33.611966 image_func-1.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-09 11:24:33.593017 image_func-1.0.6/image_func/
--rw-rw-rw-   0        0        0      766 2023-07-09 10:52:26.000000 image_func-1.0.6/image_func/__init__.py
--rw-rw-rw-   0        0        0     1653 2023-07-09 11:24:06.000000 image_func-1.0.6/image_func/a.py
-drwxrwxrwx   0        0        0        0 2023-07-09 11:24:33.609973 image_func-1.0.6/image_func.egg-info/
--rw-rw-rw-   0        0        0      577 2023-07-09 11:24:33.000000 image_func-1.0.6/image_func.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-07-09 11:24:33.000000 image_func-1.0.6/image_func.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 11:24:33.000000 image_func-1.0.6/image_func.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-07-09 11:24:33.000000 image_func-1.0.6/image_func.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-09 11:24:33.000000 image_func-1.0.6/image_func.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-09 11:24:33.612964 image_func-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      793 2023-07-09 11:24:25.000000 image_func-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 11:29:50.532254 image_func-1.0.8/
+-rw-rw-rw-   0        0        0     1477 2023-07-08 13:23:55.000000 image_func-1.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0      577 2023-07-09 11:29:50.528266 image_func-1.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-09 11:29:50.505814 image_func-1.0.8/image_func/
+-rw-rw-rw-   0        0        0     1653 2023-07-09 11:27:13.000000 image_func-1.0.8/image_func/__init__.py
+-rw-rw-rw-   0        0        0     1653 2023-07-09 11:24:06.000000 image_func-1.0.8/image_func/a.py
+drwxrwxrwx   0        0        0        0 2023-07-09 11:29:50.526270 image_func-1.0.8/image_func.egg-info/
+-rw-rw-rw-   0        0        0      577 2023-07-09 11:29:50.000000 image_func-1.0.8/image_func.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2023-07-09 11:29:50.000000 image_func-1.0.8/image_func.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 11:29:50.000000 image_func-1.0.8/image_func.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-07-09 11:29:50.000000 image_func-1.0.8/image_func.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-09 11:29:50.000000 image_func-1.0.8/image_func.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-09 11:29:50.532254 image_func-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      793 2023-07-09 11:29:45.000000 image_func-1.0.8/setup.py
```

### Comparing `image_func-1.0.6/LICENSE.txt` & `image_func-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `image_func-1.0.6/PKG-INFO` & `image_func-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image_func
-Version: 1.0.6
+Version: 1.0.8
 Summary: A module for image processing
 Author: Armankhanvsit
 Author-email: armanpconly@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `image_func-1.0.6/image_func/a.py` & `image_func-1.0.8/image_func/__init__.py`

 * *Files identical despite different names*

### Comparing `image_func-1.0.6/image_func.egg-info/PKG-INFO` & `image_func-1.0.8/image_func.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-func
-Version: 1.0.6
+Version: 1.0.8
 Summary: A module for image processing
 Author: Armankhanvsit
 Author-email: armanpconly@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `image_func-1.0.6/setup.py` & `image_func-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='image_func',
-    version='1.0.6',
+    version='1.0.8',
     author='Armankhanvsit',
     author_email='armanpconly@gmail.com',
     description='A module for image processing',
     long_description='A module for image processing using numpy, PIL, scipy, and matplotlib.',
     packages=['image_func'],
     install_requires=[
         'numpy',
```

