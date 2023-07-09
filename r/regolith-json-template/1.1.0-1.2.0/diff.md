# Comparing `tmp/regolith-json-template-1.1.0.tar.gz` & `tmp/regolith-json-template-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regolith-json-template-1.1.0.tar", last modified: Wed May 31 19:31:08 2023, max compression
+gzip compressed data, was "regolith-json-template-1.2.0.tar", last modified: Sun Jul  9 19:14:15 2023, max compression
```

## Comparing `regolith-json-template-1.1.0.tar` & `regolith-json-template-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 19:31:08.570666 regolith-json-template-1.1.0/
--rw-rw-rw-   0        0        0     1083 2023-02-24 19:44:45.000000 regolith-json-template-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     2150 2023-05-31 19:31:08.571667 regolith-json-template-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      556 2023-03-19 19:01:06.000000 regolith-json-template-1.1.0/README.rst
--rw-rw-rw-   0        0        0       90 2022-09-28 21:38:25.000000 regolith-json-template-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      764 2023-05-31 19:31:08.572668 regolith-json-template-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0       41 2022-09-28 23:50:58.000000 regolith-json-template-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-31 19:31:08.554579 regolith-json-template-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-31 19:31:08.563661 regolith-json-template-1.1.0/src/regolith_json_template/
--rw-rw-rw-   0        0        0     8118 2023-05-31 19:00:01.000000 regolith-json-template-1.1.0/src/regolith_json_template/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 19:31:08.569667 regolith-json-template-1.1.0/src/regolith_json_template.egg-info/
--rw-rw-rw-   0        0        0     2150 2023-05-31 19:31:08.000000 regolith-json-template-1.1.0/src/regolith_json_template.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-05-31 19:31:08.000000 regolith-json-template-1.1.0/src/regolith_json_template.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 19:31:08.000000 regolith-json-template-1.1.0/src/regolith_json_template.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-05-31 19:31:08.000000 regolith-json-template-1.1.0/src/regolith_json_template.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-09 19:14:15.822356 regolith-json-template-1.2.0/
+-rw-rw-rw-   0        0        0     1083 2023-02-24 19:44:45.000000 regolith-json-template-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     2150 2023-07-09 19:14:15.823349 regolith-json-template-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      556 2023-03-19 19:01:06.000000 regolith-json-template-1.2.0/README.rst
+-rw-rw-rw-   0        0        0       90 2022-09-28 21:38:25.000000 regolith-json-template-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0      764 2023-07-09 19:14:15.824351 regolith-json-template-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0       41 2022-09-28 23:50:58.000000 regolith-json-template-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 19:14:15.803604 regolith-json-template-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-09 19:14:15.814352 regolith-json-template-1.2.0/src/regolith_json_template/
+-rw-rw-rw-   0        0        0     9295 2023-07-09 19:11:03.000000 regolith-json-template-1.2.0/src/regolith_json_template/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 19:14:15.821354 regolith-json-template-1.2.0/src/regolith_json_template.egg-info/
+-rw-rw-rw-   0        0        0     2150 2023-07-09 19:14:15.000000 regolith-json-template-1.2.0/src/regolith_json_template.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-07-09 19:14:15.000000 regolith-json-template-1.2.0/src/regolith_json_template.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 19:14:15.000000 regolith-json-template-1.2.0/src/regolith_json_template.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-07-09 19:14:15.000000 regolith-json-template-1.2.0/src/regolith_json_template.egg-info/top_level.txt
```

### Comparing `regolith-json-template-1.1.0/LICENSE` & `regolith-json-template-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `regolith-json-template-1.1.0/PKG-INFO` & `regolith-json-template-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regolith-json-template
-Version: 1.1.0
+Version: 1.2.0
 Summary: A Python package for easier reuseability of the JSON Template Regolith filter for Minecraft Bedrock Edition
 Author: Nusiq
 License: MIT
 Project-URL: Source, https://github.com/Nusiq/regolith-json-template/tree/master
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `regolith-json-template-1.1.0/README.rst` & `regolith-json-template-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `regolith-json-template-1.1.0/setup.cfg` & `regolith-json-template-1.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `regolith-json-template-1.1.0/src/regolith_json_template/__init__.py` & `regolith-json-template-1.2.0/src/regolith_json_template/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from copy import deepcopy, copy
 import uuid
 import math
+import random
 from typing import Any, NamedTuple
 
-VERSION = (1, 1, 0)
+VERSION = (1, 2, 0)
 __version__ = '.'.join([str(x) for x in VERSION])
 
 EVAL_STRING_OPEN = '`'
 EVAL_STRING_CLOSE = '`'
 LIST_UNPACK_KEY = '__unpack__'
 LIST_UNPACK_OPTIONAL_VALUE = '__value__'
 
@@ -24,14 +25,22 @@
     template.
     '''
 
     def __init__(self, __key: str, **kwargs):
         self.key: str = __key
         self.scope_extension: dict[str, Any] = kwargs
 
+class JsonTemplateJoinStr:
+    '''
+    A data class used during the evalution of the template as a first item
+    of a list of strings to join and convert to one string. In JSON files
+    this class is known as "JoinStr" to reduce the amount of characters
+    '''
+    def __init__(self, join_str: str):
+        self.join_str = join_str
 
 class _Unpack(NamedTuple):
     '''
     _Unpack is an object that is used internally by the eval_json function to
     pass lists to be unpacked up from an item of the list, to the list itself.
     The value of the _Unpack object is a list of values to unpack.
     '''
@@ -129,21 +138,36 @@
                         else:  # copy the rest
                             data[evaluated_key] = deepcopy(old_data_k_value)
                         data[evaluated_key] = eval_json(
                             data[evaluated_key], child_scope)
                 else:
                     data[k] = eval_json(data[k], scope)
     elif isinstance(data, list):
+        join_strings: JsonTemplateJoinStr | None = None
         new_data = []
-        for item in data:
+        for i, item in enumerate(data):
             eval_item = eval_json(item, scope, True)
             if isinstance(eval_item, _Unpack):
-                new_data.extend(eval_item.data)
+                if (
+                        i == 0 and len(eval_item.data) > 0 and
+                        isinstance(eval_item.data[0], JsonTemplateJoinStr)):
+                    join_strings = eval_item.data[0]
+                    new_data.extend(eval_item.data[1:])
+                else:
+                    new_data.extend(eval_item.data)
+            elif i == 0 and isinstance(eval_item, JsonTemplateJoinStr):
+                join_strings = eval_item
             else:
                 new_data.append(eval_item)
+        if join_strings is not None:
+            try:
+                new_data = join_strings.join_str.join(new_data)
+            except TypeError as e:
+                raise JsonTemplateException(
+                    "Can't join non-string values using 'JoinStr'.") from e
         data = new_data
     elif isinstance(data, str):
         is_eval_val, data = is_eval_string(data)
         if is_eval_val:
             return eval_value(data, scope)
         return data
     return data
@@ -184,12 +208,12 @@
     scope to prevent the scope from being modified.
     '''
     return eval(value, copy(scope))
 
 
 DEFAULT_SCOPE = {
     'true': True, 'false': False, 'math': math, 'uuid': uuid,
-    "K": JsonTemplateK}
+    "random": random, "K": JsonTemplateK, "JoinStr": JsonTemplateJoinStr}
 '''
 The default socpe to be merged with the scope passed by the user in the regolith
 filter.
 '''
```

### Comparing `regolith-json-template-1.1.0/src/regolith_json_template.egg-info/PKG-INFO` & `regolith-json-template-1.2.0/src/regolith_json_template.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regolith-json-template
-Version: 1.1.0
+Version: 1.2.0
 Summary: A Python package for easier reuseability of the JSON Template Regolith filter for Minecraft Bedrock Edition
 Author: Nusiq
 License: MIT
 Project-URL: Source, https://github.com/Nusiq/regolith-json-template/tree/master
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

