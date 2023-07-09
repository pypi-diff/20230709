# Comparing `tmp/apache-airflow-providers-hashicorp-3.4.2rc1.tar.gz` & `tmp/apache-airflow-providers-hashicorp-3.4.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-hashicorp-3.4.2rc1.tar", last modified: Wed Jul  5 07:30:12 2023, max compression
+gzip compressed data, was "apache-airflow-providers-hashicorp-3.4.2rc2.tar", last modified: Thu Jul  6 04:50:57 2023, max compression
```

## Comparing `apache-airflow-providers-hashicorp-3.4.2rc1.tar` & `apache-airflow-providers-hashicorp-3.4.2rc2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:12.040607 apache-airflow-providers-hashicorp-3.4.2rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-hashicorp-3.4.2rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-05 07:30:10.000000 apache-airflow-providers-hashicorp-3.4.2rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-hashicorp-3.4.2rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5462 2023-07-05 07:30:12.041425 apache-airflow-providers-hashicorp-3.4.2rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3789 2023-07-05 07:30:10.000000 apache-airflow-providers-hashicorp-3.4.2rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:11.912613 apache-airflow-providers-hashicorp-3.4.2rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:11.915791 apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:11.968515 apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/
--rw-r--r--   0 root         (0) root         (0)     1534 2023-07-05 07:19:39.000000 apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:11.978383 apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/_internal_client/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/_internal_client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21223 2023-07-05 07:19:39.000000 apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/_internal_client/vault_client.py
--rw-r--r--   0 root         (0) root         (0)     2565 2023-07-05 07:30:10.000000 apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:11.988449 apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18752 2023-06-02 11:31:21.000000 apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/hooks/vault.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:11.998308 apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/secrets/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11992 2023-07-05 07:19:39.000000 apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/secrets/vault.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:30:12.035782 apache-airflow-providers-hashicorp-3.4.2rc1/apache_airflow_providers_hashicorp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5462 2023-07-05 07:30:11.000000 apache-airflow-providers-hashicorp-3.4.2rc1/apache_airflow_providers_hashicorp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      867 2023-07-05 07:30:11.000000 apache-airflow-providers-hashicorp-3.4.2rc1/apache_airflow_providers_hashicorp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:30:11.000000 apache-airflow-providers-hashicorp-3.4.2rc1/apache_airflow_providers_hashicorp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-07-05 07:30:11.000000 apache-airflow-providers-hashicorp-3.4.2rc1/apache_airflow_providers_hashicorp.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:30:11.000000 apache-airflow-providers-hashicorp-3.4.2rc1/apache_airflow_providers_hashicorp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       80 2023-07-05 07:30:11.000000 apache-airflow-providers-hashicorp-3.4.2rc1/apache_airflow_providers_hashicorp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-05 07:30:11.000000 apache-airflow-providers-hashicorp-3.4.2rc1/apache_airflow_providers_hashicorp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-hashicorp-3.4.2rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1958 2023-07-05 07:30:12.043814 apache-airflow-providers-hashicorp-3.4.2rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1701 2023-07-05 07:30:10.000000 apache-airflow-providers-hashicorp-3.4.2rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:57.637310 apache-airflow-providers-hashicorp-3.4.2rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-hashicorp-3.4.2rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-06 04:50:56.000000 apache-airflow-providers-hashicorp-3.4.2rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-hashicorp-3.4.2rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5462 2023-07-06 04:50:57.637919 apache-airflow-providers-hashicorp-3.4.2rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3789 2023-07-06 04:50:56.000000 apache-airflow-providers-hashicorp-3.4.2rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:57.557078 apache-airflow-providers-hashicorp-3.4.2rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:57.558238 apache-airflow-providers-hashicorp-3.4.2rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:57.591869 apache-airflow-providers-hashicorp-3.4.2rc2/airflow/providers/hashicorp/
+-rw-r--r--   0 root         (0) root         (0)     1534 2023-07-05 18:51:41.000000 apache-airflow-providers-hashicorp-3.4.2rc2/airflow/providers/hashicorp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:57.597701 apache-airflow-providers-hashicorp-3.4.2rc2/airflow/providers/hashicorp/_internal_client/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-hashicorp-3.4.2rc2/airflow/providers/hashicorp/_internal_client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21223 2023-07-05 07:19:39.000000 apache-airflow-providers-hashicorp-3.4.2rc2/airflow/providers/hashicorp/_internal_client/vault_client.py
+-rw-r--r--   0 root         (0) root         (0)     2565 2023-07-06 04:50:56.000000 apache-airflow-providers-hashicorp-3.4.2rc2/airflow/providers/hashicorp/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:57.603591 apache-airflow-providers-hashicorp-3.4.2rc2/airflow/providers/hashicorp/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-hashicorp-3.4.2rc2/airflow/providers/hashicorp/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18752 2023-06-02 11:31:21.000000 apache-airflow-providers-hashicorp-3.4.2rc2/airflow/providers/hashicorp/hooks/vault.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:57.610006 apache-airflow-providers-hashicorp-3.4.2rc2/airflow/providers/hashicorp/secrets/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-hashicorp-3.4.2rc2/airflow/providers/hashicorp/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11992 2023-07-05 07:19:39.000000 apache-airflow-providers-hashicorp-3.4.2rc2/airflow/providers/hashicorp/secrets/vault.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:57.634168 apache-airflow-providers-hashicorp-3.4.2rc2/apache_airflow_providers_hashicorp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5462 2023-07-06 04:50:57.000000 apache-airflow-providers-hashicorp-3.4.2rc2/apache_airflow_providers_hashicorp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      867 2023-07-06 04:50:57.000000 apache-airflow-providers-hashicorp-3.4.2rc2/apache_airflow_providers_hashicorp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:57.000000 apache-airflow-providers-hashicorp-3.4.2rc2/apache_airflow_providers_hashicorp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-07-06 04:50:57.000000 apache-airflow-providers-hashicorp-3.4.2rc2/apache_airflow_providers_hashicorp.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:57.000000 apache-airflow-providers-hashicorp-3.4.2rc2/apache_airflow_providers_hashicorp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       80 2023-07-06 04:50:57.000000 apache-airflow-providers-hashicorp-3.4.2rc2/apache_airflow_providers_hashicorp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-06 04:50:57.000000 apache-airflow-providers-hashicorp-3.4.2rc2/apache_airflow_providers_hashicorp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-hashicorp-3.4.2rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1958 2023-07-06 04:50:57.639776 apache-airflow-providers-hashicorp-3.4.2rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-07-06 04:50:56.000000 apache-airflow-providers-hashicorp-3.4.2rc2/setup.py
```

### Comparing `apache-airflow-providers-hashicorp-3.4.2rc1/LICENSE` & `apache-airflow-providers-hashicorp-3.4.2rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-hashicorp-3.4.2rc1/MANIFEST.in` & `apache-airflow-providers-hashicorp-3.4.2rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-hashicorp-3.4.2rc1/PKG-INFO` & `apache-airflow-providers-hashicorp-3.4.2rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-hashicorp
-Version: 3.4.2rc1
+Version: 3.4.2rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-hashicorp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-hashicorp/3.4.2/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-hashicorp``
 
-Release: ``3.4.2rc1``
+Release: ``3.4.2rc2``
 
 
 Hashicorp including `Hashicorp Vault <https://www.vaultproject.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-hashicorp-3.4.2rc1/README.rst` & `apache-airflow-providers-hashicorp-3.4.2rc2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-hashicorp``
 
-Release: ``3.4.2rc1``
+Release: ``3.4.2rc2``
 
 
 Hashicorp including `Hashicorp Vault <https://www.vaultproject.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/__init__.py` & `apache-airflow-providers-hashicorp-3.4.2rc2/airflow/providers/hashicorp/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/_internal_client/__init__.py` & `apache-airflow-providers-hashicorp-3.4.2rc2/airflow/providers/hashicorp/_internal_client/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/_internal_client/vault_client.py` & `apache-airflow-providers-hashicorp-3.4.2rc2/airflow/providers/hashicorp/_internal_client/vault_client.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/get_provider_info.py` & `apache-airflow-providers-hashicorp-3.4.2rc2/airflow/providers/hashicorp/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/hooks/__init__.py` & `apache-airflow-providers-hashicorp-3.4.2rc2/airflow/providers/hashicorp/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/hooks/vault.py` & `apache-airflow-providers-hashicorp-3.4.2rc2/airflow/providers/hashicorp/hooks/vault.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/secrets/__init__.py` & `apache-airflow-providers-hashicorp-3.4.2rc2/airflow/providers/hashicorp/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-hashicorp-3.4.2rc1/airflow/providers/hashicorp/secrets/vault.py` & `apache-airflow-providers-hashicorp-3.4.2rc2/airflow/providers/hashicorp/secrets/vault.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-hashicorp-3.4.2rc1/apache_airflow_providers_hashicorp.egg-info/PKG-INFO` & `apache-airflow-providers-hashicorp-3.4.2rc2/apache_airflow_providers_hashicorp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-hashicorp
-Version: 3.4.2rc1
+Version: 3.4.2rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-hashicorp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-hashicorp/3.4.2/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-hashicorp``
 
-Release: ``3.4.2rc1``
+Release: ``3.4.2rc2``
 
 
 Hashicorp including `Hashicorp Vault <https://www.vaultproject.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-hashicorp-3.4.2rc1/apache_airflow_providers_hashicorp.egg-info/SOURCES.txt` & `apache-airflow-providers-hashicorp-3.4.2rc2/apache_airflow_providers_hashicorp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-hashicorp-3.4.2rc1/pyproject.toml` & `apache-airflow-providers-hashicorp-3.4.2rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-hashicorp-3.4.2rc1/setup.cfg` & `apache-airflow-providers-hashicorp-3.4.2rc2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -54,10 +54,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.hashicorp.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.hashicorp
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-hashicorp-3.4.2rc1/setup.py` & `apache-airflow-providers-hashicorp-3.4.2rc2/setup.py`

 * *Files identical despite different names*

