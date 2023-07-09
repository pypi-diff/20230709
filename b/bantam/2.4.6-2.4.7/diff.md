# Comparing `tmp/bantam-2.4.6.tar.gz` & `tmp/bantam-2.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bantam-2.4.6.tar", last modified: Sun Jul  2 22:37:30 2023, max compression
+gzip compressed data, was "bantam-2.4.7.tar", last modified: Sun Jul  9 14:52:04 2023, max compression
```

## Comparing `bantam-2.4.6.tar` & `bantam-2.4.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-07-02 22:37:30.917922 bantam-2.4.6/
--rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-07-02 22:37:30.917922 bantam-2.4.6/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)      370 2023-06-03 15:15:17.000000 bantam-2.4.6/README
--rw-rw-r--   0 pi        (1000) pi        (1000)       54 2023-06-11 03:58:58.000000 bantam-2.4.6/requirements.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       70 2023-07-02 22:37:30.917922 bantam-2.4.6/setup.cfg
--rwxrwxr-x   0 pi        (1000) pi        (1000)     1425 2023-07-02 22:36:45.000000 bantam-2.4.6/setup.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-07-02 22:37:30.913922 bantam-2.4.6/src/
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-07-02 22:37:30.917922 bantam-2.4.6/src/bantam/
--rw-rw-r--   0 pi        (1000) pi        (1000)     4616 2023-06-11 16:48:25.000000 bantam-2.4.6/src/bantam/__init__.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    12161 2023-06-24 14:59:54.000000 bantam-2.4.6/src/bantam/api.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-07-02 22:37:30.917922 bantam-2.4.6/src/bantam/autogen/
--rw-rw-r--   0 pi        (1000) pi        (1000)        0 2023-06-03 15:15:17.000000 bantam-2.4.6/src/bantam/autogen/__init__.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3399 2023-06-03 15:15:17.000000 bantam-2.4.6/src/bantam/autogen/main.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    22974 2023-07-02 22:27:44.000000 bantam-2.4.6/src/bantam/client.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     5705 2023-06-17 16:33:30.000000 bantam-2.4.6/src/bantam/conversions.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     4954 2023-07-02 22:34:38.000000 bantam-2.4.6/src/bantam/decorators.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    50579 2023-06-24 15:02:24.000000 bantam-2.4.6/src/bantam/http.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    22114 2023-06-17 16:10:55.000000 bantam-2.4.6/src/bantam/js.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    20416 2023-06-24 14:57:43.000000 bantam-2.4.6/src/bantam/js_async.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-07-02 22:37:30.917922 bantam-2.4.6/src/bantam.egg-info/
--rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-07-02 22:37:30.000000 bantam-2.4.6/src/bantam.egg-info/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)      672 2023-07-02 22:37:30.000000 bantam-2.4.6/src/bantam.egg-info/SOURCES.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-07-02 22:37:30.000000 bantam-2.4.6/src/bantam.egg-info/dependency_links.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       61 2023-07-02 22:37:30.000000 bantam-2.4.6/src/bantam.egg-info/entry_points.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       54 2023-07-02 22:37:30.000000 bantam-2.4.6/src/bantam.egg-info/requires.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)        7 2023-07-02 22:37:30.000000 bantam-2.4.6/src/bantam.egg-info/top_level.txt
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-07-02 22:37:30.917922 bantam-2.4.6/test/
--rw-rw-r--   0 pi        (1000) pi        (1000)     5624 2023-07-02 22:27:45.000000 bantam-2.4.6/test/test_client_get.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     4670 2023-06-17 15:47:27.000000 bantam-2.4.6/test/test_client_post.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     6038 2023-06-11 01:57:09.000000 bantam-2.4.6/test/test_client_post_inherited_apis.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3469 2023-06-04 03:12:58.000000 bantam-2.4.6/test/test_conversions.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3217 2023-06-04 03:13:40.000000 bantam-2.4.6/test/test_decorators.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      191 2023-06-04 14:25:43.000000 bantam-2.4.6/test/test_http.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3029 2023-06-24 15:07:18.000000 bantam-2.4.6/test/test_js.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     2831 2023-06-24 14:29:42.000000 bantam-2.4.6/test/test_js_async.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-07-09 14:52:04.431951 bantam-2.4.7/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-07-09 14:52:04.431951 bantam-2.4.7/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      370 2023-06-03 15:15:17.000000 bantam-2.4.7/README
+-rw-rw-r--   0 pi        (1000) pi        (1000)       54 2023-07-09 14:50:58.000000 bantam-2.4.7/requirements.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       70 2023-07-09 14:52:04.431951 bantam-2.4.7/setup.cfg
+-rwxrwxr-x   0 pi        (1000) pi        (1000)     1425 2023-07-09 14:51:22.000000 bantam-2.4.7/setup.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-07-09 14:52:04.431951 bantam-2.4.7/src/
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-07-09 14:52:04.431951 bantam-2.4.7/src/bantam/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4616 2023-06-11 16:48:25.000000 bantam-2.4.7/src/bantam/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    12161 2023-06-24 14:59:54.000000 bantam-2.4.7/src/bantam/api.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-07-09 14:52:04.431951 bantam-2.4.7/src/bantam/autogen/
+-rw-rw-r--   0 pi        (1000) pi        (1000)        0 2023-06-03 15:15:17.000000 bantam-2.4.7/src/bantam/autogen/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3399 2023-06-03 15:15:17.000000 bantam-2.4.7/src/bantam/autogen/main.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    22974 2023-07-02 22:27:44.000000 bantam-2.4.7/src/bantam/client.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     5705 2023-06-17 16:33:30.000000 bantam-2.4.7/src/bantam/conversions.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4954 2023-07-02 22:34:38.000000 bantam-2.4.7/src/bantam/decorators.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    50579 2023-06-24 15:02:24.000000 bantam-2.4.7/src/bantam/http.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    22114 2023-06-17 16:10:55.000000 bantam-2.4.7/src/bantam/js.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    20416 2023-06-24 14:57:43.000000 bantam-2.4.7/src/bantam/js_async.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-07-09 14:52:04.431951 bantam-2.4.7/src/bantam.egg-info/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-07-09 14:52:04.000000 bantam-2.4.7/src/bantam.egg-info/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      672 2023-07-09 14:52:04.000000 bantam-2.4.7/src/bantam.egg-info/SOURCES.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-07-09 14:52:04.000000 bantam-2.4.7/src/bantam.egg-info/dependency_links.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       61 2023-07-09 14:52:04.000000 bantam-2.4.7/src/bantam.egg-info/entry_points.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       54 2023-07-09 14:52:04.000000 bantam-2.4.7/src/bantam.egg-info/requires.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        7 2023-07-09 14:52:04.000000 bantam-2.4.7/src/bantam.egg-info/top_level.txt
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-07-09 14:52:04.431951 bantam-2.4.7/test/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     5624 2023-07-02 22:27:45.000000 bantam-2.4.7/test/test_client_get.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4670 2023-06-17 15:47:27.000000 bantam-2.4.7/test/test_client_post.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     6038 2023-06-11 01:57:09.000000 bantam-2.4.7/test/test_client_post_inherited_apis.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3469 2023-06-04 03:12:58.000000 bantam-2.4.7/test/test_conversions.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3217 2023-06-04 03:13:40.000000 bantam-2.4.7/test/test_decorators.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      191 2023-06-04 14:25:43.000000 bantam-2.4.7/test/test_http.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3029 2023-06-24 15:07:18.000000 bantam-2.4.7/test/test_js.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     2831 2023-06-24 14:29:42.000000 bantam-2.4.7/test/test_js_async.py
```

### Comparing `bantam-2.4.6/PKG-INFO` & `bantam-2.4.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bantam
-Version: 2.4.6
+Version: 2.4.7
 Summary: small utils to automate web interface in Python
 Home-page: https://github.com/nak/bantam
-Download-URL: https://github.com/bantam/dist/2.4.6
+Download-URL: https://github.com/bantam/dist/2.4.7
 Author: John Rusnak
 Author-email: john.j.rusnak@att.net
 License: BSD 2-CLAUSE
 Keywords: auto web api python
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `bantam-2.4.6/setup.py` & `bantam-2.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 import setuptools
 
-VERSION = "2.4.6"
+VERSION = "2.4.7"
 
 setuptools.setup(
     name='bantam',
     author='John Rusnak',
     author_email='john.j.rusnak@att.net',
     version=VERSION,
     data_files=[('.', ['requirements.txt'])],
```

### Comparing `bantam-2.4.6/src/bantam/__init__.py` & `bantam-2.4.7/src/bantam/__init__.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.6/src/bantam/api.py` & `bantam-2.4.7/src/bantam/api.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.6/src/bantam/autogen/main.py` & `bantam-2.4.7/src/bantam/autogen/main.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.6/src/bantam/client.py` & `bantam-2.4.7/src/bantam/client.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.6/src/bantam/conversions.py` & `bantam-2.4.7/src/bantam/conversions.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.6/src/bantam/decorators.py` & `bantam-2.4.7/src/bantam/decorators.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.6/src/bantam/http.py` & `bantam-2.4.7/src/bantam/http.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.6/src/bantam/js.py` & `bantam-2.4.7/src/bantam/js.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.6/src/bantam/js_async.py` & `bantam-2.4.7/src/bantam/js_async.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.6/src/bantam.egg-info/PKG-INFO` & `bantam-2.4.7/src/bantam.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bantam
-Version: 2.4.6
+Version: 2.4.7
 Summary: small utils to automate web interface in Python
 Home-page: https://github.com/nak/bantam
-Download-URL: https://github.com/bantam/dist/2.4.6
+Download-URL: https://github.com/bantam/dist/2.4.7
 Author: John Rusnak
 Author-email: john.j.rusnak@att.net
 License: BSD 2-CLAUSE
 Keywords: auto web api python
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `bantam-2.4.6/src/bantam.egg-info/SOURCES.txt` & `bantam-2.4.7/src/bantam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bantam-2.4.6/test/test_client_get.py` & `bantam-2.4.7/test/test_client_get.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.6/test/test_client_post.py` & `bantam-2.4.7/test/test_client_post.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.6/test/test_client_post_inherited_apis.py` & `bantam-2.4.7/test/test_client_post_inherited_apis.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.6/test/test_conversions.py` & `bantam-2.4.7/test/test_conversions.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.6/test/test_decorators.py` & `bantam-2.4.7/test/test_decorators.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.6/test/test_js.py` & `bantam-2.4.7/test/test_js.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.6/test/test_js_async.py` & `bantam-2.4.7/test/test_js_async.py`

 * *Files identical despite different names*

