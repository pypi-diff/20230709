# Comparing `tmp/apache-airflow-providers-apache-livy-3.5.2rc1.tar.gz` & `tmp/apache-airflow-providers-apache-livy-3.5.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-apache-livy-3.5.2rc1.tar", last modified: Wed Jul  5 07:29:42 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-livy-3.5.2rc2.tar", last modified: Thu Jul  6 04:50:18 2023, max compression
```

## Comparing `apache-airflow-providers-apache-livy-3.5.2rc1.tar` & `apache-airflow-providers-apache-livy-3.5.2rc2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:42.460564 apache-airflow-providers-apache-livy-3.5.2rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-livy-3.5.2rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-05 07:29:41.000000 apache-airflow-providers-apache-livy-3.5.2rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-livy-3.5.2rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5526 2023-07-05 07:29:42.461188 apache-airflow-providers-apache-livy-3.5.2rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3847 2023-07-05 07:29:41.000000 apache-airflow-providers-apache-livy-3.5.2rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:42.369750 apache-airflow-providers-apache-livy-3.5.2rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:42.371133 apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:42.372332 apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:42.409440 apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/
--rw-r--r--   0 root         (0) root         (0)     1536 2023-07-05 07:19:39.000000 apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3103 2023-07-05 07:29:41.000000 apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:42.415266 apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31553 2023-06-28 06:26:40.000000 apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/hooks/livy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:42.421751 apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9646 2023-07-05 07:19:39.000000 apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/operators/livy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:42.427649 apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2574 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/sensors/livy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:42.433513 apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6251 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/triggers/livy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:42.458122 apache-airflow-providers-apache-livy-3.5.2rc1/apache_airflow_providers_apache_livy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5526 2023-07-05 07:29:42.000000 apache-airflow-providers-apache-livy-3.5.2rc1/apache_airflow_providers_apache_livy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      971 2023-07-05 07:29:42.000000 apache-airflow-providers-apache-livy-3.5.2rc1/apache_airflow_providers_apache_livy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:29:42.000000 apache-airflow-providers-apache-livy-3.5.2rc1/apache_airflow_providers_apache_livy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2023-07-05 07:29:42.000000 apache-airflow-providers-apache-livy-3.5.2rc1/apache_airflow_providers_apache_livy.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:29:42.000000 apache-airflow-providers-apache-livy-3.5.2rc1/apache_airflow_providers_apache_livy.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      111 2023-07-05 07:29:42.000000 apache-airflow-providers-apache-livy-3.5.2rc1/apache_airflow_providers_apache_livy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-05 07:29:42.000000 apache-airflow-providers-apache-livy-3.5.2rc1/apache_airflow_providers_apache_livy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-apache-livy-3.5.2rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2009 2023-07-05 07:29:42.463149 apache-airflow-providers-apache-livy-3.5.2rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1709 2023-07-05 07:29:41.000000 apache-airflow-providers-apache-livy-3.5.2rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:18.554874 apache-airflow-providers-apache-livy-3.5.2rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-livy-3.5.2rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-06 04:50:17.000000 apache-airflow-providers-apache-livy-3.5.2rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-livy-3.5.2rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5526 2023-07-06 04:50:18.555490 apache-airflow-providers-apache-livy-3.5.2rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3847 2023-07-06 04:50:17.000000 apache-airflow-providers-apache-livy-3.5.2rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:18.465678 apache-airflow-providers-apache-livy-3.5.2rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:18.466863 apache-airflow-providers-apache-livy-3.5.2rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:18.467984 apache-airflow-providers-apache-livy-3.5.2rc2/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:18.505003 apache-airflow-providers-apache-livy-3.5.2rc2/airflow/providers/apache/livy/
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-07-05 18:46:47.000000 apache-airflow-providers-apache-livy-3.5.2rc2/airflow/providers/apache/livy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3103 2023-07-06 04:50:17.000000 apache-airflow-providers-apache-livy-3.5.2rc2/airflow/providers/apache/livy/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:18.510873 apache-airflow-providers-apache-livy-3.5.2rc2/airflow/providers/apache/livy/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-livy-3.5.2rc2/airflow/providers/apache/livy/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31553 2023-06-28 06:26:40.000000 apache-airflow-providers-apache-livy-3.5.2rc2/airflow/providers/apache/livy/hooks/livy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:18.517147 apache-airflow-providers-apache-livy-3.5.2rc2/airflow/providers/apache/livy/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-livy-3.5.2rc2/airflow/providers/apache/livy/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9646 2023-07-05 07:19:39.000000 apache-airflow-providers-apache-livy-3.5.2rc2/airflow/providers/apache/livy/operators/livy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:18.522914 apache-airflow-providers-apache-livy-3.5.2rc2/airflow/providers/apache/livy/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-livy-3.5.2rc2/airflow/providers/apache/livy/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2574 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-livy-3.5.2rc2/airflow/providers/apache/livy/sensors/livy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:18.528522 apache-airflow-providers-apache-livy-3.5.2rc2/airflow/providers/apache/livy/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-livy-3.5.2rc2/airflow/providers/apache/livy/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6251 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-livy-3.5.2rc2/airflow/providers/apache/livy/triggers/livy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:18.552208 apache-airflow-providers-apache-livy-3.5.2rc2/apache_airflow_providers_apache_livy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5526 2023-07-06 04:50:18.000000 apache-airflow-providers-apache-livy-3.5.2rc2/apache_airflow_providers_apache_livy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      971 2023-07-06 04:50:18.000000 apache-airflow-providers-apache-livy-3.5.2rc2/apache_airflow_providers_apache_livy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:18.000000 apache-airflow-providers-apache-livy-3.5.2rc2/apache_airflow_providers_apache_livy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2023-07-06 04:50:18.000000 apache-airflow-providers-apache-livy-3.5.2rc2/apache_airflow_providers_apache_livy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:18.000000 apache-airflow-providers-apache-livy-3.5.2rc2/apache_airflow_providers_apache_livy.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      111 2023-07-06 04:50:18.000000 apache-airflow-providers-apache-livy-3.5.2rc2/apache_airflow_providers_apache_livy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-06 04:50:18.000000 apache-airflow-providers-apache-livy-3.5.2rc2/apache_airflow_providers_apache_livy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-apache-livy-3.5.2rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2009 2023-07-06 04:50:18.557371 apache-airflow-providers-apache-livy-3.5.2rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-07-06 04:50:17.000000 apache-airflow-providers-apache-livy-3.5.2rc2/setup.py
```

### Comparing `apache-airflow-providers-apache-livy-3.5.2rc1/LICENSE` & `apache-airflow-providers-apache-livy-3.5.2rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.2rc1/MANIFEST.in` & `apache-airflow-providers-apache-livy-3.5.2rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.2rc1/PKG-INFO` & `apache-airflow-providers-apache-livy-3.5.2rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-livy
-Version: 3.5.2rc1
+Version: 3.5.2rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-livy package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-livy/3.5.2/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apache-livy``
 
-Release: ``3.5.2rc1``
+Release: ``3.5.2rc2``
 
 
 `Apache Livy <https://livy.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-livy-3.5.2rc1/README.rst` & `apache-airflow-providers-apache-livy-3.5.2rc2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apache-livy``
 
-Release: ``3.5.2rc1``
+Release: ``3.5.2rc2``
 
 
 `Apache Livy <https://livy.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/__init__.py` & `apache-airflow-providers-apache-livy-3.5.2rc2/airflow/providers/apache/livy/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/get_provider_info.py` & `apache-airflow-providers-apache-livy-3.5.2rc2/airflow/providers/apache/livy/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/hooks/__init__.py` & `apache-airflow-providers-apache-livy-3.5.2rc2/airflow/providers/apache/livy/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/hooks/livy.py` & `apache-airflow-providers-apache-livy-3.5.2rc2/airflow/providers/apache/livy/hooks/livy.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/operators/__init__.py` & `apache-airflow-providers-apache-livy-3.5.2rc2/airflow/providers/apache/livy/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/operators/livy.py` & `apache-airflow-providers-apache-livy-3.5.2rc2/airflow/providers/apache/livy/operators/livy.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/sensors/__init__.py` & `apache-airflow-providers-apache-livy-3.5.2rc2/airflow/providers/apache/livy/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/sensors/livy.py` & `apache-airflow-providers-apache-livy-3.5.2rc2/airflow/providers/apache/livy/sensors/livy.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/triggers/__init__.py` & `apache-airflow-providers-apache-livy-3.5.2rc2/airflow/providers/apache/livy/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.2rc1/airflow/providers/apache/livy/triggers/livy.py` & `apache-airflow-providers-apache-livy-3.5.2rc2/airflow/providers/apache/livy/triggers/livy.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.2rc1/apache_airflow_providers_apache_livy.egg-info/PKG-INFO` & `apache-airflow-providers-apache-livy-3.5.2rc2/apache_airflow_providers_apache_livy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-livy
-Version: 3.5.2rc1
+Version: 3.5.2rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-livy package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-livy/3.5.2/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apache-livy``
 
-Release: ``3.5.2rc1``
+Release: ``3.5.2rc2``
 
 
 `Apache Livy <https://livy.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-livy-3.5.2rc1/apache_airflow_providers_apache_livy.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-livy-3.5.2rc2/apache_airflow_providers_apache_livy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.2rc1/pyproject.toml` & `apache-airflow-providers-apache-livy-3.5.2rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.2rc1/setup.cfg` & `apache-airflow-providers-apache-livy-3.5.2rc2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -56,10 +56,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.apache.livy.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.apache.livy
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-apache-livy-3.5.2rc1/setup.py` & `apache-airflow-providers-apache-livy-3.5.2rc2/setup.py`

 * *Files identical despite different names*

