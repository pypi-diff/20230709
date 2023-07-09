# Comparing `tmp/roxbot-0.9.0.tar.gz` & `tmp/roxbot-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roxbot-0.9.0.tar", last modified: Sat Jul  8 14:12:26 2023, max compression
+gzip compressed data, was "roxbot-0.9.1.tar", last modified: Sun Jul  9 12:45:32 2023, max compression
```

## Comparing `roxbot-0.9.0.tar` & `roxbot-0.9.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 14:12:26.068576 roxbot-0.9.0/
--rw-rw-rw-   0 root         (0) root         (0)     1081 2023-07-08 14:12:13.000000 roxbot-0.9.0/LICENCE
--rw-r--r--   0 root         (0) root         (0)      382 2023-07-08 14:12:26.068576 roxbot-0.9.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1734 2023-07-08 14:12:13.000000 roxbot-0.9.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      360 2023-07-08 14:12:26.069576 roxbot-0.9.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1289 2023-07-08 14:12:13.000000 roxbot-0.9.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 14:12:26.062576 roxbot-0.9.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 14:12:26.065576 roxbot-0.9.0/src/roxbot/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-08 14:12:13.000000 roxbot-0.9.0/src/roxbot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1095 2023-07-08 14:12:13.000000 roxbot-0.9.0/src/roxbot/base_classes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 14:12:26.066576 roxbot-0.9.0/src/roxbot/bridges/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-08 14:12:13.000000 roxbot-0.9.0/src/roxbot/bridges/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4917 2023-07-08 14:12:13.000000 roxbot-0.9.0/src/roxbot/bridges/web_bridge.py
--rw-rw-rw-   0 root         (0) root         (0)      334 2023-07-08 14:12:13.000000 roxbot-0.9.0/src/roxbot/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     7958 2023-07-08 14:12:13.000000 roxbot-0.9.0/src/roxbot/gps.py
--rw-rw-rw-   0 root         (0) root         (0)      441 2023-07-08 14:12:13.000000 roxbot-0.9.0/src/roxbot/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     9200 2023-07-08 14:12:13.000000 roxbot-0.9.0/src/roxbot/models.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-08 14:12:13.000000 roxbot-0.9.0/src/roxbot/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 14:12:26.067576 roxbot-0.9.0/src/roxbot/simulators/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-08 14:12:13.000000 roxbot-0.9.0/src/roxbot/simulators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      209 2023-07-08 14:12:13.000000 roxbot-0.9.0/src/roxbot/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5020 2023-07-08 14:12:13.000000 roxbot-0.9.0/src/roxbot/vectors.py
--rw-rw-rw-   0 root         (0) root         (0)     2418 2023-07-08 14:12:13.000000 roxbot-0.9.0/src/roxbot/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 14:12:26.066576 roxbot-0.9.0/src/roxbot.egg-info/
--rw-r--r--   0 root         (0) root         (0)      382 2023-07-08 14:12:26.000000 roxbot-0.9.0/src/roxbot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-08 14:12:26.000000 roxbot-0.9.0/src/roxbot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-08 14:12:26.000000 roxbot-0.9.0/src/roxbot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-07-08 14:12:26.000000 roxbot-0.9.0/src/roxbot.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-08 14:12:17.000000 roxbot-0.9.0/src/roxbot.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       84 2023-07-08 14:12:26.000000 roxbot-0.9.0/src/roxbot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-08 14:12:26.000000 roxbot-0.9.0/src/roxbot.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 14:12:26.068576 roxbot-0.9.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)      462 2023-07-08 14:12:13.000000 roxbot-0.9.0/tests/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2822 2023-07-08 14:12:13.000000 roxbot-0.9.0/tests/test_gps.py
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-07-08 14:12:13.000000 roxbot-0.9.0/tests/test_interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2345 2023-07-08 14:12:13.000000 roxbot-0.9.0/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     1847 2023-07-08 14:12:13.000000 roxbot-0.9.0/tests/test_trike.py
--rw-rw-rw-   0 root         (0) root         (0)     2781 2023-07-08 14:12:13.000000 roxbot-0.9.0/tests/test_vectors.py
--rw-rw-rw-   0 root         (0) root         (0)     1982 2023-07-08 14:12:13.000000 roxbot-0.9.0/tests/test_ws_bridge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 12:45:32.328364 roxbot-0.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1081 2023-07-09 12:45:21.000000 roxbot-0.9.1/LICENCE
+-rw-r--r--   0 root         (0) root         (0)      382 2023-07-09 12:45:32.329364 roxbot-0.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1734 2023-07-09 12:45:21.000000 roxbot-0.9.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-07-09 12:45:32.329364 roxbot-0.9.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1289 2023-07-09 12:45:21.000000 roxbot-0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 12:45:32.323364 roxbot-0.9.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 12:45:32.325364 roxbot-0.9.1/src/roxbot/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-09 12:45:21.000000 roxbot-0.9.1/src/roxbot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1095 2023-07-09 12:45:21.000000 roxbot-0.9.1/src/roxbot/base_classes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 12:45:32.327364 roxbot-0.9.1/src/roxbot/bridges/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-09 12:45:21.000000 roxbot-0.9.1/src/roxbot/bridges/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4917 2023-07-09 12:45:21.000000 roxbot-0.9.1/src/roxbot/bridges/web_bridge.py
+-rw-rw-rw-   0 root         (0) root         (0)      334 2023-07-09 12:45:21.000000 roxbot-0.9.1/src/roxbot/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     8311 2023-07-09 12:45:21.000000 roxbot-0.9.1/src/roxbot/gps.py
+-rw-rw-rw-   0 root         (0) root         (0)      441 2023-07-09 12:45:21.000000 roxbot-0.9.1/src/roxbot/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     9200 2023-07-09 12:45:21.000000 roxbot-0.9.1/src/roxbot/models.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-09 12:45:21.000000 roxbot-0.9.1/src/roxbot/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 12:45:32.327364 roxbot-0.9.1/src/roxbot/simulators/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-09 12:45:21.000000 roxbot-0.9.1/src/roxbot/simulators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-07-09 12:45:21.000000 roxbot-0.9.1/src/roxbot/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5020 2023-07-09 12:45:21.000000 roxbot-0.9.1/src/roxbot/vectors.py
+-rw-rw-rw-   0 root         (0) root         (0)     2418 2023-07-09 12:45:21.000000 roxbot-0.9.1/src/roxbot/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 12:45:32.327364 roxbot-0.9.1/src/roxbot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      382 2023-07-09 12:45:32.000000 roxbot-0.9.1/src/roxbot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-09 12:45:32.000000 roxbot-0.9.1/src/roxbot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 12:45:32.000000 roxbot-0.9.1/src/roxbot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-07-09 12:45:32.000000 roxbot-0.9.1/src/roxbot.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 12:45:24.000000 roxbot-0.9.1/src/roxbot.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       84 2023-07-09 12:45:32.000000 roxbot-0.9.1/src/roxbot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-09 12:45:32.000000 roxbot-0.9.1/src/roxbot.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 12:45:32.328364 roxbot-0.9.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      462 2023-07-09 12:45:21.000000 roxbot-0.9.1/tests/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2822 2023-07-09 12:45:21.000000 roxbot-0.9.1/tests/test_gps.py
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-07-09 12:45:21.000000 roxbot-0.9.1/tests/test_interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2345 2023-07-09 12:45:21.000000 roxbot-0.9.1/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1847 2023-07-09 12:45:21.000000 roxbot-0.9.1/tests/test_trike.py
+-rw-rw-rw-   0 root         (0) root         (0)     2781 2023-07-09 12:45:21.000000 roxbot-0.9.1/tests/test_vectors.py
+-rw-rw-rw-   0 root         (0) root         (0)     1982 2023-07-09 12:45:21.000000 roxbot-0.9.1/tests/test_ws_bridge.py
```

### Comparing `roxbot-0.9.0/LICENCE` & `roxbot-0.9.1/LICENCE`

 * *Files identical despite different names*

### Comparing `roxbot-0.9.0/README.md` & `roxbot-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `roxbot-0.9.0/setup.py` & `roxbot-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.9.0/src/roxbot/base_classes.py` & `roxbot-0.9.1/src/roxbot/base_classes.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.9.0/src/roxbot/bridges/web_bridge.py` & `roxbot-0.9.1/src/roxbot/bridges/web_bridge.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.9.0/src/roxbot/gps.py` & `roxbot-0.9.1/src/roxbot/gps.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,22 +22,32 @@
 import logging
 import operator
 from collections import OrderedDict
 from datetime import datetime
 from functools import reduce
 from math import degrees, radians
 from typing import Optional, Tuple
+import os
 
 import pydantic
 import serial_asyncio  # type: ignore
 from pymap3d import enu2geodetic, geodetic2enu  # type: ignore
 
 from roxbot.interfaces import Pose
+import warnings
 
-GPS_REF = (51.0, 6.0)
+# get gps reference from environment variable
+var = os.environ.get("GPS_REF")
+if var is None:
+    GPS_REF = (51.0, 6.0)
+    warnings.warn(f"GPS_REF environment variable not set, using default {GPS_REF}")
+else:
+    vals = var.split(",")
+    assert len(vals) == 2, f"invalid GPS_REF: {var}"
+    GPS_REF = tuple(float(x) for x in vals)  # type: ignore
 
 
 def heading_to_theta(angle_deg: float) -> float:
     """convert gps heading to theta in radians"""
     h = -1j * cmath.rect(1, radians(angle_deg))
     return -cmath.phase(h)
```

### Comparing `roxbot-0.9.0/src/roxbot/models.py` & `roxbot-0.9.1/src/roxbot/models.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.9.0/src/roxbot/vectors.py` & `roxbot-0.9.1/src/roxbot/vectors.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.9.0/src/roxbot/version.py` & `roxbot-0.9.1/src/roxbot/version.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.9.0/src/roxbot.egg-info/SOURCES.txt` & `roxbot-0.9.1/src/roxbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roxbot-0.9.0/tests/test_gps.py` & `roxbot-0.9.1/tests/test_gps.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.9.0/tests/test_models.py` & `roxbot-0.9.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.9.0/tests/test_trike.py` & `roxbot-0.9.1/tests/test_trike.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.9.0/tests/test_vectors.py` & `roxbot-0.9.1/tests/test_vectors.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.9.0/tests/test_ws_bridge.py` & `roxbot-0.9.1/tests/test_ws_bridge.py`

 * *Files identical despite different names*

