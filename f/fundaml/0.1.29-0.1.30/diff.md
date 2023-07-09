# Comparing `tmp/fundaml-0.1.29.tar.gz` & `tmp/fundaml-0.1.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fundaml-0.1.29.tar", max compression
+gzip compressed data, was "fundaml-0.1.30.tar", max compression
```

## Comparing `fundaml-0.1.29.tar` & `fundaml-0.1.30.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0     1069 2023-07-08 18:26:50.700845 fundaml-0.1.29/LICENSE
--rw-r--r--   0        0        0     2328 2023-07-08 18:26:50.700845 fundaml-0.1.29/README.md
--rw-r--r--   0        0        0     1614 2023-07-08 18:41:04.042169 fundaml-0.1.29/pyproject.toml
--rw-r--r--   0        0        0      109 2023-07-08 18:26:51.112846 fundaml-0.1.29/src/fundaml/__init__.py
--rw-r--r--   0        0        0     1058 2023-07-08 18:26:51.112846 fundaml-0.1.29/src/fundaml/eda.py
--rw-r--r--   0        0        0     1400 2023-07-08 18:26:51.112846 fundaml-0.1.29/src/fundaml/models.py
--rw-r--r--   0        0        0     1032 2023-07-08 18:26:51.112846 fundaml-0.1.29/src/fundaml/scores.py
--rw-r--r--   0        0        0    17645 2023-07-08 18:26:51.112846 fundaml-0.1.29/src/fundaml/trainers.py
--rw-r--r--   0        0        0     3199 1970-01-01 00:00:00.000000 fundaml-0.1.29/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2023-07-08 20:50:13.472075 fundaml-0.1.30/LICENSE
+-rw-r--r--   0        0        0     2328 2023-07-08 20:50:13.472075 fundaml-0.1.30/README.md
+-rw-r--r--   0        0        0     1614 2023-07-08 21:01:13.009164 fundaml-0.1.30/pyproject.toml
+-rw-r--r--   0        0        0      109 2023-07-08 20:50:13.868074 fundaml-0.1.30/src/fundaml/__init__.py
+-rw-r--r--   0        0        0     1058 2023-07-08 20:50:13.868074 fundaml-0.1.30/src/fundaml/eda.py
+-rw-r--r--   0        0        0     1400 2023-07-08 20:50:13.868074 fundaml-0.1.30/src/fundaml/models.py
+-rw-r--r--   0        0        0     1032 2023-07-08 20:50:13.868074 fundaml-0.1.30/src/fundaml/scores.py
+-rw-r--r--   0        0        0    17645 2023-07-08 20:50:13.868074 fundaml-0.1.30/src/fundaml/trainers.py
+-rw-r--r--   0        0        0     3199 1970-01-01 00:00:00.000000 fundaml-0.1.30/PKG-INFO
```

### Comparing `fundaml-0.1.29/LICENSE` & `fundaml-0.1.30/LICENSE`

 * *Files identical despite different names*

### Comparing `fundaml-0.1.29/README.md` & `fundaml-0.1.30/README.md`

 * *Files identical despite different names*

### Comparing `fundaml-0.1.29/pyproject.toml` & `fundaml-0.1.30/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fundaml"
-version = "0.1.29"
+version = "0.1.30"
 description = "A foundational machine learning library designed to streamline the end-to-end process of developing and deploying machine learning models. FundAML offers a broad array of tools and utilities for data preprocessing, model training, evaluation, and deployment, making it a fundamental solution for machine learning tasks."
 authors = ["Tony Zoght"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10"
```

### Comparing `fundaml-0.1.29/src/fundaml/eda.py` & `fundaml-0.1.30/src/fundaml/eda.py`

 * *Files identical despite different names*

### Comparing `fundaml-0.1.29/src/fundaml/models.py` & `fundaml-0.1.30/src/fundaml/models.py`

 * *Files identical despite different names*

### Comparing `fundaml-0.1.29/src/fundaml/scores.py` & `fundaml-0.1.30/src/fundaml/scores.py`

 * *Files identical despite different names*

### Comparing `fundaml-0.1.29/src/fundaml/trainers.py` & `fundaml-0.1.30/src/fundaml/trainers.py`

 * *Files identical despite different names*

### Comparing `fundaml-0.1.29/PKG-INFO` & `fundaml-0.1.30/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fundaml
-Version: 0.1.29
+Version: 0.1.30
 Summary: A foundational machine learning library designed to streamline the end-to-end process of developing and deploying machine learning models. FundAML offers a broad array of tools and utilities for data preprocessing, model training, evaluation, and deployment, making it a fundamental solution for machine learning tasks.
 License: MIT
 Author: Tony Zoght
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

