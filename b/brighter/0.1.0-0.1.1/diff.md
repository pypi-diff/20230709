# Comparing `tmp/brighter-0.1.0.tar.gz` & `tmp/brighter-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brighter-0.1.0.tar", max compression
+gzip compressed data, was "brighter-0.1.1.tar", max compression
```

## Comparing `brighter-0.1.0.tar` & `brighter-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1066 2023-07-09 15:40:26.608540 brighter-0.1.0/LICENSE
--rw-r--r--   0        0        0       10 2023-07-09 15:40:26.608640 brighter-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-09 15:52:28.332429 brighter-0.1.0/brighter/__init__.py
--rw-r--r--   0        0        0        0 2023-07-09 15:59:04.301524 brighter-0.1.0/brighter/airflow/__init__.py
--rw-r--r--   0        0        0        0 2023-07-09 15:55:04.929886 brighter-0.1.0/brighter/airflow/alerts/__init__.py
--rw-r--r--   0        0        0     2742 2023-07-09 15:58:29.472711 brighter-0.1.0/brighter/airflow/alerts/slack.py
--rw-r--r--   0        0        0        0 2023-07-09 16:05:24.135840 brighter-0.1.0/brighter/airflow/operators/__init__.py
--rw-r--r--   0        0        0     2409 2023-07-09 16:09:25.826398 brighter-0.1.0/brighter/airflow/operators/bigquery.py
--rw-r--r--   0        0        0        0 2023-07-09 16:00:07.722919 brighter-0.1.0/brighter/api/__init__.py
--rw-r--r--   0        0        0     3571 2023-07-09 16:13:31.840765 brighter-0.1.0/brighter/api/core.py
--rw-r--r--   0        0        0      618 2023-07-09 16:10:08.163283 brighter-0.1.0/brighter/collections.py
--rw-r--r--   0        0        0        0 2023-07-09 16:01:06.478943 brighter-0.1.0/brighter/gcp/__init__.py
--rw-r--r--   0        0        0     4517 2023-07-09 16:08:52.414637 brighter-0.1.0/brighter/gcp/bigquery.py
--rw-r--r--   0        0        0     1729 2023-07-09 16:04:25.274207 brighter-0.1.0/brighter/gcp/credentials.py
--rw-r--r--   0        0        0     2793 2023-07-09 16:09:14.711768 brighter-0.1.0/brighter/gcp/storage.py
--rw-r--r--   0        0        0      587 2023-07-09 16:24:55.471612 brighter-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      687 1970-01-01 00:00:00.000000 brighter-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-09 16:40:28.159564 brighter-0.1.1/LICENSE
+-rw-r--r--   0        0        0       10 2023-07-09 16:40:28.159564 brighter-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-09 16:40:28.159564 brighter-0.1.1/brighter/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 16:40:28.159564 brighter-0.1.1/brighter/airflow/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 16:40:28.159564 brighter-0.1.1/brighter/airflow/alerts/__init__.py
+-rw-r--r--   0        0        0     2742 2023-07-09 16:40:28.159564 brighter-0.1.1/brighter/airflow/alerts/slack.py
+-rw-r--r--   0        0        0        0 2023-07-09 16:40:28.159564 brighter-0.1.1/brighter/airflow/operators/__init__.py
+-rw-r--r--   0        0        0     2409 2023-07-09 16:40:28.159564 brighter-0.1.1/brighter/airflow/operators/bigquery.py
+-rw-r--r--   0        0        0        0 2023-07-09 16:40:28.159564 brighter-0.1.1/brighter/api/__init__.py
+-rw-r--r--   0        0        0     3571 2023-07-09 16:40:28.159564 brighter-0.1.1/brighter/api/core.py
+-rw-r--r--   0        0        0      618 2023-07-09 16:40:28.159564 brighter-0.1.1/brighter/collections.py
+-rw-r--r--   0        0        0        0 2023-07-09 16:40:28.159564 brighter-0.1.1/brighter/gcp/__init__.py
+-rw-r--r--   0        0        0     4517 2023-07-09 16:40:28.159564 brighter-0.1.1/brighter/gcp/bigquery.py
+-rw-r--r--   0        0        0     1729 2023-07-09 16:40:28.159564 brighter-0.1.1/brighter/gcp/credentials.py
+-rw-r--r--   0        0        0     2793 2023-07-09 16:40:28.159564 brighter-0.1.1/brighter/gcp/storage.py
+-rw-r--r--   0        0        0      587 2023-07-09 16:40:28.163564 brighter-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      687 1970-01-01 00:00:00.000000 brighter-0.1.1/PKG-INFO
```

### Comparing `brighter-0.1.0/LICENSE` & `brighter-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `brighter-0.1.0/brighter/airflow/alerts/slack.py` & `brighter-0.1.1/brighter/airflow/alerts/slack.py`

 * *Files identical despite different names*

### Comparing `brighter-0.1.0/brighter/airflow/operators/bigquery.py` & `brighter-0.1.1/brighter/airflow/operators/bigquery.py`

 * *Files identical despite different names*

### Comparing `brighter-0.1.0/brighter/api/core.py` & `brighter-0.1.1/brighter/api/core.py`

 * *Files identical despite different names*

### Comparing `brighter-0.1.0/brighter/collections.py` & `brighter-0.1.1/brighter/collections.py`

 * *Files identical despite different names*

### Comparing `brighter-0.1.0/brighter/gcp/bigquery.py` & `brighter-0.1.1/brighter/gcp/bigquery.py`

 * *Files identical despite different names*

### Comparing `brighter-0.1.0/brighter/gcp/credentials.py` & `brighter-0.1.1/brighter/gcp/credentials.py`

 * *Files identical despite different names*

### Comparing `brighter-0.1.0/brighter/gcp/storage.py` & `brighter-0.1.1/brighter/gcp/storage.py`

 * *Files identical despite different names*

### Comparing `brighter-0.1.0/pyproject.toml` & `brighter-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "brighter"
-version = "0.1.0"
+version = "0.1.1"
 description = "A simple library for data-wrangling with GCP support"
 authors = []
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11,<3.12"
```

### Comparing `brighter-0.1.0/PKG-INFO` & `brighter-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brighter
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple library for data-wrangling with GCP support
 License: MIT
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: apache-airflow (>=2.6.2,<3.0.0)
```

