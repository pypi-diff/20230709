# Comparing `tmp/re_action_template-2.0.1-py3-none-any.whl.zip` & `tmp/re_action_template-2.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 14504 bytes, number of entries: 8
+Zip file size: 14505 bytes, number of entries: 8
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 action_template/__init__.py
 -rwxr-xr-x  2.0 unx      156 b- defN 80-Jan-01 00:00 action_template/__main__.py
 -rw-r--r--  2.0 unx     2259 b- defN 80-Jan-01 00:00 action_template/main.py
--rw-r--r--  2.0 unx    30583 b- defN 80-Jan-01 00:00 re_action_template-2.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     4230 b- defN 80-Jan-01 00:00 re_action_template-2.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 re_action_template-2.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       65 b- defN 80-Jan-01 00:00 re_action_template-2.0.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      689 b- defN 16-Jan-01 00:00 re_action_template-2.0.1.dist-info/RECORD
-8 files, 38070 bytes uncompressed, 13286 bytes compressed:  65.1%
+-rw-r--r--  2.0 unx    30583 b- defN 80-Jan-01 00:00 re_action_template-2.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4230 b- defN 80-Jan-01 00:00 re_action_template-2.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 re_action_template-2.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       65 b- defN 80-Jan-01 00:00 re_action_template-2.0.2.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      689 b- defN 16-Jan-01 00:00 re_action_template-2.0.2.dist-info/RECORD
+8 files, 38070 bytes uncompressed, 13287 bytes compressed:  65.1%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: action_template/__main__.py
 Comment: 
 
 Filename: action_template/main.py
 Comment: 
 
-Filename: re_action_template-2.0.1.dist-info/LICENSE
+Filename: re_action_template-2.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: re_action_template-2.0.1.dist-info/METADATA
+Filename: re_action_template-2.0.2.dist-info/METADATA
 Comment: 
 
-Filename: re_action_template-2.0.1.dist-info/WHEEL
+Filename: re_action_template-2.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: re_action_template-2.0.1.dist-info/entry_points.txt
+Filename: re_action_template-2.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: re_action_template-2.0.1.dist-info/RECORD
+Filename: re_action_template-2.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `re_action_template-2.0.1.dist-info/LICENSE` & `re_action_template-2.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `re_action_template-2.0.1.dist-info/METADATA` & `re_action_template-2.0.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re-action-template
-Version: 2.0.1
+Version: 2.0.2
 Summary: 
 License: SSPL-1.0
 Author: Philipp Gayret
 Author-email: philipp@release-engineers.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: re-action-template Version: 2.0.1 Summary: License:
+Metadata-Version: 2.1 Name: re-action-template Version: 2.0.2 Summary: License:
 SSPL-1.0 Author: Philipp Gayret Author-email: philipp@release-engineers.com
 Requires-Python: >=3.11,<4.0 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: Markdown (>=3.3.6,<4.0.0) Requires-
 Dist: fire (>=0.5.0,<0.6.0) Requires-Dist: jinja2 (>=3.0.3,<4.0.0) Requires-
 Dist: pyyaml (>=6.0,<7.0) Description-Content-Type: text/markdown  # release-
 engineers/action-template [![Status: Production ready](https://img.shields.io/
```

## Comparing `re_action_template-2.0.1.dist-info/RECORD` & `re_action_template-2.0.2.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 action_template/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 action_template/__main__.py,sha256=L--CQs0rPatHtlKm0clm-1TxXD5DXPSAoFsTyrnk28A,156
 action_template/main.py,sha256=t9FPEE3g_69sgo-s5tjKUcYxBj7Ez-Z2IrypGy95Egg,2259
-re_action_template-2.0.1.dist-info/LICENSE,sha256=Jp0_6oDvg99Q72hGqp1nWkxHMRdlBra9z78CDwD4yLs,30583
-re_action_template-2.0.1.dist-info/METADATA,sha256=seYgLF1Thmli8HJt97kDoxJRiuazSlZOMFvFIs9Ep-g,4230
-re_action_template-2.0.1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-re_action_template-2.0.1.dist-info/entry_points.txt,sha256=DbdYeQoeg8Pnk2GzJr9LUgK9nDHUnNIpyxZVPMByx3c,65
-re_action_template-2.0.1.dist-info/RECORD,,
+re_action_template-2.0.2.dist-info/LICENSE,sha256=Jp0_6oDvg99Q72hGqp1nWkxHMRdlBra9z78CDwD4yLs,30583
+re_action_template-2.0.2.dist-info/METADATA,sha256=jObYs9xVXZuju3sIimW_dIe8lSlVcORWYDODgWjXXr4,4230
+re_action_template-2.0.2.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+re_action_template-2.0.2.dist-info/entry_points.txt,sha256=DbdYeQoeg8Pnk2GzJr9LUgK9nDHUnNIpyxZVPMByx3c,65
+re_action_template-2.0.2.dist-info/RECORD,,
```

