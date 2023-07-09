# Comparing `tmp/st_screen_resolution-0.0.1.tar.gz` & `tmp/st_screen_resolution-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_screen_resolution-0.0.1.tar", last modified: Sun Jul  9 02:27:35 2023, max compression
+gzip compressed data, was "st_screen_resolution-0.0.2.tar", last modified: Sun Jul  9 02:40:09 2023, max compression
```

## Comparing `st_screen_resolution-0.0.1.tar` & `st_screen_resolution-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 02:27:35.216977 st_screen_resolution-0.0.1/
--rw-rw-rw-   0        0        0     1082 2023-07-09 01:25:50.000000 st_screen_resolution-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       58 2023-07-09 01:25:50.000000 st_screen_resolution-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      295 2023-07-09 02:27:35.215949 st_screen_resolution-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-09 02:27:35.216977 st_screen_resolution-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      623 2023-07-09 02:21:50.000000 st_screen_resolution-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-09 02:27:35.139663 st_screen_resolution-0.0.1/st_blogpost_component/
--rw-rw-rw-   0        0        0     3369 2023-07-09 02:25:34.000000 st_screen_resolution-0.0.1/st_blogpost_component/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 02:27:35.126303 st_screen_resolution-0.0.1/st_blogpost_component/frontend/
-drwxrwxrwx   0        0        0        0 2023-07-09 02:27:35.149408 st_screen_resolution-0.0.1/st_blogpost_component/frontend/build/
--rw-rw-rw-   0        0        0      691 2023-07-09 02:24:28.000000 st_screen_resolution-0.0.1/st_blogpost_component/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0   206960 2023-07-09 01:25:50.000000 st_screen_resolution-0.0.1/st_blogpost_component/frontend/build/bootstrap.min.css
--rw-rw-rw-   0        0        0     2087 2023-07-09 02:24:28.000000 st_screen_resolution-0.0.1/st_blogpost_component/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2023-07-09 02:27:35.126816 st_screen_resolution-0.0.1/st_blogpost_component/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2023-07-09 02:27:35.190370 st_screen_resolution-0.0.1/st_blogpost_component/frontend/build/static/js/
--rw-rw-rw-   0        0        0   464228 2023-07-09 02:24:28.000000 st_screen_resolution-0.0.1/st_blogpost_component/frontend/build/static/js/2.dcb7ef86.chunk.js
--rw-rw-rw-   0        0        0     2059 2023-07-09 02:24:28.000000 st_screen_resolution-0.0.1/st_blogpost_component/frontend/build/static/js/2.dcb7ef86.chunk.js.LICENSE.txt
--rw-rw-rw-   0        0        0  1600815 2023-07-09 02:24:28.000000 st_screen_resolution-0.0.1/st_blogpost_component/frontend/build/static/js/2.dcb7ef86.chunk.js.map
--rw-rw-rw-   0        0        0     1093 2023-07-09 02:24:28.000000 st_screen_resolution-0.0.1/st_blogpost_component/frontend/build/static/js/main.061ca5f4.chunk.js
--rw-rw-rw-   0        0        0     2794 2023-07-09 02:24:28.000000 st_screen_resolution-0.0.1/st_blogpost_component/frontend/build/static/js/main.061ca5f4.chunk.js.map
--rw-rw-rw-   0        0        0     1584 2023-07-09 02:24:28.000000 st_screen_resolution-0.0.1/st_blogpost_component/frontend/build/static/js/runtime-main.0f051bbb.js
--rw-rw-rw-   0        0        0     8369 2023-07-09 02:24:28.000000 st_screen_resolution-0.0.1/st_blogpost_component/frontend/build/static/js/runtime-main.0f051bbb.js.map
-drwxrwxrwx   0        0        0        0 2023-07-09 02:27:35.214412 st_screen_resolution-0.0.1/st_screen_resolution.egg-info/
--rw-rw-rw-   0        0        0      295 2023-07-09 02:27:35.000000 st_screen_resolution-0.0.1/st_screen_resolution.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      950 2023-07-09 02:27:35.000000 st_screen_resolution-0.0.1/st_screen_resolution.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 02:27:35.000000 st_screen_resolution-0.0.1/st_screen_resolution.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-09 02:27:35.000000 st_screen_resolution-0.0.1/st_screen_resolution.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-09 02:27:35.000000 st_screen_resolution-0.0.1/st_screen_resolution.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-09 02:40:09.668135 st_screen_resolution-0.0.2/
+-rw-rw-rw-   0        0        0     1082 2023-07-09 01:25:50.000000 st_screen_resolution-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       58 2023-07-09 01:25:50.000000 st_screen_resolution-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      295 2023-07-09 02:40:09.667622 st_screen_resolution-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-09 02:40:09.668651 st_screen_resolution-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      623 2023-07-09 02:39:35.000000 st_screen_resolution-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 02:40:09.658902 st_screen_resolution-0.0.2/st_screen_resolution/
+-rw-rw-rw-   0        0        0     3369 2023-07-09 02:25:34.000000 st_screen_resolution-0.0.2/st_screen_resolution/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 02:40:09.666599 st_screen_resolution-0.0.2/st_screen_resolution.egg-info/
+-rw-rw-rw-   0        0        0      295 2023-07-09 02:40:09.000000 st_screen_resolution-0.0.2/st_screen_resolution.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-07-09 02:40:09.000000 st_screen_resolution-0.0.2/st_screen_resolution.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 02:40:09.000000 st_screen_resolution-0.0.2/st_screen_resolution.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-09 02:40:09.000000 st_screen_resolution-0.0.2/st_screen_resolution.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-09 02:40:09.000000 st_screen_resolution-0.0.2/st_screen_resolution.egg-info/top_level.txt
```

### Comparing `st_screen_resolution-0.0.1/LICENSE` & `st_screen_resolution-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `st_screen_resolution-0.0.1/setup.py` & `st_screen_resolution-0.0.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="st_screen_resolution",
-    version="0.0.1",
+    version="0.0.2",
     author="YM",
     author_email="",
     description="",
     long_description="get screen resolution in streamlit",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `st_screen_resolution-0.0.1/st_blogpost_component/__init__.py` & `st_screen_resolution-0.0.2/st_screen_resolution/__init__.py`

 * *Files identical despite different names*

