# Comparing `tmp/apache-airflow-providers-dbt-cloud-3.2.2.tar.gz` & `tmp/apache-airflow-providers-dbt-cloud-3.2.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-dbt-cloud-3.2.2.tar", last modified: Thu Jul  6 04:44:35 2023, max compression
+gzip compressed data, was "apache-airflow-providers-dbt-cloud-3.2.2rc2.tar", last modified: Thu Jul  6 04:50:38 2023, max compression
```

## Comparing `apache-airflow-providers-dbt-cloud-3.2.2.tar` & `apache-airflow-providers-dbt-cloud-3.2.2rc2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:44:35.275002 apache-airflow-providers-dbt-cloud-3.2.2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-dbt-cloud-3.2.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-06 04:44:33.000000 apache-airflow-providers-dbt-cloud-3.2.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-dbt-cloud-3.2.2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5515 2023-07-06 04:44:35.275753 apache-airflow-providers-dbt-cloud-3.2.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3847 2023-07-06 04:44:33.000000 apache-airflow-providers-dbt-cloud-3.2.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:44:35.147308 apache-airflow-providers-dbt-cloud-3.2.2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:44:35.149263 apache-airflow-providers-dbt-cloud-3.2.2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:44:35.150669 apache-airflow-providers-dbt-cloud-3.2.2/airflow/providers/dbt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:44:35.203781 apache-airflow-providers-dbt-cloud-3.2.2/airflow/providers/dbt/cloud/
--rw-r--r--   0 root         (0) root         (0)     1534 2023-07-06 04:42:33.000000 apache-airflow-providers-dbt-cloud-3.2.2/airflow/providers/dbt/cloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2966 2023-07-06 04:44:33.000000 apache-airflow-providers-dbt-cloud-3.2.2/airflow/providers/dbt/cloud/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:44:35.212828 apache-airflow-providers-dbt-cloud-3.2.2/airflow/providers/dbt/cloud/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-dbt-cloud-3.2.2/airflow/providers/dbt/cloud/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24242 2023-06-29 05:49:30.000000 apache-airflow-providers-dbt-cloud-3.2.2/airflow/providers/dbt/cloud/hooks/dbt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:44:35.222439 apache-airflow-providers-dbt-cloud-3.2.2/airflow/providers/dbt/cloud/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-dbt-cloud-3.2.2/airflow/providers/dbt/cloud/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13665 2023-07-05 07:19:39.000000 apache-airflow-providers-dbt-cloud-3.2.2/airflow/providers/dbt/cloud/operators/dbt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:44:35.231018 apache-airflow-providers-dbt-cloud-3.2.2/airflow/providers/dbt/cloud/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-dbt-cloud-3.2.2/airflow/providers/dbt/cloud/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5714 2023-07-05 07:19:39.000000 apache-airflow-providers-dbt-cloud-3.2.2/airflow/providers/dbt/cloud/sensors/dbt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:44:35.238459 apache-airflow-providers-dbt-cloud-3.2.2/airflow/providers/dbt/cloud/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-dbt-cloud-3.2.2/airflow/providers/dbt/cloud/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4649 2023-06-05 12:50:36.000000 apache-airflow-providers-dbt-cloud-3.2.2/airflow/providers/dbt/cloud/triggers/dbt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:44:35.271819 apache-airflow-providers-dbt-cloud-3.2.2/apache_airflow_providers_dbt_cloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5515 2023-07-06 04:44:35.000000 apache-airflow-providers-dbt-cloud-3.2.2/apache_airflow_providers_dbt_cloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      933 2023-07-06 04:44:35.000000 apache-airflow-providers-dbt-cloud-3.2.2/apache_airflow_providers_dbt_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:44:35.000000 apache-airflow-providers-dbt-cloud-3.2.2/apache_airflow_providers_dbt_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-07-06 04:44:35.000000 apache-airflow-providers-dbt-cloud-3.2.2/apache_airflow_providers_dbt_cloud.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:44:35.000000 apache-airflow-providers-dbt-cloud-3.2.2/apache_airflow_providers_dbt_cloud.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      106 2023-07-06 04:44:35.000000 apache-airflow-providers-dbt-cloud-3.2.2/apache_airflow_providers_dbt_cloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-06 04:44:35.000000 apache-airflow-providers-dbt-cloud-3.2.2/apache_airflow_providers_dbt_cloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-dbt-cloud-3.2.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1987 2023-07-06 04:44:35.278644 apache-airflow-providers-dbt-cloud-3.2.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1697 2023-07-06 04:44:33.000000 apache-airflow-providers-dbt-cloud-3.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:38.100429 apache-airflow-providers-dbt-cloud-3.2.2rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-06 04:50:36.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5521 2023-07-06 04:50:38.101014 apache-airflow-providers-dbt-cloud-3.2.2rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3850 2023-07-06 04:50:36.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:38.004457 apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:38.005643 apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:38.006918 apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:38.047748 apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/
+-rw-r--r--   0 root         (0) root         (0)     1534 2023-07-06 04:42:33.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2966 2023-07-06 04:50:36.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:38.054061 apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24242 2023-06-29 05:49:30.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/hooks/dbt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:38.060405 apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13665 2023-07-05 07:19:39.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/operators/dbt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:38.066375 apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5714 2023-07-05 07:19:39.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/sensors/dbt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:38.072281 apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4649 2023-06-05 12:50:36.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/triggers/dbt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:38.097790 apache-airflow-providers-dbt-cloud-3.2.2rc2/apache_airflow_providers_dbt_cloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5521 2023-07-06 04:50:37.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/apache_airflow_providers_dbt_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      933 2023-07-06 04:50:37.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/apache_airflow_providers_dbt_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:37.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/apache_airflow_providers_dbt_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-07-06 04:50:37.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/apache_airflow_providers_dbt_cloud.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:37.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/apache_airflow_providers_dbt_cloud.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      111 2023-07-06 04:50:37.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/apache_airflow_providers_dbt_cloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-06 04:50:37.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/apache_airflow_providers_dbt_cloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1995 2023-07-06 04:50:38.102975 apache-airflow-providers-dbt-cloud-3.2.2rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1697 2023-07-06 04:50:36.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/setup.py
```

### Comparing `apache-airflow-providers-dbt-cloud-3.2.2/LICENSE` & `apache-airflow-providers-dbt-cloud-3.2.2rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.2/MANIFEST.in` & `apache-airflow-providers-dbt-cloud-3.2.2rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.2/PKG-INFO` & `apache-airflow-providers-dbt-cloud-3.2.2rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-dbt-cloud
-Version: 3.2.2
+Version: 3.2.2rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-dbt-cloud package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.2.2/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-dbt-cloud``
 
-Release: ``3.2.2``
+Release: ``3.2.2rc2``
 
 
 `dbt Cloud <https://www.getdbt.com/product/what-is-dbt/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-dbt-cloud-3.2.2/README.rst` & `apache-airflow-providers-dbt-cloud-3.2.2rc2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-dbt-cloud``
 
-Release: ``3.2.2``
+Release: ``3.2.2rc2``
 
 
 `dbt Cloud <https://www.getdbt.com/product/what-is-dbt/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-dbt-cloud-3.2.2/airflow/providers/dbt/cloud/__init__.py` & `apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.2/airflow/providers/dbt/cloud/get_provider_info.py` & `apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.2/airflow/providers/dbt/cloud/hooks/__init__.py` & `apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.2/airflow/providers/dbt/cloud/hooks/dbt.py` & `apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/hooks/dbt.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.2/airflow/providers/dbt/cloud/operators/__init__.py` & `apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.2/airflow/providers/dbt/cloud/operators/dbt.py` & `apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/operators/dbt.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.2/airflow/providers/dbt/cloud/sensors/__init__.py` & `apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.2/airflow/providers/dbt/cloud/sensors/dbt.py` & `apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/sensors/dbt.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.2/airflow/providers/dbt/cloud/triggers/__init__.py` & `apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.2/airflow/providers/dbt/cloud/triggers/dbt.py` & `apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/triggers/dbt.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.2/apache_airflow_providers_dbt_cloud.egg-info/PKG-INFO` & `apache-airflow-providers-dbt-cloud-3.2.2rc2/apache_airflow_providers_dbt_cloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-dbt-cloud
-Version: 3.2.2
+Version: 3.2.2rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-dbt-cloud package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.2.2/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-dbt-cloud``
 
-Release: ``3.2.2``
+Release: ``3.2.2rc2``
 
 
 `dbt Cloud <https://www.getdbt.com/product/what-is-dbt/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-dbt-cloud-3.2.2/apache_airflow_providers_dbt_cloud.egg-info/SOURCES.txt` & `apache-airflow-providers-dbt-cloud-3.2.2rc2/apache_airflow_providers_dbt_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.2/pyproject.toml` & `apache-airflow-providers-dbt-cloud-3.2.2rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.2/setup.cfg` & `apache-airflow-providers-dbt-cloud-3.2.2rc2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -45,21 +45,21 @@
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
 	aiohttp
 	apache-airflow-providers-http
-	apache-airflow>=2.4.0
+	apache-airflow>=2.4.0.dev0
 	asgiref
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.dbt.cloud.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.dbt.cloud
 
 [egg_info]
-tag_build = 
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-dbt-cloud-3.2.2/setup.py` & `apache-airflow-providers-dbt-cloud-3.2.2rc2/setup.py`

 * *Files identical despite different names*

