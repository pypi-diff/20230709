# Comparing `tmp/LordPath-2023.7.8.1.tar.gz` & `tmp/LordPath-2023.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LordPath-2023.7.8.1.tar", last modified: Sat Jul  8 11:23:59 2023, max compression
+gzip compressed data, was "LordPath-2023.7.9.tar", last modified: Sun Jul  9 20:20:57 2023, max compression
```

## Comparing `LordPath-2023.7.8.1.tar` & `LordPath-2023.7.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 philippkitzmuller   (501) staff       (20)        0 2023-07-08 11:23:59.036468 LordPath-2023.7.8.1/
-drwxr-xr-x   0 philippkitzmuller   (501) staff       (20)        0 2023-07-08 11:23:59.032364 LordPath-2023.7.8.1/LordPath/
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)     3483 2023-05-06 13:46:10.000000 LordPath-2023.7.8.1/LordPath/__init__.py
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)      617 2022-12-09 23:13:08.000000 LordPath-2023.7.8.1/LordPath/dataset.py
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)      583 2023-03-21 08:46:08.000000 LordPath-2023.7.8.1/LordPath/descriptors.py
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)     6385 2023-03-17 16:32:55.000000 LordPath-2023.7.8.1/LordPath/filefolderclass.py
-drwxr-xr-x   0 philippkitzmuller   (501) staff       (20)        0 2023-07-08 11:23:59.035844 LordPath-2023.7.8.1/LordPath/opener/
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)     1282 2023-07-08 10:49:10.000000 LordPath-2023.7.8.1/LordPath/opener/__init__.py
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)      328 2023-03-17 16:42:56.000000 LordPath-2023.7.8.1/LordPath/opener/base.py
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)      868 2023-03-17 16:42:56.000000 LordPath-2023.7.8.1/LordPath/opener/json.py
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)      864 2023-03-17 16:42:56.000000 LordPath-2023.7.8.1/LordPath/opener/pickle.py
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)      490 2023-03-17 16:42:56.000000 LordPath-2023.7.8.1/LordPath/opener/toml.py
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)      799 2023-07-08 11:23:50.000000 LordPath-2023.7.8.1/LordPath/opener/xml.py
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)     1019 2023-03-16 23:58:05.000000 LordPath-2023.7.8.1/LordPath/opener/yaml.py
-drwxr-xr-x   0 philippkitzmuller   (501) staff       (20)        0 2023-07-08 11:23:59.033443 LordPath-2023.7.8.1/LordPath.egg-info/
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)      433 2023-07-08 11:23:59.000000 LordPath-2023.7.8.1/LordPath.egg-info/PKG-INFO
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)      450 2023-07-08 11:23:59.000000 LordPath-2023.7.8.1/LordPath.egg-info/SOURCES.txt
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)        1 2023-07-08 11:23:59.000000 LordPath-2023.7.8.1/LordPath.egg-info/dependency_links.txt
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)       23 2023-07-08 11:23:59.000000 LordPath-2023.7.8.1/LordPath.egg-info/requires.txt
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)        9 2023-07-08 11:23:59.000000 LordPath-2023.7.8.1/LordPath.egg-info/top_level.txt
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)      433 2023-07-08 11:23:59.036316 LordPath-2023.7.8.1/PKG-INFO
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)       58 2023-03-19 09:41:22.000000 LordPath-2023.7.8.1/README.rst
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)      486 2023-07-08 11:23:55.000000 LordPath-2023.7.8.1/pyproject.toml
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)       38 2023-07-08 11:23:59.036510 LordPath-2023.7.8.1/setup.cfg
+drwxr-xr-x   0 philippkitzmuller   (501) staff       (20)        0 2023-07-09 20:20:57.578766 LordPath-2023.7.9/
+drwxr-xr-x   0 philippkitzmuller   (501) staff       (20)        0 2023-07-09 20:20:57.575286 LordPath-2023.7.9/LordPath/
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)     3483 2023-05-06 13:46:10.000000 LordPath-2023.7.9/LordPath/__init__.py
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)      617 2022-12-09 23:13:08.000000 LordPath-2023.7.9/LordPath/dataset.py
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)      583 2023-03-21 08:46:08.000000 LordPath-2023.7.9/LordPath/descriptors.py
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)     6385 2023-03-17 16:32:55.000000 LordPath-2023.7.9/LordPath/filefolderclass.py
+drwxr-xr-x   0 philippkitzmuller   (501) staff       (20)        0 2023-07-09 20:20:57.578208 LordPath-2023.7.9/LordPath/opener/
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)     1282 2023-07-08 10:49:10.000000 LordPath-2023.7.9/LordPath/opener/__init__.py
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)      328 2023-03-17 16:42:56.000000 LordPath-2023.7.9/LordPath/opener/base.py
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)      868 2023-03-17 16:42:56.000000 LordPath-2023.7.9/LordPath/opener/json.py
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)      864 2023-03-17 16:42:56.000000 LordPath-2023.7.9/LordPath/opener/pickle.py
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)      490 2023-03-17 16:42:56.000000 LordPath-2023.7.9/LordPath/opener/toml.py
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)      786 2023-07-09 20:20:52.000000 LordPath-2023.7.9/LordPath/opener/xml.py
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)     1019 2023-03-16 23:58:05.000000 LordPath-2023.7.9/LordPath/opener/yaml.py
+drwxr-xr-x   0 philippkitzmuller   (501) staff       (20)        0 2023-07-09 20:20:57.576329 LordPath-2023.7.9/LordPath.egg-info/
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)      431 2023-07-09 20:20:57.000000 LordPath-2023.7.9/LordPath.egg-info/PKG-INFO
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)      450 2023-07-09 20:20:57.000000 LordPath-2023.7.9/LordPath.egg-info/SOURCES.txt
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)        1 2023-07-09 20:20:57.000000 LordPath-2023.7.9/LordPath.egg-info/dependency_links.txt
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)       23 2023-07-09 20:20:57.000000 LordPath-2023.7.9/LordPath.egg-info/requires.txt
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)        9 2023-07-09 20:20:57.000000 LordPath-2023.7.9/LordPath.egg-info/top_level.txt
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)      431 2023-07-09 20:20:57.578611 LordPath-2023.7.9/PKG-INFO
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)       58 2023-03-19 09:41:22.000000 LordPath-2023.7.9/README.rst
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)      484 2023-07-09 20:20:53.000000 LordPath-2023.7.9/pyproject.toml
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)       38 2023-07-09 20:20:57.578814 LordPath-2023.7.9/setup.cfg
```

### Comparing `LordPath-2023.7.8.1/LordPath/__init__.py` & `LordPath-2023.7.9/LordPath/__init__.py`

 * *Files identical despite different names*

### Comparing `LordPath-2023.7.8.1/LordPath/dataset.py` & `LordPath-2023.7.9/LordPath/dataset.py`

 * *Files identical despite different names*

### Comparing `LordPath-2023.7.8.1/LordPath/descriptors.py` & `LordPath-2023.7.9/LordPath/descriptors.py`

 * *Files identical despite different names*

### Comparing `LordPath-2023.7.8.1/LordPath/filefolderclass.py` & `LordPath-2023.7.9/LordPath/filefolderclass.py`

 * *Files identical despite different names*

### Comparing `LordPath-2023.7.8.1/LordPath/opener/__init__.py` & `LordPath-2023.7.9/LordPath/opener/__init__.py`

 * *Files identical despite different names*

### Comparing `LordPath-2023.7.8.1/LordPath/opener/json.py` & `LordPath-2023.7.9/LordPath/opener/json.py`

 * *Files identical despite different names*

### Comparing `LordPath-2023.7.8.1/LordPath/opener/pickle.py` & `LordPath-2023.7.9/LordPath/opener/pickle.py`

 * *Files identical despite different names*

### Comparing `LordPath-2023.7.8.1/LordPath/opener/xml.py` & `LordPath-2023.7.9/LordPath/opener/xml.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from LordPath.opener import Opener
 
 
 def load_xml(file, default=None):
     return XmlOpener.load(file, default)
 
 
-def save_xml(file, default=None):
-    return XmlOpener.save(file, default)
+def save_xml(obj, file):
+    return XmlOpener.save(obj, file)
 
 
 class XmlOpener(Opener):
     compatible_endings = ['xml']
 
     @staticmethod
     def load(file, default=None) -> ET.Element:
```

### Comparing `LordPath-2023.7.8.1/LordPath/opener/yaml.py` & `LordPath-2023.7.9/LordPath/opener/yaml.py`

 * *Files identical despite different names*

