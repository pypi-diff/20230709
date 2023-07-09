# Comparing `tmp/airflow-data-validation-4.0.4.tar.gz` & `tmp/airflow-data-validation-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow-data-validation-4.0.4.tar", max compression
+gzip compressed data, was "airflow-data-validation-4.0.5.tar", max compression
```

## Comparing `airflow-data-validation-4.0.4.tar` & `airflow-data-validation-4.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-06-06 08:59:19.718494 airflow-data-validation-4.0.4/README.md
--rw-r--r--   0        0        0        0 2023-06-08 08:24:12.682050 airflow-data-validation-4.0.4/airflow_data_validation/__init__.py
--rw-r--r--   0        0        0     9467 2023-06-11 13:32:57.418396 airflow-data-validation-4.0.4/airflow_data_validation/data_validation.py
--rw-r--r--   0        0        0      279 2023-06-08 08:49:06.605887 airflow-data-validation-4.0.4/airflow_data_validation/setup.py
--rw-r--r--   0        0        0      603 2023-06-11 13:42:15.352955 airflow-data-validation-4.0.4/pyproject.toml
--rw-r--r--   0        0        0      710 2023-06-11 13:42:24.314680 airflow-data-validation-4.0.4/setup.py
--rw-r--r--   0        0        0      694 2023-06-11 13:42:24.314934 airflow-data-validation-4.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-06 08:59:19.718494 airflow-data-validation-4.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-08 08:24:12.682050 airflow-data-validation-4.0.5/airflow_data_validation/__init__.py
+-rw-r--r--   0        0        0    10421 2023-07-09 12:00:47.761778 airflow-data-validation-4.0.5/airflow_data_validation/data_validation.py
+-rw-r--r--   0        0        0      279 2023-07-09 12:05:10.216892 airflow-data-validation-4.0.5/airflow_data_validation/setup.py
+-rw-r--r--   0        0        0      603 2023-07-09 12:11:58.824024 airflow-data-validation-4.0.5/pyproject.toml
+-rw-r--r--   0        0        0      710 2023-07-09 12:12:02.125887 airflow-data-validation-4.0.5/setup.py
+-rw-r--r--   0        0        0      694 2023-07-09 12:12:02.126101 airflow-data-validation-4.0.5/PKG-INFO
```

### Comparing `airflow-data-validation-4.0.4/airflow_data_validation/data_validation.py` & `airflow-data-validation-4.0.5/airflow_data_validation/data_validation.py`

 * *Files 8% similar despite different names*

```diff
@@ -77,14 +77,33 @@
                              AND {partition_field} = (SELECT MAX({partition_field}) FROM `{destination_table}` 
                                                     WHERE {partition_field} >= DATE_SUB(current_date, INTERVAL 1 DAY)))'''
         else:
             sql += f"WHERE {column_id} not in ({values}) )"
 
         return sql
 
+    def test_data_freshness(self, destination_table, is_partitioned, partition_field):
+
+        sql = f'''
+            SELECT MAX(_CHANGE_TIMESTAMP) dt
+              FROM appends(table `{destination_table}`, '2023-06-29', null)
+             WHERE _CHANGE_TYPE = 'INSERT'
+        '''
+        if is_partitioned:
+            sql = f'''SELECT MAX({partition_field}) dt
+                        FROM `{destination_table}` 
+                        WHERE {partition_field} >= DATE_SUB(current_date, INTERVAL 2 DAY)))'''
+
+        final_sql = f'''
+        SELECT EXISTS (SELECT *
+               FROM   ({sql}) c
+               WHERE  DATE(dt) != CURRENT_DATE()) 
+                '''
+        return final_sql
+
     def test_range_of_values(self, destination_table, column_ids_list, min_value, max_value, is_partitioned,
                              partition_field):
         column_id = ','.join(column_ids_list)
         sql = f'''
             SELECT EXISTS (
             SELECT {column_id}
             FROM `{destination_table}`
@@ -191,14 +210,17 @@
                                              min_value=min_value, max_value=max_value, partition_field=partition_field)
         elif test_name == 'expect_column_values_range_to_be_between':
             if len(column_ids_list) > 1:
                 raise ValueError("this test is only available on one column")
             sql = self.test_range_of_values(destination_table=destination_table, column_ids_list=column_ids_list,
                                             min_value=min_value, max_value=max_value,
                                             is_partitioned=is_partitioned, partition_field=partition_field)
+        elif test_name == 'expect_table_contains_todays_new_data':
+            sql = self.test_data_freshness(destination_table=destination_table,
+                                            is_partitioned=is_partitioned, partition_field=partition_field)
 
         qa_result = self.run_query(sql)
 
         if qa_result:  # True means that the quality test failed
             logging.info(f'#### {test_name} Quality Test failed ####')
             msg_text = f"You test failed {test_name}"
             logging.info(msg_text)
```

### Comparing `airflow-data-validation-4.0.4/pyproject.toml` & `airflow-data-validation-4.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "airflow-data-validation"
-version = "4.0.4"
+version = "4.0.5"
 description = ""
 authors = ["sapir.krespil <sapir.krespil@guesty.com>"]
 readme = "README.md"
 homepage = "https://github.com/guestyorg/airflow_data_validation"
 repository = "https://github.com/guestyorg/airflow_data_validation"
 packages = [{include = "airflow_data_validation"}]
```

### Comparing `airflow-data-validation-4.0.4/setup.py` & `airflow-data-validation-4.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['google-cloud-bigquery>=2.4.0,<3.0.0', 'requests>=2.0.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'airflow-data-validation',
-    'version': '4.0.4',
+    'version': '4.0.5',
     'description': '',
     'long_description': '',
     'author': 'sapir.krespil',
     'author_email': 'sapir.krespil@guesty.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/guestyorg/airflow_data_validation',
```

### Comparing `airflow-data-validation-4.0.4/PKG-INFO` & `airflow-data-validation-4.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-data-validation
-Version: 4.0.4
+Version: 4.0.5
 Summary: 
 Home-page: https://github.com/guestyorg/airflow_data_validation
 Author: sapir.krespil
 Author-email: sapir.krespil@guesty.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

