# Comparing `tmp/ir_client-0.1.0.tar.gz` & `tmp/ir_client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ir_client-0.1.0.tar", max compression
+gzip compressed data, was "ir_client-0.1.1.tar", max compression
```

## Comparing `ir_client-0.1.0.tar` & `ir_client-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1068 2023-07-09 09:40:09.015525 ir_client-0.1.0/LICENSE
--rw-r--r--   0        0        0     1064 2023-07-09 09:32:13.241585 ir_client-0.1.0/ir_client/__init__.py
--rw-r--r--   0        0        0     1167 2023-07-09 09:32:13.257593 ir_client-0.1.0/ir_client/endpoint_parameters.py
--rw-r--r--   0        0        0     1624 2023-07-09 09:33:00.701328 ir_client-0.1.0/ir_client/endpoint_types.py
--rw-r--r--   0        0        0      319 2023-07-09 09:32:13.257593 ir_client-0.1.0/ir_client/exceptions.py
--rw-r--r--   0        0        0     1611 2023-07-09 09:33:00.701328 ir_client-0.1.0/ir_client/iracing_client.py
--rw-r--r--   0        0        0        0 2023-07-09 09:32:13.289609 ir_client-0.1.0/ir_client/laps/__init__.py
--rw-r--r--   0        0        0      706 2023-07-09 09:33:00.701328 ir_client-0.1.0/ir_client/laps/mappers.py
--rw-r--r--   0        0        0      680 2023-07-09 09:33:00.705330 ir_client-0.1.0/ir_client/laps/models.py
--rw-r--r--   0        0        0        0 2023-07-09 09:32:13.305617 ir_client-0.1.0/ir_client/series_race_results/__init__.py
--rw-r--r--   0        0        0     1197 2023-07-09 09:33:00.709332 ir_client-0.1.0/ir_client/series_race_results/mappers.py
--rw-r--r--   0        0        0      332 2023-07-09 09:32:13.325627 ir_client-0.1.0/ir_client/series_race_results/models.py
--rw-r--r--   0        0        0      104 2023-07-09 09:32:13.333631 ir_client-0.1.0/ir_client/session_parameters.py
--rw-r--r--   0        0        0        0 2023-07-09 09:32:13.333631 ir_client-0.1.0/ir_client/subsession_results/__init__.py
--rw-r--r--   0        0        0     4790 2023-07-09 09:33:00.737346 ir_client-0.1.0/ir_client/subsession_results/mappers.py
--rw-r--r--   0        0        0     1462 2023-07-09 09:33:00.709332 ir_client-0.1.0/ir_client/subsession_results/models.py
--rw-r--r--   0        0        0        0 2023-07-09 09:32:13.337633 ir_client-0.1.0/ir_client/utils/__init__.py
--rw-r--r--   0        0        0      344 2023-07-09 09:32:13.337633 ir_client-0.1.0/ir_client/utils/datetime_utils.py
--rw-r--r--   0        0        0     1510 2023-07-09 09:32:13.337633 ir_client-0.1.0/ir_client/utils/enum_utils.py
--rw-r--r--   0        0        0     1540 2023-07-09 09:32:13.337633 ir_client-0.1.0/ir_client/utils/url_utils.py
--rw-r--r--   0        0        0      346 2023-07-09 09:41:43.014520 ir_client-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      650 1970-01-01 00:00:00.000000 ir_client-0.1.0/setup.py
--rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 ir_client-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-09 09:40:09.015525 ir_client-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1064 2023-07-09 09:32:13.241585 ir_client-0.1.1/ir_client/__init__.py
+-rw-r--r--   0        0        0     1167 2023-07-09 09:32:13.257593 ir_client-0.1.1/ir_client/endpoint_parameters.py
+-rw-r--r--   0        0        0     1624 2023-07-09 09:33:00.701328 ir_client-0.1.1/ir_client/endpoint_types.py
+-rw-r--r--   0        0        0      319 2023-07-09 09:32:13.257593 ir_client-0.1.1/ir_client/exceptions.py
+-rw-r--r--   0        0        0     1611 2023-07-09 09:33:00.701328 ir_client-0.1.1/ir_client/iracing_client.py
+-rw-r--r--   0        0        0        0 2023-07-09 09:32:13.289609 ir_client-0.1.1/ir_client/laps/__init__.py
+-rw-r--r--   0        0        0      706 2023-07-09 09:33:00.701328 ir_client-0.1.1/ir_client/laps/mappers.py
+-rw-r--r--   0        0        0      680 2023-07-09 09:33:00.705330 ir_client-0.1.1/ir_client/laps/models.py
+-rw-r--r--   0        0        0        0 2023-07-09 09:32:13.305617 ir_client-0.1.1/ir_client/series_race_results/__init__.py
+-rw-r--r--   0        0        0     1197 2023-07-09 09:33:00.709332 ir_client-0.1.1/ir_client/series_race_results/mappers.py
+-rw-r--r--   0        0        0      332 2023-07-09 09:32:13.325627 ir_client-0.1.1/ir_client/series_race_results/models.py
+-rw-r--r--   0        0        0      104 2023-07-09 09:32:13.333631 ir_client-0.1.1/ir_client/session_parameters.py
+-rw-r--r--   0        0        0        0 2023-07-09 09:32:13.333631 ir_client-0.1.1/ir_client/subsession_results/__init__.py
+-rw-r--r--   0        0        0     4790 2023-07-09 09:33:00.737346 ir_client-0.1.1/ir_client/subsession_results/mappers.py
+-rw-r--r--   0        0        0     1462 2023-07-09 09:33:00.709332 ir_client-0.1.1/ir_client/subsession_results/models.py
+-rw-r--r--   0        0        0        0 2023-07-09 09:32:13.337633 ir_client-0.1.1/ir_client/utils/__init__.py
+-rw-r--r--   0        0        0      344 2023-07-09 09:32:13.337633 ir_client-0.1.1/ir_client/utils/datetime_utils.py
+-rw-r--r--   0        0        0     1510 2023-07-09 09:32:13.337633 ir_client-0.1.1/ir_client/utils/enum_utils.py
+-rw-r--r--   0        0        0     1540 2023-07-09 09:32:13.337633 ir_client-0.1.1/ir_client/utils/url_utils.py
+-rw-r--r--   0        0        0      367 2023-07-09 13:36:12.283697 ir_client-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      742 1970-01-01 00:00:00.000000 ir_client-0.1.1/setup.py
+-rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 ir_client-0.1.1/PKG-INFO
```

### Comparing `ir_client-0.1.0/LICENSE` & `ir_client-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ir_client-0.1.0/ir_client/__init__.py` & `ir_client-0.1.1/ir_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ir_client-0.1.0/ir_client/endpoint_parameters.py` & `ir_client-0.1.1/ir_client/endpoint_parameters.py`

 * *Files identical despite different names*

### Comparing `ir_client-0.1.0/ir_client/endpoint_types.py` & `ir_client-0.1.1/ir_client/endpoint_types.py`

 * *Files identical despite different names*

### Comparing `ir_client-0.1.0/ir_client/iracing_client.py` & `ir_client-0.1.1/ir_client/iracing_client.py`

 * *Files identical despite different names*

### Comparing `ir_client-0.1.0/ir_client/laps/mappers.py` & `ir_client-0.1.1/ir_client/laps/mappers.py`

 * *Files identical despite different names*

### Comparing `ir_client-0.1.0/ir_client/laps/models.py` & `ir_client-0.1.1/ir_client/laps/models.py`

 * *Files identical despite different names*

### Comparing `ir_client-0.1.0/ir_client/series_race_results/mappers.py` & `ir_client-0.1.1/ir_client/series_race_results/mappers.py`

 * *Files identical despite different names*

### Comparing `ir_client-0.1.0/ir_client/subsession_results/mappers.py` & `ir_client-0.1.1/ir_client/subsession_results/mappers.py`

 * *Files identical despite different names*

### Comparing `ir_client-0.1.0/ir_client/subsession_results/models.py` & `ir_client-0.1.1/ir_client/subsession_results/models.py`

 * *Files identical despite different names*

### Comparing `ir_client-0.1.0/ir_client/utils/enum_utils.py` & `ir_client-0.1.1/ir_client/utils/enum_utils.py`

 * *Files identical despite different names*

### Comparing `ir_client-0.1.0/ir_client/utils/url_utils.py` & `ir_client-0.1.1/ir_client/utils/url_utils.py`

 * *Files identical despite different names*

### Comparing `ir_client-0.1.0/setup.py` & `ir_client-0.1.1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,24 +7,28 @@
  'ir_client.series_race_results',
  'ir_client.subsession_results',
  'ir_client.utils']
 
 package_data = \
 {'': ['*']}
 
+install_requires = \
+['requests>=2.31.0,<3.0.0']
+
 setup_kwargs = {
     'name': 'ir-client',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Library to access the iRacing web API',
     'long_description': 'None',
     'author': 'Sascha Lamp',
     'author_email': 'sascha@lamp-online.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
+    'install_requires': install_requires,
     'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

