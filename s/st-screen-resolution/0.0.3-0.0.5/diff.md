# Comparing `tmp/st_screen_resolution-0.0.3.tar.gz` & `tmp/st_screen_resolution-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_screen_resolution-0.0.3.tar", last modified: Sun Jul  9 02:51:30 2023, max compression
+gzip compressed data, was "st_screen_resolution-0.0.5.tar", last modified: Sun Jul  9 03:11:17 2023, max compression
```

## Comparing `st_screen_resolution-0.0.3.tar` & `st_screen_resolution-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 02:51:30.546918 st_screen_resolution-0.0.3/
--rw-rw-rw-   0        0        0     1082 2023-07-09 01:25:50.000000 st_screen_resolution-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       58 2023-07-09 01:25:50.000000 st_screen_resolution-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      295 2023-07-09 02:51:30.546403 st_screen_resolution-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-09 02:51:30.547435 st_screen_resolution-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      623 2023-07-09 02:51:08.000000 st_screen_resolution-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-09 02:51:30.523888 st_screen_resolution-0.0.3/st_screen_resolution/
--rw-rw-rw-   0        0        0     3355 2023-07-09 02:47:54.000000 st_screen_resolution-0.0.3/st_screen_resolution/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 02:51:30.545377 st_screen_resolution-0.0.3/st_screen_resolution.egg-info/
--rw-rw-rw-   0        0        0      295 2023-07-09 02:51:30.000000 st_screen_resolution-0.0.3/st_screen_resolution.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-07-09 02:51:30.000000 st_screen_resolution-0.0.3/st_screen_resolution.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 02:51:30.000000 st_screen_resolution-0.0.3/st_screen_resolution.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-09 02:51:30.000000 st_screen_resolution-0.0.3/st_screen_resolution.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-09 02:51:30.000000 st_screen_resolution-0.0.3/st_screen_resolution.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-09 03:11:17.760336 st_screen_resolution-0.0.5/
+-rw-rw-rw-   0        0        0     1082 2023-07-09 01:25:50.000000 st_screen_resolution-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0       57 2023-07-09 03:10:41.000000 st_screen_resolution-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      295 2023-07-09 03:11:17.759828 st_screen_resolution-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-09 03:11:17.760336 st_screen_resolution-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      623 2023-07-09 03:11:09.000000 st_screen_resolution-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 03:11:17.732190 st_screen_resolution-0.0.5/st_screen_resolution/
+-rw-rw-rw-   0        0        0     3355 2023-07-09 02:47:54.000000 st_screen_resolution-0.0.5/st_screen_resolution/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 03:11:17.727064 st_screen_resolution-0.0.5/st_screen_resolution/frontend/
+drwxrwxrwx   0        0        0        0 2023-07-09 03:11:17.748041 st_screen_resolution-0.0.5/st_screen_resolution/frontend/build/
+-rw-rw-rw-   0        0        0      691 2023-07-09 03:07:16.000000 st_screen_resolution-0.0.5/st_screen_resolution/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0   206960 2023-07-09 01:25:50.000000 st_screen_resolution-0.0.5/st_screen_resolution/frontend/build/bootstrap.min.css
+-rw-rw-rw-   0        0        0     2087 2023-07-09 03:07:16.000000 st_screen_resolution-0.0.5/st_screen_resolution/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2023-07-09 03:11:17.728093 st_screen_resolution-0.0.5/st_screen_resolution/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2023-07-09 03:11:17.758301 st_screen_resolution-0.0.5/st_screen_resolution/frontend/build/static/js/
+-rw-rw-rw-   0        0        0   464228 2023-07-09 03:07:16.000000 st_screen_resolution-0.0.5/st_screen_resolution/frontend/build/static/js/2.409ed399.chunk.js
+-rw-rw-rw-   0        0        0     2059 2023-07-09 03:07:16.000000 st_screen_resolution-0.0.5/st_screen_resolution/frontend/build/static/js/2.409ed399.chunk.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  1600815 2023-07-09 03:07:16.000000 st_screen_resolution-0.0.5/st_screen_resolution/frontend/build/static/js/2.409ed399.chunk.js.map
+-rw-rw-rw-   0        0        0     1093 2023-07-09 03:07:16.000000 st_screen_resolution-0.0.5/st_screen_resolution/frontend/build/static/js/main.1a50ca2c.chunk.js
+-rw-rw-rw-   0        0        0     2794 2023-07-09 03:07:16.000000 st_screen_resolution-0.0.5/st_screen_resolution/frontend/build/static/js/main.1a50ca2c.chunk.js.map
+-rw-rw-rw-   0        0        0     1584 2023-07-09 03:07:16.000000 st_screen_resolution-0.0.5/st_screen_resolution/frontend/build/static/js/runtime-main.0f051bbb.js
+-rw-rw-rw-   0        0        0     8369 2023-07-09 03:07:16.000000 st_screen_resolution-0.0.5/st_screen_resolution/frontend/build/static/js/runtime-main.0f051bbb.js.map
+drwxrwxrwx   0        0        0        0 2023-07-09 03:11:17.743934 st_screen_resolution-0.0.5/st_screen_resolution.egg-info/
+-rw-rw-rw-   0        0        0      295 2023-07-09 03:11:17.000000 st_screen_resolution-0.0.5/st_screen_resolution.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      939 2023-07-09 03:11:17.000000 st_screen_resolution-0.0.5/st_screen_resolution.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 03:11:17.000000 st_screen_resolution-0.0.5/st_screen_resolution.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-09 03:11:17.000000 st_screen_resolution-0.0.5/st_screen_resolution.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-09 03:11:17.000000 st_screen_resolution-0.0.5/st_screen_resolution.egg-info/top_level.txt
```

### Comparing `st_screen_resolution-0.0.3/LICENSE` & `st_screen_resolution-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `st_screen_resolution-0.0.3/setup.py` & `st_screen_resolution-0.0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="st_screen_resolution",
-    version="0.0.3",
+    version="0.0.5",
     author="YM",
     author_email="",
     description="",
     long_description="get screen resolution in streamlit",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `st_screen_resolution-0.0.3/st_screen_resolution/__init__.py` & `st_screen_resolution-0.0.5/st_screen_resolution/__init__.py`

 * *Files identical despite different names*

