# Comparing `tmp/macrostrat_database-2.1.3.tar.gz` & `tmp/macrostrat_database-3.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrostrat_database-2.1.3.tar", max compression
+gzip compressed data, was "macrostrat_database-3.0.0.dev1.tar", max compression
```

## Comparing `macrostrat_database-2.1.3.tar` & `macrostrat_database-3.0.0.dev1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     5975 2023-04-11 05:06:58.495410 macrostrat_database-2.1.3/macrostrat/database/__init__.py
--rw-r--r--   0        0        0     4719 2023-07-09 03:49:31.995548 macrostrat_database-2.1.3/macrostrat/database/mapper/__init__.py
--rw-r--r--   0        0        0      686 2022-05-26 00:55:15.936699 macrostrat_database-2.1.3/macrostrat/database/mapper/base.py
--rw-r--r--   0        0        0     2272 2022-05-26 05:21:07.121385 macrostrat_database-2.1.3/macrostrat/database/mapper/cache.py
--rw-r--r--   0        0        0     3271 2023-04-11 05:06:58.496060 macrostrat_database-2.1.3/macrostrat/database/mapper/utils.py
--rw-r--r--   0        0        0     1630 2022-05-26 00:55:15.936016 macrostrat_database-2.1.3/macrostrat/database/postgresql.py
--rw-r--r--   0        0        0    14193 2023-05-16 20:02:34.748416 macrostrat_database-2.1.3/macrostrat/database/utils.py
--rw-r--r--   0        0        0      597 2023-07-09 03:49:31.996224 macrostrat_database-2.1.3/pyproject.toml
--rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 macrostrat_database-2.1.3/PKG-INFO
+-rw-r--r--   0        0        0     5917 2023-07-09 06:43:10.650928 macrostrat_database-3.0.0.dev1/macrostrat/database/__init__.py
+-rw-r--r--   0        0        0     4719 2023-07-09 03:49:31.995548 macrostrat_database-3.0.0.dev1/macrostrat/database/mapper/__init__.py
+-rw-r--r--   0        0        0      686 2022-05-26 00:55:15.936699 macrostrat_database-3.0.0.dev1/macrostrat/database/mapper/base.py
+-rw-r--r--   0        0        0     2272 2022-05-26 05:21:07.121385 macrostrat_database-3.0.0.dev1/macrostrat/database/mapper/cache.py
+-rw-r--r--   0        0        0     3271 2023-04-11 05:06:58.496060 macrostrat_database-3.0.0.dev1/macrostrat/database/mapper/utils.py
+-rw-r--r--   0        0        0     1630 2022-05-26 00:55:15.936016 macrostrat_database-3.0.0.dev1/macrostrat/database/postgresql.py
+-rw-r--r--   0        0        0    14453 2023-07-09 06:43:10.651242 macrostrat_database-3.0.0.dev1/macrostrat/database/utils.py
+-rw-r--r--   0        0        0      603 2023-07-09 06:43:10.652705 macrostrat_database-3.0.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0      762 1970-01-01 00:00:00.000000 macrostrat_database-3.0.0.dev1/PKG-INFO
```

### Comparing `macrostrat_database-2.1.3/macrostrat/database/__init__.py` & `macrostrat_database-3.0.0.dev1/macrostrat/database/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,28 +26,26 @@
 
 class Database(object):
     mapper: Optional[DatabaseMapper] = None
     metadata: MetaData
     session: Session
     __inspector__ = None
 
-    def __init__(self, db_conn, app=None, echo_sql=False, **kwargs):
+    def __init__(self, db_conn, echo_sql=False, **kwargs):
         """
         We can pass a connection string, a **Flask** application object
         with the appropriate configuration, or nothing, in which
         case we will try to infer the correct database from
         the SPARROW_BACKEND_CONFIG file, if available.
         """
 
         compiles(Insert, "postgresql")(prefix_inserts)
 
         log.info(f"Setting up database connection '{db_conn}'")
-        self.engine = create_engine(
-            db_conn, executemany_mode="batch", echo=echo_sql, **kwargs
-        )
+        self.engine = create_engine(db_conn, echo=echo_sql, **kwargs)
         self.metadata = kwargs.get("metadata", metadata)
 
         # Scoped session for database
         # https://docs.sqlalchemy.org/en/13/orm/contextual.html#unitofwork-contextual
         # https://docs.sqlalchemy.org/en/13/orm/session_basics.html#session-faq-whentocreate
         self._session_factory = sessionmaker(bind=self.engine)
         self.session = scoped_session(self._session_factory)
```

### Comparing `macrostrat_database-2.1.3/macrostrat/database/mapper/__init__.py` & `macrostrat_database-3.0.0.dev1/macrostrat/database/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `macrostrat_database-2.1.3/macrostrat/database/mapper/base.py` & `macrostrat_database-3.0.0.dev1/macrostrat/database/mapper/base.py`

 * *Files identical despite different names*

### Comparing `macrostrat_database-2.1.3/macrostrat/database/mapper/cache.py` & `macrostrat_database-3.0.0.dev1/macrostrat/database/mapper/cache.py`

 * *Files identical despite different names*

### Comparing `macrostrat_database-2.1.3/macrostrat/database/mapper/utils.py` & `macrostrat_database-3.0.0.dev1/macrostrat/database/mapper/utils.py`

 * *Files identical despite different names*

### Comparing `macrostrat_database-2.1.3/macrostrat/database/postgresql.py` & `macrostrat_database-3.0.0.dev1/macrostrat/database/postgresql.py`

 * *Files identical despite different names*

### Comparing `macrostrat_database-2.1.3/macrostrat/database/utils.py` & `macrostrat_database-3.0.0.dev1/macrostrat/database/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from click import echo, secho
 from sqlalchemy.exc import ProgrammingError, IntegrityError, InternalError
 from sqlparse import split, format
 from sqlalchemy.sql import ClauseElement
 from sqlalchemy.orm import sessionmaker, Session
 from sqlalchemy.engine import Engine, Connection, Transaction
 from sqlalchemy.schema import Table
-from sqlalchemy import MetaData, create_engine, text
+from sqlalchemy import MetaData, create_engine, TextClause, text
 from contextlib import contextmanager
 from sqlalchemy_utils import create_database, database_exists, drop_database
 from sqlalchemy.exc import InvalidRequestError
 from macrostrat.utils import cmd, get_logger
 from time import sleep
 from typing import Union, IO
 from pathlib import Path
@@ -116,14 +116,16 @@
 
 def _get_queries(sql, interpret_as_file=None):
     if isinstance(sql, (list, tuple)):
         queries = []
         for i in sql:
             queries.extend(_get_queries(i, interpret_as_file=interpret_as_file))
         return queries
+    if isinstance(sql, TextClause):
+        return [sql]
     if isinstance(sql, SQL):
         return [sql]
 
     if sql in [None, ""]:
         return
     if interpret_as_file:
         sql = Path(sql).read_text()
@@ -168,19 +170,21 @@
     if isinstance(connectable, Engine):
         conn = connectable.connect()
 
     # Find a connection or cursor object for the connectable
     conn = connectable
     if hasattr(conn, "raw_connection"):
         conn = conn.raw_connection()
-    while hasattr(conn, "connection"):
-        if callable(conn.connection):
-            conn = conn.connection()
+    while hasattr(conn, "driver_connection") or hasattr(conn, "connection"):
+        if hasattr(conn, "driver_connection"):
+            conn = conn.driver_connection
         else:
             conn = conn.connection
+        if callable(conn):
+            conn = conn()
     if hasattr(conn, "cursor"):
         conn = conn.cursor()
 
     return conn
 
 
 def _get_connection(connectable):
@@ -254,30 +258,32 @@
                     query = SQL(query)
                 # Pre-bind the parameters using PsycoPG2
                 query = query.format(**pre_bind_params)
 
             if isinstance(query, (SQL, Composed)):
                 query = _render_query(query, connectable)
 
-            sql_text = query
+            sql_text = str(query)
             if isinstance(query, str):
                 sql_text = format(query, strip_comments=True).strip()
                 if sql_text == "":
                     continue
                 # Check for server-bound parameters in sql native style. If there are none, use
                 # the SQLAlchemy text() function, otherwise use the raw query string
                 if has_server_binds is None:
                     has_server_binds = infer_has_server_binds(sql_text)
 
             log.debug("Executing SQL: \n %s", query)
             if has_server_binds:
                 conn = _get_connection(connectable)
                 res = conn.exec_driver_sql(query, params)
             else:
-                res = connectable.execute(text(query), params=params)
+                if not isinstance(query, TextClause):
+                    query = text(query)
+                res = connectable.execute(query, params)
             yield res
             if trans is not None:
                 trans.commit()
             elif hasattr(connectable, "commit"):
                 connectable.commit()
             pretty_print(sql_text, dim=True)
         except (ProgrammingError, IntegrityError, InternalError) as err:
```

### Comparing `macrostrat_database-2.1.3/pyproject.toml` & `macrostrat_database-3.0.0.dev1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 authors = ["Daven Quinn <dev@davenquinn.com>"]
 description = "A SQLAlchemy-based database toolkit."
 name = "macrostrat.database"
 packages = [{ include = "macrostrat" }]
-version = "2.1.3"
+version = "3.0.0-dev1"
 
 [tool.poetry.dependencies]
-GeoAlchemy2 = "^0.9.4"
-SQLAlchemy = "^1.4.26"
-SQLAlchemy-Utils = "^0.37.0"
+GeoAlchemy2 = "^0.14.0"
+SQLAlchemy = "^2.0.18"
+SQLAlchemy-Utils = "^0.41.1"
 click = "^8.1.3"
 "macrostrat.utils" = "^1.0.0"
-psycopg2-binary = "^2.9.1"
+psycopg2-binary = "^2.9.6"
 python = "^3.8"
-sqlparse = "^0.4.0"
+sqlparse = "^0.4.4"
 
 [tool.poetry.dev-dependencies]
 "macrostrat.utils" = { path = "../utils", develop = true }
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
```

