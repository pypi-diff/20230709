# Comparing `tmp/LTADatamall-0.0.6.tar.gz` & `tmp/LTADatamall-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LTADatamall-0.0.6.tar", last modified: Tue Dec  6 08:24:56 2022, max compression
+gzip compressed data, was "LTADatamall-0.0.7.tar", last modified: Sun Jul  9 09:55:49 2023, max compression
```

## Comparing `LTADatamall-0.0.6.tar` & `LTADatamall-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-12-06 08:24:56.482701 LTADatamall-0.0.6/
-drwxrwxrwx   0        0        0        0 2022-12-06 08:24:56.477388 LTADatamall-0.0.6/LTADatamall/
--rw-rw-rw-   0        0        0      114 2022-10-12 13:22:26.215811 LTADatamall-0.0.6/LTADatamall/__init__.py
--rw-rw-rw-   0        0        0     1454 2022-04-22 08:37:11.000000 LTADatamall-0.0.6/LTADatamall/base.py
--rw-rw-rw-   0        0        0     1714 2022-11-06 14:36:18.791999 LTADatamall-0.0.6/LTADatamall/bus_arrival.py
--rw-rw-rw-   0        0        0     7349 2022-11-07 01:33:07.770746 LTADatamall-0.0.6/LTADatamall/bus_manager.py
--rw-rw-rw-   0        0        0     1071 2022-10-12 13:53:19.927892 LTADatamall-0.0.6/LTADatamall/bus_route.py
--rw-rw-rw-   0        0        0     1066 2022-10-12 13:20:55.305766 LTADatamall-0.0.6/LTADatamall/bus_service.py
--rw-rw-rw-   0        0        0      481 2022-10-12 13:21:09.786052 LTADatamall-0.0.6/LTADatamall/bus_stop.py
--rw-rw-rw-   0        0        0     3011 2022-11-04 04:08:35.730841 LTADatamall-0.0.6/LTADatamall/passenger_volume.py
--rw-rw-rw-   0        0        0     2427 2022-04-23 11:45:05.000000 LTADatamall-0.0.6/LTADatamall/taxi.py
--rw-rw-rw-   0        0        0     1639 2022-04-23 12:03:47.000000 LTADatamall-0.0.6/LTADatamall/train_service_alert.py
--rw-rw-rw-   0        0        0      888 2022-12-06 08:24:56.482976 LTADatamall-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1052 2022-12-06 08:23:49.977521 LTADatamall-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 09:55:49.325787 LTADatamall-0.0.7/
+drwxrwxrwx   0        0        0        0 2023-07-09 09:55:49.324787 LTADatamall-0.0.7/LTADatamall/
+-rw-rw-rw-   0        0        0      114 2022-10-12 13:22:26.215811 LTADatamall-0.0.7/LTADatamall/__init__.py
+-rw-rw-rw-   0        0        0     1454 2022-04-22 08:37:11.000000 LTADatamall-0.0.7/LTADatamall/base.py
+-rw-rw-rw-   0        0        0     1830 2023-07-09 09:49:38.310286 LTADatamall-0.0.7/LTADatamall/bus_arrival.py
+-rw-rw-rw-   0        0        0     7343 2023-07-09 09:45:47.179541 LTADatamall-0.0.7/LTADatamall/bus_manager.py
+-rw-rw-rw-   0        0        0     1071 2022-10-12 13:53:19.927892 LTADatamall-0.0.7/LTADatamall/bus_route.py
+-rw-rw-rw-   0        0        0     1066 2022-10-12 13:20:55.305766 LTADatamall-0.0.7/LTADatamall/bus_service.py
+-rw-rw-rw-   0        0        0      481 2022-10-12 13:21:09.786052 LTADatamall-0.0.7/LTADatamall/bus_stop.py
+-rw-rw-rw-   0        0        0     3011 2022-11-04 04:08:35.730841 LTADatamall-0.0.7/LTADatamall/passenger_volume.py
+-rw-rw-rw-   0        0        0     2427 2022-04-23 11:45:05.000000 LTADatamall-0.0.7/LTADatamall/taxi.py
+-rw-rw-rw-   0        0        0     1639 2022-04-23 12:03:47.000000 LTADatamall-0.0.7/LTADatamall/train_service_alert.py
+-rw-rw-rw-   0        0        0      888 2023-07-09 09:55:49.326788 LTADatamall-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1072 2023-07-09 09:51:20.439850 LTADatamall-0.0.7/setup.py
```

### Comparing `LTADatamall-0.0.6/LTADatamall/base.py` & `LTADatamall-0.0.7/LTADatamall/base.py`

 * *Files identical despite different names*

### Comparing `LTADatamall-0.0.6/LTADatamall/bus_arrival.py` & `LTADatamall-0.0.7/LTADatamall/bus_arrival.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from typing import Union, Callable, Any
+from datetime import datetime
 
 __all__ = (
     'NextBus',
     'BusArrivalService',
 )
 
 class NextBus:
     def __init__(self, **kwargs):
         load_map = {"SEA":"Seats Available", "SDA":"Standing Avaialble", "LSD":"Limited Standing"}
         type_map = {"SD":"Single Decker", "DD":"Double Decker", "BD":"Bendy"}
         self.orgin_code = kwargs.get('OrginCode','Not Available')
         self.destination_code = kwargs.get('DestinationCode','Not Available')
-        self.estimated_arrival = kwargs.get('EstimatedArrival','No Estimated Time')
+        self.estimated_arrival = datetime.strptime(kwargs['EstimatedArrival'],r"%Y-%m-%dT%H:%M:%S%z") if kwargs.get('EstimatedArrival','') != '' else 'No Estimated Time'
         self.latitude = kwargs.get('Latitude',0.0)
         self.longitude = kwargs.get('Longitude',0.0)
         self.visit_number = int(kwargs['VisitNumber']) if kwargs.get('VisitNumber','') != '' else 'Not Available'
         self.load = load_map.get(kwargs.get('Load',None),'Not Available')
         self.feature = "Not Wheel-chair Accessible" if kwargs.get('Feature',"") == "" else "Wheel-chair Accessible"
         self.type = type_map.get(kwargs.get('Type'),'Not Available')
```

### Comparing `LTADatamall-0.0.6/LTADatamall/bus_manager.py` & `LTADatamall-0.0.7/LTADatamall/bus_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
             elif len(routes) == 0:
                 raise Exception('API Returned None')
             break
         return routes
 
     # Bus Stops
     def get_stops(self,bus_stop_codes:Union[int,list[int],str,list[str]]) -> list[BusStop]:
-        all_stops = self.async_get_all_stops()
+        all_stops = self.get_all_stops()
 
         # Query single bus stop either as str or int
         if isinstance(bus_stop_codes, int) or isinstance(bus_stop_codes, str):
             return [BusStop(**i) for i in all_stops if str(i['BusStopCode']) == str(bus_stop_codes)][0]
         # Query list of stops 
         elif iter(bus_stop_codes):
             return [BusStop(**i) for i in all_stops if str(i['BusStopCode']) in list(map(str, bus_stop_codes))]
```

### Comparing `LTADatamall-0.0.6/LTADatamall/bus_route.py` & `LTADatamall-0.0.7/LTADatamall/bus_route.py`

 * *Files identical despite different names*

### Comparing `LTADatamall-0.0.6/LTADatamall/bus_service.py` & `LTADatamall-0.0.7/LTADatamall/bus_service.py`

 * *Files identical despite different names*

### Comparing `LTADatamall-0.0.6/LTADatamall/passenger_volume.py` & `LTADatamall-0.0.7/LTADatamall/passenger_volume.py`

 * *Files identical despite different names*

### Comparing `LTADatamall-0.0.6/LTADatamall/taxi.py` & `LTADatamall-0.0.7/LTADatamall/taxi.py`

 * *Files identical despite different names*

### Comparing `LTADatamall-0.0.6/LTADatamall/train_service_alert.py` & `LTADatamall-0.0.7/LTADatamall/train_service_alert.py`

 * *Files identical despite different names*

### Comparing `LTADatamall-0.0.6/PKG-INFO` & `LTADatamall-0.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: LTADatamall
-Version: 0.0.6
+Version: 0.0.7
 Summary: LTA Datamall API Wrapper
 Home-page: https://github.com/TheReaper62/ltadatamall
 Author: FishballNoodles
 Author-email: joelkhor.work@gmail.com
 License: MIT
-Download-URL: https://github.com/TheReaper62/ltadatamall/archive/refs/tags/v0.0.6.tar.gz
+Download-URL: https://github.com/TheReaper62/ltadatamall/archive/refs/tags/v0.0.7.tar.gz
 Description: UNKNOWN
 Keywords: lta,datamall,bus,timing,arrival,train,service,passenger volume,taxi
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `LTADatamall-0.0.6/setup.py` & `LTADatamall-0.0.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from distutils.core import setup
 setup(
     name='LTADatamall',
     packages=['LTADatamall'],
-    version='0.0.6',
+    version='0.0.7',
     license='MIT',
     description='LTA Datamall API Wrapper',
     author='FishballNoodles',
     author_email='joelkhor.work@gmail.com',
     url='https://github.com/TheReaper62/ltadatamall',
-    download_url='https://github.com/TheReaper62/ltadatamall/archive/refs/tags/v0.0.6.tar.gz',
+    download_url='https://github.com/TheReaper62/ltadatamall/archive/refs/tags/v0.0.7.tar.gz',
     keywords=['lta','datamall','bus','timing','arrival','train','service','passenger volume','taxi'],
     install_requires=[
         'requests',
         'aiohttp',
         'asyncio',
+        'datetime',
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
```

