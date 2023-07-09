# Comparing `tmp/omnivorex-0.0.5.tar.gz` & `tmp/omnivorex-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnivorex-0.0.5.tar", last modified: Sun Jul  9 15:16:54 2023, max compression
+gzip compressed data, was "omnivorex-0.0.6.tar", last modified: Sun Jul  9 15:29:12 2023, max compression
```

## Comparing `omnivorex-0.0.5.tar` & `omnivorex-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:16:54.607251 omnivorex-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-09 15:16:45.000000 omnivorex-0.0.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-09 15:16:45.000000 omnivorex-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-09 15:16:45.000000 omnivorex-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-09 15:16:54.607251 omnivorex-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-09 15:16:45.000000 omnivorex-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:16:54.603251 omnivorex-0.0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-09 15:16:45.000000 omnivorex-0.0.5/docs/Publish.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:16:54.603251 omnivorex-0.0.5/docs/screenshots/
--rw-r--r--   0 runner    (1001) docker     (123)   167003 2023-07-09 15:16:45.000000 omnivorex-0.0.5/docs/screenshots/omnivorex.png
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-09 15:16:45.000000 omnivorex-0.0.5/docs/textual.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:16:54.603251 omnivorex-0.0.5/omnivorex/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-09 15:16:45.000000 omnivorex-0.0.5/omnivorex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-07-09 15:16:45.000000 omnivorex-0.0.5/omnivorex/omnivorex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:16:54.607251 omnivorex-0.0.5/omnivorex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-09 15:16:54.000000 omnivorex-0.0.5/omnivorex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-09 15:16:54.000000 omnivorex-0.0.5/omnivorex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 15:16:54.000000 omnivorex-0.0.5/omnivorex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-09 15:16:54.000000 omnivorex-0.0.5/omnivorex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-09 15:16:54.000000 omnivorex-0.0.5/omnivorex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-09 15:16:54.000000 omnivorex-0.0.5/omnivorex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-09 15:16:45.000000 omnivorex-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 15:16:54.607251 omnivorex-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-09 15:16:45.000000 omnivorex-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:29:12.541040 omnivorex-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-09 15:29:08.000000 omnivorex-0.0.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-09 15:29:08.000000 omnivorex-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-09 15:29:08.000000 omnivorex-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-09 15:29:12.541040 omnivorex-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-09 15:29:08.000000 omnivorex-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:29:12.541040 omnivorex-0.0.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-09 15:29:08.000000 omnivorex-0.0.6/docs/Publish.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:29:12.541040 omnivorex-0.0.6/docs/screenshots/
+-rw-r--r--   0 runner    (1001) docker     (123)   167003 2023-07-09 15:29:08.000000 omnivorex-0.0.6/docs/screenshots/omnivorex.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-09 15:29:08.000000 omnivorex-0.0.6/docs/textual.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:29:12.541040 omnivorex-0.0.6/omnivorex/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-09 15:29:08.000000 omnivorex-0.0.6/omnivorex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-07-09 15:29:08.000000 omnivorex-0.0.6/omnivorex/omnivorex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:29:12.541040 omnivorex-0.0.6/omnivorex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-09 15:29:12.000000 omnivorex-0.0.6/omnivorex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-09 15:29:12.000000 omnivorex-0.0.6/omnivorex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 15:29:12.000000 omnivorex-0.0.6/omnivorex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-09 15:29:12.000000 omnivorex-0.0.6/omnivorex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-09 15:29:12.000000 omnivorex-0.0.6/omnivorex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-09 15:29:12.000000 omnivorex-0.0.6/omnivorex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-09 15:29:08.000000 omnivorex-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 15:29:12.541040 omnivorex-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-09 15:29:08.000000 omnivorex-0.0.6/setup.py
```

### Comparing `omnivorex-0.0.5/CONTRIBUTING.md` & `omnivorex-0.0.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `omnivorex-0.0.5/LICENSE` & `omnivorex-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `omnivorex-0.0.5/PKG-INFO` & `omnivorex-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnivorex
-Version: 0.0.5
+Version: 0.0.6
 Summary: Omnivore Terminal App - Text User Interface
 Home-page: https://github.com/yazdipour/OmnivoreX
 Author: Shahriar Yazdipour
 Author-email: git@yazdipour.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/yazdipour/OmnivoreX/issues
 Project-URL: Source Code, https://github.com/yazdipour/OmnivoreX
```

### Comparing `omnivorex-0.0.5/README.md` & `omnivorex-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `omnivorex-0.0.5/docs/Publish.md` & `omnivorex-0.0.6/docs/Publish.md`

 * *Files identical despite different names*

### Comparing `omnivorex-0.0.5/docs/screenshots/omnivorex.png` & `omnivorex-0.0.6/docs/screenshots/omnivorex.png`

 * *Files identical despite different names*

### Comparing `omnivorex-0.0.5/docs/textual.md` & `omnivorex-0.0.6/docs/textual.md`

 * *Files identical despite different names*

### Comparing `omnivorex-0.0.5/omnivorex/omnivorex.py` & `omnivorex-0.0.6/omnivorex/omnivorex.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,17 +4,17 @@
     Header,
     Button,
     MarkdownViewer,
     ListView,
 )
 from textual.containers import Container
 import os
-from .components.login_screen import LoginScreen
-from .components.article_item import ArticleItem
-from .utils import _omnivoerql_utils
+from article_item import ArticleItem
+from login_screen import LoginScreen
+from utils import _omnivoerql_utils
 
 
 class OmnivoreX(App):
     TITLE = "OmnivoreX"
     CSS_PATH = "main_screen.css"
     DEFAULT_LIMIT = 42
     OPENED_ARTICLE: ArticleItem = None
```

### Comparing `omnivorex-0.0.5/omnivorex.egg-info/PKG-INFO` & `omnivorex-0.0.6/omnivorex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnivorex
-Version: 0.0.5
+Version: 0.0.6
 Summary: Omnivore Terminal App - Text User Interface
 Home-page: https://github.com/yazdipour/OmnivoreX
 Author: Shahriar Yazdipour
 Author-email: git@yazdipour.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/yazdipour/OmnivoreX/issues
 Project-URL: Source Code, https://github.com/yazdipour/OmnivoreX
```

### Comparing `omnivorex-0.0.5/setup.py` & `omnivorex-0.0.6/setup.py`

 * *Files identical despite different names*

