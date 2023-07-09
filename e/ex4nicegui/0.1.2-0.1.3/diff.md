# Comparing `tmp/ex4nicegui-0.1.2.tar.gz` & `tmp/ex4nicegui-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ex4nicegui-0.1.2.tar", last modified: Sun Jul  9 14:56:35 2023, max compression
+gzip compressed data, was "ex4nicegui-0.1.3.tar", last modified: Sun Jul  9 18:21:01 2023, max compression
```

## Comparing `ex4nicegui-0.1.2.tar` & `ex4nicegui-0.1.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 14:56:35.024792 ex4nicegui-0.1.2/
--rw-rw-rw-   0        0        0     1094 2023-06-30 08:17:10.000000 ex4nicegui-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      481 2023-07-09 14:56:35.013834 ex4nicegui-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       12 2023-07-05 06:11:55.000000 ex4nicegui-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-09 14:56:34.953557 ex4nicegui-0.1.2/ex4nicegui/
--rw-rw-rw-   0        0        0      366 2023-07-09 14:56:18.000000 ex4nicegui-0.1.2/ex4nicegui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 14:56:34.967589 ex4nicegui-0.1.2/ex4nicegui/layout/
--rw-rw-rw-   0        0        0       31 2023-07-05 06:10:00.000000 ex4nicegui-0.1.2/ex4nicegui/layout/__init__.py
--rw-rw-rw-   0        0        0     2378 2023-07-05 06:10:00.000000 ex4nicegui-0.1.2/ex4nicegui/layout/gridbox.py
-drwxrwxrwx   0        0        0        0 2023-07-09 14:56:34.982917 ex4nicegui-0.1.2/ex4nicegui/reactive/
--rw-rw-rw-   0        0        0     1023 2023-07-09 14:56:08.000000 ex4nicegui-0.1.2/ex4nicegui/reactive/__index.py
--rw-rw-rw-   0        0        0       24 2023-07-05 06:10:00.000000 ex4nicegui-0.1.2/ex4nicegui/reactive/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 14:56:34.988900 ex4nicegui-0.1.2/ex4nicegui/reactive/draggable/
--rw-rw-rw-   0        0        0     4851 2023-07-05 09:28:02.000000 ex4nicegui-0.1.2/ex4nicegui/reactive/draggable/UseDraggable.js
--rw-rw-rw-   0        0        0     3041 2023-07-08 17:55:18.000000 ex4nicegui-0.1.2/ex4nicegui/reactive/draggable/UseDraggable.py
--rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.2/ex4nicegui/reactive/draggable/__init__.py
--rw-rw-rw-   0        0        0     1320 2023-07-05 06:10:00.000000 ex4nicegui-0.1.2/ex4nicegui/reactive/drawer.py
-drwxrwxrwx   0        0        0        0 2023-07-09 14:56:34.997877 ex4nicegui-0.1.2/ex4nicegui/reactive/echarts/
--rw-rw-rw-   0        0        0  1581614 2023-07-05 06:10:00.000000 ex4nicegui-0.1.2/ex4nicegui/reactive/echarts/ECharts.js
--rw-rw-rw-   0        0        0     2685 2023-07-09 14:56:08.000000 ex4nicegui-0.1.2/ex4nicegui/reactive/echarts/ECharts.py
--rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.2/ex4nicegui/reactive/echarts/__init__.py
--rw-rw-rw-   0        0        0     6101 2023-07-09 14:56:08.000000 ex4nicegui-0.1.2/ex4nicegui/reactive/local_file_picker.py
--rw-rw-rw-   0        0        0     1041 2023-07-08 17:55:18.000000 ex4nicegui-0.1.2/ex4nicegui/reactive/official.py
--rw-rw-rw-   0        0        0    30044 2023-07-09 14:56:08.000000 ex4nicegui-0.1.2/ex4nicegui/reactive/ref.py
--rw-rw-rw-   0        0        0       24 2023-07-09 14:56:08.000000 ex4nicegui-0.1.2/ex4nicegui/reactive/rxui.py
--rw-rw-rw-   0        0        0      803 2023-07-05 06:10:00.000000 ex4nicegui-0.1.2/ex4nicegui/reactive/signature.py
-drwxrwxrwx   0        0        0        0 2023-07-09 14:56:35.002863 ex4nicegui-0.1.2/ex4nicegui/reactive/useMouse/
--rw-rw-rw-   0        0        0     2722 2023-07-08 17:55:18.000000 ex4nicegui-0.1.2/ex4nicegui/reactive/useMouse/UseMouse.js
--rw-rw-rw-   0        0        0     2244 2023-07-08 17:55:18.000000 ex4nicegui-0.1.2/ex4nicegui/reactive/useMouse/UseMouse.py
--rw-rw-rw-   0        0        0        0 2023-07-08 17:55:18.000000 ex4nicegui-0.1.2/ex4nicegui/reactive/useMouse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 14:56:35.005855 ex4nicegui-0.1.2/ex4nicegui/tools/
--rw-rw-rw-   0        0        0       40 2023-07-08 17:55:18.000000 ex4nicegui-0.1.2/ex4nicegui/tools/__init__.py
--rw-rw-rw-   0        0        0     5024 2023-07-08 17:55:18.000000 ex4nicegui-0.1.2/ex4nicegui/tools/debug.py
-drwxrwxrwx   0        0        0        0 2023-07-09 14:56:35.011839 ex4nicegui-0.1.2/ex4nicegui/utils/
--rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.2/ex4nicegui/utils/__init__.py
--rw-rw-rw-   0        0        0      430 2023-07-08 17:55:18.000000 ex4nicegui-0.1.2/ex4nicegui/utils/common.py
--rw-rw-rw-   0        0        0     4430 2023-07-09 14:56:08.000000 ex4nicegui-0.1.2/ex4nicegui/utils/signals.py
--rw-rw-rw-   0        0        0      910 2023-07-05 06:10:00.000000 ex4nicegui-0.1.2/ex4nicegui/utils/types.py
-drwxrwxrwx   0        0        0        0 2023-07-09 14:56:34.963531 ex4nicegui-0.1.2/ex4nicegui.egg-info/
--rw-rw-rw-   0        0        0      481 2023-07-09 14:56:34.000000 ex4nicegui-0.1.2/ex4nicegui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1104 2023-07-09 14:56:34.000000 ex4nicegui-0.1.2/ex4nicegui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 14:56:34.000000 ex4nicegui-0.1.2/ex4nicegui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-09 14:56:34.000000 ex4nicegui-0.1.2/ex4nicegui.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       32 2023-07-09 14:56:34.000000 ex4nicegui-0.1.2/ex4nicegui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-09 14:56:34.000000 ex4nicegui-0.1.2/ex4nicegui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-09 14:56:35.024792 ex4nicegui-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     2073 2023-07-09 14:56:08.000000 ex4nicegui-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:21:01.030755 ex4nicegui-0.1.3/
+-rw-rw-rw-   0        0        0     1094 2023-06-30 08:17:10.000000 ex4nicegui-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      481 2023-07-09 18:21:01.029730 ex4nicegui-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2023-07-05 06:11:55.000000 ex4nicegui-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 18:21:00.944546 ex4nicegui-0.1.3/ex4nicegui/
+-rw-rw-rw-   0        0        0      366 2023-07-09 18:20:51.000000 ex4nicegui-0.1.3/ex4nicegui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:21:00.961485 ex4nicegui-0.1.3/ex4nicegui/layout/
+-rw-rw-rw-   0        0        0       31 2023-07-05 06:10:00.000000 ex4nicegui-0.1.3/ex4nicegui/layout/__init__.py
+-rw-rw-rw-   0        0        0     2378 2023-07-05 06:10:00.000000 ex4nicegui-0.1.3/ex4nicegui/layout/gridbox.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:21:00.991978 ex4nicegui-0.1.3/ex4nicegui/reactive/
+-rw-rw-rw-   0        0        0     1023 2023-07-09 14:56:08.000000 ex4nicegui-0.1.3/ex4nicegui/reactive/__index.py
+-rw-rw-rw-   0        0        0       24 2023-07-05 06:10:00.000000 ex4nicegui-0.1.3/ex4nicegui/reactive/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:21:00.997961 ex4nicegui-0.1.3/ex4nicegui/reactive/draggable/
+-rw-rw-rw-   0        0        0     4851 2023-07-05 09:28:02.000000 ex4nicegui-0.1.3/ex4nicegui/reactive/draggable/UseDraggable.js
+-rw-rw-rw-   0        0        0     3041 2023-07-08 17:55:18.000000 ex4nicegui-0.1.3/ex4nicegui/reactive/draggable/UseDraggable.py
+-rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.3/ex4nicegui/reactive/draggable/__init__.py
+-rw-rw-rw-   0        0        0     1320 2023-07-05 06:10:00.000000 ex4nicegui-0.1.3/ex4nicegui/reactive/drawer.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:21:01.010777 ex4nicegui-0.1.3/ex4nicegui/reactive/echarts/
+-rw-rw-rw-   0        0        0  1581614 2023-07-05 06:10:00.000000 ex4nicegui-0.1.3/ex4nicegui/reactive/echarts/ECharts.js
+-rw-rw-rw-   0        0        0     2685 2023-07-09 14:56:08.000000 ex4nicegui-0.1.3/ex4nicegui/reactive/echarts/ECharts.py
+-rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.3/ex4nicegui/reactive/echarts/__init__.py
+-rw-rw-rw-   0        0        0     6101 2023-07-09 14:56:08.000000 ex4nicegui-0.1.3/ex4nicegui/reactive/local_file_picker.py
+-rw-rw-rw-   0        0        0     1041 2023-07-08 17:55:18.000000 ex4nicegui-0.1.3/ex4nicegui/reactive/official.py
+-rw-rw-rw-   0        0        0    30066 2023-07-09 18:20:32.000000 ex4nicegui-0.1.3/ex4nicegui/reactive/ref.py
+-rw-rw-rw-   0        0        0       24 2023-07-09 14:56:08.000000 ex4nicegui-0.1.3/ex4nicegui/reactive/rxui.py
+-rw-rw-rw-   0        0        0      803 2023-07-05 06:10:00.000000 ex4nicegui-0.1.3/ex4nicegui/reactive/signature.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:21:01.015766 ex4nicegui-0.1.3/ex4nicegui/reactive/useMouse/
+-rw-rw-rw-   0        0        0     2722 2023-07-08 17:55:18.000000 ex4nicegui-0.1.3/ex4nicegui/reactive/useMouse/UseMouse.js
+-rw-rw-rw-   0        0        0     2244 2023-07-08 17:55:18.000000 ex4nicegui-0.1.3/ex4nicegui/reactive/useMouse/UseMouse.py
+-rw-rw-rw-   0        0        0        0 2023-07-08 17:55:18.000000 ex4nicegui-0.1.3/ex4nicegui/reactive/useMouse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:21:01.019755 ex4nicegui-0.1.3/ex4nicegui/tools/
+-rw-rw-rw-   0        0        0       40 2023-07-08 17:55:18.000000 ex4nicegui-0.1.3/ex4nicegui/tools/__init__.py
+-rw-rw-rw-   0        0        0     5024 2023-07-08 17:55:18.000000 ex4nicegui-0.1.3/ex4nicegui/tools/debug.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:21:01.027737 ex4nicegui-0.1.3/ex4nicegui/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.3/ex4nicegui/utils/__init__.py
+-rw-rw-rw-   0        0        0      430 2023-07-08 17:55:18.000000 ex4nicegui-0.1.3/ex4nicegui/utils/common.py
+-rw-rw-rw-   0        0        0     4430 2023-07-09 14:56:08.000000 ex4nicegui-0.1.3/ex4nicegui/utils/signals.py
+-rw-rw-rw-   0        0        0      910 2023-07-05 06:10:00.000000 ex4nicegui-0.1.3/ex4nicegui/utils/types.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:21:00.957503 ex4nicegui-0.1.3/ex4nicegui.egg-info/
+-rw-rw-rw-   0        0        0      481 2023-07-09 18:21:00.000000 ex4nicegui-0.1.3/ex4nicegui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1104 2023-07-09 18:21:00.000000 ex4nicegui-0.1.3/ex4nicegui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 18:21:00.000000 ex4nicegui-0.1.3/ex4nicegui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-09 18:21:00.000000 ex4nicegui-0.1.3/ex4nicegui.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       32 2023-07-09 18:21:00.000000 ex4nicegui-0.1.3/ex4nicegui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-09 18:21:00.000000 ex4nicegui-0.1.3/ex4nicegui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-09 18:21:01.031752 ex4nicegui-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     2073 2023-07-09 14:56:08.000000 ex4nicegui-0.1.3/setup.py
```

### Comparing `ex4nicegui-0.1.2/LICENSE` & `ex4nicegui-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.2/ex4nicegui/layout/gridbox.py` & `ex4nicegui-0.1.3/ex4nicegui/layout/gridbox.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.2/ex4nicegui/reactive/__index.py` & `ex4nicegui-0.1.3/ex4nicegui/reactive/__index.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.2/ex4nicegui/reactive/draggable/UseDraggable.js` & `ex4nicegui-0.1.3/ex4nicegui/reactive/draggable/UseDraggable.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.2/ex4nicegui/reactive/draggable/UseDraggable.py` & `ex4nicegui-0.1.3/ex4nicegui/reactive/draggable/UseDraggable.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.2/ex4nicegui/reactive/drawer.py` & `ex4nicegui-0.1.3/ex4nicegui/reactive/drawer.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.2/ex4nicegui/reactive/echarts/ECharts.js` & `ex4nicegui-0.1.3/ex4nicegui/reactive/echarts/ECharts.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.2/ex4nicegui/reactive/echarts/ECharts.py` & `ex4nicegui-0.1.3/ex4nicegui/reactive/echarts/ECharts.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.2/ex4nicegui/reactive/local_file_picker.py` & `ex4nicegui-0.1.3/ex4nicegui/reactive/local_file_picker.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.2/ex4nicegui/reactive/official.py` & `ex4nicegui-0.1.3/ex4nicegui/reactive/official.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.2/ex4nicegui/reactive/ref.py` & `ex4nicegui-0.1.3/ex4nicegui/reactive/ref.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
         def _():
             binder.element.value = binder.value
 
         binder.element.on("update:modelValue", handler=onValueChanged)
 
     def __init__(
         self,
-        options: TMaybeRef[Union[List, Dict]],
+        options: Union[TMaybeRef[List], TMaybeRef[Dict]],
         *,
         label: TMaybeRef[Optional[str]] = None,
         value: TMaybeRef[Any] = None,
         on_change: Optional[Callable[..., Any]] = None,
         with_input: TMaybeRef[bool] = False,
         multiple: TMaybeRef[bool] = False,
         clearable: TMaybeRef[bool] = False,
@@ -217,15 +217,15 @@
         def _():
             binder.element.value = binder.value
 
         binder.element.on("update:modelValue", handler=onValueChanged)
 
     def __init__(
         self,
-        options: TMaybeRef[Union[List, Dict]],
+        options: Union[TMaybeRef[List], TMaybeRef[Dict]],
         *,
         value: TMaybeRef[Any] = None,
         on_change: Optional[Callable[..., Any]] = None,
     ) -> None:
         kws = {"options": options, "value": value, "on_change": on_change}
 
         value_kws = _convert_kws_ref2value(kws)
```

### Comparing `ex4nicegui-0.1.2/ex4nicegui/reactive/signature.py` & `ex4nicegui-0.1.3/ex4nicegui/reactive/signature.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.2/ex4nicegui/reactive/useMouse/UseMouse.js` & `ex4nicegui-0.1.3/ex4nicegui/reactive/useMouse/UseMouse.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.2/ex4nicegui/reactive/useMouse/UseMouse.py` & `ex4nicegui-0.1.3/ex4nicegui/reactive/useMouse/UseMouse.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.2/ex4nicegui/tools/debug.py` & `ex4nicegui-0.1.3/ex4nicegui/tools/debug.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.2/ex4nicegui/utils/signals.py` & `ex4nicegui-0.1.3/ex4nicegui/utils/signals.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.2/ex4nicegui/utils/types.py` & `ex4nicegui-0.1.3/ex4nicegui/utils/types.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.2/ex4nicegui.egg-info/SOURCES.txt` & `ex4nicegui-0.1.3/ex4nicegui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.2/setup.py` & `ex4nicegui-0.1.3/setup.py`

 * *Files identical despite different names*

