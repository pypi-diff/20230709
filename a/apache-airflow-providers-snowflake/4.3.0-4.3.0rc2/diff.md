# Comparing `tmp/apache-airflow-providers-snowflake-4.3.0.tar.gz` & `tmp/apache-airflow-providers-snowflake-4.3.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-snowflake-4.3.0.tar", last modified: Thu Jul  6 04:45:13 2023, max compression
+gzip compressed data, was "apache-airflow-providers-snowflake-4.3.0rc2.tar", last modified: Thu Jul  6 04:51:33 2023, max compression
```

## Comparing `apache-airflow-providers-snowflake-4.3.0.tar` & `apache-airflow-providers-snowflake-4.3.0rc2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:45:13.770460 apache-airflow-providers-snowflake-4.3.0/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-06 04:45:12.000000 apache-airflow-providers-snowflake-4.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5867 2023-07-06 04:45:13.771038 apache-airflow-providers-snowflake-4.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4171 2023-07-06 04:45:12.000000 apache-airflow-providers-snowflake-4.3.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:45:13.659715 apache-airflow-providers-snowflake-4.3.0/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:45:13.660961 apache-airflow-providers-snowflake-4.3.0/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:45:13.700591 apache-airflow-providers-snowflake-4.3.0/airflow/providers/snowflake/
--rw-r--r--   0 root         (0) root         (0)     1534 2023-07-06 04:42:33.000000 apache-airflow-providers-snowflake-4.3.0/airflow/providers/snowflake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4949 2023-07-06 04:45:12.000000 apache-airflow-providers-snowflake-4.3.0/airflow/providers/snowflake/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:45:13.710912 apache-airflow-providers-snowflake-4.3.0/airflow/providers/snowflake/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.0/airflow/providers/snowflake/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17859 2023-06-05 12:50:36.000000 apache-airflow-providers-snowflake-4.3.0/airflow/providers/snowflake/hooks/snowflake.py
--rw-r--r--   0 root         (0) root         (0)    12676 2023-07-05 07:19:39.000000 apache-airflow-providers-snowflake-4.3.0/airflow/providers/snowflake/hooks/snowflake_sql_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:45:13.717484 apache-airflow-providers-snowflake-4.3.0/airflow/providers/snowflake/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.0/airflow/providers/snowflake/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24666 2023-07-05 07:19:39.000000 apache-airflow-providers-snowflake-4.3.0/airflow/providers/snowflake/operators/snowflake.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:45:13.730292 apache-airflow-providers-snowflake-4.3.0/airflow/providers/snowflake/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.0/airflow/providers/snowflake/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5786 2023-06-02 11:31:21.000000 apache-airflow-providers-snowflake-4.3.0/airflow/providers/snowflake/transfers/copy_into_snowflake.py
--rw-r--r--   0 root         (0) root         (0)     6054 2023-06-02 11:31:21.000000 apache-airflow-providers-snowflake-4.3.0/airflow/providers/snowflake/transfers/s3_to_snowflake.py
--rw-r--r--   0 root         (0) root         (0)     5078 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.0/airflow/providers/snowflake/transfers/snowflake_to_slack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:45:13.736071 apache-airflow-providers-snowflake-4.3.0/airflow/providers/snowflake/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-07-05 07:19:39.000000 apache-airflow-providers-snowflake-4.3.0/airflow/providers/snowflake/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4306 2023-07-05 07:19:39.000000 apache-airflow-providers-snowflake-4.3.0/airflow/providers/snowflake/triggers/snowflake_trigger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:45:13.744712 apache-airflow-providers-snowflake-4.3.0/airflow/providers/snowflake/utils/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.0/airflow/providers/snowflake/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1644 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.0/airflow/providers/snowflake/utils/common.py
--rw-r--r--   0 root         (0) root         (0)     6878 2023-06-01 07:44:14.000000 apache-airflow-providers-snowflake-4.3.0/airflow/providers/snowflake/utils/sql_api_generate_jwt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:45:13.768139 apache-airflow-providers-snowflake-4.3.0/apache_airflow_providers_snowflake.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5867 2023-07-06 04:45:13.000000 apache-airflow-providers-snowflake-4.3.0/apache_airflow_providers_snowflake.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1299 2023-07-06 04:45:13.000000 apache-airflow-providers-snowflake-4.3.0/apache_airflow_providers_snowflake.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:45:13.000000 apache-airflow-providers-snowflake-4.3.0/apache_airflow_providers_snowflake.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-07-06 04:45:13.000000 apache-airflow-providers-snowflake-4.3.0/apache_airflow_providers_snowflake.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:45:13.000000 apache-airflow-providers-snowflake-4.3.0/apache_airflow_providers_snowflake.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      217 2023-07-06 04:45:13.000000 apache-airflow-providers-snowflake-4.3.0/apache_airflow_providers_snowflake.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-06 04:45:13.000000 apache-airflow-providers-snowflake-4.3.0/apache_airflow_providers_snowflake.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-snowflake-4.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2046 2023-07-06 04:45:13.772873 apache-airflow-providers-snowflake-4.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1789 2023-07-06 04:45:12.000000 apache-airflow-providers-snowflake-4.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:33.382175 apache-airflow-providers-snowflake-4.3.0rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-06 04:51:32.000000 apache-airflow-providers-snowflake-4.3.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.0rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5873 2023-07-06 04:51:33.382708 apache-airflow-providers-snowflake-4.3.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4174 2023-07-06 04:51:32.000000 apache-airflow-providers-snowflake-4.3.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:33.267934 apache-airflow-providers-snowflake-4.3.0rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:33.269026 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:33.309311 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/
+-rw-r--r--   0 root         (0) root         (0)     1534 2023-07-06 04:42:33.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4949 2023-07-06 04:51:32.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:33.319211 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17859 2023-06-05 12:50:36.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/hooks/snowflake.py
+-rw-r--r--   0 root         (0) root         (0)    12676 2023-07-05 07:19:39.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/hooks/snowflake_sql_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:33.325917 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24666 2023-07-05 07:19:39.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/operators/snowflake.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:33.338441 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5786 2023-06-02 11:31:21.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/transfers/copy_into_snowflake.py
+-rw-r--r--   0 root         (0) root         (0)     6054 2023-06-02 11:31:21.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/transfers/s3_to_snowflake.py
+-rw-r--r--   0 root         (0) root         (0)     5078 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/transfers/snowflake_to_slack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:33.344467 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-07-05 07:19:39.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4306 2023-07-05 07:19:39.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/triggers/snowflake_trigger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:33.354559 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/utils/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/utils/common.py
+-rw-r--r--   0 root         (0) root         (0)     6878 2023-06-01 07:44:14.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/utils/sql_api_generate_jwt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:33.379560 apache-airflow-providers-snowflake-4.3.0rc2/apache_airflow_providers_snowflake.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5873 2023-07-06 04:51:33.000000 apache-airflow-providers-snowflake-4.3.0rc2/apache_airflow_providers_snowflake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1299 2023-07-06 04:51:33.000000 apache-airflow-providers-snowflake-4.3.0rc2/apache_airflow_providers_snowflake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:51:33.000000 apache-airflow-providers-snowflake-4.3.0rc2/apache_airflow_providers_snowflake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-07-06 04:51:33.000000 apache-airflow-providers-snowflake-4.3.0rc2/apache_airflow_providers_snowflake.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:51:33.000000 apache-airflow-providers-snowflake-4.3.0rc2/apache_airflow_providers_snowflake.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      227 2023-07-06 04:51:33.000000 apache-airflow-providers-snowflake-4.3.0rc2/apache_airflow_providers_snowflake.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-06 04:51:33.000000 apache-airflow-providers-snowflake-4.3.0rc2/apache_airflow_providers_snowflake.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-snowflake-4.3.0rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2059 2023-07-06 04:51:33.384605 apache-airflow-providers-snowflake-4.3.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1789 2023-07-06 04:51:32.000000 apache-airflow-providers-snowflake-4.3.0rc2/setup.py
```

### Comparing `apache-airflow-providers-snowflake-4.3.0/LICENSE` & `apache-airflow-providers-snowflake-4.3.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.0/MANIFEST.in` & `apache-airflow-providers-snowflake-4.3.0rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.0/PKG-INFO` & `apache-airflow-providers-snowflake-4.3.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-snowflake
-Version: 4.3.0
+Version: 4.3.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-snowflake package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.0/
@@ -68,15 +68,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-snowflake``
 
-Release: ``4.3.0``
+Release: ``4.3.0rc2``
 
 
 `Snowflake <https://www.snowflake.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-snowflake-4.3.0/README.rst` & `apache-airflow-providers-snowflake-4.3.0rc2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-snowflake``
 
-Release: ``4.3.0``
+Release: ``4.3.0rc2``
 
 
 `Snowflake <https://www.snowflake.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-snowflake-4.3.0/airflow/providers/snowflake/__init__.py` & `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.0/airflow/providers/snowflake/get_provider_info.py` & `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.0/airflow/providers/snowflake/hooks/__init__.py` & `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.0/airflow/providers/snowflake/hooks/snowflake.py` & `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/hooks/snowflake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.0/airflow/providers/snowflake/hooks/snowflake_sql_api.py` & `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/hooks/snowflake_sql_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.0/airflow/providers/snowflake/operators/__init__.py` & `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.0/airflow/providers/snowflake/operators/snowflake.py` & `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/operators/snowflake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.0/airflow/providers/snowflake/transfers/__init__.py` & `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.0/airflow/providers/snowflake/transfers/copy_into_snowflake.py` & `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/transfers/copy_into_snowflake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.0/airflow/providers/snowflake/transfers/s3_to_snowflake.py` & `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/transfers/s3_to_snowflake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.0/airflow/providers/snowflake/transfers/snowflake_to_slack.py` & `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/transfers/snowflake_to_slack.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.0/airflow/providers/snowflake/triggers/__init__.py` & `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.0/airflow/providers/snowflake/triggers/snowflake_trigger.py` & `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/triggers/snowflake_trigger.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.0/airflow/providers/snowflake/utils/__init__.py` & `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.0/airflow/providers/snowflake/utils/common.py` & `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/utils/common.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.0/airflow/providers/snowflake/utils/sql_api_generate_jwt.py` & `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/utils/sql_api_generate_jwt.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.0/apache_airflow_providers_snowflake.egg-info/PKG-INFO` & `apache-airflow-providers-snowflake-4.3.0rc2/apache_airflow_providers_snowflake.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-snowflake
-Version: 4.3.0
+Version: 4.3.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-snowflake package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.0/
@@ -68,15 +68,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-snowflake``
 
-Release: ``4.3.0``
+Release: ``4.3.0rc2``
 
 
 `Snowflake <https://www.snowflake.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-snowflake-4.3.0/apache_airflow_providers_snowflake.egg-info/SOURCES.txt` & `apache-airflow-providers-snowflake-4.3.0rc2/apache_airflow_providers_snowflake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.0/pyproject.toml` & `apache-airflow-providers-snowflake-4.3.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.0/setup.cfg` & `apache-airflow-providers-snowflake-4.3.0rc2/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -43,23 +43,23 @@
 include_package_data = True
 python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
-	apache-airflow-providers-common-sql>=1.3.1
-	apache-airflow>=2.4.0
+	apache-airflow-providers-common-sql>=1.3.1.dev0
+	apache-airflow>=2.4.0.dev0
 	snowflake-connector-python>=2.4.1
 	snowflake-sqlalchemy>=1.1.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.snowflake.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.snowflake
 
 [egg_info]
-tag_build = 
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-snowflake-4.3.0/setup.py` & `apache-airflow-providers-snowflake-4.3.0rc2/setup.py`

 * *Files identical despite different names*

