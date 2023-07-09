# Comparing `tmp/apache-airflow-providers-vertica-3.5.0rc1.tar.gz` & `tmp/apache-airflow-providers-vertica-3.5.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-vertica-3.5.0rc1.tar", last modified: Wed Jul  5 07:30:35 2023, max compression
+gzip compressed data, was "apache-airflow-providers-vertica-3.5.0rc2.tar", last modified: Thu Jul  6 04:51:42 2023, max compression
```

## Comparing `apache-airflow-providers-vertica-3.5.0rc1.tar` & `apache-airflow-providers-vertica-3.5.0rc2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:35.940806 apache-airflow-providers-vertica-3.5.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-vertica-3.5.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-05 07:30:34.000000 apache-airflow-providers-vertica-3.5.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-vertica-3.5.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5652 2023-07-05 07:30:35.941670 apache-airflow-providers-vertica-3.5.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3983 2023-07-05 07:30:34.000000 apache-airflow-providers-vertica-3.5.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:35.854082 apache-airflow-providers-vertica-3.5.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:35.855783 apache-airflow-providers-vertica-3.5.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:35.894887 apache-airflow-providers-vertica-3.5.0rc1/airflow/providers/vertica/
--rw-r--r--   0 root         (0) root         (0)     1532 2023-07-05 07:19:39.000000 apache-airflow-providers-vertica-3.5.0rc1/airflow/providers/vertica/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2575 2023-07-05 07:30:34.000000 apache-airflow-providers-vertica-3.5.0rc1/airflow/providers/vertica/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:35.901863 apache-airflow-providers-vertica-3.5.0rc1/airflow/providers/vertica/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-vertica-3.5.0rc1/airflow/providers/vertica/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3531 2023-06-30 08:49:17.000000 apache-airflow-providers-vertica-3.5.0rc1/airflow/providers/vertica/hooks/vertica.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:35.908735 apache-airflow-providers-vertica-3.5.0rc1/airflow/providers/vertica/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-vertica-3.5.0rc1/airflow/providers/vertica/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1976 2023-06-01 06:14:29.000000 apache-airflow-providers-vertica-3.5.0rc1/airflow/providers/vertica/operators/vertica.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:35.937335 apache-airflow-providers-vertica-3.5.0rc1/apache_airflow_providers_vertica.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5652 2023-07-05 07:30:35.000000 apache-airflow-providers-vertica-3.5.0rc1/apache_airflow_providers_vertica.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      731 2023-07-05 07:30:35.000000 apache-airflow-providers-vertica-3.5.0rc1/apache_airflow_providers_vertica.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:30:35.000000 apache-airflow-providers-vertica-3.5.0rc1/apache_airflow_providers_vertica.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-07-05 07:30:35.000000 apache-airflow-providers-vertica-3.5.0rc1/apache_airflow_providers_vertica.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:30:35.000000 apache-airflow-providers-vertica-3.5.0rc1/apache_airflow_providers_vertica.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      147 2023-07-05 07:30:35.000000 apache-airflow-providers-vertica-3.5.0rc1/apache_airflow_providers_vertica.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-05 07:30:35.000000 apache-airflow-providers-vertica-3.5.0rc1/apache_airflow_providers_vertica.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-vertica-3.5.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2004 2023-07-05 07:30:35.944513 apache-airflow-providers-vertica-3.5.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1697 2023-07-05 07:30:34.000000 apache-airflow-providers-vertica-3.5.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:42.145072 apache-airflow-providers-vertica-3.5.0rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-vertica-3.5.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-06 04:51:41.000000 apache-airflow-providers-vertica-3.5.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-vertica-3.5.0rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5652 2023-07-06 04:51:42.145674 apache-airflow-providers-vertica-3.5.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3983 2023-07-06 04:51:41.000000 apache-airflow-providers-vertica-3.5.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:42.050680 apache-airflow-providers-vertica-3.5.0rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:42.051774 apache-airflow-providers-vertica-3.5.0rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:42.093776 apache-airflow-providers-vertica-3.5.0rc2/airflow/providers/vertica/
+-rw-r--r--   0 root         (0) root         (0)     1532 2023-07-05 18:55:54.000000 apache-airflow-providers-vertica-3.5.0rc2/airflow/providers/vertica/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2575 2023-07-06 04:51:41.000000 apache-airflow-providers-vertica-3.5.0rc2/airflow/providers/vertica/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:42.100975 apache-airflow-providers-vertica-3.5.0rc2/airflow/providers/vertica/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-vertica-3.5.0rc2/airflow/providers/vertica/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3531 2023-06-30 08:49:17.000000 apache-airflow-providers-vertica-3.5.0rc2/airflow/providers/vertica/hooks/vertica.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:42.110548 apache-airflow-providers-vertica-3.5.0rc2/airflow/providers/vertica/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-vertica-3.5.0rc2/airflow/providers/vertica/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1976 2023-06-01 06:14:29.000000 apache-airflow-providers-vertica-3.5.0rc2/airflow/providers/vertica/operators/vertica.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:42.142277 apache-airflow-providers-vertica-3.5.0rc2/apache_airflow_providers_vertica.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5652 2023-07-06 04:51:41.000000 apache-airflow-providers-vertica-3.5.0rc2/apache_airflow_providers_vertica.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      731 2023-07-06 04:51:42.000000 apache-airflow-providers-vertica-3.5.0rc2/apache_airflow_providers_vertica.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:51:41.000000 apache-airflow-providers-vertica-3.5.0rc2/apache_airflow_providers_vertica.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-07-06 04:51:41.000000 apache-airflow-providers-vertica-3.5.0rc2/apache_airflow_providers_vertica.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:51:41.000000 apache-airflow-providers-vertica-3.5.0rc2/apache_airflow_providers_vertica.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      147 2023-07-06 04:51:41.000000 apache-airflow-providers-vertica-3.5.0rc2/apache_airflow_providers_vertica.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-06 04:51:41.000000 apache-airflow-providers-vertica-3.5.0rc2/apache_airflow_providers_vertica.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-vertica-3.5.0rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2004 2023-07-06 04:51:42.147547 apache-airflow-providers-vertica-3.5.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1697 2023-07-06 04:51:41.000000 apache-airflow-providers-vertica-3.5.0rc2/setup.py
```

### Comparing `apache-airflow-providers-vertica-3.5.0rc1/LICENSE` & `apache-airflow-providers-vertica-3.5.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-vertica-3.5.0rc1/MANIFEST.in` & `apache-airflow-providers-vertica-3.5.0rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-vertica-3.5.0rc1/PKG-INFO` & `apache-airflow-providers-vertica-3.5.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-vertica
-Version: 3.5.0rc1
+Version: 3.5.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-vertica package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-vertica/3.5.0/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-vertica``
 
-Release: ``3.5.0rc1``
+Release: ``3.5.0rc2``
 
 
 `Vertica <https://www.vertica.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-vertica-3.5.0rc1/README.rst` & `apache-airflow-providers-vertica-3.5.0rc2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-vertica``
 
-Release: ``3.5.0rc1``
+Release: ``3.5.0rc2``
 
 
 `Vertica <https://www.vertica.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-vertica-3.5.0rc1/airflow/providers/vertica/__init__.py` & `apache-airflow-providers-vertica-3.5.0rc2/airflow/providers/vertica/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-vertica-3.5.0rc1/airflow/providers/vertica/get_provider_info.py` & `apache-airflow-providers-vertica-3.5.0rc2/airflow/providers/vertica/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-vertica-3.5.0rc1/airflow/providers/vertica/hooks/__init__.py` & `apache-airflow-providers-vertica-3.5.0rc2/airflow/providers/vertica/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-vertica-3.5.0rc1/airflow/providers/vertica/hooks/vertica.py` & `apache-airflow-providers-vertica-3.5.0rc2/airflow/providers/vertica/hooks/vertica.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-vertica-3.5.0rc1/airflow/providers/vertica/operators/__init__.py` & `apache-airflow-providers-vertica-3.5.0rc2/airflow/providers/vertica/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-vertica-3.5.0rc1/airflow/providers/vertica/operators/vertica.py` & `apache-airflow-providers-vertica-3.5.0rc2/airflow/providers/vertica/operators/vertica.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-vertica-3.5.0rc1/apache_airflow_providers_vertica.egg-info/PKG-INFO` & `apache-airflow-providers-vertica-3.5.0rc2/apache_airflow_providers_vertica.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-vertica
-Version: 3.5.0rc1
+Version: 3.5.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-vertica package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-vertica/3.5.0/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-vertica``
 
-Release: ``3.5.0rc1``
+Release: ``3.5.0rc2``
 
 
 `Vertica <https://www.vertica.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-vertica-3.5.0rc1/apache_airflow_providers_vertica.egg-info/SOURCES.txt` & `apache-airflow-providers-vertica-3.5.0rc2/apache_airflow_providers_vertica.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-vertica-3.5.0rc1/pyproject.toml` & `apache-airflow-providers-vertica-3.5.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-vertica-3.5.0rc1/setup.cfg` & `apache-airflow-providers-vertica-3.5.0rc2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -55,10 +55,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.vertica.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.vertica
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-vertica-3.5.0rc1/setup.py` & `apache-airflow-providers-vertica-3.5.0rc2/setup.py`

 * *Files identical despite different names*

