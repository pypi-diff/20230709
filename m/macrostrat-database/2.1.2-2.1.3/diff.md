# Comparing `tmp/macrostrat_database-2.1.2.tar.gz` & `tmp/macrostrat_database-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrostrat_database-2.1.2.tar", max compression
+gzip compressed data, was "macrostrat_database-2.1.3.tar", max compression
```

## Comparing `macrostrat_database-2.1.2.tar` & `macrostrat_database-2.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     5975 2023-04-11 05:06:58.495410 macrostrat_database-2.1.2/macrostrat/database/__init__.py
--rw-r--r--   0        0        0     4665 2023-04-11 04:58:29.434832 macrostrat_database-2.1.2/macrostrat/database/mapper/__init__.py
--rw-r--r--   0        0        0      686 2022-05-26 00:55:15.936699 macrostrat_database-2.1.2/macrostrat/database/mapper/base.py
--rw-r--r--   0        0        0     2272 2022-05-26 05:21:07.121385 macrostrat_database-2.1.2/macrostrat/database/mapper/cache.py
--rw-r--r--   0        0        0     3271 2023-04-11 05:06:58.496060 macrostrat_database-2.1.2/macrostrat/database/mapper/utils.py
--rw-r--r--   0        0        0     1630 2022-05-26 00:55:15.936016 macrostrat_database-2.1.2/macrostrat/database/postgresql.py
--rw-r--r--   0        0        0    14193 2023-05-16 20:02:34.748416 macrostrat_database-2.1.2/macrostrat/database/utils.py
--rw-r--r--   0        0        0      598 2023-05-16 20:02:34.748658 macrostrat_database-2.1.2/pyproject.toml
--rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 macrostrat_database-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0     5975 2023-04-11 05:06:58.495410 macrostrat_database-2.1.3/macrostrat/database/__init__.py
+-rw-r--r--   0        0        0     4719 2023-07-09 03:49:31.995548 macrostrat_database-2.1.3/macrostrat/database/mapper/__init__.py
+-rw-r--r--   0        0        0      686 2022-05-26 00:55:15.936699 macrostrat_database-2.1.3/macrostrat/database/mapper/base.py
+-rw-r--r--   0        0        0     2272 2022-05-26 05:21:07.121385 macrostrat_database-2.1.3/macrostrat/database/mapper/cache.py
+-rw-r--r--   0        0        0     3271 2023-04-11 05:06:58.496060 macrostrat_database-2.1.3/macrostrat/database/mapper/utils.py
+-rw-r--r--   0        0        0     1630 2022-05-26 00:55:15.936016 macrostrat_database-2.1.3/macrostrat/database/postgresql.py
+-rw-r--r--   0        0        0    14193 2023-05-16 20:02:34.748416 macrostrat_database-2.1.3/macrostrat/database/utils.py
+-rw-r--r--   0        0        0      597 2023-07-09 03:49:31.996224 macrostrat_database-2.1.3/pyproject.toml
+-rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 macrostrat_database-2.1.3/PKG-INFO
```

### Comparing `macrostrat_database-2.1.2/macrostrat/database/__init__.py` & `macrostrat_database-2.1.3/macrostrat/database/__init__.py`

 * *Files identical despite different names*

### Comparing `macrostrat_database-2.1.2/macrostrat/database/mapper/__init__.py` & `macrostrat_database-2.1.3/macrostrat/database/mapper/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
 
 class DatabaseMapper:
     automap_base = BaseModel
     automap_error = None
     _models = None
     _tables = None
+    _prepared = False
 
     def __init__(self, db, **kwargs):
         # https://docs.sqlalchemy.org/en/13/orm/extensions/automap.html#sqlalchemy.ext.automap.AutomapBase.prepare
         # TODO: add the process flow described below:
         # https://docs.sqlalchemy.org/en/13/orm/extensions/automap.html#generating-mappings-from-an-existing-metadata
         self.db = db
 
@@ -78,23 +79,26 @@
             log.info("Database models for %s have been loaded from cache", schema)
             self.automap_base.prepare(
                 self.db.engine, schema=schema, **self.reflection_kwargs
             )
             return
         log.info(f"Reflecting schema {schema}")
         if schema == "public":
+            schema = None
+        if not self._prepared:
             self.automap_base.prepare(
-                self.db.engine, reflect=True, schema=None, **self.reflection_kwargs
-            )
-        else:
-            # Reflect tables in schemas we care about
-            # Note: this will not reflect views because they don't have primary keys.
-            self.automap_base.metadata.reflect(
-                bind=self.db.engine, schema=schema, **self.reflection_kwargs
+                self.db.engine, reflect=False, **self.reflection_kwargs
             )
+            self._prepared = True
+        # Reflect tables in schemas we care about
+        # Note: this will not reflect views because they don't have primary keys.
+        self.automap_base.metadata.reflect(
+            bind=self.db.engine,
+            schema=schema,
+        )
         self._models = ModelCollection(self.automap_base.classes)
         self._tables = TableCollection(self._models)
 
     def reflect_table(self, tablename, *column_args, **kwargs):
         # Warn that this method is deprecated
         warn(
             "DatabaseMapper.reflect_table is deprecated. Use Database.reflect_table instead",
```

### Comparing `macrostrat_database-2.1.2/macrostrat/database/mapper/base.py` & `macrostrat_database-2.1.3/macrostrat/database/mapper/base.py`

 * *Files identical despite different names*

### Comparing `macrostrat_database-2.1.2/macrostrat/database/mapper/cache.py` & `macrostrat_database-2.1.3/macrostrat/database/mapper/cache.py`

 * *Files identical despite different names*

### Comparing `macrostrat_database-2.1.2/macrostrat/database/mapper/utils.py` & `macrostrat_database-2.1.3/macrostrat/database/mapper/utils.py`

 * *Files identical despite different names*

### Comparing `macrostrat_database-2.1.2/macrostrat/database/postgresql.py` & `macrostrat_database-2.1.3/macrostrat/database/postgresql.py`

 * *Files identical despite different names*

### Comparing `macrostrat_database-2.1.2/macrostrat/database/utils.py` & `macrostrat_database-2.1.3/macrostrat/database/utils.py`

 * *Files identical despite different names*

### Comparing `macrostrat_database-2.1.2/pyproject.toml` & `macrostrat_database-2.1.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 [tool.poetry]
 authors = ["Daven Quinn <dev@davenquinn.com>"]
 description = "A SQLAlchemy-based database toolkit."
 name = "macrostrat.database"
-packages = [
-  {include = "macrostrat"},
-]
-version = "2.1.2"
+packages = [{ include = "macrostrat" }]
+version = "2.1.3"
 
 [tool.poetry.dependencies]
 GeoAlchemy2 = "^0.9.4"
 SQLAlchemy = "^1.4.26"
 SQLAlchemy-Utils = "^0.37.0"
 click = "^8.1.3"
 "macrostrat.utils" = "^1.0.0"
 psycopg2-binary = "^2.9.1"
 python = "^3.8"
 sqlparse = "^0.4.0"
 
 [tool.poetry.dev-dependencies]
-"macrostrat.utils" = {path = "../utils", develop = true}
+"macrostrat.utils" = { path = "../utils", develop = true }
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `macrostrat_database-2.1.2/PKG-INFO` & `macrostrat_database-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrostrat-database
-Version: 2.1.2
+Version: 2.1.3
 Summary: A SQLAlchemy-based database toolkit.
 Author: Daven Quinn
 Author-email: dev@davenquinn.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

