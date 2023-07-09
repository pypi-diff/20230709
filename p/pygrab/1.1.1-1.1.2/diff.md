# Comparing `tmp/pygrab-1.1.1.tar.gz` & `tmp/pygrab-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygrab-1.1.1.tar", last modified: Fri Jul  7 04:44:07 2023, max compression
+gzip compressed data, was "pygrab-1.1.2.tar", last modified: Sun Jul  9 21:00:17 2023, max compression
```

## Comparing `pygrab-1.1.1.tar` & `pygrab-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 04:44:07.913000 pygrab-1.1.1/
--rw-rw-rw-   0        0        0      183 2023-07-07 04:44:07.905000 pygrab-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      341 2023-05-31 05:39:20.000000 pygrab-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 04:44:07.840000 pygrab-1.1.1/pygrab/
--rw-rw-rw-   0        0        0       21 2023-05-30 03:16:15.000000 pygrab-1.1.1/pygrab/__init__.py
--rw-rw-rw-   0        0        0     3087 2023-07-07 04:12:12.000000 pygrab-1.1.1/pygrab/proxylist.py
--rw-rw-rw-   0        0        0    15788 2023-07-07 04:40:22.000000 pygrab-1.1.1/pygrab/pygrab.py
-drwxrwxrwx   0        0        0        0 2023-07-07 04:44:07.895000 pygrab-1.1.1/pygrab.egg-info/
--rw-rw-rw-   0        0        0      183 2023-07-07 04:44:07.000000 pygrab-1.1.1/pygrab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-07-07 04:44:07.000000 pygrab-1.1.1/pygrab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 04:44:07.000000 pygrab-1.1.1/pygrab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-07 04:44:07.000000 pygrab-1.1.1/pygrab.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-07 04:44:07.000000 pygrab-1.1.1/pygrab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 04:44:07.911000 pygrab-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      338 2023-07-07 04:43:39.000000 pygrab-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 21:00:17.717000 pygrab-1.1.2/
+-rw-rw-rw-   0        0        0      183 2023-07-09 21:00:17.709000 pygrab-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2023-05-31 05:39:20.000000 pygrab-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 21:00:17.652000 pygrab-1.1.2/pygrab/
+-rw-rw-rw-   0        0        0       21 2023-05-30 03:16:15.000000 pygrab-1.1.2/pygrab/__init__.py
+-rw-rw-rw-   0        0        0     3087 2023-07-07 04:12:12.000000 pygrab-1.1.2/pygrab/proxylist.py
+-rw-rw-rw-   0        0        0    15789 2023-07-09 20:58:03.000000 pygrab-1.1.2/pygrab/pygrab.py
+drwxrwxrwx   0        0        0        0 2023-07-09 21:00:17.701000 pygrab-1.1.2/pygrab.egg-info/
+-rw-rw-rw-   0        0        0      183 2023-07-09 21:00:17.000000 pygrab-1.1.2/pygrab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-07-09 21:00:17.000000 pygrab-1.1.2/pygrab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 21:00:17.000000 pygrab-1.1.2/pygrab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-09 21:00:17.000000 pygrab-1.1.2/pygrab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-09 21:00:17.000000 pygrab-1.1.2/pygrab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-09 21:00:17.715000 pygrab-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      338 2023-07-09 20:58:15.000000 pygrab-1.1.2/setup.py
```

### Comparing `pygrab-1.1.1/pygrab/proxylist.py` & `pygrab-1.1.2/pygrab/proxylist.py`

 * *Files identical despite different names*

### Comparing `pygrab-1.1.1/pygrab/pygrab.py` & `pygrab-1.1.2/pygrab/pygrab.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 modules and functions, ensuring an intuitive and seamless experience 
 in handling various types of web requests, including asynchronous tasks, 
 Javascript-enabled sites, and local requests.
 
 """
 
 
-from proxylist import ProxyList
+from .proxylist import ProxyList
 import requests as _requests
 from pyppeteer import launch as _launch
 import asyncio as _asyncio
 import time as _time
```

