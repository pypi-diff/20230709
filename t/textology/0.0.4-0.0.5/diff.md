# Comparing `tmp/textology-0.0.4.tar.gz` & `tmp/textology-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textology-0.0.4.tar", last modified: Tue Jul  4 21:45:51 2023, max compression
+gzip compressed data, was "textology-0.0.5.tar", last modified: Sun Jul  9 16:28:27 2023, max compression
```

## Comparing `textology-0.0.4.tar` & `textology-0.0.5.tar`

### file list

```diff
@@ -1,41 +1,45 @@
-drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-04 21:45:51.656418 textology-0.0.4/
--rw-r--r--   0 dfritz     (502) staff       (20)     1068 2023-07-01 18:44:36.000000 textology-0.0.4/LICENSE
--rw-r--r--   0 dfritz     (502) staff       (20)     9953 2023-07-04 21:45:51.656629 textology-0.0.4/PKG-INFO
--rw-r--r--   0 dfritz     (502) staff       (20)     8600 2023-07-04 21:28:27.000000 textology-0.0.4/README.md
--rw-r--r--   0 dfritz     (502) staff       (20)      163 2023-07-04 21:19:10.000000 textology-0.0.4/requirements-dev.txt
--rw-r--r--   0 dfritz     (502) staff       (20)       16 2023-07-04 21:18:52.000000 textology-0.0.4/requirements.txt
--rw-r--r--   0 dfritz     (502) staff       (20)     1672 2023-07-04 21:45:51.658564 textology-0.0.4/setup.cfg
--rw-r--r--   0 dfritz     (502) staff       (20)     3199 2023-07-04 21:20:02.000000 textology-0.0.4/setup.py
-drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-04 21:45:51.643479 textology-0.0.4/textology/
--rw-r--r--   0 dfritz     (502) staff       (20)       69 2023-07-04 21:44:36.000000 textology-0.0.4/textology/__init__.py
--rw-r--r--   0 dfritz     (502) staff       (20)     8044 2023-07-04 21:18:52.000000 textology-0.0.4/textology/apps.py
--rw-r--r--   0 dfritz     (502) staff       (20)     2772 2023-07-04 21:19:10.000000 textology-0.0.4/textology/history.py
--rw-r--r--   0 dfritz     (502) staff       (20)      492 2023-07-04 21:19:10.000000 textology-0.0.4/textology/logging.py
-drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-04 21:45:51.648705 textology-0.0.4/textology/observers/
--rw-r--r--   0 dfritz     (502) staff       (20)      711 2023-07-04 19:31:50.000000 textology-0.0.4/textology/observers/__init__.py
--rw-r--r--   0 dfritz     (502) staff       (20)     2944 2023-07-04 19:31:50.000000 textology-0.0.4/textology/observers/_dependencies.py
--rw-r--r--   0 dfritz     (502) staff       (20)      458 2023-07-04 19:31:50.000000 textology-0.0.4/textology/observers/_exceptions.py
--rw-r--r--   0 dfritz     (502) staff       (20)    17952 2023-07-04 21:19:10.000000 textology-0.0.4/textology/observers/_managers.py
--rw-r--r--   0 dfritz     (502) staff       (20)    15840 2023-07-04 21:18:52.000000 textology-0.0.4/textology/pytest_utils.py
--rw-r--r--   0 dfritz     (502) staff       (20)    17750 2023-07-04 21:19:10.000000 textology-0.0.4/textology/router.py
--rw-r--r--   0 dfritz     (502) staff       (20)    29247 2023-07-04 21:18:52.000000 textology-0.0.4/textology/test-template.html
-drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-04 21:45:51.655840 textology-0.0.4/textology/widgets/
--rw-r--r--   0 dfritz     (502) staff       (20)     1123 2023-07-04 21:18:52.000000 textology-0.0.4/textology/widgets/__init__.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1712 2023-07-04 21:18:52.000000 textology-0.0.4/textology/widgets/_button.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1248 2023-07-04 21:18:52.000000 textology-0.0.4/textology/widgets/_containers.py
--rw-r--r--   0 dfritz     (502) staff       (20)     9394 2023-07-04 21:18:52.000000 textology-0.0.4/textology/widgets/_extensions.py
--rw-r--r--   0 dfritz     (502) staff       (20)     7285 2023-07-04 21:18:52.000000 textology-0.0.4/textology/widgets/_horizontal_menus.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1665 2023-07-04 21:18:52.000000 textology-0.0.4/textology/widgets/_label.py
--rw-r--r--   0 dfritz     (502) staff       (20)     2058 2023-07-04 21:18:52.000000 textology-0.0.4/textology/widgets/_list_item.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1763 2023-07-04 21:18:52.000000 textology-0.0.4/textology/widgets/_list_item_header.py
--rw-r--r--   0 dfritz     (502) staff       (20)     4919 2023-07-04 21:18:52.000000 textology-0.0.4/textology/widgets/_list_view.py
--rw-r--r--   0 dfritz     (502) staff       (20)     8716 2023-07-04 21:18:52.000000 textology-0.0.4/textology/widgets/_location.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1955 2023-07-04 21:18:52.000000 textology-0.0.4/textology/widgets/_modal_dialog.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1765 2023-07-04 21:18:52.000000 textology-0.0.4/textology/widgets/_static.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1962 2023-07-04 21:18:52.000000 textology-0.0.4/textology/widgets/_store.py
-drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-04 21:45:51.646752 textology-0.0.4/textology.egg-info/
--rw-r--r--   0 dfritz     (502) staff       (20)     9953 2023-07-04 21:45:51.000000 textology-0.0.4/textology.egg-info/PKG-INFO
--rw-r--r--   0 dfritz     (502) staff       (20)      950 2023-07-04 21:45:51.000000 textology-0.0.4/textology.egg-info/SOURCES.txt
--rw-r--r--   0 dfritz     (502) staff       (20)        1 2023-07-04 21:45:51.000000 textology-0.0.4/textology.egg-info/dependency_links.txt
--rw-r--r--   0 dfritz     (502) staff       (20)      186 2023-07-04 21:45:51.000000 textology-0.0.4/textology.egg-info/requires.txt
--rw-r--r--   0 dfritz     (502) staff       (20)       10 2023-07-04 21:45:51.000000 textology-0.0.4/textology.egg-info/top_level.txt
+drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-09 16:28:27.314627 textology-0.0.5/
+-rw-r--r--   0 dfritz     (502) staff       (20)     1068 2023-07-01 18:44:36.000000 textology-0.0.5/LICENSE
+-rw-r--r--   0 dfritz     (502) staff       (20)       97 2023-07-08 19:46:35.000000 textology-0.0.5/MANIFEST.in
+-rw-r--r--   0 dfritz     (502) staff       (20)    12230 2023-07-09 16:28:27.314966 textology-0.0.5/PKG-INFO
+-rw-r--r--   0 dfritz     (502) staff       (20)    10868 2023-07-09 16:23:23.000000 textology-0.0.5/README.md
+-rw-r--r--   0 dfritz     (502) staff       (20)       22 2023-07-08 19:46:35.000000 textology-0.0.5/requirements-dev.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)      168 2023-07-08 19:46:35.000000 textology-0.0.5/requirements-full-dev.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)       16 2023-07-04 21:18:52.000000 textology-0.0.5/requirements.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)     1672 2023-07-09 16:28:27.316897 textology-0.0.5/setup.cfg
+-rw-r--r--   0 dfritz     (502) staff       (20)     3225 2023-07-08 19:46:35.000000 textology-0.0.5/setup.py
+drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-09 16:28:27.300225 textology-0.0.5/textology/
+-rw-r--r--   0 dfritz     (502) staff       (20)       69 2023-07-09 16:23:23.000000 textology-0.0.5/textology/__init__.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     9798 2023-07-09 16:23:23.000000 textology-0.0.5/textology/apps.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2362 2023-07-08 19:46:35.000000 textology-0.0.5/textology/dash_compat.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2772 2023-07-04 21:19:10.000000 textology-0.0.5/textology/history.py
+-rw-r--r--   0 dfritz     (502) staff       (20)      492 2023-07-04 21:19:10.000000 textology-0.0.5/textology/logging.py
+drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-09 16:28:27.305437 textology-0.0.5/textology/observers/
+-rw-r--r--   0 dfritz     (502) staff       (20)      711 2023-07-04 19:31:50.000000 textology-0.0.5/textology/observers/__init__.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2944 2023-07-04 19:31:50.000000 textology-0.0.5/textology/observers/_dependencies.py
+-rw-r--r--   0 dfritz     (502) staff       (20)      458 2023-07-04 19:31:50.000000 textology-0.0.5/textology/observers/_exceptions.py
+-rw-r--r--   0 dfritz     (502) staff       (20)    18649 2023-07-09 16:23:23.000000 textology-0.0.5/textology/observers/_managers.py
+-rw-r--r--   0 dfritz     (502) staff       (20)    16596 2023-07-08 19:46:35.000000 textology-0.0.5/textology/pytest_utils.py
+-rw-r--r--   0 dfritz     (502) staff       (20)    17750 2023-07-09 14:50:38.000000 textology-0.0.5/textology/router.py
+-rw-r--r--   0 dfritz     (502) staff       (20)    29250 2023-07-08 19:46:35.000000 textology-0.0.5/textology/test-template.html
+drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-09 16:28:27.313853 textology-0.0.5/textology/widgets/
+-rw-r--r--   0 dfritz     (502) staff       (20)     1165 2023-07-08 19:46:35.000000 textology-0.0.5/textology/widgets/__init__.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1712 2023-07-04 21:18:52.000000 textology-0.0.5/textology/widgets/_button.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1248 2023-07-04 21:18:52.000000 textology-0.0.5/textology/widgets/_containers.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     9394 2023-07-04 21:18:52.000000 textology-0.0.5/textology/widgets/_extensions.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     9554 2023-07-09 16:23:23.000000 textology-0.0.5/textology/widgets/_horizontal_menus.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1665 2023-07-04 21:18:52.000000 textology-0.0.5/textology/widgets/_label.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2047 2023-07-08 19:46:35.000000 textology-0.0.5/textology/widgets/_list_item.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1992 2023-07-08 19:46:35.000000 textology-0.0.5/textology/widgets/_list_item_header.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1981 2023-07-08 19:46:35.000000 textology-0.0.5/textology/widgets/_list_item_meta.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     4919 2023-07-04 21:18:52.000000 textology-0.0.5/textology/widgets/_list_view.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     8683 2023-07-09 16:23:23.000000 textology-0.0.5/textology/widgets/_location.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1955 2023-07-04 21:18:52.000000 textology-0.0.5/textology/widgets/_modal_dialog.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1765 2023-07-04 21:18:52.000000 textology-0.0.5/textology/widgets/_static.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1962 2023-07-04 21:18:52.000000 textology-0.0.5/textology/widgets/_store.py
+drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-09 16:28:27.303153 textology-0.0.5/textology.egg-info/
+-rw-r--r--   0 dfritz     (502) staff       (20)    12230 2023-07-09 16:28:27.000000 textology-0.0.5/textology.egg-info/PKG-INFO
+-rw-r--r--   0 dfritz     (502) staff       (20)     1050 2023-07-09 16:28:27.000000 textology-0.0.5/textology.egg-info/SOURCES.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)        1 2023-07-09 16:28:27.000000 textology-0.0.5/textology.egg-info/dependency_links.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)      279 2023-07-09 16:28:27.000000 textology-0.0.5/textology.egg-info/requires.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)       10 2023-07-09 16:28:27.000000 textology-0.0.5/textology.egg-info/top_level.txt
```

### Comparing `textology-0.0.4/LICENSE` & `textology-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `textology-0.0.4/PKG-INFO` & `textology-0.0.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: textology
-Version: 0.0.4
-Summary: Extensions for creating Terminal User Interfaces
+Version: 0.0.5
+Summary: Textual extensions for creating Terminal User Interfaces
 Home-page: https://github.com/dfrtz/textology
 Author: David Fritz
-Maintainer: David Fritz
 License: MIT
 Project-URL: Issue Tracker, https://github.com/dfrtz/textology/issues
 Project-URL: Source Code, https://github.com/dfrtz/textology
 Platform: MacOS
 Platform: Linux
 Platform: Windows
 Classifier: Development Status :: 4 - Beta
@@ -27,18 +26,20 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: full-dev
 License-File: LICENSE
 
+
 <div align="center">
-  <img src="https://github.com/dfrtz/textology/blob/main/docs/banner.svg" width="450">
+  <img src="https://raw.githubusercontent.com/dfrtz/textology/main/docs/banner.svg" width="450">
 </div>
 
 -----------------
 
 
 [![os: windows mac linux](https://img.shields.io/badge/os-linux_|_macos_|_windows-blue)](https://docs.python.org/3.10/)
 [![python: 3.10+](https://img.shields.io/badge/python-3.10_|_3.11-blue)](https://docs.python.org/3.10/)
@@ -66,18 +67,19 @@
 as possible to a traditional GUI experience straight from a terminal. Why? Not all environments allow full graphical
 library access, web access, etc. Specifically, Textology is inspired by the designs of frameworks such as
 Dash/FastAPI/Flask and their use of routing, context managers, and observation patterns. Textology also receives
 inspiration from other UI frameworks external to Python, such as iOS, Android, and Web frameworks. Most importantly
 however, Textology is an extension of Textual: it does not replace Textual, but rather provides additional options
 on top of the core framework.
 
-Before using Textology, be comfortable with Textual. Textology is NOT a replacement for Textual, it is an
+Before using Textology, be comfortable with Textual. For tutorials, guides, etc., refer to the
+[Textual Documentation](https://textual.textualize.io/guide/). Textology is NOT a replacement for Textual, it is an
 extension. Callbacks, widgets, screens, event lifecycles, etc., from Textual still apply to Textology extended
 widgets and applications. For other advanced features, familiarity with Dash/FastAPI/Flask principles will help.
-Examples are included for advanced features, such as callback based applications.
+Examples for Textology extensions, such as callback based applications, are included in this documentation.
 
 
 ## Table Of Contents
 
   * [Compatibility](#compatibility)
   * [Key Features](#top-features)
   * [Getting Started](#getting-started)
@@ -97,59 +99,66 @@
 
 - Extended basic widgets, such as:
   - Buttons with ability to declare callbacks inline, and track click counts
   - ListItems with metadata objects and ability to disable event messages
 - New widgets, such as:
   - ListItemHeaders (non-interactive ListItems)
   - HorizontalMenus (walkable list of ListViews with peeking at following lists)
-- "Observer" application, with "event driven architecture" to detect changes and automatically update elements in UI.
+- "Observer" apps, with "event driven architecture" to detect changes and automatically update UI elements.
 - Enhanced testing support
   - Parallel tests via python-xdist
   - Custom testing arguments, such as updating snapshots on failures
 
 
 ## Getting Started
 
 ### Installation
 
 Install Textology via pip:
 ```shell
 pip install textology
 ```
 
-For dev requirements, use the additional `[dev]` package, which installs Textual development tools and extra QA tools:
+For development of applications based on Textual/Textology (but not development of Textology itself), use the
+`[dev]` package. This installs extra Textual development tools, and requirements for Textology testing extensions.
 ```shell
 pip install textology[dev]
 ```
 
+For full development of Textology itself, use the `[full-dev]` package. This installs Textual development tools,
+requirements for Textology testing extensions, and full QA requirements to meet commit standards. This version
+has the highest library requirements, in order to match the versions used by Textology itself for testing. Required if
+developing Textology itself, or recommended if looking to match/exceed the level of QA testing used by Textology.
+```shell
+pip install textology[full-dev]
+```
+
 ### Extended Applications
 
 Some Textology app classes, such as `ObservedApp`, can replace any regular Textual App, and be used as is without any
 extensions turned on. Here is an example of the most commonly used extended application, `ObservedApp`, and its
 primary extended functionality being used. More detailed examples of applications based around routes, callbacks,
 and standard Textual applications can be found in [Examples](https://github.com/dfrtz/textology/examples).
 
 - Observer/callback application (automatic attribute monitoring and updates by element IDs without manual queries):
 ```python
 from textology.apps import ObservedApp
 from textology.observers import Modified, Select, Update
 from textology.widgets import Button, Container, Label
 
-class SimpleApp(ObservedApp):
-    def compose(self):
-        yield Container(
-            Button('Ping', id='ping-btn'),
-            Button('Pong', id='pong-btn'),
-            Button('Sing-a-long', id='sing-btn'),
-            Container(
-                id="content",
-            ),
-        )
-
-app = SimpleApp()
+app = ObservedApp(
+    layout=Container(
+        Button('Ping', id='ping-btn'),
+        Button('Pong', id='pong-btn'),
+        Button('Sing-a-long', id='sing-btn'),
+        Container(
+            id="content",
+        ),
+    )
+)
 
 @app.when(
     Modified("ping-btn", "n_clicks"),
     Update("content", "children"),
 )
 def ping(clicks):
     return Label(f"Ping pressed {clicks}")
@@ -171,25 +180,84 @@
     if not ping_clicks or not pong_clicks:
         return Label(f"Press Ping and Pong first to complete the song!")
     return Label(f"Ping, pong, sing-a-long song pressed {song_clicks}")
 
 app.run()
 ```
 
+- Observation callbacks can also be async:
+```python
+@app.when(
+    Modified("pong-btn", "n_clicks"),
+    Update("content", "children"),
+)
+async def delayed_pong(clicks):
+    await asyncio.sleep(3)
+    return Label(f"Pong pressed {clicks} and updated 3 seconds later")
+```
+
+- <details>
+  <summary>Observer/callback application (Same as above, but with Dash compatibility object and calls)</summary>
+
+    ```python
+    from textology.dash_compat import DashCompatApp, Input, Output, State
+    from textology.widgets import Button, Container, Label
+
+    app = DashCompatApp(
+        layout=Container(
+            Button('Ping', id='ping-btn'),
+            Button('Pong', id='pong-btn'),
+            Button('Sing-a-long', id='sing-btn'),
+            Container(
+                id="content",
+            ),
+        )
+    )
+
+    @app.callback(
+        Input("ping-btn", "n_clicks"),
+        Output("content", "children"),
+    )
+    def ping(clicks):
+        return Label(f"Ping pressed {clicks}")
+
+    @app.callback(
+        Input("pong-btn", "n_clicks"),
+        Output("content", "children"),
+    )
+    def pong(clicks):
+        return Label(f"Pong pressed {clicks}")
+
+    @app.callback(
+        Input("sing-btn", "n_clicks"),
+        State("ping-btn", "n_clicks"),
+        State("pong-btn", "n_clicks"),
+        Output("content", "children"),
+    )
+    def song(song_clicks, ping_clicks, pong_clicks):
+        if not ping_clicks or not pong_clicks:
+            return Label(f"Press Ping and Pong first to complete the song!")
+        return Label(f"Ping, pong, sing-a-long song pressed {song_clicks}")
+
+    app.run()
+    ```
+
+ </details>
+
 ### Extended Widgets
 
 Native Textual widgets can be directly swapped out with Textology extended equivalents. They can then be used as is
 (standard Textual usage), or with extensions (via extra keyword arguments).
 
 - Basic swap (no extensions):
 ```python
 # Replace:
 from textual.widgets import Button
 
-# With
+# With:
 from textology.widgets import Button
 ```
 
 - Instance callback extension (avoid global watchers, name/ID checks in the event watchers, and event chaining):
 ```python
 from textology.widgets import Button
 
@@ -238,19 +306,20 @@
 
 - Basic snapshot test:
 ```python
 import pytest
 from textual import App
 from textual.widgets import Button
 
+class BasicApp(App):
+    def compose(self):
+        yield Button("Click me!")
+
 @pytest.mark.asyncio
-async def test_snapshot_with_app(compare_snapshots) -> None:
-    class BasicApp(App):
-        def compose(self):
-            yield Button("Click me!", id="btn")
+async def test_snapshot_with_app(compare_snapshots):
     assert await compare_snapshots(BasicApp())
 ```
 
 Other advanced testing features include:
 - Ability to pass and App, App Pilot, or a module containing an instantiated App or Pilot, to fixtures
 - Custom snapshot paths, including reusing the same snapshot across multiple tests
 - Automatic SVG updates with `pytest --txtology-snap-update`
```

### Comparing `textology-0.0.4/README.md` & `textology-0.0.5/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+
 <div align="center">
-  <img src="https://github.com/dfrtz/textology/blob/main/docs/banner.svg" width="450">
+  <img src="https://raw.githubusercontent.com/dfrtz/textology/main/docs/banner.svg" width="450">
 </div>
 
 -----------------
 
 
 [![os: windows mac linux](https://img.shields.io/badge/os-linux_|_macos_|_windows-blue)](https://docs.python.org/3.10/)
 [![python: 3.10+](https://img.shields.io/badge/python-3.10_|_3.11-blue)](https://docs.python.org/3.10/)
@@ -31,18 +32,19 @@
 as possible to a traditional GUI experience straight from a terminal. Why? Not all environments allow full graphical
 library access, web access, etc. Specifically, Textology is inspired by the designs of frameworks such as
 Dash/FastAPI/Flask and their use of routing, context managers, and observation patterns. Textology also receives
 inspiration from other UI frameworks external to Python, such as iOS, Android, and Web frameworks. Most importantly
 however, Textology is an extension of Textual: it does not replace Textual, but rather provides additional options
 on top of the core framework.
 
-Before using Textology, be comfortable with Textual. Textology is NOT a replacement for Textual, it is an
+Before using Textology, be comfortable with Textual. For tutorials, guides, etc., refer to the
+[Textual Documentation](https://textual.textualize.io/guide/). Textology is NOT a replacement for Textual, it is an
 extension. Callbacks, widgets, screens, event lifecycles, etc., from Textual still apply to Textology extended
 widgets and applications. For other advanced features, familiarity with Dash/FastAPI/Flask principles will help.
-Examples are included for advanced features, such as callback based applications.
+Examples for Textology extensions, such as callback based applications, are included in this documentation.
 
 
 ## Table Of Contents
 
   * [Compatibility](#compatibility)
   * [Key Features](#top-features)
   * [Getting Started](#getting-started)
@@ -62,59 +64,66 @@
 
 - Extended basic widgets, such as:
   - Buttons with ability to declare callbacks inline, and track click counts
   - ListItems with metadata objects and ability to disable event messages
 - New widgets, such as:
   - ListItemHeaders (non-interactive ListItems)
   - HorizontalMenus (walkable list of ListViews with peeking at following lists)
-- "Observer" application, with "event driven architecture" to detect changes and automatically update elements in UI.
+- "Observer" apps, with "event driven architecture" to detect changes and automatically update UI elements.
 - Enhanced testing support
   - Parallel tests via python-xdist
   - Custom testing arguments, such as updating snapshots on failures
 
 
 ## Getting Started
 
 ### Installation
 
 Install Textology via pip:
 ```shell
 pip install textology
 ```
 
-For dev requirements, use the additional `[dev]` package, which installs Textual development tools and extra QA tools:
+For development of applications based on Textual/Textology (but not development of Textology itself), use the
+`[dev]` package. This installs extra Textual development tools, and requirements for Textology testing extensions.
 ```shell
 pip install textology[dev]
 ```
 
+For full development of Textology itself, use the `[full-dev]` package. This installs Textual development tools,
+requirements for Textology testing extensions, and full QA requirements to meet commit standards. This version
+has the highest library requirements, in order to match the versions used by Textology itself for testing. Required if
+developing Textology itself, or recommended if looking to match/exceed the level of QA testing used by Textology.
+```shell
+pip install textology[full-dev]
+```
+
 ### Extended Applications
 
 Some Textology app classes, such as `ObservedApp`, can replace any regular Textual App, and be used as is without any
 extensions turned on. Here is an example of the most commonly used extended application, `ObservedApp`, and its
 primary extended functionality being used. More detailed examples of applications based around routes, callbacks,
 and standard Textual applications can be found in [Examples](https://github.com/dfrtz/textology/examples).
 
 - Observer/callback application (automatic attribute monitoring and updates by element IDs without manual queries):
 ```python
 from textology.apps import ObservedApp
 from textology.observers import Modified, Select, Update
 from textology.widgets import Button, Container, Label
 
-class SimpleApp(ObservedApp):
-    def compose(self):
-        yield Container(
-            Button('Ping', id='ping-btn'),
-            Button('Pong', id='pong-btn'),
-            Button('Sing-a-long', id='sing-btn'),
-            Container(
-                id="content",
-            ),
-        )
-
-app = SimpleApp()
+app = ObservedApp(
+    layout=Container(
+        Button('Ping', id='ping-btn'),
+        Button('Pong', id='pong-btn'),
+        Button('Sing-a-long', id='sing-btn'),
+        Container(
+            id="content",
+        ),
+    )
+)
 
 @app.when(
     Modified("ping-btn", "n_clicks"),
     Update("content", "children"),
 )
 def ping(clicks):
     return Label(f"Ping pressed {clicks}")
@@ -136,25 +145,84 @@
     if not ping_clicks or not pong_clicks:
         return Label(f"Press Ping and Pong first to complete the song!")
     return Label(f"Ping, pong, sing-a-long song pressed {song_clicks}")
 
 app.run()
 ```
 
+- Observation callbacks can also be async:
+```python
+@app.when(
+    Modified("pong-btn", "n_clicks"),
+    Update("content", "children"),
+)
+async def delayed_pong(clicks):
+    await asyncio.sleep(3)
+    return Label(f"Pong pressed {clicks} and updated 3 seconds later")
+```
+
+- <details>
+  <summary>Observer/callback application (Same as above, but with Dash compatibility object and calls)</summary>
+
+    ```python
+    from textology.dash_compat import DashCompatApp, Input, Output, State
+    from textology.widgets import Button, Container, Label
+
+    app = DashCompatApp(
+        layout=Container(
+            Button('Ping', id='ping-btn'),
+            Button('Pong', id='pong-btn'),
+            Button('Sing-a-long', id='sing-btn'),
+            Container(
+                id="content",
+            ),
+        )
+    )
+
+    @app.callback(
+        Input("ping-btn", "n_clicks"),
+        Output("content", "children"),
+    )
+    def ping(clicks):
+        return Label(f"Ping pressed {clicks}")
+
+    @app.callback(
+        Input("pong-btn", "n_clicks"),
+        Output("content", "children"),
+    )
+    def pong(clicks):
+        return Label(f"Pong pressed {clicks}")
+
+    @app.callback(
+        Input("sing-btn", "n_clicks"),
+        State("ping-btn", "n_clicks"),
+        State("pong-btn", "n_clicks"),
+        Output("content", "children"),
+    )
+    def song(song_clicks, ping_clicks, pong_clicks):
+        if not ping_clicks or not pong_clicks:
+            return Label(f"Press Ping and Pong first to complete the song!")
+        return Label(f"Ping, pong, sing-a-long song pressed {song_clicks}")
+
+    app.run()
+    ```
+
+ </details>
+
 ### Extended Widgets
 
 Native Textual widgets can be directly swapped out with Textology extended equivalents. They can then be used as is
 (standard Textual usage), or with extensions (via extra keyword arguments).
 
 - Basic swap (no extensions):
 ```python
 # Replace:
 from textual.widgets import Button
 
-# With
+# With:
 from textology.widgets import Button
 ```
 
 - Instance callback extension (avoid global watchers, name/ID checks in the event watchers, and event chaining):
 ```python
 from textology.widgets import Button
 
@@ -203,19 +271,20 @@
 
 - Basic snapshot test:
 ```python
 import pytest
 from textual import App
 from textual.widgets import Button
 
+class BasicApp(App):
+    def compose(self):
+        yield Button("Click me!")
+
 @pytest.mark.asyncio
-async def test_snapshot_with_app(compare_snapshots) -> None:
-    class BasicApp(App):
-        def compose(self):
-            yield Button("Click me!", id="btn")
+async def test_snapshot_with_app(compare_snapshots):
     assert await compare_snapshots(BasicApp())
 ```
 
 Other advanced testing features include:
 - Ability to pass and App, App Pilot, or a module containing an instantiated App or Pilot, to fixtures
 - Custom snapshot paths, including reusing the same snapshot across multiple tests
 - Automatic SVG updates with `pytest --txtology-snap-update`
```

### Comparing `textology-0.0.4/setup.cfg` & `textology-0.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `textology-0.0.4/setup.py` & `textology-0.0.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,19 +28,18 @@
     with open(f"requirements{extra_type}.txt", encoding="utf-8") as input_file:
         lines = (line.strip() for line in input_file)
         return [req for req in lines if req and not req.startswith("#")]
 
 
 setup(
     name="textology",
-    description="Extensions for creating Terminal User Interfaces",
+    description="Textual extensions for creating Terminal User Interfaces",
     long_description=Path("README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     version=_find_version("textology"),
-    maintainer="David Fritz",
     author="David Fritz",
     url="https://github.com/dfrtz/textology",
     project_urls={
         "Issue Tracker": "https://github.com/dfrtz/textology/issues",
         "Source Code": "https://github.com/dfrtz/textology",
     },
     license="MIT",
@@ -66,23 +65,22 @@
     platforms=[
         "MacOS",
         "Linux",
         "Windows",
     ],
     test_suite="pytest",
     packages=find_packages(ROOT_DIR, include=["textology*"], exclude=["*test", "tests*"]),
-    package_data={"textology": ["test-template.html"]},
-    data_files=[
-        (
-            "",
-            [
-                "requirements.txt",
-                "requirements-dev.txt",
-            ],
-        )
-    ],
+    include_package_data=True,
     python_requires=">=3.10",
     install_requires=read_requirements_file(None),
     extras_require={
-        "dev": read_requirements_file("dev"),
+        "dev": [
+            *read_requirements_file(None),
+            *read_requirements_file("dev"),
+        ],
+        "full-dev": [
+            *read_requirements_file(None),
+            *read_requirements_file("dev"),
+            *read_requirements_file("full-dev"),
+        ],
     },
 )
```

### Comparing `textology-0.0.4/textology/apps.py` & `textology-0.0.5/textology/apps.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,33 +11,76 @@
 from textual.app import ComposeResult
 from textual.app import CSSPathType
 from textual.containers import Container
 from textual.css.query import NoMatches
 from textual.driver import Driver
 from textual.widget import Widget
 
-from .logging import NullLogger
 from .observers import ObserverManager
 from .widgets import Location
 
 
-class BrowserApp(App):
+class WidgetApp(App):
+    """Application with a single widget for the root layout."""
+
+    def __init__(
+        self,
+        layout: Callable | Widget | None = None,
+        driver_class: type[Driver] | None = None,
+        css_path: CSSPathType | None = None,
+        watch_css: bool = False,
+    ) -> None:
+        """Initialize an application with a layout.
+
+        Args:
+            layout: Primary content widget, or function to create primary content widget.
+            driver_class: Driver class or `None` to auto-detect.
+                This will be used by some Textual tools.
+            css_path: Path to CSS or `None` to use the `CSS_PATH` class variable.
+                To load multiple CSS files, pass a list of strings or paths which will be loaded in order.
+            watch_css: Reload CSS if the files changed.
+                This is set automatically if you are using `textual run` with the `dev` switch.
+
+        Raises:
+            CssPathError: When the supplied CSS path(s) are an unexpected type.
+        """
+        super().__init__(
+            driver_class=driver_class,
+            css_path=css_path,
+            watch_css=watch_css,
+        )
+        self.layout = layout or self.default_layout
+
+    def compose(self) -> ComposeResult:
+        """Default compose with provided layout.
+
+        Yields:
+            Layout widget set on instantiation.
+        """
+        yield self.layout if not isinstance(self.layout, Callable) else self.layout()
+
+    def default_layout(self) -> Widget:
+        """Default layout generator if a layout was not provided during initialization."""
+        return Container(id="content-window")
+
+
+class BrowserApp(WidgetApp):
     """Application capable of routing user requests, and tracking browsing history."""
 
     def __init__(
         self,
-        layout: Widget | None = None,
+        layout: Callable | Widget | None = None,
         driver_class: type[Driver] | None = None,
         css_path: CSSPathType | None = None,
         watch_css: bool = False,
     ) -> None:
         """Initialize an application with a browser history and router.
 
         Args:
-            layout: Primary content window.
+            layout: Primary content widget, or function to create primary content widget.
                 Must contain Location widget.
             driver_class: Driver class or `None` to auto-detect.
                 This will be used by some Textual tools.
             css_path: Path to CSS or `None` to use the `CSS_PATH` class variable.
                 To load multiple CSS files, pass a list of strings or paths which will be loaded in order.
             watch_css: Reload CSS if the files changed.
                 This is set automatically if you are using `textual run` with the `dev` switch.
@@ -46,40 +89,35 @@
             CssPathError: When the supplied CSS path(s) are an unexpected type.
         """
         if layout is None:
             layout = Container(
                 Location(),
                 Container(id="content-window"),
             )
+        elif isinstance(layout, Callable):
+            layout = layout()
+
         if isinstance(layout, Location):
             location = layout
         else:
             location = None
             for node in layout.walk_children():
                 if isinstance(node, Location):
                     location = node
                     break
         if not location:
             raise ValueError("Layout must contain a Location object for routing requests")
         super().__init__(
+            layout=layout,
             driver_class=driver_class,
             css_path=css_path,
             watch_css=watch_css,
         )
-        self.layout = layout
         self.location = location
 
-    def compose(self) -> ComposeResult:
-        """Default compose with provided layout.
-
-        Yields:
-            Layout Widget set on instantiation.
-        """
-        yield self.layout
-
     def back(self) -> int:
         """Go back one URL in the browser history.
 
         Returns:
             The new index in the history.
         """
         return self.location.back()
@@ -118,45 +156,48 @@
 
         Returns:
             A decorator that will register a function as capable of accepting requests to a specific path/method combo.
         """
         return self.location.route(path, methods=methods)
 
 
-class ObservedApp(App, ObserverManager):
+class ObservedApp(WidgetApp, ObserverManager):
     """Application capable of performing automatic input/output callbacks on reactive widget property updates."""
 
     def __init__(
         self,
+        layout: Callable | Widget | None = None,
         driver_class: type[Driver] | None = None,
         css_path: CSSPathType | None = None,
         watch_css: bool = False,
         logger: logging.Logger | None = None,
     ) -> None:
         """Initialize an application with tracking for input/output callbacks.
 
         Args:
+            layout: Primary content widget, or function to create primary content widget.
             driver_class: Driver class or `None` to auto-detect.
                 This will be used by some Textual tools.
             css_path: Path to CSS or `None` to use the `CSS_PATH` class variable.
                 To load multiple CSS files, pass a list of strings or paths which will be loaded in order.
             watch_css: Reload CSS if the files changed.
                 This is set automatically if you are using `textual run` with the `dev` switch.
             logger: Custom logger to send callback messages to.
 
         Raises:
             CssPathError: When the supplied CSS path(s) are an unexpected type.
         """
         super().__init__(
+            layout=layout,
             driver_class=driver_class,
             css_path=css_path,
             watch_css=watch_css,
         )
         # Manually set up observer manager mixin since App inheritance does not automatically trigger.
-        ObserverManager.__init__(self, logger=logger)
+        ObserverManager.__init__(self, logger=logger or logging.root)
 
     def apply_update(
         self,
         observer_id: str,
         component: Widget,
         component_id: str,
         component_property: str,
@@ -180,15 +221,15 @@
         try:
             return self.query_one(f"#{component_id}")
         except NoMatches:
             return None
 
     def on_mount(self, _: events.Mount) -> None:
         """Ensure the logger is fully loaded after mounting."""
-        if isinstance(self.logger, NullLogger):
+        if self.logger == logging.root:
             self.logger = self.log
 
     def _register_widget_observers(self, widget: Widget) -> None:
         """Enable observers for a newly added widget and its reactive attributes if it has an ID."""
         # Do not watch any widgets or properties for changes that have not had an observer set up.
         if widget.id not in self._observer_map:
             return
```

### Comparing `textology-0.0.4/textology/history.py` & `textology-0.0.5/textology/history.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.4/textology/observers/__init__.py` & `textology-0.0.5/textology/observers/__init__.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.4/textology/observers/_dependencies.py` & `textology-0.0.5/textology/observers/_dependencies.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.4/textology/observers/_managers.py` & `textology-0.0.5/textology/observers/_managers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 """Managers for routing component input/output requests via observation callbacks."""
 
 from __future__ import annotations
 
 import abc
+import asyncio
 import functools
 import logging
 from collections import defaultdict
+from inspect import isawaitable
 from typing import Any
 from typing import Callable
+from typing import Coroutine
 
 from textology.logging import NullLogger
 
+from ._dependencies import Dependency
 from ._dependencies import Modified
 from ._dependencies import NoUpdate
 from ._dependencies import Select
 from ._dependencies import Update
 from ._dependencies import flatten_dependencies
 from ._exceptions import PreventUpdate
 from ._exceptions import UnknownObserver
 
 # Type alias to represent function receiving 2 arguments (old value and new value) and returning nothing.
-ValueUpdateHandler = Callable[[Any, Any], None]
+ValueUpdateHandler = Callable[[Any, Any], Coroutine]
 
 
 class Observer:
     """Specification details for an input/output observer."""
 
     def __init__(
         self,
@@ -119,50 +123,55 @@
             value: Updated value to apply to the property.
         """
         setattr(component, component_property, value)
 
     def _generate_callback(self, modified_id: str, modified_property: str, observer: Observer) -> ValueUpdateHandler:
         """Create a callback wrapper that will call the original function with input/output management applied."""
 
-        def _on_update(old_value: Any, new_value: Any) -> None:
+        async def _on_update(old_value: Any, new_value: Any) -> None:
             """Process value changes for a component property and apply the requested update operations."""
             update_components = self._get_update_components(observer)
             if not update_components:
                 # One or more components missing, do not trigger callback.
                 return
+            observer_id = observer.observer_id
             args = []
-            args_setup_error = None
             for dep in observer.modifications + observer.selections:
                 if dep.component_id == modified_id and dep.component_property == modified_property:
                     args.append(old_value if isinstance(dep, Select) else new_value)
                 else:
                     try:
                         args.append(
                             self.get_callback_arg(observer.observer_id, dep.component_id, dep.component_property)
                         )
                     except Exception as error:  # pylint: disable=broad-exception-caught
-                        args_setup_error = error
-                        break
+                        self.on_callback_error(observer_id, error)
+                        return
 
-            observer_id = observer.observer_id
-            updates = None
             try:
-                if args_setup_error:
-                    raise args_setup_error
                 updates = observer.callback(*args) if not observer.external else self.send_callback(observer_id, *args)
+                if isawaitable(updates):
+                    updates = await updates
             except PreventUpdate:
-                pass
+                updates = None
             except BaseException as error:  # pylint: disable=broad-exception-caught
                 # Catch all errors to prevent fatal crashes in application callback loops.
                 self.on_callback_error(observer_id, error)
+                updates = None
 
             if updates:
-                for update_id, properties in updates.items():
-                    for update_property, value in properties.items():
-                        self.apply_update(observer_id, update_components[update_id], update_id, update_property, value)
+                try:
+                    for update_id, properties in updates.items():
+                        for update_property, value in properties.items():
+                            self.apply_update(
+                                observer_id, update_components[update_id], update_id, update_property, value
+                            )
+                except BaseException as error:  # pylint: disable=broad-exception-caught
+                    # Catch all errors to prevent fatal crashes in application callback loops.
+                    self.on_callback_error(observer_id, error)
 
         return _on_update
 
     def generate_callbacks(self, component_id: str, component_property: str) -> list[ValueUpdateHandler]:
         """Create callbacks that will manage input/output operations for all functions registered to id/property combo.
 
         Args:
@@ -258,15 +267,15 @@
         self.logger.warning(
             f'External callback {observer_id} is forwarding to local callback: override "send_callback" in {type(self)} or remove "external" from callback'
         )
         return observer.callback(*callback_args)
 
     def when(
         self,
-        *args: Any,
+        *args: Dependency,
     ) -> Callable:
         """Register a callback that triggers when observed values change.
 
         Example:
             @app.when(
                 Modified('url', 'path'),
                 Update('content-wrapper', 'content'),
@@ -310,15 +319,18 @@
     def __setattr__(self, name: str, value: Any) -> None:
         """Route attribute update request to observed value container, or original attribute."""
         if name != "_observed_values" and name in self._observed_values:
             observer = self._observed_values[name]
             old_value = observer.value
             observer.value = value
             if old_value != value and observer.callback:
-                observer.callback(old_value, value)
+                result = observer.callback(old_value, value)
+                if isawaitable(result):
+                    loop = asyncio.get_event_loop()
+                    loop.create_task(result)
         else:
             super().__setattr__(name, value)
 
     def __setup_observers__(self) -> None:
         """Initialize all observed attributes for updates."""
         for name in dir(self):
             value = getattr(self, name)
@@ -353,17 +365,19 @@
         self.callback = callback
 
 
 def _create_callback(func: Callable, updates: list[Update]) -> Callable:
     """Wrap a function with additional callback management, such as error handling and result standardization."""
 
     @functools.wraps(func)
-    def _callback(*args: Any, **kwargs: Any) -> dict[str, dict[str, Any]]:
+    async def _callback(*args: Any, **kwargs: Any) -> dict[str, dict[str, Any]]:
         """Wrap original function with additional callback management such as conversion to standardized result map."""
         results = func(*args, **kwargs)  # Invoke original callback.
+        if isawaitable(results):
+            results = await results
         if not isinstance(results, (list, tuple)):
             results = [results]
 
         if results is NoUpdate or isinstance(results, NoUpdate):
             raise PreventUpdate()
 
         component_updates = defaultdict(dict)
```

### Comparing `textology-0.0.4/textology/pytest_utils.py` & `textology-0.0.5/textology/pytest_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Utilities for helping run unit tests with pytest."""
 
 import json
 import os
 import platform
 import sqlite3
 import time
+from dataclasses import dataclass
 from datetime import datetime
 from os import PathLike
 from pathlib import Path
 from types import ModuleType
 from typing import Callable
 from typing import Iterable
 
@@ -22,20 +23,26 @@
 from textology import __version__
 
 OPT_SNAP_REPORT = "--txtology-snap-report"
 OPT_SNAP_ROOT = "--txtology-snap-root"
 OPT_SNAP_TEMPLATE = "--txtology-snap-template"
 OPT_SNAP_UPDATE = "--txtology-snap-update"
 
-TXTOLOGY_APP_KEY = pytest.StashKey[App]()
-TXTOLOGY_EXPECTED_SVG_KEY = pytest.StashKey[str]()
-TXTOLOGY_EXPECTED_PATH_KEY = pytest.StashKey[str]()
-TXTOLOGY_RESULT_SVG_KEY = pytest.StashKey[str]()
-TXTOLOGY_SNAPSHOT_TEST = pytest.StashKey[bool]()
-TXTOLOGY_SNAPSHOT_TEST_PASS = pytest.StashKey[bool]()
+TXTOLOGY_SNAPSHOTS = pytest.StashKey[list]()
+
+
+@dataclass
+class SnapshotFailure:
+    """Class for keeping track of a single snapshot failure in a test."""
+
+    pilot: Pilot
+    result: bool = False
+    result_svg: str | None = None
+    expected_svg: str | None = None
+    expected_path: str | None = None
 
 
 async def auto_pilot(
     pilot: Pilot,
     press: Iterable[str] = (),
     wait_for_animation: bool = True,
 ) -> None:
@@ -71,18 +78,19 @@
         SVG screenshot of the current screen.
     """
     await auto_pilot(pilot, press, wait_for_animation=wait_for_animation)
     svg = pilot.app.export_screenshot(title=snap_title)
     return svg
 
 
-async def compare_snapshots(
+async def compare_snapshots(  # pylint: disable=too-many-arguments
     request: FixtureRequest,
     pilot: Pilot,
     compare_to: str | PathLike | None = None,
+    test_suffix: str | None = None,
     press: Iterable[str] = (),
     snap_title: str = None,
     wait_for_animation: bool = True,
 ) -> bool:
     """Automate user actions, snapshot/screenshot the application, and compare the results.
 
     Compare a saved snapshot/screenshot of an application with a screenshot of the active application.
@@ -90,49 +98,60 @@
     New screenshots should only be permanently saved if manually validated to be correct.
 
     Args:
         request: Access to the requesting test context.
         pilot: Active test pilot for an application.
         compare_to: Path to a saved snapshot.
             Defaults to: <directory of test file>/snapshots/<name of test>.svg
+        test_suffix: Optional suffix to add to the snapshot image name after the name of the test.
+            Mutually exclusive with "compare_to" full path being provided.
         press: Key presses to run before waiting for animations to complete.
         snap_title: The title of the exported screenshot or None to use app title.
         wait_for_animation: Whether to wait for animations to complete before returning.
 
     Returns:
         True if the currently saved snapshot matches the newly generated snapshot, false otherwise.
     """
+    if compare_to and test_suffix:
+        raise ValueError("Cannot provide both a full compare_to path and test_suffix in snapshot tests")
     result_svg = await capture_snapshot(
         pilot,
         press=press,
         snap_title=snap_title,
         wait_for_animation=wait_for_animation,
     )
 
     expected_svg = None
     if not compare_to:
-        compare_to = Path(request.fspath).parent / "snapshots" / f"{request.node.name}.svg"
+        image_name = request.node.name
+        if test_suffix:
+            image_name = f"{image_name}_{test_suffix}"
+        compare_to = Path(request.fspath).parent / "snapshots" / f"{image_name}.svg"
     if os.path.exists(compare_to):
         expected_svg = Path(compare_to).read_text(encoding="UTF-8")
 
     result = result_svg == expected_svg
     if request.config.getoption(OPT_SNAP_UPDATE):
         failure_file = Path(compare_to)
         failure_file.parent.mkdir(parents=True, exist_ok=True)
         failure_file.write_text(result_svg, encoding="UTF-8")
         result = True
 
     node = request.node
-    node.stash[TXTOLOGY_SNAPSHOT_TEST] = True
-    node.stash[TXTOLOGY_SNAPSHOT_TEST_PASS] = result
     if result is False:
-        node.stash[TXTOLOGY_APP_KEY] = pilot.app
-        node.stash[TXTOLOGY_RESULT_SVG_KEY] = result_svg
-        node.stash[TXTOLOGY_EXPECTED_SVG_KEY] = expected_svg
-        node.stash[TXTOLOGY_EXPECTED_PATH_KEY] = str(compare_to)
+        node.stash[TXTOLOGY_SNAPSHOTS] = node.stash.get(TXTOLOGY_SNAPSHOTS, [])
+        node.stash[TXTOLOGY_SNAPSHOTS].append(
+            SnapshotFailure(
+                pilot=pilot,
+                result=result,
+                result_svg=result_svg,
+                expected_svg=expected_svg,
+                expected_path=str(compare_to),
+            )
+        )
     return result
 
 
 @pytest_asyncio.fixture(name="compare_snapshots")
 async def compare_snapshots_fixture(request: FixtureRequest) -> Callable:
     """Pytest fixture to automate user actions, snapshot/screenshot the application, and compare the results.
 
@@ -145,27 +164,30 @@
     Returns:
         Generated fixture to allow reuse multiple times in the same test.
     """
 
     async def _compare_snapshots(
         app_or_pilot_or_module: App | Pilot | ModuleType,
         compare_to: str | PathLike | None = None,
+        test_suffix: str | None = None,
         press: Iterable[str] = (),
         snap_title: str = None,
         wait_for_animation: bool = True,
     ) -> bool:
         """Generated fixture to automate user actions, snapshot/screenshot the application, and compare the results.
 
         See "compare_snapshots()" for more information. This is an alias to provide more direct access via pytest
         without the need to import the utilities manually, or pass along other pytest fixtures.
 
         Args:
             app_or_pilot_or_module: Application, application test pilot, or module containing either.
             compare_to: Path to a saved snapshot.
                 Defaults to: <directory of test file>/snapshots/<name of test>.py
+            test_suffix: Optional suffix to add to the snapshot image name after the name of the test.
+                Mutually exclusive with "compare_to" full path being provided.
             press: Key presses to run before waiting for animations to complete.
             snap_title: The title of the exported screenshot or None to use app title.
             wait_for_animation: Whether to wait for animations to complete before returning.
 
         Returns:
             True if the currently saved snapshot matches the newly generated snapshot, false otherwise.
         """
@@ -177,30 +199,40 @@
                     break
         if not isinstance(app_or_pilot_or_module, Pilot):
             async with app_or_pilot_or_module.run_test() as pilot:
                 return await compare_snapshots(
                     request,
                     pilot,
                     compare_to=compare_to,
+                    test_suffix=test_suffix,
                     press=press,
                     snap_title=snap_title,
                     wait_for_animation=wait_for_animation,
                 )
         return await compare_snapshots(
             request,
             app_or_pilot_or_module,
             compare_to=compare_to,
+            test_suffix=test_suffix,
             press=press,
             snap_title=snap_title,
             wait_for_animation=wait_for_animation,
         )
 
     yield _compare_snapshots
 
 
+def _snapshot_failure_factory(cur: sqlite3.Cursor, row: tuple) -> dict:
+    """Factory to convert DB rows into dicts, and rehydrate special types."""
+    fields = [column[0] for column in cur.description]
+    result = dict(zip(fields, row))
+    result["app"] = json.loads(result["app"])
+    return result
+
+
 def _get_session_root(session: pytest.Session) -> Path:
     """Find the testing session root for storing reports and shared results when run via parallel processing."""
     root_opt = session.config.getoption(OPT_SNAP_ROOT)
     pytest_root = Path(root_opt) if root_opt else Path(session.config.rootdir) / ".pytest_textology"
     if not pytest_root.exists():
         pytest_root.mkdir(parents=True, exist_ok=True)
         (pytest_root / ".gitignore").write_text("# Created automatically by textology pytest plugin.\n*\n")
@@ -274,35 +306,26 @@
     Uses basic sqlite3 database for simple locking between processes.
     """
     session_root = _get_session_root(session)
     if hasattr(session, "items"):
         with sqlite3.connect(session_root / "items.db") as con:
             cursor = con.cursor()
             for item in session.items:
-                if not item.stash.get(TXTOLOGY_SNAPSHOT_TEST, False):
-                    continue
-                if item.stash.get(TXTOLOGY_SNAPSHOT_TEST_PASS, False):
-                    continue
-                _write_snapshot_item(item, cursor)
+                for snapshot in item.stash.get(TXTOLOGY_SNAPSHOTS, []):
+                    if snapshot.result:
+                        continue
+                    _write_snapshot_failure(item, snapshot, cursor)
             con.commit()
 
     if getattr(session.config, "workerinput", None) is not None:
         # This is a worker process, no further action should be performed since session is not shared.
         return
 
     with sqlite3.connect(session_root / "items.db") as con:
-
-        def dict_factory(cur: sqlite3.Cursor, row: tuple) -> dict:
-            """Factory to convert DB rows into dicts, and rehydrate special types."""
-            fields = [column[0] for column in cur.description]
-            result = dict(zip(fields, row))
-            result["app"] = json.loads(result["app"])
-            return result
-
-        con.row_factory = dict_factory
+        con.row_factory = _snapshot_failure_factory
         cursor = con.cursor()
         failures = cursor.execute("SELECT * FROM snapshot_failures").fetchall()
 
     if failures:
         final_result = {
             "timestamp": str(datetime.utcnow()),
             "exitstatus": exitstatus,
@@ -366,34 +389,34 @@
             f"file://{config.txtology_report_path}\n"
             "\n"
             "If the new snapshots are correct, rerun using the following syntax to update the saved files:\n"
             f"pytest {OPT_SNAP_UPDATE}"
         )
 
 
-def _write_snapshot_item(item: pytest.Item, cursor: sqlite3.Cursor) -> None:
+def _write_snapshot_failure(item: pytest.Item, snapshot: SnapshotFailure, cursor: sqlite3.Cursor) -> None:
     """Save a snapshot test result from a worker process to a shared database table."""
     path, line_index, name = item.reportinfo()
-    app = item.stash.get(TXTOLOGY_APP_KEY, None)
+    app = snapshot.pilot.app
     cursor.execute(
         "INSERT INTO snapshot_failures VALUES ("
         ":path,"
         ":name,"
         ":line,"
         ":result,"
         ":expected,"
         ":expectedPath,"
         ":app)",
         {
             "path": str(path),
             "name": name,
             "line": line_index + 1,
-            "result": item.stash.get(TXTOLOGY_RESULT_SVG_KEY, None),
-            "expected": item.stash.get(TXTOLOGY_EXPECTED_SVG_KEY, None),
-            "expectedPath": item.stash.get(TXTOLOGY_EXPECTED_PATH_KEY, None),
+            "result": snapshot.result_svg,
+            "expected": snapshot.expected_svg,
+            "expectedPath": snapshot.expected_path,
             "app": json.dumps(
                 {
                     "title": app.title,
                     "python_class": str(app.__class__),
                     "driver_class": str(app.driver_class),
                     "classes": " ".join(cls for cls in app.classes) if app.classes else "",
                     "css_path": app.css_path,
```

### Comparing `textology-0.0.4/textology/router.py` & `textology-0.0.5/textology/router.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.4/textology/test-template.html` & `textology-0.0.5/textology/test-template.html`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
         .flex-column {
             display: flex;
             flex-direction: column;
         }
 
         .test-img-wrapper {
-            flex: 1;
+            width: 50%;
             margin: 8px;
         }
 
         .test-img-diff {
             mix-blend-mode: difference;
             position: absolute;
             width: 100%;
```

### Comparing `textology-0.0.4/textology/widgets/__init__.py` & `textology-0.0.5/textology/widgets/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,13 +13,14 @@
 from ._extensions import ExtendedWidget
 from ._extensions import WidgetExtension
 from ._horizontal_menus import HorizontalMenus
 from ._label import Label
 from ._list_item import LIST_ITEM_EVENT_IGNORES
 from ._list_item import ListItem
 from ._list_item_header import ListItemHeader
+from ._list_item_meta import ListItemMeta
 from ._list_view import ListView
 from ._location import Location
 from ._modal_dialog import ModalDialog
 from ._static import Static
 from ._store import JsonType
 from ._store import Store
```

### Comparing `textology-0.0.4/textology/widgets/_button.py` & `textology-0.0.5/textology/widgets/_button.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.4/textology/widgets/_containers.py` & `textology-0.0.5/textology/widgets/_containers.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.4/textology/widgets/_extensions.py` & `textology-0.0.5/textology/widgets/_extensions.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.4/textology/widgets/_horizontal_menus.py` & `textology-0.0.5/textology/widgets/_horizontal_menus.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,73 +1,94 @@
 """Progressive horizontal set of ListViews with tracking for active item and peeking at next menu."""
 
 from typing import Any
 from typing import Callable
+from typing import ClassVar
 
 from textual import containers
 from textual import events
+from textual.binding import Binding
+from textual.binding import BindingType
 from textual.reactive import reactive
 from textual.widget import Widget
 
 from ._extensions import WidgetExtension
 from ._list_item import ListItem
 from ._list_item_header import ListItemHeader
+from ._list_item_meta import ListItemMeta
 from ._list_view import ListView
 
 
 class HorizontalMenus(WidgetExtension, containers.HorizontalScroll):
     """Progressive horizontal set of ListViews with tracking for active item(s).
 
     Compared to a Tree view, horizontal menus provide quick navigation and visibility into nested objects.
     The menus can be quickly focused, selected, etc., with less vertical traversal in large objects.
     "Previewing" the next menu in a set of menus is also allowed.
     """
 
+    BINDINGS: ClassVar[list[BindingType]] = [
+        Binding("left", "focus_previous", show=False),
+        Binding("right", "focus_next", show=False),
+    ]
+
     # Currently focused item across sub-menus.
     focused: ListItem | None = reactive(None, repaint=False, init=False)
     # Current primary item highlighted across sub-menus (right-most).
     highlighted: ListItem | None = reactive(None, repaint=False, init=False)
     # All highlighted items across sub-menus.
     highlights: list[ListItem] = reactive([], repaint=False, init=False)
 
     def __init__(
         self,
-        *children: Widget,
+        *children: Widget | ListItem | ListItemMeta,
         name: str | None = None,
         id: str | None = None,
         classes: str | None = None,
         disabled: bool = False,
         can_focus: bool = False,
-        menu_creator: Callable[[int, list[ListItem]], Widget] = None,
+        menu_creator: Callable[[int, list[ListItem]], Widget] | None = None,
         **extension_configs: Any,
     ) -> None:
         """Initialize horizontal menus.
 
         Args:
-            *children: Initial menus to display.
+            *children: Initial menus, or menu items, to display.
                 Each "menu" widget must contain a ListView, but does not have to be a ListView itself.
+                If children are ListItem or ListItemMeta objects, an initial ListView will be made with menu_creator.
             name: The name of the widget.
             id: The ID of the widget in the DOM.
             classes: The CSS classes for the widget.
             disabled: Whether the widget is disabled or not.
-            can_focus: Whether the widget can be focused, or only the children.
+            can_focus: Whether the parent widget can be focused, or only the children widgets.
                 If enabled, it will take focus after all the nested ListViews, but before the next sibling.
             menu_creator: Called to create new sub-menus when an item with children is highlighted.
             extension_configs: Widget extension configurations, such as dynamically provided local callbacks by name.
         """
+        self.menu_creator = menu_creator or self._default_menu_creator
+        if any(isinstance(child, (ListItem, ListItemMeta)) for child in children):
+            if not all(isinstance(child, (ListItem, ListItemMeta)) for child in children):
+                raise ValueError("All initial children must be of same type: ListItem, ListItemMeta, or ListView")
+            for child in children:
+                child.menu_index = 0
+            children = [
+                self.menu_creator(
+                    0,
+                    [child.to_item() if isinstance(child, ListItemMeta) else child for child in children],
+                )
+            ]
         super().__init__(
             *children,
             name=name,
             id=id,
             classes=classes,
             disabled=disabled,
         )
         self.__extend_widget__(**extension_configs)
         self.can_focus = can_focus
-        self.menu_creator = menu_creator
         self.menus = []
         for child in children or []:
             menu = None
             if isinstance(child, ListView):
                 menu = child
             else:
                 for node in child.walk_children():
@@ -76,30 +97,42 @@
                         break
             if not menu:
                 raise ValueError("All menu children must contain a ListView widget")
             self.menus.append(menu)
 
     def _add_menu(self, items: list[ListItem]) -> None:
         """Create and add a menu to the list of available menus."""
-        new_menu = self.menu_creator(len(self.menus), items)
-        if new_menu:
+        if new_menu := self.menu_creator(len(self.menus), items):
             self.mount(new_menu)
             list_view = None
             if isinstance(new_menu, ListView):
                 list_view = new_menu
             else:
                 for node in new_menu.walk_children():
                     if isinstance(node, ListView):
                         list_view = node
                         break
             if not list_view:
                 raise ValueError("Menus must contain a ListView widget for navigation")
             self.menus.append(list_view)
 
-    def _find_highlighted(self) -> ListItem:
+    @staticmethod
+    def _default_menu_creator(menu_index: int, items: list) -> ListView | None:
+        """Default menu factory to create submenus when another submenu highlight changes."""
+        return (
+            ListView(
+                *items,
+                initial_index=None,
+                classes=f"--horizontal-menu-{menu_index}",
+            )
+            if any(not isinstance(item, ListItemHeader) for item in items)
+            else None
+        )
+
+    def _find_highlighted(self) -> ListItem | None:
         """Find the rightmost highlighted (most recent) item across the menu hierarchy."""
         for menu in reversed(self.menus):
             highlighted = menu.highlighted_child
             if highlighted:
                 return highlighted
         return None
 
@@ -155,19 +188,37 @@
     def show_menu(self, index: int, items: list[ListItem]) -> None:
         """Show a new set of items, either by creating a new menu, or updating an existing menu.
 
         Args:
             index: Position of the menu to create or update.
             items: New items to show in the menu at the provided index.
         """
+        for item in items:
+            item.menu_index = index
         if index >= len(self.menus):
             self._add_menu(items)
         else:
             self._update_menu(index, items)
 
     def _update_menu(self, index: int, new_items: list[ListItem]) -> None:
         """Update the items in an existing menu."""
         # Do not count headers towards the available items to display in a sub-menu.
         non_headers = [item for item in new_items if not isinstance(item, ListItemHeader)]
         self.remove_menus(index if non_headers else index - 1)
         if index < len(self.menus):
             self.menus[index].replace(new_items)
+
+    def watch_highlighted(self, old_value: ListItem | None, new_value: ListItem | None) -> None:
+        """Monitor the highlighted item to update the submenus.
+
+        Args:
+            old_value: Previously highlighted list item.
+            new_value: Newly highlighted list item.
+        """
+        if new_value == old_value or not new_value:
+            return
+        menu_items = new_value.data.get("menu_items")
+        if menu_items:
+            list_items = [item.to_item() for item in menu_items]
+            self.show_menu(new_value.menu_index + 1, list_items)
+        else:
+            self.remove_menus(new_value.menu_index)
```

### Comparing `textology-0.0.4/textology/widgets/_label.py` & `textology-0.0.5/textology/widgets/_label.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.4/textology/widgets/_list_item.py` & `textology-0.0.5/textology/widgets/_list_item.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,19 +36,20 @@
 
         Args:
             *children: Child widgets.
             name: The name of the widget.
             id: The ID of the widget in the DOM.
             classes: The CSS classes for the widget.
             disabled: Whether the widget is disabled or not.
-            data: Metadata about the list item that can be used by later events, highlight selections, etc.
-                If no child is provided for display, the data will be searched for a "name" key to use in a Label.
+            data: Optional data associated with the list item.
+                If no child is provided for display, the data will be searched for a "label" key to use in a Label.
             extension_configs: Widget extension configurations, such as dynamically provided local callbacks by name.
         """
-        if not children and (data and "name" in data):
-            children = [Label(data["name"], disable_messages=LIST_ITEM_EVENT_IGNORES)]
+        if not children and (data and "label" in data):
+            children = [Label(data["label"], disable_messages=LIST_ITEM_EVENT_IGNORES)]
 
         super().__init__(*children, name=name, id=id, classes=classes, disabled=disabled)
         if "disable_messages" not in extension_configs:
             extension_configs["disable_messages"] = LIST_ITEM_EVENT_IGNORES
         self.__extend_widget__(**extension_configs)
         self.data = data
+        self.menu_index = None
```

### Comparing `textology-0.0.4/textology/widgets/_list_item_header.py` & `textology-0.0.5/textology/widgets/_list_item_header.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,33 +26,37 @@
         self,
         *children: Widget,
         name: str | None = None,
         id: str | None = None,
         classes: str | None = None,
         disabled: bool = False,
         disable_click: bool = True,
+        data: Any = None,
         **extension_configs: Any,
     ) -> None:
         """Initialize a ListItemHeader with extension arguments.
 
         Args:
             *children: Child widgets.
             name: The name of the widget.
             id: The ID of the widget in the DOM.
             classes: The CSS classes for the widget.
             disabled: Whether the widget is disabled or not.
-            disable_click: Whether clicking the widget it disabled
+            disable_click: Whether clicking the widget it disabled.
+            data: Optional data associated with the list item.
+                If no child is provided for display, the data will be searched for a "label" key to use in a Label.
             extension_configs: Widget extension configurations, such as dynamically provided local callbacks by name.
         """
         super().__init__(
             *children,
             name=name,
             id=id,
             classes=classes,
             disabled=disabled,
+            data=data,
             **extension_configs,
         )
         self.disable_click = disable_click
 
     async def _on_click(self, event: Click) -> None:
         """Disable clicking header items."""
         if self.disable_click:
```

### Comparing `textology-0.0.4/textology/widgets/_list_view.py` & `textology-0.0.5/textology/widgets/_list_view.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.4/textology/widgets/_location.py` & `textology-0.0.5/textology/widgets/_location.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from urllib.parse import urlparse
 
 from textual import events
 from textual.message import Message
 from textual.reactive import reactive
 
 from textology.history import History
-from textology.logging import NullLogger
 from textology.router import Endpoint
 from textology.router import Request
 from textology.router import Router
 
 from ._extensions import ExtendedWidget
 
 
@@ -98,15 +97,15 @@
             enable_url_events: Whether URL update events should be sent.
             enable_history_events: Whether history update events should be sent.
             extension_configs: Widget extension configurations, such as dynamically provided local callbacks by name.
         """
         super().__init__(id=id, **extension_configs)
         self._initial_path = path
         # Manually set up router mixin since Widget inheritance does not automatically trigger.
-        Router.__init__(self, logger=logger)
+        Router.__init__(self, logger=logger or logging.root)
         self._history = History()
         self.url_events_enabled = enable_url_events
         self.history_events_enabled = enable_history_events
 
     def back(self) -> int:
         """Go back in the history.
 
@@ -190,15 +189,15 @@
 
         Alias for "url". Always updates history. For non-historical updates, see "update_url".
         """
         self.url = new_value
 
     def _on_mount(self, _: events.Mount) -> None:
         """Ensure the logger and initial path are fully loaded after mounting."""
-        if isinstance(self.logger, NullLogger):
+        if self.logger == logging.root:
             self.logger = self.log
         self.url = self._initial_path
 
     def reload(self) -> None:
         """Reload the most recent URL in the history."""
         self.update_url(self._history.value, save=False)
```

### Comparing `textology-0.0.4/textology/widgets/_modal_dialog.py` & `textology-0.0.5/textology/widgets/_modal_dialog.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.4/textology/widgets/_static.py` & `textology-0.0.5/textology/widgets/_static.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.4/textology/widgets/_store.py` & `textology-0.0.5/textology/widgets/_store.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.4/textology.egg-info/PKG-INFO` & `textology-0.0.5/textology.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: textology
-Version: 0.0.4
-Summary: Extensions for creating Terminal User Interfaces
+Version: 0.0.5
+Summary: Textual extensions for creating Terminal User Interfaces
 Home-page: https://github.com/dfrtz/textology
 Author: David Fritz
-Maintainer: David Fritz
 License: MIT
 Project-URL: Issue Tracker, https://github.com/dfrtz/textology/issues
 Project-URL: Source Code, https://github.com/dfrtz/textology
 Platform: MacOS
 Platform: Linux
 Platform: Windows
 Classifier: Development Status :: 4 - Beta
@@ -27,18 +26,20 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: full-dev
 License-File: LICENSE
 
+
 <div align="center">
-  <img src="https://github.com/dfrtz/textology/blob/main/docs/banner.svg" width="450">
+  <img src="https://raw.githubusercontent.com/dfrtz/textology/main/docs/banner.svg" width="450">
 </div>
 
 -----------------
 
 
 [![os: windows mac linux](https://img.shields.io/badge/os-linux_|_macos_|_windows-blue)](https://docs.python.org/3.10/)
 [![python: 3.10+](https://img.shields.io/badge/python-3.10_|_3.11-blue)](https://docs.python.org/3.10/)
@@ -66,18 +67,19 @@
 as possible to a traditional GUI experience straight from a terminal. Why? Not all environments allow full graphical
 library access, web access, etc. Specifically, Textology is inspired by the designs of frameworks such as
 Dash/FastAPI/Flask and their use of routing, context managers, and observation patterns. Textology also receives
 inspiration from other UI frameworks external to Python, such as iOS, Android, and Web frameworks. Most importantly
 however, Textology is an extension of Textual: it does not replace Textual, but rather provides additional options
 on top of the core framework.
 
-Before using Textology, be comfortable with Textual. Textology is NOT a replacement for Textual, it is an
+Before using Textology, be comfortable with Textual. For tutorials, guides, etc., refer to the
+[Textual Documentation](https://textual.textualize.io/guide/). Textology is NOT a replacement for Textual, it is an
 extension. Callbacks, widgets, screens, event lifecycles, etc., from Textual still apply to Textology extended
 widgets and applications. For other advanced features, familiarity with Dash/FastAPI/Flask principles will help.
-Examples are included for advanced features, such as callback based applications.
+Examples for Textology extensions, such as callback based applications, are included in this documentation.
 
 
 ## Table Of Contents
 
   * [Compatibility](#compatibility)
   * [Key Features](#top-features)
   * [Getting Started](#getting-started)
@@ -97,59 +99,66 @@
 
 - Extended basic widgets, such as:
   - Buttons with ability to declare callbacks inline, and track click counts
   - ListItems with metadata objects and ability to disable event messages
 - New widgets, such as:
   - ListItemHeaders (non-interactive ListItems)
   - HorizontalMenus (walkable list of ListViews with peeking at following lists)
-- "Observer" application, with "event driven architecture" to detect changes and automatically update elements in UI.
+- "Observer" apps, with "event driven architecture" to detect changes and automatically update UI elements.
 - Enhanced testing support
   - Parallel tests via python-xdist
   - Custom testing arguments, such as updating snapshots on failures
 
 
 ## Getting Started
 
 ### Installation
 
 Install Textology via pip:
 ```shell
 pip install textology
 ```
 
-For dev requirements, use the additional `[dev]` package, which installs Textual development tools and extra QA tools:
+For development of applications based on Textual/Textology (but not development of Textology itself), use the
+`[dev]` package. This installs extra Textual development tools, and requirements for Textology testing extensions.
 ```shell
 pip install textology[dev]
 ```
 
+For full development of Textology itself, use the `[full-dev]` package. This installs Textual development tools,
+requirements for Textology testing extensions, and full QA requirements to meet commit standards. This version
+has the highest library requirements, in order to match the versions used by Textology itself for testing. Required if
+developing Textology itself, or recommended if looking to match/exceed the level of QA testing used by Textology.
+```shell
+pip install textology[full-dev]
+```
+
 ### Extended Applications
 
 Some Textology app classes, such as `ObservedApp`, can replace any regular Textual App, and be used as is without any
 extensions turned on. Here is an example of the most commonly used extended application, `ObservedApp`, and its
 primary extended functionality being used. More detailed examples of applications based around routes, callbacks,
 and standard Textual applications can be found in [Examples](https://github.com/dfrtz/textology/examples).
 
 - Observer/callback application (automatic attribute monitoring and updates by element IDs without manual queries):
 ```python
 from textology.apps import ObservedApp
 from textology.observers import Modified, Select, Update
 from textology.widgets import Button, Container, Label
 
-class SimpleApp(ObservedApp):
-    def compose(self):
-        yield Container(
-            Button('Ping', id='ping-btn'),
-            Button('Pong', id='pong-btn'),
-            Button('Sing-a-long', id='sing-btn'),
-            Container(
-                id="content",
-            ),
-        )
-
-app = SimpleApp()
+app = ObservedApp(
+    layout=Container(
+        Button('Ping', id='ping-btn'),
+        Button('Pong', id='pong-btn'),
+        Button('Sing-a-long', id='sing-btn'),
+        Container(
+            id="content",
+        ),
+    )
+)
 
 @app.when(
     Modified("ping-btn", "n_clicks"),
     Update("content", "children"),
 )
 def ping(clicks):
     return Label(f"Ping pressed {clicks}")
@@ -171,25 +180,84 @@
     if not ping_clicks or not pong_clicks:
         return Label(f"Press Ping and Pong first to complete the song!")
     return Label(f"Ping, pong, sing-a-long song pressed {song_clicks}")
 
 app.run()
 ```
 
+- Observation callbacks can also be async:
+```python
+@app.when(
+    Modified("pong-btn", "n_clicks"),
+    Update("content", "children"),
+)
+async def delayed_pong(clicks):
+    await asyncio.sleep(3)
+    return Label(f"Pong pressed {clicks} and updated 3 seconds later")
+```
+
+- <details>
+  <summary>Observer/callback application (Same as above, but with Dash compatibility object and calls)</summary>
+
+    ```python
+    from textology.dash_compat import DashCompatApp, Input, Output, State
+    from textology.widgets import Button, Container, Label
+
+    app = DashCompatApp(
+        layout=Container(
+            Button('Ping', id='ping-btn'),
+            Button('Pong', id='pong-btn'),
+            Button('Sing-a-long', id='sing-btn'),
+            Container(
+                id="content",
+            ),
+        )
+    )
+
+    @app.callback(
+        Input("ping-btn", "n_clicks"),
+        Output("content", "children"),
+    )
+    def ping(clicks):
+        return Label(f"Ping pressed {clicks}")
+
+    @app.callback(
+        Input("pong-btn", "n_clicks"),
+        Output("content", "children"),
+    )
+    def pong(clicks):
+        return Label(f"Pong pressed {clicks}")
+
+    @app.callback(
+        Input("sing-btn", "n_clicks"),
+        State("ping-btn", "n_clicks"),
+        State("pong-btn", "n_clicks"),
+        Output("content", "children"),
+    )
+    def song(song_clicks, ping_clicks, pong_clicks):
+        if not ping_clicks or not pong_clicks:
+            return Label(f"Press Ping and Pong first to complete the song!")
+        return Label(f"Ping, pong, sing-a-long song pressed {song_clicks}")
+
+    app.run()
+    ```
+
+ </details>
+
 ### Extended Widgets
 
 Native Textual widgets can be directly swapped out with Textology extended equivalents. They can then be used as is
 (standard Textual usage), or with extensions (via extra keyword arguments).
 
 - Basic swap (no extensions):
 ```python
 # Replace:
 from textual.widgets import Button
 
-# With
+# With:
 from textology.widgets import Button
 ```
 
 - Instance callback extension (avoid global watchers, name/ID checks in the event watchers, and event chaining):
 ```python
 from textology.widgets import Button
 
@@ -238,19 +306,20 @@
 
 - Basic snapshot test:
 ```python
 import pytest
 from textual import App
 from textual.widgets import Button
 
+class BasicApp(App):
+    def compose(self):
+        yield Button("Click me!")
+
 @pytest.mark.asyncio
-async def test_snapshot_with_app(compare_snapshots) -> None:
-    class BasicApp(App):
-        def compose(self):
-            yield Button("Click me!", id="btn")
+async def test_snapshot_with_app(compare_snapshots):
     assert await compare_snapshots(BasicApp())
 ```
 
 Other advanced testing features include:
 - Ability to pass and App, App Pilot, or a module containing an instantiated App or Pilot, to fixtures
 - Custom snapshot paths, including reusing the same snapshot across multiple tests
 - Automatic SVG updates with `pytest --txtology-snap-update`
```

### Comparing `textology-0.0.4/textology.egg-info/SOURCES.txt` & `textology-0.0.5/textology.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 LICENSE
+MANIFEST.in
 README.md
 requirements-dev.txt
+requirements-full-dev.txt
 requirements.txt
 setup.cfg
 setup.py
 textology/__init__.py
 textology/apps.py
+textology/dash_compat.py
 textology/history.py
 textology/logging.py
 textology/pytest_utils.py
 textology/router.py
 textology/test-template.html
 textology.egg-info/PKG-INFO
 textology.egg-info/SOURCES.txt
@@ -24,12 +27,13 @@
 textology/widgets/_button.py
 textology/widgets/_containers.py
 textology/widgets/_extensions.py
 textology/widgets/_horizontal_menus.py
 textology/widgets/_label.py
 textology/widgets/_list_item.py
 textology/widgets/_list_item_header.py
+textology/widgets/_list_item_meta.py
 textology/widgets/_list_view.py
 textology/widgets/_location.py
 textology/widgets/_modal_dialog.py
 textology/widgets/_static.py
 textology/widgets/_store.py
```

