# Comparing `tmp/apache-airflow-providers-postgres-5.5.2.tar.gz` & `tmp/apache-airflow-providers-postgres-5.5.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-postgres-5.5.2.tar", last modified: Thu Jul  6 04:45:06 2023, max compression
+gzip compressed data, was "apache-airflow-providers-postgres-5.5.2rc2.tar", last modified: Thu Jul  6 04:51:20 2023, max compression
```

## Comparing `apache-airflow-providers-postgres-5.5.2.tar` & `apache-airflow-providers-postgres-5.5.2rc2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:45:06.376174 apache-airflow-providers-postgres-5.5.2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-postgres-5.5.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-06 04:45:05.000000 apache-airflow-providers-postgres-5.5.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-postgres-5.5.2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5803 2023-07-06 04:45:06.376752 apache-airflow-providers-postgres-5.5.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4110 2023-07-06 04:45:05.000000 apache-airflow-providers-postgres-5.5.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:45:06.302208 apache-airflow-providers-postgres-5.5.2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:45:06.303320 apache-airflow-providers-postgres-5.5.2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:45:06.336268 apache-airflow-providers-postgres-5.5.2/airflow/providers/postgres/
--rw-r--r--   0 root         (0) root         (0)     1533 2023-07-06 04:42:33.000000 apache-airflow-providers-postgres-5.5.2/airflow/providers/postgres/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3098 2023-07-06 04:45:05.000000 apache-airflow-providers-postgres-5.5.2/airflow/providers/postgres/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:45:06.342701 apache-airflow-providers-postgres-5.5.2/airflow/providers/postgres/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-postgres-5.5.2/airflow/providers/postgres/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13342 2023-07-05 07:19:39.000000 apache-airflow-providers-postgres-5.5.2/airflow/providers/postgres/hooks/postgres.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:45:06.348761 apache-airflow-providers-postgres-5.5.2/airflow/providers/postgres/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-postgres-5.5.2/airflow/providers/postgres/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3467 2023-07-05 07:19:39.000000 apache-airflow-providers-postgres-5.5.2/airflow/providers/postgres/operators/postgres.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:45:06.373548 apache-airflow-providers-postgres-5.5.2/apache_airflow_providers_postgres.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5803 2023-07-06 04:45:06.000000 apache-airflow-providers-postgres-5.5.2/apache_airflow_providers_postgres.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-07-06 04:45:06.000000 apache-airflow-providers-postgres-5.5.2/apache_airflow_providers_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:45:06.000000 apache-airflow-providers-postgres-5.5.2/apache_airflow_providers_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-07-06 04:45:06.000000 apache-airflow-providers-postgres-5.5.2/apache_airflow_providers_postgres.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:45:06.000000 apache-airflow-providers-postgres-5.5.2/apache_airflow_providers_postgres.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      187 2023-07-06 04:45:06.000000 apache-airflow-providers-postgres-5.5.2/apache_airflow_providers_postgres.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-06 04:45:06.000000 apache-airflow-providers-postgres-5.5.2/apache_airflow_providers_postgres.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-postgres-5.5.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1999 2023-07-06 04:45:06.378708 apache-airflow-providers-postgres-5.5.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1792 2023-07-06 04:45:05.000000 apache-airflow-providers-postgres-5.5.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:20.382146 apache-airflow-providers-postgres-5.5.2rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-postgres-5.5.2rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-06 04:51:19.000000 apache-airflow-providers-postgres-5.5.2rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-postgres-5.5.2rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5809 2023-07-06 04:51:20.382738 apache-airflow-providers-postgres-5.5.2rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4113 2023-07-06 04:51:19.000000 apache-airflow-providers-postgres-5.5.2rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:20.304592 apache-airflow-providers-postgres-5.5.2rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:20.305843 apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:20.340819 apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-07-06 04:42:33.000000 apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3098 2023-07-06 04:51:19.000000 apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:20.347351 apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13342 2023-07-05 07:19:39.000000 apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/hooks/postgres.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:20.353272 apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3467 2023-07-05 07:19:39.000000 apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/operators/postgres.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:20.379739 apache-airflow-providers-postgres-5.5.2rc2/apache_airflow_providers_postgres.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5809 2023-07-06 04:51:20.000000 apache-airflow-providers-postgres-5.5.2rc2/apache_airflow_providers_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-06 04:51:20.000000 apache-airflow-providers-postgres-5.5.2rc2/apache_airflow_providers_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:51:20.000000 apache-airflow-providers-postgres-5.5.2rc2/apache_airflow_providers_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-07-06 04:51:20.000000 apache-airflow-providers-postgres-5.5.2rc2/apache_airflow_providers_postgres.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:51:20.000000 apache-airflow-providers-postgres-5.5.2rc2/apache_airflow_providers_postgres.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      197 2023-07-06 04:51:20.000000 apache-airflow-providers-postgres-5.5.2rc2/apache_airflow_providers_postgres.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-06 04:51:20.000000 apache-airflow-providers-postgres-5.5.2rc2/apache_airflow_providers_postgres.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-postgres-5.5.2rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2012 2023-07-06 04:51:20.384790 apache-airflow-providers-postgres-5.5.2rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1792 2023-07-06 04:51:19.000000 apache-airflow-providers-postgres-5.5.2rc2/setup.py
```

### Comparing `apache-airflow-providers-postgres-5.5.2/LICENSE` & `apache-airflow-providers-postgres-5.5.2rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.5.2/MANIFEST.in` & `apache-airflow-providers-postgres-5.5.2rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.5.2/PKG-INFO` & `apache-airflow-providers-postgres-5.5.2rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-postgres
-Version: 5.5.2
+Version: 5.5.2rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-postgres package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.5.2/
@@ -68,15 +68,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-postgres``
 
-Release: ``5.5.2``
+Release: ``5.5.2rc2``
 
 
 `PostgreSQL <https://www.postgresql.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-postgres-5.5.2/README.rst` & `apache-airflow-providers-postgres-5.5.2rc2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-postgres``
 
-Release: ``5.5.2``
+Release: ``5.5.2rc2``
 
 
 `PostgreSQL <https://www.postgresql.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-postgres-5.5.2/airflow/providers/postgres/__init__.py` & `apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.5.2/airflow/providers/postgres/get_provider_info.py` & `apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.5.2/airflow/providers/postgres/hooks/__init__.py` & `apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.5.2/airflow/providers/postgres/hooks/postgres.py` & `apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/hooks/postgres.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.5.2/airflow/providers/postgres/operators/__init__.py` & `apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.5.2/airflow/providers/postgres/operators/postgres.py` & `apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/operators/postgres.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.5.2/apache_airflow_providers_postgres.egg-info/PKG-INFO` & `apache-airflow-providers-postgres-5.5.2rc2/apache_airflow_providers_postgres.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-postgres
-Version: 5.5.2
+Version: 5.5.2rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-postgres package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.5.2/
@@ -68,15 +68,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-postgres``
 
-Release: ``5.5.2``
+Release: ``5.5.2rc2``
 
 
 `PostgreSQL <https://www.postgresql.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-postgres-5.5.2/apache_airflow_providers_postgres.egg-info/SOURCES.txt` & `apache-airflow-providers-postgres-5.5.2rc2/apache_airflow_providers_postgres.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.5.2/pyproject.toml` & `apache-airflow-providers-postgres-5.5.2rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.5.2/setup.cfg` & `apache-airflow-providers-postgres-5.5.2rc2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -43,22 +43,22 @@
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
 	psycopg2-binary>=2.8.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.postgres.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.postgres
 
 [egg_info]
-tag_build = 
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-postgres-5.5.2/setup.py` & `apache-airflow-providers-postgres-5.5.2rc2/setup.py`

 * *Files identical despite different names*

