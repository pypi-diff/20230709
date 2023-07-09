# Comparing `tmp/comwatt-client-0.1.1.tar.gz` & `tmp/comwatt-client-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comwatt-client-0.1.1.tar", last modified: Sat Jul  8 14:20:00 2023, max compression
+gzip compressed data, was "comwatt-client-0.1.2.tar", last modified: Sun Jul  9 08:01:46 2023, max compression
```

## Comparing `comwatt-client-0.1.1.tar` & `comwatt-client-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 mat       (1000) mat       (1000)        0 2023-07-08 14:20:00.526389 comwatt-client-0.1.1/
--rw-rw-r--   0 mat       (1000) mat       (1000)      549 2023-07-08 14:20:00.526389 comwatt-client-0.1.1/PKG-INFO
--rw-rw-r--   0 mat       (1000) mat       (1000)     2706 2023-07-08 13:38:01.000000 comwatt-client-0.1.1/README.rst
-drwxrwxr-x   0 mat       (1000) mat       (1000)        0 2023-07-08 14:20:00.526389 comwatt-client-0.1.1/comwatt_client.egg-info/
--rw-rw-r--   0 mat       (1000) mat       (1000)      549 2023-07-08 14:20:00.000000 comwatt-client-0.1.1/comwatt_client.egg-info/PKG-INFO
--rw-rw-r--   0 mat       (1000) mat       (1000)      238 2023-07-08 14:20:00.000000 comwatt-client-0.1.1/comwatt_client.egg-info/SOURCES.txt
--rw-rw-r--   0 mat       (1000) mat       (1000)        1 2023-07-08 14:20:00.000000 comwatt-client-0.1.1/comwatt_client.egg-info/dependency_links.txt
--rw-rw-r--   0 mat       (1000) mat       (1000)        9 2023-07-08 14:20:00.000000 comwatt-client-0.1.1/comwatt_client.egg-info/requires.txt
--rw-rw-r--   0 mat       (1000) mat       (1000)        4 2023-07-08 14:20:00.000000 comwatt-client-0.1.1/comwatt_client.egg-info/top_level.txt
--rw-rw-r--   0 mat       (1000) mat       (1000)       38 2023-07-08 14:20:00.526389 comwatt-client-0.1.1/setup.cfg
--rw-rw-r--   0 mat       (1000) mat       (1000)      649 2023-07-08 14:19:32.000000 comwatt-client-0.1.1/setup.py
-drwxrwxr-x   0 mat       (1000) mat       (1000)        0 2023-07-08 14:20:00.526389 comwatt-client-0.1.1/src/
--rw-rw-r--   0 mat       (1000) mat       (1000)        0 2023-07-08 13:37:30.000000 comwatt-client-0.1.1/src/__init__.py
--rw-rw-r--   0 mat       (1000) mat       (1000)     6043 2023-07-08 14:02:41.000000 comwatt-client-0.1.1/src/client.py
+drwxrwxr-x   0 mat       (1000) mat       (1000)        0 2023-07-09 08:01:46.720739 comwatt-client-0.1.2/
+-rw-rw-r--   0 mat       (1000) mat       (1000)      549 2023-07-09 08:01:46.720739 comwatt-client-0.1.2/PKG-INFO
+-rw-rw-r--   0 mat       (1000) mat       (1000)     2998 2023-07-08 21:27:06.000000 comwatt-client-0.1.2/README.md
+drwxrwxr-x   0 mat       (1000) mat       (1000)        0 2023-07-09 08:01:46.716740 comwatt-client-0.1.2/comwatt-client/
+-rw-rw-r--   0 mat       (1000) mat       (1000)        0 2023-07-08 13:37:30.000000 comwatt-client-0.1.2/comwatt-client/__init__.py
+-rw-rw-r--   0 mat       (1000) mat       (1000)     7281 2023-07-08 21:26:46.000000 comwatt-client-0.1.2/comwatt-client/client.py
+drwxrwxr-x   0 mat       (1000) mat       (1000)        0 2023-07-09 08:01:46.716740 comwatt-client-0.1.2/comwatt_client.egg-info/
+-rw-rw-r--   0 mat       (1000) mat       (1000)      549 2023-07-09 08:01:46.000000 comwatt-client-0.1.2/comwatt_client.egg-info/PKG-INFO
+-rw-rw-r--   0 mat       (1000) mat       (1000)      259 2023-07-09 08:01:46.000000 comwatt-client-0.1.2/comwatt_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 mat       (1000) mat       (1000)        1 2023-07-09 08:01:46.000000 comwatt-client-0.1.2/comwatt_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 mat       (1000) mat       (1000)        9 2023-07-09 08:01:46.000000 comwatt-client-0.1.2/comwatt_client.egg-info/requires.txt
+-rw-rw-r--   0 mat       (1000) mat       (1000)       15 2023-07-09 08:01:46.000000 comwatt-client-0.1.2/comwatt_client.egg-info/top_level.txt
+-rw-rw-r--   0 mat       (1000) mat       (1000)       38 2023-07-09 08:01:46.720739 comwatt-client-0.1.2/setup.cfg
+-rw-rw-r--   0 mat       (1000) mat       (1000)      649 2023-07-09 08:01:07.000000 comwatt-client-0.1.2/setup.py
```

### Comparing `comwatt-client-0.1.1/PKG-INFO` & `comwatt-client-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comwatt-client
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python Client for Comwatt API
 Home-page: UNKNOWN
 Author: Matéo Greil
 Author-email: contact@greil.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `comwatt-client-0.1.1/README.rst` & `comwatt-client-0.1.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -6,17 +6,19 @@
 ## Features
 The client currently supports the following methods:
 
 - `authenticate(self, username, password)`: Authenticates a user with the provided username and password.
 - `get_authenticated_user(self)`: Retrieves information about the authenticated user.
 - `get_sites(self)`: Retrieves a list of sites associated with the authenticated user.
 - `get_site_networks_ts_time_ago(self, site_id, measure_kind = "VIRTUAL_QUANTITY", aggregation_level = "HOUR", aggregation_type = "SUM", time_ago_unit = "DAY", time_ago_value = 1)`: Retrieves the time series data for the networks of a specific site, based on the provided parameters.
+- `get_site_consumption_breakdown_time_ago(self, site_id, aggregation_level = "HOUR", time_ago_unit = "DAY", time_ago_value = 1)` Retrieves the consumption breakdown data for a specific site, based on the provided parameters.
 - `get_devices(self, site_id)`: Retrieves a list of devices for the specified site.
 - `get_device_ts_time_ago(self, device_id, measure_kind = "FLOW", aggregation_level = "HOUR", aggregation_type = "MAX", time_ago_unit = "DAY", time_ago_value = "1")`: Retrieves the time series data for a specific device, based on the provided parameters.
 
+
 ## Installation
 You can install the Comwatt Python Client using pip. Run the following command:
 
 ```
 pip install comwatt-client
 ```
 
@@ -26,31 +28,32 @@
 ```python
 from comwatt.client import ComwattClient
 
 # Create a Comwatt client instance
 client = ComwattClient()
 
 # Authenticate the user
-# Password should be encrypted password,
-# I don't know exactly what the encryption is for the moment,
-# so you will need to encrypt it from their webapp
 client.authenticate('username', 'password')
 
 # Get information about the authenticated user
 user_info = client.get_authenticated_user()
 print(user_info)
 
 # Get a list of sites associated with the authenticated user
 sites = client.get_sites()
 print(sites)
 
 # Get time series data for the networks of a specific site
 networks_time_series_data = client.get_site_networks_ts_time_ago(sites[0]['id'])
 print(networks_time_series_data)
 
+# Get the consumption breakdown data for a specific site, based on the provided parameters.
+consumption_breakdown_data = client.get_site_consumption_breakdown_time_ago(sites[0]['id'])
+print(consumption_breakdown_data)
+
 # Get a list of devices for a specific site
 devices = client.get_devices(sites[0]['id'])
 print(devices)
 
 # Get time series data for a specific device
 time_series_data = client.get_device_ts_time_ago(devices[0]['id'])
 print(time_series_data)
```

### Comparing `comwatt-client-0.1.1/comwatt_client.egg-info/PKG-INFO` & `comwatt-client-0.1.2/comwatt_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comwatt-client
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python Client for Comwatt API
 Home-page: UNKNOWN
 Author: Matéo Greil
 Author-email: contact@greil.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `comwatt-client-0.1.1/setup.py` & `comwatt-client-0.1.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='comwatt-client',
-    version='0.1.1',
+    version='0.1.2',
     author='Matéo Greil',
     author_email='contact@greil.fr',
     description='Python Client for Comwatt API',
     packages=find_packages(),
     install_requires=[
         'requests',
     ],
```

### Comparing `comwatt-client-0.1.1/src/client.py` & `comwatt-client-0.1.2/comwatt-client/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import requests
 import json
+import hashlib
 
 class ComwattClient:
     """
     A client for interacting with the Comwatt API.
 
     Args:
         None
@@ -13,34 +14,33 @@
         session (requests.Session): The session object for making HTTP requests.
 
     """
     def __init__(self):
         self.base_url = 'https://energy.comwatt.com/api'
         self.session = requests.Session()
 
-    # Password should be encrypted password, I don't know exactly what the encryption is for the
-    # moment, so you will need to encrypt it from their webapp
     def authenticate(self, username, password):
         """
         Authenticates a user with the provided username and password.
 
         Args:
             username (str): The username of the user.
-            password (str): The password of the user (encrypted).
+            password (str): The password of the user.
 
         Returns:
             None
 
         Raises:
             Exception: If the authentication fails.
 
         """
 
         url = f'{self.base_url}/v1/authent'
-        data = {'username': username, 'password': password}
+        encoded_password = hashlib.sha256(f'jbjaonfusor_{password}_4acuttbuik9'.encode()).hexdigest()
+        data = {'username': username, 'password': encoded_password}
 
         response = self.session.post(url, json=data)
 
         if response.status_code != 200:
             raise Exception(f'Authentication failed: {response.status_code}')
 
     def get_authenticated_user(self):
@@ -60,15 +60,15 @@
 
         url = f'{self.base_url}/users/authenticated'
 
         response = self.session.get(url)
         if response.status_code == 200:
             return response.json()
         else:
-            raise Exception(f'Error retrieving authenticated user: {response.sttaus_code}')
+            raise Exception(f'Error retrieving authenticated user: {response.status_code}')
 
     def get_sites(self):
         """
         Retrieves a list of sites associated with the authenticated user.
 
         Args:
             None
@@ -83,105 +83,141 @@
 
         url = f'{self.base_url}/sites'
 
         response = self.session.get(url)
         if response.status_code == 200:
             return response.json()
         else:
-            raise Exception(f'Error retrieving sites: {response.sttaus_code}')
+            raise Exception(f'Error retrieving sites: {response.status_code}')
 
-    def get_devices(self, site_id):
+
+    def get_site_networks_ts_time_ago(self, site_id,
+            measure_kind = "FLOW",
+            aggregation_level = "NONE",
+            aggregation_type = None,
+            time_ago_unit = "HOUR",
+            time_ago_value = 1):
         """
-        Retrieves a list of devices for the specified site.
+        Retrieves the time series data for the networks of a specific site, based on the provided parameters.
 
         Args:
             site_id (str): The ID of the site.
+            measure_kind (str): The kind of measure (default: "VIRTUAL_QUANTITY").
+            aggregation_level (str): The aggregation level (default: "HOUR").
+            aggregation_type (str): The aggregation type (default: None, can be : None, "SUM", "MAX").
+            time_ago_unit (str): The unit of time ago (default: "DAY").
+            time_ago_value (int): The value of time ago (default: 1).
 
         Returns:
-            list: A list of devices.
+            dict: The time series data.
 
         Raises:
-            Exception: If an error occurs while retrieving the devices.
+            Exception: If an error occurs while retrieving the data.
 
         """
 
-        url = f'{self.base_url}/devices?siteId={site_id}'
+        url = (f'{self.base_url}/aggregations/site-networks-ts-time-ago?'
+               f'siteId={site_id}&'
+               f'measureKind={measure_kind}&'
+               f'aggregationLevel={aggregation_level}&'
+               f'timeAgoUnit={time_ago_unit}&'
+               f'timeAgoValue={time_ago_value}')
+
+        if aggregation_type != None:
+            url += f'&aggregationType={aggregation_type}'
 
         response = self.session.get(url)
         if response.status_code == 200:
             return response.json()
         else:
-            raise Exception(f'Error retrieving sites: {response.sttaus_code}')
+            raise Exception(f'Error retrieving aggregations: {response.status_code}')
 
-    def get_device_ts_time_ago(self, device_id,
-            measure_kind = "FLOW",
+    def get_site_consumption_breakdown_time_ago(self, site_id,
             aggregation_level = "HOUR",
-            aggregation_type = "MAX",
             time_ago_unit = "DAY",
-            time_ago_value = "1"):
+            time_ago_value = 1):
         """
-        Retrieves the time series data for a specific device, based on the provided parameters.
+        Retrieves the consumption breakdown data for a specific site, based on the provided parameters.
 
         Args:
-            device_id (str): The ID of the device.
-            measure_kind (str): The kind of measure (default: "FLOW").
+            site_id (str): The ID of the site.
             aggregation_level (str): The aggregation level (default: "HOUR").
-            aggregation_type (str): The aggregation type (default: "MAX").
             time_ago_unit (str): The unit of time ago (default: "DAY").
-            time_ago_value (str): The value of time ago (default: "1").
+            time_ago_value (int): The value of time ago (default: 1).
 
         Returns:
-            dict: The time series data.
+            dict: The consumption breakdown data.
 
         Raises:
             Exception: If an error occurs while retrieving the data.
 
         """
 
-        url = (f'{self.base_url}/aggregations/device-ts-time-ago?'
-               f'deviceId={device_id}&'
-               f'measureKind={measure_kind}&'
-               f'aggregationLevel={aggregation_level}&'
-               f'aggregationType={aggregation_type}&'
-               f'timeAgoUnit={time_ago_unit}&'
-               f'timeAgoValue={time_ago_value}')
+        url = (f'{self.base_url}/aggregations/consumption-breakdown-time-ago?'
+                f'siteId={site_id}&'
+                f'aggregationLevel={aggregation_level}&'
+                f'timeAgoUnit={time_ago_unit}&'
+                f'timeAgoValue={time_ago_value}')
 
         response = self.session.get(url)
         if response.status_code == 200:
             return response.json()
         else:
             raise Exception(f'Error retrieving aggregations: {response.status_code}')
 
-    def get_site_networks_ts_time_ago(self, site_id,
-            measure_kind = "VIRTUAL_QUANTITY",
+    def get_devices(self, site_id):
+        """
+        Retrieves a list of devices for the specified site.
+
+        Args:
+            site_id (str): The ID of the site.
+
+        Returns:
+            list: A list of devices.
+
+        Raises:
+            Exception: If an error occurs while retrieving the devices.
+
+        """
+
+        url = f'{self.base_url}/devices?siteId={site_id}'
+
+        response = self.session.get(url)
+        if response.status_code == 200:
+            return response.json()
+        else:
+            raise Exception(f'Error retrieving sites: {response.status_code}')
+
+    def get_device_ts_time_ago(self, device_id,
+            measure_kind = "FLOW",
             aggregation_level = "HOUR",
-            aggregation_type = "SUM",
+            aggregation_type = "MAX",
             time_ago_unit = "DAY",
-            time_ago_value = 1):
+            time_ago_value = "1"):
         """
-        Retrieves the time series data for the networks of a specific site, based on the provided parameters.
+        Retrieves the time series data for a specific device, based on the provided parameters.
 
         Args:
-            site_id (str): The ID of the site.
-            measure_kind (str): The kind of measure (default: "VIRTUAL_QUANTITY").
+            device_id (str): The ID of the device.
+            measure_kind (str): The kind of measure (default: "FLOW").
             aggregation_level (str): The aggregation level (default: "HOUR").
-            aggregation_type (str): The aggregation type (default: "SUM").
+            aggregation_type (str): The aggregation type (default: "MAX").
             time_ago_unit (str): The unit of time ago (default: "DAY").
-            time_ago_value (int): The value of time ago (default: 1).
+            time_ago_value (str): The value of time ago (default: "1").
 
         Returns:
             dict: The time series data.
 
         Raises:
             Exception: If an error occurs while retrieving the data.
 
         """
 
-        url = (f'{self.base_url}/aggregations/site-networks-ts-time-ago?'
-               f'siteId={site_id}&'
+        url = (f'{self.base_url}/aggregations/device-ts-time-ago?'
+               f'deviceId={device_id}&'
                f'measureKind={measure_kind}&'
                f'aggregationLevel={aggregation_level}&'
                f'aggregationType={aggregation_type}&'
                f'timeAgoUnit={time_ago_unit}&'
                f'timeAgoValue={time_ago_value}')
 
         response = self.session.get(url)
```

