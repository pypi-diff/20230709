# Comparing `tmp/nescs-0.3.4.tar.gz` & `tmp/nescs-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nescs-0.3.4.tar", last modified: Sun Jul  9 07:45:10 2023, max compression
+gzip compressed data, was "nescs-0.3.5.tar", last modified: Sun Jul  9 07:48:36 2023, max compression
```

## Comparing `nescs-0.3.4.tar` & `nescs-0.3.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 twoics    (1000) twoics    (1000)        0 2023-07-09 07:45:10.691254 nescs-0.3.4/
--rw-r--r--   0 twoics    (1000) twoics    (1000)      104 2023-07-08 05:36:40.000000 nescs-0.3.4/MANIFEST.in
--rw-r--r--   0 twoics    (1000) twoics    (1000)     5092 2023-07-09 07:45:10.691254 nescs-0.3.4/PKG-INFO
--rw-r--r--   0 twoics    (1000) twoics    (1000)     4837 2023-07-09 03:13:48.000000 nescs-0.3.4/README.rst
-drwxr-xr-x   0 twoics    (1000) twoics    (1000)        0 2023-07-09 07:45:10.691254 nescs-0.3.4/nesc/
--rw-r--r--   0 twoics    (1000) twoics    (1000)       45 2023-07-08 05:36:40.000000 nescs-0.3.4/nesc/__init__.py
--rw-r--r--   0 twoics    (1000) twoics    (1000)     6964 2023-07-09 03:13:48.000000 nescs-0.3.4/nesc/service.py
-drwxr-xr-x   0 twoics    (1000) twoics    (1000)        0 2023-07-09 07:45:10.691254 nescs-0.3.4/nescs.egg-info/
--rw-r--r--   0 twoics    (1000) twoics    (1000)     5092 2023-07-09 07:45:10.000000 nescs-0.3.4/nescs.egg-info/PKG-INFO
--rw-r--r--   0 twoics    (1000) twoics    (1000)      233 2023-07-09 07:45:10.000000 nescs-0.3.4/nescs.egg-info/SOURCES.txt
--rw-r--r--   0 twoics    (1000) twoics    (1000)        1 2023-07-09 07:45:10.000000 nescs-0.3.4/nescs.egg-info/dependency_links.txt
--rw-r--r--   0 twoics    (1000) twoics    (1000)       42 2023-07-09 07:45:10.000000 nescs-0.3.4/nescs.egg-info/requires.txt
--rw-r--r--   0 twoics    (1000) twoics    (1000)        5 2023-07-09 07:45:10.000000 nescs-0.3.4/nescs.egg-info/top_level.txt
--rw-r--r--   0 twoics    (1000) twoics    (1000)       88 2023-07-09 06:58:46.000000 nescs-0.3.4/pyproject.toml
--rw-r--r--   0 twoics    (1000) twoics    (1000)      446 2023-07-09 07:45:10.691254 nescs-0.3.4/setup.cfg
--rw-r--r--   0 twoics    (1000) twoics    (1000)      131 2023-07-09 06:58:46.000000 nescs-0.3.4/setup.py
+drwxr-xr-x   0 twoics    (1000) twoics    (1000)        0 2023-07-09 07:48:36.527591 nescs-0.3.5/
+-rw-r--r--   0 twoics    (1000) twoics    (1000)      104 2023-07-08 05:36:40.000000 nescs-0.3.5/MANIFEST.in
+-rw-r--r--   0 twoics    (1000) twoics    (1000)     5091 2023-07-09 07:48:36.527591 nescs-0.3.5/PKG-INFO
+-rw-r--r--   0 twoics    (1000) twoics    (1000)     4837 2023-07-09 03:13:48.000000 nescs-0.3.5/README.rst
+drwxr-xr-x   0 twoics    (1000) twoics    (1000)        0 2023-07-09 07:48:36.527591 nescs-0.3.5/nesc/
+-rw-r--r--   0 twoics    (1000) twoics    (1000)       45 2023-07-08 05:36:40.000000 nescs-0.3.5/nesc/__init__.py
+-rw-r--r--   0 twoics    (1000) twoics    (1000)     6964 2023-07-09 03:13:48.000000 nescs-0.3.5/nesc/service.py
+drwxr-xr-x   0 twoics    (1000) twoics    (1000)        0 2023-07-09 07:48:36.527591 nescs-0.3.5/nescs.egg-info/
+-rw-r--r--   0 twoics    (1000) twoics    (1000)     5091 2023-07-09 07:48:36.000000 nescs-0.3.5/nescs.egg-info/PKG-INFO
+-rw-r--r--   0 twoics    (1000) twoics    (1000)      233 2023-07-09 07:48:36.000000 nescs-0.3.5/nescs.egg-info/SOURCES.txt
+-rw-r--r--   0 twoics    (1000) twoics    (1000)        1 2023-07-09 07:48:36.000000 nescs-0.3.5/nescs.egg-info/dependency_links.txt
+-rw-r--r--   0 twoics    (1000) twoics    (1000)       42 2023-07-09 07:48:36.000000 nescs-0.3.5/nescs.egg-info/requires.txt
+-rw-r--r--   0 twoics    (1000) twoics    (1000)        5 2023-07-09 07:48:36.000000 nescs-0.3.5/nescs.egg-info/top_level.txt
+-rw-r--r--   0 twoics    (1000) twoics    (1000)       88 2023-07-09 06:58:46.000000 nescs-0.3.5/pyproject.toml
+-rw-r--r--   0 twoics    (1000) twoics    (1000)      445 2023-07-09 07:48:36.528591 nescs-0.3.5/setup.cfg
+-rw-r--r--   0 twoics    (1000) twoics    (1000)      131 2023-07-09 06:58:46.000000 nescs-0.3.5/setup.py
```

### Comparing `nescs-0.3.4/PKG-INFO` & `nescs-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: nescs
-Version: 0.3.4
+Version: 0.3.5
 Summary: Библиотека создания моделей вложенных сериализаторов
-Home-page: https://github.com/twoics/nesc,
+Home-page: https://github.com/twoics/nesc
 Author: cifra-k
 License: MIT
 Requires-Python: >=3.8
 
 =====
 NESCS
 =====
```

### Comparing `nescs-0.3.4/README.rst` & `nescs-0.3.5/README.rst`

 * *Files identical despite different names*

### Comparing `nescs-0.3.4/nesc/service.py` & `nescs-0.3.5/nesc/service.py`

 * *Files identical despite different names*

### Comparing `nescs-0.3.4/nescs.egg-info/PKG-INFO` & `nescs-0.3.5/nescs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: nescs
-Version: 0.3.4
+Version: 0.3.5
 Summary: Библиотека создания моделей вложенных сериализаторов
-Home-page: https://github.com/twoics/nesc,
+Home-page: https://github.com/twoics/nesc
 Author: cifra-k
 License: MIT
 Requires-Python: >=3.8
 
 =====
 NESCS
 =====
```

