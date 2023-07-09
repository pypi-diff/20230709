# Comparing `tmp/ir_client-0.1.2.tar.gz` & `tmp/ir_client-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ir_client-0.1.2.tar", max compression
+gzip compressed data, was "ir_client-0.1.3.tar", max compression
```

## Comparing `ir_client-0.1.2.tar` & `ir_client-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1068 2023-07-09 09:40:09.015525 ir_client-0.1.2/LICENSE
--rw-r--r--   0        0        0     1064 2023-07-09 09:32:13.241585 ir_client-0.1.2/ir_client/__init__.py
--rw-r--r--   0        0        0     1167 2023-07-09 09:32:13.257593 ir_client-0.1.2/ir_client/endpoint_parameters.py
--rw-r--r--   0        0        0     1624 2023-07-09 09:33:00.701328 ir_client-0.1.2/ir_client/endpoint_types.py
--rw-r--r--   0        0        0      319 2023-07-09 09:32:13.257593 ir_client-0.1.2/ir_client/exceptions.py
--rw-r--r--   0        0        0     1611 2023-07-09 09:33:00.701328 ir_client-0.1.2/ir_client/iracing_client.py
--rw-r--r--   0        0        0        0 2023-07-09 09:32:13.289609 ir_client-0.1.2/ir_client/laps/__init__.py
--rw-r--r--   0        0        0      706 2023-07-09 09:33:00.701328 ir_client-0.1.2/ir_client/laps/mappers.py
--rw-r--r--   0        0        0      680 2023-07-09 09:33:00.705330 ir_client-0.1.2/ir_client/laps/models.py
--rw-r--r--   0        0        0        0 2023-07-09 09:32:13.305617 ir_client-0.1.2/ir_client/series_race_results/__init__.py
--rw-r--r--   0        0        0     1227 2023-07-09 13:51:03.543560 ir_client-0.1.2/ir_client/series_race_results/mappers.py
--rw-r--r--   0        0        0      332 2023-07-09 09:32:13.325627 ir_client-0.1.2/ir_client/series_race_results/models.py
--rw-r--r--   0        0        0      104 2023-07-09 09:32:13.333631 ir_client-0.1.2/ir_client/session_parameters.py
--rw-r--r--   0        0        0        0 2023-07-09 09:32:13.333631 ir_client-0.1.2/ir_client/subsession_results/__init__.py
--rw-r--r--   0        0        0     4790 2023-07-09 09:33:00.737346 ir_client-0.1.2/ir_client/subsession_results/mappers.py
--rw-r--r--   0        0        0     1462 2023-07-09 09:33:00.709332 ir_client-0.1.2/ir_client/subsession_results/models.py
--rw-r--r--   0        0        0        0 2023-07-09 09:32:13.337633 ir_client-0.1.2/ir_client/utils/__init__.py
--rw-r--r--   0        0        0      369 2023-07-09 13:50:23.083392 ir_client-0.1.2/ir_client/utils/collections.py
--rw-r--r--   0        0        0      344 2023-07-09 09:32:13.337633 ir_client-0.1.2/ir_client/utils/datetime_utils.py
--rw-r--r--   0        0        0     1510 2023-07-09 09:32:13.337633 ir_client-0.1.2/ir_client/utils/enum_utils.py
--rw-r--r--   0        0        0     1540 2023-07-09 09:32:13.337633 ir_client-0.1.2/ir_client/utils/url_utils.py
--rw-r--r--   0        0        0      367 2023-07-09 13:52:51.504007 ir_client-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      742 1970-01-01 00:00:00.000000 ir_client-0.1.2/setup.py
--rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 ir_client-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-09 09:40:09.015525 ir_client-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1064 2023-07-09 09:32:13.241585 ir_client-0.1.3/ir_client/__init__.py
+-rw-r--r--   0        0        0     1167 2023-07-09 09:32:13.257593 ir_client-0.1.3/ir_client/endpoint_parameters.py
+-rw-r--r--   0        0        0     1624 2023-07-09 09:33:00.701328 ir_client-0.1.3/ir_client/endpoint_types.py
+-rw-r--r--   0        0        0      319 2023-07-09 09:32:13.257593 ir_client-0.1.3/ir_client/exceptions.py
+-rw-r--r--   0        0        0     1611 2023-07-09 09:33:00.701328 ir_client-0.1.3/ir_client/iracing_client.py
+-rw-r--r--   0        0        0        0 2023-07-09 09:32:13.289609 ir_client-0.1.3/ir_client/laps/__init__.py
+-rw-r--r--   0        0        0      706 2023-07-09 09:33:00.701328 ir_client-0.1.3/ir_client/laps/mappers.py
+-rw-r--r--   0        0        0      680 2023-07-09 09:33:00.705330 ir_client-0.1.3/ir_client/laps/models.py
+-rw-r--r--   0        0        0        0 2023-07-09 09:32:13.305617 ir_client-0.1.3/ir_client/series_race_results/__init__.py
+-rw-r--r--   0        0        0     1227 2023-07-09 13:51:03.543560 ir_client-0.1.3/ir_client/series_race_results/mappers.py
+-rw-r--r--   0        0        0      332 2023-07-09 09:32:13.325627 ir_client-0.1.3/ir_client/series_race_results/models.py
+-rw-r--r--   0        0        0      104 2023-07-09 09:32:13.333631 ir_client-0.1.3/ir_client/session_parameters.py
+-rw-r--r--   0        0        0        0 2023-07-09 09:32:13.333631 ir_client-0.1.3/ir_client/subsession_results/__init__.py
+-rw-r--r--   0        0        0     4790 2023-07-09 09:33:00.737346 ir_client-0.1.3/ir_client/subsession_results/mappers.py
+-rw-r--r--   0        0        0     1462 2023-07-09 09:33:00.709332 ir_client-0.1.3/ir_client/subsession_results/models.py
+-rw-r--r--   0        0        0        0 2023-07-09 09:32:13.337633 ir_client-0.1.3/ir_client/utils/__init__.py
+-rw-r--r--   0        0        0      369 2023-07-09 13:50:23.083392 ir_client-0.1.3/ir_client/utils/collections.py
+-rw-r--r--   0        0        0      344 2023-07-09 09:32:13.337633 ir_client-0.1.3/ir_client/utils/datetime_utils.py
+-rw-r--r--   0        0        0     1510 2023-07-09 09:32:13.337633 ir_client-0.1.3/ir_client/utils/enum_utils.py
+-rw-r--r--   0        0        0     1540 2023-07-09 09:32:13.337633 ir_client-0.1.3/ir_client/utils/url_utils.py
+-rw-r--r--   0        0        0      393 2023-07-09 13:56:34.864902 ir_client-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      775 1970-01-01 00:00:00.000000 ir_client-0.1.3/setup.py
+-rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 ir_client-0.1.3/PKG-INFO
```

### Comparing `ir_client-0.1.2/LICENSE` & `ir_client-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ir_client-0.1.2/ir_client/__init__.py` & `ir_client-0.1.3/ir_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ir_client-0.1.2/ir_client/endpoint_parameters.py` & `ir_client-0.1.3/ir_client/endpoint_parameters.py`

 * *Files identical despite different names*

### Comparing `ir_client-0.1.2/ir_client/endpoint_types.py` & `ir_client-0.1.3/ir_client/endpoint_types.py`

 * *Files identical despite different names*

### Comparing `ir_client-0.1.2/ir_client/iracing_client.py` & `ir_client-0.1.3/ir_client/iracing_client.py`

 * *Files identical despite different names*

### Comparing `ir_client-0.1.2/ir_client/laps/mappers.py` & `ir_client-0.1.3/ir_client/laps/mappers.py`

 * *Files identical despite different names*

### Comparing `ir_client-0.1.2/ir_client/laps/models.py` & `ir_client-0.1.3/ir_client/laps/models.py`

 * *Files identical despite different names*

### Comparing `ir_client-0.1.2/ir_client/series_race_results/mappers.py` & `ir_client-0.1.3/ir_client/series_race_results/mappers.py`

 * *Files identical despite different names*

### Comparing `ir_client-0.1.2/ir_client/subsession_results/mappers.py` & `ir_client-0.1.3/ir_client/subsession_results/mappers.py`

 * *Files identical despite different names*

### Comparing `ir_client-0.1.2/ir_client/subsession_results/models.py` & `ir_client-0.1.3/ir_client/subsession_results/models.py`

 * *Files identical despite different names*

### Comparing `ir_client-0.1.2/ir_client/utils/enum_utils.py` & `ir_client-0.1.3/ir_client/utils/enum_utils.py`

 * *Files identical despite different names*

### Comparing `ir_client-0.1.2/ir_client/utils/url_utils.py` & `ir_client-0.1.3/ir_client/utils/url_utils.py`

 * *Files identical despite different names*

### Comparing `ir_client-0.1.2/setup.py` & `ir_client-0.1.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,19 +8,19 @@
  'ir_client.subsession_results',
  'ir_client.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['requests>=2.31.0,<3.0.0']
+['more-itertools>=9.1.0,<10.0.0', 'requests>=2.31.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'ir-client',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'Library to access the iRacing web API',
     'long_description': 'None',
     'author': 'Sascha Lamp',
     'author_email': 'sascha@lamp-online.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `ir_client-0.1.2/PKG-INFO` & `ir_client-0.1.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: ir-client
-Version: 0.1.2
+Version: 0.1.3
 Summary: Library to access the iRacing web API
 License: MIT
 Author: Sascha Lamp
 Author-email: sascha@lamp-online.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: more-itertools (>=9.1.0,<10.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
```

