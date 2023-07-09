# Comparing `tmp/petkitaio-0.1.6.tar.gz` & `tmp/petkitaio-0.1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petkitaio-0.1.6.tar", last modified: Thu Jul  6 18:48:07 2023, max compression
+gzip compressed data, was "petkitaio-0.1.6.1.tar", last modified: Sun Jul  9 20:04:05 2023, max compression
```

## Comparing `petkitaio-0.1.6.tar` & `petkitaio-0.1.6.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-07-06 18:48:07.393586 petkitaio-0.1.6/
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1067 2023-07-06 18:44:46.000000 petkitaio-0.1.6/LICENSE
--rw-r--r--   0 robertdrinovac   (501) staff       (20)     6153 2023-07-06 18:48:07.393803 petkitaio-0.1.6/PKG-INFO
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     4546 2023-07-06 18:44:46.000000 petkitaio-0.1.6/README.md
-drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-07-06 18:48:07.391261 petkitaio-0.1.6/petkitaio/
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1904 2023-07-06 18:44:46.000000 petkitaio-0.1.6/petkitaio/__init__.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)    10730 2023-07-06 18:44:46.000000 petkitaio-0.1.6/petkitaio/constants.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)      835 2023-07-06 18:44:46.000000 petkitaio-0.1.6/petkitaio/exceptions.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1392 2023-07-06 18:44:46.000000 petkitaio-0.1.6/petkitaio/model.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)    43295 2023-07-06 18:44:46.000000 petkitaio-0.1.6/petkitaio/petkit_client.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)      680 2023-07-06 18:44:46.000000 petkitaio-0.1.6/petkitaio/str_enum.py
-drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-07-06 18:48:07.393282 petkitaio-0.1.6/petkitaio.egg-info/
--rw-r--r--   0 robertdrinovac   (501) staff       (20)     6153 2023-07-06 18:48:07.000000 petkitaio-0.1.6/petkitaio.egg-info/PKG-INFO
--rw-r--r--   0 robertdrinovac   (501) staff       (20)      337 2023-07-06 18:48:07.000000 petkitaio-0.1.6/petkitaio.egg-info/SOURCES.txt
--rw-r--r--   0 robertdrinovac   (501) staff       (20)        1 2023-07-06 18:48:07.000000 petkitaio-0.1.6/petkitaio.egg-info/dependency_links.txt
--rw-r--r--   0 robertdrinovac   (501) staff       (20)       28 2023-07-06 18:48:07.000000 petkitaio-0.1.6/petkitaio.egg-info/requires.txt
--rw-r--r--   0 robertdrinovac   (501) staff       (20)       10 2023-07-06 18:48:07.000000 petkitaio-0.1.6/petkitaio.egg-info/top_level.txt
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)       38 2023-07-06 18:48:07.394341 petkitaio-0.1.6/setup.cfg
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1050 2023-07-06 18:44:46.000000 petkitaio-0.1.6/setup.py
+drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-07-09 20:04:05.159901 petkitaio-0.1.6.1/
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1067 2023-07-09 19:59:24.000000 petkitaio-0.1.6.1/LICENSE
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)     6155 2023-07-09 20:04:05.160115 petkitaio-0.1.6.1/PKG-INFO
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     4546 2023-07-09 19:59:24.000000 petkitaio-0.1.6.1/README.md
+drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-07-09 20:04:05.157588 petkitaio-0.1.6.1/petkitaio/
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1904 2023-07-09 19:59:24.000000 petkitaio-0.1.6.1/petkitaio/__init__.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)    10807 2023-07-09 19:59:24.000000 petkitaio-0.1.6.1/petkitaio/constants.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)      835 2023-07-09 19:59:24.000000 petkitaio-0.1.6.1/petkitaio/exceptions.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1392 2023-07-09 19:59:24.000000 petkitaio-0.1.6.1/petkitaio/model.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)    43340 2023-07-09 19:59:24.000000 petkitaio-0.1.6.1/petkitaio/petkit_client.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)      680 2023-07-09 19:59:24.000000 petkitaio-0.1.6.1/petkitaio/str_enum.py
+drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-07-09 20:04:05.159570 petkitaio-0.1.6.1/petkitaio.egg-info/
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)     6155 2023-07-09 20:04:05.000000 petkitaio-0.1.6.1/petkitaio.egg-info/PKG-INFO
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)      337 2023-07-09 20:04:05.000000 petkitaio-0.1.6.1/petkitaio.egg-info/SOURCES.txt
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)        1 2023-07-09 20:04:05.000000 petkitaio-0.1.6.1/petkitaio.egg-info/dependency_links.txt
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)       28 2023-07-09 20:04:05.000000 petkitaio-0.1.6.1/petkitaio.egg-info/requires.txt
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)       10 2023-07-09 20:04:05.000000 petkitaio-0.1.6.1/petkitaio.egg-info/top_level.txt
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)       38 2023-07-09 20:04:05.160680 petkitaio-0.1.6.1/setup.cfg
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1052 2023-07-09 19:59:24.000000 petkitaio-0.1.6.1/setup.py
```

### Comparing `petkitaio-0.1.6/LICENSE` & `petkitaio-0.1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `petkitaio-0.1.6/PKG-INFO` & `petkitaio-0.1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petkitaio
-Version: 0.1.6
+Version: 0.1.6.1
 Summary: Asynchronous Python library for PetKit's API
 Home-page: https://github.com/RobertD502/petkitaio
 Author: Robert Drinovac
 Author-email: unlisted@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/RobertD502/petkitaio/issues
 Project-URL: Source, https://github.com/RobertD502/petkitaio/
```

### Comparing `petkitaio-0.1.6/README.md` & `petkitaio-0.1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `petkitaio-0.1.6/petkitaio/__init__.py` & `petkitaio-0.1.6.1/petkitaio/__init__.py`

 * *Files identical despite different names*

### Comparing `petkitaio-0.1.6/petkitaio/constants.py` & `petkitaio-0.1.6.1/petkitaio/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,14 +257,15 @@
 
 BLUETOOTH_ERRORS = {
     3003: 'Bluetooth connection failed. Retrying on next update.'
 }
 
 SERVER_ERROR_CODES = {
     1: 'PetKit servers are busy. Please try again later.',
+    99: 'PetKit servers are undergoing maintenance. Please try again later.'
 }
 
 BLE_HEADER = [-6, -4, -3]
 FEEDER_LIST = ['D3', 'D4', 'D4s', 'Feeder', 'FeederMini']
 LITTER_LIST = ['T3', 'T4']
 PURIFIER_LIST = ['K2']
 WATER_FOUNTAIN_LIST = ['W5']
```

### Comparing `petkitaio-0.1.6/petkitaio/exceptions.py` & `petkitaio-0.1.6.1/petkitaio/exceptions.py`

 * *Files identical despite different names*

### Comparing `petkitaio-0.1.6/petkitaio/model.py` & `petkitaio-0.1.6.1/petkitaio/model.py`

 * *Files identical despite different names*

### Comparing `petkitaio-0.1.6/petkitaio/petkit_client.py` & `petkitaio-0.1.6.1/petkitaio/petkit_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -399,17 +399,17 @@
         async with self._session.post(url, headers=headers, data=data, timeout=self.timeout) as resp:
             return await self._response(resp)
 
     @staticmethod
     async def _response(resp: ClientResponse) -> dict[str, Any]:
         """Return response from API call."""
 
-        if resp.status != 200:
-            error = await resp.text()
-            raise PetKitError(f'PetKit API error: {error}')
+#        if resp.status != 200:
+#            error = await resp.text()
+#            raise PetKitError(f'PetKit API Error Encountered. Status: {resp.status}; Error: {error}')
         try:
             response: dict[str, Any] = await resp.json()
         except Exception as error:
             raise PetKitError(f'Could not return json {error}') from error
         if 'error' in response:
             code = response['error']['code']
             if code in AUTH_ERROR_CODES:
```

### Comparing `petkitaio-0.1.6/petkitaio/str_enum.py` & `petkitaio-0.1.6.1/petkitaio/str_enum.py`

 * *Files identical despite different names*

### Comparing `petkitaio-0.1.6/petkitaio.egg-info/PKG-INFO` & `petkitaio-0.1.6.1/petkitaio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petkitaio
-Version: 0.1.6
+Version: 0.1.6.1
 Summary: Asynchronous Python library for PetKit's API
 Home-page: https://github.com/RobertD502/petkitaio
 Author: Robert Drinovac
 Author-email: unlisted@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/RobertD502/petkitaio/issues
 Project-URL: Source, https://github.com/RobertD502/petkitaio/
```

### Comparing `petkitaio-0.1.6/setup.py` & `petkitaio-0.1.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="petkitaio",
-    version="0.1.6",
+    version="0.1.6.1",
     author="Robert Drinovac",
     author_email="unlisted@gmail.com",
     description="Asynchronous Python library for PetKit's API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/RobertD502/petkitaio',
     keywords='petkit, eversweet 3 pro, feeder mini, d4, petkit feeder, petkit water fountain, freshelement solo, pura x, pura max, pura air',
```

