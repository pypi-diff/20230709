# Comparing `tmp/simplekivy-0.0.2.tar.gz` & `tmp/simplekivy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplekivy-0.0.2.tar", last modified: Sat Jul  8 19:37:33 2023, max compression
+gzip compressed data, was "simplekivy-0.0.3.tar", last modified: Sun Jul  9 14:13:05 2023, max compression
```

## Comparing `simplekivy-0.0.2.tar` & `simplekivy-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-07-08 19:37:33.885800 simplekivy-0.0.2/
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     1057 2023-06-26 12:44:34.000000 simplekivy-0.0.2/LICENSE
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     4012 2023-07-08 19:37:33.885800 simplekivy-0.0.2/PKG-INFO
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     3460 2023-07-08 19:35:07.000000 simplekivy-0.0.2/README.md
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      693 2023-07-06 16:21:28.000000 simplekivy-0.0.2/pyproject.toml
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       38 2023-07-08 19:37:33.885800 simplekivy-0.0.2/setup.cfg
-drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-07-08 19:37:33.885800 simplekivy-0.0.2/simplekivy/
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       35 2023-06-26 13:46:46.000000 simplekivy-0.0.2/simplekivy/__init__.py
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      786 2023-07-06 16:35:37.000000 simplekivy-0.0.2/simplekivy/simplekivy.py
-drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-07-08 19:37:33.885800 simplekivy-0.0.2/simplekivy/widgets/
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       25 2023-06-25 14:58:13.000000 simplekivy-0.0.2/simplekivy/widgets/__init__.py
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     1649 2023-07-04 14:57:24.000000 simplekivy-0.0.2/simplekivy/widgets/app.py
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      443 2023-07-03 11:21:37.000000 simplekivy-0.0.2/simplekivy/widgets/main.kv
-drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-07-08 19:37:33.885800 simplekivy-0.0.2/simplekivy.egg-info/
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     4012 2023-07-08 19:37:33.000000 simplekivy-0.0.2/simplekivy.egg-info/PKG-INFO
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      300 2023-07-08 19:37:33.000000 simplekivy-0.0.2/simplekivy.egg-info/SOURCES.txt
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)        1 2023-07-08 19:37:33.000000 simplekivy-0.0.2/simplekivy.egg-info/dependency_links.txt
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       11 2023-07-08 19:37:33.000000 simplekivy-0.0.2/simplekivy.egg-info/top_level.txt
+drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-07-09 14:13:05.498063 simplekivy-0.0.3/
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     1057 2023-06-26 12:44:34.000000 simplekivy-0.0.3/LICENSE
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     4044 2023-07-09 14:13:05.494063 simplekivy-0.0.3/PKG-INFO
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     3492 2023-07-08 23:37:27.000000 simplekivy-0.0.3/README.md
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      693 2023-07-08 23:32:00.000000 simplekivy-0.0.3/pyproject.toml
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       38 2023-07-09 14:13:05.498063 simplekivy-0.0.3/setup.cfg
+drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-07-09 14:13:05.494063 simplekivy-0.0.3/simplekivy/
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       35 2023-06-26 13:46:46.000000 simplekivy-0.0.3/simplekivy/__init__.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      786 2023-07-06 16:35:37.000000 simplekivy-0.0.3/simplekivy/simplekivy.py
+drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-07-09 14:13:05.494063 simplekivy-0.0.3/simplekivy/widgets/
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       25 2023-06-25 14:58:13.000000 simplekivy-0.0.3/simplekivy/widgets/__init__.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     1763 2023-07-09 14:06:29.000000 simplekivy-0.0.3/simplekivy/widgets/app.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      443 2023-07-03 11:21:37.000000 simplekivy-0.0.3/simplekivy/widgets/main.kv
+drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-07-09 14:13:05.494063 simplekivy-0.0.3/simplekivy.egg-info/
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     4044 2023-07-09 14:13:05.000000 simplekivy-0.0.3/simplekivy.egg-info/PKG-INFO
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      300 2023-07-09 14:13:05.000000 simplekivy-0.0.3/simplekivy.egg-info/SOURCES.txt
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)        1 2023-07-09 14:13:05.000000 simplekivy-0.0.3/simplekivy.egg-info/dependency_links.txt
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       11 2023-07-09 14:13:05.000000 simplekivy-0.0.3/simplekivy.egg-info/top_level.txt
```

### Comparing `simplekivy-0.0.2/LICENSE` & `simplekivy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `simplekivy-0.0.2/PKG-INFO` & `simplekivy-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplekivy
-Version: 0.0.2
+Version: 0.0.3
 Summary: the idea is inspired by PySimpleGui , to quickly create simple kivy apps 
 Author-email: yousuf <yosefmahmoud356@gmail.com>
 Project-URL: Homepage, https://github.com/yousuf60/SimpleKivy
 Project-URL: Bug Tracker, https://github.com/yousuf60/SimpleKivy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -113,15 +113,15 @@
 
 you can also add kvlang string directly instead of using 
 `s.lang.Builder`
 or `kivy.lang.Builder`
 
 ```python
 from simplekivy import SimpleKivy
-s = SimpleKivy(title="test app")
+s = SimpleKivy(title="test app", make_app=True)
 
 def on_enter(instance):
     print(instance.text)
     
 def btn_pressed():
     print(ainput.text)
 
@@ -129,34 +129,35 @@
 #add a new method to app
 s.myapp.btn_pressed = btn_pressed
 
 KV_BTN = """
 
 Button:
     text: "press me"
-    size_hint:.4, .1
-    pos_hint: {"center_x": .5}
+    size_hint:.4, .2
+    pos_hint: {"center_x": .5, "center_y": .5}
     on_press:app.btn_pressed()
 """
 ainput = s.TextInput(hint_text="type anything", multiline=False,  size_hint=(1, None),
      height="50dp", pos_hint={"center_x":.5, "center_y":.7})
 
 ainput.bind(on_text_validate=on_enter)
 
 s + [
-    [{"orientation":"vertical", "size_hint":(1, .4)},
+    [{"orientation":"vertical", "size_hint":(1, .2)},
     s.Label(text="hello world", halign="center"),
     s.Label(text="testo")],
     ({"size_hint":(.4, .4), "pos_hint":{"center_x":.5}},
         ainput 
     ),
-    ({"size_hint": (1, .2)},
+    ({"size_hint": (1, .4)},
         KV_BTN),
 ]
 
+
 ```
 
 <img src="https://github.com/yousuf60/SimpleKivy/assets/64571068/9e9e445e-0c6f-45de-9580-cd7fbde1f010" width="500">
 
 ### Hints
 ------
```

### Comparing `simplekivy-0.0.2/README.md` & `simplekivy-0.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
 you can also add kvlang string directly instead of using 
 `s.lang.Builder`
 or `kivy.lang.Builder`
 
 ```python
 from simplekivy import SimpleKivy
-s = SimpleKivy(title="test app")
+s = SimpleKivy(title="test app", make_app=True)
 
 def on_enter(instance):
     print(instance.text)
     
 def btn_pressed():
     print(ainput.text)
 
@@ -115,34 +115,35 @@
 #add a new method to app
 s.myapp.btn_pressed = btn_pressed
 
 KV_BTN = """
 
 Button:
     text: "press me"
-    size_hint:.4, .1
-    pos_hint: {"center_x": .5}
+    size_hint:.4, .2
+    pos_hint: {"center_x": .5, "center_y": .5}
     on_press:app.btn_pressed()
 """
 ainput = s.TextInput(hint_text="type anything", multiline=False,  size_hint=(1, None),
      height="50dp", pos_hint={"center_x":.5, "center_y":.7})
 
 ainput.bind(on_text_validate=on_enter)
 
 s + [
-    [{"orientation":"vertical", "size_hint":(1, .4)},
+    [{"orientation":"vertical", "size_hint":(1, .2)},
     s.Label(text="hello world", halign="center"),
     s.Label(text="testo")],
     ({"size_hint":(.4, .4), "pos_hint":{"center_x":.5}},
         ainput 
     ),
-    ({"size_hint": (1, .2)},
+    ({"size_hint": (1, .4)},
         KV_BTN),
 ]
 
+
 ```
 
 <img src="https://github.com/yousuf60/SimpleKivy/assets/64571068/9e9e445e-0c6f-45de-9580-cd7fbde1f010" width="500">
 
 ### Hints
 ------
```

### Comparing `simplekivy-0.0.2/pyproject.toml` & `simplekivy-0.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "simplekivy"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="yousuf", email="yosefmahmoud356@gmail.com" },
 ]
 description = "the idea is inspired by PySimpleGui , to quickly create simple kivy apps "
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `simplekivy-0.0.2/simplekivy/simplekivy.py` & `simplekivy-0.0.3/simplekivy/simplekivy.py`

 * *Files identical despite different names*

### Comparing `simplekivy-0.0.2/simplekivy/widgets/app.py` & `simplekivy-0.0.3/simplekivy/widgets/app.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,52 +7,54 @@
 file_path = os.path.abspath(os.path.dirname(__file__))
 print(file_path)
 Builder.load_file(os.path.join(file_path, "main.kv"))
 
 class MainApp(App):
     widgets = []
     def on_start(self):
-        
         for widofmainlist in self.widgets:
-            if type(widofmainlist) in (list, tuple, str):
-                self.freeze(widofmainlist)
+            if type(widofmainlist) in (list, tuple,  str):
+                wid = self.freeze(widofmainlist)
+                self.add_to_root(wid)
             else:
                 self.add_to_root(widofmainlist)
 
 
     def freeze(self, wid):
         #list for boxlayout
         if type(wid) is list:
             parent = F.BoxLayout(orientation="horizontal")
             self.row_widget_adder(wid, parent)
-
+            return parent
         #tuple for floatlayout
         elif type(wid) is tuple:
             parent = F.FloatLayout()
             self.row_widget_adder(wid, parent) 
+            return parent
 
         elif type(wid) is str:
             widget = Builder.load_string(wid)
-            self.add_to_root(widget)
-
+            return widget
+        
             
 
     def add_to_root(self, widget):
         self.add_to_widget(widget, self.root)
         
 
     def add_to_widget(self, widget, parent):
         try:
             parent.add_widget(widget()) 
         except TypeError:
             parent.add_widget(widget) 
 
     def row_widget_adder(self, widofmainlist, parent):
         
+                
         for item in widofmainlist:
             #put new boxlayout or floatlayout kwargs
             if type(item) is dict:
                 parent.__init__(**item)
             elif type(item) in (list, tuple, str):
-                self.freeze(item)
+                wid = self.freeze(item)
+                self.add_to_widget(wid, parent)
             else:self.add_to_widget(item, parent)
-        self.add_to_root(parent)
```

### Comparing `simplekivy-0.0.2/simplekivy.egg-info/PKG-INFO` & `simplekivy-0.0.3/simplekivy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplekivy
-Version: 0.0.2
+Version: 0.0.3
 Summary: the idea is inspired by PySimpleGui , to quickly create simple kivy apps 
 Author-email: yousuf <yosefmahmoud356@gmail.com>
 Project-URL: Homepage, https://github.com/yousuf60/SimpleKivy
 Project-URL: Bug Tracker, https://github.com/yousuf60/SimpleKivy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -113,15 +113,15 @@
 
 you can also add kvlang string directly instead of using 
 `s.lang.Builder`
 or `kivy.lang.Builder`
 
 ```python
 from simplekivy import SimpleKivy
-s = SimpleKivy(title="test app")
+s = SimpleKivy(title="test app", make_app=True)
 
 def on_enter(instance):
     print(instance.text)
     
 def btn_pressed():
     print(ainput.text)
 
@@ -129,34 +129,35 @@
 #add a new method to app
 s.myapp.btn_pressed = btn_pressed
 
 KV_BTN = """
 
 Button:
     text: "press me"
-    size_hint:.4, .1
-    pos_hint: {"center_x": .5}
+    size_hint:.4, .2
+    pos_hint: {"center_x": .5, "center_y": .5}
     on_press:app.btn_pressed()
 """
 ainput = s.TextInput(hint_text="type anything", multiline=False,  size_hint=(1, None),
      height="50dp", pos_hint={"center_x":.5, "center_y":.7})
 
 ainput.bind(on_text_validate=on_enter)
 
 s + [
-    [{"orientation":"vertical", "size_hint":(1, .4)},
+    [{"orientation":"vertical", "size_hint":(1, .2)},
     s.Label(text="hello world", halign="center"),
     s.Label(text="testo")],
     ({"size_hint":(.4, .4), "pos_hint":{"center_x":.5}},
         ainput 
     ),
-    ({"size_hint": (1, .2)},
+    ({"size_hint": (1, .4)},
         KV_BTN),
 ]
 
+
 ```
 
 <img src="https://github.com/yousuf60/SimpleKivy/assets/64571068/9e9e445e-0c6f-45de-9580-cd7fbde1f010" width="500">
 
 ### Hints
 ------
```

