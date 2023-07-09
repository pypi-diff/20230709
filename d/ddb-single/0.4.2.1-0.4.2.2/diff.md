# Comparing `tmp/ddb_single-0.4.2.1.zip` & `tmp/ddb_single-0.4.2.2.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 24702 bytes, number of entries: 22
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-09 05:25 ddb_single-0.4.2.1/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-09 05:25 ddb_single-0.4.2.1/ddb_single/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-09 05:25 ddb_single-0.4.2.1/ddb_single.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-09 05:25 ddb_single-0.4.2.1/tests/
--rw-r--r--  2.0 unx       38 b- defN 23-Jul-09 05:25 ddb_single-0.4.2.1/setup.cfg
--rw-r--r--  2.0 unx     8806 b- defN 23-Jul-09 05:25 ddb_single-0.4.2.1/PKG-INFO
--rw-r--r--  2.0 unx      784 b- defN 23-Jul-09 05:25 ddb_single-0.4.2.1/setup.py
--rw-r--r--  2.0 unx    10375 b- defN 23-Jul-09 05:25 ddb_single-0.4.2.1/ddb_single/query.py
--rw-r--r--  2.0 unx    22402 b- defN 23-Jul-09 05:25 ddb_single-0.4.2.1/ddb_single/table.py
--rw-r--r--  2.0 unx    14953 b- defN 23-Jul-09 05:25 ddb_single-0.4.2.1/ddb_single/model.py
--rw-r--r--  2.0 unx      284 b- defN 23-Jul-09 05:25 ddb_single-0.4.2.1/ddb_single/__init__.py
--rw-r--r--  2.0 unx     6118 b- defN 23-Jul-09 05:25 ddb_single-0.4.2.1/ddb_single/utils_botos.py
--rw-r--r--  2.0 unx     8806 b- defN 23-Jul-09 05:25 ddb_single-0.4.2.1/ddb_single.egg-info/PKG-INFO
--rw-r--r--  2.0 unx       11 b- defN 23-Jul-09 05:25 ddb_single-0.4.2.1/ddb_single.egg-info/top_level.txt
--rw-r--r--  2.0 unx      389 b- defN 23-Jul-09 05:25 ddb_single-0.4.2.1/ddb_single.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Jul-09 05:25 ddb_single-0.4.2.1/ddb_single.egg-info/requires.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-09 05:25 ddb_single-0.4.2.1/ddb_single.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx     6403 b- defN 23-Jul-09 05:25 ddb_single-0.4.2.1/tests/test_query.py
--rw-r--r--  2.0 unx     5926 b- defN 23-Jul-09 05:25 ddb_single-0.4.2.1/tests/test_desc.py
--rw-r--r--  2.0 unx     3036 b- defN 23-Jul-09 05:25 ddb_single-0.4.2.1/tests/test_batch.py
--rw-r--r--  2.0 unx     3706 b- defN 23-Jul-09 05:25 ddb_single-0.4.2.1/tests/test_relation.py
--rw-r--r--  2.0 unx     2123 b- defN 23-Jul-09 05:25 ddb_single-0.4.2.1/tests/test_search.py
-22 files, 94167 bytes uncompressed, 21316 bytes compressed:  77.4%
+Zip file size: 24722 bytes, number of entries: 22
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-09 05:33 ddb_single-0.4.2.2/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-09 05:33 ddb_single-0.4.2.2/ddb_single/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-09 05:33 ddb_single-0.4.2.2/ddb_single.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-09 05:33 ddb_single-0.4.2.2/tests/
+-rw-r--r--  2.0 unx       38 b- defN 23-Jul-09 05:33 ddb_single-0.4.2.2/setup.cfg
+-rw-r--r--  2.0 unx     8806 b- defN 23-Jul-09 05:33 ddb_single-0.4.2.2/PKG-INFO
+-rw-r--r--  2.0 unx      840 b- defN 23-Jul-09 05:33 ddb_single-0.4.2.2/setup.py
+-rw-r--r--  2.0 unx    10375 b- defN 23-Jul-09 05:33 ddb_single-0.4.2.2/ddb_single/query.py
+-rw-r--r--  2.0 unx    22402 b- defN 23-Jul-09 05:33 ddb_single-0.4.2.2/ddb_single/table.py
+-rw-r--r--  2.0 unx    14953 b- defN 23-Jul-09 05:33 ddb_single-0.4.2.2/ddb_single/model.py
+-rw-r--r--  2.0 unx      284 b- defN 23-Jul-09 05:33 ddb_single-0.4.2.2/ddb_single/__init__.py
+-rw-r--r--  2.0 unx     6118 b- defN 23-Jul-09 05:33 ddb_single-0.4.2.2/ddb_single/utils_botos.py
+-rw-r--r--  2.0 unx     8806 b- defN 23-Jul-09 05:33 ddb_single-0.4.2.2/ddb_single.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-09 05:33 ddb_single-0.4.2.2/ddb_single.egg-info/top_level.txt
+-rw-r--r--  2.0 unx      389 b- defN 23-Jul-09 05:33 ddb_single-0.4.2.2/ddb_single.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Jul-09 05:33 ddb_single-0.4.2.2/ddb_single.egg-info/requires.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-09 05:33 ddb_single-0.4.2.2/ddb_single.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx     6403 b- defN 23-Jul-09 05:33 ddb_single-0.4.2.2/tests/test_query.py
+-rw-r--r--  2.0 unx     5926 b- defN 23-Jul-09 05:33 ddb_single-0.4.2.2/tests/test_desc.py
+-rw-r--r--  2.0 unx     3036 b- defN 23-Jul-09 05:33 ddb_single-0.4.2.2/tests/test_batch.py
+-rw-r--r--  2.0 unx     3706 b- defN 23-Jul-09 05:33 ddb_single-0.4.2.2/tests/test_relation.py
+-rw-r--r--  2.0 unx     2123 b- defN 23-Jul-09 05:33 ddb_single-0.4.2.2/tests/test_search.py
+22 files, 94223 bytes uncompressed, 21336 bytes compressed:  77.4%
```

## zipnote {}

```diff
@@ -1,67 +1,67 @@
-Filename: ddb_single-0.4.2.1/
+Filename: ddb_single-0.4.2.2/
 Comment: 
 
-Filename: ddb_single-0.4.2.1/ddb_single/
+Filename: ddb_single-0.4.2.2/ddb_single/
 Comment: 
 
-Filename: ddb_single-0.4.2.1/ddb_single.egg-info/
+Filename: ddb_single-0.4.2.2/ddb_single.egg-info/
 Comment: 
 
-Filename: ddb_single-0.4.2.1/tests/
+Filename: ddb_single-0.4.2.2/tests/
 Comment: 
 
-Filename: ddb_single-0.4.2.1/setup.cfg
+Filename: ddb_single-0.4.2.2/setup.cfg
 Comment: 
 
-Filename: ddb_single-0.4.2.1/PKG-INFO
+Filename: ddb_single-0.4.2.2/PKG-INFO
 Comment: 
 
-Filename: ddb_single-0.4.2.1/setup.py
+Filename: ddb_single-0.4.2.2/setup.py
 Comment: 
 
-Filename: ddb_single-0.4.2.1/ddb_single/query.py
+Filename: ddb_single-0.4.2.2/ddb_single/query.py
 Comment: 
 
-Filename: ddb_single-0.4.2.1/ddb_single/table.py
+Filename: ddb_single-0.4.2.2/ddb_single/table.py
 Comment: 
 
-Filename: ddb_single-0.4.2.1/ddb_single/model.py
+Filename: ddb_single-0.4.2.2/ddb_single/model.py
 Comment: 
 
-Filename: ddb_single-0.4.2.1/ddb_single/__init__.py
+Filename: ddb_single-0.4.2.2/ddb_single/__init__.py
 Comment: 
 
-Filename: ddb_single-0.4.2.1/ddb_single/utils_botos.py
+Filename: ddb_single-0.4.2.2/ddb_single/utils_botos.py
 Comment: 
 
-Filename: ddb_single-0.4.2.1/ddb_single.egg-info/PKG-INFO
+Filename: ddb_single-0.4.2.2/ddb_single.egg-info/PKG-INFO
 Comment: 
 
-Filename: ddb_single-0.4.2.1/ddb_single.egg-info/top_level.txt
+Filename: ddb_single-0.4.2.2/ddb_single.egg-info/top_level.txt
 Comment: 
 
-Filename: ddb_single-0.4.2.1/ddb_single.egg-info/SOURCES.txt
+Filename: ddb_single-0.4.2.2/ddb_single.egg-info/SOURCES.txt
 Comment: 
 
-Filename: ddb_single-0.4.2.1/ddb_single.egg-info/requires.txt
+Filename: ddb_single-0.4.2.2/ddb_single.egg-info/requires.txt
 Comment: 
 
-Filename: ddb_single-0.4.2.1/ddb_single.egg-info/dependency_links.txt
+Filename: ddb_single-0.4.2.2/ddb_single.egg-info/dependency_links.txt
 Comment: 
 
-Filename: ddb_single-0.4.2.1/tests/test_query.py
+Filename: ddb_single-0.4.2.2/tests/test_query.py
 Comment: 
 
-Filename: ddb_single-0.4.2.1/tests/test_desc.py
+Filename: ddb_single-0.4.2.2/tests/test_desc.py
 Comment: 
 
-Filename: ddb_single-0.4.2.1/tests/test_batch.py
+Filename: ddb_single-0.4.2.2/tests/test_batch.py
 Comment: 
 
-Filename: ddb_single-0.4.2.1/tests/test_relation.py
+Filename: ddb_single-0.4.2.2/tests/test_relation.py
 Comment: 
 
-Filename: ddb_single-0.4.2.1/tests/test_search.py
+Filename: ddb_single-0.4.2.2/tests/test_search.py
 Comment: 
 
 Zip file comment:
```

## Comparing `ddb_single-0.4.2.1/PKG-INFO` & `ddb_single-0.4.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddb_single
-Version: 0.4.2.1
+Version: 0.4.2.2
 Summary: Python DynamoDB interface, specialized in single-table design.
 Home-page: https://github.com/medaka0213/DynamoDB-SingleTable
 Author: medaka
 License: MIT
 Keywords: aws dynamodb serverless
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
```

## Comparing `ddb_single-0.4.2.1/setup.py` & `ddb_single-0.4.2.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 DESCRIPTION = "Python DynamoDB interface, specialized in single-table design."
 LONG_DESCRIPTION = DESCRIPTION
 if os.path.exists("readme.md"):
     with open("readme.md", "r") as fp:
         LONG_DESCRIPTION = fp.read()
 
+print("ddb_single version:", ddb_single.__version__)
+
 setup(
     name="ddb_single",
     version=ddb_single.__version__,
     description=DESCRIPTION,
     url="https://github.com/medaka0213/DynamoDB-SingleTable",
     author="medaka",
     license="MIT",
```

## Comparing `ddb_single-0.4.2.1/ddb_single/query.py` & `ddb_single-0.4.2.2/ddb_single/query.py`

 * *Files identical despite different names*

## Comparing `ddb_single-0.4.2.1/ddb_single/table.py` & `ddb_single-0.4.2.2/ddb_single/table.py`

 * *Files identical despite different names*

## Comparing `ddb_single-0.4.2.1/ddb_single/model.py` & `ddb_single-0.4.2.2/ddb_single/model.py`

 * *Files identical despite different names*

## Comparing `ddb_single-0.4.2.1/ddb_single/utils_botos.py` & `ddb_single-0.4.2.2/ddb_single/utils_botos.py`

 * *Files identical despite different names*

## Comparing `ddb_single-0.4.2.1/ddb_single.egg-info/PKG-INFO` & `ddb_single-0.4.2.2/ddb_single.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddb-single
-Version: 0.4.2.1
+Version: 0.4.2.2
 Summary: Python DynamoDB interface, specialized in single-table design.
 Home-page: https://github.com/medaka0213/DynamoDB-SingleTable
 Author: medaka
 License: MIT
 Keywords: aws dynamodb serverless
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
```

## Comparing `ddb_single-0.4.2.1/tests/test_query.py` & `ddb_single-0.4.2.2/tests/test_query.py`

 * *Files identical despite different names*

## Comparing `ddb_single-0.4.2.1/tests/test_desc.py` & `ddb_single-0.4.2.2/tests/test_desc.py`

 * *Files identical despite different names*

## Comparing `ddb_single-0.4.2.1/tests/test_batch.py` & `ddb_single-0.4.2.2/tests/test_batch.py`

 * *Files identical despite different names*

## Comparing `ddb_single-0.4.2.1/tests/test_relation.py` & `ddb_single-0.4.2.2/tests/test_relation.py`

 * *Files identical despite different names*

## Comparing `ddb_single-0.4.2.1/tests/test_search.py` & `ddb_single-0.4.2.2/tests/test_search.py`

 * *Files identical despite different names*

