# Comparing `tmp/auto_dataclass-0.1.4.tar.gz` & `tmp/auto_dataclass-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_dataclass-0.1.4.tar", last modified: Sun Jul  9 11:59:55 2023, max compression
+gzip compressed data, was "auto_dataclass-0.1.5.tar", last modified: Sun Jul  9 12:49:45 2023, max compression
```

## Comparing `auto_dataclass-0.1.4.tar` & `auto_dataclass-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      733 2023-06-26 10:45:19.360030 auto_dataclass-0.1.4/.github/workflows/tests.yml
--rw-r--r--   0        0        0       34 2023-06-26 13:42:13.912977 auto_dataclass-0.1.4/.gitignore
--rw-r--r--   0        0        0     1083 2023-06-26 10:54:50.375568 auto_dataclass-0.1.4/LICENSE
--rw-r--r--   0        0        0     3398 2023-06-30 05:52:53.057973 auto_dataclass-0.1.4/README.md
--rw-r--r--   0        0        0      106 2023-07-09 11:24:45.393572 auto_dataclass-0.1.4/auto_dataclass/__init__.py
--rw-r--r--   0        0        0     5290 2023-07-09 11:50:05.167991 auto_dataclass-0.1.4/auto_dataclass/dj_model_to_dataclass.py
--rw-r--r--   0        0        0      150 2023-07-07 06:32:16.675179 auto_dataclass-0.1.4/auto_dataclass/exceptions.py
--rw-r--r--   0        0        0     4582 2023-06-26 10:25:32.846753 auto_dataclass-0.1.4/poetry.lock
--rw-r--r--   0        0        0      682 2023-06-26 13:56:04.307932 auto_dataclass-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     6824 2023-07-07 06:32:16.687179 auto_dataclass-0.1.4/tests/tests_errors.py
--rw-r--r--   0        0        0     4248 2023-07-09 11:51:10.171923 auto_dataclass-0.1.4/tests/tests_to_dto_func.py
--rw-r--r--   0        0        0     4120 2023-07-07 06:12:51.136314 auto_dataclass-0.1.4/tests/tests_to_dto_func_with_recursive.py
--rw-r--r--   0        0        0     3760 1970-01-01 00:00:00.000000 auto_dataclass-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      733 2023-06-26 10:45:19.360030 auto_dataclass-0.1.5/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       34 2023-06-26 13:42:13.912977 auto_dataclass-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1083 2023-06-26 10:54:50.375568 auto_dataclass-0.1.5/LICENSE
+-rw-r--r--   0        0        0     3398 2023-06-30 05:52:53.057973 auto_dataclass-0.1.5/README.md
+-rw-r--r--   0        0        0      106 2023-07-09 12:49:05.591772 auto_dataclass-0.1.5/auto_dataclass/__init__.py
+-rw-r--r--   0        0        0     5530 2023-07-09 12:49:01.091778 auto_dataclass-0.1.5/auto_dataclass/dj_model_to_dataclass.py
+-rw-r--r--   0        0        0      150 2023-07-07 06:32:16.675179 auto_dataclass-0.1.5/auto_dataclass/exceptions.py
+-rw-r--r--   0        0        0     4582 2023-06-26 10:25:32.846753 auto_dataclass-0.1.5/poetry.lock
+-rw-r--r--   0        0        0      682 2023-06-26 13:56:04.307932 auto_dataclass-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     6824 2023-07-07 06:32:16.687179 auto_dataclass-0.1.5/tests/tests_errors.py
+-rw-r--r--   0        0        0     4941 2023-07-09 12:18:41.210179 auto_dataclass-0.1.5/tests/tests_to_dto_func.py
+-rw-r--r--   0        0        0     4120 2023-07-07 06:12:51.136314 auto_dataclass-0.1.5/tests/tests_to_dto_func_with_recursive.py
+-rw-r--r--   0        0        0     3760 1970-01-01 00:00:00.000000 auto_dataclass-0.1.5/PKG-INFO
```

### Comparing `auto_dataclass-0.1.4/.github/workflows/tests.yml` & `auto_dataclass-0.1.5/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `auto_dataclass-0.1.4/LICENSE` & `auto_dataclass-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_dataclass-0.1.4/README.md` & `auto_dataclass-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `auto_dataclass-0.1.4/auto_dataclass/dj_model_to_dataclass.py` & `auto_dataclass-0.1.5/auto_dataclass/dj_model_to_dataclass.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,28 +45,34 @@
                 elif is_dataclass(origin_type) and field_data is not None:
                     obj_for_dataclass[field.name] = self._get_dataclass_object(
                         field_data, origin_type
                     )
                 else:
                     obj_for_dataclass[field.name] = field_data
             else:
-                if field.default is dataclasses.MISSING:
-                    raise ConversionError(
-                        f"Field name '{field.name}' doesn't exist in {data}"
-                    )
-                obj_for_dataclass[field.name] = field.default
+                obj_for_dataclass[field.name] = self._get_default_value_or_error(field, data)
 
         return dc(**obj_for_dataclass)
 
     @staticmethod
     def _is_field_name_exists_in_data(data: Model, field: dataclasses.Field) -> bool | None:
         if hasattr(data, field.name):
             return True
         return False
 
+    @staticmethod
+    def _get_default_value_or_error(field: dataclasses.Field, data: Model):
+        if field.default is dataclasses.MISSING:
+            if field.default_factory is dataclasses.MISSING:
+                raise ConversionError(
+                    f"Field name '{field.name}' doesn't exist in {data}"
+                )
+            return field.default_factory()
+        return field.default
+
     def _get_origin_field_type(self, field_type):
         is_list = False
         origin_type = get_origin(field_type)
         if origin_type is Union or origin_type is UnionType:
             field_type = field_type.__args__[0]
         if hasattr(field_type, "__origin__") and field_type.__origin__ is list:
             field_type = field_type.__args__[0]
```

### Comparing `auto_dataclass-0.1.4/poetry.lock` & `auto_dataclass-0.1.5/poetry.lock`

 * *Files identical despite different names*

### Comparing `auto_dataclass-0.1.4/pyproject.toml` & `auto_dataclass-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `auto_dataclass-0.1.4/tests/tests_errors.py` & `auto_dataclass-0.1.5/tests/tests_errors.py`

 * *Files identical despite different names*

### Comparing `auto_dataclass-0.1.4/tests/tests_to_dto_func.py` & `auto_dataclass-0.1.5/tests/tests_to_dto_func.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import List
 from unittest import TestCase
 from unittest.mock import Mock, MagicMock
 
 from django.db.models import Model
 
 from auto_dataclass.dj_model_to_dataclass import FromOrmToDataclass
@@ -108,14 +108,35 @@
 
         mock_model = Mock(spec=Model)
         result = self.converter.to_dto(mock_model, OuterTestDataclass)
 
         self.assertIsInstance(result, OuterTestDataclass)
         self.assertEqual(result.dc, None)
 
+    def test_to_dto_list_of_python_types_with_default_value(self) -> None:
+        @dataclass
+        class TestDataclass:
+            id: int
+            name: List[str] = field(default_factory=list)
+
+        @dataclass
+        class OuterTestDataclass:
+            dc: TestDataclass
+
+        mock_model_with_list = Mock(spec=Model)
+        mock_model_with_list.id = 1
+        mock_model = Mock(spec=Model)
+        mock_model.dc = mock_model_with_list
+
+        result = self.converter.to_dto(mock_model, OuterTestDataclass)
+
+        self.assertIsInstance(result, OuterTestDataclass)
+        self.assertIsInstance(result.dc, TestDataclass)
+        self.assertEqual(result.dc.name, [])
+
     @staticmethod
     def get_db_model_object():
         model = Mock(spec=Model)
         model.id = 1
         model.name = "first"
         return model
```

### Comparing `auto_dataclass-0.1.4/tests/tests_to_dto_func_with_recursive.py` & `auto_dataclass-0.1.5/tests/tests_to_dto_func_with_recursive.py`

 * *Files identical despite different names*

### Comparing `auto_dataclass-0.1.4/PKG-INFO` & `auto_dataclass-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto_dataclass
-Version: 0.1.4
+Version: 0.1.5
 Summary: The package, helps to automatically transform data to DTO (DataClass) object
 Author-email: Oleksandr Zhydyk <zhydykalex@ukr.net>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Home, https://github.com/OleksandrZhydyk/Auto-Dataclass.git
 
 ## Auto dataclass
```

