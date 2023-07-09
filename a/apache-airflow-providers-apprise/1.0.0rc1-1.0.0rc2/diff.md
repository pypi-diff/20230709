# Comparing `tmp/apache-airflow-providers-apprise-1.0.0rc1.tar.gz` & `tmp/apache-airflow-providers-apprise-1.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-apprise-1.0.0rc1.tar", last modified: Wed Jul  5 07:29:46 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apprise-1.0.0rc2.tar", last modified: Thu Jul  6 04:50:24 2023, max compression
```

## Comparing `apache-airflow-providers-apprise-1.0.0rc1.tar` & `apache-airflow-providers-apprise-1.0.0rc2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:46.362268 apache-airflow-providers-apprise-1.0.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apprise-1.0.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-05 07:29:45.000000 apache-airflow-providers-apprise-1.0.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apprise-1.0.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4402 2023-07-05 07:29:46.362969 apache-airflow-providers-apprise-1.0.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2760 2023-07-05 07:29:45.000000 apache-airflow-providers-apprise-1.0.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:46.279516 apache-airflow-providers-apprise-1.0.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:46.280791 apache-airflow-providers-apprise-1.0.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:46.318072 apache-airflow-providers-apprise-1.0.0rc1/airflow/providers/apprise/
--rw-r--r--   0 root         (0) root         (0)     1532 2023-07-01 07:31:12.000000 apache-airflow-providers-apprise-1.0.0rc1/airflow/providers/apprise/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2010 2023-07-05 07:29:45.000000 apache-airflow-providers-apprise-1.0.0rc1/airflow/providers/apprise/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:46.324751 apache-airflow-providers-apprise-1.0.0rc1/airflow/providers/apprise/hooks/
--rw-r--r--   0 root         (0) root         (0)     1053 2023-06-24 10:23:12.000000 apache-airflow-providers-apprise-1.0.0rc1/airflow/providers/apprise/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5224 2023-06-29 05:49:30.000000 apache-airflow-providers-apprise-1.0.0rc1/airflow/providers/apprise/hooks/apprise.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:46.330608 apache-airflow-providers-apprise-1.0.0rc1/airflow/providers/apprise/notifications/
--rw-r--r--   0 root         (0) root         (0)     1053 2023-06-24 10:23:12.000000 apache-airflow-providers-apprise-1.0.0rc1/airflow/providers/apprise/notifications/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3714 2023-06-24 10:23:12.000000 apache-airflow-providers-apprise-1.0.0rc1/airflow/providers/apprise/notifications/apprise.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:46.353873 apache-airflow-providers-apprise-1.0.0rc1/apache_airflow_providers_apprise.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4402 2023-07-05 07:29:46.000000 apache-airflow-providers-apprise-1.0.0rc1/apache_airflow_providers_apprise.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      739 2023-07-05 07:29:46.000000 apache-airflow-providers-apprise-1.0.0rc1/apache_airflow_providers_apprise.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:29:46.000000 apache-airflow-providers-apprise-1.0.0rc1/apache_airflow_providers_apprise.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-07-05 07:29:46.000000 apache-airflow-providers-apprise-1.0.0rc1/apache_airflow_providers_apprise.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:29:46.000000 apache-airflow-providers-apprise-1.0.0rc1/apache_airflow_providers_apprise.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       35 2023-07-05 07:29:46.000000 apache-airflow-providers-apprise-1.0.0rc1/apache_airflow_providers_apprise.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-05 07:29:46.000000 apache-airflow-providers-apprise-1.0.0rc1/apache_airflow_providers_apprise.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-apprise-1.0.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1941 2023-07-05 07:29:46.365420 apache-airflow-providers-apprise-1.0.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1644 2023-07-05 07:29:45.000000 apache-airflow-providers-apprise-1.0.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:24.258325 apache-airflow-providers-apprise-1.0.0rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apprise-1.0.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-06 04:50:23.000000 apache-airflow-providers-apprise-1.0.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apprise-1.0.0rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4402 2023-07-06 04:50:24.258938 apache-airflow-providers-apprise-1.0.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2760 2023-07-06 04:50:23.000000 apache-airflow-providers-apprise-1.0.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:24.180173 apache-airflow-providers-apprise-1.0.0rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:24.181246 apache-airflow-providers-apprise-1.0.0rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:24.214239 apache-airflow-providers-apprise-1.0.0rc2/airflow/providers/apprise/
+-rw-r--r--   0 root         (0) root         (0)     1532 2023-07-05 18:47:43.000000 apache-airflow-providers-apprise-1.0.0rc2/airflow/providers/apprise/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2010 2023-07-06 04:50:23.000000 apache-airflow-providers-apprise-1.0.0rc2/airflow/providers/apprise/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:24.220052 apache-airflow-providers-apprise-1.0.0rc2/airflow/providers/apprise/hooks/
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-06-24 10:23:12.000000 apache-airflow-providers-apprise-1.0.0rc2/airflow/providers/apprise/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5224 2023-06-29 05:49:30.000000 apache-airflow-providers-apprise-1.0.0rc2/airflow/providers/apprise/hooks/apprise.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:24.225678 apache-airflow-providers-apprise-1.0.0rc2/airflow/providers/apprise/notifications/
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-06-24 10:23:12.000000 apache-airflow-providers-apprise-1.0.0rc2/airflow/providers/apprise/notifications/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3714 2023-06-24 10:23:12.000000 apache-airflow-providers-apprise-1.0.0rc2/airflow/providers/apprise/notifications/apprise.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:24.255907 apache-airflow-providers-apprise-1.0.0rc2/apache_airflow_providers_apprise.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4402 2023-07-06 04:50:24.000000 apache-airflow-providers-apprise-1.0.0rc2/apache_airflow_providers_apprise.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      739 2023-07-06 04:50:24.000000 apache-airflow-providers-apprise-1.0.0rc2/apache_airflow_providers_apprise.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:24.000000 apache-airflow-providers-apprise-1.0.0rc2/apache_airflow_providers_apprise.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-07-06 04:50:24.000000 apache-airflow-providers-apprise-1.0.0rc2/apache_airflow_providers_apprise.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:24.000000 apache-airflow-providers-apprise-1.0.0rc2/apache_airflow_providers_apprise.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       35 2023-07-06 04:50:24.000000 apache-airflow-providers-apprise-1.0.0rc2/apache_airflow_providers_apprise.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-06 04:50:24.000000 apache-airflow-providers-apprise-1.0.0rc2/apache_airflow_providers_apprise.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-apprise-1.0.0rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1941 2023-07-06 04:50:24.260830 apache-airflow-providers-apprise-1.0.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-07-06 04:50:23.000000 apache-airflow-providers-apprise-1.0.0rc2/setup.py
```

### Comparing `apache-airflow-providers-apprise-1.0.0rc1/LICENSE` & `apache-airflow-providers-apprise-1.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apprise-1.0.0rc1/MANIFEST.in` & `apache-airflow-providers-apprise-1.0.0rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apprise-1.0.0rc1/PKG-INFO` & `apache-airflow-providers-apprise-1.0.0rc2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apprise
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apprise package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apprise/1.0.0/
@@ -66,15 +66,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apprise``
 
-Release: ``1.0.0rc1``
+Release: ``1.0.0rc2``
 
 
 `Apprise <https://github.com/caronc/apprise>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apprise-1.0.0rc1/README.rst` & `apache-airflow-providers-apprise-1.0.0rc2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apprise``
 
-Release: ``1.0.0rc1``
+Release: ``1.0.0rc2``
 
 
 `Apprise <https://github.com/caronc/apprise>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apprise-1.0.0rc1/airflow/providers/apprise/__init__.py` & `apache-airflow-providers-apprise-1.0.0rc2/airflow/providers/apprise/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apprise-1.0.0rc1/airflow/providers/apprise/get_provider_info.py` & `apache-airflow-providers-apprise-1.0.0rc2/airflow/providers/apprise/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apprise-1.0.0rc1/airflow/providers/apprise/hooks/__init__.py` & `apache-airflow-providers-apprise-1.0.0rc2/airflow/providers/apprise/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apprise-1.0.0rc1/airflow/providers/apprise/hooks/apprise.py` & `apache-airflow-providers-apprise-1.0.0rc2/airflow/providers/apprise/hooks/apprise.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apprise-1.0.0rc1/airflow/providers/apprise/notifications/__init__.py` & `apache-airflow-providers-apprise-1.0.0rc2/airflow/providers/apprise/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apprise-1.0.0rc1/airflow/providers/apprise/notifications/apprise.py` & `apache-airflow-providers-apprise-1.0.0rc2/airflow/providers/apprise/notifications/apprise.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apprise-1.0.0rc1/apache_airflow_providers_apprise.egg-info/PKG-INFO` & `apache-airflow-providers-apprise-1.0.0rc2/apache_airflow_providers_apprise.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apprise
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apprise package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apprise/1.0.0/
@@ -66,15 +66,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apprise``
 
-Release: ``1.0.0rc1``
+Release: ``1.0.0rc2``
 
 
 `Apprise <https://github.com/caronc/apprise>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apprise-1.0.0rc1/apache_airflow_providers_apprise.egg-info/SOURCES.txt` & `apache-airflow-providers-apprise-1.0.0rc2/apache_airflow_providers_apprise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apprise-1.0.0rc1/pyproject.toml` & `apache-airflow-providers-apprise-1.0.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apprise-1.0.0rc1/setup.cfg` & `apache-airflow-providers-apprise-1.0.0rc2/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -54,10 +54,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.apprise.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.apprise
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-apprise-1.0.0rc1/setup.py` & `apache-airflow-providers-apprise-1.0.0rc2/setup.py`

 * *Files identical despite different names*

