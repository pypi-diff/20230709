# Comparing `tmp/zein-0.0.5.tar.gz` & `tmp/zein-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zein-0.0.5.tar", last modified: Sun Jul  9 12:38:33 2023, max compression
+gzip compressed data, was "zein-0.0.6.tar", last modified: Sun Jul  9 12:46:22 2023, max compression
```

## Comparing `zein-0.0.5.tar` & `zein-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 12:38:33.037207 zein-0.0.5/
--rw-rw-rw-   0        0        0     1070 2023-07-03 16:08:37.000000 zein-0.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0      831 2023-07-09 12:38:33.037207 zein-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1783 2023-07-03 16:08:38.000000 zein-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-07-09 12:38:33.037207 zein-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1278 2023-07-09 12:38:23.000000 zein-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-09 12:38:33.002013 zein-0.0.5/zein/
--rw-rw-rw-   0        0        0       42 2023-07-03 20:47:55.000000 zein-0.0.5/zein/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 12:38:33.021586 zein-0.0.5/zein/images/
--rw-rw-rw-   0        0        0       39 2023-07-03 16:08:38.000000 zein-0.0.5/zein/images/__init__.py
--rw-rw-rw-   0        0        0     2094 2023-07-09 12:05:54.000000 zein-0.0.5/zein/images/_utils.py
--rw-rw-rw-   0        0        0     4148 2023-07-08 19:32:14.000000 zein-0.0.5/zein/images/images_module.py
-drwxrwxrwx   0        0        0        0 2023-07-09 12:38:33.021586 zein-0.0.5/zein/text/
--rw-rw-rw-   0        0        0       35 2023-07-03 16:08:40.000000 zein-0.0.5/zein/text/__init__.py
--rw-rw-rw-   0        0        0     1650 2023-07-09 12:29:03.000000 zein-0.0.5/zein/text/_utils.py
--rw-rw-rw-   0        0        0     3271 2023-07-09 12:03:46.000000 zein-0.0.5/zein/text/ar.py
--rw-rw-rw-   0        0        0      583 2023-07-08 19:30:44.000000 zein-0.0.5/zein/text/text_module.py
-drwxrwxrwx   0        0        0        0 2023-07-09 12:38:33.017387 zein-0.0.5/zein.egg-info/
--rw-rw-rw-   0        0        0      831 2023-07-09 12:38:32.000000 zein-0.0.5/zein.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2023-07-09 12:38:32.000000 zein-0.0.5/zein.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 12:38:32.000000 zein-0.0.5/zein.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-09 12:38:32.000000 zein-0.0.5/zein.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       69 2023-07-09 12:38:32.000000 zein-0.0.5/zein.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-09 12:38:32.000000 zein-0.0.5/zein.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-09 12:46:22.052432 zein-0.0.6/
+-rw-rw-rw-   0        0        0     1070 2023-07-03 16:08:37.000000 zein-0.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      831 2023-07-09 12:46:22.036842 zein-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1783 2023-07-03 16:08:38.000000 zein-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-09 12:46:22.052432 zein-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1333 2023-07-09 12:46:15.000000 zein-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 12:46:22.005567 zein-0.0.6/zein/
+-rw-rw-rw-   0        0        0       42 2023-07-03 20:47:55.000000 zein-0.0.6/zein/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 12:46:22.036842 zein-0.0.6/zein/images/
+-rw-rw-rw-   0        0        0       39 2023-07-03 16:08:38.000000 zein-0.0.6/zein/images/__init__.py
+-rw-rw-rw-   0        0        0     2094 2023-07-09 12:05:54.000000 zein-0.0.6/zein/images/_utils.py
+-rw-rw-rw-   0        0        0     4148 2023-07-08 19:32:14.000000 zein-0.0.6/zein/images/images_module.py
+drwxrwxrwx   0        0        0        0 2023-07-09 12:46:22.036842 zein-0.0.6/zein/text/
+-rw-rw-rw-   0        0        0       35 2023-07-03 16:08:40.000000 zein-0.0.6/zein/text/__init__.py
+-rw-rw-rw-   0        0        0     1650 2023-07-09 12:29:03.000000 zein-0.0.6/zein/text/_utils.py
+-rw-rw-rw-   0        0        0     3271 2023-07-09 12:03:46.000000 zein-0.0.6/zein/text/ar.py
+-rw-rw-rw-   0        0        0      583 2023-07-08 19:30:44.000000 zein-0.0.6/zein/text/text_module.py
+drwxrwxrwx   0        0        0        0 2023-07-09 12:46:22.021220 zein-0.0.6/zein.egg-info/
+-rw-rw-rw-   0        0        0      831 2023-07-09 12:46:21.000000 zein-0.0.6/zein.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2023-07-09 12:46:21.000000 zein-0.0.6/zein.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 12:46:21.000000 zein-0.0.6/zein.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-09 12:46:21.000000 zein-0.0.6/zein.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       69 2023-07-09 12:46:21.000000 zein-0.0.6/zein.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-09 12:46:21.000000 zein-0.0.6/zein.egg-info/top_level.txt
```

### Comparing `zein-0.0.5/LICENSE.txt` & `zein-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zein-0.0.5/PKG-INFO` & `zein-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zein
-Version: 0.0.5
+Version: 0.0.6
 Summary: A python library for ensuring the safety and security of ML models
 Home-page: UNKNOWN
 Author: Mohamed Elsayed
 Author-email: <mohamedelsayed3487@gmail.com>
 License: UNKNOWN
 Keywords: python,arabic filtering,text filtering,profanity check
 Platform: UNKNOWN
```

### Comparing `zein-0.0.5/README.md` & `zein-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `zein-0.0.5/setup.py` & `zein-0.0.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'A python library for ensuring the safety and security of ML models'
 LONG_DESCRIPTION = 'A python library for ensuring the safety and security of ML models and their outputs for the Arabic and Islamic community'
 
 # Setting up
 setup(
     name="zein",
     version=VERSION,
     author="Mohamed Elsayed",
     author_email="<mohamedelsayed3487@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
-    packages=find_packages(),
+    #packages=find_packages(),
+    packages=["zein", "zein.text", "zein.images"],
     package_data= {
       'zein': ['data/*.csv'],
     },
+
     include_package_data=True,
     zip_safe=False,
     install_requires=['pandas', 'pickle', 'tensorflow==2.6.0'],
     extras_require={
         "scikit-learn": ["scikit-learn>=0.24.2"],
     },
     keywords=['python','arabic filtering', 'text filtering', 'profanity check'],
```

### Comparing `zein-0.0.5/zein/images/_utils.py` & `zein-0.0.6/zein/images/_utils.py`

 * *Files identical despite different names*

### Comparing `zein-0.0.5/zein/images/images_module.py` & `zein-0.0.6/zein/images/images_module.py`

 * *Files identical despite different names*

### Comparing `zein-0.0.5/zein/text/_utils.py` & `zein-0.0.6/zein/text/_utils.py`

 * *Files identical despite different names*

### Comparing `zein-0.0.5/zein/text/ar.py` & `zein-0.0.6/zein/text/ar.py`

 * *Files identical despite different names*

### Comparing `zein-0.0.5/zein/text/text_module.py` & `zein-0.0.6/zein/text/text_module.py`

 * *Files identical despite different names*

### Comparing `zein-0.0.5/zein.egg-info/PKG-INFO` & `zein-0.0.6/zein.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zein
-Version: 0.0.5
+Version: 0.0.6
 Summary: A python library for ensuring the safety and security of ML models
 Home-page: UNKNOWN
 Author: Mohamed Elsayed
 Author-email: <mohamedelsayed3487@gmail.com>
 License: UNKNOWN
 Keywords: python,arabic filtering,text filtering,profanity check
 Platform: UNKNOWN
```

