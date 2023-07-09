# Comparing `tmp/dataclass_codec-0.4.0.tar.gz` & `tmp/dataclass_codec-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclass_codec-0.4.0.tar", max compression
+gzip compressed data, was "dataclass_codec-0.4.1.tar", max compression
```

## Comparing `dataclass_codec-0.4.0.tar` & `dataclass_codec-0.4.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      101 2023-06-21 01:55:42.515322 dataclass_codec-0.4.0/README.md
--rw-r--r--   0        0        0      600 2023-07-04 18:08:54.207588 dataclass_codec-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      246 2023-06-18 01:48:53.622553 dataclass_codec-0.4.0/src/dataclass_codec/__init__.py
--rw-r--r--   0        0        0    11675 2023-07-04 18:06:19.677208 dataclass_codec-0.4.0/src/dataclass_codec/decode.py
--rw-r--r--   0        0        0     2929 2023-06-21 01:55:42.515322 dataclass_codec-0.4.0/src/dataclass_codec/encode.py
--rw-r--r--   0        0        0        0 2023-06-18 00:31:15.872983 dataclass_codec-0.4.0/src/dataclass_codec/py.typed
--rw-r--r--   0        0        0    16856 2023-07-04 18:07:07.947335 dataclass_codec-0.4.0/src/dataclass_codec/tests/test_dataclass_codec.py
--rw-r--r--   0        0        0      391 2023-07-04 17:50:20.533913 dataclass_codec-0.4.0/src/dataclass_codec/types_predicates.py
--rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 dataclass_codec-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      101 2023-06-21 01:50:47.819434 dataclass_codec-0.4.1/README.md
+-rw-r--r--   0        0        0      600 2023-07-09 04:07:53.767051 dataclass_codec-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      246 2023-06-21 01:44:15.139451 dataclass_codec-0.4.1/src/dataclass_codec/__init__.py
+-rw-r--r--   0        0        0    15242 2023-07-09 03:57:07.697077 dataclass_codec-0.4.1/src/dataclass_codec/decode.py
+-rw-r--r--   0        0        0     2929 2023-06-21 01:51:35.509431 dataclass_codec-0.4.1/src/dataclass_codec/encode.py
+-rw-r--r--   0        0        0        0 2023-06-21 01:44:15.139451 dataclass_codec-0.4.1/src/dataclass_codec/py.typed
+-rw-r--r--   0        0        0    21509 2023-07-09 04:07:07.587053 dataclass_codec-0.4.1/src/dataclass_codec/tests/test_dataclass_codec.py
+-rw-r--r--   0        0        0      436 2023-07-09 03:52:02.877095 dataclass_codec-0.4.1/src/dataclass_codec/types_predicates.py
+-rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 dataclass_codec-0.4.1/PKG-INFO
```

### Comparing `dataclass_codec-0.4.0/pyproject.toml` & `dataclass_codec-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataclass-codec"
-version = "0.4.0"
+version = "0.4.1"
 description = ""
 authors = ["lucas.silva <lucas.silva@jeaholding.com.br>"]
 readme = "README.md"
 packages = [{include = "dataclass_codec", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `dataclass_codec-0.4.0/src/dataclass_codec/decode.py` & `dataclass_codec-0.4.1/src/dataclass_codec/decode.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 import base64
 from contextlib import contextmanager
 from contextvars import ContextVar
 from dataclasses import MISSING, Field, dataclass
 from datetime import date, datetime, time
 from decimal import Decimal
 from enum import Enum
+from operator import indexOf
 from typing import (
+    TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Generator,
+    Generic,
     List,
     Optional,
     Tuple,
     Type,
     TypeVar,
     Union,
     cast,
+    get_args,
 )
 from uuid import UUID
 
 from dataclass_codec.types_predicates import (
     is_dataclass_predicate,
     is_enum_predicate,
     is_generic_dataclass_predicate,
 )
 
+if TYPE_CHECKING:
+    pass
+
 
 ANYTYPE = Type[Any]
 
 
 TYPEMATCHPREDICATE = Callable[[ANYTYPE], bool]
 DECODEIT = Callable[[Any, ANYTYPE], Any]
 TYPEDECODER = Callable[[Any, ANYTYPE, DECODEIT], Any]
@@ -105,29 +112,95 @@
         error_list().append((current_path(), e))
         if not decode_context().collect_errors:
             raise
     finally:
         current_path_cxt_var.reset(token)
 
 
+TYPES_PATH = Tuple[Type[Any], ...]
+
+types_path_cxt_var = ContextVar[TYPES_PATH]("types_path_cxt_var", default=())
+
+
+@contextmanager
+def types_path_scope(
+    types_path: TYPES_PATH,
+) -> Generator[None, Any, None]:
+    token = types_path_cxt_var.set(types_path)
+    try:
+        yield
+    finally:
+        types_path_cxt_var.reset(token)
+
+
+def current_types_path() -> TYPES_PATH:
+    return types_path_cxt_var.get()
+
+
+def discover_typevar(_type: Type[Any]) -> Any:
+    if len(current_types_path()) == 0:
+        raise TypeError(f"Cannot decode {_type}")
+
+    typevar_context = [*current_types_path()][::-1]
+
+    types_path: Tuple[Type[Any], ...] = ()
+    index = -1
+    for t in typevar_context:
+        base_t = t
+        types_path = types_path + (base_t,)
+        while hasattr(base_t, "__origin__") or hasattr(
+            base_t, "__orig_bases__"
+        ):
+            if hasattr(base_t, "__origin__"):
+                if hasattr(base_t.__origin__, "__orig_bases__"):
+                    if hasattr(
+                        base_t.__origin__.__orig_bases__[0], "__origin__"
+                    ):
+                        if (
+                            base_t.__origin__.__orig_bases__[0].__origin__
+                            is Generic
+                        ):
+                            index = indexOf(
+                                base_t.__origin__.__orig_bases__[0].__args__,
+                                _type,
+                            )
+                            if index != -1:
+                                break
+
+                base_t = base_t.__origin__
+            else:
+                base_t = base_t.__orig_bases__[0]
+
+    if index == -1:
+        raise TypeError(f"Typevar {_type} not found in {types_path}")
+    corresponding_type = base_t.__args__[index]
+    return corresponding_type
+
+
 def raw_decode(
     obj: Any,
     obj_type: Type[T],
     decoders: Dict[ANYTYPE, TYPEDECODER],
     decoders_by_predicate: List[Tuple[TYPEMATCHPREDICATE, TYPEDECODER]],
 ) -> T:
     def decode_it(obj: Any, _type: ANYTYPE) -> Any:
+        if isinstance(_type, TypeVar):
+            _type = discover_typevar(_type)
         return raw_decode(obj, _type, decoders, decoders_by_predicate)
 
+    if isinstance(obj_type, TypeVar):
+        obj_type.__bound__
+
     if obj_type in decoders:
         return cast(T, decoders[obj_type](obj, obj_type, decode_it))
 
     for predicate, decoder in decoders_by_predicate:
         if predicate(obj_type):
-            return cast(T, decoder(obj, obj_type, decode_it))
+            with types_path_scope(current_types_path() + (obj_type,)):
+                return cast(T, decoder(obj, obj_type, decode_it))
 
     raise TypeError(f"Cannot decode {obj_type}")
 
 
 def primitive_hook(_type: ANYTYPE) -> TYPEDECODER:
     def decode_primitive(
         obj: Any, _type: ANYTYPE, _decode_it: DECODEIT
@@ -146,15 +219,15 @@
                 time,
             )
 
         if ctx.primitive_cast_values and type_can_cast(_type):
             return _type(obj)
 
         if ctx.strict and _type(obj) != obj:
-            raise TypeError(f"Cannot decode {obj} as {_type}")
+            raise TypeError(f"Cannot decode {obj} ({type(obj)}) as {_type}")
 
         return obj
 
     return decode_primitive
 
 
 def list_hook(obj: Any, _type: ANYTYPE, decode_it: DECODEIT) -> Any:
@@ -243,28 +316,36 @@
         _type
     ), "{} is not a dataclass".format(_type.__name__)
 
     assert isinstance(obj, dict), "{} is {} not dict".format(
         current_path(), type(obj)
     )
 
-    def make_value(k: str) -> Any:
+    def make_value(k: str, t: Type[Any]) -> Any:
         with current_path_scope(current_path() + "." + k):
             if k not in obj:
                 if cxt.dataclass_unset_as_none:
                     return None
                 else:
                     raise ValueError(f"Missing key {k}")
 
-            return decode_it(obj[k], _type.__args__[0])
+            if isinstance(t, TypeVar):
+                generic_args: Tuple[Any, ...] = get_args(
+                    _type.__origin__.__orig_bases__[0]
+                )
+                index = indexOf(generic_args, t)
+                if index == -1:
+                    raise TypeError(f"Typevar {t} not found in {generic_args}")
+                t = _type.__args__[index]
+            return decode_it(obj[k], t)
 
     return _type(
         **{
-            k: make_value(k)
-            for k in _type.__origin__.__dataclass_fields__.keys()
+            k: make_value(k, t.type)
+            for k, t in _type.__origin__.__dataclass_fields__.items()
         }
     )
 
 
 def decimal_from_str(obj: Any, _type: ANYTYPE, _decode_it: DECODEIT) -> Any:
     assert isinstance(
         obj, (str, int, float)
@@ -421,14 +502,51 @@
     (is_new_type_predicate, generic_new_type_decoder),
     (is_enum_predicate, enum_decoder),
     # This must be last
     (inherits_some_class_predicate, generic_inheritance_decoder),
 ]
 
 
+TYPEVAR_MAP = Dict[TypeVar, Type[Any]]
+
+typevar_context_cxt_var = ContextVar[TYPEVAR_MAP](
+    "typevar_context_cxt_var", default={}
+)
+
+
+@contextmanager
+def typevar_context_scope(
+    typevar_context: TYPEVAR_MAP,
+) -> Generator[None, Any, None]:
+    token = typevar_context_cxt_var.set(typevar_context)
+    try:
+        yield
+    finally:
+        typevar_context_cxt_var.reset(token)
+
+
+def get_root_generic_type(_type: Type[Any]) -> Optional[Type[Any]]:
+    if hasattr(_type, "__origin__"):
+        if _type.__origin__ is Generic:
+            return _type
+        return get_root_generic_type(_type.__origin__)
+    elif hasattr(_type, "__orig_bases__"):
+        if len(_type.__orig_bases__) == 0:
+            return _type
+        if len(_type.__orig_bases__) > 1:
+            raise TypeError(f"Cannot decode {type(_type)} with multiple bases")
+        if _type.__orig_bases__[0] is Generic:
+            return _type
+
+        return get_root_generic_type(_type.__orig_bases__[0])
+    else:
+        return None
+
+
 def decode(obj: Any, _type: Type[T]) -> T:
     if _type is None:
         _type = type(obj)
+
     with current_path_scope("$"):
         return raw_decode(
             obj, _type, DEFAULT_DECODERS, DEFAULT_DECODERS_BY_PREDICATE
         )
```

### Comparing `dataclass_codec-0.4.0/src/dataclass_codec/encode.py` & `dataclass_codec-0.4.1/src/dataclass_codec/encode.py`

 * *Files identical despite different names*

### Comparing `dataclass_codec-0.4.0/src/dataclass_codec/tests/test_dataclass_codec.py` & `dataclass_codec-0.4.1/src/dataclass_codec/tests/test_dataclass_codec.py`

 * *Files 20% similar despite different names*

```diff
@@ -612,7 +612,193 @@
 
     def test_default_factory(self) -> None:
         @dataclass
         class Dummy:
             a: List[int] = field(default_factory=list)
 
         assert decode({}, Dummy) == Dummy([])
+
+    def test_generic_dataclass_pagination(self) -> None:
+        T = TypeVar("T")
+
+        @dataclass
+        class PaginationData:
+            count: int
+            current: int
+
+        @dataclass
+        class Pagination(Generic[T]):
+            data: List[T]
+            pagination: PaginationData
+
+        @dataclass
+        class Dummy:
+            a: str
+
+        class DummyPagination(Pagination[Dummy]):
+            pass
+
+        dict_dummy_pagination = {
+            "data": [{"a": "hello"}],
+            "pagination": {"count": 1, "current": 1},
+        }
+
+        assert decode(
+            dict_dummy_pagination, DummyPagination
+        ) == DummyPagination(
+            data=[Dummy(a="hello")],
+            pagination=PaginationData(count=1, current=1),
+        )
+
+        DummyPagination2 = Pagination[Dummy]
+
+        assert decode(
+            dict_dummy_pagination, DummyPagination2
+        ) == DummyPagination2(
+            data=[Dummy(a="hello")],
+            pagination=PaginationData(count=1, current=1),
+        )
+
+    def test_double_generic_dataclass(self) -> None:
+        T = TypeVar("T")
+        U = TypeVar("U")
+
+        @dataclass
+        class Dummy(Generic[T, U]):
+            a: T
+            b: U
+
+        assert decode({"a": 1, "b": "hello"}, Dummy[int, str]) == Dummy(
+            a=1, b="hello"
+        )
+
+    def test_complex_double_generic_class(self) -> None:
+        T = TypeVar("T")
+        U = TypeVar("U")
+
+        @dataclass
+        class PaginationData:
+            count: int
+            current: int
+
+        @dataclass
+        class Pagination(Generic[T]):
+            data: List[T]
+            pagination: PaginationData
+
+        @dataclass
+        class Dummy(Generic[T, U]):
+            a: T
+            b: U
+
+        class DummyPagination(Pagination[Dummy[int, str]]):
+            pass
+
+        dict_dummy_pagination = {
+            "data": [{"a": 1, "b": "hello"}],
+            "pagination": {"count": 1, "current": 1},
+        }
+
+        assert decode(
+            dict_dummy_pagination, DummyPagination
+        ) == DummyPagination(
+            data=[Dummy(a=1, b="hello")],
+            pagination=PaginationData(count=1, current=1),
+        )
+
+    def test_triple_generic_dataclass(self) -> None:
+        T = TypeVar("T")
+        U = TypeVar("U")
+        V = TypeVar("V")
+
+        @dataclass
+        class Dummy(Generic[T, U, V]):
+            a: T
+            b: U
+            c: V
+
+        assert decode(
+            {"a": 1, "b": "hello", "c": 1.1}, Dummy[int, str, float]
+        ) == Dummy(a=1, b="hello", c=1.1)
+
+    def test_complex_triple_generic_class(self) -> None:
+        T = TypeVar("T")
+        U = TypeVar("U")
+        V = TypeVar("V")
+
+        @dataclass
+        class PaginationData:
+            count: int
+            current: int
+
+        @dataclass
+        class Pagination(Generic[T]):
+            data: List[T]
+            pagination: PaginationData
+
+        @dataclass
+        class Dummy(Generic[T, U, V]):
+            a: T
+            b: U
+            c: V
+
+        class DummyPagination(Pagination[Dummy[int, str, float]]):
+            pass
+
+        dict_dummy_pagination = {
+            "data": [{"a": 1, "b": "hello", "c": 1.1}],
+            "pagination": {"count": 1, "current": 1},
+        }
+
+        assert decode(
+            dict_dummy_pagination, DummyPagination
+        ) == DummyPagination(
+            data=[Dummy(a=1, b="hello", c=1.1)],
+            pagination=PaginationData(count=1, current=1),
+        )
+
+    def test_generic_without_type(self) -> None:
+        T = TypeVar("T")
+
+        @dataclass
+        class Dummy(Generic[T]):
+            a: T
+
+        with pytest.raises(TypeError):
+            decode({"a": 1}, Dummy)
+
+    def test_generic_with_wrong_type(self) -> None:
+        T = TypeVar("T")
+
+        @dataclass
+        class Dummy(Generic[T]):
+            a: T
+
+        with pytest.raises(TypeError):
+            with decode_context_scope(
+                DecodeContext(
+                    primitive_cast_values=False,
+                    strict=True,
+                )
+            ):
+                decode({"a": 1}, Dummy[str])
+
+    def test_direct_generic(self) -> None:
+        T = TypeVar("T")
+
+        @dataclass
+        class Dummy(Generic[T]):
+            a: T
+
+        @dataclass
+        class Dummy2:
+            dummy: Dummy[int]
+
+        @dataclass
+        class DummyMap(Generic[T]):
+            dummy: Dict[str, Dummy[T]]
+
+        assert decode({"dummy": {"a": 1}}, Dummy2) == Dummy2(dummy=Dummy(a=1))
+
+        assert decode({"dummy": {"a": {"a": 1}}}, DummyMap[int]) == DummyMap(
+            dummy={"a": Dummy(a=1)}
+        )
```

### Comparing `dataclass_codec-0.4.0/PKG-INFO` & `dataclass_codec-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataclass-codec
-Version: 0.4.0
+Version: 0.4.1
 Summary: 
 Author: lucas.silva
 Author-email: lucas.silva@jeaholding.com.br
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

