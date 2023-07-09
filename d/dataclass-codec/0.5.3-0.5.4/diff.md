# Comparing `tmp/dataclass_codec-0.5.3.tar.gz` & `tmp/dataclass_codec-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclass_codec-0.5.3.tar", max compression
+gzip compressed data, was "dataclass_codec-0.5.4.tar", max compression
```

## Comparing `dataclass_codec-0.5.3.tar` & `dataclass_codec-0.5.4.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0    10143 2023-07-09 19:00:29.355476 dataclass_codec-0.5.3/README.md
--rw-r--r--   0        0        0      600 2023-07-09 19:00:42.995473 dataclass_codec-0.5.3/pyproject.toml
--rw-r--r--   0        0        0      246 2023-06-21 01:44:15.139451 dataclass_codec-0.5.3/src/dataclass_codec/__init__.py
--rw-r--r--   0        0        0    15242 2023-07-09 03:57:07.697077 dataclass_codec-0.5.3/src/dataclass_codec/decode.py
--rw-r--r--   0        0        0     2929 2023-06-21 01:51:35.509431 dataclass_codec-0.5.3/src/dataclass_codec/encode.py
--rw-r--r--   0        0        0        0 2023-06-21 01:44:15.139451 dataclass_codec-0.5.3/src/dataclass_codec/py.typed
--rw-r--r--   0        0        0    21509 2023-07-09 04:07:07.587053 dataclass_codec-0.5.3/src/dataclass_codec/tests/test_dataclass_codec.py
--rw-r--r--   0        0        0      436 2023-07-09 03:52:02.877095 dataclass_codec-0.5.3/src/dataclass_codec/types_predicates.py
--rw-r--r--   0        0        0    10596 1970-01-01 00:00:00.000000 dataclass_codec-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0    10143 2023-07-09 19:00:29.355476 dataclass_codec-0.5.4/README.md
+-rw-r--r--   0        0        0      577 2023-07-09 20:22:10.354295 dataclass_codec-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0      246 2023-06-21 01:44:15.139451 dataclass_codec-0.5.4/src/dataclass_codec/__init__.py
+-rw-r--r--   0        0        0    15936 2023-07-09 20:21:35.834303 dataclass_codec-0.5.4/src/dataclass_codec/decode.py
+-rw-r--r--   0        0        0     2929 2023-06-21 01:51:35.509431 dataclass_codec-0.5.4/src/dataclass_codec/encode.py
+-rw-r--r--   0        0        0        0 2023-06-21 01:44:15.139451 dataclass_codec-0.5.4/src/dataclass_codec/py.typed
+-rw-r--r--   0        0        0    21758 2023-07-09 20:21:53.334299 dataclass_codec-0.5.4/src/dataclass_codec/tests/test_dataclass_codec.py
+-rw-r--r--   0        0        0      845 2023-07-09 20:21:53.284299 dataclass_codec-0.5.4/src/dataclass_codec/tests/test_python3_9.py
+-rw-r--r--   0        0        0      436 2023-07-09 03:52:02.877095 dataclass_codec-0.5.4/src/dataclass_codec/types_predicates.py
+-rw-r--r--   0        0        0    10596 1970-01-01 00:00:00.000000 dataclass_codec-0.5.4/PKG-INFO
```

### Comparing `dataclass_codec-0.5.3/README.md` & `dataclass_codec-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `dataclass_codec-0.5.3/pyproject.toml` & `dataclass_codec-0.5.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataclass-codec"
-version = "0.5.3"
+version = "0.5.4"
 description = ""
 authors = ["lucas.silva <lucas.silva@jeaholding.com.br>"]
 readme = "README.md"
 packages = [{include = "dataclass_codec", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -20,13 +20,12 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.mypy]
-python_version = "3.8"
 strict_optional = true
 strict = true
 
 [tool.black]
 line-length = 79
```

### Comparing `dataclass_codec-0.5.3/src/dataclass_codec/decode.py` & `dataclass_codec-0.5.4/src/dataclass_codec/decode.py`

 * *Files 1% similar despite different names*

```diff
@@ -376,14 +376,36 @@
     def make_value(i: int) -> Any:
         with current_path_scope(current_path() + f"[{i}]"):
             return decode_it(obj[i], _type.__args__[0])
 
     return [make_value(i) for i in range(len(obj))]
 
 
+def is_generic_tuple_predicate(_type: ANYTYPE) -> bool:
+    return hasattr(_type, "__origin__") and _type.__origin__ is tuple
+
+
+def generic_tuple_decoder(
+    obj: Any, _type: ANYTYPE, decode_it: DECODEIT
+) -> Any:
+    assert is_generic_tuple_predicate(_type), "{} is not a tuple".format(
+        _type.__name__
+    )
+
+    assert isinstance(obj, tuple), "{} is {} not tuple".format(
+        current_path(), type(obj)
+    )
+
+    def make_value(i: int) -> Any:
+        with current_path_scope(current_path() + f"[{i}]"):
+            return decode_it(obj[i], _type.__args__[0])
+
+    return tuple([make_value(i) for i in range(len(obj))])
+
+
 def is_generic_dict_predicate(_type: ANYTYPE) -> bool:
     return hasattr(_type, "__origin__") and _type.__origin__ is dict
 
 
 def generic_dict_decoder(obj: Any, _type: ANYTYPE, decode_it: DECODEIT) -> Any:
     assert is_generic_dict_predicate(_type), "{} is not a dict".format(
         _type.__name__
@@ -494,14 +516,15 @@
 DEFAULT_DECODERS_BY_PREDICATE: List[Tuple[TYPEMATCHPREDICATE, TYPEDECODER]] = [
     (is_any_type_predicate, any_type_decoder),
     (is_dataclass_predicate, dataclass_from_primitive_dict),
     (is_generic_dataclass_predicate, generic_dataclass_from_primitive_dict),
     (is_generic_list_predicate, generic_list_decoder),
     (is_generic_dict_predicate, generic_dict_decoder),
     (is_union_predicate, generic_union_decoder),
+    (is_generic_tuple_predicate, generic_tuple_decoder),
     # This must be before is_enum_predicate
     (is_new_type_predicate, generic_new_type_decoder),
     (is_enum_predicate, enum_decoder),
     # This must be last
     (inherits_some_class_predicate, generic_inheritance_decoder),
 ]
```

### Comparing `dataclass_codec-0.5.3/src/dataclass_codec/encode.py` & `dataclass_codec-0.5.4/src/dataclass_codec/encode.py`

 * *Files identical despite different names*

### Comparing `dataclass_codec-0.5.3/src/dataclass_codec/tests/test_dataclass_codec.py` & `dataclass_codec-0.5.4/src/dataclass_codec/tests/test_dataclass_codec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 import base64
 from dataclasses import dataclass, field
 from datetime import date, datetime, time, timezone
 from decimal import Decimal
 from enum import Enum
 import json
-from typing import Any, Dict, Generic, List, NewType, Optional, TypeVar, Union
+from typing import (
+    Any,
+    Dict,
+    Generic,
+    List,
+    NewType,
+    Optional,
+    TypeVar,
+    Union,
+)
 
 import pytest
 
 from dataclass_codec import (
     encode,
     decode,
     decode_context_scope,
@@ -244,17 +253,23 @@
 
     def test_encode_none(self) -> None:
         assert encode(None) is None
 
     def test_encode_list(self) -> None:
         assert encode([1, 2, 3]) == [1, 2, 3]
 
+    def test_decode_list(self) -> None:
+        assert decode([1, 2, 3], List[int]) == [1, 2, 3]
+
     def test_encode_tuple(self) -> None:
         assert encode((1, 2, 3)) == [1, 2, 3]
 
+    # def test_decode_tuple(self) -> None:
+    #     assert decode((1, 2, 3), Tuple[int, int, int]) == (1, 2, 3)
+
     def test_encode_dict(self) -> None:
         assert encode({"a": 1}) == {"a": 1}
 
     def test_encode_datetime(self) -> None:
         assert (
             encode(datetime(2020, 1, 1, 0, 0, 0, tzinfo=timezone.utc))
             == "2020-01-01T00:00:00+00:00"
```

### Comparing `dataclass_codec-0.5.3/PKG-INFO` & `dataclass_codec-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataclass-codec
-Version: 0.5.3
+Version: 0.5.4
 Summary: 
 Author: lucas.silva
 Author-email: lucas.silva@jeaholding.com.br
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

