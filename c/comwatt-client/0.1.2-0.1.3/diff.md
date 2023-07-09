# Comparing `tmp/comwatt-client-0.1.2.tar.gz` & `tmp/comwatt-client-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comwatt-client-0.1.2.tar", last modified: Sun Jul  9 08:01:46 2023, max compression
+gzip compressed data, was "comwatt-client-0.1.3.tar", last modified: Sun Jul  9 13:24:39 2023, max compression
```

## Comparing `comwatt-client-0.1.2.tar` & `comwatt-client-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 mat       (1000) mat       (1000)        0 2023-07-09 08:01:46.720739 comwatt-client-0.1.2/
--rw-rw-r--   0 mat       (1000) mat       (1000)      549 2023-07-09 08:01:46.720739 comwatt-client-0.1.2/PKG-INFO
--rw-rw-r--   0 mat       (1000) mat       (1000)     2998 2023-07-08 21:27:06.000000 comwatt-client-0.1.2/README.md
-drwxrwxr-x   0 mat       (1000) mat       (1000)        0 2023-07-09 08:01:46.716740 comwatt-client-0.1.2/comwatt-client/
--rw-rw-r--   0 mat       (1000) mat       (1000)        0 2023-07-08 13:37:30.000000 comwatt-client-0.1.2/comwatt-client/__init__.py
--rw-rw-r--   0 mat       (1000) mat       (1000)     7281 2023-07-08 21:26:46.000000 comwatt-client-0.1.2/comwatt-client/client.py
-drwxrwxr-x   0 mat       (1000) mat       (1000)        0 2023-07-09 08:01:46.716740 comwatt-client-0.1.2/comwatt_client.egg-info/
--rw-rw-r--   0 mat       (1000) mat       (1000)      549 2023-07-09 08:01:46.000000 comwatt-client-0.1.2/comwatt_client.egg-info/PKG-INFO
--rw-rw-r--   0 mat       (1000) mat       (1000)      259 2023-07-09 08:01:46.000000 comwatt-client-0.1.2/comwatt_client.egg-info/SOURCES.txt
--rw-rw-r--   0 mat       (1000) mat       (1000)        1 2023-07-09 08:01:46.000000 comwatt-client-0.1.2/comwatt_client.egg-info/dependency_links.txt
--rw-rw-r--   0 mat       (1000) mat       (1000)        9 2023-07-09 08:01:46.000000 comwatt-client-0.1.2/comwatt_client.egg-info/requires.txt
--rw-rw-r--   0 mat       (1000) mat       (1000)       15 2023-07-09 08:01:46.000000 comwatt-client-0.1.2/comwatt_client.egg-info/top_level.txt
--rw-rw-r--   0 mat       (1000) mat       (1000)       38 2023-07-09 08:01:46.720739 comwatt-client-0.1.2/setup.cfg
--rw-rw-r--   0 mat       (1000) mat       (1000)      649 2023-07-09 08:01:07.000000 comwatt-client-0.1.2/setup.py
+drwxrwxr-x   0 mat       (1000) mat       (1000)        0 2023-07-09 13:24:39.523130 comwatt-client-0.1.3/
+-rw-rw-r--   0 mat       (1000) mat       (1000)      549 2023-07-09 13:24:39.523130 comwatt-client-0.1.3/PKG-INFO
+-rw-rw-r--   0 mat       (1000) mat       (1000)     2998 2023-07-08 21:27:06.000000 comwatt-client-0.1.3/README.md
+drwxrwxr-x   0 mat       (1000) mat       (1000)        0 2023-07-09 13:24:39.519130 comwatt-client-0.1.3/comwatt-client/
+-rw-rw-r--   0 mat       (1000) mat       (1000)       63 2023-07-09 13:23:14.000000 comwatt-client-0.1.3/comwatt-client/__init__.py
+-rw-rw-r--   0 mat       (1000) mat       (1000)     7281 2023-07-08 21:26:46.000000 comwatt-client-0.1.3/comwatt-client/client.py
+drwxrwxr-x   0 mat       (1000) mat       (1000)        0 2023-07-09 13:24:39.523130 comwatt-client-0.1.3/comwatt_client.egg-info/
+-rw-rw-r--   0 mat       (1000) mat       (1000)      549 2023-07-09 13:24:39.000000 comwatt-client-0.1.3/comwatt_client.egg-info/PKG-INFO
+-rw-rw-r--   0 mat       (1000) mat       (1000)      259 2023-07-09 13:24:39.000000 comwatt-client-0.1.3/comwatt_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 mat       (1000) mat       (1000)        1 2023-07-09 13:24:39.000000 comwatt-client-0.1.3/comwatt_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 mat       (1000) mat       (1000)        9 2023-07-09 13:24:39.000000 comwatt-client-0.1.3/comwatt_client.egg-info/requires.txt
+-rw-rw-r--   0 mat       (1000) mat       (1000)       15 2023-07-09 13:24:39.000000 comwatt-client-0.1.3/comwatt_client.egg-info/top_level.txt
+-rw-rw-r--   0 mat       (1000) mat       (1000)       38 2023-07-09 13:24:39.523130 comwatt-client-0.1.3/setup.cfg
+-rw-rw-r--   0 mat       (1000) mat       (1000)      649 2023-07-09 13:23:42.000000 comwatt-client-0.1.3/setup.py
```

### Comparing `comwatt-client-0.1.2/PKG-INFO` & `comwatt-client-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comwatt-client
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python Client for Comwatt API
 Home-page: UNKNOWN
 Author: Matéo Greil
 Author-email: contact@greil.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `comwatt-client-0.1.2/README.md` & `comwatt-client-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `comwatt-client-0.1.2/comwatt-client/client.py` & `comwatt-client-0.1.3/comwatt-client/client.py`

 * *Files identical despite different names*

### Comparing `comwatt-client-0.1.2/comwatt_client.egg-info/PKG-INFO` & `comwatt-client-0.1.3/comwatt_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comwatt-client
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python Client for Comwatt API
 Home-page: UNKNOWN
 Author: Matéo Greil
 Author-email: contact@greil.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `comwatt-client-0.1.2/setup.py` & `comwatt-client-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='comwatt-client',
-    version='0.1.2',
+    version='0.1.3',
     author='Matéo Greil',
     author_email='contact@greil.fr',
     description='Python Client for Comwatt API',
     packages=find_packages(),
     install_requires=[
         'requests',
     ],
```

