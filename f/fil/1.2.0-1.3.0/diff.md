# Comparing `tmp/fil-1.2.0.tar.gz` & `tmp/fil-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fil-1.2.0.tar", max compression
+gzip compressed data, was "fil-1.3.0.tar", max compression
```

## Comparing `fil-1.2.0.tar` & `fil-1.3.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      782 2023-05-02 15:39:14.592872 fil-1.2.0/README.md
--rw-r--r--   0        0        0     5633 2023-05-28 10:47:19.543564 fil-1.2.0/fil.py
--rw-r--r--   0        0        0      496 2023-05-28 10:48:29.683341 fil-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1351 1970-01-01 00:00:00.000000 fil-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      782 2023-05-02 15:39:14.592872 fil-1.3.0/README.md
+-rw-r--r--   0        0        0     5633 2023-05-28 10:47:19.543564 fil-1.3.0/fil.py
+-rw-r--r--   0        0        0      492 2023-07-09 14:56:16.279353 fil-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1329 1970-01-01 00:00:00.000000 fil-1.3.0/PKG-INFO
```

### Comparing `fil-1.2.0/README.md` & `fil-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `fil-1.2.0/fil.py` & `fil-1.3.0/fil.py`

 * *Files identical despite different names*

### Comparing `fil-1.2.0/PKG-INFO` & `fil-1.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: fil
-Version: 1.2.0
+Version: 1.3.0
 Summary: 🏺 Read/write JSON/TOML/Yaml/txt 🏺
 License: MIT
 Author: Tom Ritchford
 Author-email: tom@swirly.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: safer (>=4.6.1,<5.0.0)
+Requires-Dist: safer
 Description-Content-Type: text/markdown
 
 ## Example 1: read a file
 
     d1 = fil.read('file.json')   # Any Json
     d2 = fil.read('file.toml')   # A dict
     d3 = fil.read('file.yaml')   # Any JSON
```

