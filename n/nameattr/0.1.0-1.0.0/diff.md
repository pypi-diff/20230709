# Comparing `tmp/nameattr-0.1.0-py3-none-any.whl.zip` & `tmp/nameattr-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
 Zip file size: 5112 bytes, number of entries: 9
--rw-r--r--  2.0 unx     1024 b- defN 23-Jul-09 03:45 nameattr/__init__.py
--rw-r--r--  2.0 unx     2237 b- defN 23-Jul-09 03:45 nameattr/_match.py
--rw-r--r--  2.0 unx     1723 b- defN 23-Jul-09 03:45 nameattr/_text.py
--rw-r--r--  2.0 unx     1524 b- defN 23-Jul-09 03:45 nameattr/_type.py
--rw-r--r--  2.0 unx     1069 b- defN 23-Jul-09 03:46 nameattr-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      972 b- defN 23-Jul-09 03:46 nameattr-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 03:46 nameattr-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-09 03:46 nameattr-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      689 b- defN 23-Jul-09 03:46 nameattr-0.1.0.dist-info/RECORD
+-rw-r--r--  2.0 unx     1024 b- defN 23-Jul-09 03:48 nameattr/__init__.py
+-rw-r--r--  2.0 unx     2237 b- defN 23-Jul-09 03:48 nameattr/_match.py
+-rw-r--r--  2.0 unx     1723 b- defN 23-Jul-09 03:48 nameattr/_text.py
+-rw-r--r--  2.0 unx     1524 b- defN 23-Jul-09 03:48 nameattr/_type.py
+-rw-r--r--  2.0 unx     1069 b- defN 23-Jul-09 03:49 nameattr-1.0.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      972 b- defN 23-Jul-09 03:49 nameattr-1.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 03:49 nameattr-1.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-09 03:49 nameattr-1.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      689 b- defN 23-Jul-09 03:49 nameattr-1.0.0.dist-info/RECORD
 9 files, 9339 bytes uncompressed, 3934 bytes compressed:  57.9%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: nameattr/_text.py
 Comment: 
 
 Filename: nameattr/_type.py
 Comment: 
 
-Filename: nameattr-0.1.0.dist-info/LICENSE
+Filename: nameattr-1.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: nameattr-0.1.0.dist-info/METADATA
+Filename: nameattr-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: nameattr-0.1.0.dist-info/WHEEL
+Filename: nameattr-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: nameattr-0.1.0.dist-info/top_level.txt
+Filename: nameattr-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: nameattr-0.1.0.dist-info/RECORD
+Filename: nameattr-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nameattr/__init__.py

```diff
@@ -1,12 +1,12 @@
 import importlib
 import nltk
 
 
-__version__ = "0.1.0"
+__version__ = "1.0.0"
 
 
 _FIND_TYPES = ("text",)
 _type_funcs = []
 
 
 for find_type in _FIND_TYPES:
```

## Comparing `nameattr-0.1.0.dist-info/LICENSE` & `nameattr-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `nameattr-0.1.0.dist-info/METADATA` & `nameattr-1.0.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nameattr
-Version: 0.1.0
+Version: 1.0.0
 Summary: Identify possible attribution of input data
 Author-email: Matt Wisniewski <healthycrowd@mattw.life>
 License: MIT
 Project-URL: homepage, https://github.com/healthycrowd/nameattr
 Keywords: nameattr,utility,name,attribution,ner,name,entity,recognition
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

## Comparing `nameattr-0.1.0.dist-info/RECORD` & `nameattr-1.0.0.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-nameattr/__init__.py,sha256=5ssrzxi8ZVICWkd1mjLa5rpDUdKY0faJOZTIa-qtT3A,1024
+nameattr/__init__.py,sha256=mzJp04NYl1lpSeG6ZomcZBJcxNf9IwH5najTyCECHcE,1024
 nameattr/_match.py,sha256=fYeIv8jkxe4PmIyPNyYb4Dk8cSOj5Bc2Luwbw7-pG3A,2237
 nameattr/_text.py,sha256=AnQCzs9SkHubgSoArJVnUv_Zv215kcEu2EOn7PnRDlM,1723
 nameattr/_type.py,sha256=bX2ZLbUG6TChKENim2HDmoxTeKOPLD69UMj7arOmBE4,1524
-nameattr-0.1.0.dist-info/LICENSE,sha256=s1m2uS8ATMP1tmDdlqhtecX2AYDTccvP16kT1JtW7kM,1069
-nameattr-0.1.0.dist-info/METADATA,sha256=9CHJTOHviW_9hAjk4aqqQ8eBgQQAJ0lY3LoSlNahyuI,972
-nameattr-0.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-nameattr-0.1.0.dist-info/top_level.txt,sha256=067u3oOIL7ml5KytcARIF2Yuz38W1V7gAEV0DdWUEDI,9
-nameattr-0.1.0.dist-info/RECORD,,
+nameattr-1.0.0.dist-info/LICENSE,sha256=s1m2uS8ATMP1tmDdlqhtecX2AYDTccvP16kT1JtW7kM,1069
+nameattr-1.0.0.dist-info/METADATA,sha256=A8kIFUBlU-R4-h7Ljy-RbXQvLV-5qfaqrgly8VYm27k,972
+nameattr-1.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+nameattr-1.0.0.dist-info/top_level.txt,sha256=067u3oOIL7ml5KytcARIF2Yuz38W1V7gAEV0DdWUEDI,9
+nameattr-1.0.0.dist-info/RECORD,,
```

