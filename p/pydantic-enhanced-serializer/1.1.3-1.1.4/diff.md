# Comparing `tmp/pydantic_enhanced_serializer-1.1.3-py3-none-any.whl.zip` & `tmp/pydantic_enhanced_serializer-1.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 15729 bytes, number of entries: 15
+Zip file size: 15841 bytes, number of entries: 15
 -rw-r--r--  2.0 unx      309 b- defN 23-Mar-08 23:12 pydantic_enhanced_serializer/__init__.py
--rw-r--r--  2.0 unx     9424 b- defN 23-Apr-27 05:29 pydantic_enhanced_serializer/fieldsets.py
+-rw-r--r--  2.0 unx     9424 b- defN 23-Jul-08 03:07 pydantic_enhanced_serializer/fieldsets.py
 -rw-r--r--  2.0 unx     2724 b- defN 23-Jun-22 04:36 pydantic_enhanced_serializer/models.py
--rw-r--r--  2.0 unx     3960 b- defN 23-Mar-08 23:11 pydantic_enhanced_serializer/path_put.py
+-rw-r--r--  2.0 unx     4363 b- defN 23-Jul-08 22:14 pydantic_enhanced_serializer/path_put.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-08 23:11 pydantic_enhanced_serializer/py.typed
--rw-r--r--  2.0 unx     4222 b- defN 23-Jun-22 06:24 pydantic_enhanced_serializer/render.py
--rw-r--r--  2.0 unx     6632 b- defN 23-Jun-23 00:45 pydantic_enhanced_serializer/schema.py
+-rw-r--r--  2.0 unx     4222 b- defN 23-Jul-08 03:30 pydantic_enhanced_serializer/render.py
+-rw-r--r--  2.0 unx     6632 b- defN 23-Jul-08 02:01 pydantic_enhanced_serializer/schema.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-08 23:11 pydantic_enhanced_serializer/integrations/__init__.py
 -rw-r--r--  2.0 unx     1401 b- defN 23-Mar-08 23:47 pydantic_enhanced_serializer/integrations/django_ninja.py
 -rw-r--r--  2.0 unx     6078 b- defN 23-Mar-08 23:14 pydantic_enhanced_serializer/integrations/fastapi.py
--rw-r--r--  2.0 unx     1073 b- defN 23-Jun-23 01:06 pydantic_enhanced_serializer-1.1.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     6021 b- defN 23-Jun-23 01:06 pydantic_enhanced_serializer-1.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-23 01:06 pydantic_enhanced_serializer-1.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       29 b- defN 23-Jun-23 01:06 pydantic_enhanced_serializer-1.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1488 b- defN 23-Jun-23 01:06 pydantic_enhanced_serializer-1.1.3.dist-info/RECORD
-15 files, 43453 bytes uncompressed, 13171 bytes compressed:  69.7%
+-rw-r--r--  2.0 unx     1073 b- defN 23-Jul-08 22:17 pydantic_enhanced_serializer-1.1.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6021 b- defN 23-Jul-08 22:17 pydantic_enhanced_serializer-1.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-08 22:17 pydantic_enhanced_serializer-1.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       29 b- defN 23-Jul-08 22:17 pydantic_enhanced_serializer-1.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1488 b- defN 23-Jul-08 22:17 pydantic_enhanced_serializer-1.1.4.dist-info/RECORD
+15 files, 43856 bytes uncompressed, 13283 bytes compressed:  69.7%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: pydantic_enhanced_serializer/integrations/django_ninja.py
 Comment: 
 
 Filename: pydantic_enhanced_serializer/integrations/fastapi.py
 Comment: 
 
-Filename: pydantic_enhanced_serializer-1.1.3.dist-info/LICENSE
+Filename: pydantic_enhanced_serializer-1.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: pydantic_enhanced_serializer-1.1.3.dist-info/METADATA
+Filename: pydantic_enhanced_serializer-1.1.4.dist-info/METADATA
 Comment: 
 
-Filename: pydantic_enhanced_serializer-1.1.3.dist-info/WHEEL
+Filename: pydantic_enhanced_serializer-1.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: pydantic_enhanced_serializer-1.1.3.dist-info/top_level.txt
+Filename: pydantic_enhanced_serializer-1.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: pydantic_enhanced_serializer-1.1.3.dist-info/RECORD
+Filename: pydantic_enhanced_serializer-1.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pydantic_enhanced_serializer/path_put.py

```diff
@@ -59,14 +59,18 @@
 
     >>> path_put({"things": [{"s1": "v1"}]}, "things.0", {"s2": "v2"})
     {'things': [{'s1': 'v1', 's2': 'v2'}]}
 
     >>> path_put({"things": [{"s1": "v1", "sub": {"ss1": "sv1"}}]}, "things.0.sub", {"ss2": "sv2"})
     {'things': [{'s1': 'v1', 'sub': {'ss1': 'sv1', 'ss2': 'sv2'}}]}
 
+    >>> path_put({"thing": {"thing_id": "foo", "subs": [{"sub_id": 1, "sprop1": 11}]}},\
+            "thing.subs", [{"sub_id": 1, "sprop2": 22}])
+    {'thing': {'thing_id': 'foo', 'subs': [{'sub_id': 1, 'sprop1': 11, 'sprop2': 22}]}}
+
     """
     if data is None:
         return value
 
     if not path:
         path = []
 
@@ -93,15 +97,19 @@
     if not path:
         if isinstance(value, dict):
             data.update(value)
         return
 
     path0 = path.pop(0)
     if not path:
-        if path0 in data and isinstance(value, dict):
+        if path0 in data and isinstance(data[path0], list) and isinstance(value, list):
+            for a, b in zip(data[path0], value):
+                a.update(b)
+
+        elif path0 in data and isinstance(value, dict):
             data[path0].update(value)
         else:
             data[path0] = value
         return
 
     if path0 not in data:
         if path and (isinstance(path[0], int) or path[0].isnumeric()):
```

## Comparing `pydantic_enhanced_serializer-1.1.3.dist-info/LICENSE` & `pydantic_enhanced_serializer-1.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pydantic_enhanced_serializer-1.1.3.dist-info/METADATA` & `pydantic_enhanced_serializer-1.1.4.dist-info/METADATA`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-enhanced-serializer
-Version: 1.1.3
+Version: 1.1.4
 Summary: Pydantic extension that allows user selection of object fields or expansions inline when serializing models
 Home-page: https://github.com/adamsussman/pydantic-enhanced-serializer
 Author: Adam Sussman
 Author-email: adam.sussman@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pydantic
```

## Comparing `pydantic_enhanced_serializer-1.1.3.dist-info/RECORD` & `pydantic_enhanced_serializer-1.1.4.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 pydantic_enhanced_serializer/__init__.py,sha256=YDA4Ntaq4mBBR0nDyHFXlvqE_OWJ6mzsCHlxjX71nYc,309
 pydantic_enhanced_serializer/fieldsets.py,sha256=YU94v7aW5dDNkGmhZXkWYlCKb2up1iXKsYaoPPKApNc,9424
 pydantic_enhanced_serializer/models.py,sha256=ZGoQZ9cHTT9icObGvfWFkeBYRSQUKYYbligdsiDvX94,2724
-pydantic_enhanced_serializer/path_put.py,sha256=CPqpjErHgzvipU6B326A-XpSbhTtWJzGeV9UODzMUjY,3960
+pydantic_enhanced_serializer/path_put.py,sha256=ok7CfP6NxdySSW36CBINhnGtNKas2R-edUh2g4kGJ3A,4363
 pydantic_enhanced_serializer/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pydantic_enhanced_serializer/render.py,sha256=OsnGmTjDr93Xi1vYWcM5YgNDpsZbpsAa5Ct724-BxBw,4222
 pydantic_enhanced_serializer/schema.py,sha256=1fCBy35ULkefakzqFOdyIykJUFlCQ7dK5V2y80o41fQ,6632
 pydantic_enhanced_serializer/integrations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pydantic_enhanced_serializer/integrations/django_ninja.py,sha256=Z60LR0vfM4wbpvWo_qfEhcsUn4ufXU80xwD4zbPGIdI,1401
 pydantic_enhanced_serializer/integrations/fastapi.py,sha256=6qBNdbafvEAmVDBVS0h_AedDnevh_Ilv3bztF3pcYHY,6078
-pydantic_enhanced_serializer-1.1.3.dist-info/LICENSE,sha256=INaSDKc7Y-fYndT1E_X93xe_8Ez3nkemMNtk3TaFH9c,1073
-pydantic_enhanced_serializer-1.1.3.dist-info/METADATA,sha256=g8AtCVzd-cHrt4tGJa-exG_T04rfejYcUySRkOLqK98,6021
-pydantic_enhanced_serializer-1.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pydantic_enhanced_serializer-1.1.3.dist-info/top_level.txt,sha256=QCypSWZi8vRHdmuu-4xOAqUWN78nQShuGw0yMB4RLI4,29
-pydantic_enhanced_serializer-1.1.3.dist-info/RECORD,,
+pydantic_enhanced_serializer-1.1.4.dist-info/LICENSE,sha256=INaSDKc7Y-fYndT1E_X93xe_8Ez3nkemMNtk3TaFH9c,1073
+pydantic_enhanced_serializer-1.1.4.dist-info/METADATA,sha256=lHfSsBKvJ8-aV0KeJUC27WpESBxPEb29Ip3XUxb8M90,6021
+pydantic_enhanced_serializer-1.1.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pydantic_enhanced_serializer-1.1.4.dist-info/top_level.txt,sha256=QCypSWZi8vRHdmuu-4xOAqUWN78nQShuGw0yMB4RLI4,29
+pydantic_enhanced_serializer-1.1.4.dist-info/RECORD,,
```

