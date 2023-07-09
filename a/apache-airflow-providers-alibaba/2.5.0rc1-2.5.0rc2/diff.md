# Comparing `tmp/apache-airflow-providers-alibaba-2.5.0rc1.tar.gz` & `tmp/apache-airflow-providers-alibaba-2.5.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-alibaba-2.5.0rc1.tar", last modified: Wed Jul  5 07:29:29 2023, max compression
+gzip compressed data, was "apache-airflow-providers-alibaba-2.5.0rc2.tar", last modified: Thu Jul  6 04:49:59 2023, max compression
```

## Comparing `apache-airflow-providers-alibaba-2.5.0rc1.tar` & `apache-airflow-providers-alibaba-2.5.0rc2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:29.287224 apache-airflow-providers-alibaba-2.5.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-alibaba-2.5.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-05 07:29:27.000000 apache-airflow-providers-alibaba-2.5.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-alibaba-2.5.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4609 2023-07-05 07:29:29.287840 apache-airflow-providers-alibaba-2.5.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2967 2023-07-05 07:29:27.000000 apache-airflow-providers-alibaba-2.5.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:29.121996 apache-airflow-providers-alibaba-2.5.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:29.123924 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:29.195935 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/
--rw-r--r--   0 root         (0) root         (0)     1532 2023-07-05 07:19:39.000000 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:29.201380 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:29.214984 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14367 2023-06-28 06:26:40.000000 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/hooks/analyticdb_spark.py
--rw-r--r--   0 root         (0) root         (0)    12520 2023-06-28 06:26:40.000000 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/hooks/oss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:29.222802 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/log/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8577 2023-06-28 06:26:40.000000 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/log/oss_task_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:29.236099 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8288 2023-06-28 06:26:40.000000 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/operators/analyticdb_spark.py
--rw-r--r--   0 root         (0) root         (0)     6320 2023-06-02 11:31:21.000000 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/operators/oss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:29.248743 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2543 2023-06-28 06:26:40.000000 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/sensors/analyticdb_spark.py
--rw-r--r--   0 root         (0) root         (0)     3656 2023-06-28 06:26:40.000000 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/sensors/oss_key.py
--rw-r--r--   0 root         (0) root         (0)     4248 2023-07-05 07:29:27.000000 apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:29.284191 apache-airflow-providers-alibaba-2.5.0rc1/apache_airflow_providers_alibaba.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4609 2023-07-05 07:29:29.000000 apache-airflow-providers-alibaba-2.5.0rc1/apache_airflow_providers_alibaba.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1178 2023-07-05 07:29:29.000000 apache-airflow-providers-alibaba-2.5.0rc1/apache_airflow_providers_alibaba.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:29:29.000000 apache-airflow-providers-alibaba-2.5.0rc1/apache_airflow_providers_alibaba.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-07-05 07:29:29.000000 apache-airflow-providers-alibaba-2.5.0rc1/apache_airflow_providers_alibaba.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:29:29.000000 apache-airflow-providers-alibaba-2.5.0rc1/apache_airflow_providers_alibaba.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      104 2023-07-05 07:29:29.000000 apache-airflow-providers-alibaba-2.5.0rc1/apache_airflow_providers_alibaba.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-05 07:29:29.000000 apache-airflow-providers-alibaba-2.5.0rc1/apache_airflow_providers_alibaba.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-alibaba-2.5.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2012 2023-07-05 07:29:29.290250 apache-airflow-providers-alibaba-2.5.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1644 2023-07-05 07:29:27.000000 apache-airflow-providers-alibaba-2.5.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:49:59.177219 apache-airflow-providers-alibaba-2.5.0rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-alibaba-2.5.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-06 04:49:57.000000 apache-airflow-providers-alibaba-2.5.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-alibaba-2.5.0rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4609 2023-07-06 04:49:59.177788 apache-airflow-providers-alibaba-2.5.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2967 2023-07-06 04:49:57.000000 apache-airflow-providers-alibaba-2.5.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:49:59.070784 apache-airflow-providers-alibaba-2.5.0rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:49:59.072128 apache-airflow-providers-alibaba-2.5.0rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:49:59.113752 apache-airflow-providers-alibaba-2.5.0rc2/airflow/providers/alibaba/
+-rw-r--r--   0 root         (0) root         (0)     1532 2023-07-05 18:42:18.000000 apache-airflow-providers-alibaba-2.5.0rc2/airflow/providers/alibaba/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:49:59.116692 apache-airflow-providers-alibaba-2.5.0rc2/airflow/providers/alibaba/cloud/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-alibaba-2.5.0rc2/airflow/providers/alibaba/cloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:49:59.125374 apache-airflow-providers-alibaba-2.5.0rc2/airflow/providers/alibaba/cloud/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-alibaba-2.5.0rc2/airflow/providers/alibaba/cloud/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14367 2023-06-28 06:26:40.000000 apache-airflow-providers-alibaba-2.5.0rc2/airflow/providers/alibaba/cloud/hooks/analyticdb_spark.py
+-rw-r--r--   0 root         (0) root         (0)    12520 2023-06-28 06:26:40.000000 apache-airflow-providers-alibaba-2.5.0rc2/airflow/providers/alibaba/cloud/hooks/oss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:49:59.133138 apache-airflow-providers-alibaba-2.5.0rc2/airflow/providers/alibaba/cloud/log/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-alibaba-2.5.0rc2/airflow/providers/alibaba/cloud/log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8577 2023-06-28 06:26:40.000000 apache-airflow-providers-alibaba-2.5.0rc2/airflow/providers/alibaba/cloud/log/oss_task_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:49:59.141886 apache-airflow-providers-alibaba-2.5.0rc2/airflow/providers/alibaba/cloud/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-alibaba-2.5.0rc2/airflow/providers/alibaba/cloud/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8288 2023-06-28 06:26:40.000000 apache-airflow-providers-alibaba-2.5.0rc2/airflow/providers/alibaba/cloud/operators/analyticdb_spark.py
+-rw-r--r--   0 root         (0) root         (0)     6320 2023-06-02 11:31:21.000000 apache-airflow-providers-alibaba-2.5.0rc2/airflow/providers/alibaba/cloud/operators/oss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:49:59.150558 apache-airflow-providers-alibaba-2.5.0rc2/airflow/providers/alibaba/cloud/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-alibaba-2.5.0rc2/airflow/providers/alibaba/cloud/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2543 2023-06-28 06:26:40.000000 apache-airflow-providers-alibaba-2.5.0rc2/airflow/providers/alibaba/cloud/sensors/analyticdb_spark.py
+-rw-r--r--   0 root         (0) root         (0)     3656 2023-06-28 06:26:40.000000 apache-airflow-providers-alibaba-2.5.0rc2/airflow/providers/alibaba/cloud/sensors/oss_key.py
+-rw-r--r--   0 root         (0) root         (0)     4248 2023-07-06 04:49:57.000000 apache-airflow-providers-alibaba-2.5.0rc2/airflow/providers/alibaba/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:49:59.174908 apache-airflow-providers-alibaba-2.5.0rc2/apache_airflow_providers_alibaba.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4609 2023-07-06 04:49:58.000000 apache-airflow-providers-alibaba-2.5.0rc2/apache_airflow_providers_alibaba.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1178 2023-07-06 04:49:59.000000 apache-airflow-providers-alibaba-2.5.0rc2/apache_airflow_providers_alibaba.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:49:58.000000 apache-airflow-providers-alibaba-2.5.0rc2/apache_airflow_providers_alibaba.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-07-06 04:49:58.000000 apache-airflow-providers-alibaba-2.5.0rc2/apache_airflow_providers_alibaba.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:49:58.000000 apache-airflow-providers-alibaba-2.5.0rc2/apache_airflow_providers_alibaba.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      104 2023-07-06 04:49:58.000000 apache-airflow-providers-alibaba-2.5.0rc2/apache_airflow_providers_alibaba.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-06 04:49:58.000000 apache-airflow-providers-alibaba-2.5.0rc2/apache_airflow_providers_alibaba.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-alibaba-2.5.0rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2012 2023-07-06 04:49:59.179718 apache-airflow-providers-alibaba-2.5.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-07-06 04:49:57.000000 apache-airflow-providers-alibaba-2.5.0rc2/setup.py
```

### Comparing `apache-airflow-providers-alibaba-2.5.0rc1/LICENSE` & `apache-airflow-providers-alibaba-2.5.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.5.0rc1/MANIFEST.in` & `apache-airflow-providers-alibaba-2.5.0rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.5.0rc1/PKG-INFO` & `apache-airflow-providers-alibaba-2.5.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-alibaba
-Version: 2.5.0rc1
+Version: 2.5.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-alibaba package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-alibaba/2.5.0/
@@ -66,15 +66,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-alibaba``
 
-Release: ``2.5.0rc1``
+Release: ``2.5.0rc2``
 
 
 Alibaba Cloud integration (including `Alibaba Cloud <https://www.alibabacloud.com//>`__).
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-alibaba-2.5.0rc1/README.rst` & `apache-airflow-providers-alibaba-2.5.0rc2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-alibaba``
 
-Release: ``2.5.0rc1``
+Release: ``2.5.0rc2``
 
 
 Alibaba Cloud integration (including `Alibaba Cloud <https://www.alibabacloud.com//>`__).
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/__init__.py` & `apache-airflow-providers-alibaba-2.5.0rc2/airflow/providers/alibaba/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/__init__.py` & `apache-airflow-providers-alibaba-2.5.0rc2/airflow/providers/alibaba/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/hooks/__init__.py` & `apache-airflow-providers-alibaba-2.5.0rc2/airflow/providers/alibaba/cloud/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/hooks/analyticdb_spark.py` & `apache-airflow-providers-alibaba-2.5.0rc2/airflow/providers/alibaba/cloud/hooks/analyticdb_spark.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/hooks/oss.py` & `apache-airflow-providers-alibaba-2.5.0rc2/airflow/providers/alibaba/cloud/hooks/oss.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/log/__init__.py` & `apache-airflow-providers-alibaba-2.5.0rc2/airflow/providers/alibaba/cloud/log/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/log/oss_task_handler.py` & `apache-airflow-providers-alibaba-2.5.0rc2/airflow/providers/alibaba/cloud/log/oss_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/operators/__init__.py` & `apache-airflow-providers-alibaba-2.5.0rc2/airflow/providers/alibaba/cloud/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/operators/analyticdb_spark.py` & `apache-airflow-providers-alibaba-2.5.0rc2/airflow/providers/alibaba/cloud/operators/analyticdb_spark.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/operators/oss.py` & `apache-airflow-providers-alibaba-2.5.0rc2/airflow/providers/alibaba/cloud/operators/oss.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/sensors/__init__.py` & `apache-airflow-providers-alibaba-2.5.0rc2/airflow/providers/alibaba/cloud/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/sensors/analyticdb_spark.py` & `apache-airflow-providers-alibaba-2.5.0rc2/airflow/providers/alibaba/cloud/sensors/analyticdb_spark.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/cloud/sensors/oss_key.py` & `apache-airflow-providers-alibaba-2.5.0rc2/airflow/providers/alibaba/cloud/sensors/oss_key.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.5.0rc1/airflow/providers/alibaba/get_provider_info.py` & `apache-airflow-providers-alibaba-2.5.0rc2/airflow/providers/alibaba/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.5.0rc1/apache_airflow_providers_alibaba.egg-info/PKG-INFO` & `apache-airflow-providers-alibaba-2.5.0rc2/apache_airflow_providers_alibaba.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-alibaba
-Version: 2.5.0rc1
+Version: 2.5.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-alibaba package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-alibaba/2.5.0/
@@ -66,15 +66,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-alibaba``
 
-Release: ``2.5.0rc1``
+Release: ``2.5.0rc2``
 
 
 Alibaba Cloud integration (including `Alibaba Cloud <https://www.alibabacloud.com//>`__).
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-alibaba-2.5.0rc1/apache_airflow_providers_alibaba.egg-info/SOURCES.txt` & `apache-airflow-providers-alibaba-2.5.0rc2/apache_airflow_providers_alibaba.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.5.0rc1/pyproject.toml` & `apache-airflow-providers-alibaba-2.5.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.5.0rc1/setup.cfg` & `apache-airflow-providers-alibaba-2.5.0rc2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -56,10 +56,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.alibaba.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.alibaba
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-alibaba-2.5.0rc1/setup.py` & `apache-airflow-providers-alibaba-2.5.0rc2/setup.py`

 * *Files identical despite different names*

