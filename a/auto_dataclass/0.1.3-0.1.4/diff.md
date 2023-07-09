# Comparing `tmp/auto_dataclass-0.1.3.tar.gz` & `tmp/auto_dataclass-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_dataclass-0.1.3.tar", last modified: Fri Jul  7 07:17:17 2023, max compression
+gzip compressed data, was "auto_dataclass-0.1.4.tar", last modified: Sun Jul  9 11:59:55 2023, max compression
```

## Comparing `auto_dataclass-0.1.3.tar` & `auto_dataclass-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      733 2023-06-26 10:45:19.360030 auto_dataclass-0.1.3/.github/workflows/tests.yml
--rw-r--r--   0        0        0       34 2023-06-26 13:42:13.912977 auto_dataclass-0.1.3/.gitignore
--rw-r--r--   0        0        0     1083 2023-06-26 10:54:50.375568 auto_dataclass-0.1.3/LICENSE
--rw-r--r--   0        0        0     3398 2023-06-30 05:52:53.057973 auto_dataclass-0.1.3/README.md
--rw-r--r--   0        0        0      106 2023-07-07 07:17:11.863140 auto_dataclass-0.1.3/auto_dataclass/__init__.py
--rw-r--r--   0        0        0     5091 2023-07-07 07:15:22.971138 auto_dataclass-0.1.3/auto_dataclass/dj_model_to_dataclass.py
--rw-r--r--   0        0        0      150 2023-07-07 06:32:16.675179 auto_dataclass-0.1.3/auto_dataclass/exceptions.py
--rw-r--r--   0        0        0     4582 2023-06-26 10:25:32.846753 auto_dataclass-0.1.3/poetry.lock
--rw-r--r--   0        0        0      682 2023-06-26 13:56:04.307932 auto_dataclass-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     6824 2023-07-07 06:32:16.687179 auto_dataclass-0.1.3/tests/tests_errors.py
--rw-r--r--   0        0        0     3809 2023-07-07 07:13:49.279129 auto_dataclass-0.1.3/tests/tests_to_dto_func.py
--rw-r--r--   0        0        0     4120 2023-07-07 06:12:51.136314 auto_dataclass-0.1.3/tests/tests_to_dto_func_with_recursive.py
--rw-r--r--   0        0        0     3760 1970-01-01 00:00:00.000000 auto_dataclass-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      733 2023-06-26 10:45:19.360030 auto_dataclass-0.1.4/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       34 2023-06-26 13:42:13.912977 auto_dataclass-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1083 2023-06-26 10:54:50.375568 auto_dataclass-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3398 2023-06-30 05:52:53.057973 auto_dataclass-0.1.4/README.md
+-rw-r--r--   0        0        0      106 2023-07-09 11:24:45.393572 auto_dataclass-0.1.4/auto_dataclass/__init__.py
+-rw-r--r--   0        0        0     5290 2023-07-09 11:50:05.167991 auto_dataclass-0.1.4/auto_dataclass/dj_model_to_dataclass.py
+-rw-r--r--   0        0        0      150 2023-07-07 06:32:16.675179 auto_dataclass-0.1.4/auto_dataclass/exceptions.py
+-rw-r--r--   0        0        0     4582 2023-06-26 10:25:32.846753 auto_dataclass-0.1.4/poetry.lock
+-rw-r--r--   0        0        0      682 2023-06-26 13:56:04.307932 auto_dataclass-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     6824 2023-07-07 06:32:16.687179 auto_dataclass-0.1.4/tests/tests_errors.py
+-rw-r--r--   0        0        0     4248 2023-07-09 11:51:10.171923 auto_dataclass-0.1.4/tests/tests_to_dto_func.py
+-rw-r--r--   0        0        0     4120 2023-07-07 06:12:51.136314 auto_dataclass-0.1.4/tests/tests_to_dto_func_with_recursive.py
+-rw-r--r--   0        0        0     3760 1970-01-01 00:00:00.000000 auto_dataclass-0.1.4/PKG-INFO
```

### Comparing `auto_dataclass-0.1.3/.github/workflows/tests.yml` & `auto_dataclass-0.1.4/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `auto_dataclass-0.1.3/LICENSE` & `auto_dataclass-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_dataclass-0.1.3/README.md` & `auto_dataclass-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `auto_dataclass-0.1.3/auto_dataclass/dj_model_to_dataclass.py` & `auto_dataclass-0.1.4/auto_dataclass/dj_model_to_dataclass.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,38 +29,43 @@
         self._check_future_dataclasses_arg(future_dataclasses)
         checked_data = self._is_data_dj_model_type(data)
         return self._to_dataclass_obj(checked_data, checked_dc)
 
     def _to_dataclass_obj(self, data: Model, dc: dataclass) -> dataclass:
         obj_for_dataclass = {}
         for field in dataclasses.fields(dc):
-            if self._is_field_name_exists_in_data(data, field.name):
+            if self._is_field_name_exists_in_data(data, field):
 
                 field_data = getattr(data, field.name)
                 origin_type, is_list = self._get_origin_field_type(field.type)
 
                 if is_list and is_dataclass(origin_type) and field_data is not None:
                     obj_for_dataclass[field.name] = self._get_list_of_dataclass_objects(
                         field_data, origin_type
                     )
                 elif is_dataclass(origin_type) and field_data is not None:
                     obj_for_dataclass[field.name] = self._get_dataclass_object(
                         field_data, origin_type
                     )
                 else:
                     obj_for_dataclass[field.name] = field_data
+            else:
+                if field.default is dataclasses.MISSING:
+                    raise ConversionError(
+                        f"Field name '{field.name}' doesn't exist in {data}"
+                    )
+                obj_for_dataclass[field.name] = field.default
+
         return dc(**obj_for_dataclass)
 
     @staticmethod
-    def _is_field_name_exists_in_data(data: Model, field_name: str) -> bool | None:
-        if hasattr(data, field_name):
+    def _is_field_name_exists_in_data(data: Model, field: dataclasses.Field) -> bool | None:
+        if hasattr(data, field.name):
             return True
-        raise ConversionError(
-            f"Field name '{field_name}' doesn't exist in {data}"
-        )
+        return False
 
     def _get_origin_field_type(self, field_type):
         is_list = False
         origin_type = get_origin(field_type)
         if origin_type is Union or origin_type is UnionType:
             field_type = field_type.__args__[0]
         if hasattr(field_type, "__origin__") and field_type.__origin__ is list:
```

### Comparing `auto_dataclass-0.1.3/poetry.lock` & `auto_dataclass-0.1.4/poetry.lock`

 * *Files identical despite different names*

### Comparing `auto_dataclass-0.1.3/pyproject.toml` & `auto_dataclass-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `auto_dataclass-0.1.3/tests/tests_errors.py` & `auto_dataclass-0.1.4/tests/tests_errors.py`

 * *Files identical despite different names*

### Comparing `auto_dataclass-0.1.3/tests/tests_to_dto_func.py` & `auto_dataclass-0.1.4/tests/tests_to_dto_func.py`

 * *Files 11% similar despite different names*

```diff
@@ -95,14 +95,27 @@
         mock_model = Mock(spec=Model)
         mock_model.dc = self.get_db_model_object()
         result = self.converter.to_dto(mock_model, OuterTestDataclass)
 
         self.assertIsInstance(result, OuterTestDataclass)
         self.assertEqual(result.dc, InnerTestDataclass(id=1, name="first"))
 
+    def test__to_dto_db_related_object_or_none_default_value(self) -> None:
+        InnerTestDataclass = self.TestDataclass
+
+        @dataclass
+        class OuterTestDataclass:
+            dc: InnerTestDataclass | None = None
+
+        mock_model = Mock(spec=Model)
+        result = self.converter.to_dto(mock_model, OuterTestDataclass)
+
+        self.assertIsInstance(result, OuterTestDataclass)
+        self.assertEqual(result.dc, None)
+
     @staticmethod
     def get_db_model_object():
         model = Mock(spec=Model)
         model.id = 1
         model.name = "first"
         return model
```

### Comparing `auto_dataclass-0.1.3/tests/tests_to_dto_func_with_recursive.py` & `auto_dataclass-0.1.4/tests/tests_to_dto_func_with_recursive.py`

 * *Files identical despite different names*

### Comparing `auto_dataclass-0.1.3/PKG-INFO` & `auto_dataclass-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto_dataclass
-Version: 0.1.3
+Version: 0.1.4
 Summary: The package, helps to automatically transform data to DTO (DataClass) object
 Author-email: Oleksandr Zhydyk <zhydykalex@ukr.net>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Home, https://github.com/OleksandrZhydyk/Auto-Dataclass.git
 
 ## Auto dataclass
```

