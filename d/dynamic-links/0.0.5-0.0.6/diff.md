# Comparing `tmp/dynamic-links-0.0.5.tar.gz` & `tmp/dynamic-links-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic-links-0.0.5.tar", last modified: Sun Jul  9 04:52:45 2023, max compression
+gzip compressed data, was "dynamic-links-0.0.6.tar", last modified: Sun Jul  9 05:44:31 2023, max compression
```

## Comparing `dynamic-links-0.0.5.tar` & `dynamic-links-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 pic        (501) staff       (20)        0 2023-07-09 04:52:45.732798 dynamic-links-0.0.5/
--rw-r--r--   0 pic        (501) staff       (20)     6301 2023-07-09 04:52:45.732662 dynamic-links-0.0.5/PKG-INFO
--rw-r--r--   0 pic        (501) staff       (20)     6028 2023-07-09 04:44:56.000000 dynamic-links-0.0.5/README.md
-drwxr-xr-x   0 pic        (501) staff       (20)        0 2023-07-09 04:52:45.731752 dynamic-links-0.0.5/dlframe/
--rw-r--r--   0 pic        (501) staff       (20)     2614 2023-07-08 17:27:46.000000 dynamic-links-0.0.5/dlframe/CalculationNode.py
--rw-r--r--   0 pic        (501) staff       (20)     3958 2023-07-09 04:46:22.000000 dynamic-links-0.0.5/dlframe/CalculationNodeManager.py
--rw-r--r--   0 pic        (501) staff       (20)     2048 2023-06-27 04:00:46.000000 dynamic-links-0.0.5/dlframe/ExecutionNode.py
--rw-r--r--   0 pic        (501) staff       (20)      939 2023-06-27 05:19:42.000000 dynamic-links-0.0.5/dlframe/Logger.py
--rw-r--r--   0 pic        (501) staff       (20)     5277 2023-07-08 16:20:45.000000 dynamic-links-0.0.5/dlframe/WebManager.py
--rw-r--r--   0 pic        (501) staff       (20)      141 2023-06-26 17:09:16.000000 dynamic-links-0.0.5/dlframe/__init__.py
-drwxr-xr-x   0 pic        (501) staff       (20)        0 2023-07-09 04:52:45.732473 dynamic-links-0.0.5/dynamic_links.egg-info/
--rw-r--r--   0 pic        (501) staff       (20)     6301 2023-07-09 04:52:45.000000 dynamic-links-0.0.5/dynamic_links.egg-info/PKG-INFO
--rw-r--r--   0 pic        (501) staff       (20)      348 2023-07-09 04:52:45.000000 dynamic-links-0.0.5/dynamic_links.egg-info/SOURCES.txt
--rw-r--r--   0 pic        (501) staff       (20)        1 2023-07-09 04:52:45.000000 dynamic-links-0.0.5/dynamic_links.egg-info/dependency_links.txt
--rw-r--r--   0 pic        (501) staff       (20)       30 2023-07-09 04:52:45.000000 dynamic-links-0.0.5/dynamic_links.egg-info/requires.txt
--rw-r--r--   0 pic        (501) staff       (20)        8 2023-07-09 04:52:45.000000 dynamic-links-0.0.5/dynamic_links.egg-info/top_level.txt
--rw-r--r--   0 pic        (501) staff       (20)       38 2023-07-09 04:52:45.732840 dynamic-links-0.0.5/setup.cfg
--rw-r--r--   0 pic        (501) staff       (20)      682 2023-07-09 04:48:53.000000 dynamic-links-0.0.5/setup.py
+drwxr-xr-x   0 pic        (501) staff       (20)        0 2023-07-09 05:44:31.509507 dynamic-links-0.0.6/
+-rw-r--r--   0 pic        (501) staff       (20)     6301 2023-07-09 05:44:31.509358 dynamic-links-0.0.6/PKG-INFO
+-rw-r--r--   0 pic        (501) staff       (20)     6028 2023-07-09 04:44:56.000000 dynamic-links-0.0.6/README.md
+drwxr-xr-x   0 pic        (501) staff       (20)        0 2023-07-09 05:44:31.508453 dynamic-links-0.0.6/dlframe/
+-rw-r--r--   0 pic        (501) staff       (20)     2645 2023-07-09 05:06:10.000000 dynamic-links-0.0.6/dlframe/CalculationNode.py
+-rw-r--r--   0 pic        (501) staff       (20)     4034 2023-07-09 05:32:50.000000 dynamic-links-0.0.6/dlframe/CalculationNodeManager.py
+-rw-r--r--   0 pic        (501) staff       (20)     2048 2023-06-27 04:00:46.000000 dynamic-links-0.0.6/dlframe/ExecutionNode.py
+-rw-r--r--   0 pic        (501) staff       (20)      939 2023-06-27 05:19:42.000000 dynamic-links-0.0.6/dlframe/Logger.py
+-rw-r--r--   0 pic        (501) staff       (20)     5277 2023-07-08 16:20:45.000000 dynamic-links-0.0.6/dlframe/WebManager.py
+-rw-r--r--   0 pic        (501) staff       (20)      141 2023-06-26 17:09:16.000000 dynamic-links-0.0.6/dlframe/__init__.py
+drwxr-xr-x   0 pic        (501) staff       (20)        0 2023-07-09 05:44:31.509166 dynamic-links-0.0.6/dynamic_links.egg-info/
+-rw-r--r--   0 pic        (501) staff       (20)     6301 2023-07-09 05:44:31.000000 dynamic-links-0.0.6/dynamic_links.egg-info/PKG-INFO
+-rw-r--r--   0 pic        (501) staff       (20)      348 2023-07-09 05:44:31.000000 dynamic-links-0.0.6/dynamic_links.egg-info/SOURCES.txt
+-rw-r--r--   0 pic        (501) staff       (20)        1 2023-07-09 05:44:31.000000 dynamic-links-0.0.6/dynamic_links.egg-info/dependency_links.txt
+-rw-r--r--   0 pic        (501) staff       (20)       30 2023-07-09 05:44:31.000000 dynamic-links-0.0.6/dynamic_links.egg-info/requires.txt
+-rw-r--r--   0 pic        (501) staff       (20)        8 2023-07-09 05:44:31.000000 dynamic-links-0.0.6/dynamic_links.egg-info/top_level.txt
+-rw-r--r--   0 pic        (501) staff       (20)       38 2023-07-09 05:44:31.509556 dynamic-links-0.0.6/setup.cfg
+-rw-r--r--   0 pic        (501) staff       (20)      682 2023-07-09 05:09:12.000000 dynamic-links-0.0.6/setup.py
```

### Comparing `dynamic-links-0.0.5/PKG-INFO` & `dynamic-links-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-links
-Version: 0.0.5
+Version: 0.0.6
 Summary: a calculation framework
 Home-page: https://github.com/picpic2013/dlframe-back
 Author: PIC
 Author-email: picpic2019@gmail.com
 License: MIT
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
```

### Comparing `dynamic-links-0.0.5/README.md` & `dynamic-links-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `dynamic-links-0.0.5/dlframe/CalculationNode.py` & `dynamic-links-0.0.6/dlframe/CalculationNode.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         node = CalculationNode('function_call', self.node_manager, self)
         self.next_nodes.append(node)
 
         node.is_function = True
         node.function_args = all_args
         node.function_kwargs = all_kwargs
 
-        if self.element_dict is not None and type(next(iter(self.element_dict.values()))) == type:
+        if self.element_dict is not None and len(self.element_dict) > 0 and type(next(iter(self.element_dict.values()))) == type:
             for t in self.element_dict.values():
                 assert type(t) == type, 'elements should have same type'
             node.is_init_function = True
 
         for arg in all_args:
             arg.next_nodes.append(node)
             node.last_nodes.append(arg)
```

### Comparing `dynamic-links-0.0.5/dlframe/CalculationNodeManager.py` & `dynamic-links-0.0.6/dlframe/CalculationNodeManager.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,24 +50,24 @@
             for next_node in current_node.node.next_nodes:
                 next_node_name = id(next_node)
                 node_dict[next_node_name].in_degree -= 1
                 if node_dict[next_node_name].in_degree == 0:
                     node_queue.put(next_node_name)
         return self
     
-    def register(self, class_type_name=None, option_name=None, element=None, display=None):
+    def register(self, class_type_name, option_name=None, element=None, display=None):
         if type(option_name) == dict:
             if display is None:
                 display = True
             return self.register_element(class_type_name, option_name, display)
         if element is not None:
             if option_name is None:
                 option_name = element.__name__
             node = None
-            if class_type_name is None or class_type_name not in self.class_type_name2node.keys():
+            if class_type_name not in self.class_type_name2node.keys():
                 element_dict = {option_name: element}
                 if class_type_name is None:
                     class_type_name = '__Element__' + str(element_dict)
                 elif display is None:
                     display = True
                 node = CalculationNode(class_type_name, self, None, element_dict, is_root_node=True)
                 self.class_type_name2node.setdefault(class_type_name, node)
@@ -81,8 +81,10 @@
             return node
         def _warp_function_(raw_element, class_type_name=class_type_name, option_name=option_name, display=display, self=self):
             self.register(class_type_name, option_name, raw_element, display)
             return raw_element
         return _warp_function_
     
     def __getitem__(self, key):
-        return self.class_type_name2node[key]
+        if key in self.class_type_name2node.keys():
+            return self.class_type_name2node[key]
+        return self.register(key, {}, display=True)
```

### Comparing `dynamic-links-0.0.5/dlframe/ExecutionNode.py` & `dynamic-links-0.0.6/dlframe/ExecutionNode.py`

 * *Files identical despite different names*

### Comparing `dynamic-links-0.0.5/dlframe/Logger.py` & `dynamic-links-0.0.6/dlframe/Logger.py`

 * *Files identical despite different names*

### Comparing `dynamic-links-0.0.5/dlframe/WebManager.py` & `dynamic-links-0.0.6/dlframe/WebManager.py`

 * *Files identical despite different names*

### Comparing `dynamic-links-0.0.5/dynamic_links.egg-info/PKG-INFO` & `dynamic-links-0.0.6/dynamic_links.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-links
-Version: 0.0.5
+Version: 0.0.6
 Summary: a calculation framework
 Home-page: https://github.com/picpic2013/dlframe-back
 Author: PIC
 Author-email: picpic2019@gmail.com
 License: MIT
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
```

### Comparing `dynamic-links-0.0.5/setup.py` & `dynamic-links-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 with open(os.path.join(here, 'README.md'), 'r',encoding='UTF-8') as mdFile:
     long_description = mdFile.read()
 
 setup(
     name='dynamic-links', 
-    version='0.0.5', 
+    version='0.0.6', 
     packages=['dlframe'], 
     url='https://github.com/picpic2013/dlframe-back', 
     license='MIT', 
     author='PIC', 
     author_email='picpic2019@gmail.com', 
     description='a calculation framework', 
     long_description=long_description,
```

