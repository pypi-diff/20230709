# Comparing `tmp/macrostrat_database-3.0.0.dev1.tar.gz` & `tmp/macrostrat_database-3.0.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrostrat_database-3.0.0.dev1.tar", max compression
+gzip compressed data, was "macrostrat_database-3.0.0.dev2.tar", max compression
```

## Comparing `macrostrat_database-3.0.0.dev1.tar` & `macrostrat_database-3.0.0.dev2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     5917 2023-07-09 06:43:10.650928 macrostrat_database-3.0.0.dev1/macrostrat/database/__init__.py
--rw-r--r--   0        0        0     4719 2023-07-09 03:49:31.995548 macrostrat_database-3.0.0.dev1/macrostrat/database/mapper/__init__.py
--rw-r--r--   0        0        0      686 2022-05-26 00:55:15.936699 macrostrat_database-3.0.0.dev1/macrostrat/database/mapper/base.py
--rw-r--r--   0        0        0     2272 2022-05-26 05:21:07.121385 macrostrat_database-3.0.0.dev1/macrostrat/database/mapper/cache.py
--rw-r--r--   0        0        0     3271 2023-04-11 05:06:58.496060 macrostrat_database-3.0.0.dev1/macrostrat/database/mapper/utils.py
--rw-r--r--   0        0        0     1630 2022-05-26 00:55:15.936016 macrostrat_database-3.0.0.dev1/macrostrat/database/postgresql.py
--rw-r--r--   0        0        0    14453 2023-07-09 06:43:10.651242 macrostrat_database-3.0.0.dev1/macrostrat/database/utils.py
--rw-r--r--   0        0        0      603 2023-07-09 06:43:10.652705 macrostrat_database-3.0.0.dev1/pyproject.toml
--rw-r--r--   0        0        0      762 1970-01-01 00:00:00.000000 macrostrat_database-3.0.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0     5917 2023-07-09 06:43:10.650928 macrostrat_database-3.0.0.dev2/macrostrat/database/__init__.py
+-rw-r--r--   0        0        0     4411 2023-07-09 06:48:00.909017 macrostrat_database-3.0.0.dev2/macrostrat/database/mapper/__init__.py
+-rw-r--r--   0        0        0      686 2022-05-26 00:55:15.936699 macrostrat_database-3.0.0.dev2/macrostrat/database/mapper/base.py
+-rw-r--r--   0        0        0     2272 2022-05-26 05:21:07.121385 macrostrat_database-3.0.0.dev2/macrostrat/database/mapper/cache.py
+-rw-r--r--   0        0        0     3271 2023-04-11 05:06:58.496060 macrostrat_database-3.0.0.dev2/macrostrat/database/mapper/utils.py
+-rw-r--r--   0        0        0     1630 2022-05-26 00:55:15.936016 macrostrat_database-3.0.0.dev2/macrostrat/database/postgresql.py
+-rw-r--r--   0        0        0    14453 2023-07-09 06:43:10.651242 macrostrat_database-3.0.0.dev2/macrostrat/database/utils.py
+-rw-r--r--   0        0        0      603 2023-07-09 06:48:38.687047 macrostrat_database-3.0.0.dev2/pyproject.toml
+-rw-r--r--   0        0        0      762 1970-01-01 00:00:00.000000 macrostrat_database-3.0.0.dev2/PKG-INFO
```

### Comparing `macrostrat_database-3.0.0.dev1/macrostrat/database/__init__.py` & `macrostrat_database-3.0.0.dev2/macrostrat/database/__init__.py`

 * *Files identical despite different names*

### Comparing `macrostrat_database-3.0.0.dev1/macrostrat/database/mapper/__init__.py` & `macrostrat_database-3.0.0.dev2/macrostrat/database/mapper/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,24 +80,16 @@
             self.automap_base.prepare(
                 self.db.engine, schema=schema, **self.reflection_kwargs
             )
             return
         log.info(f"Reflecting schema {schema}")
         if schema == "public":
             schema = None
-        if not self._prepared:
-            self.automap_base.prepare(
-                self.db.engine, reflect=False, **self.reflection_kwargs
-            )
-            self._prepared = True
-        # Reflect tables in schemas we care about
-        # Note: this will not reflect views because they don't have primary keys.
-        self.automap_base.metadata.reflect(
-            bind=self.db.engine,
-            schema=schema,
+        self.automap_base.prepare(
+            self.db.engine, reflect=False, schema=schema, **self.reflection_kwargs
         )
         self._models = ModelCollection(self.automap_base.classes)
         self._tables = TableCollection(self._models)
 
     def reflect_table(self, tablename, *column_args, **kwargs):
         # Warn that this method is deprecated
         warn(
```

### Comparing `macrostrat_database-3.0.0.dev1/macrostrat/database/mapper/base.py` & `macrostrat_database-3.0.0.dev2/macrostrat/database/mapper/base.py`

 * *Files identical despite different names*

### Comparing `macrostrat_database-3.0.0.dev1/macrostrat/database/mapper/cache.py` & `macrostrat_database-3.0.0.dev2/macrostrat/database/mapper/cache.py`

 * *Files identical despite different names*

### Comparing `macrostrat_database-3.0.0.dev1/macrostrat/database/mapper/utils.py` & `macrostrat_database-3.0.0.dev2/macrostrat/database/mapper/utils.py`

 * *Files identical despite different names*

### Comparing `macrostrat_database-3.0.0.dev1/macrostrat/database/postgresql.py` & `macrostrat_database-3.0.0.dev2/macrostrat/database/postgresql.py`

 * *Files identical despite different names*

### Comparing `macrostrat_database-3.0.0.dev1/macrostrat/database/utils.py` & `macrostrat_database-3.0.0.dev2/macrostrat/database/utils.py`

 * *Files identical despite different names*

### Comparing `macrostrat_database-3.0.0.dev1/pyproject.toml` & `macrostrat_database-3.0.0.dev2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 authors = ["Daven Quinn <dev@davenquinn.com>"]
 description = "A SQLAlchemy-based database toolkit."
 name = "macrostrat.database"
 packages = [{ include = "macrostrat" }]
-version = "3.0.0-dev1"
+version = "3.0.0-dev2"
 
 [tool.poetry.dependencies]
 GeoAlchemy2 = "^0.14.0"
 SQLAlchemy = "^2.0.18"
 SQLAlchemy-Utils = "^0.41.1"
 click = "^8.1.3"
 "macrostrat.utils" = "^1.0.0"
```

### Comparing `macrostrat_database-3.0.0.dev1/PKG-INFO` & `macrostrat_database-3.0.0.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrostrat-database
-Version: 3.0.0.dev1
+Version: 3.0.0.dev2
 Summary: A SQLAlchemy-based database toolkit.
 Author: Daven Quinn
 Author-email: dev@davenquinn.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

