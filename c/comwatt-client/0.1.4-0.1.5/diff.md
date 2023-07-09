# Comparing `tmp/comwatt-client-0.1.4.tar.gz` & `tmp/comwatt-client-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comwatt-client-0.1.4.tar", last modified: Sun Jul  9 13:34:05 2023, max compression
+gzip compressed data, was "comwatt-client-0.1.5.tar", last modified: Sun Jul  9 13:37:26 2023, max compression
```

## Comparing `comwatt-client-0.1.4.tar` & `comwatt-client-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 mat       (1000) mat       (1000)        0 2023-07-09 13:34:05.732703 comwatt-client-0.1.4/
--rw-rw-r--   0 mat       (1000) mat       (1000)      549 2023-07-09 13:34:05.732703 comwatt-client-0.1.4/PKG-INFO
--rw-rw-r--   0 mat       (1000) mat       (1000)     2998 2023-07-08 21:27:06.000000 comwatt-client-0.1.4/README.md
-drwxrwxr-x   0 mat       (1000) mat       (1000)        0 2023-07-09 13:34:05.732703 comwatt-client-0.1.4/comwatt-client/
--rw-rw-r--   0 mat       (1000) mat       (1000)       63 2023-07-09 13:23:14.000000 comwatt-client-0.1.4/comwatt-client/__init__.py
--rw-rw-r--   0 mat       (1000) mat       (1000)     7281 2023-07-09 13:33:08.000000 comwatt-client-0.1.4/comwatt-client/comwatt-client.py
-drwxrwxr-x   0 mat       (1000) mat       (1000)        0 2023-07-09 13:34:05.732703 comwatt-client-0.1.4/comwatt_client.egg-info/
--rw-rw-r--   0 mat       (1000) mat       (1000)      549 2023-07-09 13:34:05.000000 comwatt-client-0.1.4/comwatt_client.egg-info/PKG-INFO
--rw-rw-r--   0 mat       (1000) mat       (1000)      267 2023-07-09 13:34:05.000000 comwatt-client-0.1.4/comwatt_client.egg-info/SOURCES.txt
--rw-rw-r--   0 mat       (1000) mat       (1000)        1 2023-07-09 13:34:05.000000 comwatt-client-0.1.4/comwatt_client.egg-info/dependency_links.txt
--rw-rw-r--   0 mat       (1000) mat       (1000)        9 2023-07-09 13:34:05.000000 comwatt-client-0.1.4/comwatt_client.egg-info/requires.txt
--rw-rw-r--   0 mat       (1000) mat       (1000)       15 2023-07-09 13:34:05.000000 comwatt-client-0.1.4/comwatt_client.egg-info/top_level.txt
--rw-rw-r--   0 mat       (1000) mat       (1000)       38 2023-07-09 13:34:05.732703 comwatt-client-0.1.4/setup.cfg
--rw-rw-r--   0 mat       (1000) mat       (1000)      649 2023-07-09 13:33:49.000000 comwatt-client-0.1.4/setup.py
+drwxrwxr-x   0 mat       (1000) mat       (1000)        0 2023-07-09 13:37:26.682937 comwatt-client-0.1.5/
+-rw-rw-r--   0 mat       (1000) mat       (1000)      549 2023-07-09 13:37:26.682937 comwatt-client-0.1.5/PKG-INFO
+-rw-rw-r--   0 mat       (1000) mat       (1000)     2998 2023-07-08 21:27:06.000000 comwatt-client-0.1.5/README.md
+drwxrwxr-x   0 mat       (1000) mat       (1000)        0 2023-07-09 13:37:26.678937 comwatt-client-0.1.5/comwatt_client/
+-rw-rw-r--   0 mat       (1000) mat       (1000)       63 2023-07-09 13:36:52.000000 comwatt-client-0.1.5/comwatt_client/__init__.py
+-rw-rw-r--   0 mat       (1000) mat       (1000)     7281 2023-07-09 13:36:52.000000 comwatt-client-0.1.5/comwatt_client/comwatt_client.py
+drwxrwxr-x   0 mat       (1000) mat       (1000)        0 2023-07-09 13:37:26.682937 comwatt-client-0.1.5/comwatt_client.egg-info/
+-rw-rw-r--   0 mat       (1000) mat       (1000)      549 2023-07-09 13:37:26.000000 comwatt-client-0.1.5/comwatt_client.egg-info/PKG-INFO
+-rw-rw-r--   0 mat       (1000) mat       (1000)      267 2023-07-09 13:37:26.000000 comwatt-client-0.1.5/comwatt_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 mat       (1000) mat       (1000)        1 2023-07-09 13:37:26.000000 comwatt-client-0.1.5/comwatt_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 mat       (1000) mat       (1000)        9 2023-07-09 13:37:26.000000 comwatt-client-0.1.5/comwatt_client.egg-info/requires.txt
+-rw-rw-r--   0 mat       (1000) mat       (1000)       15 2023-07-09 13:37:26.000000 comwatt-client-0.1.5/comwatt_client.egg-info/top_level.txt
+-rw-rw-r--   0 mat       (1000) mat       (1000)       38 2023-07-09 13:37:26.682937 comwatt-client-0.1.5/setup.cfg
+-rw-rw-r--   0 mat       (1000) mat       (1000)      649 2023-07-09 13:37:16.000000 comwatt-client-0.1.5/setup.py
```

### Comparing `comwatt-client-0.1.4/PKG-INFO` & `comwatt-client-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comwatt-client
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python Client for Comwatt API
 Home-page: UNKNOWN
 Author: Matéo Greil
 Author-email: contact@greil.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `comwatt-client-0.1.4/README.md` & `comwatt-client-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `comwatt-client-0.1.4/comwatt-client/comwatt-client.py` & `comwatt-client-0.1.5/comwatt_client/comwatt_client.py`

 * *Files identical despite different names*

### Comparing `comwatt-client-0.1.4/comwatt_client.egg-info/PKG-INFO` & `comwatt-client-0.1.5/comwatt_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comwatt-client
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python Client for Comwatt API
 Home-page: UNKNOWN
 Author: Matéo Greil
 Author-email: contact@greil.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `comwatt-client-0.1.4/setup.py` & `comwatt-client-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='comwatt-client',
-    version='0.1.4',
+    version='0.1.5',
     author='Matéo Greil',
     author_email='contact@greil.fr',
     description='Python Client for Comwatt API',
     packages=find_packages(),
     install_requires=[
         'requests',
     ],
```

