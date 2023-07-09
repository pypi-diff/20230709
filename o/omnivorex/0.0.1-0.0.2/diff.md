# Comparing `tmp/omnivorex-0.0.1.tar.gz` & `tmp/omnivorex-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnivorex-0.0.1.tar", last modified: Sun Jul  9 14:05:41 2023, max compression
+gzip compressed data, was "omnivorex-0.0.2.tar", last modified: Sun Jul  9 14:24:42 2023, max compression
```

## Comparing `omnivorex-0.0.1.tar` & `omnivorex-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:05:41.175993 omnivorex-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-09 14:05:36.000000 omnivorex-0.0.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-09 14:05:36.000000 omnivorex-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-09 14:05:36.000000 omnivorex-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-09 14:05:41.175993 omnivorex-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-09 14:05:36.000000 omnivorex-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:05:41.171993 omnivorex-0.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-09 14:05:36.000000 omnivorex-0.0.1/docs/Publish.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:05:41.171993 omnivorex-0.0.1/docs/screenshots/
--rw-r--r--   0 runner    (1001) docker     (123)   167003 2023-07-09 14:05:36.000000 omnivorex-0.0.1/docs/screenshots/omnivorex.png
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-09 14:05:36.000000 omnivorex-0.0.1/docs/textual.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:05:41.175993 omnivorex-0.0.1/omnivorex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-09 14:05:41.000000 omnivorex-0.0.1/omnivorex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-09 14:05:41.000000 omnivorex-0.0.1/omnivorex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 14:05:41.000000 omnivorex-0.0.1/omnivorex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-09 14:05:41.000000 omnivorex-0.0.1/omnivorex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-09 14:05:41.000000 omnivorex-0.0.1/omnivorex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-09 14:05:41.000000 omnivorex-0.0.1/omnivorex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-09 14:05:36.000000 omnivorex-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 14:05:41.175993 omnivorex-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-09 14:05:36.000000 omnivorex-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:05:41.171993 omnivorex-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:05:41.175993 omnivorex-0.0.1/src/omnivorex/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-09 14:05:36.000000 omnivorex-0.0.1/src/omnivorex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-09 14:05:36.000000 omnivorex-0.0.1/src/omnivorex/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-07-09 14:05:36.000000 omnivorex-0.0.1/src/omnivorex/main_screen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:24:42.571819 omnivorex-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-09 14:24:34.000000 omnivorex-0.0.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-09 14:24:34.000000 omnivorex-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-09 14:24:34.000000 omnivorex-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-09 14:24:42.571819 omnivorex-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-09 14:24:34.000000 omnivorex-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:24:42.571819 omnivorex-0.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-09 14:24:34.000000 omnivorex-0.0.2/docs/Publish.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:24:42.571819 omnivorex-0.0.2/docs/screenshots/
+-rw-r--r--   0 runner    (1001) docker     (123)   167003 2023-07-09 14:24:34.000000 omnivorex-0.0.2/docs/screenshots/omnivorex.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-09 14:24:34.000000 omnivorex-0.0.2/docs/textual.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:24:42.571819 omnivorex-0.0.2/omnivorex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-09 14:24:42.000000 omnivorex-0.0.2/omnivorex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-09 14:24:42.000000 omnivorex-0.0.2/omnivorex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 14:24:42.000000 omnivorex-0.0.2/omnivorex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-09 14:24:42.000000 omnivorex-0.0.2/omnivorex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-09 14:24:42.000000 omnivorex-0.0.2/omnivorex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-09 14:24:42.000000 omnivorex-0.0.2/omnivorex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-09 14:24:34.000000 omnivorex-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 14:24:42.571819 omnivorex-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-09 14:24:34.000000 omnivorex-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:24:42.571819 omnivorex-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:24:42.571819 omnivorex-0.0.2/src/omnivorex/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-09 14:24:34.000000 omnivorex-0.0.2/src/omnivorex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-09 14:24:34.000000 omnivorex-0.0.2/src/omnivorex/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-07-09 14:24:34.000000 omnivorex-0.0.2/src/omnivorex/main_screen.py
```

### Comparing `omnivorex-0.0.1/CONTRIBUTING.md` & `omnivorex-0.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `omnivorex-0.0.1/LICENSE` & `omnivorex-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `omnivorex-0.0.1/PKG-INFO` & `omnivorex-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnivorex
-Version: 0.0.1
+Version: 0.0.2
 Summary: Omnivore Terminal App - Text User Interface
 Home-page: https://github.com/yazdipour/OmnivoreX
 Author: Shahriar Yazdipour
 Author-email: git@yazdipour.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/yazdipour/OmnivoreX/issues
 Project-URL: Source Code, https://github.com/yazdipour/OmnivoreX
```

### Comparing `omnivorex-0.0.1/README.md` & `omnivorex-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `omnivorex-0.0.1/docs/Publish.md` & `omnivorex-0.0.2/docs/Publish.md`

 * *Files identical despite different names*

### Comparing `omnivorex-0.0.1/docs/screenshots/omnivorex.png` & `omnivorex-0.0.2/docs/screenshots/omnivorex.png`

 * *Files identical despite different names*

### Comparing `omnivorex-0.0.1/docs/textual.md` & `omnivorex-0.0.2/docs/textual.md`

 * *Files identical despite different names*

### Comparing `omnivorex-0.0.1/omnivorex.egg-info/PKG-INFO` & `omnivorex-0.0.2/omnivorex.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnivorex
-Version: 0.0.1
+Version: 0.0.2
 Summary: Omnivore Terminal App - Text User Interface
 Home-page: https://github.com/yazdipour/OmnivoreX
 Author: Shahriar Yazdipour
 Author-email: git@yazdipour.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/yazdipour/OmnivoreX/issues
 Project-URL: Source Code, https://github.com/yazdipour/OmnivoreX
```

### Comparing `omnivorex-0.0.1/setup.py` & `omnivorex-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `omnivorex-0.0.1/src/omnivorex/main_screen.py` & `omnivorex-0.0.2/src/omnivorex/main_screen.py`

 * *Files identical despite different names*

