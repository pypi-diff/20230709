# Comparing `tmp/autotraders-1.6.3.tar.gz` & `tmp/autotraders-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotraders-1.6.3.tar", last modified: Sat Jul  8 22:49:08 2023, max compression
+gzip compressed data, was "autotraders-1.6.4.tar", last modified: Sat Jul  8 22:53:35 2023, max compression
```

## Comparing `autotraders-1.6.3.tar` & `autotraders-1.6.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:49:08.627117 autotraders-1.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-08 22:48:56.000000 autotraders-1.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-08 22:49:08.627117 autotraders-1.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-08 22:48:56.000000 autotraders-1.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:49:08.623117 autotraders-1.6.3/autotraders/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-08 22:48:56.000000 autotraders-1.6.3/autotraders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-08 22:48:56.000000 autotraders-1.6.3/autotraders/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-08 22:48:56.000000 autotraders-1.6.3/autotraders/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:49:08.623117 autotraders-1.6.3/autotraders/faction/
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-08 22:48:56.000000 autotraders-1.6.3/autotraders/faction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-07-08 22:48:56.000000 autotraders-1.6.3/autotraders/faction/contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:49:08.623117 autotraders-1.6.3/autotraders/map/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 22:48:56.000000 autotraders-1.6.3/autotraders/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-08 22:48:56.000000 autotraders-1.6.3/autotraders/map/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-07-08 22:48:56.000000 autotraders-1.6.3/autotraders/map/waypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:49:08.623117 autotraders-1.6.3/autotraders/map/waypoint_types/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-08 22:48:56.000000 autotraders-1.6.3/autotraders/map/waypoint_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-08 22:48:56.000000 autotraders-1.6.3/autotraders/map/waypoint_types/jumpgate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-08 22:48:56.000000 autotraders-1.6.3/autotraders/map/waypoint_types/marketplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-08 22:48:56.000000 autotraders-1.6.3/autotraders/map/waypoint_types/shipyard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-08 22:48:56.000000 autotraders-1.6.3/autotraders/paginated_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-08 22:48:56.000000 autotraders-1.6.3/autotraders/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:49:08.623117 autotraders-1.6.3/autotraders/shared_models/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-08 22:48:56.000000 autotraders-1.6.3/autotraders/shared_models/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-08 22:48:56.000000 autotraders-1.6.3/autotraders/shared_models/map_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-08 22:48:56.000000 autotraders-1.6.3/autotraders/shared_models/ship_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-08 22:48:56.000000 autotraders-1.6.3/autotraders/shared_models/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-08 22:48:56.000000 autotraders-1.6.3/autotraders/shared_models/trait.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-08 22:48:56.000000 autotraders-1.6.3/autotraders/shared_models/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:49:08.627117 autotraders-1.6.3/autotraders/ship/
--rw-r--r--   0 runner    (1001) docker     (123)    11104 2023-07-08 22:48:56.000000 autotraders-1.6.3/autotraders/ship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-08 22:48:56.000000 autotraders-1.6.3/autotraders/ship/cargo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-08 22:48:56.000000 autotraders-1.6.3/autotraders/ship/nav.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-08 22:48:56.000000 autotraders-1.6.3/autotraders/ship/ship_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-08 22:48:56.000000 autotraders-1.6.3/autotraders/ship/states.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-08 22:48:56.000000 autotraders-1.6.3/autotraders/ship/survey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-08 22:48:56.000000 autotraders-1.6.3/autotraders/space_traders_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-07-08 22:48:56.000000 autotraders-1.6.3/autotraders/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-08 22:48:56.000000 autotraders-1.6.3/autotraders/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-08 22:48:56.000000 autotraders-1.6.3/autotraders/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:49:08.623117 autotraders-1.6.3/autotraders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-08 22:49:08.000000 autotraders-1.6.3/autotraders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-08 22:49:08.000000 autotraders-1.6.3/autotraders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 22:49:08.000000 autotraders-1.6.3/autotraders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-08 22:49:08.000000 autotraders-1.6.3/autotraders.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-08 22:49:08.000000 autotraders-1.6.3/autotraders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-08 22:48:56.000000 autotraders-1.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 22:49:08.627117 autotraders-1.6.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:49:08.627117 autotraders-1.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-08 22:48:56.000000 autotraders-1.6.3/tests/test_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-08 22:48:56.000000 autotraders-1.6.3/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-08 22:48:56.000000 autotraders-1.6.3/tests/test_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-07-08 22:48:56.000000 autotraders-1.6.3/tests/test_ship.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-08 22:48:56.000000 autotraders-1.6.3/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:53:35.264073 autotraders-1.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-08 22:53:23.000000 autotraders-1.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-08 22:53:35.264073 autotraders-1.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-08 22:53:23.000000 autotraders-1.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:53:35.260073 autotraders-1.6.4/autotraders/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:53:35.260073 autotraders-1.6.4/autotraders/faction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/faction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/faction/contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:53:35.260073 autotraders-1.6.4/autotraders/map/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/map/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/map/waypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:53:35.260073 autotraders-1.6.4/autotraders/map/waypoint_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/map/waypoint_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/map/waypoint_types/jumpgate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/map/waypoint_types/marketplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/map/waypoint_types/shipyard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/paginated_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:53:35.260073 autotraders-1.6.4/autotraders/shared_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/shared_models/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/shared_models/map_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/shared_models/ship_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/shared_models/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/shared_models/trait.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/shared_models/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:53:35.260073 autotraders-1.6.4/autotraders/ship/
+-rw-r--r--   0 runner    (1001) docker     (123)    11104 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/ship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/ship/cargo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/ship/nav.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/ship/ship_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/ship/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/ship/survey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/space_traders_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:53:35.260073 autotraders-1.6.4/autotraders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-08 22:53:35.000000 autotraders-1.6.4/autotraders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-08 22:53:35.000000 autotraders-1.6.4/autotraders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 22:53:35.000000 autotraders-1.6.4/autotraders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-08 22:53:35.000000 autotraders-1.6.4/autotraders.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-08 22:53:35.000000 autotraders-1.6.4/autotraders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-08 22:53:23.000000 autotraders-1.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 22:53:35.264073 autotraders-1.6.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:53:35.264073 autotraders-1.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-08 22:53:23.000000 autotraders-1.6.4/tests/test_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-08 22:53:23.000000 autotraders-1.6.4/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-08 22:53:23.000000 autotraders-1.6.4/tests/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-07-08 22:53:23.000000 autotraders-1.6.4/tests/test_ship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-08 22:53:23.000000 autotraders-1.6.4/tests/test_util.py
```

### Comparing `autotraders-1.6.3/LICENSE` & `autotraders-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.3/PKG-INFO` & `autotraders-1.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.6.3
+Version: 1.6.4
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://comsictraders.github.io/autotraders/
 Project-URL: Repository, https://github.com/comsictraders/autotraders.git
 Project-URL: Changelog, https://github.com/comsictraders/autotraders/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://comsictraders.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/comsictraders/autotraders/issues
```

### Comparing `autotraders-1.6.3/README.md` & `autotraders-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.3/autotraders/agent.py` & `autotraders-1.6.4/autotraders/agent.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.3/autotraders/faction/__init__.py` & `autotraders-1.6.4/autotraders/faction/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.3/autotraders/faction/contract.py` & `autotraders-1.6.4/autotraders/faction/contract.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.3/autotraders/map/system.py` & `autotraders-1.6.4/autotraders/map/system.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.3/autotraders/map/waypoint.py` & `autotraders-1.6.4/autotraders/map/waypoint.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.3/autotraders/map/waypoint_types/__init__.py` & `autotraders-1.6.4/autotraders/map/waypoint_types/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.3/autotraders/map/waypoint_types/jumpgate.py` & `autotraders-1.6.4/autotraders/map/waypoint_types/jumpgate.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.3/autotraders/map/waypoint_types/marketplace.py` & `autotraders-1.6.4/autotraders/map/waypoint_types/marketplace.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.3/autotraders/map/waypoint_types/shipyard.py` & `autotraders-1.6.4/autotraders/map/waypoint_types/shipyard.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.3/autotraders/paginated_list.py` & `autotraders-1.6.4/autotraders/paginated_list.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.3/autotraders/session.py` & `autotraders-1.6.4/autotraders/session.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.3/autotraders/shared_models/map_symbol.py` & `autotraders-1.6.4/autotraders/shared_models/map_symbol.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.3/autotraders/shared_models/transaction.py` & `autotraders-1.6.4/autotraders/shared_models/transaction.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.3/autotraders/ship/__init__.py` & `autotraders-1.6.4/autotraders/ship/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.3/autotraders/ship/cargo.py` & `autotraders-1.6.4/autotraders/ship/cargo.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.3/autotraders/ship/nav.py` & `autotraders-1.6.4/autotraders/ship/nav.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.3/autotraders/ship/ship_components.py` & `autotraders-1.6.4/autotraders/ship/ship_components.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.3/autotraders/space_traders_entity.py` & `autotraders-1.6.4/autotraders/space_traders_entity.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.3/autotraders/status.py` & `autotraders-1.6.4/autotraders/status.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.3/autotraders/util.py` & `autotraders-1.6.4/autotraders/util.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.3/autotraders.egg-info/PKG-INFO` & `autotraders-1.6.4/autotraders.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.6.3
+Version: 1.6.4
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://comsictraders.github.io/autotraders/
 Project-URL: Repository, https://github.com/comsictraders/autotraders.git
 Project-URL: Changelog, https://github.com/comsictraders/autotraders/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://comsictraders.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/comsictraders/autotraders/issues
```

### Comparing `autotraders-1.6.3/autotraders.egg-info/SOURCES.txt` & `autotraders-1.6.4/autotraders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.3/pyproject.toml` & `autotraders-1.6.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.3/tests/test_init.py` & `autotraders-1.6.4/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.3/tests/test_map.py` & `autotraders-1.6.4/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.3/tests/test_ship.py` & `autotraders-1.6.4/tests/test_ship.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.3/tests/test_util.py` & `autotraders-1.6.4/tests/test_util.py`

 * *Files identical despite different names*

