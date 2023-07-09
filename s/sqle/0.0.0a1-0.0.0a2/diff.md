# Comparing `tmp/sqle-0.0.0a1.tar.gz` & `tmp/sqle-0.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqle-0.0.0a1.tar", max compression
+gzip compressed data, was "sqle-0.0.0a2.tar", max compression
```

## Comparing `sqle-0.0.0a1.tar` & `sqle-0.0.0a2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1063 2023-04-13 11:39:12.312030 sqle-0.0.0a1/LICENSE
--rw-r--r--   0        0        0      150 2023-04-15 12:19:38.626033 sqle-0.0.0a1/README.md
--rw-r--r--   0        0        0      454 2023-05-11 13:05:52.210381 sqle-0.0.0a1/pyproject.toml
--rw-r--r--   0        0        0      146 2023-05-11 13:05:41.995233 sqle-0.0.0a1/sqle/__init__.py
--rw-r--r--   0        0        0     3116 2023-05-11 12:53:41.995931 sqle-0.0.0a1/sqle/adapter.py
--rw-r--r--   0        0        0        0 2023-03-11 12:58:20.091961 sqle-0.0.0a1/sqle/contrib/__init__.py
--rw-r--r--   0        0        0      150 2023-03-08 11:10:17.217492 sqle-0.0.0a1/sqle/contrib/class_property.py
--rw-r--r--   0        0        0      157 2023-04-12 15:49:20.785386 sqle-0.0.0a1/sqle/contrib/text.py
--rw-r--r--   0        0        0      435 2023-04-08 13:03:01.529379 sqle-0.0.0a1/sqle/exceptions.py
--rw-r--r--   0        0        0     2331 2023-04-15 12:21:27.817079 sqle-0.0.0a1/sqle/query.py
--rw-r--r--   0        0        0       46 2023-02-15 15:56:29.472877 sqle-0.0.0a1/sqle/settings.py
--rw-r--r--   0        0        0     3166 2023-04-15 12:21:27.830628 sqle-0.0.0a1/sqle/sql.py
--rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 sqle-0.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-13 11:39:12.312030 sqle-0.0.0a2/LICENSE
+-rw-r--r--   0        0        0      150 2023-04-15 12:19:38.626033 sqle-0.0.0a2/README.md
+-rw-r--r--   0        0        0      454 2023-07-09 07:49:20.710527 sqle-0.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0      146 2023-07-09 07:49:52.998354 sqle-0.0.0a2/sqle/__init__.py
+-rw-r--r--   0        0        0     5925 2023-07-09 08:34:29.591957 sqle-0.0.0a2/sqle/adapter.py
+-rw-r--r--   0        0        0        0 2023-03-11 12:58:20.091961 sqle-0.0.0a2/sqle/contrib/__init__.py
+-rw-r--r--   0        0        0      150 2023-03-08 11:10:17.217492 sqle-0.0.0a2/sqle/contrib/class_property.py
+-rw-r--r--   0        0        0      157 2023-04-12 15:49:20.785386 sqle-0.0.0a2/sqle/contrib/text.py
+-rw-r--r--   0        0        0      435 2023-04-08 13:03:01.529379 sqle-0.0.0a2/sqle/exceptions.py
+-rw-r--r--   0        0        0     2331 2023-04-15 12:21:27.817079 sqle-0.0.0a2/sqle/query.py
+-rw-r--r--   0        0        0       46 2023-02-15 15:56:29.472877 sqle-0.0.0a2/sqle/settings.py
+-rw-r--r--   0        0        0     3162 2023-07-09 06:36:36.016572 sqle-0.0.0a2/sqle/sql.py
+-rw-r--r--   0        0        0      222 2023-06-02 16:29:51.580146 sqle-0.0.0a2/sqle/sqle-sqlite.code-workspace
+-rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 sqle-0.0.0a2/PKG-INFO
```

### Comparing `sqle-0.0.0a1/LICENSE` & `sqle-0.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `sqle-0.0.0a1/sqle/query.py` & `sqle-0.0.0a2/sqle/query.py`

 * *Files identical despite different names*

### Comparing `sqle-0.0.0a1/sqle/sql.py` & `sqle-0.0.0a2/sqle/sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,18 +65,18 @@
             **params,
         }
 
     # Factory
 
     @classmethod
     def create_instance(
-        cls,
+        cls: Type[T],
         name: str = SQL_ENVIRONMENT_DEFAULT_INSTANCE_NAME,
         **connection_factories: Callable,
-    ) -> Type[SQLEnvironment]:
+    ) -> Type[T]:
         sql_environment_instance = type(name, cls.__bases__, dict(cls.__dict__))
 
         for adapter_name, adapter_factory in cls.adapters.items():
             connection_factory = connection_factories.get(adapter_name)
 
             if not connection_factory and not cls.get_default_adapter(adapter_name):
                 raise TSQLValueError(
```

### Comparing `sqle-0.0.0a1/PKG-INFO` & `sqle-0.0.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqle
-Version: 0.0.0a1
+Version: 0.0.0a2
 Summary: 
 License: MIT
 Author: acrius
 Author-email: acrius@mail.ru
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

