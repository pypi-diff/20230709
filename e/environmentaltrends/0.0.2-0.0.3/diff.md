# Comparing `tmp/environmentaltrends-0.0.2.tar.gz` & `tmp/environmentaltrends-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "environmentaltrends-0.0.2.tar", max compression
+gzip compressed data, was "environmentaltrends-0.0.3.tar", max compression
```

## Comparing `environmentaltrends-0.0.2.tar` & `environmentaltrends-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       51 2023-07-09 04:57:58.671540 environmentaltrends-0.0.2/environmentaltrends/__init__.py
--rw-r--r--   0        0        0    20215 2023-07-09 04:57:58.672539 environmentaltrends-0.0.2/environmentaltrends/data_prep.py
--rw-r--r--   0        0        0    13621 2023-07-09 04:57:58.673538 environmentaltrends-0.0.2/environmentaltrends/single_trend_analysis.py
--rw-r--r--   0        0        0     6084 2023-07-09 04:57:58.674538 environmentaltrends-0.0.2/environmentaltrends/trends.py
--rw-r--r--   0        0        0    10751 2023-07-09 04:57:58.675538 environmentaltrends-0.0.2/environmentaltrends/validation.py
--rw-r--r--   0        0        0    11558 2023-07-09 04:57:58.669539 environmentaltrends-0.0.2/LICENSE
--rw-r--r--   0        0        0      576 2023-07-09 04:57:58.675538 environmentaltrends-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      119 2023-07-09 04:57:58.670539 environmentaltrends-0.0.2/README.md
--rw-r--r--   0        0        0      951 1970-01-01 00:00:00.000000 environmentaltrends-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       50 2023-07-09 05:48:12.464261 environmentaltrends-0.0.3/environmentaltrends/__init__.py
+-rw-r--r--   0        0        0    20215 2023-07-09 04:57:58.672539 environmentaltrends-0.0.3/environmentaltrends/data_prep.py
+-rw-r--r--   0        0        0    13621 2023-07-09 04:57:58.673538 environmentaltrends-0.0.3/environmentaltrends/single_trend_analysis.py
+-rw-r--r--   0        0        0     6084 2023-07-09 04:57:58.674538 environmentaltrends-0.0.3/environmentaltrends/trends.py
+-rw-r--r--   0        0        0    10751 2023-07-09 04:57:58.675538 environmentaltrends-0.0.3/environmentaltrends/validation.py
+-rw-r--r--   0        0        0    11558 2023-07-09 04:57:58.669539 environmentaltrends-0.0.3/LICENSE
+-rw-r--r--   0        0        0      576 2023-07-09 05:48:12.471262 environmentaltrends-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      119 2023-07-09 04:57:58.670539 environmentaltrends-0.0.3/README.md
+-rw-r--r--   0        0        0      951 1970-01-01 00:00:00.000000 environmentaltrends-0.0.3/PKG-INFO
```

### Comparing `environmentaltrends-0.0.2/environmentaltrends/data_prep.py` & `environmentaltrends-0.0.3/environmentaltrends/data_prep.py`

 * *Files identical despite different names*

### Comparing `environmentaltrends-0.0.2/environmentaltrends/single_trend_analysis.py` & `environmentaltrends-0.0.3/environmentaltrends/single_trend_analysis.py`

 * *Files identical despite different names*

### Comparing `environmentaltrends-0.0.2/environmentaltrends/trends.py` & `environmentaltrends-0.0.3/environmentaltrends/trends.py`

 * *Files identical despite different names*

### Comparing `environmentaltrends-0.0.2/environmentaltrends/validation.py` & `environmentaltrends-0.0.3/environmentaltrends/validation.py`

 * *Files identical despite different names*

### Comparing `environmentaltrends-0.0.2/LICENSE` & `environmentaltrends-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `environmentaltrends-0.0.2/pyproject.toml` & `environmentaltrends-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "environmentaltrends"
-version = "0.0.2"
+version = "0.0.3"
 description = "A python package for analysing environmental data for trends."
 authors = ["Kurt van Ness <vanness.kurt@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/kurtvanness/EnvironmentalTrends"
 license = "Apache-2.0"
 packages = [{include = "environmentaltrends"}]
```

### Comparing `environmentaltrends-0.0.2/PKG-INFO` & `environmentaltrends-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: environmentaltrends
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python package for analysing environmental data for trends.
 Home-page: https://github.com/kurtvanness/EnvironmentalTrends
 License: Apache-2.0
 Author: Kurt van Ness
 Author-email: vanness.kurt@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

