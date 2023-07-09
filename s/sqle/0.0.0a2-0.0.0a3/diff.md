# Comparing `tmp/sqle-0.0.0a2.tar.gz` & `tmp/sqle-0.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqle-0.0.0a2.tar", max compression
+gzip compressed data, was "sqle-0.0.0a3.tar", max compression
```

## Comparing `sqle-0.0.0a2.tar` & `sqle-0.0.0a3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1063 2023-04-13 11:39:12.312030 sqle-0.0.0a2/LICENSE
--rw-r--r--   0        0        0      150 2023-04-15 12:19:38.626033 sqle-0.0.0a2/README.md
--rw-r--r--   0        0        0      454 2023-07-09 07:49:20.710527 sqle-0.0.0a2/pyproject.toml
--rw-r--r--   0        0        0      146 2023-07-09 07:49:52.998354 sqle-0.0.0a2/sqle/__init__.py
--rw-r--r--   0        0        0     5925 2023-07-09 08:34:29.591957 sqle-0.0.0a2/sqle/adapter.py
--rw-r--r--   0        0        0        0 2023-03-11 12:58:20.091961 sqle-0.0.0a2/sqle/contrib/__init__.py
--rw-r--r--   0        0        0      150 2023-03-08 11:10:17.217492 sqle-0.0.0a2/sqle/contrib/class_property.py
--rw-r--r--   0        0        0      157 2023-04-12 15:49:20.785386 sqle-0.0.0a2/sqle/contrib/text.py
--rw-r--r--   0        0        0      435 2023-04-08 13:03:01.529379 sqle-0.0.0a2/sqle/exceptions.py
--rw-r--r--   0        0        0     2331 2023-04-15 12:21:27.817079 sqle-0.0.0a2/sqle/query.py
--rw-r--r--   0        0        0       46 2023-02-15 15:56:29.472877 sqle-0.0.0a2/sqle/settings.py
--rw-r--r--   0        0        0     3162 2023-07-09 06:36:36.016572 sqle-0.0.0a2/sqle/sql.py
--rw-r--r--   0        0        0      222 2023-06-02 16:29:51.580146 sqle-0.0.0a2/sqle/sqle-sqlite.code-workspace
--rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 sqle-0.0.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-13 11:39:12.312030 sqle-0.0.0a3/LICENSE
+-rw-r--r--   0        0        0      150 2023-04-15 12:19:38.626033 sqle-0.0.0a3/README.md
+-rw-r--r--   0        0        0      483 2023-07-09 10:46:45.257964 sqle-0.0.0a3/pyproject.toml
+-rw-r--r--   0        0        0      146 2023-07-09 10:58:25.090884 sqle-0.0.0a3/sqle/__init__.py
+-rw-r--r--   0        0        0     5925 2023-07-09 08:34:29.591957 sqle-0.0.0a3/sqle/adapter.py
+-rw-r--r--   0        0        0        0 2023-03-11 12:58:20.091961 sqle-0.0.0a3/sqle/contrib/__init__.py
+-rw-r--r--   0        0        0      150 2023-03-08 11:10:17.217492 sqle-0.0.0a3/sqle/contrib/class_property.py
+-rw-r--r--   0        0        0      157 2023-04-12 15:49:20.785386 sqle-0.0.0a3/sqle/contrib/text.py
+-rw-r--r--   0        0        0      435 2023-04-08 13:03:01.529379 sqle-0.0.0a3/sqle/exceptions.py
+-rw-r--r--   0        0        0     2331 2023-04-15 12:21:27.817079 sqle-0.0.0a3/sqle/query.py
+-rw-r--r--   0        0        0       46 2023-02-15 15:56:29.472877 sqle-0.0.0a3/sqle/settings.py
+-rw-r--r--   0        0        0     3162 2023-07-09 06:36:36.016572 sqle-0.0.0a3/sqle/sql.py
+-rw-r--r--   0        0        0      222 2023-06-02 16:29:51.580146 sqle-0.0.0a3/sqle/sqle-sqlite.code-workspace
+-rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 sqle-0.0.0a3/PKG-INFO
```

### Comparing `sqle-0.0.0a2/LICENSE` & `sqle-0.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `sqle-0.0.0a2/sqle/adapter.py` & `sqle-0.0.0a3/sqle/adapter.py`

 * *Files identical despite different names*

### Comparing `sqle-0.0.0a2/sqle/query.py` & `sqle-0.0.0a3/sqle/query.py`

 * *Files identical despite different names*

### Comparing `sqle-0.0.0a2/sqle/sql.py` & `sqle-0.0.0a3/sqle/sql.py`

 * *Files identical despite different names*

### Comparing `sqle-0.0.0a2/PKG-INFO` & `sqle-0.0.0a3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: sqle
-Version: 0.0.0a2
+Version: 0.0.0a3
 Summary: 
 License: MIT
 Author: acrius
 Author-email: acrius@mail.ru
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: typing-extensions (>=4.7.1,<5.0.0)
 Description-Content-Type: text/markdown
 
 # SQLE
 
 Python package designed to execute pure sql queries.
 
 | :exclamation:  This is alpha version    |
```

