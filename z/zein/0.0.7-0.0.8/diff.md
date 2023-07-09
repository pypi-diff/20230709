# Comparing `tmp/zein-0.0.7.tar.gz` & `tmp/zein-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zein-0.0.7.tar", last modified: Sun Jul  9 12:56:11 2023, max compression
+gzip compressed data, was "zein-0.0.8.tar", last modified: Sun Jul  9 13:09:24 2023, max compression
```

## Comparing `zein-0.0.7.tar` & `zein-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 12:56:11.021708 zein-0.0.7/
--rw-rw-rw-   0        0        0     1070 2023-07-03 16:08:37.000000 zein-0.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0      831 2023-07-09 12:56:11.021708 zein-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1783 2023-07-03 16:08:38.000000 zein-0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-07-09 12:56:11.021708 zein-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1333 2023-07-09 12:55:56.000000 zein-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-09 12:56:10.986250 zein-0.0.7/zein/
--rw-rw-rw-   0        0        0       44 2023-07-09 12:53:52.000000 zein-0.0.7/zein/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 12:56:11.006087 zein-0.0.7/zein/images/
--rw-rw-rw-   0        0        0       39 2023-07-03 16:08:38.000000 zein-0.0.7/zein/images/__init__.py
--rw-rw-rw-   0        0        0     2094 2023-07-09 12:05:54.000000 zein-0.0.7/zein/images/_utils.py
--rw-rw-rw-   0        0        0     4148 2023-07-08 19:32:14.000000 zein-0.0.7/zein/images/images_module.py
-drwxrwxrwx   0        0        0        0 2023-07-09 12:56:11.006087 zein-0.0.7/zein/text/
--rw-rw-rw-   0        0        0       35 2023-07-03 16:08:40.000000 zein-0.0.7/zein/text/__init__.py
--rw-rw-rw-   0        0        0     1650 2023-07-09 12:29:03.000000 zein-0.0.7/zein/text/_utils.py
--rw-rw-rw-   0        0        0     3271 2023-07-09 12:03:46.000000 zein-0.0.7/zein/text/ar.py
--rw-rw-rw-   0        0        0      583 2023-07-08 19:30:44.000000 zein-0.0.7/zein/text/text_module.py
-drwxrwxrwx   0        0        0        0 2023-07-09 12:56:11.001765 zein-0.0.7/zein.egg-info/
--rw-rw-rw-   0        0        0      831 2023-07-09 12:56:10.000000 zein-0.0.7/zein.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2023-07-09 12:56:10.000000 zein-0.0.7/zein.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 12:56:10.000000 zein-0.0.7/zein.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-09 12:56:10.000000 zein-0.0.7/zein.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       69 2023-07-09 12:56:10.000000 zein-0.0.7/zein.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-09 12:56:10.000000 zein-0.0.7/zein.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-09 13:09:24.662822 zein-0.0.8/
+-rw-rw-rw-   0        0        0     1070 2023-07-03 16:08:37.000000 zein-0.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0      831 2023-07-09 13:09:24.662822 zein-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1783 2023-07-03 16:08:38.000000 zein-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-09 13:09:24.662822 zein-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1333 2023-07-09 13:09:16.000000 zein-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 13:09:24.629847 zein-0.0.8/zein/
+-rw-rw-rw-   0        0        0       44 2023-07-09 13:04:32.000000 zein-0.0.8/zein/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 13:09:24.653783 zein-0.0.8/zein/images/
+-rw-rw-rw-   0        0        0       39 2023-07-03 16:08:38.000000 zein-0.0.8/zein/images/__init__.py
+-rw-rw-rw-   0        0        0     2094 2023-07-09 12:05:54.000000 zein-0.0.8/zein/images/_utils.py
+-rw-rw-rw-   0        0        0     4148 2023-07-08 19:32:14.000000 zein-0.0.8/zein/images/images_module.py
+drwxrwxrwx   0        0        0        0 2023-07-09 13:09:24.662822 zein-0.0.8/zein/text/
+-rw-rw-rw-   0        0        0       35 2023-07-09 13:04:57.000000 zein-0.0.8/zein/text/__init__.py
+-rw-rw-rw-   0        0        0     1650 2023-07-09 12:29:03.000000 zein-0.0.8/zein/text/_utils.py
+-rw-rw-rw-   0        0        0     3271 2023-07-09 12:03:46.000000 zein-0.0.8/zein/text/ar.py
+-rw-rw-rw-   0        0        0      583 2023-07-08 19:30:44.000000 zein-0.0.8/zein/text/text_module.py
+drwxrwxrwx   0        0        0        0 2023-07-09 13:09:24.644807 zein-0.0.8/zein.egg-info/
+-rw-rw-rw-   0        0        0      831 2023-07-09 13:09:24.000000 zein-0.0.8/zein.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2023-07-09 13:09:24.000000 zein-0.0.8/zein.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 13:09:24.000000 zein-0.0.8/zein.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-09 13:09:24.000000 zein-0.0.8/zein.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       69 2023-07-09 13:09:24.000000 zein-0.0.8/zein.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-09 13:09:24.000000 zein-0.0.8/zein.egg-info/top_level.txt
```

### Comparing `zein-0.0.7/LICENSE.txt` & `zein-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zein-0.0.7/PKG-INFO` & `zein-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zein
-Version: 0.0.7
+Version: 0.0.8
 Summary: A python library for ensuring the safety and security of ML models
 Home-page: UNKNOWN
 Author: Mohamed Elsayed
 Author-email: <mohamedelsayed3487@gmail.com>
 License: UNKNOWN
 Keywords: python,arabic filtering,text filtering,profanity check
 Platform: UNKNOWN
```

### Comparing `zein-0.0.7/README.md` & `zein-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `zein-0.0.7/setup.py` & `zein-0.0.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESCRIPTION = 'A python library for ensuring the safety and security of ML models'
 LONG_DESCRIPTION = 'A python library for ensuring the safety and security of ML models and their outputs for the Arabic and Islamic community'
 
 # Setting up
 setup(
     name="zein",
     version=VERSION,
@@ -20,15 +20,15 @@
     packages=["zein", "zein.text", "zein.images"],
     package_data= {
       'zein': ['data/*.csv'],
     },
 
     include_package_data=True,
     zip_safe=False,
-    install_requires=['pandas', 'pickle', 'tensorflow==2.6.0'],
+    install_requires=['pandas', 'joblib', 'tensorflow==2.6.0'],
     extras_require={
         "scikit-learn": ["scikit-learn>=0.24.2"],
     },
     keywords=['python','arabic filtering', 'text filtering', 'profanity check'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
```

### Comparing `zein-0.0.7/zein/images/_utils.py` & `zein-0.0.8/zein/images/_utils.py`

 * *Files identical despite different names*

### Comparing `zein-0.0.7/zein/images/images_module.py` & `zein-0.0.8/zein/images/images_module.py`

 * *Files identical despite different names*

### Comparing `zein-0.0.7/zein/text/_utils.py` & `zein-0.0.8/zein/text/_utils.py`

 * *Files identical despite different names*

### Comparing `zein-0.0.7/zein/text/ar.py` & `zein-0.0.8/zein/text/ar.py`

 * *Files identical despite different names*

### Comparing `zein-0.0.7/zein/text/text_module.py` & `zein-0.0.8/zein/text/text_module.py`

 * *Files identical despite different names*

### Comparing `zein-0.0.7/zein.egg-info/PKG-INFO` & `zein-0.0.8/zein.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zein
-Version: 0.0.7
+Version: 0.0.8
 Summary: A python library for ensuring the safety and security of ML models
 Home-page: UNKNOWN
 Author: Mohamed Elsayed
 Author-email: <mohamedelsayed3487@gmail.com>
 License: UNKNOWN
 Keywords: python,arabic filtering,text filtering,profanity check
 Platform: UNKNOWN
```

