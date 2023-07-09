# Comparing `tmp/fm91-0.0.16.tar.gz` & `tmp/fm91-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fm91-0.0.16.tar", max compression
+gzip compressed data, was "fm91-0.0.17.tar", max compression
```

## Comparing `fm91-0.0.16.tar` & `fm91-0.0.17.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-07-09 06:14:10.961033 fm91-0.0.16/fm91/__init__.py
--rw-r--r--   0        0        0    10847 2023-07-09 07:19:35.248188 fm91-0.0.16/fm91/main.py
--rw-r--r--   0        0        0      429 2023-07-09 07:38:34.447600 fm91-0.0.16/pyproject.toml
--rw-r--r--   0        0        0     5648 2023-07-09 07:21:21.821375 fm91-0.0.16/README.md
--rw-r--r--   0        0        0     5779 1970-01-01 00:00:00.000000 fm91-0.0.16/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-09 06:14:10.961033 fm91-0.0.17/fm91/__init__.py
+-rw-r--r--   0        0        0    10847 2023-07-09 07:19:35.248188 fm91-0.0.17/fm91/main.py
+-rw-r--r--   0        0        0      427 2023-07-09 07:41:33.677757 fm91-0.0.17/pyproject.toml
+-rw-r--r--   0        0        0     5648 2023-07-09 07:21:21.821375 fm91-0.0.17/README.md
+-rw-r--r--   0        0        0     5779 1970-01-01 00:00:00.000000 fm91-0.0.17/PKG-INFO
```

### Comparing `fm91-0.0.16/fm91/main.py` & `fm91-0.0.17/fm91/main.py`

 * *Files identical despite different names*

### Comparing `fm91-0.0.16/README.md` & `fm91-0.0.17/README.md`

 * *Files identical despite different names*

### Comparing `fm91-0.0.16/PKG-INFO` & `fm91-0.0.17/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fm91
-Version: 0.0.16
+Version: 0.0.17
 Summary: A simple fastapi manager
 Author: abirmunna
 Author-email: mtmunna82@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

