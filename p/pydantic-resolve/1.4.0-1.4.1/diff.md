# Comparing `tmp/pydantic_resolve-1.4.0.tar.gz` & `tmp/pydantic_resolve-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_resolve-1.4.0.tar", max compression
+gzip compressed data, was "pydantic_resolve-1.4.1.tar", max compression
```

## Comparing `pydantic_resolve-1.4.0.tar` & `pydantic_resolve-1.4.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-1.4.0/LICENSE
--rw-r--r--   0        0        0      587 2023-07-03 08:03:54.897877 pydantic_resolve-1.4.0/pydantic_resolve/__init__.py
--rw-r--r--   0        0        0       90 2023-07-06 09:03:09.289534 pydantic_resolve-1.4.0/pydantic_resolve/constant.py
--rw-r--r--   0        0        0     3410 2023-07-06 10:43:29.600208 pydantic_resolve-1.4.0/pydantic_resolve/core.py
--rw-r--r--   0        0        0      229 2023-06-01 01:21:44.326847 pydantic_resolve-1.4.0/pydantic_resolve/exceptions.py
--rw-r--r--   0        0        0     6269 2023-07-06 10:42:54.099454 pydantic_resolve-1.4.0/pydantic_resolve/resolver.py
--rw-r--r--   0        0        0     4811 2023-07-03 08:00:07.994871 pydantic_resolve-1.4.0/pydantic_resolve/util.py
--rw-r--r--   0        0        0      814 2023-07-06 09:59:43.049219 pydantic_resolve-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     7660 2023-07-04 04:23:48.147702 pydantic_resolve-1.4.0/README.md
--rw-r--r--   0        0        0     8235 1970-01-01 00:00:00.000000 pydantic_resolve-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-1.4.1/LICENSE
+-rw-r--r--   0        0        0      587 2023-07-03 08:03:54.897877 pydantic_resolve-1.4.1/pydantic_resolve/__init__.py
+-rw-r--r--   0        0        0      228 2023-07-09 02:37:13.250821 pydantic_resolve-1.4.1/pydantic_resolve/constant.py
+-rw-r--r--   0        0        0     3552 2023-07-08 14:14:06.292603 pydantic_resolve-1.4.1/pydantic_resolve/core.py
+-rw-r--r--   0        0        0      229 2023-06-01 01:21:44.326847 pydantic_resolve-1.4.1/pydantic_resolve/exceptions.py
+-rw-r--r--   0        0        0     6512 2023-07-09 03:16:50.755677 pydantic_resolve-1.4.1/pydantic_resolve/resolver.py
+-rw-r--r--   0        0        0     6158 2023-07-09 03:16:50.754667 pydantic_resolve-1.4.1/pydantic_resolve/util.py
+-rw-r--r--   0        0        0      814 2023-07-06 14:14:21.541726 pydantic_resolve-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     7660 2023-07-04 04:23:48.147702 pydantic_resolve-1.4.1/README.md
+-rw-r--r--   0        0        0     8235 1970-01-01 00:00:00.000000 pydantic_resolve-1.4.1/PKG-INFO
```

### Comparing `pydantic_resolve-1.4.0/LICENSE` & `pydantic_resolve-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.4.0/pydantic_resolve/__init__.py` & `pydantic_resolve-1.4.1/pydantic_resolve/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.4.0/pydantic_resolve/core.py` & `pydantic_resolve-1.4.1/pydantic_resolve/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 from inspect import ismethod, iscoroutine
 from pydantic import BaseModel
-from dataclasses import is_dataclass
+from dataclasses import is_dataclass, fields as dc_fields
 from typing import TypeVar
 from .exceptions import ResolverTargetAttrNotFound, DataloaderDependCantBeResolved
 from .constant import PREFIX, POST_PREFIX, RESOLVER, ATTRIBUTE
 
 T = TypeVar("T")
 
 def is_list(target) -> bool:
@@ -30,17 +30,19 @@
     """
     # TODO: if pydantic object, read field from __fields__
     resolver_fields = set()
     fields = dir(target)
     resolvers = [f for f in fields if f.startswith(PREFIX)]
 
     if isinstance(target, BaseModel):
-        attributes = target.__fields__.keys()
+        attributes = list(target.__fields__.keys())
+    elif is_dataclass(target):
+        attributes = [f.name for f in dc_fields(target)]
     else:
-        attributes = [f for f in fields if not f.startswith('__')]
+        raise AttributeError('invalid type: should be pydantic object or dataclass object')
 
     for field in resolvers:
         attr = target.__getattribute__(field)
         if ismethod(attr):
             resolver_fields.add(field.replace(PREFIX, ''))
             yield (field, attr, RESOLVER)
```

### Comparing `pydantic_resolve-1.4.0/pydantic_resolve/resolver.py` & `pydantic_resolve-1.4.1/pydantic_resolve/resolver.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import inspect
 import contextvars
 from inspect import iscoroutine
 from typing import TypeVar, Dict
 from .exceptions import ResolverTargetAttrNotFound, LoaderFieldNotProvidedError, MissingAnnotationError
 from typing import Any, Callable, Optional
 from pydantic_resolve import core
-from .constant import PREFIX, POST_PREFIX, ATTRIBUTE, RESOLVER
-from .util import get_class_field_annotations
+from .constant import HAS_MAPPER_FUNCTION, PREFIX, POST_PREFIX, ATTRIBUTE, RESOLVER
+from .util import get_class_field_annotations, try_parse_data_to_target_field_type
 from inspect import isclass
 from aiodataloader import DataLoader
 
 
 def LoaderDepend(  # noqa: N802
     dependency: Optional[Callable[..., Any]] = None,
 ) -> Any:
@@ -104,42 +104,45 @@
 
                     cache_provider[cache_key] = loader
                     self.ctx.set(cache_provider)
                 params[k] = loader
         return method(**params)
 
 
-    async def resolve_obj(self, target, field, attr):
+    async def resolve_obj_field(self, target, field, attr):
         target_attr_name = str(field).replace(PREFIX, '')
 
         if not hasattr(target, target_attr_name):
             raise ResolverTargetAttrNotFound(f"attribute {target_attr_name} not found")
 
         if self.ensure_type:
             if not attr.__annotations__:
                 raise MissingAnnotationError(f'{field}: return annotation is required')
 
         val = self.exec_method(attr)
         while iscoroutine(val) or asyncio.isfuture(val):
             val = await val
 
         val = await self.resolve(val)  
+
+        if not getattr(attr, HAS_MAPPER_FUNCTION, False):  # defined in util.mapper
+            val = try_parse_data_to_target_field_type(target, target_attr_name, val)
         target.__setattr__(target_attr_name, val)
 
 
     async def resolve(self, target: T) -> T:
         """ entry: resolve dataclass object or pydantic object / or list in place """
         if isinstance(target, (list, tuple)):
             await asyncio.gather(*[self.resolve(t) for t in target])
 
         if core.is_acceptable_type(target):
             tasks = []
             for field, attr, _type in core.iter_over_object_resolvers_and_acceptable_fields(target):
                 if _type == ATTRIBUTE: tasks.append(self.resolve(attr))
-                if _type == RESOLVER: tasks.append(self.resolve_obj(target, field, attr))
+                if _type == RESOLVER: tasks.append(self.resolve_obj_field(target, field, attr))
 
             await asyncio.gather(*tasks)
 
             # execute post methods, take no params
             for post_key in core.iter_over_object_post_methods(target):
                 post_attr_name = post_key.replace(POST_PREFIX, '')
                 if not hasattr(target, post_attr_name):
```

### Comparing `pydantic_resolve-1.4.0/pydantic_resolve/util.py` & `pydantic_resolve-1.4.1/pydantic_resolve/util.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import asyncio
 from collections import defaultdict
 from dataclasses import is_dataclass
 import functools
-from pydantic import BaseModel
+from pydantic import BaseModel, parse_obj_as
 from inspect import iscoroutine
-from typing import Any, DefaultDict, Sequence, Type, TypeVar, List, Callable, Optional, Mapping, Union, Iterator
+from typing import Any, DefaultDict, Sequence, Type, TypeVar, List, Callable, Optional, Mapping, Union, Iterator, ForwardRef
 import types
+from .constant import PYDANTIC_FORWARD_REF_UPDATED, HAS_MAPPER_FUNCTION
+
+from pydantic_resolve.core import is_acceptable_type
 
 def get_class_field_annotations(cls: Type):
     anno = cls.__dict__.get('__annotations__') or {}
     return anno.keys()
 
 
 T = TypeVar("T")
@@ -48,14 +51,18 @@
     """
     execute post-transform function after the value is reolved
     func_or_class:
         is func: run func
         is class: call auto_mapping to have a try
     """
     def inner(inner_fn):
+
+        # if mapper provided, auto map from target type will be disabled
+        setattr(inner_fn, HAS_MAPPER_FUNCTION, True)
+
         @functools.wraps(inner_fn)
         async def wrap(*args, **kwargs):
 
             retVal = inner_fn(*args, **kwargs)
             while iscoroutine(retVal) or asyncio.isfuture(retVal):
                 retVal = await retVal  # get final result
             
@@ -132,8 +139,45 @@
                     base_field = base.__fields__.get(k)
                     if not base_field:
                         raise AttributeError(f'{k} not existed in {base.__name__}.')
                     if base_field and base_field.type_ != field.type_:
                         raise AttributeError(f'type of {k} not consistent with {base.__name__}'  )
             return  kls
         return inner()
-    return wrap
+    return wrap
+
+
+def forwrad_ref(kls: BaseModel):
+    kls.update_forward_refs()
+    setattr(kls, PYDANTIC_FORWARD_REF_UPDATED, True)
+
+    for field in kls.__fields__.values():
+        if issubclass(field.type_, BaseModel):
+            forwrad_ref(field.type_)
+
+def try_parse_data_to_target_field_type(target, field_name, data):
+    """
+    parse to pydantic or dataclass object
+    1. get type of target field
+    2. parse
+    """
+    field_type = None
+
+    # 1. get type of target field
+    if isinstance(target, BaseModel):
+        _fields = target.__fields__
+        field_type = _fields[field_name].annotation
+        # research/2_update_forward_ref.py
+        if getattr(target.__class__, PYDANTIC_FORWARD_REF_UPDATED, False):
+            forwrad_ref(target.__class__)
+
+    elif is_dataclass(target):
+        _fields = target.__dataclass_fields__
+        field_type = _fields[field_name].type
+
+    # 2. parse
+    if field_type:
+        result = parse_obj_as(field_type, data)
+        return result
+    
+    else:
+        return data
```

### Comparing `pydantic_resolve-1.4.0/pyproject.toml` & `pydantic_resolve-1.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-resolve"
-version = "1.4.0"
+version = "1.4.1"
 description = "Make pydantic have a GraphQL-like assembly experience."
 authors = ["tangkikodo <allmonday@126.com>"]
 readme = "README.md"
 repository = "https://github.com/allmonday/pydantic_resolve"
 keywords = ["pydantic", "fastapi"]
 license = "MIT"
 packages = [{include = "pydantic_resolve"}]
```

### Comparing `pydantic_resolve-1.4.0/README.md` & `pydantic_resolve-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.4.0/PKG-INFO` & `pydantic_resolve-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-resolve
-Version: 1.4.0
+Version: 1.4.1
 Summary: Make pydantic have a GraphQL-like assembly experience.
 Home-page: https://github.com/allmonday/pydantic_resolve
 License: MIT
 Keywords: pydantic,fastapi
 Author: tangkikodo
 Author-email: allmonday@126.com
 Requires-Python: >=3.7,<4.0
```

