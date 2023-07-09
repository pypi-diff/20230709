# Comparing `tmp/LTADatamall-0.0.7.tar.gz` & `tmp/LTADatamall-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LTADatamall-0.0.7.tar", last modified: Sun Jul  9 09:55:49 2023, max compression
+gzip compressed data, was "LTADatamall-0.0.8.tar", last modified: Sun Jul  9 11:20:39 2023, max compression
```

## Comparing `LTADatamall-0.0.7.tar` & `LTADatamall-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 09:55:49.325787 LTADatamall-0.0.7/
-drwxrwxrwx   0        0        0        0 2023-07-09 09:55:49.324787 LTADatamall-0.0.7/LTADatamall/
--rw-rw-rw-   0        0        0      114 2022-10-12 13:22:26.215811 LTADatamall-0.0.7/LTADatamall/__init__.py
--rw-rw-rw-   0        0        0     1454 2022-04-22 08:37:11.000000 LTADatamall-0.0.7/LTADatamall/base.py
--rw-rw-rw-   0        0        0     1830 2023-07-09 09:49:38.310286 LTADatamall-0.0.7/LTADatamall/bus_arrival.py
--rw-rw-rw-   0        0        0     7343 2023-07-09 09:45:47.179541 LTADatamall-0.0.7/LTADatamall/bus_manager.py
--rw-rw-rw-   0        0        0     1071 2022-10-12 13:53:19.927892 LTADatamall-0.0.7/LTADatamall/bus_route.py
--rw-rw-rw-   0        0        0     1066 2022-10-12 13:20:55.305766 LTADatamall-0.0.7/LTADatamall/bus_service.py
--rw-rw-rw-   0        0        0      481 2022-10-12 13:21:09.786052 LTADatamall-0.0.7/LTADatamall/bus_stop.py
--rw-rw-rw-   0        0        0     3011 2022-11-04 04:08:35.730841 LTADatamall-0.0.7/LTADatamall/passenger_volume.py
--rw-rw-rw-   0        0        0     2427 2022-04-23 11:45:05.000000 LTADatamall-0.0.7/LTADatamall/taxi.py
--rw-rw-rw-   0        0        0     1639 2022-04-23 12:03:47.000000 LTADatamall-0.0.7/LTADatamall/train_service_alert.py
--rw-rw-rw-   0        0        0      888 2023-07-09 09:55:49.326788 LTADatamall-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1072 2023-07-09 09:51:20.439850 LTADatamall-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 11:20:39.386620 LTADatamall-0.0.8/
+drwxrwxrwx   0        0        0        0 2023-07-09 11:20:39.386620 LTADatamall-0.0.8/LTADatamall/
+-rw-rw-rw-   0        0        0      114 2022-10-12 13:22:26.215811 LTADatamall-0.0.8/LTADatamall/__init__.py
+-rw-rw-rw-   0        0        0     1454 2023-07-09 10:22:21.116926 LTADatamall-0.0.8/LTADatamall/base.py
+-rw-rw-rw-   0        0        0     2326 2023-07-09 11:07:28.895084 LTADatamall-0.0.8/LTADatamall/bus_arrival.py
+-rw-rw-rw-   0        0        0     7343 2023-07-09 10:27:12.194195 LTADatamall-0.0.8/LTADatamall/bus_manager.py
+-rw-rw-rw-   0        0        0     1071 2023-07-09 10:27:46.830674 LTADatamall-0.0.8/LTADatamall/bus_route.py
+-rw-rw-rw-   0        0        0     1066 2023-07-09 10:28:02.064605 LTADatamall-0.0.8/LTADatamall/bus_service.py
+-rw-rw-rw-   0        0        0      481 2023-07-09 10:28:17.650348 LTADatamall-0.0.8/LTADatamall/bus_stop.py
+-rw-rw-rw-   0        0        0     3015 2023-07-09 10:27:12.194195 LTADatamall-0.0.8/LTADatamall/passenger_volume.py
+-rw-rw-rw-   0        0        0     2427 2023-07-09 10:28:48.376594 LTADatamall-0.0.8/LTADatamall/taxi.py
+-rw-rw-rw-   0        0        0     1639 2023-07-09 10:25:28.451140 LTADatamall-0.0.8/LTADatamall/train_service_alert.py
+-rw-rw-rw-   0        0        0      888 2023-07-09 11:20:39.387942 LTADatamall-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1072 2023-07-09 11:20:35.797691 LTADatamall-0.0.8/setup.py
```

### Comparing `LTADatamall-0.0.7/LTADatamall/base.py` & `LTADatamall-0.0.8/LTADatamall/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from typing import Any
 
 from aiohttp import ClientSession, ClientConnectorError
 from requests import Session, exceptions
 
 class DataFrame:
     def __init__(self, API_KEY:str):
-        self.BASE_URL = "http://datamall2.mytransport.sg/ltaodataservice"
-        self.HEADERS = {"Accept": "application/json", "AccountKey": API_KEY}
+        self.BASE_URL = 'http://datamall2.mytransport.sg/ltaodataservice'
+        self.HEADERS = {'Accept': 'application/json', 'AccountKey': API_KEY}
 
     def send(self, path, params:dict[str,Any]={}, json:dict[str,Any]={}):
         with Session() as session:
             try:
-                response = session.get(self.BASE_URL+"/"+path, params=params, headers=self.HEADERS,json=json)
+                response = session.get(self.BASE_URL+'/'+path, params=params, headers=self.HEADERS,json=json)
                 if response.status_code == 200:
                     return response.json()
                 else:
                     raise Exception(f"An Error Occured: {response.reason}")
             except exceptions.RequestException as error:
                 raise Exception(str(error)) from None
 
     async def async_send(self, path, params:dict[str,Any]={}, json:dict[str,Any]={}):
         async with ClientSession() as session:
             try:
-                async with session.get(self.BASE_URL+"/"+path, params=params, headers=self.HEADERS, json=json) as response:
+                async with session.get(self.BASE_URL+'/'+path, params=params, headers=self.HEADERS, json=json) as response:
                     if response.status == 200:
                         return await response.json()
                     else:
                         raise Exception(f"An Error Occured: {response.reason}")
             except ClientConnectorError as error:
                 raise Exception(str(error)) from None
```

### Comparing `LTADatamall-0.0.7/LTADatamall/bus_manager.py` & `LTADatamall-0.0.8/LTADatamall/bus_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,111 +16,111 @@
         super().__init__(API_KEY)
 
     # Bus Arrival
     def get_bus_arrival(self, bus_stop_code: Union[str, int, BusStop], service_no: Optional[Union[str, int]] = None) -> list[BusArrivalService]:
         params = {'BusStopCode': bus_stop_code} if not isinstance(bus_stop_code,BusStop) else {'BusStopCode': bus_stop_code.bus_stop_code}
         if service_no != None:
             params['ServiceNo'] = service_no
-        response = self.send("BusArrivalv2", params=params)
+        response = self.send('BusArrivalv2', params=params)
         if response.get('Services', False):
             return [BusArrivalService(**i) for i in response['Services']]
-        raise Exception('API Returned None')
+        raise Exception("API Returned None")
 
     async def async_get_bus_arrival(self, bus_stop_code: Union[str, int, BusStop], service_no: Optional[Union[str, int]] = None) -> list[BusArrivalService]:
         params = {'BusStopCode': bus_stop_code} if not isinstance(bus_stop_code,BusStop) else {'BusStopCode': bus_stop_code.bus_stop_code}
         if service_no != None:
             params['ServiceNo'] = service_no
-        response = await self.async_send("BusArrivalv2", params=params)
+        response = await self.async_send('BusArrivalv2', params=params)
         if response.get('Services', False):
             return [BusArrivalService(**i) for i in response['Services']]
-        raise Exception('API Returned None')
+        raise Exception("API Returned None")
 
     # Bus Services
     def get_services(self, services: list[Union[str, int]] = []) -> list[BusService]:
-        response = self.send("BusServices")
+        response = self.send('BusServices')
         if response.get('value', False):
             return [BusService(**i) for i in response['value'] if i['ServiceNo'] in list(map(str, services))]
-        raise Exception('API Returned None')
+        raise Exception("API Returned None")
 
     async def async_get_services(self, services: list[Union[str, int]] = []) -> list[BusService]:
-        response = await self.async_send("BusServices")
+        response = await self.async_send('BusServices')
         if response.get('value', False):
             return [BusService(**i) for i in response['value'] if i['ServiceNo'] in list(map(str, services))]
-        raise Exception('API Returned None')
+        raise Exception("API Returned None")
 
     def get_all_services(self) -> list[BusService]:
         services = []
         while len(services)%500 == 0:
-            response = self.send('BusServices',params={"$skip":len(services)})
+            response = self.send('BusServices',params={'$skip':len(services)})
             if response.get('value', False):
                 services.extend([BusService(**i) for i in response['value']])
                 continue
             elif len(services) == 0:
-                raise Exception('API Returned None')
+                raise Exception("API Returned None")
             break
         return services
 
     def async_get_all_services(self) -> list[BusService]:
         services = []
         while len(services)%500 == 0:
-            response = self.async_send('BuServices',params={"$skip":len(services)})
+            response = self.async_send('BuServices',params={'$skip':len(services)})
             if response.get('value', False):
                 services.extend([BusService(**i) for i in response['value']])
                 continue
             elif len(services) == 0:
-                raise Exception('API Returned None')
+                raise Exception("API Returned None")
             break
         return services
 
     # Bus Routes
     def get_routes(self, **filters) -> list[BusRoute]:
         response = self.send('BusRoute')
 
         def processed_filter(raw_dict: dict[str, Any]) -> bool:
             for key, value in filters.items():
                 if raw_dict.get(key, None) != value:
                     return False
             return True
         if response.get('value', False):
             return [BusRoute(**i) for i in response['value'] if processed_filter(i)]
-        raise Exception('API Returned None')
+        raise Exception("API Returned None")
 
     async def async_get_routes(self, **filters) -> list[BusRoute]:
         response = await self.async_send('BusRoute')
 
         def processed_filter(raw_dict: dict[str, Any]) -> bool:
             for key, value in filters.items():
                 if raw_dict.get(key, None) != value:
                     return False
             return True
         if response.get('value', False):
             return [BusRoute(**i) for i in response['value'] if processed_filter(i)]
-        raise Exception('API Returned None')
+        raise Exception("API Returned None")
 
     def get_all_routes(self) -> list[BusRoute]:
         routes = []
         while len(routes)%500 == 0:
-            response = self.send('BusRoutes',params={"$skip":len(routes)})
+            response = self.send('BusRoutes',params={'$skip':len(routes)})
             if response.get('value', False):
                 routes.extend([BusRoute(**i) for i in response['value']])
                 continue
             elif len(routes) == 0:
-                raise Exception('API Returned None')
+                raise Exception("API Returned None")
             break
         return routes
 
     def async_get_all_routes(self) -> list[BusRoute]:
         routes = []
         while len(routes)%500 == 0:
-            response = self.async_send('BusRoutes',params={"$skip":len(routes)})
+            response = self.async_send('BusRoutes',params={'$skip':len(routes)})
             if response.get('value', False):
                 routes.extend([BusRoute(**i) for i in response['value']])
                 continue
             elif len(routes) == 0:
-                raise Exception('API Returned None')
+                raise Exception("API Returned None")
             break
         return routes
 
     # Bus Stops
     def get_stops(self,bus_stop_codes:Union[int,list[int],str,list[str]]) -> list[BusStop]:
         all_stops = self.get_all_stops()
 
@@ -139,27 +139,27 @@
         # Query list of stops 
         elif iter(bus_stop_codes):
             return [BusStop(**i) for i in all_stops if str(i['BusStopCode']) in list(map(str,bus_stop_codes))]
 
     def get_all_stops(self) -> list[BusStop]:
         stops = []
         while len(stops)%500 == 0:
-            response = self.send('BusStops',params={"$skip":len(stops)})
+            response = self.send('BusStops',params={'$skip':len(stops)})
             if response.get('value', False):
                 stops.extend([BusStop(**i) for i in response['value']])
                 continue
             elif len(stops) == 0:
-                raise Exception('API Returned None')
+                raise Exception("API Returned None")
             break
         return stops
 
     def async_get_all_stops(self) -> list[BusStop]:
         stops = []
         while len(stops)%500 == 0:
-            response = self.async_send('BusStops',params={"$skip":len(stops)})
+            response = self.async_send('BusStops',params={'$skip':len(stops)})
             if response.get('value', False):
                 stops.extend([BusStop(**i) for i in response['value']])
                 continue
             elif len(stops) == 0:
-                raise Exception('API Returned None')
+                raise Exception("API Returned None")
             break
         return stops
```

### Comparing `LTADatamall-0.0.7/LTADatamall/bus_route.py` & `LTADatamall-0.0.8/LTADatamall/bus_route.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 
 __all__ = (
     'BusRoute',
 )
 
 class BusRoute:
     def __init__(self, **kwargs):
-        operator_map = {"SBST": "SBS Transit",
-                        "SMRT": "SMRT Corporation",
-                        "TTS": "Tower Transit Singapore",
-                        "GAS": "Go Ahead Singapore"}
+        operator_map = {'SBST': "SBS Transit",
+                        'SMRT': "SMRT Corporation",
+                        'TTS': "Tower Transit Singapore",
+                        'GAS': "Go Ahead Singapore"}
         self.service_no = kwargs.get('ServiceNo',None)
         self.operator = kwargs.get('Operator',None)
         self.direction = kwargs.get('Direction',None)
         self.stop_sequence = kwargs.get('StopSequence',None)
         self.bus_stop_code = kwargs.get('BusStopCode',None)
         self.distance = kwargs.get('Distance',None)
         self.wd_firstbus = kwargs.get('WD_FirstBus',None)
```

### Comparing `LTADatamall-0.0.7/LTADatamall/bus_service.py` & `LTADatamall-0.0.8/LTADatamall/bus_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 
 __all__ = (
     'BusService',
 )
 
 class BusService:
     def __init__(self, **kwargs):
-        operator_map = {"SBST": "SBS Transit",
-                        "SMRT": "SMRT Corporation",
-                        "TTS": "Tower Transit Singapore",
-                        "GAS": "Go Ahead Singapore"}
-        self.service_no = kwargs.get("ServiceNo",None)
-        self.operator = operator_map.get(kwargs.get("Operator",None),'Not Available')
-        self.direction = kwargs.get("Direction",None)
-        self.category = kwargs.get("Category",None)
-        self.origin_code = kwargs.get("OriginCode",None)
-        self.destination_code = kwargs.get("DestinationCode",None)
-        self.am_peak_freq = kwargs.get("AM_Peak_Freq",None)
-        self.am_offpeak_freq = kwargs.get("AM_Offpeak_Freq",None)
-        self.pm_peak_freq = kwargs.get("PM_Peak_Freq",None)
-        self.pm_offpeak_freq = kwargs.get("PM_Offpeak_Freq",None)
-        self.loop_desc = kwargs.get("LoopDesc",None)
+        operator_map = {'SBST': "SBS Transit",
+                        'SMRT': "SMRT Corporation",
+                        'TTS': "Tower Transit Singapore",
+                        'GAS': "Go Ahead Singapore"}
+        self.service_no = kwargs.get('ServiceNo',None)
+        self.operator = operator_map.get(kwargs.get('Operator',None),"Not Available")
+        self.direction = kwargs.get('Direction',None)
+        self.category = kwargs.get('Category',None)
+        self.origin_code = kwargs.get('OriginCode',None)
+        self.destination_code = kwargs.get('DestinationCode',None)
+        self.am_peak_freq = kwargs.get('AM_Peak_Freq',None)
+        self.am_offpeak_freq = kwargs.get('AM_Offpeak_Freq',None)
+        self.pm_peak_freq = kwargs.get('PM_Peak_Freq',None)
+        self.pm_offpeak_freq = kwargs.get('PM_Offpeak_Freq',None)
+        self.loop_desc = kwargs.get('LoopDesc',None)
```

### Comparing `LTADatamall-0.0.7/LTADatamall/passenger_volume.py` & `LTADatamall-0.0.8/LTADatamall/passenger_volume.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,72 +5,72 @@
 __all__ = (
     'PassengerVolume',
 )
 
 class PassengerVolume(DataFrame):
     def __init__(self, api_key: str):
         super().__init__(api_key)
-    '''
+        '''
         date:str (YYYYMM)
-        Example : "201912"
+        Example : '201912'
         Up to Last 3 Months
         '''
 
     # By Bus Stop
-    def pv_bus_stop(self, date: str = "") -> str:
-        params = {"Date": date} if date != "" else {}
+    def pv_bus_stop(self, date: str = '') -> str:
+        params = {'Date': date} if date != '' else {}
         response = self.send('PV/Bus', params=params)
         if response.get('value', False):
-            return response.get('Link', 'Not Available')
-        raise Exception('API Returned None')
+            return response.get('Link', "Not Available")
+        raise Exception("API Returned None")
 
-    async def async_pv_bus_stop(self, date: str ="") -> str:
-        params = {"Date": date} if date != "" else {}
+    async def async_pv_bus_stop(self, date: str ='') -> str:
+        params = {'Date': date} if date != '' else {}
         response = await self.async_send('PV/Bus', params=params)
         if response.get('value', False):
-            return response.get('Link', 'Not Available')
-        raise Exception('API Returned None')
+            return response.get('Link', "Not Available")
+        raise Exception("API Returned None")
 
     # By Orgin Destination Bus Stops
-    def pv_od_bus_stop(self, date: str ="") -> str:
-        params = {"Date": date} if date != "" else {}
+    def pv_od_bus_stop(self, date: str ='') -> str:
+        params = {'Date': date} if date != '' else {}
         response = self.send('PV/ODBus', params=params)
         if response.get('value', False):
-            return response.get('Link', 'Not Available')
-        raise Exception('API Returned None')
+            return response.get('Link', "Not Available")
+        raise Exception("API Returned None")
 
-    async def async_pv_od_bus_stop(self, date: str ="") -> str:
-        params = {"Date": date} if date != "" else {}
+    async def async_pv_od_bus_stop(self, date: str ='') -> str:
+        params = {'Date': date} if date != '' else {}
         response = await self.async_send('PV/ODBus', params=params)
         if response.get('value', False):
-            return response.get('Link', 'Not Available')
-        raise Exception('API Returned None')
+            return response.get('Link', "Not Available")
+        raise Exception("API Returned None")
 
     # By Orgin Destination Train Stations
-    def pv_od_train_destination(self, date: str ="") -> str:
-        params = {"Date": date} if date != "" else {}
+    def pv_od_train_destination(self, date: str ='') -> str:
+        params = {'Date': date} if date != '' else {}
         response = self.send('PV/ODTrain', params=params)
         if response.get('value', False):
-            return response.get('Link', 'Not Available')
-        raise Exception('API Returned None')
+            return response.get('Link', "Not Available")
+        raise Exception("API Returned None")
 
-    async def async_pv_od_train_destination(self, date: str ="") -> str:
-        params = {"Date": date} if date != "" else {}
+    async def async_pv_od_train_destination(self, date: str ='') -> str:
+        params = {'Date': date} if date != '' else {}
         response = await self.async_send('PV/ODTrain', params=params)
         if response.get('value', False):
-            return response.get('Link', 'Not Available')
-        raise Exception('API Returned None')
+            return response.get('Link', "Not Available")
+        raise Exception("API Returned None")
 
     # By Train Stations
-    def pv_od_train_destination(self, date: str ="") -> str:
-        params = {"Date": date} if date != "" else {}
+    def pv_od_train_destination(self, date: str ='') -> str:
+        params = {'Date': date} if date != '' else {}
         response = self.send('PV/Train', params=params)
         if response.get('value', False):
-            return response.get('Link', 'Not Available')
-        raise Exception('API Returned None')
+            return response.get('Link', "Not Available")
+        raise Exception("API Returned None")
 
-    async def async_pv_od_train_destination(self, date: str ="") -> str:
-        params = {"Date": date} if date != "" else {}
+    async def async_pv_od_train_destination(self, date: str ='') -> str:
+        params = {'Date': date} if date != '' else {}
         response = await self.async_send('PV/Train', params=params)
         if response.get('value', False):
-            return response.get('Link', 'Not Available')
-        raise Exception('API Returned None')
+            return response.get('Link', "Not Available")
+        raise Exception("API Returned None")
```

### Comparing `LTADatamall-0.0.7/LTADatamall/taxi.py` & `LTADatamall-0.0.8/LTADatamall/taxi.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,51 +12,51 @@
     def __init__(self,**kwargs):
         self.latitude = float(kwargs.get('Latitude',0))
         self.longitude = float(kwargs.get('Longitude',0))
 
 class TaxiStand:
     def __init__(self,**kwargs):
         ownership_map = {
-            "LTA" : "Land Transport Authority",
-            "CCS" : "Clear Channel Singapore",
-            "Private" : "Private",
+            'LTA' : "Land Transport Authority",
+            'CCS' : "Clear Channel Singapore",
+            'Private' : "Private",
         }
-        self.taxi_code = kwargs.get('TaxiCode', 'Not Available')
+        self.taxi_code = kwargs.get('TaxiCode', "Not Available")
         self.latitude = float(kwargs.get('Latitude',0))
         self.longitude = float(kwargs.get('Longitude',0))
-        self.bfa = kwargs.get('Bfa','Not Available')
-        self.ownership = ownership_map.get(kwargs.get('Ownership',None),'Not Available')
-        self.type = kwargs.get('Type','Not Available')
-        self.name = kwargs.get('Name','Not Available')
+        self.bfa = kwargs.get('Bfa',"Not Available")
+        self.ownership = ownership_map.get(kwargs.get('Ownership',None),"Not Available")
+        self.type = kwargs.get('Type',"Not Available")
+        self.name = kwargs.get('Name',"Not Available")
 
 class TaxiManager(DataFrame):
     def __init__(self, api_key: str):
         super().__init__(api_key)
 
     # Available Taxis
     def get_availability(self):
         response = self.send('Taxi-Availability')
         if response.get('value',False):
             return [AvailableTaxi(**i) for i in response['value']]
-        raise Exception('API Returned None')
+        raise Exception("API Returned None")
 
     async def async_get_availability(self):
         response = await self.async_send('Taxi-Availability')
         if response.get('value',False):
             return [AvailableTaxi(**i) for i in response['value']]
-        raise Exception('API Returned None')
+        raise Exception("API Returned None")
 
     # Taxi Stands
     def get_taxi_stands(self,taxi_codes:Union[str,list[str]]=[]):
         response = self.send('TaxiStands')
         taxi_codes = [taxi_codes] if not isinstance(taxi_codes,(tuple,list)) else taxi_codes
         if response.get('value',False):
             return [TaxiStand(**i) for i in response['value'] if i['TaxiCode'] in taxi_codes and taxi_codes!=[]]
-        raise Exception('API Returned None')
+        raise Exception("API Returned None")
 
     async def async_get_taxi_stands(self, taxi_codes: Union[str, list[str]] = []):
         response = await self.async_send('TaxiStands')
         taxi_codes = [taxi_codes] if not isinstance(
             taxi_codes, (tuple, list)) else taxi_codes
         if response.get('value', False):
             return [TaxiStand(**i) for i in response['value'] if i['TaxiCode'] in taxi_codes and taxi_codes != []]
-        raise Exception('API Returned None')
+        raise Exception("API Returned None")
```

### Comparing `LTADatamall-0.0.7/LTADatamall/train_service_alert.py` & `LTADatamall-0.0.8/LTADatamall/train_service_alert.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,36 +3,36 @@
 __all = (
     'TrainServiceAlertManager',
     'TrainServiceAlert'
 )
 
 class TrainServiceAlert:
     def __init__(self,**kwargs):
-        self.status = kwargs.get('Status','Not Available')
-        self.line = kwargs.get('Line','Not Available')
-        self.direction = kwargs.get('Direction','Not Available')
+        self.status = kwargs.get('Status',"Not Available")
+        self.line = kwargs.get('Line',"Not Available")
+        self.direction = kwargs.get('Direction',"Not Available")
         self.stations = kwargs.get('Stations',None)
         self.free_public_bus = kwargs.get('FreePublicBus',None)
         self.free_mrt_shuttle = kwargs.get('FreeMRTShuttle',None)
-        self.mrt_shuttle_direction = kwargs.get('MRTShuttleDirection','Not Available')
-        self.message = kwargs.get('Message','No Message')
+        self.mrt_shuttle_direction = kwargs.get('MRTShuttleDirection',"Not Available")
+        self.message = kwargs.get('Message',"No Message")
 
         self.stations = self.stations.split(',') if self.stations!=None else "Not Available"
         self.free_public_bus = self.free_public_bus.split(',') if self.free_public_bus!=None else "Not Available"
         self.free_mrt_shuttle = self.free_mrt_shuttle.split(',') if self.free_mrt_shuttle!=None else "Not Available"
 
 class TrainServiceAlertManager(DataFrame):
     def __init__(self, api_key: str):
         super().__init__(api_key)
 
     # Get Alerts 
     def get_alerts(self) -> str:
         response = self.send('TrainServiceAlerts')
         if response.get('value', False):
             return [TrainServiceAlert(**alert) for alert in response['value']]
-        raise Exception('API Returned None')
+        raise Exception("API Returned None")
 
     async def async_get_alerts(self) -> str:
         response = self.async_send('TrainServiceAlerts')
         if response.get('value', False):
             return [TrainServiceAlert(**alert) for alert in response['value']]
-        raise Exception('API Returned None')
+        raise Exception("API Returned None")
```

### Comparing `LTADatamall-0.0.7/PKG-INFO` & `LTADatamall-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: LTADatamall
-Version: 0.0.7
+Version: 0.0.8
 Summary: LTA Datamall API Wrapper
 Home-page: https://github.com/TheReaper62/ltadatamall
 Author: FishballNoodles
 Author-email: joelkhor.work@gmail.com
 License: MIT
-Download-URL: https://github.com/TheReaper62/ltadatamall/archive/refs/tags/v0.0.7.tar.gz
+Download-URL: https://github.com/TheReaper62/ltadatamall/archive/refs/tags/v0.0.8.tar.gz
 Description: UNKNOWN
 Keywords: lta,datamall,bus,timing,arrival,train,service,passenger volume,taxi
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `LTADatamall-0.0.7/setup.py` & `LTADatamall-0.0.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
     name='LTADatamall',
     packages=['LTADatamall'],
-    version='0.0.7',
+    version='0.0.8',
     license='MIT',
     description='LTA Datamall API Wrapper',
     author='FishballNoodles',
     author_email='joelkhor.work@gmail.com',
     url='https://github.com/TheReaper62/ltadatamall',
-    download_url='https://github.com/TheReaper62/ltadatamall/archive/refs/tags/v0.0.7.tar.gz',
+    download_url='https://github.com/TheReaper62/ltadatamall/archive/refs/tags/v0.0.8.tar.gz',
     keywords=['lta','datamall','bus','timing','arrival','train','service','passenger volume','taxi'],
     install_requires=[
         'requests',
         'aiohttp',
         'asyncio',
         'datetime',
     ],
```

