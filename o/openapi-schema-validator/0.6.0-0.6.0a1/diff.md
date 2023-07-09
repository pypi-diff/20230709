# Comparing `tmp/openapi_schema_validator-0.6.0.tar.gz` & `tmp/openapi_schema_validator-0.6.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapi_schema_validator-0.6.0.tar", max compression
+gzip compressed data, was "openapi_schema_validator-0.6.0a1.tar", max compression
```

## Comparing `openapi_schema_validator-0.6.0.tar` & `openapi_schema_validator-0.6.0a1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1509 2023-07-09 11:13:34.814132 openapi_schema_validator-0.6.0/LICENSE
--rw-r--r--   0        0        0     4076 2023-07-09 11:13:34.814132 openapi_schema_validator-0.6.0/README.rst
--rw-r--r--   0        0        0      829 2023-07-09 11:13:34.814132 openapi_schema_validator-0.6.0/openapi_schema_validator/__init__.py
--rw-r--r--   0        0        0     2483 2023-07-09 11:13:34.814132 openapi_schema_validator-0.6.0/openapi_schema_validator/_format.py
--rw-r--r--   0        0        0      697 2023-07-09 11:13:34.814132 openapi_schema_validator-0.6.0/openapi_schema_validator/_types.py
--rw-r--r--   0        0        0     8173 2023-07-09 11:13:34.814132 openapi_schema_validator-0.6.0/openapi_schema_validator/_validators.py
--rw-r--r--   0        0        0        0 2023-07-09 11:13:34.814132 openapi_schema_validator-0.6.0/openapi_schema_validator/py.typed
--rw-r--r--   0        0        0      590 2023-07-09 11:13:34.814132 openapi_schema_validator-0.6.0/openapi_schema_validator/shortcuts.py
--rw-r--r--   0        0        0     3732 2023-07-09 11:13:34.814132 openapi_schema_validator-0.6.0/openapi_schema_validator/validators.py
--rw-r--r--   0        0        0     2270 2023-07-09 11:13:34.814132 openapi_schema_validator-0.6.0/pyproject.toml
--rw-r--r--   0        0        0    27167 2023-07-09 11:13:34.814132 openapi_schema_validator-0.6.0/tests/integration/test_validators.py
--rw-r--r--   0        0        0      615 2023-07-09 11:13:34.814132 openapi_schema_validator-0.6.0/tests/unit/test_shortcut.py
--rw-r--r--   0        0        0     5253 1970-01-01 00:00:00.000000 openapi_schema_validator-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1509 2023-06-13 18:14:06.484796 openapi_schema_validator-0.6.0a1/LICENSE
+-rw-r--r--   0        0        0     4076 2023-06-13 18:14:06.488796 openapi_schema_validator-0.6.0a1/README.rst
+-rw-r--r--   0        0        0      831 2023-06-13 18:14:06.488796 openapi_schema_validator-0.6.0a1/openapi_schema_validator/__init__.py
+-rw-r--r--   0        0        0     2483 2023-06-13 18:14:06.488796 openapi_schema_validator-0.6.0a1/openapi_schema_validator/_format.py
+-rw-r--r--   0        0        0      697 2023-06-13 18:14:06.488796 openapi_schema_validator-0.6.0a1/openapi_schema_validator/_types.py
+-rw-r--r--   0        0        0     8173 2023-06-13 18:14:06.488796 openapi_schema_validator-0.6.0a1/openapi_schema_validator/_validators.py
+-rw-r--r--   0        0        0        0 2023-06-13 18:14:06.488796 openapi_schema_validator-0.6.0a1/openapi_schema_validator/py.typed
+-rw-r--r--   0        0        0      590 2023-06-13 18:14:06.488796 openapi_schema_validator-0.6.0a1/openapi_schema_validator/shortcuts.py
+-rw-r--r--   0        0        0     3732 2023-06-13 18:14:06.488796 openapi_schema_validator-0.6.0a1/openapi_schema_validator/validators.py
+-rw-r--r--   0        0        0     2302 2023-06-13 18:14:06.488796 openapi_schema_validator-0.6.0a1/pyproject.toml
+-rw-r--r--   0        0        0    25624 2023-06-13 18:14:06.488796 openapi_schema_validator-0.6.0a1/tests/integration/test_validators.py
+-rw-r--r--   0        0        0      615 2023-06-13 18:14:06.488796 openapi_schema_validator-0.6.0a1/tests/unit/test_shortcut.py
+-rw-r--r--   0        0        0     5257 1970-01-01 00:00:00.000000 openapi_schema_validator-0.6.0a1/PKG-INFO
```

### Comparing `openapi_schema_validator-0.6.0/LICENSE` & `openapi_schema_validator-0.6.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi_schema_validator-0.6.0/README.rst` & `openapi_schema_validator-0.6.0a1/README.rst`

 * *Files identical despite different names*

### Comparing `openapi_schema_validator-0.6.0/openapi_schema_validator/__init__.py` & `openapi_schema_validator-0.6.0a1/openapi_schema_validator/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from openapi_schema_validator.validators import OAS30ReadValidator
 from openapi_schema_validator.validators import OAS30Validator
 from openapi_schema_validator.validators import OAS30WriteValidator
 from openapi_schema_validator.validators import OAS31Validator
 
 __author__ = "Artur Maciag"
 __email__ = "maciag.artur@gmail.com"
-__version__ = "0.6.0"
+__version__ = "0.6.0a1"
 __url__ = "https://github.com/python-openapi/openapi-schema-validator"
 __license__ = "3-clause BSD License"
 
 __all__ = [
     "validate",
     "OAS30ReadValidator",
     "OAS30WriteValidator",
```

### Comparing `openapi_schema_validator-0.6.0/openapi_schema_validator/_format.py` & `openapi_schema_validator-0.6.0a1/openapi_schema_validator/_format.py`

 * *Files identical despite different names*

### Comparing `openapi_schema_validator-0.6.0/openapi_schema_validator/_types.py` & `openapi_schema_validator-0.6.0a1/openapi_schema_validator/_types.py`

 * *Files identical despite different names*

### Comparing `openapi_schema_validator-0.6.0/openapi_schema_validator/_validators.py` & `openapi_schema_validator-0.6.0a1/openapi_schema_validator/_validators.py`

 * *Files identical despite different names*

### Comparing `openapi_schema_validator-0.6.0/openapi_schema_validator/shortcuts.py` & `openapi_schema_validator-0.6.0a1/openapi_schema_validator/shortcuts.py`

 * *Files identical despite different names*

### Comparing `openapi_schema_validator-0.6.0/openapi_schema_validator/validators.py` & `openapi_schema_validator-0.6.0a1/openapi_schema_validator/validators.py`

 * *Files identical despite different names*

### Comparing `openapi_schema_validator-0.6.0/pyproject.toml` & `openapi_schema_validator-0.6.0a1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 [tool.coverage.run]
 branch = true
 source =["openapi_schema_validator"]
 
 [tool.coverage.xml]
 output = "reports/coverage.xml"
 
-[tool.deptry.per_rule_ignores]
-DEP002 = ["rfc3339-validator"]
+[tool.deptry]
+ignore_unused = ["rfc3339-validator"]
 
 [tool.mypy]
 files = "openapi_schema_validator"
 strict = true
 
 [[tool.mypy.overrides]]
 module = "jsonschema.*"
@@ -26,15 +26,15 @@
 
 [[tool.mypy.overrides]]
 module = "rfc3339_validator"
 ignore_missing_imports = true
 
 [tool.poetry]
 name = "openapi-schema-validator"
-version = "0.6.0"
+version = "0.6.0a1"
 description = "OpenAPI schema validation for Python"
 authors = ["Artur Maciag <maciag.artur@gmail.com>"]
 license = "BSD-3-Clause"
 readme = "README.rst"
 repository = "https://github.com/python-openapi/openapi-schema-validator"
 keywords = ["openapi", "swagger", "schema"]
 classifiers = [
@@ -51,31 +51,31 @@
 ]
 include = [
     {path = "tests", format = "sdist"},
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8.0"
-jsonschema = "^4.18.0"
+jsonschema = {version = "^4.18.0a1", allow-prereleases = true}
 rfc3339-validator = "*" # requred by jsonschema for date-time checker
 jsonschema-specifications = "^2023.5.2"
 
 [tool.poetry.extras]
 docs = ["sphinx", "sphinx-immaterial"]
 
 [tool.poetry.dev-dependencies]
 black = "^23.3.0"
 isort = "^5.9.1"
 pre-commit = "*"
 pytest = "^7"
 pytest-flake8 = "*"
 pytest-cov = "*"
-mypy = "^1.4"
+mypy = "^1.3"
 flynt = "^0.78"
-deptry = "^0.12.0"
+deptry = "^0.11.0"
 
 [tool.poetry.group.docs.dependencies]
 sphinx = ">=5.3,<8.0"
 sphinx-immaterial = "^0.11.0"
 
 [tool.pytest.ini_options]
 addopts = """
```

### Comparing `openapi_schema_validator-0.6.0/tests/integration/test_validators.py` & `openapi_schema_validator-0.6.0a1/tests/integration/test_validators.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 from base64 import b64encode
 
 import pytest
 from jsonschema import ValidationError
-from referencing import Registry
-from referencing import Resource
-from referencing.jsonschema import DRAFT202012
 
 from openapi_schema_validator import OAS30ReadValidator
 from openapi_schema_validator import OAS30Validator
 from openapi_schema_validator import OAS30WriteValidator
 from openapi_schema_validator import OAS31Validator
 from openapi_schema_validator import oas30_format_checker
 from openapi_schema_validator import oas31_format_checker
@@ -97,59 +94,14 @@
     def test_string_invalid(self, validator_class, value):
         schema = {"type": "string"}
         validator = validator_class(schema)
 
         with pytest.raises(ValidationError):
             validator.validate(value)
 
-    def test_referencing(self, validator_class):
-        name_schema = Resource.from_contents(
-            {
-                "$schema": "https://json-schema.org/draft/2020-12/schema",
-                "type": "string",
-            }
-        )
-        age_schema = DRAFT202012.create_resource(
-            {
-                "type": "integer",
-                "format": "int32",
-                "minimum": 0,
-                "maximum": 120,
-            }
-        )
-        birth_date_schema = Resource.from_contents(
-            {
-                "type": "string",
-                "format": "date",
-            },
-            default_specification=DRAFT202012,
-        )
-        registry = Registry().with_resources(
-            [
-                ("urn:name-schema", name_schema),
-                ("urn:age-schema", age_schema),
-                ("urn:birth-date-schema", birth_date_schema),
-            ],
-        )
-        schema = {
-            "type": "object",
-            "required": ["name"],
-            "properties": {
-                "name": {"$ref": "urn:name-schema"},
-                "age": {"$ref": "urn:age-schema"},
-                "birth-date": {"$ref": "urn:birth-date-schema"},
-            },
-            "additionalProperties": False,
-        }
-
-        validator = validator_class(schema, registry=registry)
-        result = validator.validate({"name": "John", "age": 23}, schema)
-
-        assert result is None
-
 
 class TestOAS30ValidatorValidate(BaseTestOASValidatorValidate):
     @pytest.fixture
     def validator_class(self):
         return OAS30Validator
 
     @pytest.fixture
```

### Comparing `openapi_schema_validator-0.6.0/tests/unit/test_shortcut.py` & `openapi_schema_validator-0.6.0a1/tests/unit/test_shortcut.py`

 * *Files identical despite different names*

### Comparing `openapi_schema_validator-0.6.0/PKG-INFO` & `openapi_schema_validator-0.6.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapi-schema-validator
-Version: 0.6.0
+Version: 0.6.0a1
 Summary: OpenAPI schema validation for Python
 Home-page: https://github.com/python-openapi/openapi-schema-validator
 License: BSD-3-Clause
 Keywords: openapi,swagger,schema
 Author: Artur Maciag
 Author-email: maciag.artur@gmail.com
 Requires-Python: >=3.8.0,<4.0.0
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: docs
-Requires-Dist: jsonschema (>=4.18.0,<5.0.0)
+Requires-Dist: jsonschema (>=4.18.0a1,<5.0.0)
 Requires-Dist: jsonschema-specifications (>=2023.5.2,<2024.0.0)
 Requires-Dist: rfc3339-validator
 Project-URL: Repository, https://github.com/python-openapi/openapi-schema-validator
 Description-Content-Type: text/x-rst
 
 ************************
 openapi-schema-validator
```

