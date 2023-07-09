# Comparing `tmp/ddb_single-0.4.2.4.zip` & `tmp/ddb_single-0.4.3.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 18955 bytes, number of entries: 16
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-09 05:58 ddb_single-0.4.2.4/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-09 05:58 ddb_single-0.4.2.4/ddb_single/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-09 05:58 ddb_single-0.4.2.4/ddb_single.egg-info/
--rw-r--r--  2.0 unx       38 b- defN 23-Jul-09 05:58 ddb_single-0.4.2.4/setup.cfg
--rw-r--r--  2.0 unx     8806 b- defN 23-Jul-09 05:58 ddb_single-0.4.2.4/PKG-INFO
--rw-r--r--  2.0 unx      840 b- defN 23-Jul-09 05:57 ddb_single-0.4.2.4/setup.py
--rw-r--r--  2.0 unx    10375 b- defN 23-Jul-09 05:57 ddb_single-0.4.2.4/ddb_single/query.py
--rw-r--r--  2.0 unx    22402 b- defN 23-Jul-09 05:57 ddb_single-0.4.2.4/ddb_single/table.py
--rw-r--r--  2.0 unx    14953 b- defN 23-Jul-09 05:57 ddb_single-0.4.2.4/ddb_single/model.py
--rw-r--r--  2.0 unx      213 b- defN 23-Jul-09 05:58 ddb_single-0.4.2.4/ddb_single/__init__.py
--rw-r--r--  2.0 unx     6118 b- defN 23-Jul-09 05:57 ddb_single-0.4.2.4/ddb_single/utils_botos.py
--rw-r--r--  2.0 unx     8806 b- defN 23-Jul-09 05:58 ddb_single-0.4.2.4/ddb_single.egg-info/PKG-INFO
--rw-r--r--  2.0 unx       11 b- defN 23-Jul-09 05:58 ddb_single-0.4.2.4/ddb_single.egg-info/top_level.txt
--rw-r--r--  2.0 unx      286 b- defN 23-Jul-09 05:58 ddb_single-0.4.2.4/ddb_single.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Jul-09 05:58 ddb_single-0.4.2.4/ddb_single.egg-info/requires.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-09 05:58 ddb_single-0.4.2.4/ddb_single.egg-info/dependency_links.txt
-16 files, 72855 bytes uncompressed, 16461 bytes compressed:  77.4%
+Zip file size: 19139 bytes, number of entries: 16
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-09 06:10 ddb_single-0.4.3/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-09 06:10 ddb_single-0.4.3/ddb_single/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-09 06:10 ddb_single-0.4.3/ddb_single.egg-info/
+-rw-r--r--  2.0 unx       38 b- defN 23-Jul-09 06:10 ddb_single-0.4.3/setup.cfg
+-rw-r--r--  2.0 unx     8804 b- defN 23-Jul-09 06:10 ddb_single-0.4.3/PKG-INFO
+-rw-r--r--  2.0 unx     1167 b- defN 23-Jul-09 06:09 ddb_single-0.4.3/setup.py
+-rw-r--r--  2.0 unx    10375 b- defN 23-Jul-09 06:09 ddb_single-0.4.3/ddb_single/query.py
+-rw-r--r--  2.0 unx    22402 b- defN 23-Jul-09 06:09 ddb_single-0.4.3/ddb_single/table.py
+-rw-r--r--  2.0 unx    14953 b- defN 23-Jul-09 06:09 ddb_single-0.4.3/ddb_single/model.py
+-rw-r--r--  2.0 unx      211 b- defN 23-Jul-09 06:10 ddb_single-0.4.3/ddb_single/__init__.py
+-rw-r--r--  2.0 unx     6118 b- defN 23-Jul-09 06:09 ddb_single-0.4.3/ddb_single/utils_botos.py
+-rw-r--r--  2.0 unx     8804 b- defN 23-Jul-09 06:10 ddb_single-0.4.3/ddb_single.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-09 06:10 ddb_single-0.4.3/ddb_single.egg-info/top_level.txt
+-rw-r--r--  2.0 unx      286 b- defN 23-Jul-09 06:10 ddb_single-0.4.3/ddb_single.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Jul-09 06:10 ddb_single-0.4.3/ddb_single.egg-info/requires.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-09 06:10 ddb_single-0.4.3/ddb_single.egg-info/dependency_links.txt
+16 files, 73176 bytes uncompressed, 16709 bytes compressed:  77.2%
```

## zipnote {}

```diff
@@ -1,49 +1,49 @@
-Filename: ddb_single-0.4.2.4/
+Filename: ddb_single-0.4.3/
 Comment: 
 
-Filename: ddb_single-0.4.2.4/ddb_single/
+Filename: ddb_single-0.4.3/ddb_single/
 Comment: 
 
-Filename: ddb_single-0.4.2.4/ddb_single.egg-info/
+Filename: ddb_single-0.4.3/ddb_single.egg-info/
 Comment: 
 
-Filename: ddb_single-0.4.2.4/setup.cfg
+Filename: ddb_single-0.4.3/setup.cfg
 Comment: 
 
-Filename: ddb_single-0.4.2.4/PKG-INFO
+Filename: ddb_single-0.4.3/PKG-INFO
 Comment: 
 
-Filename: ddb_single-0.4.2.4/setup.py
+Filename: ddb_single-0.4.3/setup.py
 Comment: 
 
-Filename: ddb_single-0.4.2.4/ddb_single/query.py
+Filename: ddb_single-0.4.3/ddb_single/query.py
 Comment: 
 
-Filename: ddb_single-0.4.2.4/ddb_single/table.py
+Filename: ddb_single-0.4.3/ddb_single/table.py
 Comment: 
 
-Filename: ddb_single-0.4.2.4/ddb_single/model.py
+Filename: ddb_single-0.4.3/ddb_single/model.py
 Comment: 
 
-Filename: ddb_single-0.4.2.4/ddb_single/__init__.py
+Filename: ddb_single-0.4.3/ddb_single/__init__.py
 Comment: 
 
-Filename: ddb_single-0.4.2.4/ddb_single/utils_botos.py
+Filename: ddb_single-0.4.3/ddb_single/utils_botos.py
 Comment: 
 
-Filename: ddb_single-0.4.2.4/ddb_single.egg-info/PKG-INFO
+Filename: ddb_single-0.4.3/ddb_single.egg-info/PKG-INFO
 Comment: 
 
-Filename: ddb_single-0.4.2.4/ddb_single.egg-info/top_level.txt
+Filename: ddb_single-0.4.3/ddb_single.egg-info/top_level.txt
 Comment: 
 
-Filename: ddb_single-0.4.2.4/ddb_single.egg-info/SOURCES.txt
+Filename: ddb_single-0.4.3/ddb_single.egg-info/SOURCES.txt
 Comment: 
 
-Filename: ddb_single-0.4.2.4/ddb_single.egg-info/requires.txt
+Filename: ddb_single-0.4.3/ddb_single.egg-info/requires.txt
 Comment: 
 
-Filename: ddb_single-0.4.2.4/ddb_single.egg-info/dependency_links.txt
+Filename: ddb_single-0.4.3/ddb_single.egg-info/dependency_links.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `ddb_single-0.4.2.4/PKG-INFO` & `ddb_single-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddb_single
-Version: 0.4.2.4
+Version: 0.4.3
 Summary: Python DynamoDB interface, specialized in single-table design.
 Home-page: https://github.com/medaka0213/DynamoDB-SingleTable
 Author: medaka
 License: MIT
 Keywords: aws dynamodb serverless
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
```

## Comparing `ddb_single-0.4.2.4/ddb_single/query.py` & `ddb_single-0.4.3/ddb_single/query.py`

 * *Files identical despite different names*

## Comparing `ddb_single-0.4.2.4/ddb_single/table.py` & `ddb_single-0.4.3/ddb_single/table.py`

 * *Files identical despite different names*

## Comparing `ddb_single-0.4.2.4/ddb_single/model.py` & `ddb_single-0.4.3/ddb_single/model.py`

 * *Files identical despite different names*

## Comparing `ddb_single-0.4.2.4/ddb_single/utils_botos.py` & `ddb_single-0.4.3/ddb_single/utils_botos.py`

 * *Files identical despite different names*

## Comparing `ddb_single-0.4.2.4/ddb_single.egg-info/PKG-INFO` & `ddb_single-0.4.3/ddb_single.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddb-single
-Version: 0.4.2.4
+Version: 0.4.3
 Summary: Python DynamoDB interface, specialized in single-table design.
 Home-page: https://github.com/medaka0213/DynamoDB-SingleTable
 Author: medaka
 License: MIT
 Keywords: aws dynamodb serverless
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
```

