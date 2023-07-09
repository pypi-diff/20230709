# Comparing `tmp/pyipp-0.9.1.tar.gz` & `tmp/pyipp-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyipp-0.9.1.tar", last modified: Wed Apr  8 17:47:42 2020, max compression
+gzip compressed data, was "dist/pyipp-0.9.2.tar", last modified: Fri Apr 10 05:12:29 2020, max compression
```

## Comparing `pyipp-0.9.1.tar` & `pyipp-0.9.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-08 17:47:42.723843 pyipp-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (116)       78 2020-04-08 17:47:36.000000 pyipp-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     1750 2020-04-08 17:47:42.723843 pyipp-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      682 2020-04-08 17:47:36.000000 pyipp-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-08 17:47:42.723843 pyipp-0.9.1/pyipp/
--rw-r--r--   0 runner    (1001) docker     (116)      229 2020-04-08 17:47:36.000000 pyipp-0.9.1/pyipp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       65 2020-04-08 17:47:36.000000 pyipp-0.9.1/pyipp/__version__.py
--rw-r--r--   0 runner    (1001) docker     (116)      760 2020-04-08 17:47:36.000000 pyipp-0.9.1/pyipp/const.py
--rw-r--r--   0 runner    (1001) docker     (116)     7733 2020-04-08 17:47:36.000000 pyipp-0.9.1/pyipp/enums.py
--rw-r--r--   0 runner    (1001) docker     (116)      438 2020-04-08 17:47:36.000000 pyipp-0.9.1/pyipp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     7327 2020-04-08 17:47:36.000000 pyipp-0.9.1/pyipp/ipp.py
--rw-r--r--   0 runner    (1001) docker     (116)     4564 2020-04-08 17:47:36.000000 pyipp-0.9.1/pyipp/models.py
--rw-r--r--   0 runner    (1001) docker     (116)     9193 2020-04-08 17:47:36.000000 pyipp-0.9.1/pyipp/parser.py
--rw-r--r--   0 runner    (1001) docker     (116)     2743 2020-04-08 17:47:36.000000 pyipp-0.9.1/pyipp/serializer.py
--rw-r--r--   0 runner    (1001) docker     (116)     1460 2020-04-08 17:47:36.000000 pyipp-0.9.1/pyipp/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-08 17:47:42.723843 pyipp-0.9.1/pyipp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1750 2020-04-08 17:47:42.000000 pyipp-0.9.1/pyipp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      370 2020-04-08 17:47:42.000000 pyipp-0.9.1/pyipp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-04-08 17:47:42.000000 pyipp-0.9.1/pyipp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-04-08 17:47:42.000000 pyipp-0.9.1/pyipp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       44 2020-04-08 17:47:42.000000 pyipp-0.9.1/pyipp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        6 2020-04-08 17:47:42.000000 pyipp-0.9.1/pyipp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-04-08 17:47:42.723843 pyipp-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1728 2020-04-08 17:47:36.000000 pyipp-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-10 05:12:29.215235 pyipp-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (116)       78 2020-04-10 05:12:18.000000 pyipp-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     1750 2020-04-10 05:12:29.215235 pyipp-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      682 2020-04-10 05:12:18.000000 pyipp-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-10 05:12:29.215235 pyipp-0.9.2/pyipp/
+-rw-r--r--   0 runner    (1001) docker     (116)      229 2020-04-10 05:12:18.000000 pyipp-0.9.2/pyipp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)       65 2020-04-10 05:12:18.000000 pyipp-0.9.2/pyipp/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      760 2020-04-10 05:12:18.000000 pyipp-0.9.2/pyipp/const.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7733 2020-04-10 05:12:18.000000 pyipp-0.9.2/pyipp/enums.py
+-rw-r--r--   0 runner    (1001) docker     (116)      438 2020-04-10 05:12:18.000000 pyipp-0.9.2/pyipp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7327 2020-04-10 05:12:18.000000 pyipp-0.9.2/pyipp/ipp.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5225 2020-04-10 05:12:18.000000 pyipp-0.9.2/pyipp/models.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9193 2020-04-10 05:12:18.000000 pyipp-0.9.2/pyipp/parser.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2743 2020-04-10 05:12:18.000000 pyipp-0.9.2/pyipp/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1460 2020-04-10 05:12:18.000000 pyipp-0.9.2/pyipp/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-10 05:12:29.215235 pyipp-0.9.2/pyipp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     1750 2020-04-10 05:12:29.000000 pyipp-0.9.2/pyipp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      370 2020-04-10 05:12:29.000000 pyipp-0.9.2/pyipp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-04-10 05:12:29.000000 pyipp-0.9.2/pyipp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-04-10 05:12:29.000000 pyipp-0.9.2/pyipp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)       44 2020-04-10 05:12:29.000000 pyipp-0.9.2/pyipp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        6 2020-04-10 05:12:29.000000 pyipp-0.9.2/pyipp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2020-04-10 05:12:29.215235 pyipp-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1728 2020-04-10 05:12:18.000000 pyipp-0.9.2/setup.py
```

### Comparing `pyipp-0.9.1/PKG-INFO` & `pyipp-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyipp
-Version: 0.9.1
+Version: 0.9.2
 Summary: Asynchronous Python client for Internet Printing Protocol (IPP).
 Home-page: https://github.com/ctalkington/python-ipp
 Author: Chris Talkington
 Author-email: chris@talkingtontech.com
 License: MIT license
 Description: # Python: Internet Printing Protocol (IPP) Client
```

### Comparing `pyipp-0.9.1/README.md` & `pyipp-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `pyipp-0.9.1/pyipp/const.py` & `pyipp-0.9.2/pyipp/const.py`

 * *Files identical despite different names*

### Comparing `pyipp-0.9.1/pyipp/enums.py` & `pyipp-0.9.2/pyipp/enums.py`

 * *Files identical despite different names*

### Comparing `pyipp-0.9.1/pyipp/ipp.py` & `pyipp-0.9.2/pyipp/ipp.py`

 * *Files identical despite different names*

### Comparing `pyipp-0.9.1/pyipp/models.py` & `pyipp-0.9.2/pyipp/models.py`

 * *Files 19% similar despite different names*

```diff
@@ -110,50 +110,69 @@
     markers: List[Marker]
     state: State
 
     @staticmethod
     def from_dict(data):
         """Return Printer object from IPP response."""
         markers = []
+        mlen = 0
         marker_colors = []
         marker_levels = []
         marker_types = []
         marker_highs = []
         marker_lows = []
 
         marker_names = None
         if isinstance(data.get("marker-names"), List):
             marker_names = data["marker-names"]
+            mlen = len(marker_names)
+
+            for k in range(mlen):
+                marker_colors.append("")
+                marker_levels.append(-2)
+                marker_types.append("unknown")
+                marker_highs.append(100)
+                marker_lows.append(0)
 
         if isinstance(data.get("marker-colors"), List):
-            marker_colors = data["marker-colors"]
+            for k, v in enumerate(data["marker-colors"]):
+                if k < mlen:
+                    marker_colors[k] = v
 
         if isinstance(data.get("marker-levels"), List):
-            marker_levels = data["marker-levels"]
+            for k, v in enumerate(data["marker-levels"]):
+                if k < mlen:
+                    marker_levels[k] = v
 
         if isinstance(data.get("marker-high-levels"), List):
-            marker_highs = data["marker-high-levels"]
+            for k, v in enumerate(data["marker-high-levels"]):
+                if k < mlen:
+                    marker_highs[k] = v
 
         if isinstance(data.get("marker-low-levels"), List):
-            marker_lows = data["marker-low-levels"]
+            for k, v in enumerate(data["marker-low-levels"]):
+                if k < mlen:
+                    marker_lows[k] = v
 
         if isinstance(data.get("marker-types"), List):
-            marker_types = data["marker-types"]
+            for k, v in enumerate(data["marker-types"]):
+                if k < mlen:
+                    marker_types[k] = v
 
-        if isinstance(marker_names, List) and len(marker_names) > 0:
+        if isinstance(marker_names, List) and mlen > 0:
             markers = [
                 Marker(
                     marker_id=marker_id,
                     marker_type=marker_types[marker_id],
                     name=marker_names[marker_id],
                     color=marker_colors[marker_id],
                     level=marker_levels[marker_id],
                     high_level=marker_highs[marker_id],
                     low_level=marker_lows[marker_id],
                 )
-                for marker_id in range(len(marker_names))
+                for marker_id in range(mlen)
             ]
             markers.sort(key=lambda x: x.name)
 
         return Printer(
             info=Info.from_dict(data), markers=markers, state=State.from_dict(data)
         )
```

### Comparing `pyipp-0.9.1/pyipp/parser.py` & `pyipp-0.9.2/pyipp/parser.py`

 * *Files identical despite different names*

### Comparing `pyipp-0.9.1/pyipp/serializer.py` & `pyipp-0.9.2/pyipp/serializer.py`

 * *Files identical despite different names*

### Comparing `pyipp-0.9.1/pyipp/tags.py` & `pyipp-0.9.2/pyipp/tags.py`

 * *Files identical despite different names*

### Comparing `pyipp-0.9.1/pyipp.egg-info/PKG-INFO` & `pyipp-0.9.2/pyipp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyipp
-Version: 0.9.1
+Version: 0.9.2
 Summary: Asynchronous Python client for Internet Printing Protocol (IPP).
 Home-page: https://github.com/ctalkington/python-ipp
 Author: Chris Talkington
 Author-email: chris@talkingtontech.com
 License: MIT license
 Description: # Python: Internet Printing Protocol (IPP) Client
```

### Comparing `pyipp-0.9.1/setup.py` & `pyipp-0.9.2/setup.py`

 * *Files identical despite different names*

