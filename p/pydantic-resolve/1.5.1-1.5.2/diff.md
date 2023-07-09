# Comparing `tmp/pydantic_resolve-1.5.1.tar.gz` & `tmp/pydantic_resolve-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_resolve-1.5.1.tar", max compression
+gzip compressed data, was "pydantic_resolve-1.5.2.tar", max compression
```

## Comparing `pydantic_resolve-1.5.1.tar` & `pydantic_resolve-1.5.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-1.5.1/LICENSE
--rw-r--r--   0        0        0      587 2023-07-03 08:03:54.897877 pydantic_resolve-1.5.1/pydantic_resolve/__init__.py
--rw-r--r--   0        0        0      228 2023-07-09 02:37:13.250821 pydantic_resolve-1.5.1/pydantic_resolve/constant.py
--rw-r--r--   0        0        0     3552 2023-07-08 14:14:06.292603 pydantic_resolve-1.5.1/pydantic_resolve/core.py
--rw-r--r--   0        0        0      229 2023-06-01 01:21:44.326847 pydantic_resolve-1.5.1/pydantic_resolve/exceptions.py
--rw-r--r--   0        0        0     6512 2023-07-09 03:52:57.064430 pydantic_resolve-1.5.1/pydantic_resolve/resolver.py
--rw-r--r--   0        0        0     6158 2023-07-09 03:16:50.754667 pydantic_resolve-1.5.1/pydantic_resolve/util.py
--rw-r--r--   0        0        0      814 2023-07-09 03:55:40.833882 pydantic_resolve-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     7660 2023-07-04 04:23:48.147702 pydantic_resolve-1.5.1/README.md
--rw-r--r--   0        0        0     8235 1970-01-01 00:00:00.000000 pydantic_resolve-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-1.5.2/LICENSE
+-rw-r--r--   0        0        0      636 2023-07-09 14:14:07.250336 pydantic_resolve-1.5.2/pydantic_resolve/__init__.py
+-rw-r--r--   0        0        0      228 2023-07-09 02:37:13.250821 pydantic_resolve-1.5.2/pydantic_resolve/constant.py
+-rw-r--r--   0        0        0     3500 2023-07-09 14:33:28.855034 pydantic_resolve-1.5.2/pydantic_resolve/core.py
+-rw-r--r--   0        0        0      229 2023-06-01 01:21:44.326847 pydantic_resolve-1.5.2/pydantic_resolve/exceptions.py
+-rw-r--r--   0        0        0     6466 2023-07-09 14:08:38.068320 pydantic_resolve-1.5.2/pydantic_resolve/resolver.py
+-rw-r--r--   0        0        0     6308 2023-07-09 14:47:21.962032 pydantic_resolve-1.5.2/pydantic_resolve/util.py
+-rw-r--r--   0        0        0      814 2023-07-09 14:53:35.697368 pydantic_resolve-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     7472 2023-07-09 04:03:38.318092 pydantic_resolve-1.5.2/README.md
+-rw-r--r--   0        0        0     8050 1970-01-01 00:00:00.000000 pydantic_resolve-1.5.2/PKG-INFO
```

### Comparing `pydantic_resolve-1.5.1/LICENSE` & `pydantic_resolve-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.5.1/pydantic_resolve/core.py` & `pydantic_resolve-1.5.2/pydantic_resolve/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,25 +24,24 @@
 
 def iter_over_object_resolvers_and_acceptable_fields(target):
     """
         return 
         1. method starts with resolve_,  eg: resolve_name, resolve_age
         2. field of pydantic or dataclass, which is not resolved by step1. (if `resolve_name` already exists, it will skip `name` )
     """
-    # TODO: if pydantic object, read field from __fields__
     resolver_fields = set()
     fields = dir(target)
     resolvers = [f for f in fields if f.startswith(PREFIX)]
 
     if isinstance(target, BaseModel):
         attributes = list(target.__fields__.keys())
     elif is_dataclass(target):
         attributes = [f.name for f in dc_fields(target)]
     else:
-        raise AttributeError('invalid type: should be pydantic object or dataclass object')
+        raise AttributeError('invalid type: should be pydantic object or dataclass object')  # noqa
 
     for field in resolvers:
         attr = target.__getattribute__(field)
         if ismethod(attr):
             resolver_fields.add(field.replace(PREFIX, ''))
             yield (field, attr, RESOLVER)
```

### Comparing `pydantic_resolve-1.5.1/pydantic_resolve/resolver.py` & `pydantic_resolve-1.5.2/pydantic_resolve/resolver.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 import inspect
 import contextvars
 from inspect import iscoroutine
 from typing import TypeVar, Dict
 from .exceptions import ResolverTargetAttrNotFound, LoaderFieldNotProvidedError, MissingAnnotationError
 from typing import Any, Callable, Optional
 from pydantic_resolve import core
-from .constant import HAS_MAPPER_FUNCTION, PREFIX, POST_PREFIX, ATTRIBUTE, RESOLVER
-from .util import get_class_field_annotations, try_parse_data_to_target_field_type
-from inspect import isclass
 from aiodataloader import DataLoader
+from inspect import isclass
+
+import pydantic_resolve.constant as const
+import pydantic_resolve.util as util
 
 
 def LoaderDepend(  # noqa: N802
     dependency: Optional[Callable[..., Any]] = None,
 ) -> Any:
     return Depends(dependency=dependency)
 
@@ -87,15 +88,15 @@
                         # and pick config from 'loader_filters' param, only for DataClass
                         filter_config_provider = self.loader_filters_ctx.get()
                         filter_config = filter_config_provider.get(Base, {})
 
                         # class ExampleLoader(DataLoader):
                         #     filtar_x: bool  <--------------- set this field
 
-                        for field in get_class_field_annotations(Base):
+                        for field in util.get_class_field_annotations(Base):
                             try:
                                 value = filter_config[field]
                                 setattr(loader, field, value)
                             except KeyError:
                                 raise LoaderFieldNotProvidedError(f'{cache_key}.{field} not found in Resolver()')
 
                     # build loader from batch_load_fn, filters config is impossible
@@ -105,51 +106,51 @@
                     cache_provider[cache_key] = loader
                     self.ctx.set(cache_provider)
                 params[k] = loader
         return method(**params)
 
 
     async def resolve_obj_field(self, target, field, attr):
-        target_attr_name = str(field).replace(PREFIX, '')
+        target_attr_name = str(field).replace(const.PREFIX, '')
 
         if not hasattr(target, target_attr_name):
             raise ResolverTargetAttrNotFound(f"attribute {target_attr_name} not found")
 
         if self.ensure_type:
             if not attr.__annotations__:
                 raise MissingAnnotationError(f'{field}: return annotation is required')
 
         val = self.exec_method(attr)
         while iscoroutine(val) or asyncio.isfuture(val):
             val = await val
 
-        if not getattr(attr, HAS_MAPPER_FUNCTION, False):  # defined in util.mapper
-            val = try_parse_data_to_target_field_type(target, target_attr_name, val)
+        if not getattr(attr, const.HAS_MAPPER_FUNCTION, False):  # defined in util.mapper
+            val = util.try_parse_data_to_target_field_type(target, target_attr_name, val)
 
         val = await self.resolve(val)
 
         target.__setattr__(target_attr_name, val)
 
 
     async def resolve(self, target: T) -> T:
         """ entry: resolve dataclass object or pydantic object / or list in place """
         if isinstance(target, (list, tuple)):
             await asyncio.gather(*[self.resolve(t) for t in target])
 
         if core.is_acceptable_type(target):
             tasks = []
             for field, attr, _type in core.iter_over_object_resolvers_and_acceptable_fields(target):
-                if _type == ATTRIBUTE: tasks.append(self.resolve(attr))
-                if _type == RESOLVER: tasks.append(self.resolve_obj_field(target, field, attr))
+                if _type == const.ATTRIBUTE: tasks.append(self.resolve(attr))
+                if _type == const.RESOLVER: tasks.append(self.resolve_obj_field(target, field, attr))
 
             await asyncio.gather(*tasks)
 
             # execute post methods, take no params
             for post_key in core.iter_over_object_post_methods(target):
-                post_attr_name = post_key.replace(POST_PREFIX, '')
+                post_attr_name = post_key.replace(const.POST_PREFIX, '')
                 if not hasattr(target, post_attr_name):
                     raise ResolverTargetAttrNotFound(f"fail to run {post_key}(), attribute {post_attr_name} not found")
 
                 post_method = target.__getattribute__(post_key)
                 post_method()
 
         return target
```

### Comparing `pydantic_resolve-1.5.1/pydantic_resolve/util.py` & `pydantic_resolve-1.5.2/pydantic_resolve/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import asyncio
+import types
+import functools
 from collections import defaultdict
 from dataclasses import is_dataclass
-import functools
 from pydantic import BaseModel, parse_obj_as
 from inspect import iscoroutine
-from typing import Any, DefaultDict, Sequence, Type, TypeVar, List, Callable, Optional, Mapping, Union, Iterator, ForwardRef
-import types
-from .constant import PYDANTIC_FORWARD_REF_UPDATED, HAS_MAPPER_FUNCTION
+from typing import Any, DefaultDict, Sequence, Type, TypeVar, List, Callable, Optional, Mapping, Union, Iterator
+
+import pydantic_resolve.constant as const
 
-from pydantic_resolve.core import is_acceptable_type
 
 def get_class_field_annotations(cls: Type):
     anno = cls.__dict__.get('__annotations__') or {}
     return anno.keys()
 
 
 T = TypeVar("T")
@@ -53,15 +53,15 @@
     func_or_class:
         is func: run func
         is class: call auto_mapping to have a try
     """
     def inner(inner_fn):
 
         # if mapper provided, auto map from target type will be disabled
-        setattr(inner_fn, HAS_MAPPER_FUNCTION, True)
+        setattr(inner_fn, const.HAS_MAPPER_FUNCTION, True)
 
         @functools.wraps(inner_fn)
         async def wrap(*args, **kwargs):
 
             retVal = inner_fn(*args, **kwargs)
             while iscoroutine(retVal) or asyncio.isfuture(retVal):
                 retVal = await retVal  # get final result
@@ -128,56 +128,66 @@
     """
     used with pydantic class to make sure a class's field is 
     subset of target class
     """
     def wrap(kls):
         assert issubclass(base, BaseModel), 'base should be pydantic class'
         assert issubclass(kls, BaseModel), 'class should be pydantic class'
+
         @functools.wraps(kls)
         def inner():
             for k, field in kls.__fields__.items():
                 if field.required:
                     base_field = base.__fields__.get(k)
                     if not base_field:
                         raise AttributeError(f'{k} not existed in {base.__name__}.')
                     if base_field and base_field.type_ != field.type_:
                         raise AttributeError(f'type of {k} not consistent with {base.__name__}'  )
             return  kls
         return inner()
     return wrap
 
 
-def forwrad_ref(kls: BaseModel):
+def update_forward_refs(kls: BaseModel):
+    """
+    recursively update refs.
+    """
     kls.update_forward_refs()
-    setattr(kls, PYDANTIC_FORWARD_REF_UPDATED, True)
+    setattr(kls, const.PYDANTIC_FORWARD_REF_UPDATED, True)
 
     for field in kls.__fields__.values():
         if issubclass(field.type_, BaseModel):
-            forwrad_ref(field.type_)
+            update_forward_refs(field.type_)
+
 
 def try_parse_data_to_target_field_type(target, field_name, data):
     """
     parse to pydantic or dataclass object
     1. get type of target field
     2. parse
     """
     field_type = None
 
     # 1. get type of target field
     if isinstance(target, BaseModel):
-        _fields = target.__fields__
-        field_type = _fields[field_name].annotation
+        _fields = target.__class__.__fields__
+        field_type = _fields[field_name].outer_type_
+
+        # handle optional logic
+        if data is None and _fields[field_name].required == False:
+            return data
+
         # research/2_update_forward_ref.py
-        if getattr(target.__class__, PYDANTIC_FORWARD_REF_UPDATED, False):
-            forwrad_ref(target.__class__)
+        if getattr(target.__class__, const.PYDANTIC_FORWARD_REF_UPDATED, False):
+            update_forward_refs(target.__class__)
 
     elif is_dataclass(target):
         _fields = target.__dataclass_fields__
         field_type = _fields[field_name].type
 
     # 2. parse
     if field_type:
         result = parse_obj_as(field_type, data)
         return result
     
     else:
-        return data
+        return data  #noqa
```

### Comparing `pydantic_resolve-1.5.1/pyproject.toml` & `pydantic_resolve-1.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-resolve"
-version = "1.5.1"
+version = "1.5.2"
 description = "Make pydantic have a GraphQL-like assembly experience."
 authors = ["tangkikodo <allmonday@126.com>"]
 readme = "README.md"
 repository = "https://github.com/allmonday/pydantic_resolve"
 keywords = ["pydantic", "fastapi"]
 license = "MIT"
 packages = [{include = "pydantic_resolve"}]
```

### Comparing `pydantic_resolve-1.5.1/README.md` & `pydantic_resolve-1.5.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 class Contact(BaseModel):
     number: Optional[int]
 
 class Friend(BaseModel):
     name: str
 
     contact: Optional[Contact] = None
-    @mapper(Contact)                                          # 1. resolve dataloader and map return dict to Contact object
     def resolve_contact(self, contact_loader=LoaderDepend(contact_batch_load_fn)):
         return contact_loader.load(self.name)
 
     is_contact_10: bool = False
     def post_is_contact_10(self):                             # 3. after resolve_contact executed, do extra computation
         if self.contact:
             if str(self.contact.number).startswith('10'):
@@ -71,30 +70,28 @@
 
     greeting: str = ''
     async def resolve_greeting(self):
         await asyncio.sleep(1)
         return f"hello, i'm {self.name}, {self.age} years old."
 
     contact: Optional[Contact] = None
-    @mapper(Contact)
     def resolve_contact(self, contact_loader=LoaderDepend(contact_batch_load_fn)):
         return contact_loader.load(self.name)
 
     friends: List[Friend] = []
-    @mapper(lambda names: [Friend(name=name) for name in names])
+    @mapper(lambda names: [Friend(name=name) for name in names])  # manually convert
     def resolve_friends(self, friend_loader=LoaderDepend(friends_batch_load_fn)):
         return friend_loader.load(self.name)
 
     friend_count: int = 0
     def post_friend_count(self):
         self.friend_count = len(self.friends)
 
 class Root(BaseModel):
     users: List[User] = []
-    @mapper(lambda items: [User(**item) for item in items])
     def resolve_users(self):
         return [
             {"name": "tangkikodo", "age": 19},
             {"name": "john", "age": 20},
             {"name": "trump", "age": 21},
             {"name": "sally", "age": 22},
             {"name": "no man", "age": 23},
```

### Comparing `pydantic_resolve-1.5.1/PKG-INFO` & `pydantic_resolve-1.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-resolve
-Version: 1.5.1
+Version: 1.5.2
 Summary: Make pydantic have a GraphQL-like assembly experience.
 Home-page: https://github.com/allmonday/pydantic_resolve
 License: MIT
 Keywords: pydantic,fastapi
 Author: tangkikodo
 Author-email: allmonday@126.com
 Requires-Python: >=3.7,<4.0
@@ -71,15 +71,14 @@
 class Contact(BaseModel):
     number: Optional[int]
 
 class Friend(BaseModel):
     name: str
 
     contact: Optional[Contact] = None
-    @mapper(Contact)                                          # 1. resolve dataloader and map return dict to Contact object
     def resolve_contact(self, contact_loader=LoaderDepend(contact_batch_load_fn)):
         return contact_loader.load(self.name)
 
     is_contact_10: bool = False
     def post_is_contact_10(self):                             # 3. after resolve_contact executed, do extra computation
         if self.contact:
             if str(self.contact.number).startswith('10'):
@@ -93,30 +92,28 @@
 
     greeting: str = ''
     async def resolve_greeting(self):
         await asyncio.sleep(1)
         return f"hello, i'm {self.name}, {self.age} years old."
 
     contact: Optional[Contact] = None
-    @mapper(Contact)
     def resolve_contact(self, contact_loader=LoaderDepend(contact_batch_load_fn)):
         return contact_loader.load(self.name)
 
     friends: List[Friend] = []
-    @mapper(lambda names: [Friend(name=name) for name in names])
+    @mapper(lambda names: [Friend(name=name) for name in names])  # manually convert
     def resolve_friends(self, friend_loader=LoaderDepend(friends_batch_load_fn)):
         return friend_loader.load(self.name)
 
     friend_count: int = 0
     def post_friend_count(self):
         self.friend_count = len(self.friends)
 
 class Root(BaseModel):
     users: List[User] = []
-    @mapper(lambda items: [User(**item) for item in items])
     def resolve_users(self):
         return [
             {"name": "tangkikodo", "age": 19},
             {"name": "john", "age": 20},
             {"name": "trump", "age": 21},
             {"name": "sally", "age": 22},
             {"name": "no man", "age": 23},
```

