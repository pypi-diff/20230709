# Comparing `tmp/ddb_single-0.4.0.zip` & `tmp/ddb_single-0.4.1.zip`

## zipinfo {}

```diff
@@ -1,23 +1,24 @@
-Zip file size: 23449 bytes, number of entries: 21
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-01 10:21 ddb_single-0.4.0/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-01 10:21 ddb_single-0.4.0/tests/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-01 10:21 ddb_single-0.4.0/ddb_single/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-01 10:21 ddb_single-0.4.0/ddb_single.egg-info/
--rw-r--r--  2.0 unx       38 b- defN 23-Jul-01 10:21 ddb_single-0.4.0/setup.cfg
--rw-r--r--  2.0 unx      774 b- defN 23-Jul-01 10:20 ddb_single-0.4.0/setup.py
--rw-r--r--  2.0 unx     8804 b- defN 23-Jul-01 10:21 ddb_single-0.4.0/PKG-INFO
--rw-r--r--  2.0 unx     6403 b- defN 23-Jul-01 10:20 ddb_single-0.4.0/tests/test_query.py
--rw-r--r--  2.0 unx     2123 b- defN 23-Jul-01 10:20 ddb_single-0.4.0/tests/test_search.py
--rw-r--r--  2.0 unx     3706 b- defN 23-Jul-01 10:20 ddb_single-0.4.0/tests/test_relation.py
--rw-r--r--  2.0 unx     3036 b- defN 23-Jul-01 10:20 ddb_single-0.4.0/tests/test_batch.py
--rw-r--r--  2.0 unx      284 b- defN 23-Jul-01 10:20 ddb_single-0.4.0/ddb_single/__init__.py
--rw-r--r--  2.0 unx    22402 b- defN 23-Jul-01 10:20 ddb_single-0.4.0/ddb_single/table.py
--rw-r--r--  2.0 unx     6118 b- defN 23-Jul-01 10:20 ddb_single-0.4.0/ddb_single/utils_botos.py
--rw-r--r--  2.0 unx    13992 b- defN 23-Jul-01 10:20 ddb_single-0.4.0/ddb_single/model.py
--rw-r--r--  2.0 unx    10375 b- defN 23-Jul-01 10:20 ddb_single-0.4.0/ddb_single/query.py
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-01 10:21 ddb_single-0.4.0/ddb_single.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Jul-01 10:21 ddb_single-0.4.0/ddb_single.egg-info/requires.txt
--rw-r--r--  2.0 unx       11 b- defN 23-Jul-01 10:21 ddb_single-0.4.0/ddb_single.egg-info/top_level.txt
--rw-r--r--  2.0 unx     8804 b- defN 23-Jul-01 10:21 ddb_single-0.4.0/ddb_single.egg-info/PKG-INFO
--rw-r--r--  2.0 unx      370 b- defN 23-Jul-01 10:21 ddb_single-0.4.0/ddb_single.egg-info/SOURCES.txt
-21 files, 87247 bytes uncompressed, 20297 bytes compressed:  76.7%
+Zip file size: 24633 bytes, number of entries: 22
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-09 05:02 ddb_single-0.4.1/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-09 05:02 ddb_single-0.4.1/ddb_single/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-09 05:02 ddb_single-0.4.1/ddb_single.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-09 05:02 ddb_single-0.4.1/tests/
+-rw-r--r--  2.0 unx       38 b- defN 23-Jul-09 05:02 ddb_single-0.4.1/setup.cfg
+-rw-r--r--  2.0 unx     8804 b- defN 23-Jul-09 05:02 ddb_single-0.4.1/PKG-INFO
+-rw-r--r--  2.0 unx      824 b- defN 23-Jul-09 05:02 ddb_single-0.4.1/setup.py
+-rw-r--r--  2.0 unx    10375 b- defN 23-Jul-09 05:02 ddb_single-0.4.1/ddb_single/query.py
+-rw-r--r--  2.0 unx    22402 b- defN 23-Jul-09 05:02 ddb_single-0.4.1/ddb_single/table.py
+-rw-r--r--  2.0 unx    14953 b- defN 23-Jul-09 05:02 ddb_single-0.4.1/ddb_single/model.py
+-rw-r--r--  2.0 unx      284 b- defN 23-Jul-09 05:02 ddb_single-0.4.1/ddb_single/__init__.py
+-rw-r--r--  2.0 unx     6118 b- defN 23-Jul-09 05:02 ddb_single-0.4.1/ddb_single/utils_botos.py
+-rw-r--r--  2.0 unx     8804 b- defN 23-Jul-09 05:02 ddb_single-0.4.1/ddb_single.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-09 05:02 ddb_single-0.4.1/ddb_single.egg-info/top_level.txt
+-rw-r--r--  2.0 unx      389 b- defN 23-Jul-09 05:02 ddb_single-0.4.1/ddb_single.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Jul-09 05:02 ddb_single-0.4.1/ddb_single.egg-info/requires.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-09 05:02 ddb_single-0.4.1/ddb_single.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx     6403 b- defN 23-Jul-09 05:02 ddb_single-0.4.1/tests/test_query.py
+-rw-r--r--  2.0 unx     5926 b- defN 23-Jul-09 05:02 ddb_single-0.4.1/tests/test_desc.py
+-rw-r--r--  2.0 unx     3036 b- defN 23-Jul-09 05:02 ddb_single-0.4.1/tests/test_batch.py
+-rw-r--r--  2.0 unx     3706 b- defN 23-Jul-09 05:02 ddb_single-0.4.1/tests/test_relation.py
+-rw-r--r--  2.0 unx     2123 b- defN 23-Jul-09 05:02 ddb_single-0.4.1/tests/test_search.py
+22 files, 94203 bytes uncompressed, 21335 bytes compressed:  77.4%
```

## zipnote {}

```diff
@@ -1,64 +1,67 @@
-Filename: ddb_single-0.4.0/
+Filename: ddb_single-0.4.1/
 Comment: 
 
-Filename: ddb_single-0.4.0/tests/
+Filename: ddb_single-0.4.1/ddb_single/
 Comment: 
 
-Filename: ddb_single-0.4.0/ddb_single/
+Filename: ddb_single-0.4.1/ddb_single.egg-info/
 Comment: 
 
-Filename: ddb_single-0.4.0/ddb_single.egg-info/
+Filename: ddb_single-0.4.1/tests/
 Comment: 
 
-Filename: ddb_single-0.4.0/setup.cfg
+Filename: ddb_single-0.4.1/setup.cfg
 Comment: 
 
-Filename: ddb_single-0.4.0/setup.py
+Filename: ddb_single-0.4.1/PKG-INFO
 Comment: 
 
-Filename: ddb_single-0.4.0/PKG-INFO
+Filename: ddb_single-0.4.1/setup.py
 Comment: 
 
-Filename: ddb_single-0.4.0/tests/test_query.py
+Filename: ddb_single-0.4.1/ddb_single/query.py
 Comment: 
 
-Filename: ddb_single-0.4.0/tests/test_search.py
+Filename: ddb_single-0.4.1/ddb_single/table.py
 Comment: 
 
-Filename: ddb_single-0.4.0/tests/test_relation.py
+Filename: ddb_single-0.4.1/ddb_single/model.py
 Comment: 
 
-Filename: ddb_single-0.4.0/tests/test_batch.py
+Filename: ddb_single-0.4.1/ddb_single/__init__.py
 Comment: 
 
-Filename: ddb_single-0.4.0/ddb_single/__init__.py
+Filename: ddb_single-0.4.1/ddb_single/utils_botos.py
 Comment: 
 
-Filename: ddb_single-0.4.0/ddb_single/table.py
+Filename: ddb_single-0.4.1/ddb_single.egg-info/PKG-INFO
 Comment: 
 
-Filename: ddb_single-0.4.0/ddb_single/utils_botos.py
+Filename: ddb_single-0.4.1/ddb_single.egg-info/top_level.txt
 Comment: 
 
-Filename: ddb_single-0.4.0/ddb_single/model.py
+Filename: ddb_single-0.4.1/ddb_single.egg-info/SOURCES.txt
 Comment: 
 
-Filename: ddb_single-0.4.0/ddb_single/query.py
+Filename: ddb_single-0.4.1/ddb_single.egg-info/requires.txt
 Comment: 
 
-Filename: ddb_single-0.4.0/ddb_single.egg-info/dependency_links.txt
+Filename: ddb_single-0.4.1/ddb_single.egg-info/dependency_links.txt
 Comment: 
 
-Filename: ddb_single-0.4.0/ddb_single.egg-info/requires.txt
+Filename: ddb_single-0.4.1/tests/test_query.py
 Comment: 
 
-Filename: ddb_single-0.4.0/ddb_single.egg-info/top_level.txt
+Filename: ddb_single-0.4.1/tests/test_desc.py
 Comment: 
 
-Filename: ddb_single-0.4.0/ddb_single.egg-info/PKG-INFO
+Filename: ddb_single-0.4.1/tests/test_batch.py
 Comment: 
 
-Filename: ddb_single-0.4.0/ddb_single.egg-info/SOURCES.txt
+Filename: ddb_single-0.4.1/tests/test_relation.py
+Comment: 
+
+Filename: ddb_single-0.4.1/tests/test_search.py
 Comment: 
 
 Zip file comment:
```

## Comparing `ddb_single-0.4.0/setup.py` & `ddb_single-0.4.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import ddb_single
+import os
 from setuptools import setup
 
-with open("readme.md", "r") as fp:
-    LONG_DESCRIPTION = fp.read()
+if os.path.exists("readme.md"):
+    with open("readme.md", "r") as fp:
+        LONG_DESCRIPTION = fp.read()
 
 with open("requirements.txt", "r") as fp:
     INSTALL_REQUIRES = fp.read().splitlines()
 
-
 setup(
     name="ddb_single",
     version=ddb_single.__version__,
     description="Python DynamoDB interface, specialized in single-table design.",
     url="https://github.com/medaka0213/DynamoDB-SingleTable",
     author="medaka",
     license="MIT",
```

## Comparing `ddb_single-0.4.0/PKG-INFO` & `ddb_single-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddb_single
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python DynamoDB interface, specialized in single-table design.
 Home-page: https://github.com/medaka0213/DynamoDB-SingleTable
 Author: medaka
 License: MIT
 Keywords: aws dynamodb serverless
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
```

## Comparing `ddb_single-0.4.0/tests/test_query.py` & `ddb_single-0.4.1/tests/test_query.py`

 * *Files identical despite different names*

## Comparing `ddb_single-0.4.0/tests/test_search.py` & `ddb_single-0.4.1/tests/test_search.py`

 * *Files identical despite different names*

## Comparing `ddb_single-0.4.0/tests/test_relation.py` & `ddb_single-0.4.1/tests/test_relation.py`

 * *Files identical despite different names*

## Comparing `ddb_single-0.4.0/tests/test_batch.py` & `ddb_single-0.4.1/tests/test_batch.py`

 * *Files identical despite different names*

## Comparing `ddb_single-0.4.0/ddb_single/table.py` & `ddb_single-0.4.1/ddb_single/table.py`

 * *Files identical despite different names*

## Comparing `ddb_single-0.4.0/ddb_single/utils_botos.py` & `ddb_single-0.4.1/ddb_single/utils_botos.py`

 * *Files identical despite different names*

## Comparing `ddb_single-0.4.0/ddb_single/model.py` & `ddb_single-0.4.1/ddb_single/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -81,14 +81,27 @@
         return self.type in [
             FieldType.LIST,
             FieldType.STRING_SET,
             FieldType.NUMBER_SET,
             FieldType.BINARY_SET,
         ]
 
+    def describe(self):
+        return {
+            "type": self.type.name,
+            "nullable": self.nullable,
+            "primary_key": self.primary_key,
+            "secondary_key": self.secondary_key,
+            "unique_key": self.unique_key,
+            "search_key": self.search_key,
+            "relation": self.relation.__model_name__ if self.relation else None,
+            "reletion_by_unique": self.reletion_by_unique,
+            "ignore_case": self.ignore_case,
+        }
+
     def validate(self, value=None, skip=False):
         """
         Args:
             value: The value to be validated. If not provided, the value of the field will be used.
         Returns:
             The validated value.
         """
@@ -398,11 +411,27 @@
         """
         Args:
             key: DBField name.
         Returns:
             DBField: DBField instance.
         """
         res = self.__class__.__dict__.get(key)
-        print("__getitem__", res)
+        logger.debug(f"__getitem__ {res}")
         if isinstance(res, DBField):
             return res
         raise KeyError(f"Key {key} not found")
+
+    @classmethod
+    def describe(cls):
+        """
+        Returns:
+            dict: The description of the model.
+        """
+        fields = {}
+        for k, v in cls.__dict__.items():
+            if isinstance(v, DBField):
+                fields[k] = v.describe()
+        return {
+            "model_name": cls.__model_name__,
+            "table_name": cls.__table__.__table_name__,
+            "fields": fields,
+        }
```

## Comparing `ddb_single-0.4.0/ddb_single/query.py` & `ddb_single-0.4.1/ddb_single/query.py`

 * *Files identical despite different names*

## Comparing `ddb_single-0.4.0/ddb_single.egg-info/PKG-INFO` & `ddb_single-0.4.1/ddb_single.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddb-single
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python DynamoDB interface, specialized in single-table design.
 Home-page: https://github.com/medaka0213/DynamoDB-SingleTable
 Author: medaka
 License: MIT
 Keywords: aws dynamodb serverless
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
```

