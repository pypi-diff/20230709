# Comparing `tmp/lmcloud-0.3.7.tar.gz` & `tmp/lmcloud-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmcloud-0.3.7.tar", last modified: Sun Jul  9 12:45:20 2023, max compression
+gzip compressed data, was "lmcloud-0.3.8.tar", last modified: Sun Jul  9 13:50:23 2023, max compression
```

## Comparing `lmcloud-0.3.7.tar` & `lmcloud-0.3.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:45:20.412451 lmcloud-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-09 12:45:02.000000 lmcloud-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-07-09 12:45:20.412451 lmcloud-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-07-09 12:45:02.000000 lmcloud-0.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:45:20.412451 lmcloud-0.3.7/lmcloud/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-09 12:45:02.000000 lmcloud-0.3.7/lmcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-09 12:45:02.000000 lmcloud-0.3.7/lmcloud/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-09 12:45:02.000000 lmcloud-0.3.7/lmcloud/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-07-09 12:45:02.000000 lmcloud-0.3.7/lmcloud/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-07-09 12:45:02.000000 lmcloud-0.3.7/lmcloud/lmbluetooth.py
--rw-r--r--   0 runner    (1001) docker     (123)    23165 2023-07-09 12:45:02.000000 lmcloud-0.3.7/lmcloud/lmcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-07-09 12:45:02.000000 lmcloud-0.3.7/lmcloud/lmlocalapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:45:20.412451 lmcloud-0.3.7/lmcloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-07-09 12:45:20.000000 lmcloud-0.3.7/lmcloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-09 12:45:20.000000 lmcloud-0.3.7/lmcloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 12:45:20.000000 lmcloud-0.3.7/lmcloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-09 12:45:20.000000 lmcloud-0.3.7/lmcloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-09 12:45:20.000000 lmcloud-0.3.7/lmcloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 12:45:20.412451 lmcloud-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-09 12:45:02.000000 lmcloud-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:50:23.701481 lmcloud-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-09 13:50:10.000000 lmcloud-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-07-09 13:50:23.701481 lmcloud-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-07-09 13:50:10.000000 lmcloud-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:50:23.701481 lmcloud-0.3.8/lmcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-09 13:50:10.000000 lmcloud-0.3.8/lmcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-09 13:50:10.000000 lmcloud-0.3.8/lmcloud/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-09 13:50:10.000000 lmcloud-0.3.8/lmcloud/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-07-09 13:50:10.000000 lmcloud-0.3.8/lmcloud/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-07-09 13:50:10.000000 lmcloud-0.3.8/lmcloud/lmbluetooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23367 2023-07-09 13:50:10.000000 lmcloud-0.3.8/lmcloud/lmcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-07-09 13:50:10.000000 lmcloud-0.3.8/lmcloud/lmlocalapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:50:23.701481 lmcloud-0.3.8/lmcloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-07-09 13:50:23.000000 lmcloud-0.3.8/lmcloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-09 13:50:23.000000 lmcloud-0.3.8/lmcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 13:50:23.000000 lmcloud-0.3.8/lmcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-09 13:50:23.000000 lmcloud-0.3.8/lmcloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-09 13:50:23.000000 lmcloud-0.3.8/lmcloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 13:50:23.701481 lmcloud-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-09 13:50:10.000000 lmcloud-0.3.8/setup.py
```

### Comparing `lmcloud-0.3.7/LICENSE` & `lmcloud-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lmcloud-0.3.7/PKG-INFO` & `lmcloud-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: lmcloud
-Version: 0.3.7
+Version: 0.3.8
 Summary: A Python implementation of the new La Marzocco API
 Home-page: https://github.com/zweckj/lmcloud
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # La Marzocco Client
 This is a library to interface with La Marzocco's "new" Home machines (currently only the Micra).
```

### Comparing `lmcloud-0.3.7/README.md` & `lmcloud-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `lmcloud-0.3.7/lmcloud/const.py` & `lmcloud-0.3.8/lmcloud/const.py`

 * *Files identical despite different names*

### Comparing `lmcloud-0.3.7/lmcloud/helpers.py` & `lmcloud-0.3.8/lmcloud/helpers.py`

 * *Files identical despite different names*

### Comparing `lmcloud-0.3.7/lmcloud/lmbluetooth.py` & `lmcloud-0.3.8/lmcloud/lmbluetooth.py`

 * *Files identical despite different names*

### Comparing `lmcloud-0.3.7/lmcloud/lmcloud.py` & `lmcloud-0.3.8/lmcloud/lmcloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,62 +81,35 @@
         return self._statistics
 
     @property
     def schedule(self):
         return schedule_out_to_in(self.config[WEEKLY_SCHEDULING_CONFIG])
     
     @property 
-    def current_status(self):
-        """ 
-        Build object which holds status for lamarzocco Home Assistant Integration
-        """
-
-        state = {
-            "power":                        self.power,
-            "enable_prebrewing":            True if self.config[PRE_INFUSION_SETTINGS]["mode"] == "Enabled" else False,
-            "enable_preinfusion":           True if self.config[PRE_INFUSION_SETTINGS]["mode"] == "TypeB" else False,
-            "steam_boiler_enable":          self.steam_boiler_enabled,
-            "global_auto":                  self.config[WEEKLY_SCHEDULING_CONFIG]["enabled"],
-            "coffee_temp":                  self._config_coffeeboiler[CURRENT],
-            "coffee_set_temp":              self._config_coffeeboiler[TARGET],
-            "steam_temp":                   self._config_steamboiler[CURRENT],
-            "steam_set_temp":               self._config_steamboiler[TARGET],
-            "water_reservoir_contact":      self.config[TANK_STATUS],
-            "plumbin_enable":               self.config[PLUMBED_IN],
-            "drinks_k1":                    self.statistics[0]["count"],
-            "total_flushing":               self.statistics[1]["count"],
-            "date_received:":               self.date_received,
-            "machine_name":                 self.machine_info[MACHINE_NAME],
-            "model_name":                   self.machine_info[MODEL_NAME],
-            "update_available":             self.firmware_version != self.latest_firmware_version,
-            "heating_state":                self.heating_state,
-        }
-
-        doses = parse_doses(self.config)
-        preinfusion_settings = parse_preinfusion_settings(self.config)
-        schedule = schedule_out_to_hass(self.config)
-        return state | doses | preinfusion_settings | schedule
+    def current_status(self) -> dict:
+        return self._current_status
     
 
     '''
     *******************************************
     ***********  Functions ********************
     *******************************************
     '''
 
     def __init__(self):
         _logger.setLevel(logging.DEBUG)
-        self._lm_local_api      = None
-        self._lm_bluetooth      = None
-        self. _config           = {}
-        self. _status           = {}
+        self._lm_local_api         = None
+        self._lm_bluetooth         = None
+        self. _config              = {}
+        self. _status              = {}
+        self._current_status       = {}
         self. _config_steamboiler  = {}
         self. _config_coffeeboiler = {}
-        self. _statistics       = {}
-        self._use_websocket     = False
+        self. _statistics          = {}
+        self._use_websocket        = False
 
 
     @classmethod
     async def create(cls, credentials):
         '''
         Initialize a cloud only client
         '''
@@ -273,14 +246,15 @@
 
         self._config_coffeeboiler = next(item for item in self.config[BOILERS] if item["id"] == COFFEE_BOILER_NAME)
         self._config_steamboiler  = next(item for item in self.config[BOILERS] if item["id"] == STEAM_BOILER_NAME)
 
 
         await self._update_statistics_obj()
         self._date_received = datetime.now()
+        self._current_status = self._build_current_status()
 
 
     async def get_statistics(self):
         '''
         Get statistics
         '''
 
@@ -603,22 +577,24 @@
 
         url = f"{self._gw_url_with_serial}/scheduling"
         data = {"enable": enable, "days": schedule}
         response = await self._rest_api_call(url=url, verb="POST", data=data)
         self._config[WEEKLY_SCHEDULING_CONFIG] = schedule_in_to_out(enable, schedule)
         return response
 
+
     async def set_auto_on_off(self, day_of_week, hour_on, minute_on, hour_off, minute_off):
         schedule = self.schedule
         idx = [index for (index, d) in enumerate(schedule) if d["day"] == day_of_week.upper()][0]
         schedule[idx]["enable"] = True
         schedule[idx]["on"] = f"{hour_on:02d}:{minute_on:02d}"
         schedule[idx]["off"] = f"{hour_off:02d}:{minute_off:02d}"
         return await self.configure_schedule(self.config[WEEKLY_SCHEDULING_CONFIG]["enabled"], schedule)
     
+
     async def set_auto_on_off_enable(self, day_of_week, enable):
         schedule = self.schedule
         idx = [index for (index, d) in enumerate(schedule) if d["day"] == day_of_week.upper()][0]
         schedule[idx]["enable"] = enable
         return await self.configure_schedule(self.config[WEEKLY_SCHEDULING_CONFIG]["enabled"], schedule)
 
 
@@ -629,7 +605,38 @@
         '''
 
         url = f"{self._gw_url_with_serial}/enable-backflush"
         data = {"enable": True}
         response = await self._rest_api_call(url=url, verb="POST", data=data)
         self._config[BACKFLUSH_ENABLED] = True
         return response
+
+    def _build_current_status(self):
+        """ 
+        Build object which holds status for lamarzocco Home Assistant Integration
+        """
+
+        state = {
+            "power":                        self.power,
+            "enable_prebrewing":            True if self.config[PRE_INFUSION_SETTINGS]["mode"] == "Enabled" else False,
+            "enable_preinfusion":           True if self.config[PRE_INFUSION_SETTINGS]["mode"] == "TypeB" else False,
+            "steam_boiler_enable":          self.steam_boiler_enabled,
+            "global_auto":                  self.config[WEEKLY_SCHEDULING_CONFIG]["enabled"],
+            "coffee_temp":                  self._config_coffeeboiler[CURRENT],
+            "coffee_set_temp":              self._config_coffeeboiler[TARGET],
+            "steam_temp":                   self._config_steamboiler[CURRENT],
+            "steam_set_temp":               self._config_steamboiler[TARGET],
+            "water_reservoir_contact":      self.config[TANK_STATUS],
+            "plumbin_enable":               self.config[PLUMBED_IN],
+            "drinks_k1":                    self.statistics[0]["count"],
+            "total_flushing":               self.statistics[1]["count"],
+            "date_received:":               self.date_received,
+            "machine_name":                 self.machine_info[MACHINE_NAME],
+            "model_name":                   self.machine_info[MODEL_NAME],
+            "update_available":             self.firmware_version != self.latest_firmware_version,
+            "heating_state":                self.heating_state,
+        }
+
+        doses = parse_doses(self.config)
+        preinfusion_settings = parse_preinfusion_settings(self.config)
+        schedule = schedule_out_to_hass(self.config)
+        return state | doses | preinfusion_settings | schedule
```

### Comparing `lmcloud-0.3.7/lmcloud/lmlocalapi.py` & `lmcloud-0.3.8/lmcloud/lmlocalapi.py`

 * *Files identical despite different names*

### Comparing `lmcloud-0.3.7/lmcloud.egg-info/PKG-INFO` & `lmcloud-0.3.8/lmcloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: lmcloud
-Version: 0.3.7
+Version: 0.3.8
 Summary: A Python implementation of the new La Marzocco API
 Home-page: https://github.com/zweckj/lmcloud
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # La Marzocco Client
 This is a library to interface with La Marzocco's "new" Home machines (currently only the Micra).
```

### Comparing `lmcloud-0.3.7/setup.py` & `lmcloud-0.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import setuptools
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setuptools.setup(
     name="lmcloud",
-    version="0.3.7",
+    version="0.3.8",
     description="A Python implementation of the new La Marzocco API",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/zweckj/lmcloud",
     author="Josef Zweck",
     author_email="24647999+zweckj@users.noreply.github.com",
     license="MIT",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: Implementation :: CPython",
     ],
     packages=setuptools.find_packages(),
     install_requires=["httpx>=0.16.1", "authlib>=0.15.5,<1.0", "aiohttp>=3.8.4", "websockets>=11.0.2", "bleak>=0.20.2"],
     package_data={
         "license": ["LICENSE"],
     },
```

