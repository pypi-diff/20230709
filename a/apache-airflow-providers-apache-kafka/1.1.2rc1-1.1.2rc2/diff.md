# Comparing `tmp/apache-airflow-providers-apache-kafka-1.1.2rc1.tar.gz` & `tmp/apache-airflow-providers-apache-kafka-1.1.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-apache-kafka-1.1.2rc1.tar", last modified: Wed Jul  5 07:29:39 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-kafka-1.1.2rc2.tar", last modified: Thu Jul  6 04:50:15 2023, max compression
```

## Comparing `apache-airflow-providers-apache-kafka-1.1.2rc1.tar` & `apache-airflow-providers-apache-kafka-1.1.2rc2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:39.800284 apache-airflow-providers-apache-kafka-1.1.2rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-05 07:29:38.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4488 2023-07-05 07:29:39.800932 apache-airflow-providers-apache-kafka-1.1.2rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2826 2023-07-05 07:29:38.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:39.673005 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:39.674100 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:39.675729 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:39.724412 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/
--rw-r--r--   0 root         (0) root         (0)     1537 2023-07-05 07:19:39.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3048 2023-07-05 07:29:38.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:39.743020 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2736 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/hooks/base.py
--rw-r--r--   0 root         (0) root         (0)     2353 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/hooks/client.py
--rw-r--r--   0 root         (0) root         (0)     1677 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/hooks/consume.py
--rw-r--r--   0 root         (0) root         (0)     1551 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/hooks/produce.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:39.753928 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8020 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/operators/consume.py
--rw-r--r--   0 root         (0) root         (0)     4951 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/operators/produce.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:39.760817 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8219 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/sensors/kafka.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:39.767737 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4940 2023-07-01 06:49:42.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/triggers/await_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:39.797219 apache-airflow-providers-apache-kafka-1.1.2rc1/apache_airflow_providers_apache_kafka.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4488 2023-07-05 07:29:39.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/apache_airflow_providers_apache_kafka.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1196 2023-07-05 07:29:39.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/apache_airflow_providers_apache_kafka.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:29:39.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/apache_airflow_providers_apache_kafka.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-07-05 07:29:39.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/apache_airflow_providers_apache_kafka.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:29:39.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/apache_airflow_providers_apache_kafka.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       58 2023-07-05 07:29:39.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/apache_airflow_providers_apache_kafka.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-05 07:29:39.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/apache_airflow_providers_apache_kafka.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2000 2023-07-05 07:29:39.803229 apache-airflow-providers-apache-kafka-1.1.2rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-05 07:29:38.000000 apache-airflow-providers-apache-kafka-1.1.2rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:15.670131 apache-airflow-providers-apache-kafka-1.1.2rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-kafka-1.1.2rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-06 04:50:14.000000 apache-airflow-providers-apache-kafka-1.1.2rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-kafka-1.1.2rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4488 2023-07-06 04:50:15.670700 apache-airflow-providers-apache-kafka-1.1.2rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2826 2023-07-06 04:50:14.000000 apache-airflow-providers-apache-kafka-1.1.2rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:15.571594 apache-airflow-providers-apache-kafka-1.1.2rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:15.572630 apache-airflow-providers-apache-kafka-1.1.2rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:15.573666 apache-airflow-providers-apache-kafka-1.1.2rc2/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:15.609486 apache-airflow-providers-apache-kafka-1.1.2rc2/airflow/providers/apache/kafka/
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-07-05 18:46:30.000000 apache-airflow-providers-apache-kafka-1.1.2rc2/airflow/providers/apache/kafka/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3048 2023-07-06 04:50:14.000000 apache-airflow-providers-apache-kafka-1.1.2rc2/airflow/providers/apache/kafka/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:15.624107 apache-airflow-providers-apache-kafka-1.1.2rc2/airflow/providers/apache/kafka/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kafka-1.1.2rc2/airflow/providers/apache/kafka/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2736 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kafka-1.1.2rc2/airflow/providers/apache/kafka/hooks/base.py
+-rw-r--r--   0 root         (0) root         (0)     2353 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kafka-1.1.2rc2/airflow/providers/apache/kafka/hooks/client.py
+-rw-r--r--   0 root         (0) root         (0)     1677 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kafka-1.1.2rc2/airflow/providers/apache/kafka/hooks/consume.py
+-rw-r--r--   0 root         (0) root         (0)     1551 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kafka-1.1.2rc2/airflow/providers/apache/kafka/hooks/produce.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:15.632721 apache-airflow-providers-apache-kafka-1.1.2rc2/airflow/providers/apache/kafka/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kafka-1.1.2rc2/airflow/providers/apache/kafka/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8020 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kafka-1.1.2rc2/airflow/providers/apache/kafka/operators/consume.py
+-rw-r--r--   0 root         (0) root         (0)     4951 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kafka-1.1.2rc2/airflow/providers/apache/kafka/operators/produce.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:15.638474 apache-airflow-providers-apache-kafka-1.1.2rc2/airflow/providers/apache/kafka/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kafka-1.1.2rc2/airflow/providers/apache/kafka/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8219 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-kafka-1.1.2rc2/airflow/providers/apache/kafka/sensors/kafka.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:15.644327 apache-airflow-providers-apache-kafka-1.1.2rc2/airflow/providers/apache/kafka/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kafka-1.1.2rc2/airflow/providers/apache/kafka/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4940 2023-07-01 06:49:42.000000 apache-airflow-providers-apache-kafka-1.1.2rc2/airflow/providers/apache/kafka/triggers/await_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:15.667750 apache-airflow-providers-apache-kafka-1.1.2rc2/apache_airflow_providers_apache_kafka.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4488 2023-07-06 04:50:15.000000 apache-airflow-providers-apache-kafka-1.1.2rc2/apache_airflow_providers_apache_kafka.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1196 2023-07-06 04:50:15.000000 apache-airflow-providers-apache-kafka-1.1.2rc2/apache_airflow_providers_apache_kafka.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:15.000000 apache-airflow-providers-apache-kafka-1.1.2rc2/apache_airflow_providers_apache_kafka.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-07-06 04:50:15.000000 apache-airflow-providers-apache-kafka-1.1.2rc2/apache_airflow_providers_apache_kafka.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:15.000000 apache-airflow-providers-apache-kafka-1.1.2rc2/apache_airflow_providers_apache_kafka.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       58 2023-07-06 04:50:15.000000 apache-airflow-providers-apache-kafka-1.1.2rc2/apache_airflow_providers_apache_kafka.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-06 04:50:15.000000 apache-airflow-providers-apache-kafka-1.1.2rc2/apache_airflow_providers_apache_kafka.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-apache-kafka-1.1.2rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2000 2023-07-06 04:50:15.672671 apache-airflow-providers-apache-kafka-1.1.2rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-06 04:50:14.000000 apache-airflow-providers-apache-kafka-1.1.2rc2/setup.py
```

### Comparing `apache-airflow-providers-apache-kafka-1.1.2rc1/LICENSE` & `apache-airflow-providers-apache-kafka-1.1.2rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.2rc1/MANIFEST.in` & `apache-airflow-providers-apache-kafka-1.1.2rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.2rc1/PKG-INFO` & `apache-airflow-providers-apache-kafka-1.1.2rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-kafka
-Version: 1.1.2rc1
+Version: 1.1.2rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-kafka package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-kafka/1.1.2/
@@ -66,15 +66,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apache-kafka``
 
-Release: ``1.1.2rc1``
+Release: ``1.1.2rc2``
 
 
 `Apache Kafka  <https://kafka.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-kafka-1.1.2rc1/README.rst` & `apache-airflow-providers-apache-kafka-1.1.2rc2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apache-kafka``
 
-Release: ``1.1.2rc1``
+Release: ``1.1.2rc2``
 
 
 `Apache Kafka  <https://kafka.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/__init__.py` & `apache-airflow-providers-apache-kafka-1.1.2rc2/airflow/providers/apache/kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/get_provider_info.py` & `apache-airflow-providers-apache-kafka-1.1.2rc2/airflow/providers/apache/kafka/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/hooks/__init__.py` & `apache-airflow-providers-apache-kafka-1.1.2rc2/airflow/providers/apache/kafka/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/hooks/base.py` & `apache-airflow-providers-apache-kafka-1.1.2rc2/airflow/providers/apache/kafka/hooks/base.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/hooks/client.py` & `apache-airflow-providers-apache-kafka-1.1.2rc2/airflow/providers/apache/kafka/hooks/client.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/hooks/consume.py` & `apache-airflow-providers-apache-kafka-1.1.2rc2/airflow/providers/apache/kafka/hooks/consume.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/hooks/produce.py` & `apache-airflow-providers-apache-kafka-1.1.2rc2/airflow/providers/apache/kafka/hooks/produce.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/operators/__init__.py` & `apache-airflow-providers-apache-kafka-1.1.2rc2/airflow/providers/apache/kafka/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/operators/consume.py` & `apache-airflow-providers-apache-kafka-1.1.2rc2/airflow/providers/apache/kafka/operators/consume.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/operators/produce.py` & `apache-airflow-providers-apache-kafka-1.1.2rc2/airflow/providers/apache/kafka/operators/produce.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/sensors/__init__.py` & `apache-airflow-providers-apache-kafka-1.1.2rc2/airflow/providers/apache/kafka/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/sensors/kafka.py` & `apache-airflow-providers-apache-kafka-1.1.2rc2/airflow/providers/apache/kafka/sensors/kafka.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/triggers/__init__.py` & `apache-airflow-providers-apache-kafka-1.1.2rc2/airflow/providers/apache/kafka/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.2rc1/airflow/providers/apache/kafka/triggers/await_message.py` & `apache-airflow-providers-apache-kafka-1.1.2rc2/airflow/providers/apache/kafka/triggers/await_message.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.2rc1/apache_airflow_providers_apache_kafka.egg-info/PKG-INFO` & `apache-airflow-providers-apache-kafka-1.1.2rc2/apache_airflow_providers_apache_kafka.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-kafka
-Version: 1.1.2rc1
+Version: 1.1.2rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-kafka package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-kafka/1.1.2/
@@ -66,15 +66,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apache-kafka``
 
-Release: ``1.1.2rc1``
+Release: ``1.1.2rc2``
 
 
 `Apache Kafka  <https://kafka.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-kafka-1.1.2rc1/apache_airflow_providers_apache_kafka.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-kafka-1.1.2rc2/apache_airflow_providers_apache_kafka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.2rc1/pyproject.toml` & `apache-airflow-providers-apache-kafka-1.1.2rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.2rc1/setup.cfg` & `apache-airflow-providers-apache-kafka-1.1.2rc2/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -55,10 +55,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.apache.kafka.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.apache.kafka
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-apache-kafka-1.1.2rc1/setup.py` & `apache-airflow-providers-apache-kafka-1.1.2rc2/setup.py`

 * *Files identical despite different names*

