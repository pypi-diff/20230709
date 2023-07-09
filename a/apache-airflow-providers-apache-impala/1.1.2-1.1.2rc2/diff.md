# Comparing `tmp/apache-airflow-providers-apache-impala-1.1.2.tar.gz` & `tmp/apache-airflow-providers-apache-impala-1.1.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-apache-impala-1.1.2.tar", last modified: Thu Jul  6 04:44:10 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-impala-1.1.2rc2.tar", last modified: Thu Jul  6 04:50:13 2023, max compression
```

## Comparing `apache-airflow-providers-apache-impala-1.1.2.tar` & `apache-airflow-providers-apache-impala-1.1.2rc2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:44:10.012817 apache-airflow-providers-apache-impala-1.1.2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-impala-1.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-06 04:44:08.000000 apache-airflow-providers-apache-impala-1.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-impala-1.1.2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5573 2023-07-06 04:44:10.014370 apache-airflow-providers-apache-impala-1.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3858 2023-07-06 04:44:08.000000 apache-airflow-providers-apache-impala-1.1.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:44:09.801883 apache-airflow-providers-apache-impala-1.1.2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:44:09.804511 apache-airflow-providers-apache-impala-1.1.2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:44:09.806457 apache-airflow-providers-apache-impala-1.1.2/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:44:09.903403 apache-airflow-providers-apache-impala-1.1.2/airflow/providers/apache/impala/
--rw-r--r--   0 root         (0) root         (0)     1538 2023-07-06 04:42:33.000000 apache-airflow-providers-apache-impala-1.1.2/airflow/providers/apache/impala/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2114 2023-07-06 04:44:08.000000 apache-airflow-providers-apache-impala-1.1.2/airflow/providers/apache/impala/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:44:09.919365 apache-airflow-providers-apache-impala-1.1.2/airflow/providers/apache/impala/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-impala-1.1.2/airflow/providers/apache/impala/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1559 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-impala-1.1.2/airflow/providers/apache/impala/hooks/impala.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:44:10.005354 apache-airflow-providers-apache-impala-1.1.2/apache_airflow_providers_apache_impala.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5573 2023-07-06 04:44:09.000000 apache-airflow-providers-apache-impala-1.1.2/apache_airflow_providers_apache_impala.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      701 2023-07-06 04:44:09.000000 apache-airflow-providers-apache-impala-1.1.2/apache_airflow_providers_apache_impala.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:44:09.000000 apache-airflow-providers-apache-impala-1.1.2/apache_airflow_providers_apache_impala.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      110 2023-07-06 04:44:09.000000 apache-airflow-providers-apache-impala-1.1.2/apache_airflow_providers_apache_impala.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:44:09.000000 apache-airflow-providers-apache-impala-1.1.2/apache_airflow_providers_apache_impala.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      120 2023-07-06 04:44:09.000000 apache-airflow-providers-apache-impala-1.1.2/apache_airflow_providers_apache_impala.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-06 04:44:09.000000 apache-airflow-providers-apache-impala-1.1.2/apache_airflow_providers_apache_impala.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-apache-impala-1.1.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1987 2023-07-06 04:44:10.020068 apache-airflow-providers-apache-impala-1.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1801 2023-07-06 04:44:08.000000 apache-airflow-providers-apache-impala-1.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:13.808405 apache-airflow-providers-apache-impala-1.1.2rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-impala-1.1.2rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-06 04:50:12.000000 apache-airflow-providers-apache-impala-1.1.2rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-impala-1.1.2rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5579 2023-07-06 04:50:13.808966 apache-airflow-providers-apache-impala-1.1.2rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3861 2023-07-06 04:50:12.000000 apache-airflow-providers-apache-impala-1.1.2rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:13.726298 apache-airflow-providers-apache-impala-1.1.2rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:13.727558 apache-airflow-providers-apache-impala-1.1.2rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:13.728786 apache-airflow-providers-apache-impala-1.1.2rc2/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:13.763440 apache-airflow-providers-apache-impala-1.1.2rc2/airflow/providers/apache/impala/
+-rw-r--r--   0 root         (0) root         (0)     1538 2023-07-06 04:42:33.000000 apache-airflow-providers-apache-impala-1.1.2rc2/airflow/providers/apache/impala/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-07-06 04:50:12.000000 apache-airflow-providers-apache-impala-1.1.2rc2/airflow/providers/apache/impala/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:13.769763 apache-airflow-providers-apache-impala-1.1.2rc2/airflow/providers/apache/impala/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-impala-1.1.2rc2/airflow/providers/apache/impala/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-impala-1.1.2rc2/airflow/providers/apache/impala/hooks/impala.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:13.805664 apache-airflow-providers-apache-impala-1.1.2rc2/apache_airflow_providers_apache_impala.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5579 2023-07-06 04:50:13.000000 apache-airflow-providers-apache-impala-1.1.2rc2/apache_airflow_providers_apache_impala.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      701 2023-07-06 04:50:13.000000 apache-airflow-providers-apache-impala-1.1.2rc2/apache_airflow_providers_apache_impala.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:13.000000 apache-airflow-providers-apache-impala-1.1.2rc2/apache_airflow_providers_apache_impala.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      110 2023-07-06 04:50:13.000000 apache-airflow-providers-apache-impala-1.1.2rc2/apache_airflow_providers_apache_impala.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:13.000000 apache-airflow-providers-apache-impala-1.1.2rc2/apache_airflow_providers_apache_impala.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      125 2023-07-06 04:50:13.000000 apache-airflow-providers-apache-impala-1.1.2rc2/apache_airflow_providers_apache_impala.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-06 04:50:13.000000 apache-airflow-providers-apache-impala-1.1.2rc2/apache_airflow_providers_apache_impala.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-apache-impala-1.1.2rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1995 2023-07-06 04:50:13.810962 apache-airflow-providers-apache-impala-1.1.2rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1801 2023-07-06 04:50:12.000000 apache-airflow-providers-apache-impala-1.1.2rc2/setup.py
```

### Comparing `apache-airflow-providers-apache-impala-1.1.2/LICENSE` & `apache-airflow-providers-apache-impala-1.1.2rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-impala-1.1.2/MANIFEST.in` & `apache-airflow-providers-apache-impala-1.1.2rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-impala-1.1.2/PKG-INFO` & `apache-airflow-providers-apache-impala-1.1.2rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-impala
-Version: 1.1.2
+Version: 1.1.2rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-impala package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-impala/1.1.2/
@@ -68,15 +68,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apache-impala``
 
-Release: ``1.1.2``
+Release: ``1.1.2rc2``
 
 
 `Apache Impala <https://impala.apache.org/>`__.
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-impala-1.1.2/README.rst` & `apache-airflow-providers-apache-impala-1.1.2rc2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apache-impala``
 
-Release: ``1.1.2``
+Release: ``1.1.2rc2``
 
 
 `Apache Impala <https://impala.apache.org/>`__.
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-impala-1.1.2/airflow/providers/apache/impala/__init__.py` & `apache-airflow-providers-apache-impala-1.1.2rc2/airflow/providers/apache/impala/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-impala-1.1.2/airflow/providers/apache/impala/get_provider_info.py` & `apache-airflow-providers-apache-impala-1.1.2rc2/airflow/providers/apache/impala/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-impala-1.1.2/airflow/providers/apache/impala/hooks/__init__.py` & `apache-airflow-providers-apache-impala-1.1.2rc2/airflow/providers/apache/impala/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-impala-1.1.2/airflow/providers/apache/impala/hooks/impala.py` & `apache-airflow-providers-apache-impala-1.1.2rc2/airflow/providers/apache/impala/hooks/impala.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-impala-1.1.2/apache_airflow_providers_apache_impala.egg-info/PKG-INFO` & `apache-airflow-providers-apache-impala-1.1.2rc2/apache_airflow_providers_apache_impala.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-impala
-Version: 1.1.2
+Version: 1.1.2rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-impala package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-impala/1.1.2/
@@ -68,15 +68,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apache-impala``
 
-Release: ``1.1.2``
+Release: ``1.1.2rc2``
 
 
 `Apache Impala <https://impala.apache.org/>`__.
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-impala-1.1.2/apache_airflow_providers_apache_impala.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-impala-1.1.2rc2/apache_airflow_providers_apache_impala.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-impala-1.1.2/pyproject.toml` & `apache-airflow-providers-apache-impala-1.1.2rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-impala-1.1.2/setup.cfg` & `apache-airflow-providers-apache-impala-1.1.2rc2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -43,21 +43,21 @@
 include_package_data = True
 python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
-	apache-airflow>=2.4.0
+	apache-airflow>=2.4.0.dev0
 	impyla>=0.18.0,<1.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.apache.impala.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.apache.impala
 
 [egg_info]
-tag_build = 
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-apache-impala-1.1.2/setup.py` & `apache-airflow-providers-apache-impala-1.1.2rc2/setup.py`

 * *Files identical despite different names*

