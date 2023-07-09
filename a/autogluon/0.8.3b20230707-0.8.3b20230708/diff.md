# Comparing `tmp/autogluon-0.8.3b20230707.tar.gz` & `tmp/autogluon-0.8.3b20230708.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon-0.8.3b20230707.tar", last modified: Fri Jul  7 09:04:46 2023, max compression
+gzip compressed data, was "autogluon-0.8.3b20230708.tar", last modified: Sat Jul  8 09:04:43 2023, max compression
```

## Comparing `autogluon-0.8.3b20230707.tar` & `autogluon-0.8.3b20230708.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:04:46.013241 autogluon-0.8.3b20230707/
--rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-07-07 09:04:46.013241 autogluon-0.8.3b20230707/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 09:04:46.013241 autogluon-0.8.3b20230707/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-07 09:03:45.000000 autogluon-0.8.3b20230707/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:04:46.009241 autogluon-0.8.3b20230707/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:04:46.009241 autogluon-0.8.3b20230707/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:04:46.013241 autogluon-0.8.3b20230707/src/autogluon/_internal_/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 09:03:45.000000 autogluon-0.8.3b20230707/src/autogluon/_internal_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:04:46.013241 autogluon-0.8.3b20230707/src/autogluon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-07-07 09:04:45.000000 autogluon-0.8.3b20230707/src/autogluon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-07 09:04:45.000000 autogluon-0.8.3b20230707/src/autogluon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 09:04:45.000000 autogluon-0.8.3b20230707/src/autogluon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 09:04:45.000000 autogluon-0.8.3b20230707/src/autogluon.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-07 09:04:45.000000 autogluon-0.8.3b20230707/src/autogluon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 09:04:45.000000 autogluon-0.8.3b20230707/src/autogluon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 09:04:45.000000 autogluon-0.8.3b20230707/src/autogluon.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:04:43.197320 autogluon-0.8.3b20230708/
+-rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-07-08 09:04:43.197320 autogluon-0.8.3b20230708/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 09:04:43.197320 autogluon-0.8.3b20230708/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-08 09:03:52.000000 autogluon-0.8.3b20230708/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:04:43.193320 autogluon-0.8.3b20230708/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:04:43.193320 autogluon-0.8.3b20230708/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:04:43.197320 autogluon-0.8.3b20230708/src/autogluon/_internal_/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 09:03:52.000000 autogluon-0.8.3b20230708/src/autogluon/_internal_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:04:43.197320 autogluon-0.8.3b20230708/src/autogluon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-07-08 09:04:43.000000 autogluon-0.8.3b20230708/src/autogluon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-08 09:04:43.000000 autogluon-0.8.3b20230708/src/autogluon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 09:04:43.000000 autogluon-0.8.3b20230708/src/autogluon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-08 09:04:43.000000 autogluon-0.8.3b20230708/src/autogluon.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-08 09:04:43.000000 autogluon-0.8.3b20230708/src/autogluon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-08 09:04:43.000000 autogluon-0.8.3b20230708/src/autogluon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 09:04:43.000000 autogluon-0.8.3b20230708/src/autogluon.egg-info/zip-safe
```

### Comparing `autogluon-0.8.3b20230707/PKG-INFO` & `autogluon-0.8.3b20230708/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 0.8.3b20230707
+Version: 0.8.3b20230708
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon-0.8.3b20230707/setup.py` & `autogluon-0.8.3b20230708/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon-0.8.3b20230707/src/autogluon.egg-info/PKG-INFO` & `autogluon-0.8.3b20230708/src/autogluon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 0.8.3b20230707
+Version: 0.8.3b20230708
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

