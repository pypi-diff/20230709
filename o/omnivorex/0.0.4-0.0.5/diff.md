# Comparing `tmp/omnivorex-0.0.4.tar.gz` & `tmp/omnivorex-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnivorex-0.0.4.tar", last modified: Sun Jul  9 14:35:20 2023, max compression
+gzip compressed data, was "omnivorex-0.0.5.tar", last modified: Sun Jul  9 15:16:54 2023, max compression
```

## Comparing `omnivorex-0.0.4.tar` & `omnivorex-0.0.5.tar`

### file list

```diff
@@ -1,26 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:35:20.478670 omnivorex-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-09 14:35:16.000000 omnivorex-0.0.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-09 14:35:16.000000 omnivorex-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-09 14:35:16.000000 omnivorex-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-09 14:35:20.478670 omnivorex-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-09 14:35:16.000000 omnivorex-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:35:20.478670 omnivorex-0.0.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-09 14:35:16.000000 omnivorex-0.0.4/docs/Publish.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:35:20.478670 omnivorex-0.0.4/docs/screenshots/
--rw-r--r--   0 runner    (1001) docker     (123)   167003 2023-07-09 14:35:16.000000 omnivorex-0.0.4/docs/screenshots/omnivorex.png
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-09 14:35:16.000000 omnivorex-0.0.4/docs/textual.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:35:20.478670 omnivorex-0.0.4/omnivorex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-09 14:35:20.000000 omnivorex-0.0.4/omnivorex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-09 14:35:20.000000 omnivorex-0.0.4/omnivorex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 14:35:20.000000 omnivorex-0.0.4/omnivorex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-09 14:35:20.000000 omnivorex-0.0.4/omnivorex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-09 14:35:20.000000 omnivorex-0.0.4/omnivorex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-09 14:35:20.000000 omnivorex-0.0.4/omnivorex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-09 14:35:16.000000 omnivorex-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 14:35:20.478670 omnivorex-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-09 14:35:16.000000 omnivorex-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:35:20.478670 omnivorex-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:35:20.478670 omnivorex-0.0.4/src/omnivorex/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-09 14:35:16.000000 omnivorex-0.0.4/src/omnivorex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-09 14:35:16.000000 omnivorex-0.0.4/src/omnivorex/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-09 14:35:16.000000 omnivorex-0.0.4/src/omnivorex/main_screen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:16:54.607251 omnivorex-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-09 15:16:45.000000 omnivorex-0.0.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-09 15:16:45.000000 omnivorex-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-09 15:16:45.000000 omnivorex-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-09 15:16:54.607251 omnivorex-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-09 15:16:45.000000 omnivorex-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:16:54.603251 omnivorex-0.0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-09 15:16:45.000000 omnivorex-0.0.5/docs/Publish.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:16:54.603251 omnivorex-0.0.5/docs/screenshots/
+-rw-r--r--   0 runner    (1001) docker     (123)   167003 2023-07-09 15:16:45.000000 omnivorex-0.0.5/docs/screenshots/omnivorex.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-09 15:16:45.000000 omnivorex-0.0.5/docs/textual.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:16:54.603251 omnivorex-0.0.5/omnivorex/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-09 15:16:45.000000 omnivorex-0.0.5/omnivorex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-07-09 15:16:45.000000 omnivorex-0.0.5/omnivorex/omnivorex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:16:54.607251 omnivorex-0.0.5/omnivorex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-09 15:16:54.000000 omnivorex-0.0.5/omnivorex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-09 15:16:54.000000 omnivorex-0.0.5/omnivorex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 15:16:54.000000 omnivorex-0.0.5/omnivorex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-09 15:16:54.000000 omnivorex-0.0.5/omnivorex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-09 15:16:54.000000 omnivorex-0.0.5/omnivorex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-09 15:16:54.000000 omnivorex-0.0.5/omnivorex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-09 15:16:45.000000 omnivorex-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 15:16:54.607251 omnivorex-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-09 15:16:45.000000 omnivorex-0.0.5/setup.py
```

### Comparing `omnivorex-0.0.4/CONTRIBUTING.md` & `omnivorex-0.0.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `omnivorex-0.0.4/LICENSE` & `omnivorex-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `omnivorex-0.0.4/PKG-INFO` & `omnivorex-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnivorex
-Version: 0.0.4
+Version: 0.0.5
 Summary: Omnivore Terminal App - Text User Interface
 Home-page: https://github.com/yazdipour/OmnivoreX
 Author: Shahriar Yazdipour
 Author-email: git@yazdipour.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/yazdipour/OmnivoreX/issues
 Project-URL: Source Code, https://github.com/yazdipour/OmnivoreX
@@ -31,18 +31,18 @@
 
 ```bash
 pip install omnivorex
 ```
 
 ## Usage
 
-1. Get your Omnivore API Key from [here](https://dashboard.omnivore.io/developers).
+1. Get your Omnivore API Key from [here](https://omnivore.app/settings/api).
 
 2. Run the command:
 
 ```bash
 omnivorex
 ```
 
 ## Screenshots
 
-![OmnivoreX](/docs/screenshots/omnivorex.png)
+![OmnivoreX](https://raw.githubusercontent.com/yazdipour/OmnivoreX/main/docs/screenshots/omnivorex.png)
```

### Comparing `omnivorex-0.0.4/README.md` & `omnivorex-0.0.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 
 ```bash
 pip install omnivorex
 ```
 
 ## Usage
 
-1. Get your Omnivore API Key from [here](https://dashboard.omnivore.io/developers).
+1. Get your Omnivore API Key from [here](https://omnivore.app/settings/api).
 
 2. Run the command:
 
 ```bash
 omnivorex
 ```
 
 ## Screenshots
 
-![OmnivoreX](/docs/screenshots/omnivorex.png)
+![OmnivoreX](https://raw.githubusercontent.com/yazdipour/OmnivoreX/main/docs/screenshots/omnivorex.png)
```

### Comparing `omnivorex-0.0.4/docs/Publish.md` & `omnivorex-0.0.5/docs/Publish.md`

 * *Files identical despite different names*

### Comparing `omnivorex-0.0.4/docs/screenshots/omnivorex.png` & `omnivorex-0.0.5/docs/screenshots/omnivorex.png`

 * *Files identical despite different names*

### Comparing `omnivorex-0.0.4/docs/textual.md` & `omnivorex-0.0.5/docs/textual.md`

 * *Files identical despite different names*

### Comparing `omnivorex-0.0.4/omnivorex.egg-info/PKG-INFO` & `omnivorex-0.0.5/omnivorex.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnivorex
-Version: 0.0.4
+Version: 0.0.5
 Summary: Omnivore Terminal App - Text User Interface
 Home-page: https://github.com/yazdipour/OmnivoreX
 Author: Shahriar Yazdipour
 Author-email: git@yazdipour.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/yazdipour/OmnivoreX/issues
 Project-URL: Source Code, https://github.com/yazdipour/OmnivoreX
@@ -31,18 +31,18 @@
 
 ```bash
 pip install omnivorex
 ```
 
 ## Usage
 
-1. Get your Omnivore API Key from [here](https://dashboard.omnivore.io/developers).
+1. Get your Omnivore API Key from [here](https://omnivore.app/settings/api).
 
 2. Run the command:
 
 ```bash
 omnivorex
 ```
 
 ## Screenshots
 
-![OmnivoreX](/docs/screenshots/omnivorex.png)
+![OmnivoreX](https://raw.githubusercontent.com/yazdipour/OmnivoreX/main/docs/screenshots/omnivorex.png)
```

### Comparing `omnivorex-0.0.4/setup.py` & `omnivorex-0.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 setup(
     name="omnivorex",
     version=VERSION,
     description="Omnivore Terminal App - Text User Interface",
     author="Shahriar Yazdipour",
     author_email="git@yazdipour.com",
-    packages=["src.omnivorex"],
+    packages=["omnivorex"],
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     license="MIT",
     keywords="omnivore cli terminal readlater client tui rich textualize textual",
     url=PROJECT_URLS["Source Code"],
     project_urls=PROJECT_URLS,
     python_requires=">=3",
@@ -48,11 +48,11 @@
     install_requires=[
         "python-dotenv",
         "omnivoreql>=0.2.1",
         "textual==0.29.0",
     ],
     entry_points={
         "console_scripts": [
-            "omnivorex=src.omnivorex.__main__:main",
+            "omnivorex=omnivorex.omnivorex:main",
         ],
     },
 )
```

### Comparing `omnivorex-0.0.4/src/omnivorex/main_screen.py` & `omnivorex-0.0.5/omnivorex/omnivorex.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,16 @@
-from textual.app import App, ComposeResult
+from textual.app import App
 from textual.widgets import (
-    Input,
     Footer,
     Header,
     Button,
-    Static,
     MarkdownViewer,
-    Markdown,
     ListView,
-    ListItem,
-    Label,
 )
-from textual.containers import Container, Horizontal, ScrollableContainer, Grid
-from textual.reactive import reactive
-from textual.screen import ModalScreen
-from textual import on
+from textual.containers import Container
 import os
 from .components.login_screen import LoginScreen
 from .components.article_item import ArticleItem
 from .utils import _omnivoerql_utils
 
 
 class OmnivoreX(App):
@@ -143,9 +135,13 @@
         lv = self.query_one("#list_view", ListView)
         cursor = 0 if len(lv.children) == 0 else lv.children[-1].details["cursor"]
         self.populate_listview(
             _omnivoerql_utils.get_articles(cursor, self.DEFAULT_LIMIT)
         )
 
 
-if __name__ == "__main__":
+def main():
     OmnivoreX().run()
+
+
+if __name__ == "__main__":
+    main()
```

