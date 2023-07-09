# Comparing `tmp/polyfactory-2.5.0.tar.gz` & `tmp/polyfactory-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyfactory-2.5.0.tar", max compression
+gzip compressed data, was "polyfactory-2.6.0.tar", max compression
```

## Comparing `polyfactory-2.5.0.tar` & `polyfactory-2.6.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0     1092 2023-06-30 19:43:25.009172 polyfactory-2.5.0/LICENSE
--rw-r--r--   0        0        0    24136 2023-06-30 19:43:25.009172 polyfactory-2.5.0/docs/PYPI_README.md
--rw-r--r--   0        0        0      425 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/__init__.py
--rw-r--r--   0        0        0      875 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/constants.py
--rw-r--r--   0        0        0     1037 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/decorators.py
--rw-r--r--   0        0        0      591 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/exceptions.py
--rw-r--r--   0        0        0      257 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/factories/__init__.py
--rw-r--r--   0        0        0    33045 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/factories/base.py
--rw-r--r--   0        0        0     2758 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/factories/beanie_odm_factory.py
--rw-r--r--   0        0        0     1681 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/factories/dataclass_factory.py
--rw-r--r--   0        0        0     2392 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/factories/msgspec_factory.py
--rw-r--r--   0        0        0     2192 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/factories/odmantic_odm_factory.py
--rw-r--r--   0        0        0    10468 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/factories/pydantic_factory.py
--rw-r--r--   0        0        0     1431 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/factories/typed_dict_factory.py
--rw-r--r--   0        0        0     7084 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/field_meta.py
--rw-r--r--   0        0        0     3317 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/fields.py
--rw-r--r--   0        0        0     1192 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/persistence.py
--rw-r--r--   0        0        0        0 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/py.typed
--rw-r--r--   0        0        0     2850 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/pytest_plugin.py
--rw-r--r--   0        0        0        0 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/utils/__init__.py
--rw-r--r--   0        0        0     3852 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/utils/helpers.py
--rw-r--r--   0        0        0     3498 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/utils/predicates.py
--rw-r--r--   0        0        0        0 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/value_generators/__init__.py
--rw-r--r--   0        0        0     1605 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/value_generators/complex_types.py
--rw-r--r--   0        0        0     1885 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/value_generators/constrained_collections.py
--rw-r--r--   0        0        0     1125 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/value_generators/constrained_dates.py
--rw-r--r--   0        0        0    13429 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/value_generators/constrained_numbers.py
--rw-r--r--   0        0        0      433 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/value_generators/constrained_path.py
--rw-r--r--   0        0        0     3846 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/value_generators/constrained_strings.py
--rw-r--r--   0        0        0      440 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/value_generators/constrained_url.py
--rw-r--r--   0        0        0      446 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/value_generators/constrained_uuid.py
--rw-r--r--   0        0        0     3635 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/value_generators/primitives.py
--rw-r--r--   0        0        0     6172 2023-06-30 19:43:25.013172 polyfactory-2.5.0/polyfactory/value_generators/regex.py
--rw-r--r--   0        0        0     6733 2023-06-30 19:43:25.013172 polyfactory-2.5.0/pyproject.toml
--rw-r--r--   0        0        0    26005 1970-01-01 00:00:00.000000 polyfactory-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-07-09 18:26:30.435526 polyfactory-2.6.0/LICENSE
+-rw-r--r--   0        0        0    24136 2023-07-09 18:26:30.435526 polyfactory-2.6.0/docs/PYPI_README.md
+-rw-r--r--   0        0        0      425 2023-07-09 18:26:30.439527 polyfactory-2.6.0/polyfactory/__init__.py
+-rw-r--r--   0        0        0     2525 2023-07-09 18:26:30.439527 polyfactory-2.6.0/polyfactory/collection_extender.py
+-rw-r--r--   0        0        0      912 2023-07-09 18:26:30.439527 polyfactory-2.6.0/polyfactory/constants.py
+-rw-r--r--   0        0        0     1037 2023-07-09 18:26:30.439527 polyfactory-2.6.0/polyfactory/decorators.py
+-rw-r--r--   0        0        0      591 2023-07-09 18:26:30.439527 polyfactory-2.6.0/polyfactory/exceptions.py
+-rw-r--r--   0        0        0      257 2023-07-09 18:26:30.439527 polyfactory-2.6.0/polyfactory/factories/__init__.py
+-rw-r--r--   0        0        0    33696 2023-07-09 18:26:30.439527 polyfactory-2.6.0/polyfactory/factories/base.py
+-rw-r--r--   0        0        0     2758 2023-07-09 18:26:30.439527 polyfactory-2.6.0/polyfactory/factories/beanie_odm_factory.py
+-rw-r--r--   0        0        0     1912 2023-07-09 18:26:30.439527 polyfactory-2.6.0/polyfactory/factories/dataclass_factory.py
+-rw-r--r--   0        0        0     2684 2023-07-09 18:26:30.443527 polyfactory-2.6.0/polyfactory/factories/msgspec_factory.py
+-rw-r--r--   0        0        0     2192 2023-07-09 18:26:30.443527 polyfactory-2.6.0/polyfactory/factories/odmantic_odm_factory.py
+-rw-r--r--   0        0        0    13500 2023-07-09 18:26:30.443527 polyfactory-2.6.0/polyfactory/factories/pydantic_factory.py
+-rw-r--r--   0        0        0     1650 2023-07-09 18:26:30.443527 polyfactory-2.6.0/polyfactory/factories/typed_dict_factory.py
+-rw-r--r--   0        0        0     8230 2023-07-09 18:26:30.443527 polyfactory-2.6.0/polyfactory/field_meta.py
+-rw-r--r--   0        0        0     3317 2023-07-09 18:26:30.443527 polyfactory-2.6.0/polyfactory/fields.py
+-rw-r--r--   0        0        0     1192 2023-07-09 18:26:30.443527 polyfactory-2.6.0/polyfactory/persistence.py
+-rw-r--r--   0        0        0        0 2023-07-09 18:26:30.443527 polyfactory-2.6.0/polyfactory/py.typed
+-rw-r--r--   0        0        0     2850 2023-07-09 18:26:30.443527 polyfactory-2.6.0/polyfactory/pytest_plugin.py
+-rw-r--r--   0        0        0        0 2023-07-09 18:26:30.443527 polyfactory-2.6.0/polyfactory/utils/__init__.py
+-rw-r--r--   0        0        0     3852 2023-07-09 18:26:30.443527 polyfactory-2.6.0/polyfactory/utils/helpers.py
+-rw-r--r--   0        0        0     3764 2023-07-09 18:26:30.443527 polyfactory-2.6.0/polyfactory/utils/predicates.py
+-rw-r--r--   0        0        0        0 2023-07-09 18:26:30.443527 polyfactory-2.6.0/polyfactory/value_generators/__init__.py
+-rw-r--r--   0        0        0     1948 2023-07-09 18:26:30.443527 polyfactory-2.6.0/polyfactory/value_generators/complex_types.py
+-rw-r--r--   0        0        0     1885 2023-07-09 18:26:30.443527 polyfactory-2.6.0/polyfactory/value_generators/constrained_collections.py
+-rw-r--r--   0        0        0     1125 2023-07-09 18:26:30.443527 polyfactory-2.6.0/polyfactory/value_generators/constrained_dates.py
+-rw-r--r--   0        0        0    13429 2023-07-09 18:26:30.443527 polyfactory-2.6.0/polyfactory/value_generators/constrained_numbers.py
+-rw-r--r--   0        0        0      433 2023-07-09 18:26:30.443527 polyfactory-2.6.0/polyfactory/value_generators/constrained_path.py
+-rw-r--r--   0        0        0     3846 2023-07-09 18:26:30.443527 polyfactory-2.6.0/polyfactory/value_generators/constrained_strings.py
+-rw-r--r--   0        0        0      440 2023-07-09 18:26:30.443527 polyfactory-2.6.0/polyfactory/value_generators/constrained_url.py
+-rw-r--r--   0        0        0      446 2023-07-09 18:26:30.443527 polyfactory-2.6.0/polyfactory/value_generators/constrained_uuid.py
+-rw-r--r--   0        0        0     3635 2023-07-09 18:26:30.443527 polyfactory-2.6.0/polyfactory/value_generators/primitives.py
+-rw-r--r--   0        0        0     6172 2023-07-09 18:26:30.443527 polyfactory-2.6.0/polyfactory/value_generators/regex.py
+-rw-r--r--   0        0        0     6900 2023-07-09 18:26:30.443527 polyfactory-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0    26005 1970-01-01 00:00:00.000000 polyfactory-2.6.0/PKG-INFO
```

### Comparing `polyfactory-2.5.0/LICENSE` & `polyfactory-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `polyfactory-2.5.0/docs/PYPI_README.md` & `polyfactory-2.6.0/docs/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `polyfactory-2.5.0/polyfactory/constants.py` & `polyfactory-2.6.0/polyfactory/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 from collections import abc, defaultdict, deque
 from random import Random
 from typing import (
-    Any,
     DefaultDict,
     Deque,
     Dict,
     FrozenSet,
     Iterable,
     List,
     Mapping,
@@ -38,10 +37,11 @@
     abc.Iterable: list,
     abc.Mapping: dict,
     abc.Sequence: list,
     abc.Set: set,
     UnionType: Union,
 }
 
-IGNORED_TYPE_ARGS: set[Any] = {Ellipsis}
-
 DEFAULT_RANDOM = Random()
+RANDOMIZE_COLLECTION_LENGTH = False
+MIN_COLLECTION_LENGTH = 0
+MAX_COLLECTION_LENGTH = 5
```

### Comparing `polyfactory-2.5.0/polyfactory/decorators.py` & `polyfactory-2.6.0/polyfactory/decorators.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.5.0/polyfactory/exceptions.py` & `polyfactory-2.6.0/polyfactory/exceptions.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.5.0/polyfactory/factories/base.py` & `polyfactory-2.6.0/polyfactory/factories/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,20 @@
     cast,
 )
 from uuid import NAMESPACE_DNS, UUID, uuid1, uuid3, uuid5
 
 from faker import Faker
 from typing_extensions import get_args
 
-from polyfactory.constants import DEFAULT_RANDOM
+from polyfactory.constants import (
+    DEFAULT_RANDOM,
+    MAX_COLLECTION_LENGTH,
+    MIN_COLLECTION_LENGTH,
+    RANDOMIZE_COLLECTION_LENGTH,
+)
 from polyfactory.exceptions import (
     ConfigurationException,
     MissingBuildKwargException,
     ParameterException,
 )
 from polyfactory.fields import Fixture, Ignore, PostGenerated, Require, Use
 from polyfactory.utils.helpers import unwrap_annotation, unwrap_args, unwrap_optional
@@ -116,56 +121,38 @@
             pydantic.IPvAnyAddress: cls.__faker__.ipv4,
             pydantic.IPvAnyInterface: cls.__faker__.ipv4,
             pydantic.IPvAnyNetwork: lambda: cls.__faker__.ipv4(network=True),
             pydantic.PastDate: cls.__faker__.past_date,
             pydantic.FutureDate: cls.__faker__.future_date,
         }
 
+        if pydantic.VERSION.startswith("1"):
+            # v1 only values - these will raise an exception in v2
+            # in pydantic v2 these are all aliases for Annotated with a constraint.
+            # we therefore do not need them in v2
+            mapping.update(
+                {  # pyright: ignore
+                    pydantic.PyObject: lambda: "decimal.Decimal",
+                    pydantic.AmqpDsn: lambda: "amqps://example.com",
+                    pydantic.KafkaDsn: lambda: "kafka://localhost:9092",
+                    pydantic.PostgresDsn: lambda: "postgresql://user:secret@localhost",
+                    pydantic.RedisDsn: lambda: "redis://localhost:6379/0",
+                    pydantic.FilePath: lambda: Path(realpath(__file__)),
+                    pydantic.DirectoryPath: lambda: Path(realpath(__file__)).parent,
+                    pydantic.UUID1: uuid1,
+                    pydantic.UUID3: lambda: uuid3(NAMESPACE_DNS, cls.__faker__.pystr()),
+                    pydantic.UUID4: cls.__faker__.uuid4,
+                    pydantic.UUID5: lambda: uuid5(NAMESPACE_DNS, cls.__faker__.pystr()),
+                    pydantic.color.Color: cls.__faker__.hex_color,  # pyright: ignore
+                }
+            )
+
     except ImportError:
         mapping = {}
 
-    with suppress(ImportError):
-        # v1 only values - these will raise an exception in v2
-        # in pydantic v2 these are all aliases for Annotated with a constraint.
-        # we therefore do not need them in v2
-        from pydantic import (
-            UUID1,
-            UUID3,
-            UUID4,
-            UUID5,
-            AmqpDsn,
-            DirectoryPath,
-            FilePath,
-            KafkaDsn,
-            PostgresDsn,
-            PyObject,
-            RedisDsn,
-        )
-
-        mapping.update(
-            {  # pyright: ignore
-                PyObject: lambda: "decimal.Decimal",
-                AmqpDsn: lambda: "amqps://example.com",
-                KafkaDsn: lambda: "kafka://localhost:9092",
-                PostgresDsn: lambda: "postgresql://user:secret@localhost",
-                RedisDsn: lambda: "redis://localhost:6379/0",
-                FilePath: lambda: Path(realpath(__file__)),
-                DirectoryPath: lambda: Path(realpath(__file__)).parent,
-                UUID1: uuid1,
-                UUID3: lambda: uuid3(NAMESPACE_DNS, cls.__faker__.pystr()),
-                UUID4: cls.__faker__.uuid4,
-                UUID5: lambda: uuid5(NAMESPACE_DNS, cls.__faker__.pystr()),
-            }
-        )
-
-    with suppress(ImportError):
-        # this might be removed by pydantic 2
-        from pydantic import color
-
-        mapping[color.Color] = cls.__faker__.hex_color  # pyright: ignore
     return mapping
 
 
 T = TypeVar("T")
 
 
 class BaseFactory(ABC, Generic[T]):
@@ -211,14 +198,26 @@
     An instance of 'random.Random' to use.
     """
     __random_seed__: ClassVar[int]
     """
     An integer to seed the factory's Faker and Random instances with.
     This attribute can be used to control random generation.
     """
+    __randomize_collection_length__: ClassVar[bool] = RANDOMIZE_COLLECTION_LENGTH
+    """
+    Flag dictating whether to randomize collections lengths.
+    """
+    __min_collection_length__: ClassVar[int] = MIN_COLLECTION_LENGTH
+    """
+    An integer value that defines minimum length of a collection.
+    """
+    __max_collection_length__: ClassVar[int] = MAX_COLLECTION_LENGTH
+    """
+    An integer value that defines maximum length of a collection.
+    """
 
     # cached attributes
     _fields_metadata: list[FieldMeta]
     # BaseFactory only attributes
     _factory_type_mapping: ClassVar[dict[Any, type[BaseFactory[Any]]]]
     _base_factories: ClassVar[list[type[BaseFactory[Any]]]]
 
@@ -227,14 +226,19 @@
 
         if not hasattr(BaseFactory, "_base_factories"):
             BaseFactory._base_factories = []
 
         if not hasattr(BaseFactory, "_factory_type_mapping"):
             BaseFactory._factory_type_mapping = {}
 
+        if cls.__min_collection_length__ > cls.__max_collection_length__:
+            raise ConfigurationException(
+                "Minimum collection length shouldn't be greater than maximum collection length"
+            )
+
         if "__is_base_factory__" not in cls.__dict__ or not cls.__is_base_factory__:
             model = getattr(cls, "__model__", None)
             if not model:
                 raise ConfigurationException(
                     f"required configuration attribute '__model__' is not set on {cls.__name__}"
                 )
             if not cls.is_supported_type(model):
@@ -602,17 +606,14 @@
 
         :returns: An arbitrary value.
 
         """
         if cls.is_ignored_type(field_meta.annotation):
             return None
 
-        if field_meta.constraints and field_meta.constraints.pop("constant", False):
-            return field_meta.default
-
         if cls.should_set_none_value(field_meta=field_meta):
             return None
 
         unwrapped_annotation = unwrap_annotation(field_meta.annotation, random=cls.__random__)
 
         if is_literal(annotation=unwrapped_annotation) and (literal_args := get_args(unwrapped_annotation)):
             return cls.__random__.choice(literal_args)
@@ -628,15 +629,18 @@
                 **(field_build_parameters if isinstance(field_build_parameters, Mapping) else {})
             )
 
         if BaseFactory.is_batch_factory_type(annotation=unwrapped_annotation):
             factory = cls._get_or_create_factory(model=field_meta.type_args[0])
             if isinstance(field_build_parameters, Sequence):
                 return [factory.build(**field_parameters) for field_parameters in field_build_parameters]
-            return factory.batch(size=cls.__random__.randint(1, 10))
+            if not cls.__randomize_collection_length__:
+                return [factory.build()]
+            batch_size = cls.__random__.randint(cls.__min_collection_length__, cls.__max_collection_length__)
+            return factory.batch(size=batch_size)
 
         if (origin := get_type_origin(unwrapped_annotation)) and issubclass(origin, Collection):
             return handle_collection_type(field_meta, origin, cls)
 
         if is_union(field_meta.annotation) and field_meta.children:
             return cls.get_field_value(cls.__random__.choice(field_meta.children))
```

### Comparing `polyfactory-2.5.0/polyfactory/factories/beanie_odm_factory.py` & `polyfactory-2.6.0/polyfactory/factories/beanie_odm_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.5.0/polyfactory/factories/dataclass_factory.py` & `polyfactory-2.6.0/polyfactory/factories/dataclass_factory.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,11 +45,14 @@
 
             fields_meta.append(
                 FieldMeta.from_type(
                     annotation=model_type_hints[field.name],
                     name=field.name,
                     default=default_value,
                     random=cls.__random__,
+                    randomize_collection_length=cls.__randomize_collection_length__,
+                    min_collection_length=cls.__min_collection_length__,
+                    max_collection_length=cls.__max_collection_length__,
                 )
             )
 
         return fields_meta
```

### Comparing `polyfactory-2.5.0/polyfactory/factories/msgspec_factory.py` & `polyfactory-2.6.0/polyfactory/factories/msgspec_factory.py`

 * *Files 23% similar despite different names*

```diff
@@ -64,11 +64,17 @@
             elif field.default_factory is not msgspec.NODEFAULT:
                 default_value = field.default_factory()
             else:
                 default_value = Null
 
             fields_meta.append(
                 FieldMeta.from_type(
-                    annotation=annotation, name=field.name, default=default_value, random=cls.__random__
+                    annotation=annotation,
+                    name=field.name,
+                    default=default_value,
+                    random=cls.__random__,
+                    randomize_collection_length=cls.__randomize_collection_length__,
+                    min_collection_length=cls.__min_collection_length__,
+                    max_collection_length=cls.__max_collection_length__,
                 )
             )
         return fields_meta
```

### Comparing `polyfactory-2.5.0/polyfactory/factories/odmantic_odm_factory.py` & `polyfactory-2.6.0/polyfactory/factories/odmantic_odm_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.5.0/polyfactory/factories/pydantic_factory.py` & `polyfactory-2.6.0/polyfactory/factories/pydantic_factory.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,57 +2,64 @@
 
 from contextlib import suppress
 from typing import (
     TYPE_CHECKING,
     Any,
     ClassVar,
     Generic,
-    Literal,
     Mapping,
+    Tuple,
     TypeVar,
     cast,
 )
 
+from typing_extensions import Literal, get_args, get_origin
+
+from polyfactory.collection_extender import CollectionExtender
+from polyfactory.constants import MAX_COLLECTION_LENGTH, MIN_COLLECTION_LENGTH, RANDOMIZE_COLLECTION_LENGTH
 from polyfactory.exceptions import MissingDependencyException
 from polyfactory.factories.base import BaseFactory
 from polyfactory.field_meta import Constraints, FieldMeta, Null
 from polyfactory.utils.helpers import unwrap_new_type, unwrap_optional
 from polyfactory.utils.predicates import is_optional_union, is_safe_subclass
 
 try:
-    from pydantic import BaseModel
+    from pydantic import VERSION, BaseModel
     from pydantic.fields import FieldInfo
 except ImportError as e:
     raise MissingDependencyException("pydantic is not installed") from e
 
 try:
     from pydantic.fields import ModelField  # type: ignore[attr-defined]
 
-    pydantic_version: Literal[1, 2] = 1
 except ImportError:
-    pydantic_version = 2
-
     ModelField = Any
     from pydantic_core import PydanticUndefined as Undefined
 
 if TYPE_CHECKING:
     from random import Random
 
     from typing_extensions import TypeGuard
 
-
 T = TypeVar("T", bound=BaseModel)
 
 
 class PydanticFieldMeta(FieldMeta):
     """Field meta subclass capable of handling pydantic ModelFields"""
 
     @classmethod
     def from_field_info(
-        cls, field_name: str, field_info: FieldInfo, use_alias: bool, random: Random
+        cls,
+        field_name: str,
+        field_info: FieldInfo,
+        use_alias: bool,
+        random: Random,
+        randomize_collection_length: bool = RANDOMIZE_COLLECTION_LENGTH,
+        min_collection_length: int = MIN_COLLECTION_LENGTH,
+        max_collection_length: int = MAX_COLLECTION_LENGTH,
     ) -> PydanticFieldMeta:
         """Create an instance from a pydantic field info.
 
         :param field_name: The name of the field.
         :param field_info: A pydantic FieldInfo instance.
         :param use_alias: Whether to use the field alias.
         :param random: A random.Random instance.
@@ -84,32 +91,47 @@
 
         return PydanticFieldMeta.from_type(
             name=name,
             random=random,
             annotation=annotation,
             default=default_value,
             constraints=cast("Constraints", {k: v for k, v in constraints.items() if v is not None}) or None,
+            randomize_collection_length=randomize_collection_length,
+            min_collection_length=min_collection_length,
+            max_collection_length=max_collection_length,
         )
 
     @classmethod
-    def from_model_field(
-        cls, model_field: ModelField, use_alias: bool  # pyright: ignore
-    ) -> PydanticFieldMeta:  # pragma: no cover
+    def from_model_field(  # pragma: no cover
+        cls,
+        model_field: ModelField,  # pyright: ignore
+        use_alias: bool,
+        random: Random,
+        randomize_collection_length: bool,
+        min_collection_length: int,
+        max_collection_length: int,
+    ) -> PydanticFieldMeta:
         """Create an instance from a pydantic model field.
 
         :param model_field: A pydantic ModelField.
         :param use_alias: Whether to use the field alias.
+        :param random: An instance of random.Random.
+        :param randomize_collection_length: A boolean flag whether to randomize collections lengths
+        :param min_collection_length: Minimum number of elements in randomized collection
+        :param max_collection_length: Maximum number of elements in randomized collection
 
         :returns: A PydanticFieldMeta instance.
 
         """
         from pydantic import AmqpDsn, AnyHttpUrl, AnyUrl, HttpUrl, KafkaDsn, PostgresDsn, RedisDsn
         from pydantic.fields import DeferredType, Undefined  # type: ignore
 
-        if callable(model_field.default_factory):
+        if model_field.default is not Undefined:
+            default_value = model_field.default
+        elif callable(model_field.default_factory):
             default_value = model_field.default_factory()
         else:
             default_value = model_field.default if model_field.default is not Undefined else Null
 
         name = model_field.alias if model_field.alias and use_alias else model_field.name
 
         outer_type = unwrap_new_type(model_field.outer_type_)
@@ -118,15 +140,14 @@
             if isinstance(model_field.annotation, DeferredType)
             else unwrap_new_type(model_field.annotation)
         )
 
         constraints = cast(
             "Constraints",
             {
-                "constant": bool(model_field.field_info.const) or None,
                 "ge": getattr(outer_type, "ge", model_field.field_info.ge),
                 "gt": getattr(outer_type, "gt", model_field.field_info.gt),
                 "le": getattr(outer_type, "le", model_field.field_info.le),
                 "lt": getattr(outer_type, "lt", model_field.field_info.lt),
                 "min_length": (
                     getattr(outer_type, "min_length", model_field.field_info.min_length)
                     or getattr(outer_type, "min_items", model_field.field_info.min_items)
@@ -143,38 +164,70 @@
                 "upper_case": getattr(outer_type, "to_upper", None),
                 "lower_case": getattr(outer_type, "to_lower", None),
                 "item_type": getattr(outer_type, "item_type", None),
             },
         )
 
         # pydantic v1 has constraints set for these values, but we generate them using faker
-        if pydantic_version == 1 and unwrap_optional(annotation) in (
+        if unwrap_optional(annotation) in (
             AnyUrl,
             HttpUrl,
             KafkaDsn,
             PostgresDsn,
             RedisDsn,
             AmqpDsn,
             AnyHttpUrl,
         ):
             constraints = {}
 
+        if model_field.field_info.const and (
+            default_value is None or isinstance(default_value, (int, bool, str, bytes))
+        ):
+            annotation = Literal[default_value]  # pyright: ignore
+
         children: list[FieldMeta] = []
-        if model_field.key_field:
-            children.append(PydanticFieldMeta.from_model_field(model_field.key_field, use_alias))
-        if model_field.sub_fields:
+        if model_field.key_field or model_field.sub_fields:
+            number_of_args = (
+                random.randint(min_collection_length, max_collection_length) if randomize_collection_length else 1
+            )
+            fields_to_iterate = (
+                ([model_field.key_field, *model_field.sub_fields])
+                if model_field.key_field is not None
+                else model_field.sub_fields
+            )
+            type_args = tuple(
+                (
+                    sub_field.outer_type_
+                    if isinstance(sub_field.annotation, DeferredType)
+                    else unwrap_new_type(sub_field.annotation)
+                )
+                for sub_field in fields_to_iterate
+            )
+            type_arg_to_sub_field = dict(zip(type_args, fields_to_iterate))
+            if get_origin(outer_type) in (tuple, Tuple) and get_args(outer_type)[-1] == Ellipsis:
+                # pydantic removes ellipses from Tuples in sub_fields
+                type_args += (...,)
+            extended_type_args = CollectionExtender.extend_type_args(annotation, type_args, number_of_args)
             children.extend(
-                PydanticFieldMeta.from_model_field(sub_field, use_alias) for sub_field in model_field.sub_fields
+                PydanticFieldMeta.from_model_field(
+                    type_arg_to_sub_field[arg],
+                    use_alias,
+                    random,
+                    randomize_collection_length,
+                    min_collection_length,
+                    max_collection_length,
+                )
+                for arg in extended_type_args
             )
 
         return PydanticFieldMeta(
             name=name,
             random=cls.random,
             annotation=annotation,
-            children=children,
+            children=children or None,
             default=default_value,
             constraints=cast("Constraints", {k: v for k, v in constraints.items() if v is not None}) or None,
         )
 
 
 class ModelFactory(Generic[T], BaseFactory[T]):
     """Base factory for pydantic models"""
@@ -203,29 +256,36 @@
         """Retrieve a list of fields from the factory's model.
 
 
         :returns: A list of field MetaData instances.
 
         """
         if "_fields_metadata" not in cls.__dict__:
-            if pydantic_version == 1:
+            if VERSION.startswith("1"):
                 cls._fields_metadata = [
                     PydanticFieldMeta.from_model_field(
                         field,
                         use_alias=not cls.__model__.__config__.allow_population_by_field_name,
+                        random=cls.__random__,
+                        randomize_collection_length=cls.__randomize_collection_length__,
+                        min_collection_length=cls.__min_collection_length__,
+                        max_collection_length=cls.__max_collection_length__,
                     )
                     for field in cls.__model__.__fields__.values()  # type: ignore[attr-defined]
                 ]
             else:
                 cls._fields_metadata = [
                     PydanticFieldMeta.from_field_info(
                         field_info=field_info,
                         field_name=field_name,
                         random=cls.__random__,
                         use_alias=not cls.__model__.model_config.get("populate_by_name", False),
+                        randomize_collection_length=cls.__randomize_collection_length__,
+                        min_collection_length=cls.__min_collection_length__,
+                        max_collection_length=cls.__max_collection_length__,
                     )
                     for field_name, field_info in cls.__model__.model_fields.items()
                 ]
         return cls._fields_metadata
 
     @classmethod
     def build(cls, factory_use_construct: bool = False, **kwargs: Any) -> T:
```

### Comparing `polyfactory-2.5.0/polyfactory/factories/typed_dict_factory.py` & `polyfactory-2.6.0/polyfactory/factories/typed_dict_factory.py`

 * *Files 20% similar despite different names*

```diff
@@ -36,11 +36,14 @@
 
         fields_meta: list["FieldMeta"] = [
             FieldMeta.from_type(
                 annotation=annotation,
                 random=cls.__random__,
                 name=field_name,
                 default=getattr(cls.__model__, field_name, Null),
+                randomize_collection_length=cls.__randomize_collection_length__,
+                min_collection_length=cls.__min_collection_length__,
+                max_collection_length=cls.__max_collection_length__,
             )
             for field_name, annotation in model_type_hints.items()
         ]
         return fields_meta
```

### Comparing `polyfactory-2.5.0/polyfactory/field_meta.py` & `polyfactory-2.6.0/polyfactory/field_meta.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 from __future__ import annotations
 
 from dataclasses import asdict, is_dataclass
 from typing import TYPE_CHECKING, Any, Literal, Pattern, TypedDict, cast
 
-from polyfactory.constants import DEFAULT_RANDOM, IGNORED_TYPE_ARGS, TYPE_MAPPING
+from polyfactory.collection_extender import CollectionExtender
+from polyfactory.constants import (
+    DEFAULT_RANDOM,
+    MAX_COLLECTION_LENGTH,
+    MIN_COLLECTION_LENGTH,
+    RANDOMIZE_COLLECTION_LENGTH,
+    TYPE_MAPPING,
+)
 from polyfactory.utils.helpers import normalize_annotation, unwrap_annotated, unwrap_args, unwrap_new_type
 from polyfactory.utils.predicates import is_annotated
 
 if TYPE_CHECKING:
     import datetime
     from random import Random
 
@@ -28,15 +35,14 @@
     default_path: NotRequired[str]
 
 
 class Constraints(TypedDict):
     """Metadata regarding a type constraints, if any"""
 
     allow_inf_nan: NotRequired[bool]
-    constant: NotRequired[bool]
     decimal_places: NotRequired[int]
     ge: NotRequired[int | float | Decimal]
     gt: NotRequired[int | float | Decimal]
     item_type: NotRequired[Any]
     le: NotRequired[int | float | Decimal]
     lower_case: NotRequired[bool]
     lt: NotRequired[int | float | Decimal]
@@ -85,32 +91,41 @@
 
     @property
     def type_args(self) -> tuple[Any, ...]:
         """Return the normalized type args of the annotation, if any.
 
         :returns: a tuple of types.
         """
-        return tuple(arg for arg in unwrap_args(self.annotation, random=self.random) if arg not in IGNORED_TYPE_ARGS)
+        return tuple(
+            TYPE_MAPPING[arg] if arg in TYPE_MAPPING else arg
+            for arg in unwrap_args(self.annotation, random=self.random)
+        )
 
     @classmethod
     def from_type(
         cls,
         annotation: Any,
         random: Random = DEFAULT_RANDOM,
         name: str = "",
         default: Any = Null,
         constraints: Constraints | None = None,
+        randomize_collection_length: bool = RANDOMIZE_COLLECTION_LENGTH,
+        min_collection_length: int = MIN_COLLECTION_LENGTH,
+        max_collection_length: int = MAX_COLLECTION_LENGTH,
     ) -> Self:
         """Builder method to create a FieldMeta from a type annotation.
 
         :param annotation: A type annotation.
         :param random: An instance of random.Random.
         :param name: Field name
         :param default: Default value, if any.
         :param constraints: A dictionary of constraints, if any.
+        :param randomize_collection_length: A boolean flag whether to randomize collections lengths
+        :param min_collection_length: Minimum number of elements in randomized collection
+        :param max_collection_length: Maximum number of elements in randomized collection
 
         :returns: A field meta instance.
         """
         field_type = normalize_annotation(annotation, random=random)
 
         if not constraints and is_annotated(annotation):
             _, metadata = unwrap_annotated(annotation, random=random)
@@ -121,16 +136,28 @@
             random=random,
             name=name,
             default=default,
             children=None,
             constraints=constraints,
         )
         if field.type_args:
+            if randomize_collection_length:
+                number_of_args = random.randint(min_collection_length, max_collection_length)
+            else:
+                number_of_args = 1
+            extended_type_args = CollectionExtender.extend_type_args(field.annotation, field.type_args, number_of_args)
             field.children = [
-                FieldMeta.from_type(annotation=unwrap_new_type(arg), random=random) for arg in field.type_args
+                FieldMeta.from_type(
+                    annotation=unwrap_new_type(arg),
+                    random=random,
+                    randomize_collection_length=randomize_collection_length,
+                    min_collection_length=min_collection_length,
+                    max_collection_length=max_collection_length,
+                )
+                for arg in extended_type_args
             ]
         return field
 
     @classmethod
     def parse_constraints(cls, metadata: list[Any]) -> "Constraints":
         constraints = {}
 
@@ -151,15 +178,14 @@
                 constraints["url"] = {k: v for k, v in value_dict.items() if v is not None}
             else:
                 constraints.update(
                     {
                         k: v
                         for k, v in {
                             "allow_inf_nan": getattr(value, "allow_inf_nan", None),
-                            "constant": getattr(value, "const", None) is not None,
                             "decimal_places": getattr(value, "decimal_places", None),
                             "ge": getattr(value, "ge", None),
                             "gt": getattr(value, "gt", None),
                             "item_type": getattr(value, "item_type", None),
                             "le": getattr(value, "le", None),
                             "lower_case": getattr(value, "to_lower", None),
                             "lt": getattr(value, "lt", None),
```

### Comparing `polyfactory-2.5.0/polyfactory/fields.py` & `polyfactory-2.6.0/polyfactory/fields.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.5.0/polyfactory/persistence.py` & `polyfactory-2.6.0/polyfactory/persistence.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.5.0/polyfactory/pytest_plugin.py` & `polyfactory-2.6.0/polyfactory/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.5.0/polyfactory/utils/helpers.py` & `polyfactory-2.6.0/polyfactory/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.5.0/polyfactory/utils/predicates.py` & `polyfactory-2.6.0/polyfactory/utils/predicates.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,23 @@
     return (
         annotation is Any
         or getattr(annotation, "_name", "") == "typing.Any"
         or (get_origin(annotation) in UNION_TYPES and Any in get_args(annotation))
     )
 
 
+def is_dict_key_or_value_type(annotation: Any) -> "TypeGuard[Any]":
+    """Determine whether a given annotation is a valid dict key or value type:
+    ``typing.KT`` or ``typing.VT``.
+
+    :returns: A typeguard.
+    """
+    return str(annotation) in {"~KT", "~VT"}
+
+
 def is_union(annotation: Any) -> "TypeGuard[Any | Any]":
     """Determine whether a given annotation is 'typing.Union'.
 
     :param annotation: A type annotation.
 
     :returns: A typeguard.
     """
```

### Comparing `polyfactory-2.5.0/polyfactory/value_generators/complex_types.py` & `polyfactory-2.6.0/polyfactory/value_generators/complex_types.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,27 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, AbstractSet, Any, MutableMapping, MutableSequence, Set
+from typing import (
+    TYPE_CHECKING,
+    AbstractSet,
+    Any,
+    Iterable,
+    MutableMapping,
+    MutableSequence,
+    Set,
+    Tuple,
+    cast,
+)
 
 from typing_extensions import is_typeddict
 
+from polyfactory.field_meta import FieldMeta
+
 if TYPE_CHECKING:
     from polyfactory.factories.base import BaseFactory
-    from polyfactory.field_meta import FieldMeta
 
 
 def handle_collection_type(field_meta: FieldMeta, container_type: type, factory: type[BaseFactory[Any]]) -> Any:
     """Handle generation of container types recursively.
 
     :param container_type: A type that can accept type arguments.
     :param factory: A factory.
@@ -19,27 +30,32 @@
     :returns: A built result.
     """
     container = container_type()
     if not field_meta.children:
         return container
 
     if issubclass(container_type, MutableMapping) or is_typeddict(container_type):
-        key = factory.get_field_value(field_meta.children[0])
-        value = factory.get_field_value(field_meta.children[1])
-        container[key] = value
-
-    elif issubclass(container_type, MutableSequence):
-        container.append(factory.get_field_value(field_meta.children[0]))
+        for key_field_meta, value_field_meta in cast(
+            Iterable[Tuple[FieldMeta, FieldMeta]], zip(field_meta.children[::2], field_meta.children[1::2])
+        ):
+            key = factory.get_field_value(key_field_meta)
+            value = factory.get_field_value(value_field_meta)
+            container[key] = value
+        return container
 
-    elif issubclass(container_type, Set):
-        container.add(factory.get_field_value(field_meta.children[0]))
+    if issubclass(container_type, MutableSequence):
+        for subfield_meta in field_meta.children:
+            container.append(factory.get_field_value(subfield_meta))
+        return container
 
-    elif issubclass(container_type, AbstractSet):
-        container = container.union(handle_collection_type(field_meta, set, factory))
+    if issubclass(container_type, Set):
+        for subfield_meta in field_meta.children:
+            container.add(factory.get_field_value(subfield_meta))
+        return container
 
-    elif issubclass(container_type, tuple):
-        container = container_type(map(factory.get_field_value, field_meta.children))
+    if issubclass(container_type, AbstractSet):
+        return container.union(handle_collection_type(field_meta, set, factory))
 
-    else:
-        raise NotImplementedError(f"Unsupported container type: {container_type}")
+    if issubclass(container_type, tuple):
+        return container_type(map(factory.get_field_value, field_meta.children))
 
-    return container
+    raise NotImplementedError(f"Unsupported container type: {container_type}")
```

### Comparing `polyfactory-2.5.0/polyfactory/value_generators/constrained_collections.py` & `polyfactory-2.6.0/polyfactory/value_generators/constrained_collections.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.5.0/polyfactory/value_generators/constrained_dates.py` & `polyfactory-2.6.0/polyfactory/value_generators/constrained_dates.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.5.0/polyfactory/value_generators/constrained_numbers.py` & `polyfactory-2.6.0/polyfactory/value_generators/constrained_numbers.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.5.0/polyfactory/value_generators/constrained_strings.py` & `polyfactory-2.6.0/polyfactory/value_generators/constrained_strings.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.5.0/polyfactory/value_generators/primitives.py` & `polyfactory-2.6.0/polyfactory/value_generators/primitives.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.5.0/polyfactory/value_generators/regex.py` & `polyfactory-2.6.0/polyfactory/value_generators/regex.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.5.0/pyproject.toml` & `polyfactory-2.6.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 [tool.poetry]
 name = "polyfactory"
-version = "2.5.0"
+version = "2.6.0"
 description = "Mock data generation factories"
 authors = [
     "Na'aman Hirschfeld <nhirschfeld@gmail.com>",
-    "Peter Schutt <peter.github@proton.me>",
     "Cody Fincher <cody.fincher@gmail.com>",
     "Janek Nouvertné <provinzkraut@posteo.de>",
     "Jacob Coffee <jacob@z7x.org>",
 ]
 maintainers = [
     "Na'aman Hirschfeld <nhirschfeld@gmail.com>",
-    "Peter Schutt <peter.github@proton.me>",
     "Cody Fincher <cody.fincher@gmail.com>",
     "Janek Nouvertné <provinzkraut@posteo.de>",
     "Jacob Coffee <jacob@z7x.org>",
 ]
 license = "MIT"
 readme = "docs/PYPI_README.md"
 homepage = "https://github.com/litestar-org/polyfactory"
@@ -64,35 +62,36 @@
 faker = "*"
 msgspec = { version = "*", optional = true }
 odmantic = { version = "*", optional = true }
 pydantic = { version = "*", optional = true }
 typing-extensions = "*"
 
 [tool.poetry.group.dev.dependencies]
+annotated-types = "*"
 beanie = "*"
 email-validator = "*"
 hypothesis = "*"
 mongomock-motor = "*"
-msgspec = "*"
+msgspec = { git = "https://github.com/jcrist/msgspec.git", branch = "main" }
 odmantic = "*"
 pre-commit = "*"
-pydantic = "*"
+pydantic = { git = "https://github.com/pydantic/pydantic", branch = "main" }
 pytest = "*"
 pytest-asyncio = "*"
 pytest-cov = "*"
-annotated-types = "*"
+sourcery = "*"
 
 [tool.poetry.group.docs.dependencies]
-sphinx-autobuild = "*"
-blacken-docs = "*"
 auto-pytabs = "*"
-sphinxcontrib-mermaid = "*"
-sphinx-copybutton = "*"
-sphinx = "*"
+blacken-docs = "*"
 litestar-sphinx-theme = { git = "https://github.com/litestar-org/litestar-sphinx-theme.git" }
+sphinx = "*"
+sphinx-autobuild = "*"
+sphinx-copybutton = "*"
+sphinxcontrib-mermaid = "*"
 
 [tool.poetry.extras]
 pydantic = ["pydantic"]
 msgspec = ["msgspec"]
 odmantic = ["odmantic", "pydantic"]
 beanie = ["beanie", "pydantic"]
 
@@ -177,14 +176,15 @@
     "D106", # pydocstyle - missing docstring in public nested class
     "D107", # pydocstyle - missing docstring in __init__
     "D202", # pydocstyle - no blank lines allowed after function docstring
     "D205", # pydocstyle - 1 blank line required between summary line and description
     "D415", # pydocstyle - first line should end with a period, question mark, or exclamation point
     "E501", # pycodestyle line too long, handled by black
     "N818", # pep8-naming - exception name should be named with an Error suffix
+    "S311", # flake8-bandit - Standard pseudo-random generators are not suitable for security/cryptographic purposes
     "UP037", # pyupgrade - removes quotes from type annotation
 ]
 line-length = 120
 src = ["polyfactory", "tests", "docs/examples"]
 target-version = "py38"
 
 [tool.ruff.pydocstyle]
```

### Comparing `polyfactory-2.5.0/PKG-INFO` & `polyfactory-2.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyfactory
-Version: 2.5.0
+Version: 2.6.0
 Summary: Mock data generation factories
 Home-page: https://github.com/litestar-org/polyfactory
 License: MIT
 Keywords: beanie,dataclasses,factory,faker,litestar,mock,msgspec,odmantic,pydantic,pytest,tdd,testing,typeddict
 Author: Na'aman Hirschfeld
 Author-email: nhirschfeld@gmail.com
 Maintainer: Na'aman Hirschfeld
```

