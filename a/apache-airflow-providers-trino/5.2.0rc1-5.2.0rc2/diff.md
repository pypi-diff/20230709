# Comparing `tmp/apache-airflow-providers-trino-5.2.0rc1.tar.gz` & `tmp/apache-airflow-providers-trino-5.2.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-trino-5.2.0rc1.tar", last modified: Wed Jul  5 07:30:34 2023, max compression
+gzip compressed data, was "apache-airflow-providers-trino-5.2.0rc2.tar", last modified: Thu Jul  6 04:51:40 2023, max compression
```

## Comparing `apache-airflow-providers-trino-5.2.0rc1.tar` & `apache-airflow-providers-trino-5.2.0rc2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:34.041403 apache-airflow-providers-trino-5.2.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.2.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-05 07:30:32.000000 apache-airflow-providers-trino-5.2.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.2.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5821 2023-07-05 07:30:34.042484 apache-airflow-providers-trino-5.2.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4137 2023-07-05 07:30:32.000000 apache-airflow-providers-trino-5.2.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:33.932620 apache-airflow-providers-trino-5.2.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:33.933834 apache-airflow-providers-trino-5.2.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:33.970786 apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/
--rw-r--r--   0 root         (0) root         (0)     1530 2023-07-05 07:19:39.000000 apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3068 2023-07-05 07:30:32.000000 apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:33.978141 apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9579 2023-06-25 14:35:06.000000 apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/hooks/trino.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:33.986231 apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3169 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/operators/trino.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:33.997483 apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/transfers/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4999 2023-06-02 11:31:21.000000 apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/transfers/gcs_to_trino.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:34.037432 apache-airflow-providers-trino-5.2.0rc1/apache_airflow_providers_trino.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5821 2023-07-05 07:30:33.000000 apache-airflow-providers-trino-5.2.0rc1/apache_airflow_providers_trino.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      797 2023-07-05 07:30:33.000000 apache-airflow-providers-trino-5.2.0rc1/apache_airflow_providers_trino.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:30:33.000000 apache-airflow-providers-trino-5.2.0rc1/apache_airflow_providers_trino.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      102 2023-07-05 07:30:33.000000 apache-airflow-providers-trino-5.2.0rc1/apache_airflow_providers_trino.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:30:33.000000 apache-airflow-providers-trino-5.2.0rc1/apache_airflow_providers_trino.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      197 2023-07-05 07:30:33.000000 apache-airflow-providers-trino-5.2.0rc1/apache_airflow_providers_trino.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-05 07:30:33.000000 apache-airflow-providers-trino-5.2.0rc1/apache_airflow_providers_trino.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-trino-5.2.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1999 2023-07-05 07:30:34.045371 apache-airflow-providers-trino-5.2.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1767 2023-07-05 07:30:32.000000 apache-airflow-providers-trino-5.2.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:40.318871 apache-airflow-providers-trino-5.2.0rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.2.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-06 04:51:39.000000 apache-airflow-providers-trino-5.2.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.2.0rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5821 2023-07-06 04:51:40.319536 apache-airflow-providers-trino-5.2.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4137 2023-07-06 04:51:39.000000 apache-airflow-providers-trino-5.2.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:40.233436 apache-airflow-providers-trino-5.2.0rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:40.237418 apache-airflow-providers-trino-5.2.0rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:40.273142 apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/
+-rw-r--r--   0 root         (0) root         (0)     1530 2023-07-05 18:55:40.000000 apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3068 2023-07-06 04:51:39.000000 apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:40.278826 apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9579 2023-06-25 14:35:06.000000 apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/hooks/trino.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:40.284621 apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3169 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/operators/trino.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:40.290307 apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/transfers/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4999 2023-06-02 11:31:21.000000 apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/transfers/gcs_to_trino.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:40.315854 apache-airflow-providers-trino-5.2.0rc2/apache_airflow_providers_trino.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5821 2023-07-06 04:51:40.000000 apache-airflow-providers-trino-5.2.0rc2/apache_airflow_providers_trino.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      797 2023-07-06 04:51:40.000000 apache-airflow-providers-trino-5.2.0rc2/apache_airflow_providers_trino.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:51:40.000000 apache-airflow-providers-trino-5.2.0rc2/apache_airflow_providers_trino.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      102 2023-07-06 04:51:40.000000 apache-airflow-providers-trino-5.2.0rc2/apache_airflow_providers_trino.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:51:40.000000 apache-airflow-providers-trino-5.2.0rc2/apache_airflow_providers_trino.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      197 2023-07-06 04:51:40.000000 apache-airflow-providers-trino-5.2.0rc2/apache_airflow_providers_trino.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-06 04:51:40.000000 apache-airflow-providers-trino-5.2.0rc2/apache_airflow_providers_trino.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-trino-5.2.0rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1999 2023-07-06 04:51:40.321552 apache-airflow-providers-trino-5.2.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1767 2023-07-06 04:51:39.000000 apache-airflow-providers-trino-5.2.0rc2/setup.py
```

### Comparing `apache-airflow-providers-trino-5.2.0rc1/LICENSE` & `apache-airflow-providers-trino-5.2.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.2.0rc1/MANIFEST.in` & `apache-airflow-providers-trino-5.2.0rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.2.0rc1/PKG-INFO` & `apache-airflow-providers-trino-5.2.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-trino
-Version: 5.2.0rc1
+Version: 5.2.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-trino package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-trino/5.2.0/
@@ -68,15 +68,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-trino``
 
-Release: ``5.2.0rc1``
+Release: ``5.2.0rc2``
 
 
 `Trino <https://trino.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-trino-5.2.0rc1/README.rst` & `apache-airflow-providers-trino-5.2.0rc2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-trino``
 
-Release: ``5.2.0rc1``
+Release: ``5.2.0rc2``
 
 
 `Trino <https://trino.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/__init__.py` & `apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/get_provider_info.py` & `apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/hooks/__init__.py` & `apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/hooks/trino.py` & `apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/hooks/trino.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/operators/__init__.py` & `apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/operators/trino.py` & `apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/operators/trino.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/transfers/__init__.py` & `apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.2.0rc1/airflow/providers/trino/transfers/gcs_to_trino.py` & `apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/transfers/gcs_to_trino.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.2.0rc1/apache_airflow_providers_trino.egg-info/PKG-INFO` & `apache-airflow-providers-trino-5.2.0rc2/apache_airflow_providers_trino.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-trino
-Version: 5.2.0rc1
+Version: 5.2.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-trino package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-trino/5.2.0/
@@ -68,15 +68,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-trino``
 
-Release: ``5.2.0rc1``
+Release: ``5.2.0rc2``
 
 
 `Trino <https://trino.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-trino-5.2.0rc1/apache_airflow_providers_trino.egg-info/SOURCES.txt` & `apache-airflow-providers-trino-5.2.0rc2/apache_airflow_providers_trino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.2.0rc1/pyproject.toml` & `apache-airflow-providers-trino-5.2.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.2.0rc1/setup.cfg` & `apache-airflow-providers-trino-5.2.0rc2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -56,10 +56,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.trino.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.trino
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-trino-5.2.0rc1/setup.py` & `apache-airflow-providers-trino-5.2.0rc2/setup.py`

 * *Files identical despite different names*

