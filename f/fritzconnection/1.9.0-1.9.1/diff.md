# Comparing `tmp/fritzconnection-1.9.0.tar.gz` & `tmp/fritzconnection-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fritzconnection-1.9.0.tar", last modified: Wed Jan  5 13:07:26 2022, max compression
+gzip compressed data, was "dist/fritzconnection-1.9.1.tar", last modified: Mon Jan 17 12:57:17 2022, max compression
```

## Comparing `fritzconnection-1.9.0.tar` & `fritzconnection-1.9.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 klaus      (501) staff       (20)        0 2022-01-05 13:07:26.842033 fritzconnection-1.9.0/
--rw-r--r--   0 klaus      (501) staff       (20)     1060 2021-12-26 17:00:50.000000 fritzconnection-1.9.0/LICENSE.txt
--rw-r--r--   0 klaus      (501) staff       (20)      132 2019-09-09 12:57:48.000000 fritzconnection-1.9.0/MANIFEST.in
--rw-r--r--   0 klaus      (501) staff       (20)     2599 2022-01-05 13:07:26.841400 fritzconnection-1.9.0/PKG-INFO
--rw-r--r--   0 klaus      (501) staff       (20)     1600 2022-01-04 22:39:17.000000 fritzconnection-1.9.0/README.rst
-drwxr-xr-x   0 klaus      (501) staff       (20)        0 2022-01-05 13:07:26.808602 fritzconnection-1.9.0/fritzconnection/
--rw-r--r--   0 klaus      (501) staff       (20)      388 2022-01-05 12:56:13.000000 fritzconnection-1.9.0/fritzconnection/__init__.py
-drwxr-xr-x   0 klaus      (501) staff       (20)        0 2022-01-05 13:07:26.823246 fritzconnection-1.9.0/fritzconnection/cli/
--rw-r--r--   0 klaus      (501) staff       (20)      171 2020-07-23 16:09:25.000000 fritzconnection-1.9.0/fritzconnection/cli/__init__.py
--rw-r--r--   0 klaus      (501) staff       (20)     2320 2020-07-23 16:09:25.000000 fritzconnection-1.9.0/fritzconnection/cli/fritzcall.py
--rw-r--r--   0 klaus      (501) staff       (20)     2507 2021-12-28 09:27:36.000000 fritzconnection-1.9.0/fritzconnection/cli/fritzhomeauto.py
--rw-r--r--   0 klaus      (501) staff       (20)     1157 2020-07-23 16:09:25.000000 fritzconnection-1.9.0/fritzconnection/cli/fritzhosts.py
--rw-r--r--   0 klaus      (501) staff       (20)     5846 2021-12-26 16:59:02.000000 fritzconnection-1.9.0/fritzconnection/cli/fritzinspection.py
--rw-r--r--   0 klaus      (501) staff       (20)     3057 2021-02-13 09:33:35.000000 fritzconnection-1.9.0/fritzconnection/cli/fritzmonitor.py
--rw-r--r--   0 klaus      (501) staff       (20)     2303 2020-07-23 16:09:25.000000 fritzconnection-1.9.0/fritzconnection/cli/fritzphonebook.py
--rw-r--r--   0 klaus      (501) staff       (20)     1466 2021-12-28 09:27:36.000000 fritzconnection-1.9.0/fritzconnection/cli/fritzstatus.py
--rw-r--r--   0 klaus      (501) staff       (20)     2110 2021-12-28 09:27:36.000000 fritzconnection-1.9.0/fritzconnection/cli/fritzwlan.py
--rw-r--r--   0 klaus      (501) staff       (20)     2010 2020-07-23 16:09:25.000000 fritzconnection-1.9.0/fritzconnection/cli/utils.py
-drwxr-xr-x   0 klaus      (501) staff       (20)        0 2022-01-05 13:07:26.831375 fritzconnection-1.9.0/fritzconnection/core/
--rw-r--r--   0 klaus      (501) staff       (20)        1 2020-07-23 16:09:25.000000 fritzconnection-1.9.0/fritzconnection/core/__init__.py
--rw-r--r--   0 klaus      (501) staff       (20)     3264 2021-12-28 09:27:36.000000 fritzconnection-1.9.0/fritzconnection/core/devices.py
--rw-r--r--   0 klaus      (501) staff       (20)     5353 2021-12-28 09:27:36.000000 fritzconnection-1.9.0/fritzconnection/core/exceptions.py
--rw-r--r--   0 klaus      (501) staff       (20)    11285 2021-12-28 09:27:36.000000 fritzconnection-1.9.0/fritzconnection/core/fritzconnection.py
--rw-r--r--   0 klaus      (501) staff       (20)     9403 2021-12-28 09:27:36.000000 fritzconnection-1.9.0/fritzconnection/core/fritzmonitor.py
--rw-r--r--   0 klaus      (501) staff       (20)     2906 2021-12-28 09:27:36.000000 fritzconnection-1.9.0/fritzconnection/core/logger.py
--rw-r--r--   0 klaus      (501) staff       (20)    13281 2021-12-28 09:27:36.000000 fritzconnection-1.9.0/fritzconnection/core/processor.py
--rw-r--r--   0 klaus      (501) staff       (20)     9627 2021-12-28 09:27:36.000000 fritzconnection-1.9.0/fritzconnection/core/soaper.py
--rw-r--r--   0 klaus      (501) staff       (20)     2865 2021-12-28 09:27:36.000000 fritzconnection-1.9.0/fritzconnection/core/utils.py
-drwxr-xr-x   0 klaus      (501) staff       (20)        0 2022-01-05 13:07:26.840272 fritzconnection-1.9.0/fritzconnection/lib/
--rw-r--r--   0 klaus      (501) staff       (20)      211 2020-07-23 16:09:25.000000 fritzconnection-1.9.0/fritzconnection/lib/__init__.py
--rw-r--r--   0 klaus      (501) staff       (20)     1589 2021-07-24 12:53:03.000000 fritzconnection-1.9.0/fritzconnection/lib/fritzbase.py
--rw-r--r--   0 klaus      (501) staff       (20)     7055 2021-12-28 09:27:36.000000 fritzconnection-1.9.0/fritzconnection/lib/fritzcall.py
--rw-r--r--   0 klaus      (501) staff       (20)     3203 2022-01-04 16:18:52.000000 fritzconnection-1.9.0/fritzconnection/lib/fritzhomeauto.py
--rw-r--r--   0 klaus      (501) staff       (20)     7074 2022-01-03 14:39:23.000000 fritzconnection-1.9.0/fritzconnection/lib/fritzhosts.py
--rw-r--r--   0 klaus      (501) staff       (20)     6105 2021-12-28 09:27:36.000000 fritzconnection-1.9.0/fritzconnection/lib/fritzphonebook.py
--rw-r--r--   0 klaus      (501) staff       (20)     9999 2022-01-04 16:18:52.000000 fritzconnection-1.9.0/fritzconnection/lib/fritzstatus.py
--rw-r--r--   0 klaus      (501) staff       (20)     1427 2021-12-28 09:27:36.000000 fritzconnection-1.9.0/fritzconnection/lib/fritztools.py
--rw-r--r--   0 klaus      (501) staff       (20)    10741 2022-01-04 16:19:16.000000 fritzconnection-1.9.0/fritzconnection/lib/fritzwlan.py
-drwxr-xr-x   0 klaus      (501) staff       (20)        0 2022-01-05 13:07:26.812333 fritzconnection-1.9.0/fritzconnection.egg-info/
--rw-r--r--   0 klaus      (501) staff       (20)     2599 2022-01-05 13:07:26.000000 fritzconnection-1.9.0/fritzconnection.egg-info/PKG-INFO
--rw-r--r--   0 klaus      (501) staff       (20)     1265 2022-01-05 13:07:26.000000 fritzconnection-1.9.0/fritzconnection.egg-info/SOURCES.txt
--rw-r--r--   0 klaus      (501) staff       (20)        1 2022-01-05 13:07:26.000000 fritzconnection-1.9.0/fritzconnection.egg-info/dependency_links.txt
--rw-r--r--   0 klaus      (501) staff       (20)      437 2022-01-05 13:07:26.000000 fritzconnection-1.9.0/fritzconnection.egg-info/entry_points.txt
--rw-r--r--   0 klaus      (501) staff       (20)       36 2022-01-05 13:07:26.000000 fritzconnection-1.9.0/fritzconnection.egg-info/requires.txt
--rw-r--r--   0 klaus      (501) staff       (20)       16 2022-01-05 13:07:26.000000 fritzconnection-1.9.0/fritzconnection.egg-info/top_level.txt
--rw-r--r--   0 klaus      (501) staff       (20)       38 2022-01-05 13:07:26.842242 fritzconnection-1.9.0/setup.cfg
--rw-r--r--   0 klaus      (501) staff       (20)     2270 2022-01-04 16:19:16.000000 fritzconnection-1.9.0/setup.py
+drwxr-xr-x   0 klaus      (501) staff       (20)        0 2022-01-17 12:57:17.000000 fritzconnection-1.9.1/
+-rw-r--r--   0 klaus      (501) staff       (20)     1060 2021-12-26 17:00:50.000000 fritzconnection-1.9.1/LICENSE.txt
+-rw-r--r--   0 klaus      (501) staff       (20)      132 2019-09-09 12:57:48.000000 fritzconnection-1.9.1/MANIFEST.in
+-rw-r--r--   0 klaus      (501) staff       (20)     3024 2022-01-17 12:57:17.000000 fritzconnection-1.9.1/PKG-INFO
+-rw-r--r--   0 klaus      (501) staff       (20)     1600 2022-01-17 12:17:09.000000 fritzconnection-1.9.1/README.rst
+drwxr-xr-x   0 klaus      (501) staff       (20)        0 2022-01-17 12:57:17.000000 fritzconnection-1.9.1/fritzconnection/
+-rw-r--r--   0 klaus      (501) staff       (20)      388 2022-01-17 12:28:18.000000 fritzconnection-1.9.1/fritzconnection/__init__.py
+drwxr-xr-x   0 klaus      (501) staff       (20)        0 2022-01-17 12:57:17.000000 fritzconnection-1.9.1/fritzconnection/cli/
+-rw-r--r--   0 klaus      (501) staff       (20)      171 2020-07-23 16:09:25.000000 fritzconnection-1.9.1/fritzconnection/cli/__init__.py
+-rw-r--r--   0 klaus      (501) staff       (20)     2320 2020-07-23 16:09:25.000000 fritzconnection-1.9.1/fritzconnection/cli/fritzcall.py
+-rw-r--r--   0 klaus      (501) staff       (20)     2507 2021-12-28 09:27:36.000000 fritzconnection-1.9.1/fritzconnection/cli/fritzhomeauto.py
+-rw-r--r--   0 klaus      (501) staff       (20)     1157 2020-07-23 16:09:25.000000 fritzconnection-1.9.1/fritzconnection/cli/fritzhosts.py
+-rw-r--r--   0 klaus      (501) staff       (20)     5846 2021-12-26 16:59:02.000000 fritzconnection-1.9.1/fritzconnection/cli/fritzinspection.py
+-rw-r--r--   0 klaus      (501) staff       (20)     3057 2021-02-13 09:33:35.000000 fritzconnection-1.9.1/fritzconnection/cli/fritzmonitor.py
+-rw-r--r--   0 klaus      (501) staff       (20)     2303 2020-07-23 16:09:25.000000 fritzconnection-1.9.1/fritzconnection/cli/fritzphonebook.py
+-rw-r--r--   0 klaus      (501) staff       (20)     1466 2021-12-28 09:27:36.000000 fritzconnection-1.9.1/fritzconnection/cli/fritzstatus.py
+-rw-r--r--   0 klaus      (501) staff       (20)     2110 2021-12-28 09:27:36.000000 fritzconnection-1.9.1/fritzconnection/cli/fritzwlan.py
+-rw-r--r--   0 klaus      (501) staff       (20)     2010 2020-07-23 16:09:25.000000 fritzconnection-1.9.1/fritzconnection/cli/utils.py
+drwxr-xr-x   0 klaus      (501) staff       (20)        0 2022-01-17 12:57:17.000000 fritzconnection-1.9.1/fritzconnection/core/
+-rw-r--r--   0 klaus      (501) staff       (20)        1 2020-07-23 16:09:25.000000 fritzconnection-1.9.1/fritzconnection/core/__init__.py
+-rw-r--r--   0 klaus      (501) staff       (20)     3264 2021-12-28 09:27:36.000000 fritzconnection-1.9.1/fritzconnection/core/devices.py
+-rw-r--r--   0 klaus      (501) staff       (20)     5353 2021-12-28 09:27:36.000000 fritzconnection-1.9.1/fritzconnection/core/exceptions.py
+-rw-r--r--   0 klaus      (501) staff       (20)    11285 2021-12-28 09:27:36.000000 fritzconnection-1.9.1/fritzconnection/core/fritzconnection.py
+-rw-r--r--   0 klaus      (501) staff       (20)     9403 2021-12-28 09:27:36.000000 fritzconnection-1.9.1/fritzconnection/core/fritzmonitor.py
+-rw-r--r--   0 klaus      (501) staff       (20)     2906 2021-12-28 09:27:36.000000 fritzconnection-1.9.1/fritzconnection/core/logger.py
+-rw-r--r--   0 klaus      (501) staff       (20)    13281 2021-12-28 09:27:36.000000 fritzconnection-1.9.1/fritzconnection/core/processor.py
+-rw-r--r--   0 klaus      (501) staff       (20)     9627 2021-12-28 09:27:36.000000 fritzconnection-1.9.1/fritzconnection/core/soaper.py
+-rw-r--r--   0 klaus      (501) staff       (20)     2865 2022-01-16 13:07:05.000000 fritzconnection-1.9.1/fritzconnection/core/utils.py
+drwxr-xr-x   0 klaus      (501) staff       (20)        0 2022-01-17 12:57:17.000000 fritzconnection-1.9.1/fritzconnection/lib/
+-rw-r--r--   0 klaus      (501) staff       (20)      211 2020-07-23 16:09:25.000000 fritzconnection-1.9.1/fritzconnection/lib/__init__.py
+-rw-r--r--   0 klaus      (501) staff       (20)     1589 2021-07-24 12:53:03.000000 fritzconnection-1.9.1/fritzconnection/lib/fritzbase.py
+-rw-r--r--   0 klaus      (501) staff       (20)     7055 2021-12-28 09:27:36.000000 fritzconnection-1.9.1/fritzconnection/lib/fritzcall.py
+-rw-r--r--   0 klaus      (501) staff       (20)     3231 2022-01-17 12:17:09.000000 fritzconnection-1.9.1/fritzconnection/lib/fritzhomeauto.py
+-rw-r--r--   0 klaus      (501) staff       (20)     7074 2022-01-16 13:07:05.000000 fritzconnection-1.9.1/fritzconnection/lib/fritzhosts.py
+-rw-r--r--   0 klaus      (501) staff       (20)     6105 2021-12-28 09:27:36.000000 fritzconnection-1.9.1/fritzconnection/lib/fritzphonebook.py
+-rw-r--r--   0 klaus      (501) staff       (20)     9999 2022-01-17 12:17:09.000000 fritzconnection-1.9.1/fritzconnection/lib/fritzstatus.py
+-rw-r--r--   0 klaus      (501) staff       (20)     1427 2021-12-28 09:27:36.000000 fritzconnection-1.9.1/fritzconnection/lib/fritztools.py
+-rw-r--r--   0 klaus      (501) staff       (20)    11119 2022-01-17 12:17:22.000000 fritzconnection-1.9.1/fritzconnection/lib/fritzwlan.py
+drwxr-xr-x   0 klaus      (501) staff       (20)        0 2022-01-17 12:57:17.000000 fritzconnection-1.9.1/fritzconnection.egg-info/
+-rw-r--r--   0 klaus      (501) staff       (20)     3024 2022-01-17 12:57:17.000000 fritzconnection-1.9.1/fritzconnection.egg-info/PKG-INFO
+-rw-r--r--   0 klaus      (501) staff       (20)     1265 2022-01-17 12:57:17.000000 fritzconnection-1.9.1/fritzconnection.egg-info/SOURCES.txt
+-rw-r--r--   0 klaus      (501) staff       (20)        1 2022-01-17 12:57:17.000000 fritzconnection-1.9.1/fritzconnection.egg-info/dependency_links.txt
+-rw-r--r--   0 klaus      (501) staff       (20)      437 2022-01-17 12:57:17.000000 fritzconnection-1.9.1/fritzconnection.egg-info/entry_points.txt
+-rw-r--r--   0 klaus      (501) staff       (20)       36 2022-01-17 12:57:17.000000 fritzconnection-1.9.1/fritzconnection.egg-info/requires.txt
+-rw-r--r--   0 klaus      (501) staff       (20)       16 2022-01-17 12:57:17.000000 fritzconnection-1.9.1/fritzconnection.egg-info/top_level.txt
+-rw-r--r--   0 klaus      (501) staff       (20)       38 2022-01-17 12:57:17.000000 fritzconnection-1.9.1/setup.cfg
+-rw-r--r--   0 klaus      (501) staff       (20)     2270 2022-01-04 16:19:16.000000 fritzconnection-1.9.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `fritzconnection-1.9.0/LICENSE.txt` & `fritzconnection-1.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fritzconnection-1.9.0/PKG-INFO` & `fritzconnection-1.9.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,71 @@
 Metadata-Version: 2.1
 Name: fritzconnection
-Version: 1.9.0
+Version: 1.9.1
 Summary: Communicate with the AVM FRITZ!Box
 Home-page: https://github.com/kbr/fritzconnection
 Author: Klaus Bremer
 Author-email: bremer@bremer-media.com
 License: MIT
+Description: 
+        ===============
+        fritzconnection
+        ===============
+        
+        
+        .. image::
+            https://img.shields.io/pypi/pyversions/fritzconnection.svg
+            :alt: Python versions
+            :target: https://pypi.org/project/fritzconnection/
+        
+        .. image::
+            https://img.shields.io/pypi/l/fritzconnection.svg
+            :target: https://pypi.org/project/fritzconnection/
+        
+        
+        Python-Tool to communicate with the AVM Fritz!Box.
+        Uses the TR-064 protocol over UPnP.
+        
+        Installation:
+        -------------
+        
+        For installation use pip ::
+        
+            $ pip install fritzconnection
+            or
+            $ pip install fritzconnection[qr]
+        
+        The latter will enable QR-code creation for wifi login.
+        
+        Quickstart:
+        -----------
+        
+        Using fritzconnection is as easy as: ::
+        
+            from fritzconnection import FritzConnection
+        
+            fc = FritzConnection(address='192.168.178.1')
+            fc.reconnect()  # get a new external ip from the provider
+            print(fc)  # print router model informations
+        
+        In general FritzConnection can execute every action provided by the (model-specific) API. For i.e. this can be network settings, status informations, access to home automation devices and much more.
+        
+        The basic method FritzConnection provides to access the FritzOS-API is the `call_action()` method. A reconnection by means of *call_action()* would look like this: ::
+        
+            fc = FritzConnection(address='192.168.178.1')
+            fc.call_action("WANIPConn1", "ForceTermination")
+        
+        The package comes with a library providing modules as examples how to implement applications on top of FritzConnection.
+        
+        
+        Documentation
+        -------------
+        
+        The full documentation and release notes are at https://fritzconnection.readthedocs.org
+        
 Keywords: AVM FRITZ!Box fritzbox fritz
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -19,66 +75,7 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >= 3.6
 Provides-Extra: qr
-License-File: LICENSE.txt
-
-
-===============
-fritzconnection
-===============
-
-
-.. image::
-    https://img.shields.io/pypi/pyversions/fritzconnection.svg
-    :alt: Python versions
-    :target: https://pypi.org/project/fritzconnection/
-
-.. image::
-    https://img.shields.io/pypi/l/fritzconnection.svg
-    :target: https://pypi.org/project/fritzconnection/
-
-
-Python-Tool to communicate with the AVM Fritz!Box.
-Uses the TR-064 protocol over UPnP.
-
-Installation:
--------------
-
-For installation use pip ::
-
-    $ pip install fritzconnection
-    or
-    $ pip install fritzconnection[qr]
-
-The latter will enable QR-code creation for wifi login.
-
-Quickstart:
------------
-
-Using fritzconnection is as easy as: ::
-
-    from fritzconnection import FritzConnection
-
-    fc = FritzConnection(address='192.168.178.1')
-    fc.reconnect()  # get a new external ip from the provider
-    print(fc)  # print router model informations
-
-In general FritzConnection can execute every action provided by the (model-specific) API. For i.e. this can be network settings, status informations, access to home automation devices and much more.
-
-The basic method FritzConnection provides to access the FritzOS-API is the `call_action()` method. A reconnection by means of *call_action()* would look like this: ::
-
-    fc = FritzConnection(address='192.168.178.1')
-    fc.call_action("WANIPConn1", "ForceTermination")
-
-The package comes with a library providing modules as examples how to implement applications on top of FritzConnection.
-
-
-Documentation
--------------
-
-The full documentation and release notes are at https://fritzconnection.readthedocs.org
-
-
```

### Comparing `fritzconnection-1.9.0/README.rst` & `fritzconnection-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `fritzconnection-1.9.0/fritzconnection/cli/fritzcall.py` & `fritzconnection-1.9.1/fritzconnection/cli/fritzcall.py`

 * *Files identical despite different names*

### Comparing `fritzconnection-1.9.0/fritzconnection/cli/fritzhomeauto.py` & `fritzconnection-1.9.1/fritzconnection/cli/fritzhomeauto.py`

 * *Files identical despite different names*

### Comparing `fritzconnection-1.9.0/fritzconnection/cli/fritzhosts.py` & `fritzconnection-1.9.1/fritzconnection/cli/fritzhosts.py`

 * *Files identical despite different names*

### Comparing `fritzconnection-1.9.0/fritzconnection/cli/fritzinspection.py` & `fritzconnection-1.9.1/fritzconnection/cli/fritzinspection.py`

 * *Files identical despite different names*

### Comparing `fritzconnection-1.9.0/fritzconnection/cli/fritzmonitor.py` & `fritzconnection-1.9.1/fritzconnection/cli/fritzmonitor.py`

 * *Files identical despite different names*

### Comparing `fritzconnection-1.9.0/fritzconnection/cli/fritzphonebook.py` & `fritzconnection-1.9.1/fritzconnection/cli/fritzphonebook.py`

 * *Files identical despite different names*

### Comparing `fritzconnection-1.9.0/fritzconnection/cli/fritzstatus.py` & `fritzconnection-1.9.1/fritzconnection/cli/fritzstatus.py`

 * *Files identical despite different names*

### Comparing `fritzconnection-1.9.0/fritzconnection/cli/fritzwlan.py` & `fritzconnection-1.9.1/fritzconnection/cli/fritzwlan.py`

 * *Files identical despite different names*

### Comparing `fritzconnection-1.9.0/fritzconnection/cli/utils.py` & `fritzconnection-1.9.1/fritzconnection/cli/utils.py`

 * *Files identical despite different names*

### Comparing `fritzconnection-1.9.0/fritzconnection/core/devices.py` & `fritzconnection-1.9.1/fritzconnection/core/devices.py`

 * *Files identical despite different names*

### Comparing `fritzconnection-1.9.0/fritzconnection/core/exceptions.py` & `fritzconnection-1.9.1/fritzconnection/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `fritzconnection-1.9.0/fritzconnection/core/fritzconnection.py` & `fritzconnection-1.9.1/fritzconnection/core/fritzconnection.py`

 * *Files identical despite different names*

### Comparing `fritzconnection-1.9.0/fritzconnection/core/fritzmonitor.py` & `fritzconnection-1.9.1/fritzconnection/core/fritzmonitor.py`

 * *Files identical despite different names*

### Comparing `fritzconnection-1.9.0/fritzconnection/core/logger.py` & `fritzconnection-1.9.1/fritzconnection/core/logger.py`

 * *Files identical despite different names*

### Comparing `fritzconnection-1.9.0/fritzconnection/core/processor.py` & `fritzconnection-1.9.1/fritzconnection/core/processor.py`

 * *Files identical despite different names*

### Comparing `fritzconnection-1.9.0/fritzconnection/core/soaper.py` & `fritzconnection-1.9.1/fritzconnection/core/soaper.py`

 * *Files identical despite different names*

### Comparing `fritzconnection-1.9.0/fritzconnection/core/utils.py` & `fritzconnection-1.9.1/fritzconnection/core/utils.py`

 * *Files identical despite different names*

### Comparing `fritzconnection-1.9.0/fritzconnection/lib/fritzbase.py` & `fritzconnection-1.9.1/fritzconnection/lib/fritzbase.py`

 * *Files identical despite different names*

### Comparing `fritzconnection-1.9.0/fritzconnection/lib/fritzcall.py` & `fritzconnection-1.9.1/fritzconnection/lib/fritzcall.py`

 * *Files identical despite different names*

### Comparing `fritzconnection-1.9.0/fritzconnection/lib/fritzhomeauto.py` & `fritzconnection-1.9.1/fritzconnection/lib/fritzhomeauto.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,18 +68,18 @@
     def device_information(self):
         """
         Returns a list of dictionaries for all known homeauto-devices.
         """
         info = list()
         for n in itertools.count():
             try:
-                info = self.get_device_information_by_index(n)
+                device_information = self.get_device_information_by_index(n)
             except IndexError:
                 break
-            info.append(info)
+            info.append(device_information)
         return info
 
     def set_switch(self, identifier, on=True):
         """
         Sets a switch state on devices providing a switch state.
         'identifier' must be the AIN of the device. 'on' is a boolean
         whether the switch should be on (True) or off (False).
```

### Comparing `fritzconnection-1.9.0/fritzconnection/lib/fritzhosts.py` & `fritzconnection-1.9.1/fritzconnection/lib/fritzhosts.py`

 * *Files identical despite different names*

### Comparing `fritzconnection-1.9.0/fritzconnection/lib/fritzphonebook.py` & `fritzconnection-1.9.1/fritzconnection/lib/fritzphonebook.py`

 * *Files identical despite different names*

### Comparing `fritzconnection-1.9.0/fritzconnection/lib/fritzstatus.py` & `fritzconnection-1.9.1/fritzconnection/lib/fritzstatus.py`

 * *Files identical despite different names*

### Comparing `fritzconnection-1.9.0/fritzconnection/lib/fritztools.py` & `fritzconnection-1.9.1/fritzconnection/lib/fritztools.py`

 * *Files identical despite different names*

### Comparing `fritzconnection-1.9.0/fritzconnection/lib/fritzwlan.py` & `fritzconnection-1.9.1/fritzconnection/lib/fritzwlan.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     SEGNO_INSTALLED = True
 
 # important: don't set an extension number here:
 SERVICE = 'WLANConfiguration'
 DEFAULT_PASSWORD_LENGTH = 12
 
 
-def get_wifi_qr_code(instance, kind='svg'):
+def get_wifi_qr_code(instance, kind='svg', security=None, hidden=False):
     """
     Returns a file-like object providing a bytestring representing a
     qr-code for wlan access. `instance` is a FritzWLAN or FritzGuestWLAN
     instance. `kind` describes the type of the qr-code. Supported types
     are: 'svg', 'png' and 'pdf'. Default is 'svg'.
 
     This function is not intended to get called directly. Instead it is
@@ -54,17 +54,30 @@
     >>> ....fobj.write(stream.read())
 
     If the `segno` is not installed the call will trigger an
     AttributeError when called on an instance and a NameError when
     called directly.
 
     .. versionadded:: 1.9.0
+
+    The parameters `security` and `hidden` allow to forward these
+    informations to the `segno` library. `security` is `None` or a
+    string like `WPA2`. `hidden` is a boolean value indicating the
+    visibility of the network .
+
+    .. versionadded:: 1.9.1
+
     """
     stream = io.BytesIO()
-    qr_code = segno.helpers.make_wifi(instance.ssid, instance.get_password())
+    qr_code = segno.helpers.make_wifi(
+        ssid=instance.ssid,
+        password=instance.get_password(),
+        security=security,
+        hidden=hidden
+    )
     qr_code.save(out=stream, kind=kind)
     stream.seek(0)
     return stream
 
 
 def _qr_code_enabler(cls):
     """Classdecorator to inject qr-capabilities at import time."""
```

### Comparing `fritzconnection-1.9.0/fritzconnection.egg-info/PKG-INFO` & `fritzconnection-1.9.1/fritzconnection.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,71 @@
 Metadata-Version: 2.1
 Name: fritzconnection
-Version: 1.9.0
+Version: 1.9.1
 Summary: Communicate with the AVM FRITZ!Box
 Home-page: https://github.com/kbr/fritzconnection
 Author: Klaus Bremer
 Author-email: bremer@bremer-media.com
 License: MIT
+Description: 
+        ===============
+        fritzconnection
+        ===============
+        
+        
+        .. image::
+            https://img.shields.io/pypi/pyversions/fritzconnection.svg
+            :alt: Python versions
+            :target: https://pypi.org/project/fritzconnection/
+        
+        .. image::
+            https://img.shields.io/pypi/l/fritzconnection.svg
+            :target: https://pypi.org/project/fritzconnection/
+        
+        
+        Python-Tool to communicate with the AVM Fritz!Box.
+        Uses the TR-064 protocol over UPnP.
+        
+        Installation:
+        -------------
+        
+        For installation use pip ::
+        
+            $ pip install fritzconnection
+            or
+            $ pip install fritzconnection[qr]
+        
+        The latter will enable QR-code creation for wifi login.
+        
+        Quickstart:
+        -----------
+        
+        Using fritzconnection is as easy as: ::
+        
+            from fritzconnection import FritzConnection
+        
+            fc = FritzConnection(address='192.168.178.1')
+            fc.reconnect()  # get a new external ip from the provider
+            print(fc)  # print router model informations
+        
+        In general FritzConnection can execute every action provided by the (model-specific) API. For i.e. this can be network settings, status informations, access to home automation devices and much more.
+        
+        The basic method FritzConnection provides to access the FritzOS-API is the `call_action()` method. A reconnection by means of *call_action()* would look like this: ::
+        
+            fc = FritzConnection(address='192.168.178.1')
+            fc.call_action("WANIPConn1", "ForceTermination")
+        
+        The package comes with a library providing modules as examples how to implement applications on top of FritzConnection.
+        
+        
+        Documentation
+        -------------
+        
+        The full documentation and release notes are at https://fritzconnection.readthedocs.org
+        
 Keywords: AVM FRITZ!Box fritzbox fritz
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -19,66 +75,7 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >= 3.6
 Provides-Extra: qr
-License-File: LICENSE.txt
-
-
-===============
-fritzconnection
-===============
-
-
-.. image::
-    https://img.shields.io/pypi/pyversions/fritzconnection.svg
-    :alt: Python versions
-    :target: https://pypi.org/project/fritzconnection/
-
-.. image::
-    https://img.shields.io/pypi/l/fritzconnection.svg
-    :target: https://pypi.org/project/fritzconnection/
-
-
-Python-Tool to communicate with the AVM Fritz!Box.
-Uses the TR-064 protocol over UPnP.
-
-Installation:
--------------
-
-For installation use pip ::
-
-    $ pip install fritzconnection
-    or
-    $ pip install fritzconnection[qr]
-
-The latter will enable QR-code creation for wifi login.
-
-Quickstart:
------------
-
-Using fritzconnection is as easy as: ::
-
-    from fritzconnection import FritzConnection
-
-    fc = FritzConnection(address='192.168.178.1')
-    fc.reconnect()  # get a new external ip from the provider
-    print(fc)  # print router model informations
-
-In general FritzConnection can execute every action provided by the (model-specific) API. For i.e. this can be network settings, status informations, access to home automation devices and much more.
-
-The basic method FritzConnection provides to access the FritzOS-API is the `call_action()` method. A reconnection by means of *call_action()* would look like this: ::
-
-    fc = FritzConnection(address='192.168.178.1')
-    fc.call_action("WANIPConn1", "ForceTermination")
-
-The package comes with a library providing modules as examples how to implement applications on top of FritzConnection.
-
-
-Documentation
--------------
-
-The full documentation and release notes are at https://fritzconnection.readthedocs.org
-
-
```

### Comparing `fritzconnection-1.9.0/fritzconnection.egg-info/SOURCES.txt` & `fritzconnection-1.9.1/fritzconnection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fritzconnection-1.9.0/setup.py` & `fritzconnection-1.9.1/setup.py`

 * *Files identical despite different names*

