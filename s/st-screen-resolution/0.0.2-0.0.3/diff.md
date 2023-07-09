# Comparing `tmp/st_screen_resolution-0.0.2.tar.gz` & `tmp/st_screen_resolution-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_screen_resolution-0.0.2.tar", last modified: Sun Jul  9 02:40:09 2023, max compression
+gzip compressed data, was "st_screen_resolution-0.0.3.tar", last modified: Sun Jul  9 02:51:30 2023, max compression
```

## Comparing `st_screen_resolution-0.0.2.tar` & `st_screen_resolution-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 02:40:09.668135 st_screen_resolution-0.0.2/
--rw-rw-rw-   0        0        0     1082 2023-07-09 01:25:50.000000 st_screen_resolution-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       58 2023-07-09 01:25:50.000000 st_screen_resolution-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      295 2023-07-09 02:40:09.667622 st_screen_resolution-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-09 02:40:09.668651 st_screen_resolution-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      623 2023-07-09 02:39:35.000000 st_screen_resolution-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-09 02:40:09.658902 st_screen_resolution-0.0.2/st_screen_resolution/
--rw-rw-rw-   0        0        0     3369 2023-07-09 02:25:34.000000 st_screen_resolution-0.0.2/st_screen_resolution/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 02:40:09.666599 st_screen_resolution-0.0.2/st_screen_resolution.egg-info/
--rw-rw-rw-   0        0        0      295 2023-07-09 02:40:09.000000 st_screen_resolution-0.0.2/st_screen_resolution.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-07-09 02:40:09.000000 st_screen_resolution-0.0.2/st_screen_resolution.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 02:40:09.000000 st_screen_resolution-0.0.2/st_screen_resolution.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-09 02:40:09.000000 st_screen_resolution-0.0.2/st_screen_resolution.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-09 02:40:09.000000 st_screen_resolution-0.0.2/st_screen_resolution.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-09 02:51:30.546918 st_screen_resolution-0.0.3/
+-rw-rw-rw-   0        0        0     1082 2023-07-09 01:25:50.000000 st_screen_resolution-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       58 2023-07-09 01:25:50.000000 st_screen_resolution-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      295 2023-07-09 02:51:30.546403 st_screen_resolution-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-09 02:51:30.547435 st_screen_resolution-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      623 2023-07-09 02:51:08.000000 st_screen_resolution-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 02:51:30.523888 st_screen_resolution-0.0.3/st_screen_resolution/
+-rw-rw-rw-   0        0        0     3355 2023-07-09 02:47:54.000000 st_screen_resolution-0.0.3/st_screen_resolution/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 02:51:30.545377 st_screen_resolution-0.0.3/st_screen_resolution.egg-info/
+-rw-rw-rw-   0        0        0      295 2023-07-09 02:51:30.000000 st_screen_resolution-0.0.3/st_screen_resolution.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-07-09 02:51:30.000000 st_screen_resolution-0.0.3/st_screen_resolution.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 02:51:30.000000 st_screen_resolution-0.0.3/st_screen_resolution.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-09 02:51:30.000000 st_screen_resolution-0.0.3/st_screen_resolution.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-09 02:51:30.000000 st_screen_resolution-0.0.3/st_screen_resolution.egg-info/top_level.txt
```

### Comparing `st_screen_resolution-0.0.2/LICENSE` & `st_screen_resolution-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `st_screen_resolution-0.0.2/setup.py` & `st_screen_resolution-0.0.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="st_screen_resolution",
-    version="0.0.2",
+    version="0.0.3",
     author="YM",
     author_email="",
     description="",
     long_description="get screen resolution in streamlit",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `st_screen_resolution-0.0.2/st_screen_resolution/__init__.py` & `st_screen_resolution-0.0.3/st_screen_resolution/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import os
 import streamlit.components.v1 as components
-import requests
 # Create a _RELEASE constant. We'll set this to False while we're developing
 # the component, and True when we're ready to package and distribute it.
 # (This is, of course, optional - there are innumerable ways to manage your
 # release process.)
-_RELEASE = False
+_RELEASE = True
 
 # Declare a Streamlit component. `declare_component` returns a function
 # that is used to create instances of the component. We're naming this
 # function "_component_func", with an underscore prefix, because we don't want
 # to expose it directly to users. Instead, we will create a custom wrapper
 # function, below, that will serve as our component's public API.
 
 # It's worth noting that this call to `declare_component` is the
 # *only thing* you need to do to create the binding between Streamlit and
 # your component frontend. Everything else we do in this file is simply a
 # best practice.
 
-if _RELEASE:
+if not _RELEASE:
     _component_func = components.declare_component(
         # We give the component a simple, descriptive name ("my_component"
         # does not fit this bill, so please choose something better for your
         # own component :)
         "my_component",
         # Pass `url` here to tell Streamlit that the component will be served
         # by the local dev server that you run via `npm run start`.
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-import os import streamlit.components.v1 as components import requests # Create
-a _RELEASE constant. We'll set this to False while we're developing # the
-component, and True when we're ready to package and distribute it. # (This is,
-of course, optional - there are innumerable ways to manage your # release
-process.) _RELEASE = False # Declare a Streamlit component. `declare_component`
-returns a function # that is used to create instances of the component. We're
-naming this # function "_component_func", with an underscore prefix, because we
-don't want # to expose it directly to users. Instead, we will create a custom
-wrapper # function, below, that will serve as our component's public API. #
-It's worth noting that this call to `declare_component` is the # *only thing*
-you need to do to create the binding between Streamlit and # your component
-frontend. Everything else we do in this file is simply a # best practice. if
+import os import streamlit.components.v1 as components # Create a _RELEASE
+constant. We'll set this to False while we're developing # the component, and
+True when we're ready to package and distribute it. # (This is, of course,
+optional - there are innumerable ways to manage your # release process.)
+_RELEASE = True # Declare a Streamlit component. `declare_component` returns a
+function # that is used to create instances of the component. We're naming this
+# function "_component_func", with an underscore prefix, because we don't want
+# to expose it directly to users. Instead, we will create a custom wrapper #
+function, below, that will serve as our component's public API. # It's worth
+noting that this call to `declare_component` is the # *only thing* you need to
+do to create the binding between Streamlit and # your component frontend.
+Everything else we do in this file is simply a # best practice. if not
 _RELEASE: _component_func = components.declare_component( # We give the
 component a simple, descriptive name ("my_component" # does not fit this bill,
 so please choose something better for your # own component :) "my_component", #
 Pass `url` here to tell Streamlit that the component will be served # by the
 local dev server that you run via `npm run start`. # (This is useful while your
 component is in development.) url="http://172.20.0.1:3000/", ) else: # When
 we're distributing a production version of the component, we'll # replace the
```

