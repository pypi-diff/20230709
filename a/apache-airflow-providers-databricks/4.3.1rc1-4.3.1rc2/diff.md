# Comparing `tmp/apache-airflow-providers-databricks-4.3.1rc1.tar.gz` & `tmp/apache-airflow-providers-databricks-4.3.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-databricks-4.3.1rc1.tar", last modified: Wed Jul  5 07:29:54 2023, max compression
+gzip compressed data, was "apache-airflow-providers-databricks-4.3.1rc2.tar", last modified: Thu Jul  6 04:50:35 2023, max compression
```

## Comparing `apache-airflow-providers-databricks-4.3.1rc1.tar` & `apache-airflow-providers-databricks-4.3.1rc2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:54.885886 apache-airflow-providers-databricks-4.3.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-databricks-4.3.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-05 07:29:53.000000 apache-airflow-providers-databricks-4.3.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-databricks-4.3.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5810 2023-07-05 07:29:54.886486 apache-airflow-providers-databricks-4.3.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4129 2023-07-05 07:29:53.000000 apache-airflow-providers-databricks-4.3.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:54.768560 apache-airflow-providers-databricks-4.3.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:54.769712 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:54.810050 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/
--rw-r--r--   0 root         (0) root         (0)     1535 2023-07-05 07:19:39.000000 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5527 2023-07-05 07:29:53.000000 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:54.822625 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16773 2023-06-29 05:49:30.000000 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/hooks/databricks.py
--rw-r--r--   0 root         (0) root         (0)    26696 2023-06-29 05:49:30.000000 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/hooks/databricks_base.py
--rw-r--r--   0 root         (0) root         (0)     9359 2023-06-17 16:45:00.000000 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/hooks/databricks_sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:54.835759 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33530 2023-07-05 07:19:39.000000 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/operators/databricks.py
--rw-r--r--   0 root         (0) root         (0)    13181 2023-06-29 05:49:30.000000 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/operators/databricks_repos.py
--rw-r--r--   0 root         (0) root         (0)    17010 2023-06-29 14:43:21.000000 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/operators/databricks_sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:54.844918 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9827 2023-06-29 05:49:30.000000 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/sensors/databricks_partition.py
--rw-r--r--   0 root         (0) root         (0)     5543 2023-06-01 07:44:14.000000 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/sensors/databricks_sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:54.851439 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/triggers/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3997 2023-06-18 13:29:11.000000 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/triggers/databricks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:54.857448 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/utils/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2945 2023-06-29 05:49:30.000000 apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/utils/databricks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:54.883118 apache-airflow-providers-databricks-4.3.1rc1/apache_airflow_providers_databricks.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5810 2023-07-05 07:29:54.000000 apache-airflow-providers-databricks-4.3.1rc1/apache_airflow_providers_databricks.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1362 2023-07-05 07:29:54.000000 apache-airflow-providers-databricks-4.3.1rc1/apache_airflow_providers_databricks.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:29:54.000000 apache-airflow-providers-databricks-4.3.1rc1/apache_airflow_providers_databricks.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-07-05 07:29:54.000000 apache-airflow-providers-databricks-4.3.1rc1/apache_airflow_providers_databricks.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:29:54.000000 apache-airflow-providers-databricks-4.3.1rc1/apache_airflow_providers_databricks.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      200 2023-07-05 07:29:54.000000 apache-airflow-providers-databricks-4.3.1rc1/apache_airflow_providers_databricks.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-05 07:29:54.000000 apache-airflow-providers-databricks-4.3.1rc1/apache_airflow_providers_databricks.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-databricks-4.3.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2082 2023-07-05 07:29:54.888468 apache-airflow-providers-databricks-4.3.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1715 2023-07-05 07:29:53.000000 apache-airflow-providers-databricks-4.3.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:35.029129 apache-airflow-providers-databricks-4.3.1rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-databricks-4.3.1rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-06 04:50:33.000000 apache-airflow-providers-databricks-4.3.1rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-databricks-4.3.1rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5810 2023-07-06 04:50:35.029888 apache-airflow-providers-databricks-4.3.1rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4129 2023-07-06 04:50:33.000000 apache-airflow-providers-databricks-4.3.1rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:34.896378 apache-airflow-providers-databricks-4.3.1rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:34.897567 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:34.943174 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-07-05 18:49:44.000000 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5527 2023-07-06 04:50:33.000000 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:34.957520 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16773 2023-06-29 05:49:30.000000 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/hooks/databricks.py
+-rw-r--r--   0 root         (0) root         (0)    26696 2023-06-29 05:49:30.000000 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/hooks/databricks_base.py
+-rw-r--r--   0 root         (0) root         (0)     9359 2023-06-17 16:45:00.000000 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/hooks/databricks_sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:34.971570 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33530 2023-07-05 07:19:39.000000 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/operators/databricks.py
+-rw-r--r--   0 root         (0) root         (0)    13181 2023-06-29 05:49:30.000000 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/operators/databricks_repos.py
+-rw-r--r--   0 root         (0) root         (0)    17010 2023-06-29 14:43:21.000000 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/operators/databricks_sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:34.983172 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9827 2023-06-29 05:49:30.000000 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/sensors/databricks_partition.py
+-rw-r--r--   0 root         (0) root         (0)     5543 2023-06-01 07:44:14.000000 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/sensors/databricks_sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:34.990705 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/triggers/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3997 2023-06-18 13:29:11.000000 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/triggers/databricks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:34.999085 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/utils/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2945 2023-06-29 05:49:30.000000 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/utils/databricks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:35.026528 apache-airflow-providers-databricks-4.3.1rc2/apache_airflow_providers_databricks.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5810 2023-07-06 04:50:34.000000 apache-airflow-providers-databricks-4.3.1rc2/apache_airflow_providers_databricks.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1362 2023-07-06 04:50:34.000000 apache-airflow-providers-databricks-4.3.1rc2/apache_airflow_providers_databricks.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:34.000000 apache-airflow-providers-databricks-4.3.1rc2/apache_airflow_providers_databricks.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-07-06 04:50:34.000000 apache-airflow-providers-databricks-4.3.1rc2/apache_airflow_providers_databricks.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:34.000000 apache-airflow-providers-databricks-4.3.1rc2/apache_airflow_providers_databricks.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      200 2023-07-06 04:50:34.000000 apache-airflow-providers-databricks-4.3.1rc2/apache_airflow_providers_databricks.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-06 04:50:34.000000 apache-airflow-providers-databricks-4.3.1rc2/apache_airflow_providers_databricks.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-databricks-4.3.1rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2082 2023-07-06 04:50:35.032113 apache-airflow-providers-databricks-4.3.1rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1715 2023-07-06 04:50:33.000000 apache-airflow-providers-databricks-4.3.1rc2/setup.py
```

### Comparing `apache-airflow-providers-databricks-4.3.1rc1/LICENSE` & `apache-airflow-providers-databricks-4.3.1rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.1rc1/MANIFEST.in` & `apache-airflow-providers-databricks-4.3.1rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.1rc1/PKG-INFO` & `apache-airflow-providers-databricks-4.3.1rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-databricks
-Version: 4.3.1rc1
+Version: 4.3.1rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-databricks package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.3.1/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-databricks``
 
-Release: ``4.3.1rc1``
+Release: ``4.3.1rc2``
 
 
 `Databricks <https://databricks.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-databricks-4.3.1rc1/README.rst` & `apache-airflow-providers-databricks-4.3.1rc2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-databricks``
 
-Release: ``4.3.1rc1``
+Release: ``4.3.1rc2``
 
 
 `Databricks <https://databricks.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/__init__.py` & `apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/get_provider_info.py` & `apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/hooks/__init__.py` & `apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/hooks/databricks.py` & `apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/hooks/databricks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/hooks/databricks_base.py` & `apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/hooks/databricks_base.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/hooks/databricks_sql.py` & `apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/hooks/databricks_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/operators/__init__.py` & `apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/operators/databricks.py` & `apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/operators/databricks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/operators/databricks_repos.py` & `apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/operators/databricks_repos.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/operators/databricks_sql.py` & `apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/operators/databricks_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/sensors/__init__.py` & `apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/sensors/databricks_partition.py` & `apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/sensors/databricks_partition.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/sensors/databricks_sql.py` & `apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/sensors/databricks_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/triggers/__init__.py` & `apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/triggers/databricks.py` & `apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/triggers/databricks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/utils/__init__.py` & `apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.1rc1/airflow/providers/databricks/utils/databricks.py` & `apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/utils/databricks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.1rc1/apache_airflow_providers_databricks.egg-info/PKG-INFO` & `apache-airflow-providers-databricks-4.3.1rc2/apache_airflow_providers_databricks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-databricks
-Version: 4.3.1rc1
+Version: 4.3.1rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-databricks package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.3.1/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-databricks``
 
-Release: ``4.3.1rc1``
+Release: ``4.3.1rc2``
 
 
 `Databricks <https://databricks.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-databricks-4.3.1rc1/apache_airflow_providers_databricks.egg-info/SOURCES.txt` & `apache-airflow-providers-databricks-4.3.1rc2/apache_airflow_providers_databricks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.1rc1/pyproject.toml` & `apache-airflow-providers-databricks-4.3.1rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.1rc1/setup.cfg` & `apache-airflow-providers-databricks-4.3.1rc2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -57,10 +57,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.databricks.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.databricks
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-databricks-4.3.1rc1/setup.py` & `apache-airflow-providers-databricks-4.3.1rc2/setup.py`

 * *Files identical despite different names*

