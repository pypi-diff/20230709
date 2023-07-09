# Comparing `tmp/omnivorex-0.0.3.tar.gz` & `tmp/omnivorex-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnivorex-0.0.3.tar", last modified: Sun Jul  9 14:31:27 2023, max compression
+gzip compressed data, was "omnivorex-0.0.4.tar", last modified: Sun Jul  9 14:35:20 2023, max compression
```

## Comparing `omnivorex-0.0.3.tar` & `omnivorex-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:31:27.525086 omnivorex-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-09 14:31:22.000000 omnivorex-0.0.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-09 14:31:22.000000 omnivorex-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-09 14:31:22.000000 omnivorex-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-09 14:31:27.525086 omnivorex-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-09 14:31:22.000000 omnivorex-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:31:27.525086 omnivorex-0.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-09 14:31:22.000000 omnivorex-0.0.3/docs/Publish.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:31:27.525086 omnivorex-0.0.3/docs/screenshots/
--rw-r--r--   0 runner    (1001) docker     (123)   167003 2023-07-09 14:31:22.000000 omnivorex-0.0.3/docs/screenshots/omnivorex.png
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-09 14:31:22.000000 omnivorex-0.0.3/docs/textual.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:31:27.525086 omnivorex-0.0.3/omnivorex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-09 14:31:27.000000 omnivorex-0.0.3/omnivorex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-09 14:31:27.000000 omnivorex-0.0.3/omnivorex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 14:31:27.000000 omnivorex-0.0.3/omnivorex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-09 14:31:27.000000 omnivorex-0.0.3/omnivorex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-09 14:31:27.000000 omnivorex-0.0.3/omnivorex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-09 14:31:27.000000 omnivorex-0.0.3/omnivorex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-09 14:31:22.000000 omnivorex-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 14:31:27.529086 omnivorex-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-09 14:31:22.000000 omnivorex-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:31:27.525086 omnivorex-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:31:27.525086 omnivorex-0.0.3/src/omnivorex/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-09 14:31:22.000000 omnivorex-0.0.3/src/omnivorex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-09 14:31:22.000000 omnivorex-0.0.3/src/omnivorex/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-07-09 14:31:22.000000 omnivorex-0.0.3/src/omnivorex/main_screen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:35:20.478670 omnivorex-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-09 14:35:16.000000 omnivorex-0.0.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-09 14:35:16.000000 omnivorex-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-09 14:35:16.000000 omnivorex-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-09 14:35:20.478670 omnivorex-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-09 14:35:16.000000 omnivorex-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:35:20.478670 omnivorex-0.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-09 14:35:16.000000 omnivorex-0.0.4/docs/Publish.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:35:20.478670 omnivorex-0.0.4/docs/screenshots/
+-rw-r--r--   0 runner    (1001) docker     (123)   167003 2023-07-09 14:35:16.000000 omnivorex-0.0.4/docs/screenshots/omnivorex.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-09 14:35:16.000000 omnivorex-0.0.4/docs/textual.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:35:20.478670 omnivorex-0.0.4/omnivorex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-09 14:35:20.000000 omnivorex-0.0.4/omnivorex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-09 14:35:20.000000 omnivorex-0.0.4/omnivorex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 14:35:20.000000 omnivorex-0.0.4/omnivorex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-09 14:35:20.000000 omnivorex-0.0.4/omnivorex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-09 14:35:20.000000 omnivorex-0.0.4/omnivorex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-09 14:35:20.000000 omnivorex-0.0.4/omnivorex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-09 14:35:16.000000 omnivorex-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 14:35:20.478670 omnivorex-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-09 14:35:16.000000 omnivorex-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:35:20.478670 omnivorex-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:35:20.478670 omnivorex-0.0.4/src/omnivorex/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-09 14:35:16.000000 omnivorex-0.0.4/src/omnivorex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-09 14:35:16.000000 omnivorex-0.0.4/src/omnivorex/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-09 14:35:16.000000 omnivorex-0.0.4/src/omnivorex/main_screen.py
```

### Comparing `omnivorex-0.0.3/CONTRIBUTING.md` & `omnivorex-0.0.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `omnivorex-0.0.3/LICENSE` & `omnivorex-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `omnivorex-0.0.3/PKG-INFO` & `omnivorex-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnivorex
-Version: 0.0.3
+Version: 0.0.4
 Summary: Omnivore Terminal App - Text User Interface
 Home-page: https://github.com/yazdipour/OmnivoreX
 Author: Shahriar Yazdipour
 Author-email: git@yazdipour.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/yazdipour/OmnivoreX/issues
 Project-URL: Source Code, https://github.com/yazdipour/OmnivoreX
```

### Comparing `omnivorex-0.0.3/README.md` & `omnivorex-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `omnivorex-0.0.3/docs/Publish.md` & `omnivorex-0.0.4/docs/Publish.md`

 * *Files identical despite different names*

### Comparing `omnivorex-0.0.3/docs/screenshots/omnivorex.png` & `omnivorex-0.0.4/docs/screenshots/omnivorex.png`

 * *Files identical despite different names*

### Comparing `omnivorex-0.0.3/docs/textual.md` & `omnivorex-0.0.4/docs/textual.md`

 * *Files identical despite different names*

### Comparing `omnivorex-0.0.3/omnivorex.egg-info/PKG-INFO` & `omnivorex-0.0.4/omnivorex.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnivorex
-Version: 0.0.3
+Version: 0.0.4
 Summary: Omnivore Terminal App - Text User Interface
 Home-page: https://github.com/yazdipour/OmnivoreX
 Author: Shahriar Yazdipour
 Author-email: git@yazdipour.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/yazdipour/OmnivoreX/issues
 Project-URL: Source Code, https://github.com/yazdipour/OmnivoreX
```

### Comparing `omnivorex-0.0.3/setup.py` & `omnivorex-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `omnivorex-0.0.3/src/omnivorex/main_screen.py` & `omnivorex-0.0.4/src/omnivorex/main_screen.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
     Label,
 )
 from textual.containers import Container, Horizontal, ScrollableContainer, Grid
 from textual.reactive import reactive
 from textual.screen import ModalScreen
 from textual import on
 import os
-from components.login_screen import LoginScreen
-from components.article_item import ArticleItem
-from utils import _omnivoerql_utils
+from .components.login_screen import LoginScreen
+from .components.article_item import ArticleItem
+from .utils import _omnivoerql_utils
 
 
 class OmnivoreX(App):
     TITLE = "OmnivoreX"
     CSS_PATH = "main_screen.css"
     DEFAULT_LIMIT = 42
     OPENED_ARTICLE: ArticleItem = None
```

