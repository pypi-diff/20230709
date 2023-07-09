# Comparing `tmp/apache-airflow-providers-common-sql-1.6.0rc1.tar.gz` & `tmp/apache-airflow-providers-common-sql-1.6.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-common-sql-1.6.0rc1.tar", last modified: Wed Jul  5 07:29:52 2023, max compression
+gzip compressed data, was "apache-airflow-providers-common-sql-1.6.0rc2.tar", last modified: Thu Jul  6 04:50:33 2023, max compression
```

## Comparing `apache-airflow-providers-common-sql-1.6.0rc1.tar` & `apache-airflow-providers-common-sql-1.6.0rc2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:52.932599 apache-airflow-providers-common-sql-1.6.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-common-sql-1.6.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-05 07:29:51.000000 apache-airflow-providers-common-sql-1.6.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-common-sql-1.6.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5566 2023-07-05 07:29:52.933230 apache-airflow-providers-common-sql-1.6.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3861 2023-07-05 07:29:51.000000 apache-airflow-providers-common-sql-1.6.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:52.846572 apache-airflow-providers-common-sql-1.6.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:52.847607 apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:52.848699 apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:52.885380 apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/
--rw-r--r--   0 root         (0) root         (0)     1535 2023-07-05 07:19:39.000000 apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2599 2023-07-05 07:29:51.000000 apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:52.891800 apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23794 2023-06-29 14:43:21.000000 apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/hooks/sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:52.898281 apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    46803 2023-06-29 14:43:21.000000 apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/operators/sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:52.904996 apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4726 2023-06-05 12:50:36.000000 apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/sensors/sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:52.929896 apache-airflow-providers-common-sql-1.6.0rc1/apache_airflow_providers_common_sql.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5566 2023-07-05 07:29:52.000000 apache-airflow-providers-common-sql-1.6.0rc1/apache_airflow_providers_common_sql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      855 2023-07-05 07:29:52.000000 apache-airflow-providers-common-sql-1.6.0rc1/apache_airflow_providers_common_sql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:29:52.000000 apache-airflow-providers-common-sql-1.6.0rc1/apache_airflow_providers_common_sql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-07-05 07:29:52.000000 apache-airflow-providers-common-sql-1.6.0rc1/apache_airflow_providers_common_sql.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:29:52.000000 apache-airflow-providers-common-sql-1.6.0rc1/apache_airflow_providers_common_sql.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      120 2023-07-05 07:29:52.000000 apache-airflow-providers-common-sql-1.6.0rc1/apache_airflow_providers_common_sql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-05 07:29:52.000000 apache-airflow-providers-common-sql-1.6.0rc1/apache_airflow_providers_common_sql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-common-sql-1.6.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1970 2023-07-05 07:29:52.935124 apache-airflow-providers-common-sql-1.6.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1782 2023-07-05 07:29:51.000000 apache-airflow-providers-common-sql-1.6.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:33.010937 apache-airflow-providers-common-sql-1.6.0rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-common-sql-1.6.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-06 04:50:31.000000 apache-airflow-providers-common-sql-1.6.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-common-sql-1.6.0rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5566 2023-07-06 04:50:33.011661 apache-airflow-providers-common-sql-1.6.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3861 2023-07-06 04:50:31.000000 apache-airflow-providers-common-sql-1.6.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:32.923094 apache-airflow-providers-common-sql-1.6.0rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:32.924264 apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:32.925494 apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:32.964214 apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-07-05 18:48:54.000000 apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2599 2023-07-06 04:50:31.000000 apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:32.970182 apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23801 2023-07-05 14:56:16.000000 apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/hooks/sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:32.976491 apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    46900 2023-07-05 14:56:16.000000 apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/operators/sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:32.982791 apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4726 2023-06-05 12:50:36.000000 apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/sensors/sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:33.008107 apache-airflow-providers-common-sql-1.6.0rc2/apache_airflow_providers_common_sql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5566 2023-07-06 04:50:32.000000 apache-airflow-providers-common-sql-1.6.0rc2/apache_airflow_providers_common_sql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      855 2023-07-06 04:50:32.000000 apache-airflow-providers-common-sql-1.6.0rc2/apache_airflow_providers_common_sql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:32.000000 apache-airflow-providers-common-sql-1.6.0rc2/apache_airflow_providers_common_sql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-07-06 04:50:32.000000 apache-airflow-providers-common-sql-1.6.0rc2/apache_airflow_providers_common_sql.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:32.000000 apache-airflow-providers-common-sql-1.6.0rc2/apache_airflow_providers_common_sql.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      120 2023-07-06 04:50:32.000000 apache-airflow-providers-common-sql-1.6.0rc2/apache_airflow_providers_common_sql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-06 04:50:32.000000 apache-airflow-providers-common-sql-1.6.0rc2/apache_airflow_providers_common_sql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-common-sql-1.6.0rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1970 2023-07-06 04:50:33.013643 apache-airflow-providers-common-sql-1.6.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-07-06 04:50:31.000000 apache-airflow-providers-common-sql-1.6.0rc2/setup.py
```

### Comparing `apache-airflow-providers-common-sql-1.6.0rc1/LICENSE` & `apache-airflow-providers-common-sql-1.6.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.6.0rc1/MANIFEST.in` & `apache-airflow-providers-common-sql-1.6.0rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.6.0rc1/PKG-INFO` & `apache-airflow-providers-common-sql-1.6.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-common-sql
-Version: 1.6.0rc1
+Version: 1.6.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-common-sql package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.0/
@@ -68,15 +68,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-common-sql``
 
-Release: ``1.6.0rc1``
+Release: ``1.6.0rc2``
 
 
 `Common SQL Provider <https://en.wikipedia.org/wiki/SQL>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-common-sql-1.6.0rc1/README.rst` & `apache-airflow-providers-common-sql-1.6.0rc2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-common-sql``
 
-Release: ``1.6.0rc1``
+Release: ``1.6.0rc2``
 
 
 `Common SQL Provider <https://en.wikipedia.org/wiki/SQL>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/__init__.py` & `apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/get_provider_info.py` & `apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/hooks/__init__.py` & `apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/hooks/sql.py` & `apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/hooks/sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -534,15 +534,15 @@
         """
         Returns database dialect used for SQL parsing.
 
         For a list of supported dialects check: https://openlineage.io/docs/development/sql#sql-dialects
         """
         return "generic"
 
-    def get_openlineage_default_schema(self) -> str:
+    def get_openlineage_default_schema(self) -> str | None:
         """
         Returns default schema specific to database.
 
         .. seealso::
             - :class:`airflow.providers.openlineage.sqlparser.SQLParser`
         """
         return self.__schema or "public"
```

### Comparing `apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/operators/__init__.py` & `apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/operators/sql.py` & `apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/operators/sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -316,15 +316,19 @@
                 default_schema=hook.get_openlineage_default_schema(),
             )
         except AttributeError:
             self.log.debug("%s failed to get database dialect", hook)
             return None
 
         operator_lineage = sql_parser.generate_openlineage_metadata_from_sql(
-            sql=self.sql, hook=hook, database_info=database_info, database=self.database
+            sql=self.sql,
+            hook=hook,
+            database_info=database_info,
+            database=self.database,
+            sqlalchemy_engine=hook.get_sqlalchemy_engine(),
         )
 
         return operator_lineage
 
     def get_openlineage_facets_on_complete(self, task_instance) -> OperatorLineage | None:
         operator_lineage = self.get_openlineage_facets_on_start() or OperatorLineage()
```

### Comparing `apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/sensors/__init__.py` & `apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/sensors/sql.py` & `apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/sensors/sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.6.0rc1/apache_airflow_providers_common_sql.egg-info/PKG-INFO` & `apache-airflow-providers-common-sql-1.6.0rc2/apache_airflow_providers_common_sql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-common-sql
-Version: 1.6.0rc1
+Version: 1.6.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-common-sql package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.0/
@@ -68,15 +68,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-common-sql``
 
-Release: ``1.6.0rc1``
+Release: ``1.6.0rc2``
 
 
 `Common SQL Provider <https://en.wikipedia.org/wiki/SQL>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-common-sql-1.6.0rc1/apache_airflow_providers_common_sql.egg-info/SOURCES.txt` & `apache-airflow-providers-common-sql-1.6.0rc2/apache_airflow_providers_common_sql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.6.0rc1/pyproject.toml` & `apache-airflow-providers-common-sql-1.6.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.6.0rc1/setup.cfg` & `apache-airflow-providers-common-sql-1.6.0rc2/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -54,10 +54,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.common.sql.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.common.sql
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-common-sql-1.6.0rc1/setup.py` & `apache-airflow-providers-common-sql-1.6.0rc2/setup.py`

 * *Files identical despite different names*

