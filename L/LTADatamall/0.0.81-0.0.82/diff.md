# Comparing `tmp/LTADatamall-0.0.81.tar.gz` & `tmp/LTADatamall-0.0.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LTADatamall-0.0.81.tar", last modified: Sun Jul  9 11:33:28 2023, max compression
+gzip compressed data, was "LTADatamall-0.0.82.tar", last modified: Sun Jul  9 12:44:06 2023, max compression
```

## Comparing `LTADatamall-0.0.81.tar` & `LTADatamall-0.0.82.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 11:33:28.314671 LTADatamall-0.0.81/
-drwxrwxrwx   0        0        0        0 2023-07-09 11:33:28.313671 LTADatamall-0.0.81/LTADatamall/
--rw-rw-rw-   0        0        0      114 2022-10-12 13:22:26.215811 LTADatamall-0.0.81/LTADatamall/__init__.py
--rw-rw-rw-   0        0        0     1454 2023-07-09 10:22:21.116926 LTADatamall-0.0.81/LTADatamall/base.py
--rw-rw-rw-   0        0        0     2392 2023-07-09 11:32:53.999952 LTADatamall-0.0.81/LTADatamall/bus_arrival.py
--rw-rw-rw-   0        0        0     7343 2023-07-09 10:27:12.194195 LTADatamall-0.0.81/LTADatamall/bus_manager.py
--rw-rw-rw-   0        0        0     1071 2023-07-09 10:27:46.830674 LTADatamall-0.0.81/LTADatamall/bus_route.py
--rw-rw-rw-   0        0        0     1066 2023-07-09 10:28:02.064605 LTADatamall-0.0.81/LTADatamall/bus_service.py
--rw-rw-rw-   0        0        0      481 2023-07-09 10:28:17.650348 LTADatamall-0.0.81/LTADatamall/bus_stop.py
--rw-rw-rw-   0        0        0     3015 2023-07-09 10:27:12.194195 LTADatamall-0.0.81/LTADatamall/passenger_volume.py
--rw-rw-rw-   0        0        0     2427 2023-07-09 10:28:48.376594 LTADatamall-0.0.81/LTADatamall/taxi.py
--rw-rw-rw-   0        0        0     1639 2023-07-09 10:25:28.451140 LTADatamall-0.0.81/LTADatamall/train_service_alert.py
--rw-rw-rw-   0        0        0      890 2023-07-09 11:33:28.315676 LTADatamall-0.0.81/PKG-INFO
--rw-rw-rw-   0        0        0     1074 2023-07-09 11:33:18.206622 LTADatamall-0.0.81/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 12:44:06.851473 LTADatamall-0.0.82/
+drwxrwxrwx   0        0        0        0 2023-07-09 12:44:06.850474 LTADatamall-0.0.82/LTADatamall/
+-rw-rw-rw-   0        0        0      114 2022-10-12 13:22:26.215811 LTADatamall-0.0.82/LTADatamall/__init__.py
+-rw-rw-rw-   0        0        0     1454 2023-07-09 10:22:21.116926 LTADatamall-0.0.82/LTADatamall/base.py
+-rw-rw-rw-   0        0        0     2400 2023-07-09 12:43:53.597309 LTADatamall-0.0.82/LTADatamall/bus_arrival.py
+-rw-rw-rw-   0        0        0     7343 2023-07-09 10:27:12.194195 LTADatamall-0.0.82/LTADatamall/bus_manager.py
+-rw-rw-rw-   0        0        0     1071 2023-07-09 10:27:46.830674 LTADatamall-0.0.82/LTADatamall/bus_route.py
+-rw-rw-rw-   0        0        0     1066 2023-07-09 10:28:02.064605 LTADatamall-0.0.82/LTADatamall/bus_service.py
+-rw-rw-rw-   0        0        0      481 2023-07-09 10:28:17.650348 LTADatamall-0.0.82/LTADatamall/bus_stop.py
+-rw-rw-rw-   0        0        0     3015 2023-07-09 10:27:12.194195 LTADatamall-0.0.82/LTADatamall/passenger_volume.py
+-rw-rw-rw-   0        0        0     2427 2023-07-09 10:28:48.376594 LTADatamall-0.0.82/LTADatamall/taxi.py
+-rw-rw-rw-   0        0        0     1639 2023-07-09 10:25:28.451140 LTADatamall-0.0.82/LTADatamall/train_service_alert.py
+-rw-rw-rw-   0        0        0      890 2023-07-09 12:44:06.851473 LTADatamall-0.0.82/PKG-INFO
+-rw-rw-rw-   0        0        0     1074 2023-07-09 12:44:00.285369 LTADatamall-0.0.82/setup.py
```

### Comparing `LTADatamall-0.0.81/LTADatamall/base.py` & `LTADatamall-0.0.82/LTADatamall/base.py`

 * *Files identical despite different names*

### Comparing `LTADatamall-0.0.81/LTADatamall/bus_arrival.py` & `LTADatamall-0.0.82/LTADatamall/bus_arrival.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,12 +40,12 @@
         self.next_1: NextBus = NextBus(**kwargs.get('NextBus',{}))
         self.next_2: NextBus = NextBus(**kwargs.get('NextBus2',{}))
         self.next_3: NextBus = NextBus(**kwargs.get('NextBus3',{}))
         self.secs_to_arrival : Optional[int] = None
         if self.next_1.estimated_arrival == "No Estimated Time":
             self.secs_to_arrival = None
         secs_to_arrival = self.next_1.estimated_arrival - timezone('Asia/Singapore').localize(datetime.now())
-        if secs_to_arrival.days != -1:
+        if secs_to_arrival.days == -1:
             self.secs_to_arrival = 0
         else:
-            self.secs_to_arrival = secs_to_arrival
+            self.secs_to_arrival = secs_to_arrival.seconds
```

### Comparing `LTADatamall-0.0.81/LTADatamall/bus_manager.py` & `LTADatamall-0.0.82/LTADatamall/bus_manager.py`

 * *Files identical despite different names*

### Comparing `LTADatamall-0.0.81/LTADatamall/bus_route.py` & `LTADatamall-0.0.82/LTADatamall/bus_route.py`

 * *Files identical despite different names*

### Comparing `LTADatamall-0.0.81/LTADatamall/bus_service.py` & `LTADatamall-0.0.82/LTADatamall/bus_service.py`

 * *Files identical despite different names*

### Comparing `LTADatamall-0.0.81/LTADatamall/passenger_volume.py` & `LTADatamall-0.0.82/LTADatamall/passenger_volume.py`

 * *Files identical despite different names*

### Comparing `LTADatamall-0.0.81/LTADatamall/taxi.py` & `LTADatamall-0.0.82/LTADatamall/taxi.py`

 * *Files identical despite different names*

### Comparing `LTADatamall-0.0.81/LTADatamall/train_service_alert.py` & `LTADatamall-0.0.82/LTADatamall/train_service_alert.py`

 * *Files identical despite different names*

### Comparing `LTADatamall-0.0.81/PKG-INFO` & `LTADatamall-0.0.82/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: LTADatamall
-Version: 0.0.81
+Version: 0.0.82
 Summary: LTA Datamall API Wrapper
 Home-page: https://github.com/TheReaper62/ltadatamall
 Author: FishballNoodles
 Author-email: joelkhor.work@gmail.com
 License: MIT
-Download-URL: https://github.com/TheReaper62/ltadatamall/archive/refs/tags/v0.0.81.tar.gz
+Download-URL: https://github.com/TheReaper62/ltadatamall/archive/refs/tags/v0.0.82.tar.gz
 Description: UNKNOWN
 Keywords: lta,datamall,bus,timing,arrival,train,service,passenger volume,taxi
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `LTADatamall-0.0.81/setup.py` & `LTADatamall-0.0.82/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
     name='LTADatamall',
     packages=['LTADatamall'],
-    version='0.0.81',
+    version='0.0.82',
     license='MIT',
     description='LTA Datamall API Wrapper',
     author='FishballNoodles',
     author_email='joelkhor.work@gmail.com',
     url='https://github.com/TheReaper62/ltadatamall',
-    download_url='https://github.com/TheReaper62/ltadatamall/archive/refs/tags/v0.0.81.tar.gz',
+    download_url='https://github.com/TheReaper62/ltadatamall/archive/refs/tags/v0.0.82.tar.gz',
     keywords=['lta','datamall','bus','timing','arrival','train','service','passenger volume','taxi'],
     install_requires=[
         'requests',
         'aiohttp',
         'asyncio',
         'datetime',
     ],
```

