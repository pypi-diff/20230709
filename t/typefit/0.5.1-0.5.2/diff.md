# Comparing `tmp/typefit-0.5.1.tar.gz` & `tmp/typefit-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typefit-0.5.1.tar", max compression
+gzip compressed data, was "typefit-0.5.2.tar", max compression
```

## Comparing `typefit-0.5.1.tar` & `typefit-0.5.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      484 2023-07-08 16:45:32.055478 typefit-0.5.1/LICENSE
--rw-r--r--   0        0        0     1477 2023-07-08 16:45:32.055478 typefit-0.5.1/README.md
--rw-r--r--   0        0        0     1351 2023-07-08 16:45:32.059479 typefit-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      268 2023-07-08 16:45:32.059479 typefit-0.5.1/src/typefit/__init__.py
--rw-r--r--   0        0        0    15459 2023-07-08 16:45:32.059479 typefit-0.5.1/src/typefit/api.py
--rw-r--r--   0        0        0     2008 2023-07-08 16:45:32.059479 typefit-0.5.1/src/typefit/compat.py
--rw-r--r--   0        0        0     8895 2023-07-08 16:45:32.059479 typefit-0.5.1/src/typefit/fitting.py
--rw-r--r--   0        0        0      453 2023-07-08 16:45:32.059479 typefit-0.5.1/src/typefit/httpx_models.py
--rw-r--r--   0        0        0     2428 2023-07-08 16:45:32.059479 typefit-0.5.1/src/typefit/meta.py
--rw-r--r--   0        0        0     1204 2023-07-08 16:45:32.059479 typefit-0.5.1/src/typefit/narrows.py
--rw-r--r--   0        0        0    23219 2023-07-08 16:45:32.059479 typefit-0.5.1/src/typefit/nodes.py
--rw-r--r--   0        0        0     9722 2023-07-08 16:45:32.059479 typefit-0.5.1/src/typefit/reporting.py
--rw-r--r--   0        0        0     7517 2023-07-08 16:45:32.059479 typefit-0.5.1/src/typefit/serialize.py
--rw-r--r--   0        0        0     2895 2023-07-08 16:45:32.059479 typefit-0.5.1/src/typefit/utils.py
--rw-r--r--   0        0        0     2170 1970-01-01 00:00:00.000000 typefit-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      484 2023-07-08 17:49:32.308079 typefit-0.5.2/LICENSE
+-rw-r--r--   0        0        0     1477 2023-07-08 17:49:32.308079 typefit-0.5.2/README.md
+-rw-r--r--   0        0        0     1351 2023-07-08 17:49:32.312080 typefit-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      268 2023-07-08 17:49:32.312080 typefit-0.5.2/src/typefit/__init__.py
+-rw-r--r--   0        0        0    15459 2023-07-08 17:49:32.312080 typefit-0.5.2/src/typefit/api.py
+-rw-r--r--   0        0        0     2008 2023-07-08 17:49:32.312080 typefit-0.5.2/src/typefit/compat.py
+-rw-r--r--   0        0        0     9525 2023-07-08 17:49:32.312080 typefit-0.5.2/src/typefit/fitting.py
+-rw-r--r--   0        0        0      453 2023-07-08 17:49:32.312080 typefit-0.5.2/src/typefit/httpx_models.py
+-rw-r--r--   0        0        0     2428 2023-07-08 17:49:32.312080 typefit-0.5.2/src/typefit/meta.py
+-rw-r--r--   0        0        0     1204 2023-07-08 17:49:32.312080 typefit-0.5.2/src/typefit/narrows.py
+-rw-r--r--   0        0        0    23219 2023-07-08 17:49:32.312080 typefit-0.5.2/src/typefit/nodes.py
+-rw-r--r--   0        0        0     9722 2023-07-08 17:49:32.312080 typefit-0.5.2/src/typefit/reporting.py
+-rw-r--r--   0        0        0     7517 2023-07-08 17:49:32.312080 typefit-0.5.2/src/typefit/serialize.py
+-rw-r--r--   0        0        0     2895 2023-07-08 17:49:32.312080 typefit-0.5.2/src/typefit/utils.py
+-rw-r--r--   0        0        0     2170 1970-01-01 00:00:00.000000 typefit-0.5.2/PKG-INFO
```

### Comparing `typefit-0.5.1/README.md` & `typefit-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `typefit-0.5.1/pyproject.toml` & `typefit-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "typefit"
-version = "0.5.1"
+version = "0.5.2"
 
 description = "Fits JSON values into Python type-anotated objects"
 license = "WTFPL"
 authors = [
     "Rémy Sanchez <remy.sanchez@hyperthese.net>"
 ]
```

### Comparing `typefit-0.5.1/src/typefit/api.py` & `typefit-0.5.2/src/typefit/api.py`

 * *Files identical despite different names*

### Comparing `typefit-0.5.1/src/typefit/compat.py` & `typefit-0.5.2/src/typefit/compat.py`

 * *Files identical despite different names*

### Comparing `typefit-0.5.1/src/typefit/fitting.py` & `typefit-0.5.2/src/typefit/fitting.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 from collections import abc
 from enum import Enum
 from inspect import isclass
-from typing import Any, Callable, Mapping, MutableSequence, Optional, Type, Union
+from types import UnionType
+from typing import (
+    Any,
+    Callable,
+    Literal,
+    Mapping,
+    MutableSequence,
+    Optional,
+    Type,
+    Union,
+)
 
 from .compat import get_args, get_origin
 from .nodes import *
 from .reporting import ErrorReporter, LogErrorReporter, PrettyJson5Formatter
 
 
 class Fitter:
@@ -127,14 +137,28 @@
             out = t(value.value)
         except ValueError:
             value.fail(f"No match in enum {t!r}")
         else:
             value.fit_success = True
             return out
 
+    def _fit_literal(self, t: Type[T], value: Node) -> T:
+        """
+        Tries to find back the right literal value
+        """
+
+        if get_origin(t) is not Literal:
+            value.fail(f"Type {t!r} is not a literal")
+
+        if value.value in get_args(t):
+            value.fit_success = True
+            return value.value
+
+        raise value.fail(f"No match in literal {t!r} (got {value!r})")
+
     def fit_node(self, t: Type[T], value: Node) -> T:
         """
         Tries to find the right fit according to the type you're trying to
         match and the node type.
 
         Notes
         -----
@@ -150,22 +174,26 @@
             A node you want to fit into a type
 
         Raises
         ------
         ValueError
         """
 
-        if get_origin(t) is Union:
+        origin = get_origin(t)
+
+        if origin is Union or origin is UnionType:
             return self._fit_union(t, value)
         elif t is Any:
             return self._fit_any(t, value)
         elif isinstance(value, (MappingNode, ListNode)):
             return value.fit(t)
         elif t is None or t is None.__class__:
             return self._fit_none(t, value)
+        elif origin is Literal:
+            return self._fit_literal(t, value)
         elif isclass(t):
             if issubclass(t, Enum):
                 return self._fit_enum(t, value)
             else:
                 return self._fit_class(t, value)
         else:
             value.fail("Could not fit. This error can never be reached in theory.")
@@ -219,15 +247,17 @@
         else:
             for injector in self.root_injectors:
                 injector(out)
 
             return out
 
 
-def typefit(t: Type[T], value: Any, context: Optional[Mapping[str, Any]] = None) -> T:
+def typefit(
+    t: Type[T] | UnionType, value: Any, context: Optional[Mapping[str, Any]] = None
+) -> T:
     """
     Fits a JSON-decoded value into native Python type-annotated objects.
 
     This uses the default sane settings but it might not be up to your taste.
     By example, errors will be reported in the logging module using ANSI escape
     codes for syntactical coloration, however depending on the situation you
     might not want that.
```

### Comparing `typefit-0.5.1/src/typefit/meta.py` & `typefit-0.5.2/src/typefit/meta.py`

 * *Files identical despite different names*

### Comparing `typefit-0.5.1/src/typefit/narrows.py` & `typefit-0.5.2/src/typefit/narrows.py`

 * *Files identical despite different names*

### Comparing `typefit-0.5.1/src/typefit/nodes.py` & `typefit-0.5.2/src/typefit/nodes.py`

 * *Files identical despite different names*

### Comparing `typefit-0.5.1/src/typefit/reporting.py` & `typefit-0.5.2/src/typefit/reporting.py`

 * *Files identical despite different names*

### Comparing `typefit-0.5.1/src/typefit/serialize.py` & `typefit-0.5.2/src/typefit/serialize.py`

 * *Files identical despite different names*

### Comparing `typefit-0.5.1/src/typefit/utils.py` & `typefit-0.5.2/src/typefit/utils.py`

 * *Files identical despite different names*

### Comparing `typefit-0.5.1/PKG-INFO` & `typefit-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typefit
-Version: 0.5.1
+Version: 0.5.2
 Summary: Fits JSON values into Python type-anotated objects
 Home-page: https://github.com/Xowap/typefit/
 License: WTFPL
 Keywords: typing,json,api
 Author: Rémy Sanchez
 Author-email: remy.sanchez@hyperthese.net
 Requires-Python: >=3.10,<4.0
```

