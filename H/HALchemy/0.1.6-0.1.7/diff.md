# Comparing `tmp/HALchemy-0.1.6-py3-none-any.whl.zip` & `tmp/HALchemy-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5482 bytes, number of entries: 7
+Zip file size: 5500 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat       73 b- defN 23-Jul-04 01:21 halchemy/__init__.py
 -rw-rw-rw-  2.0 fat     6308 b- defN 23-Jul-06 16:47 halchemy/api.py
 -rw-rw-rw-  2.0 fat     2548 b- defN 23-Jul-01 18:46 halchemy/requests_helper.py
--rw-rw-rw-  2.0 fat     1872 b- defN 23-Jul-07 22:03 HALchemy-0.1.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-07 22:03 HALchemy-0.1.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-07 22:03 HALchemy-0.1.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      532 b- defN 23-Jul-07 22:03 HALchemy-0.1.6.dist-info/RECORD
-7 files, 11434 bytes uncompressed, 4540 bytes compressed:  60.3%
+-rw-rw-rw-  2.0 fat     1976 b- defN 23-Jul-09 03:41 HALchemy-0.1.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-09 03:41 HALchemy-0.1.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-09 03:41 HALchemy-0.1.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      532 b- defN 23-Jul-09 03:41 HALchemy-0.1.7.dist-info/RECORD
+7 files, 11538 bytes uncompressed, 4558 bytes compressed:  60.5%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: halchemy/api.py
 Comment: 
 
 Filename: halchemy/requests_helper.py
 Comment: 
 
-Filename: HALchemy-0.1.6.dist-info/METADATA
+Filename: HALchemy-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: HALchemy-0.1.6.dist-info/WHEEL
+Filename: HALchemy-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: HALchemy-0.1.6.dist-info/top_level.txt
+Filename: HALchemy-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: HALchemy-0.1.6.dist-info/RECORD
+Filename: HALchemy-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `HALchemy-0.1.6.dist-info/METADATA` & `HALchemy-0.1.7.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HALchemy
-Version: 0.1.6
+Version: 0.1.7
 Summary: Toolkit for creating clients of HAL based Hypermedia APIs.
 Home-page: https://github.com/pointw-dev/HALchemy
 Author: Michael Ottoson
 Author-email: michael@pointw.com
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
@@ -15,17 +15,17 @@
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 
 # HALchemy for Python
 **HAL-based Hypermedia API clients for humans.**
 
-![](../../img/halchemy-full-word.png)
+![](https://github.com/pointw-dev/HALchemy/blob/main/img/halchemy-full-word.png?raw=True)
 
-![](../../img/python.png)
+![](https://github.com/pointw-dev/HALchemy/blob/main/img/python.png?raw=True)
 
 
 > This project has lofty goals, and is in its very early stages.  Please use with caution and beware of breaking changes until at least v0.7.0
 
 
 
 ## Getting started
```

## Comparing `HALchemy-0.1.6.dist-info/RECORD` & `HALchemy-0.1.7.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 halchemy/__init__.py,sha256=uOY88fxo04Ofw2_FpvGJ6LziQpDTE2o6aWfNP5May5M,73
 halchemy/api.py,sha256=tYG6iNs2smqPmt-TKzlBbihMUXmWiMcl1OZ_yQ1ReBw,6308
 halchemy/requests_helper.py,sha256=7mV5ts4jN3viuvpTWoYogkap8v1HpYe0wIWxf9N0KMI,2548
-HALchemy-0.1.6.dist-info/METADATA,sha256=uYJ_A4j_4uX5xgLvdOiaAUk0cTpIAG1HtX0wilHkiWY,1872
-HALchemy-0.1.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-HALchemy-0.1.6.dist-info/top_level.txt,sha256=QDAX4T2q2TC09LWO_LgEyuEBr-lPTU86p48miwnpfzw,9
-HALchemy-0.1.6.dist-info/RECORD,,
+HALchemy-0.1.7.dist-info/METADATA,sha256=GBsf6qbbi_j5Nxb-Q8ItCCj7Yw5vaHkB9IvCz1M2euI,1976
+HALchemy-0.1.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+HALchemy-0.1.7.dist-info/top_level.txt,sha256=QDAX4T2q2TC09LWO_LgEyuEBr-lPTU86p48miwnpfzw,9
+HALchemy-0.1.7.dist-info/RECORD,,
```

