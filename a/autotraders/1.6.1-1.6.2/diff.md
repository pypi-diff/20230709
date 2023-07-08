# Comparing `tmp/autotraders-1.6.1.tar.gz` & `tmp/autotraders-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotraders-1.6.1.tar", last modified: Fri Jun 30 00:48:36 2023, max compression
+gzip compressed data, was "autotraders-1.6.2.tar", last modified: Sat Jul  8 22:31:14 2023, max compression
```

## Comparing `autotraders-1.6.1.tar` & `autotraders-1.6.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:48:36.788461 autotraders-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-30 00:48:21.000000 autotraders-1.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-30 00:48:36.784461 autotraders-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-30 00:48:21.000000 autotraders-1.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:48:36.780461 autotraders-1.6.1/autotraders/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:48:36.780461 autotraders-1.6.1/autotraders/faction/
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/faction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/faction/contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:48:36.780461 autotraders-1.6.1/autotraders/map/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/map/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/map/waypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:48:36.784461 autotraders-1.6.1/autotraders/map/waypoint_types/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/map/waypoint_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/map/waypoint_types/jumpgate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/map/waypoint_types/marketplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/map/waypoint_types/shipyard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/paginated_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:48:36.784461 autotraders-1.6.1/autotraders/shared_models/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/shared_models/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/shared_models/map_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/shared_models/ship_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/shared_models/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/shared_models/trait.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/shared_models/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:48:36.784461 autotraders-1.6.1/autotraders/ship/
--rw-r--r--   0 runner    (1001) docker     (123)    11034 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/ship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/ship/cargo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/ship/nav.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/ship/ship_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/ship/states.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/ship/survey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/space_traders_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-30 00:48:21.000000 autotraders-1.6.1/autotraders/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:48:36.780461 autotraders-1.6.1/autotraders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-30 00:48:36.000000 autotraders-1.6.1/autotraders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-30 00:48:36.000000 autotraders-1.6.1/autotraders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 00:48:36.000000 autotraders-1.6.1/autotraders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-30 00:48:36.000000 autotraders-1.6.1/autotraders.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-30 00:48:36.000000 autotraders-1.6.1/autotraders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-30 00:48:21.000000 autotraders-1.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 00:48:36.788461 autotraders-1.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:48:36.784461 autotraders-1.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-30 00:48:21.000000 autotraders-1.6.1/tests/test_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-30 00:48:21.000000 autotraders-1.6.1/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-30 00:48:21.000000 autotraders-1.6.1/tests/test_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-30 00:48:21.000000 autotraders-1.6.1/tests/test_ship.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-30 00:48:21.000000 autotraders-1.6.1/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:31:14.113417 autotraders-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-08 22:31:00.000000 autotraders-1.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-08 22:31:14.113417 autotraders-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-08 22:31:00.000000 autotraders-1.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:31:14.109417 autotraders-1.6.2/autotraders/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-08 22:31:00.000000 autotraders-1.6.2/autotraders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-08 22:31:00.000000 autotraders-1.6.2/autotraders/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-08 22:31:00.000000 autotraders-1.6.2/autotraders/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:31:14.113417 autotraders-1.6.2/autotraders/faction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-08 22:31:00.000000 autotraders-1.6.2/autotraders/faction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-07-08 22:31:00.000000 autotraders-1.6.2/autotraders/faction/contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:31:14.113417 autotraders-1.6.2/autotraders/map/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 22:31:00.000000 autotraders-1.6.2/autotraders/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-08 22:31:00.000000 autotraders-1.6.2/autotraders/map/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-07-08 22:31:00.000000 autotraders-1.6.2/autotraders/map/waypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:31:14.113417 autotraders-1.6.2/autotraders/map/waypoint_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-08 22:31:00.000000 autotraders-1.6.2/autotraders/map/waypoint_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-08 22:31:00.000000 autotraders-1.6.2/autotraders/map/waypoint_types/jumpgate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-08 22:31:00.000000 autotraders-1.6.2/autotraders/map/waypoint_types/marketplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-08 22:31:00.000000 autotraders-1.6.2/autotraders/map/waypoint_types/shipyard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-08 22:31:00.000000 autotraders-1.6.2/autotraders/paginated_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-08 22:31:00.000000 autotraders-1.6.2/autotraders/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:31:14.113417 autotraders-1.6.2/autotraders/shared_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-08 22:31:00.000000 autotraders-1.6.2/autotraders/shared_models/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-08 22:31:00.000000 autotraders-1.6.2/autotraders/shared_models/map_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-08 22:31:00.000000 autotraders-1.6.2/autotraders/shared_models/ship_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-08 22:31:00.000000 autotraders-1.6.2/autotraders/shared_models/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-08 22:31:00.000000 autotraders-1.6.2/autotraders/shared_models/trait.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-08 22:31:00.000000 autotraders-1.6.2/autotraders/shared_models/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:31:14.113417 autotraders-1.6.2/autotraders/ship/
+-rw-r--r--   0 runner    (1001) docker     (123)    11104 2023-07-08 22:31:00.000000 autotraders-1.6.2/autotraders/ship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-08 22:31:00.000000 autotraders-1.6.2/autotraders/ship/cargo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-08 22:31:00.000000 autotraders-1.6.2/autotraders/ship/nav.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-08 22:31:00.000000 autotraders-1.6.2/autotraders/ship/ship_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-08 22:31:00.000000 autotraders-1.6.2/autotraders/ship/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-08 22:31:00.000000 autotraders-1.6.2/autotraders/ship/survey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-08 22:31:00.000000 autotraders-1.6.2/autotraders/space_traders_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-07-08 22:31:00.000000 autotraders-1.6.2/autotraders/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-08 22:31:00.000000 autotraders-1.6.2/autotraders/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-08 22:31:00.000000 autotraders-1.6.2/autotraders/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:31:14.113417 autotraders-1.6.2/autotraders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-08 22:31:14.000000 autotraders-1.6.2/autotraders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-08 22:31:14.000000 autotraders-1.6.2/autotraders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 22:31:14.000000 autotraders-1.6.2/autotraders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-08 22:31:14.000000 autotraders-1.6.2/autotraders.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-08 22:31:14.000000 autotraders-1.6.2/autotraders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-08 22:31:00.000000 autotraders-1.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 22:31:14.113417 autotraders-1.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:31:14.113417 autotraders-1.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-08 22:31:00.000000 autotraders-1.6.2/tests/test_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-08 22:31:00.000000 autotraders-1.6.2/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-08 22:31:00.000000 autotraders-1.6.2/tests/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-07-08 22:31:00.000000 autotraders-1.6.2/tests/test_ship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-08 22:31:00.000000 autotraders-1.6.2/tests/test_util.py
```

### Comparing `autotraders-1.6.1/LICENSE` & `autotraders-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.1/PKG-INFO` & `autotraders-1.6.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.6.1
+Version: 1.6.2
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
-Project-URL: Homepage, https://arihant2math.github.io/autotraders/
-Project-URL: Documentation, https://arihant2math.github.io/autotraders/
-Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
+Project-URL: Homepage, https://comsictraders.github.io/autotraders/
+Project-URL: Repository, https://github.com/comsictraders/autotraders.git
+Project-URL: Changelog, https://github.com/comsictraders/autotraders/blob/master/CHANGELOG.md
+Project-URL: Documentation, https://comsictraders.github.io/autotraders/
+Project-URL: Bug Tracker, https://github.com/comsictraders/autotraders/issues
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Development Status :: 4 - Beta
+Classifier: Topic :: Internet
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Autotraders
 [![Downloads](https://static.pepy.tech/badge/autotraders)](https://pepy.tech/project/autotraders)
 [![Python package](https://github.com/cosmictraders/autotraders/actions/workflows/python-package.yml/badge.svg)](https://github.com/cosmictraders/autotraders/actions/workflows/python-package.yml)
```

### Comparing `autotraders-1.6.1/README.md` & `autotraders-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.1/autotraders/agent.py` & `autotraders-1.6.2/autotraders/agent.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.1/autotraders/faction/__init__.py` & `autotraders-1.6.2/autotraders/faction/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,15 +37,15 @@
                 + "factions?limit="
                 + str(num_per_page)
                 + "&page="
                 + str(p)
             )
             j = r.json()
             if "error" in j:
-                raise SpaceTradersException(j["error"]["message"], r.status_code)
+                raise SpaceTradersException(j["error"], r.status_code)
             factions = []
             for f in j["data"]:
                 faction = Faction(f["symbol"], session, f)
                 factions.append(faction)
             return factions, r.json()["meta"]["total"]
 
         return PaginatedList(paginated_func, page)
```

### Comparing `autotraders-1.6.1/autotraders/faction/contract.py` & `autotraders-1.6.2/autotraders/faction/contract.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     @staticmethod
     def negotiate(ship_symbol, session):
         r = session.post(
             session.base_url + "my/ships/" + ship_symbol + "/negotiate/contract"
         )
         j = r.json()
         if "error" in j:
-            raise SpaceTradersException(j["error"]["message"], r.status_code)
+            raise SpaceTradersException(j["error"], r.status_code)
         c = Contract(j["data"]["contract"]["id"], session, j["data"]["contract"])
         return c
 
     def fulfill(self):
         j = self.post("fulfill")
         self.update(j["data"]["contract"])
 
@@ -78,15 +78,15 @@
                 + "my/contracts?limit="
                 + str(num_per_page)
                 + "&page="
                 + str(p)
             )
             j = r.json()
             if "error" in j:
-                raise SpaceTradersException(j["error"]["message"], r.status_code)
+                raise SpaceTradersException(j["error"], r.status_code)
             contracts = []
             for contract in j["data"]:
                 c = Contract(contract["id"], session, contract)
                 contracts.append(c)
             return contracts, r.json()["meta"]["total"]
 
         return PaginatedList(paginated_func, page)
```

### Comparing `autotraders-1.6.1/autotraders/map/system.py` & `autotraders-1.6.2/autotraders/map/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,27 +30,30 @@
             Waypoint(w["symbol"], self.session, w) for w in data["waypoints"]
         ]
         self.x = data["x"]
         self.y = data["y"]
         self.factions = data["factions"]
         self.star_type = data["type"]
 
+    def __str__(self):
+        return str(self.symbol)
+
     @staticmethod
     def all(session, page: int = 1) -> PaginatedList:
         def paginated_func(p, num_per_page):
             r = session.get(
                 session.base_url
                 + "systems?limit="
                 + str(num_per_page)
                 + "&page="
                 + str(p)
             )
             j = r.json()
             if "error" in j:
-                raise SpaceTradersException(j["error"]["message"], r.status_code)
+                raise SpaceTradersException(j["error"], r.status_code)
             systems = []
             for system in j["data"]:
                 s = System(system["symbol"], session, system)
                 systems.append(s)
             return systems, j["meta"]["total"]
 
         return PaginatedList(paginated_func, page)
```

### Comparing `autotraders-1.6.1/autotraders/map/waypoint.py` & `autotraders-1.6.2/autotraders/map/waypoint.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,29 +52,32 @@
             self.shipyard = (
                 len([trait for trait in self.traits if trait.symbol == "SHIPYARD"]) > 0
             )
         else:
             self.marketplace = None
             self.shipyard = None
 
+    def __str__(self):
+        return str(self.symbol)
+
     @staticmethod
     def all(session, system_symbol, page: int = 1) -> PaginatedList:
         def paginated_func(p, num_per_page):
             r = session.get(
                 session.base_url
                 + "systems/"
                 + system_symbol
                 + "/waypoints?limit="
                 + str(num_per_page)
                 + "&page="
                 + str(p)
             )
             j = r.json()
             if "error" in j:
-                raise SpaceTradersException(j["error"]["message"], r.status_code)
+                raise SpaceTradersException(j["error"], r.status_code)
             waypoints = []
             for w in j["data"]:
                 waypoint = Waypoint(w["symbol"], session, w)
                 waypoints.append(waypoint)
             return waypoints, j["meta"]["total"]
 
         return PaginatedList(paginated_func, page)
```

### Comparing `autotraders-1.6.1/autotraders/map/waypoint_types/__init__.py` & `autotraders-1.6.2/autotraders/map/waypoint_types/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.1/autotraders/map/waypoint_types/jumpgate.py` & `autotraders-1.6.2/autotraders/map/waypoint_types/jumpgate.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.1/autotraders/map/waypoint_types/marketplace.py` & `autotraders-1.6.2/autotraders/map/waypoint_types/marketplace.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.1/autotraders/map/waypoint_types/shipyard.py` & `autotraders-1.6.2/autotraders/map/waypoint_types/shipyard.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.1/autotraders/paginated_list.py` & `autotraders-1.6.2/autotraders/paginated_list.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 import math
 
 
-class PaginatedList:
+class PaginatedList:  # TODO: Don't use :param: for attrs
+    """
+    :param page: The current page
+    :param num_per_page: The number of items per a page
+    :param total: Total number of items
+    :param pages: number of pages
+    """
+
     def __init__(self, func, page, num_per_page=20):
         """
         A paginated list with caching
         :param func: Function to get page (must accept two ints denoting the page number and number of items per page
         and should return the data and total number of items)
         :param page: Page to start on
         :param num_per_page: How many items per a page
@@ -25,14 +32,21 @@
         self.page += 1
         return self.current()
 
     def prev(self):
         self.page -= 1
         return self.current()
 
+    def all(self):
+        """Gets all the pages and returns the list of all pages"""
+        for page in range(1, self.pages):
+            self.page = page
+            self.current()
+        return self.stitch()
+
     def __getitem__(self, key):
         assert type(key) is int
         self.page = key
         return self.current()
 
     def current(self):
         if self.inner.get(self.page) is None:
```

### Comparing `autotraders-1.6.1/autotraders/session.py` & `autotraders-1.6.2/autotraders/session.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.1/autotraders/shared_models/map_symbol.py` & `autotraders-1.6.2/autotraders/shared_models/map_symbol.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.1/autotraders/shared_models/transaction.py` & `autotraders-1.6.2/autotraders/shared_models/transaction.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.1/autotraders/ship/__init__.py` & `autotraders-1.6.2/autotraders/ship/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 class Crew:
     def __init__(self, data):
         self.current: int = data["current"]
         self.required: int = data["required"]
         self.capacity: int = data["capacity"]
         self.morale = data["morale"]
         self.wages = data["wages"]
+        self.rotation = data["rotation"]
 
 
 class Registration:
     def __init__(self, data):
         self.name: str = data["name"]
         self.faction_symbol: str = data["factionSymbol"]
         self.role: str = data["role"]
@@ -102,14 +103,17 @@
         if "cargo" in data:
             self.cargo = Cargo(self.symbol, self.session, data["cargo"])
         if "registration" in data:
             self.registration = Registration(data["registration"])
         if self.modules is not None and self.mounts is not None:
             self.capabilities = Capabilities(self.modules, self.mounts)
 
+    def __str__(self):
+        return self.symbol
+
     async def navigate_async(self, waypoint: Union[str, MapSymbol], interval=1):
         """Attempts to move ship to the provided waypoint.
         If the request succeeds, this function waits for the ship to arrive.
         :param interval: Frequency of updates in seconds (default: 1)
         """
         j = self.post("navigate", data={"waypointSymbol": str(waypoint)})
         self.update(j["data"])
@@ -149,15 +153,15 @@
             data=json.dumps(
                 {"flightMode": new_flight_mode}
             )  # Requests is so dumb I spent 30 minutes debugging this
             # just to find that its requests fault for sending a body of "flightMode=DRIFT".
         )
         j = r.json()
         if "error" in j:
-            raise SpaceTradersException(j["error"]["message"], r.status_code)
+            raise SpaceTradersException(j["error"], r.status_code)
         self.update({"nav": j["data"]})
 
     def dock(self):
         j = self.post("dock")
         self.update(j["data"])
 
     def orbit(self):
@@ -301,15 +305,15 @@
                 + "my/ships?limit="
                 + str(num_per_page)
                 + "&page="
                 + str(p)
             )
             j = r.json()
             if "error" in j:
-                raise SpaceTradersException(j["error"]["message"], r.status_code)
+                raise SpaceTradersException(j["error"], r.status_code)
             ships = []
             for ship in j["data"]:
                 s = Ship(ship["symbol"], session, ship)
                 ships.append(s)
             return ships, r.json()["meta"]["total"]
 
         return PaginatedList(paginated_func, page)
```

### Comparing `autotraders-1.6.1/autotraders/ship/cargo.py` & `autotraders-1.6.2/autotraders/ship/cargo.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.1/autotraders/ship/nav.py` & `autotraders-1.6.2/autotraders/ship/nav.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from datetime import datetime, timezone
 
 from autotraders import AutoTradersSession
 from autotraders.shared_models.map_symbol import MapSymbol
+from autotraders.ship.states import NavState, FlightMode
 from autotraders.space_traders_entity import SpaceTradersEntity
 from autotraders.time import parse_time
 
 
 class Route:
     def __init__(self, data):
         self.destination = MapSymbol(data["destination"]["symbol"])
@@ -24,12 +25,12 @@
 
     def __init__(self, symbol, session: AutoTradersSession, data=None):
         super().__init__(session, "my/ships/" + symbol, data)
 
     def update(self, data: dict = None) -> None:
         if data is None:
             data = self.get("nav")["data"]
-        self.status = data["status"]
+        self.status = NavState(data["status"])
         self.location = MapSymbol(data["waypointSymbol"])
-        self.flight_mode = data["flightMode"]
+        self.flight_mode = FlightMode(data["flightMode"])
         self.route = Route(data["route"])
         self.moving = self.route.moving
```

### Comparing `autotraders-1.6.1/autotraders/ship/ship_components.py` & `autotraders-1.6.2/autotraders/ship/ship_components.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.1/autotraders/space_traders_entity.py` & `autotraders-1.6.2/autotraders/space_traders_entity.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                 self.action_url + action,
                 data=json.dumps(data),
             )
         else:
             r = self.session.post(self.action_url + action)
         j = r.json()
         if "error" in j:
-            raise SpaceTradersException(j["error"]["message"], r.status_code)
+            raise SpaceTradersException(j["error"], r.status_code)
         return j
 
     def update(self, data: dict = None):
         """
         :param data: If you have data from an api requests, you can provide it here. If not provided, an API request
         will be sent.
         :raise IOException: If the server fails
```

### Comparing `autotraders-1.6.1/autotraders/status.py` & `autotraders-1.6.2/autotraders/status.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     """returns the API status, with reset dates, see the Status class for more info."""
     if session is None:
         r = requests.get("https://api.spacetraders.io/v2/")
     else:
         r = session.get("https://api.spacetraders.io/v2/")
     j = r.json()
     if "error" in j:
-        raise SpaceTradersException(j["error"]["message"], r.status_code)
+        raise SpaceTradersException(j["error"], r.status_code)
     s = Status()
     s.status = j["status"]
     s.version = j["version"]
     s.reset_date = parse_time(j["resetDate"])
     s.description = j["description"]
     s.stats = j["stats"]
     s.next_reset = parse_time(j["serverResets"]["next"])
```

### Comparing `autotraders-1.6.1/autotraders/util.py` & `autotraders-1.6.2/autotraders/util.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.1/autotraders.egg-info/PKG-INFO` & `autotraders-1.6.2/autotraders.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.6.1
+Version: 1.6.2
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
-Project-URL: Homepage, https://arihant2math.github.io/autotraders/
-Project-URL: Documentation, https://arihant2math.github.io/autotraders/
-Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
+Project-URL: Homepage, https://comsictraders.github.io/autotraders/
+Project-URL: Repository, https://github.com/comsictraders/autotraders.git
+Project-URL: Changelog, https://github.com/comsictraders/autotraders/blob/master/CHANGELOG.md
+Project-URL: Documentation, https://comsictraders.github.io/autotraders/
+Project-URL: Bug Tracker, https://github.com/comsictraders/autotraders/issues
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Development Status :: 4 - Beta
+Classifier: Topic :: Internet
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Autotraders
 [![Downloads](https://static.pepy.tech/badge/autotraders)](https://pepy.tech/project/autotraders)
 [![Python package](https://github.com/cosmictraders/autotraders/actions/workflows/python-package.yml/badge.svg)](https://github.com/cosmictraders/autotraders/actions/workflows/python-package.yml)
```

### Comparing `autotraders-1.6.1/autotraders.egg-info/SOURCES.txt` & `autotraders-1.6.2/autotraders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.1/tests/test_init.py` & `autotraders-1.6.2/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.1/tests/test_map.py` & `autotraders-1.6.2/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.1/tests/test_ship.py` & `autotraders-1.6.2/tests/test_ship.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.1/tests/test_util.py` & `autotraders-1.6.2/tests/test_util.py`

 * *Files identical despite different names*

