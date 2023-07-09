# Comparing `tmp/lmcloud-0.3.6.tar.gz` & `tmp/lmcloud-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmcloud-0.3.6.tar", last modified: Sat Jul  8 12:25:18 2023, max compression
+gzip compressed data, was "lmcloud-0.3.7.tar", last modified: Sun Jul  9 12:45:20 2023, max compression
```

## Comparing `lmcloud-0.3.6.tar` & `lmcloud-0.3.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:25:18.830167 lmcloud-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-08 12:25:02.000000 lmcloud-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-07-08 12:25:18.830167 lmcloud-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-07-08 12:25:02.000000 lmcloud-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:25:18.830167 lmcloud-0.3.6/lmcloud/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-08 12:25:02.000000 lmcloud-0.3.6/lmcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-08 12:25:02.000000 lmcloud-0.3.6/lmcloud/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-08 12:25:02.000000 lmcloud-0.3.6/lmcloud/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-08 12:25:02.000000 lmcloud-0.3.6/lmcloud/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-07-08 12:25:02.000000 lmcloud-0.3.6/lmcloud/lmbluetooth.py
--rw-r--r--   0 runner    (1001) docker     (123)    22549 2023-07-08 12:25:02.000000 lmcloud-0.3.6/lmcloud/lmcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-07-08 12:25:02.000000 lmcloud-0.3.6/lmcloud/lmlocalapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:25:18.830167 lmcloud-0.3.6/lmcloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-07-08 12:25:18.000000 lmcloud-0.3.6/lmcloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-08 12:25:18.000000 lmcloud-0.3.6/lmcloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 12:25:18.000000 lmcloud-0.3.6/lmcloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-08 12:25:18.000000 lmcloud-0.3.6/lmcloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 12:25:18.000000 lmcloud-0.3.6/lmcloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 12:25:18.830167 lmcloud-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-08 12:25:02.000000 lmcloud-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:45:20.412451 lmcloud-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-09 12:45:02.000000 lmcloud-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-07-09 12:45:20.412451 lmcloud-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-07-09 12:45:02.000000 lmcloud-0.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:45:20.412451 lmcloud-0.3.7/lmcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-09 12:45:02.000000 lmcloud-0.3.7/lmcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-09 12:45:02.000000 lmcloud-0.3.7/lmcloud/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-09 12:45:02.000000 lmcloud-0.3.7/lmcloud/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-07-09 12:45:02.000000 lmcloud-0.3.7/lmcloud/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-07-09 12:45:02.000000 lmcloud-0.3.7/lmcloud/lmbluetooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23165 2023-07-09 12:45:02.000000 lmcloud-0.3.7/lmcloud/lmcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-07-09 12:45:02.000000 lmcloud-0.3.7/lmcloud/lmlocalapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:45:20.412451 lmcloud-0.3.7/lmcloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-07-09 12:45:20.000000 lmcloud-0.3.7/lmcloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-09 12:45:20.000000 lmcloud-0.3.7/lmcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 12:45:20.000000 lmcloud-0.3.7/lmcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-09 12:45:20.000000 lmcloud-0.3.7/lmcloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-09 12:45:20.000000 lmcloud-0.3.7/lmcloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 12:45:20.412451 lmcloud-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-09 12:45:02.000000 lmcloud-0.3.7/setup.py
```

### Comparing `lmcloud-0.3.6/LICENSE` & `lmcloud-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lmcloud-0.3.6/PKG-INFO` & `lmcloud-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmcloud
-Version: 0.3.6
+Version: 0.3.7
 Summary: A Python implementation of the new La Marzocco API
 Home-page: https://github.com/zweckj/lmcloud
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `lmcloud-0.3.6/README.md` & `lmcloud-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `lmcloud-0.3.6/lmcloud/const.py` & `lmcloud-0.3.7/lmcloud/const.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 GW_MACHINE_BASE_URL = "https://gw-lmz.lamarzocco.io/v1/home/machines"
 
 POLLING_DELAY_S = 20
 POLLING_DELAY_STATISTICS_S = 60
 
 MODEL_LMU = "Micra"
 
+BT_MODEL_NAMES = [
+    "MICRA",
+    "MINI",
+    "GS3"
+]
+
 # Key Names for Dictionaries
 KEY = "key"
 SERIAL_NUMBER = "serial_number"
 MACHINE_NAME = "machine_name"
 MODEL_NAME = "model_name"
 
 # Dict keys are camel case for local API, all upper for remote API
```

### Comparing `lmcloud-0.3.6/lmcloud/lmbluetooth.py` & `lmcloud-0.3.7/lmcloud/lmbluetooth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 import base64
 import logging
 from bleak import BleakScanner, BleakClient, BLEDevice, BleakError
 from .exceptions import BluetoothDeviceNotFound
-from .const import SETTINGS_CHARACTERISTIC, AUTH_CHARACTERISTIC, MODEL_LMU
+from .const import SETTINGS_CHARACTERISTIC, AUTH_CHARACTERISTIC, BT_MODEL_NAMES
 
 _logger = logging.getLogger(__name__)
 
 
 class LMBluetooth:
     """
     class to interact with machine via Bluetooth
@@ -42,15 +42,15 @@
     async def discover_device(self, scanner):
         """
         find machine
         """
         devices = await scanner.discover()
         for d in devices:
             if d.name:
-                if MODEL_LMU.upper() in d.name:
+                if d.name.startswith(tuple(BT_MODEL_NAMES)):
                     self._address = d.address
                     self._name = d.name
 
     async def write_bluetooth_message(self, message, characteristic: str):
         """
         connect to machine and write a message
         """
```

### Comparing `lmcloud-0.3.6/lmcloud/lmcloud.py` & `lmcloud-0.3.7/lmcloud/lmcloud.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,98 +23,102 @@
         self._client = value
 
     @property
     def machine_info(self):
         return self._machine_info
 
     @property
-    def model_name(self):
+    def model_name(self) -> str:
         return self._machine_info[MODEL_NAME]
     
     @property 
-    def firmware_version(self):
+    def firmware_version(self) -> str:
         return self._firmware["machine_firmware"]["version"]
+    
+    @property
+    def latest_firmware_version(self) -> str:
+        return self._firmware["machine_firmware"]["targetVersion"]
+    
+    @property
+    def date_received(self):
+        return self._date_received
 
     @property
     def config(self):
         """ 
         Return the config with capitalized keys to be consistent across local/remote APIs 
         """
-
         return self._config
     
     @property
+    def power(self) -> bool:
+        return True if self.config[MACHINE_MODE] == "BrewingMode" else False
+    
+    @property 
+    def steam_boiler_enabled(self) -> bool:
+        return self._config_steamboiler["isEnabled"]
+    
+    @property
+    def is_heating(self) -> bool:
+        coffee_heating = (float(self._config_coffeeboiler["current"]) < float(self._config_coffeeboiler["target"])) \
+            and self.power 
+        steam_heating = float(self._config_steamboiler["current"]) < float(self._config_steamboiler["target"]) \
+            and self.power and self.steam_boiler_enabled
+        return coffee_heating or steam_heating
+    
+    @property 
+    def heating_state(self) -> list:
+        return [
+            "heating_on" if self.power else "heating_off",
+            "steam_heater_on" if self.steam_boiler_enabled else "steam_heater_off"
+        ]
+
+    @property
     def status(self):
         return self._status
     
     @property
     def statistics(self):
         return self._statistics
+
+    @property
+    def schedule(self):
+        return schedule_out_to_in(self.config[WEEKLY_SCHEDULING_CONFIG])
     
     @property 
     def current_status(self):
         """ 
         Build object which holds status for lamarzocco Home Assistant Integration
         """
 
-        return {
-            "power": True if self.config[MACHINE_MODE] == "BrewingMode" else False,
-            "enable_prebrewing": True if self.config[PRE_INFUSION_SETTINGS]["mode"] == "Enabled" else False,
-            "enable_preinfusion": True if self.config[PRE_INFUSION_SETTINGS]["mode"] == "TypeB" else False,
-            "steam_boiler_enable": self._config_steamboiler["isEnabled"],
-            "global_auto": self.config[WEEKLY_SCHEDULING_CONFIG]["enabled"],
-            "coffee_temp": self._config_coffeeboiler[CURRENT],
-            "coffee_set_temp": self._config_coffeeboiler[TARGET],
-            "steam_temp": self._config_steamboiler[CURRENT],
-            "steam_set_temp": self._config_steamboiler[TARGET],
-            "water_reservoir_contact": self.config[TANK_STATUS],
-            "plumbin_enable": self.config[PLUMBED_IN],
-            "drinks_k1":        self.statistics[0]["count"],
-            "total_flushing":   self.statistics[1]["count"]
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
         }
 
-
-    '''
-    *******************************************
-    ***  Getters for current machine state ****
-    *******************************************
-    '''
-
-    # will return current machine mode (Brewing/StandBy)
-    async def get_machine_mode(self):
-        await self.update_local_machine_status()
-        return self.config[MACHINE_MODE]
-
-    async def get_coffee_boiler_enabled(self):
-        await self.update_local_machine_status()
-        return self._config_coffeeboiler["isEnabled"]
-
-    async def get_steam_boiler_enabled(self):
-        await self.update_local_machine_status()
-        return self._config_steamboiler["isEnabled"]
-
-    async def get_coffee_temp(self):
-        await self.update_local_machine_status()
-        return self.config[BOILER_TARGET_TEMP][COFFEE_BOILER_NAME]
-
-    async def get_steam_temp(self):
-        await self.update_local_machine_status()
-        return self.config[BOILER_TARGET_TEMP][STEAM_BOILER_NAME]
-
-    async def get_plumbin_enabled(self):
-        await self.update_local_machine_status()
-        return self.config[PLUMBED_IN]
-
-    async def get_preinfusion_settings(self):
-        await self.update_local_machine_status()
-        return self.config[PRE_INFUSION_SETTINGS]
-
-    async def get_schedule(self):
-        await self.update_local_machine_status()
-        return schedule_out_to_in(self.config[WEEKLY_SCHEDULING_CONFIG])
+        doses = parse_doses(self.config)
+        preinfusion_settings = parse_preinfusion_settings(self.config)
+        schedule = schedule_out_to_hass(self.config)
+        return state | doses | preinfusion_settings | schedule
     
 
     '''
     *******************************************
     ***********  Functions ********************
     *******************************************
     '''
@@ -147,27 +151,28 @@
 
     @classmethod
     async def create_with_local_api(cls, credentials, ip, port=8081, use_websocket=False, use_bluetooth=False, bluetooth_scanner=None):
         '''
         Also initialize a local API client
         '''
         self = cls()
-        self.init_with_local_api(credentials, ip, port, use_websocket, use_bluetooth, bluetooth_scanner)
+        await self.init_with_local_api(credentials, ip, port, use_websocket, use_bluetooth, bluetooth_scanner)
 
         await self.update_local_machine_status(in_init=True)
         return self
     
 
     async def init_with_local_api(self, credentials, ip, port=8081, use_websocket=False, use_bluetooth=False, bluetooth_scanner=None):
         ''' init where data is loaded '''
         self.client = await self._connect(credentials)
         self._machine_info = await self._get_machine_info()
         self._lm_local_api = LMLocalAPI(local_ip=ip, local_port=port, local_bearer=self.machine_info[KEY])
         self._gw_url_with_serial = GW_MACHINE_BASE_URL + "/" + self.machine_info[SERIAL_NUMBER]
         self._firmware = await self.get_firmware()
+        self._date_received = datetime.now()
 
         # init websockets if set
         if use_websocket:
             self._use_websocket = True
             asyncio.create_task(self._lm_local_api.websocket_connect())
 
         # init bluetooth if set
@@ -267,14 +272,15 @@
             await self._update_config_obj()     
 
         self._config_coffeeboiler = next(item for item in self.config[BOILERS] if item["id"] == COFFEE_BOILER_NAME)
         self._config_steamboiler  = next(item for item in self.config[BOILERS] if item["id"] == STEAM_BOILER_NAME)
 
 
         await self._update_statistics_obj()
+        self._date_received = datetime.now()
 
 
     async def get_statistics(self):
         '''
         Get statistics
         '''
 
@@ -464,15 +470,15 @@
         Enable/Disable Pre-Brew or Pre-Infusion (mutually exclusive)
         '''
 
         if mode != "Disabled" and mode != "TypeB" and mode != "Enabled":
             msg = "Pre-Infusion/Pre-Brew can only be TypeB (PreInfusion), Enabled (Pre-Brew) or Disabled"
             _logger.debug(msg)
             raise ValueError(msg)
-        elif mode == "TypedB" and not (await self.get_plumbin_enabled()):
+        elif mode == "TypedB" and not self.config[PLUMBED_IN]:
             msg = "Pre-Infusion can only be enabled when plumbin is enabled"
             _logger.debug(msg)
             raise ValueError(msg)
         else:
             url = f"{self._gw_url_with_serial}/enable-preinfusion"
             data = {"mode": mode}
             response = await self._rest_api_call(url=url, verb="POST", data=data)
@@ -598,23 +604,23 @@
         url = f"{self._gw_url_with_serial}/scheduling"
         data = {"enable": enable, "days": schedule}
         response = await self._rest_api_call(url=url, verb="POST", data=data)
         self._config[WEEKLY_SCHEDULING_CONFIG] = schedule_in_to_out(enable, schedule)
         return response
 
     async def set_auto_on_off(self, day_of_week, hour_on, minute_on, hour_off, minute_off):
-        schedule = await self.get_schedule()
+        schedule = self.schedule
         idx = [index for (index, d) in enumerate(schedule) if d["day"] == day_of_week.upper()][0]
         schedule[idx]["enable"] = True
         schedule[idx]["on"] = f"{hour_on:02d}:{minute_on:02d}"
         schedule[idx]["off"] = f"{hour_off:02d}:{minute_off:02d}"
         return await self.configure_schedule(self.config[WEEKLY_SCHEDULING_CONFIG]["enabled"], schedule)
     
     async def set_auto_on_off_enable(self, day_of_week, enable):
-        schedule = await self.get_schedule()
+        schedule = self.schedule
         idx = [index for (index, d) in enumerate(schedule) if d["day"] == day_of_week.upper()][0]
         schedule[idx]["enable"] = enable
         return await self.configure_schedule(self.config[WEEKLY_SCHEDULING_CONFIG]["enabled"], schedule)
 
 
 
     async def start_backflush(self):
```

### Comparing `lmcloud-0.3.6/lmcloud/lmlocalapi.py` & `lmcloud-0.3.7/lmcloud/lmlocalapi.py`

 * *Files identical despite different names*

### Comparing `lmcloud-0.3.6/lmcloud.egg-info/PKG-INFO` & `lmcloud-0.3.7/lmcloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmcloud
-Version: 0.3.6
+Version: 0.3.7
 Summary: A Python implementation of the new La Marzocco API
 Home-page: https://github.com/zweckj/lmcloud
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `lmcloud-0.3.6/setup.py` & `lmcloud-0.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setuptools.setup(
     name="lmcloud",
-    version="0.3.6",
+    version="0.3.7",
     description="A Python implementation of the new La Marzocco API",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/zweckj/lmcloud",
     author="Josef Zweck",
     author_email="24647999+zweckj@users.noreply.github.com",
     license="MIT",
```

