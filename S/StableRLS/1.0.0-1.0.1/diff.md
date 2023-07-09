# Comparing `tmp/StableRLS-1.0.0.tar.gz` & `tmp/StableRLS-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StableRLS-1.0.0.tar", last modified: Sun Jul  9 15:09:23 2023, max compression
+gzip compressed data, was "StableRLS-1.0.1.tar", last modified: Sun Jul  9 15:24:52 2023, max compression
```

## Comparing `StableRLS-1.0.0.tar` & `StableRLS-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 cao2851   (1000) cao2851   (1000)        0 2023-07-09 15:09:23.937448 StableRLS-1.0.0/
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)    35148 2023-03-21 15:46:09.000000 StableRLS-1.0.0/LICENSE.txt
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)      330 2023-07-09 15:09:23.937448 StableRLS-1.0.0/PKG-INFO
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)     4314 2023-07-09 15:09:21.000000 StableRLS-1.0.0/README.md
-drwxrwxr-x   0 cao2851   (1000) cao2851   (1000)        0 2023-07-09 15:09:23.933448 StableRLS-1.0.0/StableRLS.egg-info/
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)      330 2023-07-09 15:09:23.000000 StableRLS-1.0.0/StableRLS.egg-info/PKG-INFO
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)      307 2023-07-09 15:09:23.000000 StableRLS-1.0.0/StableRLS.egg-info/SOURCES.txt
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)        1 2023-07-09 15:09:23.000000 StableRLS-1.0.0/StableRLS.egg-info/dependency_links.txt
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)       37 2023-07-09 15:09:23.000000 StableRLS-1.0.0/StableRLS.egg-info/requires.txt
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)       10 2023-07-09 15:09:23.000000 StableRLS-1.0.0/StableRLS.egg-info/top_level.txt
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)       38 2023-07-09 15:09:23.937448 StableRLS-1.0.0/setup.cfg
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)      491 2023-07-09 14:54:06.000000 StableRLS-1.0.0/setup.py
-drwxrwxr-x   0 cao2851   (1000) cao2851   (1000)        0 2023-07-09 15:09:23.937448 StableRLS-1.0.0/stablerls/
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)        0 2023-03-21 15:46:09.000000 StableRLS-1.0.0/stablerls/__init__.py
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)     2918 2023-07-09 15:00:17.000000 StableRLS-1.0.0/stablerls/configreader.py
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)     2868 2023-07-09 15:00:25.000000 StableRLS-1.0.0/stablerls/createFMU.py
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)     4188 2023-07-01 15:03:04.000000 StableRLS-1.0.0/stablerls/fmutools.py
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)    17470 2023-07-01 15:03:05.000000 StableRLS-1.0.0/stablerls/gymFMU.py
+drwxrwxr-x   0 cao2851   (1000) cao2851   (1000)        0 2023-07-09 15:24:52.034358 StableRLS-1.0.1/
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)    35148 2023-03-21 15:46:09.000000 StableRLS-1.0.1/LICENSE.txt
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)     4686 2023-07-09 15:24:52.034358 StableRLS-1.0.1/PKG-INFO
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)     4314 2023-07-09 15:09:21.000000 StableRLS-1.0.1/README.md
+drwxrwxr-x   0 cao2851   (1000) cao2851   (1000)        0 2023-07-09 15:24:52.034358 StableRLS-1.0.1/StableRLS.egg-info/
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)     4686 2023-07-09 15:24:52.000000 StableRLS-1.0.1/StableRLS.egg-info/PKG-INFO
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)      307 2023-07-09 15:24:52.000000 StableRLS-1.0.1/StableRLS.egg-info/SOURCES.txt
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)        1 2023-07-09 15:24:52.000000 StableRLS-1.0.1/StableRLS.egg-info/dependency_links.txt
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)       37 2023-07-09 15:24:52.000000 StableRLS-1.0.1/StableRLS.egg-info/requires.txt
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)       10 2023-07-09 15:24:52.000000 StableRLS-1.0.1/StableRLS.egg-info/top_level.txt
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)       38 2023-07-09 15:24:52.034358 StableRLS-1.0.1/setup.cfg
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)      744 2023-07-09 15:24:11.000000 StableRLS-1.0.1/setup.py
+drwxrwxr-x   0 cao2851   (1000) cao2851   (1000)        0 2023-07-09 15:24:52.034358 StableRLS-1.0.1/stablerls/
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)        0 2023-03-21 15:46:09.000000 StableRLS-1.0.1/stablerls/__init__.py
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)     2918 2023-07-09 15:00:17.000000 StableRLS-1.0.1/stablerls/configreader.py
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)     2868 2023-07-09 15:00:25.000000 StableRLS-1.0.1/stablerls/createFMU.py
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)     4188 2023-07-01 15:03:04.000000 StableRLS-1.0.1/stablerls/fmutools.py
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)    17470 2023-07-01 15:03:05.000000 StableRLS-1.0.1/stablerls/gymFMU.py
```

### Comparing `StableRLS-1.0.0/LICENSE.txt` & `StableRLS-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `StableRLS-1.0.0/README.md` & `StableRLS-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `StableRLS-1.0.0/stablerls/configreader.py` & `StableRLS-1.0.1/stablerls/configreader.py`

 * *Files identical despite different names*

### Comparing `StableRLS-1.0.0/stablerls/createFMU.py` & `StableRLS-1.0.1/stablerls/createFMU.py`

 * *Files identical despite different names*

### Comparing `StableRLS-1.0.0/stablerls/fmutools.py` & `StableRLS-1.0.1/stablerls/fmutools.py`

 * *Files identical despite different names*

### Comparing `StableRLS-1.0.0/stablerls/gymFMU.py` & `StableRLS-1.0.1/stablerls/gymFMU.py`

 * *Files identical despite different names*

