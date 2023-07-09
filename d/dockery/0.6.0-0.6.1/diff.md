# Comparing `tmp/dockery-0.6.0.tar.gz` & `tmp/dockery-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dockery-0.6.0.tar", last modified: Sat Jul  1 22:04:02 2023, max compression
+gzip compressed data, was "dockery-0.6.1.tar", last modified: Sun Jul  9 04:29:01 2023, max compression
```

## Comparing `dockery-0.6.0.tar` & `dockery-0.6.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1082 2023-07-01 22:03:55.067526 dockery-0.6.0/LICENSE
--rw-r--r--   0        0        0     1636 2023-07-01 22:03:55.067526 dockery-0.6.0/README.md
--rw-r--r--   0        0        0      777 2023-07-01 22:04:02.795653 dockery-0.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-01 22:03:55.067526 dockery-0.6.0/src/dockery/__init__.py
--rw-r--r--   0        0        0     1760 2023-07-01 22:03:55.067526 dockery-0.6.0/src/dockery/custom_widgets.py
--rw-r--r--   0        0        0     6046 2023-07-01 22:03:55.067526 dockery-0.6.0/src/dockery/gui.py
--rw-r--r--   0        0        0     1775 2023-07-01 22:03:55.067526 dockery-0.6.0/src/dockery/images.py
--rw-r--r--   0        0        0     1883 2023-07-01 22:03:55.067526 dockery-0.6.0/src/dockery/logs.py
--rw-r--r--   0        0        0     3738 2023-07-01 22:03:55.067526 dockery-0.6.0/src/dockery/main.py
--rw-r--r--   0        0        0     1742 2023-07-01 22:03:55.067526 dockery-0.6.0/src/dockery/networks.py
--rw-r--r--   0        0        0     1070 2023-07-01 22:03:55.067526 dockery-0.6.0/src/dockery/style.css
--rw-r--r--   0        0        0     1328 2023-07-01 22:03:55.067526 dockery-0.6.0/src/dockery/utils.py
--rw-r--r--   0        0        0     1723 2023-07-01 22:03:55.067526 dockery-0.6.0/src/dockery/volumes.py
--rw-r--r--   0        0        0     2143 1970-01-01 00:00:00.000000 dockery-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-07-09 04:28:52.567377 dockery-0.6.1/LICENSE
+-rw-r--r--   0        0        0     1636 2023-07-09 04:28:52.567377 dockery-0.6.1/README.md
+-rw-r--r--   0        0        0      777 2023-07-09 04:29:01.383348 dockery-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-09 04:28:52.567377 dockery-0.6.1/src/dockery/__init__.py
+-rw-r--r--   0        0        0     4792 2023-07-09 04:28:52.567377 dockery-0.6.1/src/dockery/containers.py
+-rw-r--r--   0        0        0     1775 2023-07-09 04:28:52.567377 dockery-0.6.1/src/dockery/custom_widgets.py
+-rw-r--r--   0        0        0     1612 2023-07-09 04:28:52.567377 dockery-0.6.1/src/dockery/gui.py
+-rw-r--r--   0        0        0     1809 2023-07-09 04:28:52.567377 dockery-0.6.1/src/dockery/images.py
+-rw-r--r--   0        0        0     2019 2023-07-09 04:28:52.567377 dockery-0.6.1/src/dockery/logs.py
+-rw-r--r--   0        0        0     3738 2023-07-09 04:28:52.567377 dockery-0.6.1/src/dockery/main.py
+-rw-r--r--   0        0        0     1742 2023-07-09 04:28:52.571377 dockery-0.6.1/src/dockery/networks.py
+-rw-r--r--   0        0        0     1070 2023-07-09 04:28:52.571377 dockery-0.6.1/src/dockery/style.css
+-rw-r--r--   0        0        0     1353 2023-07-09 04:28:52.571377 dockery-0.6.1/src/dockery/utils.py
+-rw-r--r--   0        0        0     1723 2023-07-09 04:28:52.571377 dockery-0.6.1/src/dockery/volumes.py
+-rw-r--r--   0        0        0     2143 1970-01-01 00:00:00.000000 dockery-0.6.1/PKG-INFO
```

### Comparing `dockery-0.6.0/LICENSE` & `dockery-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dockery-0.6.0/README.md` & `dockery-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `dockery-0.6.0/pyproject.toml` & `dockery-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dockery"
-version = "0.6.0"
+version = "0.6.1"
 description = "Graphical interface for Docker in your console"
 authors = [
     { name = "Mariano Carrazana", email = "marianocarrazana@gmail.com" },
 ]
 dependencies = [
     "docker>=6.1.3",
     "textual>=0.28.0",
```

### Comparing `dockery-0.6.0/src/dockery/custom_widgets.py` & `dockery-0.6.1/src/dockery/custom_widgets.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         super().__init__(shrink=True, expand=True, **kargs)
 
     def render(self) -> TextType:
         return self.text
 
     def watch_color(self, new_color: str):
         if new_color != "":
-            self.styles.outline = (self.variant, new_color)
+            self.styles.outline = (self.variant, new_color) # type: ignore
 
     def on_mount(self) -> None:
         self.text = self.start_text
         self.color = self.start_color
 
 
 class ResponsiveGrid(VerticalScroll):
```

### Comparing `dockery-0.6.0/src/dockery/images.py` & `dockery-0.6.1/src/dockery/images.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,22 +37,23 @@
 
 
 class ImageWidget(Static):
     def __init__(self, image: Image, client: DockerClient, **kargs):
         self.image = image
         self.client = client
         self.attrs = image.attrs or {}
-        self.isize = self.attrs.get("Size", 0) / 1000 / 1000
+        self.isize = self.attrs.get("Size", 0) / 1000000
+        self.short_id = self.image.short_id.replace("sha256:", "")
         if self.image.tags:
             self.tag = self.image.tags[0]
         elif self.image.id:
             self.tag = self.image.id.replace("sha256:", "")
         else:
             self.tag = ""
         super().__init__(**kargs)
 
     def compose(self) -> ComposeResult:
         yield Vertical(
             Label("[b]" + self.tag),
-            Label(self.image.short_id.replace("sha256:", "")),
+            Label(self.short_id),
             Label(f"Size: {self.isize:.2f}MB"),
         )
```

### Comparing `dockery-0.6.0/src/dockery/logs.py` & `dockery-0.6.1/src/dockery/logs.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,20 +10,25 @@
 
 
 class LogsButton(Static):
     def __init__(self, container: Container, **kargs):
         self.container = container
         super().__init__(**kargs)
 
+    def on_mount(self) -> None:
+        self.logs_container = self.app.query_one(
+            "VerticalScroll#container-logs", VerticalScroll
+        )
+        self.tabs = self.app.query_one("#nav", Tabs)
+
     async def on_click(self) -> None:
-        cl = self.app.query_one("VerticalScroll#container-logs", VerticalScroll)
-        await cl.remove_children()
+        await self.logs_container.remove_children()
         lc = LogsContainer(self.container)
-        await cl.mount(lc)
-        self.app.query_one("#nav", Tabs).active = "container-logs"
+        await self.logs_container.mount(lc)
+        self.tabs.active = "container-logs"
 
     def compose(self) -> ComposeResult:
         yield CustomButton(":notebook:Logs", color="blue")
 
 
 class LogsContainer(TextLog):
     last_log = reactive("")
```

### Comparing `dockery-0.6.0/src/dockery/main.py` & `dockery-0.6.1/src/dockery/main.py`

 * *Files identical despite different names*

### Comparing `dockery-0.6.0/src/dockery/networks.py` & `dockery-0.6.1/src/dockery/networks.py`

 * *Files identical despite different names*

### Comparing `dockery-0.6.0/src/dockery/style.css` & `dockery-0.6.1/src/dockery/style.css`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 }
 
 .stats-text {
     width: 1fr;
 }
 
 .stats-text > Horizontal > ReactiveString {
-    width: 12;
+    width: 20;
     height: 1;
 }
 
 CustomButton {
     height: 3;
     padding: 1 2;
     width: auto;
```

### Comparing `dockery-0.6.0/src/dockery/utils.py` & `dockery-0.6.1/src/dockery/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,26 +21,26 @@
     if system_delta == 0:
         return 0.0
 
     percentage = (delta / system_delta) * len_cpu * 100
     return percentage
 
 
-def get_mem_usage(stats: dict) -> float:
+def get_mem_usage(stats: dict) -> tuple:
     mem_stats = stats["memory_stats"]
     if len(mem_stats) == 0:
-        return 0.0
+        return (0, 0.0)
     mem_used = (
         mem_stats["usage"]
         - mem_stats["stats"].get("cache", 0)
         + mem_stats["stats"]["active_file"]
     )
     limit = stats["memory_stats"]["limit"]
     percentage = mem_used / limit * 100
-    return percentage
+    return (mem_used/1000000, percentage)
 
 
 def var_dump(obj: Any, syntax: Literal["json", "yaml"] = "yaml"):
     if syntax == "yaml":
         text_obj = yaml.safe_dump(obj, indent=2)
     elif syntax == "json":
         text_obj = json.dumps(obj, default=str, indent=2)
```

### Comparing `dockery-0.6.0/src/dockery/volumes.py` & `dockery-0.6.1/src/dockery/volumes.py`

 * *Files identical despite different names*

### Comparing `dockery-0.6.0/PKG-INFO` & `dockery-0.6.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dockery
-Version: 0.6.0
+Version: 0.6.1
 Summary: Graphical interface for Docker in your console
 Author-Email: Mariano Carrazana <marianocarrazana@gmail.com>
 License: MIT
 Project-URL: Bug tracker, https://github.com/marianocarrazana/dockery/issues
 Project-URL: Source code, https://github.com/marianocarrazana/dockery
 Requires-Python: >=3.9
 Requires-Dist: docker>=6.1.3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dockery Version: 0.6.0 Summary: Graphical interface
+Metadata-Version: 2.1 Name: dockery Version: 0.6.1 Summary: Graphical interface
 for Docker in your console Author-Email: Mariano Carrazana
 gmail.com> License: MIT Project-URL: Bug tracker, https://github.com/
 marianocarrazana/dockery/issues Project-URL: Source code, https://github.com/
 marianocarrazana/dockery Requires-Python: >=3.9 Requires-Dist: docker>=6.1.3
 Requires-Dist: textual>=0.28.0 Requires-Dist: click>=8.1.3 Requires-Dist:
 pyyaml>=6.0 Description-Content-Type: text/markdown # dockery Graphical
 interface for Docker in your console [![Release](https://github.com/
```

