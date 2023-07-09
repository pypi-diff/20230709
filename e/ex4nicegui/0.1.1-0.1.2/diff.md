# Comparing `tmp/ex4nicegui-0.1.1.tar.gz` & `tmp/ex4nicegui-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ex4nicegui-0.1.1.tar", last modified: Sat Jul  8 17:56:04 2023, max compression
+gzip compressed data, was "ex4nicegui-0.1.2.tar", last modified: Sun Jul  9 14:56:35 2023, max compression
```

## Comparing `ex4nicegui-0.1.1.tar` & `ex4nicegui-0.1.2.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 17:56:04.549298 ex4nicegui-0.1.1/
--rw-rw-rw-   0        0        0     1094 2023-06-30 08:17:10.000000 ex4nicegui-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      481 2023-07-08 17:56:04.535102 ex4nicegui-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       12 2023-07-05 06:11:55.000000 ex4nicegui-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-08 17:56:04.447999 ex4nicegui-0.1.1/ex4nicegui/
--rw-rw-rw-   0        0        0      366 2023-07-08 17:55:31.000000 ex4nicegui-0.1.1/ex4nicegui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-08 17:56:04.462315 ex4nicegui-0.1.1/ex4nicegui/layout/
--rw-rw-rw-   0        0        0       31 2023-07-05 06:10:00.000000 ex4nicegui-0.1.1/ex4nicegui/layout/__init__.py
--rw-rw-rw-   0        0        0     2378 2023-07-05 06:10:00.000000 ex4nicegui-0.1.1/ex4nicegui/layout/gridbox.py
-drwxrwxrwx   0        0        0        0 2023-07-08 17:56:04.474210 ex4nicegui-0.1.1/ex4nicegui/reactive/
--rw-rw-rw-   0        0        0      829 2023-07-08 17:55:18.000000 ex4nicegui-0.1.1/ex4nicegui/reactive/__index.py
--rw-rw-rw-   0        0        0       24 2023-07-05 06:10:00.000000 ex4nicegui-0.1.1/ex4nicegui/reactive/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-08 17:56:04.478167 ex4nicegui-0.1.1/ex4nicegui/reactive/draggable/
--rw-rw-rw-   0        0        0     4851 2023-07-05 09:28:02.000000 ex4nicegui-0.1.1/ex4nicegui/reactive/draggable/UseDraggable.js
--rw-rw-rw-   0        0        0     3041 2023-07-08 17:55:18.000000 ex4nicegui-0.1.1/ex4nicegui/reactive/draggable/UseDraggable.py
--rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.1/ex4nicegui/reactive/draggable/__init__.py
--rw-rw-rw-   0        0        0     1320 2023-07-05 06:10:00.000000 ex4nicegui-0.1.1/ex4nicegui/reactive/drawer.py
-drwxrwxrwx   0        0        0        0 2023-07-08 17:56:04.521402 ex4nicegui-0.1.1/ex4nicegui/reactive/echarts/
--rw-rw-rw-   0        0        0  1581614 2023-07-05 06:10:00.000000 ex4nicegui-0.1.1/ex4nicegui/reactive/echarts/ECharts.js
--rw-rw-rw-   0        0        0     2709 2023-07-05 06:10:00.000000 ex4nicegui-0.1.1/ex4nicegui/reactive/echarts/ECharts.py
--rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.1/ex4nicegui/reactive/echarts/__init__.py
--rw-rw-rw-   0        0        0     6100 2023-07-08 17:55:18.000000 ex4nicegui-0.1.1/ex4nicegui/reactive/local_file_picker.py
--rw-rw-rw-   0        0        0     1041 2023-07-08 17:55:18.000000 ex4nicegui-0.1.1/ex4nicegui/reactive/official.py
--rw-rw-rw-   0        0        0    25676 2023-07-08 17:55:18.000000 ex4nicegui-0.1.1/ex4nicegui/reactive/ref.py
--rw-rw-rw-   0        0        0      803 2023-07-05 06:10:00.000000 ex4nicegui-0.1.1/ex4nicegui/reactive/signature.py
-drwxrwxrwx   0        0        0        0 2023-07-08 17:56:04.524100 ex4nicegui-0.1.1/ex4nicegui/reactive/useMouse/
--rw-rw-rw-   0        0        0     2244 2023-07-08 17:55:18.000000 ex4nicegui-0.1.1/ex4nicegui/reactive/useMouse/UseMouse.py
--rw-rw-rw-   0        0        0        0 2023-07-08 17:55:18.000000 ex4nicegui-0.1.1/ex4nicegui/reactive/useMouse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-08 17:56:04.527096 ex4nicegui-0.1.1/ex4nicegui/tools/
--rw-rw-rw-   0        0        0       40 2023-07-08 17:55:18.000000 ex4nicegui-0.1.1/ex4nicegui/tools/__init__.py
--rw-rw-rw-   0        0        0     5024 2023-07-08 17:55:18.000000 ex4nicegui-0.1.1/ex4nicegui/tools/debug.py
-drwxrwxrwx   0        0        0        0 2023-07-08 17:56:04.533080 ex4nicegui-0.1.1/ex4nicegui/utils/
--rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.1/ex4nicegui/utils/__init__.py
--rw-rw-rw-   0        0        0      430 2023-07-08 17:55:18.000000 ex4nicegui-0.1.1/ex4nicegui/utils/common.py
--rw-rw-rw-   0        0        0     4404 2023-07-08 17:55:18.000000 ex4nicegui-0.1.1/ex4nicegui/utils/signals.py
--rw-rw-rw-   0        0        0      910 2023-07-05 06:10:00.000000 ex4nicegui-0.1.1/ex4nicegui/utils/types.py
-drwxrwxrwx   0        0        0        0 2023-07-08 17:56:04.459321 ex4nicegui-0.1.1/ex4nicegui.egg-info/
--rw-rw-rw-   0        0        0      481 2023-07-08 17:56:04.000000 ex4nicegui-0.1.1/ex4nicegui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1035 2023-07-08 17:56:04.000000 ex4nicegui-0.1.1/ex4nicegui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 17:56:04.000000 ex4nicegui-0.1.1/ex4nicegui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-08 17:56:04.000000 ex4nicegui-0.1.1/ex4nicegui.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       32 2023-07-08 17:56:04.000000 ex4nicegui-0.1.1/ex4nicegui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-08 17:56:04.000000 ex4nicegui-0.1.1/ex4nicegui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-08 17:56:04.549298 ex4nicegui-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1533 2023-07-05 06:10:00.000000 ex4nicegui-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 14:56:35.024792 ex4nicegui-0.1.2/
+-rw-rw-rw-   0        0        0     1094 2023-06-30 08:17:10.000000 ex4nicegui-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      481 2023-07-09 14:56:35.013834 ex4nicegui-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2023-07-05 06:11:55.000000 ex4nicegui-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 14:56:34.953557 ex4nicegui-0.1.2/ex4nicegui/
+-rw-rw-rw-   0        0        0      366 2023-07-09 14:56:18.000000 ex4nicegui-0.1.2/ex4nicegui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 14:56:34.967589 ex4nicegui-0.1.2/ex4nicegui/layout/
+-rw-rw-rw-   0        0        0       31 2023-07-05 06:10:00.000000 ex4nicegui-0.1.2/ex4nicegui/layout/__init__.py
+-rw-rw-rw-   0        0        0     2378 2023-07-05 06:10:00.000000 ex4nicegui-0.1.2/ex4nicegui/layout/gridbox.py
+drwxrwxrwx   0        0        0        0 2023-07-09 14:56:34.982917 ex4nicegui-0.1.2/ex4nicegui/reactive/
+-rw-rw-rw-   0        0        0     1023 2023-07-09 14:56:08.000000 ex4nicegui-0.1.2/ex4nicegui/reactive/__index.py
+-rw-rw-rw-   0        0        0       24 2023-07-05 06:10:00.000000 ex4nicegui-0.1.2/ex4nicegui/reactive/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 14:56:34.988900 ex4nicegui-0.1.2/ex4nicegui/reactive/draggable/
+-rw-rw-rw-   0        0        0     4851 2023-07-05 09:28:02.000000 ex4nicegui-0.1.2/ex4nicegui/reactive/draggable/UseDraggable.js
+-rw-rw-rw-   0        0        0     3041 2023-07-08 17:55:18.000000 ex4nicegui-0.1.2/ex4nicegui/reactive/draggable/UseDraggable.py
+-rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.2/ex4nicegui/reactive/draggable/__init__.py
+-rw-rw-rw-   0        0        0     1320 2023-07-05 06:10:00.000000 ex4nicegui-0.1.2/ex4nicegui/reactive/drawer.py
+drwxrwxrwx   0        0        0        0 2023-07-09 14:56:34.997877 ex4nicegui-0.1.2/ex4nicegui/reactive/echarts/
+-rw-rw-rw-   0        0        0  1581614 2023-07-05 06:10:00.000000 ex4nicegui-0.1.2/ex4nicegui/reactive/echarts/ECharts.js
+-rw-rw-rw-   0        0        0     2685 2023-07-09 14:56:08.000000 ex4nicegui-0.1.2/ex4nicegui/reactive/echarts/ECharts.py
+-rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.2/ex4nicegui/reactive/echarts/__init__.py
+-rw-rw-rw-   0        0        0     6101 2023-07-09 14:56:08.000000 ex4nicegui-0.1.2/ex4nicegui/reactive/local_file_picker.py
+-rw-rw-rw-   0        0        0     1041 2023-07-08 17:55:18.000000 ex4nicegui-0.1.2/ex4nicegui/reactive/official.py
+-rw-rw-rw-   0        0        0    30044 2023-07-09 14:56:08.000000 ex4nicegui-0.1.2/ex4nicegui/reactive/ref.py
+-rw-rw-rw-   0        0        0       24 2023-07-09 14:56:08.000000 ex4nicegui-0.1.2/ex4nicegui/reactive/rxui.py
+-rw-rw-rw-   0        0        0      803 2023-07-05 06:10:00.000000 ex4nicegui-0.1.2/ex4nicegui/reactive/signature.py
+drwxrwxrwx   0        0        0        0 2023-07-09 14:56:35.002863 ex4nicegui-0.1.2/ex4nicegui/reactive/useMouse/
+-rw-rw-rw-   0        0        0     2722 2023-07-08 17:55:18.000000 ex4nicegui-0.1.2/ex4nicegui/reactive/useMouse/UseMouse.js
+-rw-rw-rw-   0        0        0     2244 2023-07-08 17:55:18.000000 ex4nicegui-0.1.2/ex4nicegui/reactive/useMouse/UseMouse.py
+-rw-rw-rw-   0        0        0        0 2023-07-08 17:55:18.000000 ex4nicegui-0.1.2/ex4nicegui/reactive/useMouse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 14:56:35.005855 ex4nicegui-0.1.2/ex4nicegui/tools/
+-rw-rw-rw-   0        0        0       40 2023-07-08 17:55:18.000000 ex4nicegui-0.1.2/ex4nicegui/tools/__init__.py
+-rw-rw-rw-   0        0        0     5024 2023-07-08 17:55:18.000000 ex4nicegui-0.1.2/ex4nicegui/tools/debug.py
+drwxrwxrwx   0        0        0        0 2023-07-09 14:56:35.011839 ex4nicegui-0.1.2/ex4nicegui/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.2/ex4nicegui/utils/__init__.py
+-rw-rw-rw-   0        0        0      430 2023-07-08 17:55:18.000000 ex4nicegui-0.1.2/ex4nicegui/utils/common.py
+-rw-rw-rw-   0        0        0     4430 2023-07-09 14:56:08.000000 ex4nicegui-0.1.2/ex4nicegui/utils/signals.py
+-rw-rw-rw-   0        0        0      910 2023-07-05 06:10:00.000000 ex4nicegui-0.1.2/ex4nicegui/utils/types.py
+drwxrwxrwx   0        0        0        0 2023-07-09 14:56:34.963531 ex4nicegui-0.1.2/ex4nicegui.egg-info/
+-rw-rw-rw-   0        0        0      481 2023-07-09 14:56:34.000000 ex4nicegui-0.1.2/ex4nicegui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1104 2023-07-09 14:56:34.000000 ex4nicegui-0.1.2/ex4nicegui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 14:56:34.000000 ex4nicegui-0.1.2/ex4nicegui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-09 14:56:34.000000 ex4nicegui-0.1.2/ex4nicegui.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       32 2023-07-09 14:56:34.000000 ex4nicegui-0.1.2/ex4nicegui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-09 14:56:34.000000 ex4nicegui-0.1.2/ex4nicegui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-09 14:56:35.024792 ex4nicegui-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     2073 2023-07-09 14:56:08.000000 ex4nicegui-0.1.2/setup.py
```

### Comparing `ex4nicegui-0.1.1/LICENSE` & `ex4nicegui-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.1/ex4nicegui/layout/gridbox.py` & `ex4nicegui-0.1.2/ex4nicegui/layout/gridbox.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.1/ex4nicegui/reactive/draggable/UseDraggable.js` & `ex4nicegui-0.1.2/ex4nicegui/reactive/draggable/UseDraggable.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.1/ex4nicegui/reactive/draggable/UseDraggable.py` & `ex4nicegui-0.1.2/ex4nicegui/reactive/draggable/UseDraggable.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.1/ex4nicegui/reactive/drawer.py` & `ex4nicegui-0.1.2/ex4nicegui/reactive/drawer.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.1/ex4nicegui/reactive/echarts/ECharts.js` & `ex4nicegui-0.1.2/ex4nicegui/reactive/echarts/ECharts.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.1/ex4nicegui/reactive/echarts/ECharts.py` & `ex4nicegui-0.1.2/ex4nicegui/reactive/echarts/ECharts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Callable, Optional
 from dataclasses import dataclass
 from nicegui.helpers import KWONLY_SLOTS
 from nicegui.events import handle_event, EventArguments
 from nicegui.dependencies import register_component
 from nicegui.element import Element
-from pathlib import Path
+
 
 register_component("ECharts", __file__, "ECharts.js")
 
 _Chart_Click_Args = [
     "componentType",
     "seriesType",
     "seriesIndex",
```

### Comparing `ex4nicegui-0.1.1/ex4nicegui/reactive/local_file_picker.py` & `ex4nicegui-0.1.2/ex4nicegui/reactive/local_file_picker.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         _type_: open,result
             open:打开选择框函数
             result: 获取结果的信号函数。
 
     例子:
         ```python
 
-        fp = local_file_picker(dir=r"E:\dataset", ext=[".xlsx"])
+        fp = local_file_picker(dir=r"D://dataset", ext=[".xlsx"])
         fp.open()
 
         # 获取结果
         fp.value
         ```
     """
     # data define
```

### Comparing `ex4nicegui-0.1.1/ex4nicegui/reactive/official.py` & `ex4nicegui-0.1.2/ex4nicegui/reactive/official.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.1/ex4nicegui/reactive/ref.py` & `ex4nicegui-0.1.2/ex4nicegui/reactive/ref.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from nicegui.elements.mixins.value_element import ValueElement
 from nicegui.elements.mixins.color_elements import (
     TextColorElement,
     QUASAR_COLORS,
     TAILWIND_COLORS,
 )
 from nicegui.page_layout import Drawer
+from ex4nicegui.reactive.echarts.ECharts import echarts
 
 T = TypeVar("T")
 
 TWidget = TypeVar("TWidget")
 
 
 class BindableUi(Generic[TWidget]):
@@ -167,14 +168,15 @@
             "multiple": multiple,
             "clearable": clearable,
         }
 
         value_kws = _convert_kws_ref2value(kws)
 
         element = ui.select(**value_kws)
+        element.classes("min-w-[10rem]")
 
         super().__init__(value, element)
 
         for key, value in kws.items():
             if is_ref(value):
                 self.bind_prop(key, value)
 
@@ -769,14 +771,37 @@
         @effect
         def _():
             self._element_picker._props["value"] = ref_ui.value
 
         return self
 
 
+class ColorPickerLazyBindableUi(ColorPickerBindableUi):
+    def __init__(
+        self,
+        color: TMaybeRef[str] = "",
+        *,
+        on_pick: Callable[..., Any] | None = None,
+        value: TMaybeRef[bool] = False,
+    ) -> None:
+        super().__init__(color, on_pick=on_pick, value=value)
+
+    def _ex_setup(self):
+        ele = self._element_picker
+
+        # @effect
+        # def _():
+        #     ele._props["modelValue"] = self.value
+
+        def onModelValueChanged(args):
+            self._ref.value = args["args"]  # type: ignore
+
+        ele.on("change", handler=onModelValueChanged)
+
+
 _TAggridValue = Dict
 
 
 class AggridBindableUi(SingleValueBindableUi[_TAggridValue, ui.aggrid]):
     def __init__(self, value: _TAggridValue, element: ui.aggrid) -> None:
         super().__init__(value, element)
 
@@ -846,17 +871,41 @@
         super().__init__(element)
 
         for key, value in kws.items():
             if is_ref(value):
                 self.bind_prop(key, value)  # type: ignore
 
     @staticmethod
-    def from_pandas(df):
+    def from_pandas(df: TMaybeRef):
+        if is_ref(df):
+
+            @ref_computed
+            def cp_convert_df():
+                return utils_common.convert_dataframe(df.value)
+
+            @ref_computed
+            def cp_rows():
+                return cp_convert_df.value.to_dict("records")
+
+            @ref_computed
+            def cp_cols():
+                return [
+                    {
+                        "name": col,
+                        "label": col,
+                        "field": col,
+                    }
+                    for col in cp_convert_df.value.columns
+                ]
+
+            return TableBindableUi(cp_cols, cp_rows)
+
         df = utils_common.convert_dataframe(df)
         rows = df.to_dict("records")
+
         cols = [
             {
                 "name": col,
                 "label": col,
                 "field": col,
             }
             for col in df.columns
@@ -925,7 +974,134 @@
 
     def __enter__(self):
         self.element.__enter__()
         return self
 
     def __exit__(self, *_: Any):
         self.element.__exit__(*_)
+
+
+class EChartsBindableUi(BindableUi[echarts]):
+    def __init__(
+        self,
+        options: TMaybeRef[Dict],
+    ) -> None:
+        kws = {
+            "options": options,
+        }
+
+        value_kws = _convert_kws_ref2value(kws)
+
+        element = echarts(**value_kws)
+
+        super().__init__(element)
+
+        for key, value in kws.items():
+            if is_ref(value):
+                self.bind_prop(key, value)  # type: ignore
+
+    @staticmethod
+    def _pyecharts2opts(chart):
+        import simplejson as json
+        from pyecharts.charts.chart import Base
+
+        if isinstance(chart, Base):
+            return json.loads(chart.dump_options())
+
+        return {}
+
+    @staticmethod
+    def from_pyecharts(chart: TMaybeRef):
+        if is_ref(chart):
+
+            @ref_computed
+            def chart_opt():
+                return EChartsBindableUi._pyecharts2opts(chart.value)
+
+            return EChartsBindableUi(chart_opt)
+
+        return EChartsBindableUi(EChartsBindableUi._pyecharts2opts(chart))
+
+    def bind_prop(self, prop: str, ref_ui: ReadonlyRef):
+        if prop == "options":
+            return self.bind_options(ref_ui)
+
+        return super().bind_prop(prop, ref_ui)
+
+    def bind_options(self, ref_ui: ReadonlyRef[Dict]):
+        @effect
+        def _():
+            ele = self.element
+            ele.update_options(ref_ui.value)
+            ele.update()
+
+        return self
+
+
+class RowBindableUi(BindableUi[ui.row]):
+    def __init__(
+        self,
+    ) -> None:
+        element = ui.row()
+
+        super().__init__(element)
+
+    def __enter__(self):
+        self.element.__enter__()
+        return self
+
+    def __exit__(self, *_: Any):
+        self.element.__exit__(*_)
+
+
+class CardBindableUi(BindableUi[ui.card]):
+    def __init__(
+        self,
+    ) -> None:
+        element = ui.card()
+
+        super().__init__(element)
+
+    def __enter__(self):
+        self.element.__enter__()
+        return self
+
+    def __exit__(self, *_: Any):
+        self.element.__exit__(*_)
+
+    def tight(self):
+        """Removes padding and gaps between nested elements."""
+        self.element._classes.clear()
+        self.element._style.clear()
+        return self
+
+
+class CardSectionBindableUi(BindableUi[ui.card_section]):
+    def __init__(
+        self,
+    ) -> None:
+        element = ui.card_section()
+
+        super().__init__(element)
+
+    def __enter__(self):
+        self.element.__enter__()
+        return self
+
+    def __exit__(self, *_: Any):
+        self.element.__exit__(*_)
+
+
+class CardActionsBindableUi(BindableUi[ui.card_actions]):
+    def __init__(
+        self,
+    ) -> None:
+        element = ui.card_actions()
+
+        super().__init__(element)
+
+    def __enter__(self):
+        self.element.__enter__()
+        return self
+
+    def __exit__(self, *_: Any):
+        self.element.__exit__(*_)
```

### Comparing `ex4nicegui-0.1.1/ex4nicegui/reactive/signature.py` & `ex4nicegui-0.1.2/ex4nicegui/reactive/signature.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.1/ex4nicegui/reactive/useMouse/UseMouse.py` & `ex4nicegui-0.1.2/ex4nicegui/reactive/useMouse/UseMouse.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.1/ex4nicegui/tools/debug.py` & `ex4nicegui-0.1.2/ex4nicegui/tools/debug.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.1/ex4nicegui/utils/signals.py` & `ex4nicegui-0.1.2/ex4nicegui/utils/signals.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     fn: Callable[[], T],
     desc="",
     *,
     debug_trigger: Optional[Callable[..., None]] = None,
     priority_level: int = 1,
 ) -> ReadonlyRef[T]:
     getter = computed(fn, debug_trigger, priority_level)
-    return DescReadonlyRef(getter, desc)
+    return cast(DescReadonlyRef[T], DescReadonlyRef(getter, desc))
 
 
 def ref_computed_with_opts(
     desc="",
     debug_trigger: Optional[Callable[..., None]] = None,
     priority_level: int = 1,
 ):
```

### Comparing `ex4nicegui-0.1.1/ex4nicegui/utils/types.py` & `ex4nicegui-0.1.2/ex4nicegui/utils/types.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.1/ex4nicegui.egg-info/SOURCES.txt` & `ex4nicegui-0.1.2/ex4nicegui.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,21 +12,23 @@
 ex4nicegui/layout/gridbox.py
 ex4nicegui/reactive/__index.py
 ex4nicegui/reactive/__init__.py
 ex4nicegui/reactive/drawer.py
 ex4nicegui/reactive/local_file_picker.py
 ex4nicegui/reactive/official.py
 ex4nicegui/reactive/ref.py
+ex4nicegui/reactive/rxui.py
 ex4nicegui/reactive/signature.py
 ex4nicegui/reactive/draggable/UseDraggable.js
 ex4nicegui/reactive/draggable/UseDraggable.py
 ex4nicegui/reactive/draggable/__init__.py
 ex4nicegui/reactive/echarts/ECharts.js
 ex4nicegui/reactive/echarts/ECharts.py
 ex4nicegui/reactive/echarts/__init__.py
+ex4nicegui/reactive/useMouse/UseMouse.js
 ex4nicegui/reactive/useMouse/UseMouse.py
 ex4nicegui/reactive/useMouse/__init__.py
 ex4nicegui/tools/__init__.py
 ex4nicegui/tools/debug.py
 ex4nicegui/utils/__init__.py
 ex4nicegui/utils/common.py
 ex4nicegui/utils/signals.py
```

### Comparing `ex4nicegui-0.1.1/setup.py` & `ex4nicegui-0.1.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,27 @@
 #!/usr/bin/env python
 """The setup script."""
 
+from pathlib import Path
 from setuptools import setup, find_packages
 import ex4nicegui
 
 
+def get_data_files(base):
+    base = Path(base)
+
+    all_js_files = base.rglob("*.js")
+
+    all_infos = ({"dir": js.parent.name, "js": str(js)} for js in all_js_files)
+
+    all_infos = ((info["dir"], [info["js"]]) for info in all_infos)
+
+    return list(all_infos)
+
+
 with open("README.md", encoding="utf8") as readme_file:
     readme = readme_file.read()
 
 requirements = ["signe", "nicegui", "typing_extensions"]
 
 test_requirements = ["pytest>=3"]
 
@@ -32,27 +45,34 @@
     install_requires=requirements,
     license="MIT license",
     # long_description=readme,
     include_package_data=True,
     keywords=["nicegui", "ex4nicegui", "webui"],
     name="ex4nicegui",
     packages=find_packages(include=["ex4nicegui", "ex4nicegui.*"]),
-    data_files=[
-        (
-            "echarts",
-            [
-                "ex4nicegui/reactive/echarts/ECharts.js",
-            ],
-        ),
-        (
-            "draggable",
-            [
-                "ex4nicegui/reactive/draggable/UseDraggable.js",
-            ],
-        ),
-    ],
+    data_files=get_data_files("ex4nicegui/reactive"),
+    # data_files=[
+    #     (
+    #         "echarts",
+    #         [
+    #             "ex4nicegui/reactive/echarts/ECharts.js",
+    #         ],
+    #     ),
+    #     (
+    #         "draggable",
+    #         [
+    #             "ex4nicegui/reactive/draggable/UseDraggable.js",
+    #         ],
+    #     ),
+    #     (
+    #         "useMouse",
+    #         [
+    #             "ex4nicegui/reactive/useMouse/UseMouse.js",
+    #         ],
+    #     ),
+    # ],
     test_suite="__tests",
     tests_require=test_requirements,
     url="",
     version=ex4nicegui.__version__,
     zip_safe=False,
 )
```

