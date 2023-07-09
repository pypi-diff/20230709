# Comparing `tmp/lcwc-0.6.tar.gz` & `tmp/lcwc-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lcwc-0.6.tar", last modified: Fri Jun 30 18:48:35 2023, max compression
+gzip compressed data, was "lcwc-0.7.tar", last modified: Sun Jul  9 20:05:33 2023, max compression
```

## Comparing `lcwc-0.6.tar` & `lcwc-0.7.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 18:48:35.420009 lcwc-0.6/
--rw-rw-rw-   0        0        0     1058 2023-01-16 14:14:04.000000 lcwc-0.6/LICENSE
--rw-rw-rw-   0        0        0     2325 2023-06-30 18:48:35.419510 lcwc-0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1671 2023-06-10 14:58:54.000000 lcwc-0.6/README.md
--rw-rw-rw-   0        0        0      802 2023-06-30 18:44:05.000000 lcwc-0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-30 18:48:35.420009 lcwc-0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-30 18:48:35.381510 lcwc-0.6/src/
-drwxrwxrwx   0        0        0        0 2023-06-30 18:48:35.398009 lcwc-0.6/src/lcwc/
--rw-rw-rw-   0        0        0      120 2023-06-30 18:41:06.000000 lcwc-0.6/src/lcwc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 18:48:35.407009 lcwc-0.6/src/lcwc/arcgis/
--rw-rw-rw-   0        0        0       72 2023-06-30 18:00:38.000000 lcwc-0.6/src/lcwc/arcgis/__init__.py
--rw-rw-rw-   0        0        0     6273 2023-06-30 18:39:48.000000 lcwc-0.6/src/lcwc/arcgis/client.py
--rw-rw-rw-   0        0        0     1631 2023-06-30 18:39:07.000000 lcwc-0.6/src/lcwc/arcgis/incident.py
--rw-rw-rw-   0        0        0      326 2023-06-24 14:32:45.000000 lcwc-0.6/src/lcwc/category.py
--rw-rw-rw-   0        0        0      318 2023-06-30 18:02:43.000000 lcwc-0.6/src/lcwc/client.py
-drwxrwxrwx   0        0        0        0 2023-06-30 18:48:35.411011 lcwc-0.6/src/lcwc/feed/
--rw-rw-rw-   0        0        0       68 2023-06-30 17:57:06.000000 lcwc-0.6/src/lcwc/feed/__init__.py
--rw-rw-rw-   0        0        0     4468 2023-06-30 18:37:18.000000 lcwc-0.6/src/lcwc/feed/client.py
--rw-rw-rw-   0        0        0      926 2023-06-30 18:37:26.000000 lcwc-0.6/src/lcwc/feed/incident.py
-drwxrwxrwx   0        0        0        0 2023-06-30 18:48:35.412009 lcwc-0.6/src/lcwc/feed/utils/
--rw-rw-rw-   0        0        0     2373 2023-06-30 18:38:10.000000 lcwc-0.6/src/lcwc/feed/utils/__init__.py
--rw-rw-rw-   0        0        0     1486 2023-06-30 18:36:44.000000 lcwc-0.6/src/lcwc/incident.py
--rw-rw-rw-   0        0        0      512 2023-06-30 18:35:11.000000 lcwc-0.6/src/lcwc/unit.py
-drwxrwxrwx   0        0        0        0 2023-06-30 18:48:35.414511 lcwc-0.6/src/lcwc/utils/
--rw-rw-rw-   0        0        0      610 2023-06-30 17:20:03.000000 lcwc-0.6/src/lcwc/utils/__init__.py
--rw-rw-rw-   0        0        0     4162 2023-06-24 14:32:45.000000 lcwc-0.6/src/lcwc/utils/restadapter.py
-drwxrwxrwx   0        0        0        0 2023-06-30 18:48:35.418010 lcwc-0.6/src/lcwc/web/
--rw-rw-rw-   0        0        0       64 2023-06-30 17:55:06.000000 lcwc-0.6/src/lcwc/web/__init__.py
--rw-rw-rw-   0        0        0     3972 2023-06-30 18:34:22.000000 lcwc-0.6/src/lcwc/web/client.py
--rw-rw-rw-   0        0        0     2459 2023-06-30 18:31:01.000000 lcwc-0.6/src/lcwc/web/incident.py
-drwxrwxrwx   0        0        0        0 2023-06-30 18:48:35.403510 lcwc-0.6/src/lcwc.egg-info/
--rw-rw-rw-   0        0        0     2325 2023-06-30 18:48:35.000000 lcwc-0.6/src/lcwc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      610 2023-06-30 18:48:35.000000 lcwc-0.6/src/lcwc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 18:48:35.000000 lcwc-0.6/src/lcwc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-06-30 18:48:35.000000 lcwc-0.6/src/lcwc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-30 18:48:35.000000 lcwc-0.6/src/lcwc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-09 20:05:33.259806 lcwc-0.7/
+-rw-rw-rw-   0        0        0     1058 2023-01-16 14:14:04.000000 lcwc-0.7/LICENSE
+-rw-rw-rw-   0        0        0     2325 2023-07-09 20:05:33.259306 lcwc-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1671 2023-06-10 14:58:54.000000 lcwc-0.7/README.md
+-rw-rw-rw-   0        0        0      802 2023-07-09 20:05:21.000000 lcwc-0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-09 20:05:33.260306 lcwc-0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-09 20:05:33.215306 lcwc-0.7/src/
+drwxrwxrwx   0        0        0        0 2023-07-09 20:05:33.233306 lcwc-0.7/src/lcwc/
+-rw-rw-rw-   0        0        0      124 2023-07-09 20:01:56.000000 lcwc-0.7/src/lcwc/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 20:05:33.243308 lcwc-0.7/src/lcwc/arcgis/
+-rw-rw-rw-   0        0        0       72 2023-06-30 18:00:38.000000 lcwc-0.7/src/lcwc/arcgis/__init__.py
+-rw-rw-rw-   0        0        0     6502 2023-07-09 20:01:56.000000 lcwc-0.7/src/lcwc/arcgis/client.py
+-rw-rw-rw-   0        0        0      769 2023-07-07 07:11:12.000000 lcwc-0.7/src/lcwc/arcgis/incident.py
+-rw-rw-rw-   0        0        0      326 2023-06-24 14:32:45.000000 lcwc-0.7/src/lcwc/category.py
+-rw-rw-rw-   0        0        0      318 2023-06-30 18:02:43.000000 lcwc-0.7/src/lcwc/client.py
+drwxrwxrwx   0        0        0        0 2023-07-09 20:05:33.246306 lcwc-0.7/src/lcwc/feed/
+-rw-rw-rw-   0        0        0       68 2023-06-30 17:57:06.000000 lcwc-0.7/src/lcwc/feed/__init__.py
+-rw-rw-rw-   0        0        0     4468 2023-06-30 18:37:18.000000 lcwc-0.7/src/lcwc/feed/client.py
+-rw-rw-rw-   0        0        0      241 2023-07-05 13:46:18.000000 lcwc-0.7/src/lcwc/feed/incident.py
+drwxrwxrwx   0        0        0        0 2023-07-09 20:05:33.248806 lcwc-0.7/src/lcwc/feed/utils/
+-rw-rw-rw-   0        0        0     2373 2023-06-30 18:38:10.000000 lcwc-0.7/src/lcwc/feed/utils/__init__.py
+-rw-rw-rw-   0        0        0      651 2023-07-01 15:08:06.000000 lcwc-0.7/src/lcwc/incident.py
+-rw-rw-rw-   0        0        0      330 2023-07-09 20:02:44.000000 lcwc-0.7/src/lcwc/unit.py
+drwxrwxrwx   0        0        0        0 2023-07-09 20:05:33.253308 lcwc-0.7/src/lcwc/utils/
+-rw-rw-rw-   0        0        0      668 2023-07-09 06:50:55.000000 lcwc-0.7/src/lcwc/utils/__init__.py
+-rw-rw-rw-   0        0        0     1737 2023-07-07 07:17:11.000000 lcwc-0.7/src/lcwc/utils/encoding.py
+-rw-rw-rw-   0        0        0     4286 2023-07-05 15:08:28.000000 lcwc-0.7/src/lcwc/utils/restadapter.py
+drwxrwxrwx   0        0        0        0 2023-07-09 20:05:33.258306 lcwc-0.7/src/lcwc/web/
+-rw-rw-rw-   0        0        0       64 2023-06-30 17:55:06.000000 lcwc-0.7/src/lcwc/web/__init__.py
+-rw-rw-rw-   0        0        0     3972 2023-06-30 18:34:22.000000 lcwc-0.7/src/lcwc/web/client.py
+-rw-rw-rw-   0        0        0      232 2023-06-30 20:31:48.000000 lcwc-0.7/src/lcwc/web/incident.py
+drwxrwxrwx   0        0        0        0 2023-07-09 20:05:33.239806 lcwc-0.7/src/lcwc.egg-info/
+-rw-rw-rw-   0        0        0     2325 2023-07-09 20:05:33.000000 lcwc-0.7/src/lcwc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      637 2023-07-09 20:05:33.000000 lcwc-0.7/src/lcwc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 20:05:33.000000 lcwc-0.7/src/lcwc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-07-09 20:05:33.000000 lcwc-0.7/src/lcwc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-09 20:05:33.000000 lcwc-0.7/src/lcwc.egg-info/top_level.txt
```

### Comparing `lcwc-0.6/LICENSE` & `lcwc-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lcwc-0.6/PKG-INFO` & `lcwc-0.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcwc
-Version: 0.6
+Version: 0.7
 Summary: Python library for fetching the Lancaster County-Wide Communications live incident list.
 Author-email: Nate Shoffner <nate.shoffner@gmail.com>
 Project-URL: Homepage, https://github.com/NateShoffner/python-lcwc
 Project-URL: Bug Tracker, https://github.com/NateShoffner/python-lcwc/issues
 Keywords: lcwc,lancaster,police,fire,ems,dispatch,911,incident
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lcwc-0.6/README.md` & `lcwc-0.7/README.md`

 * *Files identical despite different names*

### Comparing `lcwc-0.6/pyproject.toml` & `lcwc-0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lcwc"
-version = "0.6"
+version = "0.7"
 authors = [
   { name="Nate Shoffner", email="nate.shoffner@gmail.com" },
 ]
 description = "Python library for fetching the Lancaster County-Wide Communications live incident list."
 keywords = ["lcwc", "lancaster", "police", "fire", "ems", "dispatch", "911", "incident"]
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `lcwc-0.6/src/lcwc/arcgis/client.py` & `lcwc-0.7/src/lcwc/arcgis/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,26 @@
+import logging
 import aiohttp
 import datetime
 import json
 import re
 from lcwc import Client
 from lcwc.arcgis.incident import ArcGISIncident, Coordinates
 from lcwc.category import IncidentCategory
 from lcwc.unit import Unit
 from lcwc.utils.restadapter import RestAdapter, RestException
 
 
 class ArcGISClient(Client):
     """Client for the ArcGIS REST API"""
 
+    def __init__(self) -> None:
+        super().__init__()
+        self.logger = logging.getLogger(__name__)
+
     @property
     def name(self) -> str:
         return "ArcGISClient"
 
     async def get_incidents(
         self, session: aiohttp.ClientSession, timeout: int = 10
     ) -> list[ArcGISIncident]:
@@ -66,15 +71,16 @@
         incidents = []
 
         for cat in IncidentCategory:
             if cat == IncidentCategory.UNKNOWN:
                 continue
 
             if cat not in layer_mapping:
-                print(f"No layer mapping for {cat}")
+                self.logger.error(f"No layer mapping for {cat}")
+                continue
 
             layer_id = layer_mapping[cat]
 
             """ Actual spatial extent of Lancaster County based LanCo GIS data
             lanco_spatial = {
                 'xmin': -8548898.732776089,
                 'ymin': 4845979.963808246,
@@ -114,26 +120,28 @@
                 session,
                 "utility.arcgis.com",
                 "usrsvcs/servers/a1f6aa7faab44b1582029509c46dce86/rest/services/Maps/Public_LiveFeeds/MapServer/",
             )
 
             try:
                 resp = await adapter.get(endpoint=f"{layer_id}/query", ep_params=params)
+
             except RestException as e:
-                print(f"{cat} Error: {e}")
+                self.logger.error(f"{cat} Error: {e}")
                 continue
 
+            self.logger.debug(f"{resp.url}")
+
             if resp.status_code != 200:
-                print(f"Error: {resp.status_code} for {cat}")
+                self.logger.error(f"Error: {resp.status_code} for {cat}")
                 continue
 
             error = resp.data.get("error", None)
             if error:
-                print(resp.url)
-                print(f"Error: {error}")
+                self.logger.error(f"Response error: {error}")
                 continue
 
             if "features" not in resp.data:
                 continue
 
             for feature in resp.data["features"]:
                 incident = self.__parse_incident(cat, feature)
@@ -175,15 +183,15 @@
 
         incident = ArcGISIncident(
             category,
             date,
             description,
             municipality,
             intersection,
+            units,
             number,
             priority,
             agency,
             public,
-            coords,
-            units,
+            coords
         )
         return incident
```

### Comparing `lcwc-0.6/src/lcwc/feed/client.py` & `lcwc-0.7/src/lcwc/feed/client.py`

 * *Files identical despite different names*

### Comparing `lcwc-0.6/src/lcwc/feed/utils/__init__.py` & `lcwc-0.7/src/lcwc/feed/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lcwc-0.6/src/lcwc/utils/__init__.py` & `lcwc-0.7/src/lcwc/utils/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import datetime
 from lcwc.web.incident import WebIncident as Incident
 
+from .encoding import IncidentEncoder, IncidentDecoder
+
 
 def is_related_incident(a: Incident, b: Incident, delta: datetime.timedelta) -> bool:
     """Determines if two incidents are related based on the intersection and time delta
 
     :param a: The first incident
     :param b: The second incident
     :param delta: The time delta
```

### Comparing `lcwc-0.6/src/lcwc/utils/restadapter.py` & `lcwc-0.7/src/lcwc/utils/restadapter.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,25 +6,28 @@
 
 class Result:
     def __init__(
         self,
         status_code: int,
         headers: Dict,
         message: str = "",
+        url: str = "",
         data: List[Dict] = None,
     ):
         """
         Result returned from low-level RestAdapter
         :param status_code: Standard HTTP Status code
         :param message: Human readable result
+        :param url: URL of the response
         :param data: Python List of Dictionaries (or maybe just a single Dictionary on error)
         """
         self.status_code = int(status_code)
         self.headers = headers
         self.message = str(message)
+        self.url = url
         self.data = data if data else []
 
 
 class RestException(Exception):
     pass
 
 
@@ -96,14 +99,15 @@
         # If status_code in 200-299 range, return success Result with data, otherwise raise exception
         is_success = 299 >= status_code >= 200  # 200 to 299 is OK
         if is_success:
             return Result(
                 status_code,
                 headers=response.headers,
                 message=response.reason,
+                url=response.url,
                 data=data_out,
             )
         raise RestException(f"{status_code}: {response.reason}")
 
     async def get(self, endpoint: str, ep_params: Dict = None) -> Result:
         return await self._do(http_method="GET", endpoint=endpoint, ep_params=ep_params)
```

### Comparing `lcwc-0.6/src/lcwc/web/client.py` & `lcwc-0.7/src/lcwc/web/client.py`

 * *Files identical despite different names*

### Comparing `lcwc-0.6/src/lcwc.egg-info/PKG-INFO` & `lcwc-0.7/src/lcwc.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcwc
-Version: 0.6
+Version: 0.7
 Summary: Python library for fetching the Lancaster County-Wide Communications live incident list.
 Author-email: Nate Shoffner <nate.shoffner@gmail.com>
 Project-URL: Homepage, https://github.com/NateShoffner/python-lcwc
 Project-URL: Bug Tracker, https://github.com/NateShoffner/python-lcwc/issues
 Keywords: lcwc,lancaster,police,fire,ems,dispatch,911,incident
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lcwc-0.6/src/lcwc.egg-info/SOURCES.txt` & `lcwc-0.7/src/lcwc.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -15,11 +15,12 @@
 src/lcwc/arcgis/client.py
 src/lcwc/arcgis/incident.py
 src/lcwc/feed/__init__.py
 src/lcwc/feed/client.py
 src/lcwc/feed/incident.py
 src/lcwc/feed/utils/__init__.py
 src/lcwc/utils/__init__.py
+src/lcwc/utils/encoding.py
 src/lcwc/utils/restadapter.py
 src/lcwc/web/__init__.py
 src/lcwc/web/client.py
 src/lcwc/web/incident.py
```

