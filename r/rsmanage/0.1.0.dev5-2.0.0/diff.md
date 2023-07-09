# Comparing `tmp/rsmanage-0.1.0.dev5.tar.gz` & `tmp/rsmanage-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rsmanage-0.1.0.dev5.tar", max compression
+gzip compressed data, was "rsmanage-2.0.0.tar", max compression
```

## Comparing `rsmanage-0.1.0.dev5.tar` & `rsmanage-2.0.0.tar`

### file list

```diff
@@ -1,25 +1,33 @@
--rw-r--r--   0        0        0      758 2023-04-05 20:58:49.149531 rsmanage-0.1.0.dev5/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-03-09 19:14:49.266646 rsmanage-0.1.0.dev5/rsptx/configuration/.DS_Store
--rw-r--r--   0        0        0      115 2023-03-09 19:09:51.074639 rsmanage-0.1.0.dev5/rsptx/configuration/__init__.py
--rw-r--r--   0        0        0     6793 2023-04-05 14:23:33.015521 rsmanage-0.1.0.dev5/rsptx/configuration/core.py
--rw-r--r--   0        0        0      170 2023-03-09 22:13:07.158703 rsmanage-0.1.0.dev5/rsptx/db/__init__.py
--rw-r--r--   0        0        0     3781 2023-03-09 21:50:03.983895 rsmanage-0.1.0.dev5/rsptx/db/async_session.py
--rw-r--r--   0        0        0        0 2023-03-02 01:20:30.170791 rsmanage-0.1.0.dev5/rsptx/db/core.py
--rw-r--r--   0        0        0    47266 2023-04-05 20:16:01.784815 rsmanage-0.1.0.dev5/rsptx/db/crud.py
--rw-r--r--   0        0        0    34702 2023-04-05 19:35:42.455585 rsmanage-0.1.0.dev5/rsptx/db/models.py
--rw-r--r--   0        0        0      157 2023-03-09 20:28:09.484265 rsmanage-0.1.0.dev5/rsptx/logging/__init__.py
--rw-r--r--   0        0        0     1287 2023-03-08 23:05:08.643659 rsmanage-0.1.0.dev5/rsptx/logging/applogger.py
--rw-r--r--   0        0        0        0 2023-03-08 22:56:40.930613 rsmanage-0.1.0.dev5/rsptx/logging/core.py
--rw-r--r--   0        0        0       61 2023-03-09 22:36:30.128028 rsmanage-0.1.0.dev5/rsptx/response_helpers/__init__.py
--rw-r--r--   0        0        0     2027 2023-03-09 22:36:59.204561 rsmanage-0.1.0.dev5/rsptx/response_helpers/core.py
--rw-r--r--   0        0        0        1 2023-04-05 14:13:55.936220 rsmanage-0.1.0.dev5/rsptx/rsmanage/.ruff_cache/.gitignore
--rw-r--r--   0        0        0        8 2023-04-05 14:13:55.975431 rsmanage-0.1.0.dev5/rsptx/rsmanage/.ruff_cache/.update-informer
--rw-r--r--   0        0        0       43 2023-04-05 14:13:55.936129 rsmanage-0.1.0.dev5/rsptx/rsmanage/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       16 2023-04-05 14:13:55.936874 rsmanage-0.1.0.dev5/rsptx/rsmanage/.ruff_cache/content/2a4b723e63e7a02b
--rw-r--r--   0        0        0       92 2023-04-05 14:20:53.448803 rsmanage-0.1.0.dev5/rsptx/rsmanage/.ruff_cache/content/92f53d3a4ad427c5
--rw-r--r--   0        0        0       53 2023-04-04 00:34:17.783475 rsmanage-0.1.0.dev5/rsptx/rsmanage/__init__.py
--rw-r--r--   0        0        0    31063 2023-04-05 20:17:43.700226 rsmanage-0.1.0.dev5/rsptx/rsmanage/core.py
--rw-r--r--   0        0        0      102 2023-03-09 18:36:55.992558 rsmanage-0.1.0.dev5/rsptx/validation/__init__.py
--rw-r--r--   0        0        0        0 2023-03-08 23:10:27.223914 rsmanage-0.1.0.dev5/rsptx/validation/core.py
--rw-r--r--   0        0        0     7516 2023-03-08 23:12:14.553121 rsmanage-0.1.0.dev5/rsptx/validation/schemas.py
--rw-r--r--   0        0        0      854 1970-01-01 00:00:00.000000 rsmanage-0.1.0.dev5/PKG-INFO
+-rw-r--r--   0        0        0      993 2023-07-09 21:47:46.956336 rsmanage-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0       56 2023-06-03 21:54:38.113541 rsmanage-2.0.0/rsptx/build_tools/__init__.py
+-rw-r--r--   0        0        0    25694 2023-07-07 15:17:16.506394 rsmanage-2.0.0/rsptx/build_tools/core.py
+-rw-r--r--   0        0        0       53 2023-05-10 23:20:24.383591 rsmanage-2.0.0/rsptx/cl_utils/__init__.py
+-rw-r--r--   0        0        0    11142 2023-07-03 20:59:47.910307 rsmanage-2.0.0/rsptx/cl_utils/core.py
+-rw-r--r--   0        0        0     6148 2023-03-09 19:14:49.266646 rsmanage-2.0.0/rsptx/configuration/.DS_Store
+-rw-r--r--   0        0        0      115 2023-03-09 19:09:51.074639 rsmanage-2.0.0/rsptx/configuration/__init__.py
+-rw-r--r--   0        0        0     6876 2023-06-21 20:11:39.653403 rsmanage-2.0.0/rsptx/configuration/core.py
+-rw-r--r--   0        0        0        1 2023-04-06 18:13:38.636909 rsmanage-2.0.0/rsptx/db/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-04-06 18:13:38.636752 rsmanage-2.0.0/rsptx/db/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     8238 2023-04-06 22:58:10.066413 rsmanage-2.0.0/rsptx/db/.ruff_cache/content/895fda5609e2f73d
+-rw-r--r--   0        0        0     4076 2023-04-06 18:13:38.649509 rsmanage-2.0.0/rsptx/db/.ruff_cache/content/97776eeb3613080b
+-rw-r--r--   0        0        0      170 2023-03-09 22:13:07.158703 rsmanage-2.0.0/rsptx/db/__init__.py
+-rw-r--r--   0        0        0     3781 2023-03-09 21:50:03.983895 rsmanage-2.0.0/rsptx/db/async_session.py
+-rw-r--r--   0        0        0        0 2023-03-02 01:20:30.170791 rsmanage-2.0.0/rsptx/db/core.py
+-rw-r--r--   0        0        0    69010 2023-06-07 15:57:51.302871 rsmanage-2.0.0/rsptx/db/crud.py
+-rw-r--r--   0        0        0    35422 2023-04-19 23:28:28.033383 rsmanage-2.0.0/rsptx/db/models.py
+-rw-r--r--   0        0        0      157 2023-03-09 20:28:09.484265 rsmanage-2.0.0/rsptx/logging/__init__.py
+-rw-r--r--   0        0        0     1287 2023-03-08 23:05:08.643659 rsmanage-2.0.0/rsptx/logging/applogger.py
+-rw-r--r--   0        0        0        0 2023-03-08 22:56:40.930613 rsmanage-2.0.0/rsptx/logging/core.py
+-rw-r--r--   0        0        0       61 2023-03-09 22:36:30.128028 rsmanage-2.0.0/rsptx/response_helpers/__init__.py
+-rw-r--r--   0        0        0     2027 2023-03-09 22:36:59.204561 rsmanage-2.0.0/rsptx/response_helpers/core.py
+-rw-r--r--   0        0        0        1 2023-04-05 14:13:55.936220 rsmanage-2.0.0/rsptx/rsmanage/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0        8 2023-04-05 14:13:55.975431 rsmanage-2.0.0/rsptx/rsmanage/.ruff_cache/.update-informer
+-rw-r--r--   0        0        0       43 2023-04-05 14:13:55.936129 rsmanage-2.0.0/rsptx/rsmanage/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       16 2023-04-05 14:13:55.936874 rsmanage-2.0.0/rsptx/rsmanage/.ruff_cache/content/2a4b723e63e7a02b
+-rw-r--r--   0        0        0       92 2023-04-05 14:20:53.448803 rsmanage-2.0.0/rsptx/rsmanage/.ruff_cache/content/92f53d3a4ad427c5
+-rw-r--r--   0        0        0       53 2023-04-04 00:34:17.783475 rsmanage-2.0.0/rsptx/rsmanage/__init__.py
+-rw-r--r--   0        0        0    30434 2023-06-21 19:27:19.014674 rsmanage-2.0.0/rsptx/rsmanage/core.py
+-rw-r--r--   0        0        0      102 2023-03-09 18:36:55.992558 rsmanage-2.0.0/rsptx/validation/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-08 23:10:27.223914 rsmanage-2.0.0/rsptx/validation/core.py
+-rw-r--r--   0        0        0     7516 2023-03-08 23:12:14.553121 rsmanage-2.0.0/rsptx/validation/schemas.py
+-rw-r--r--   0        0        0     1123 1970-01-01 00:00:00.000000 rsmanage-2.0.0/PKG-INFO
```

### Comparing `rsmanage-0.1.0.dev5/pyproject.toml` & `rsmanage-2.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 [tool.poetry]
 name = "rsmanage"
-version = "0.1.0dev5"
+version = "2.0.0"
 description = ""
 authors = ['Brad Miller <bonelake@mac.com>']
 license = ""
 
 packages = [
     {include = "rsptx"},
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 asyncclick = "^8.1.3.4"
 redis = "^4.5.4"
-runestone = "^6.6.1"
 pgcli = "^3.5.0"
 sqlalchemy = "^1.4.0"
 psycopg2-binary = "^2.9.6"
 anyio = "^3.6.2"
 pydantic = {version = "^1.10.7", extras = ["dotenv"]}
 asyncpg = "^0.27.0"
 greenlet = "^2.0.2"
 pyhumps = "^3.8.0"
 fastapi = "^0.95.0"
 pydal = "^20221110.1"
+myst-parser = "^1.0.0"
+sphinx-reredirects = "^0.1.2"
+lxml = "^4.9.2"
+paver = "^1.3.4"
+sphinxcontrib-paverutils = "^1.17.0"
+runestone = "^7.0.0"
+python-dotenv = "^1.0.0"
+
+[tool.poetry.group.dev.dependencies]
+runestone = {path = "../interactives", develop=true}
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 # Scripts
```

### Comparing `rsmanage-0.1.0.dev5/rsptx/configuration/.DS_Store` & `rsmanage-2.0.0/rsptx/configuration/.DS_Store`

 * *Files identical despite different names*

### Comparing `rsmanage-0.1.0.dev5/rsptx/configuration/core.py` & `rsmanage-2.0.0/rsptx/configuration/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,16 @@
     class Config:
         env_file = ".env"
         env_file_encoding = "utf-8"
 
     google_ga: str = ""
 
     # The path to the Runestone application inside web2py.
-    runestone_path: str = Path(os.environ.get("RUNESTONE_PATH")).resolve()
+
+    runestone_path: str = Path(os.environ.get("RUNESTONE_PATH", Path.home())).resolve()
 
     # _`book_path`: specify the directory to serve books from. For now, default to serving from the same place as the Runestone server, since the server uses some of these files.
     book_path: Path = runestone_path / "books"
 
     # The path to store error logs.
     error_path: Path = Path.home() / "Runestone/errors"
 
@@ -71,17 +72,19 @@
     #
     # .. admonition:: warning
     #
     #    When using an Enum for a configuration setting you cannot compare against
     #    a string.  The value will actually be ``BookServerConfig.development``` or whatever.
     #    Our style will be to compare against the Enum not the ``.name`` attribute.
     #
-    book_server_config: BookServerConfig = "development"  # type: ignore
     server_config: str = "development"
 
+    # server_config is the master make sure everything else matches
+    book_server_config: BookServerConfig = server_config  # type: ignore
+
     # Database setup: this must be an standard (synchronous) connection; for example:
     #
     # - ``sqlite:///./runestone.db``
     # - ``postgresql://postgres:bully@localhost/runestone``
     dburl: str = f"sqlite:///{runestone_path}/runestone.db"
     dev_dburl: str = f"sqlite:///{runestone_path}/runestone_dev.db"
     test_dburl: str = f"sqlite:///{runestone_path}/runestone_test.db"
```

### Comparing `rsmanage-0.1.0.dev5/rsptx/db/async_session.py` & `rsmanage-2.0.0/rsptx/db/async_session.py`

 * *Files identical despite different names*

### Comparing `rsmanage-0.1.0.dev5/rsptx/db/models.py` & `rsmanage-2.0.0/rsptx/db/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,16 @@
     Date,
     DateTime,
     JSON,
     Text,
     types,
     Float,
     inspect,
+    LargeBinary,
+    CHAR,
 )
 from sqlalchemy.ext.declarative import declared_attr
 from sqlalchemy.sql.schema import UniqueConstraint
 
 # Local application imports
 # -------------------------
 from .async_session import Base
@@ -424,14 +426,24 @@
     ## @validator("username")
     ## def username_unique(cls, v):
     ##     if bookserver.crud.fetch_user(v):
     ##         raise ValueError("username must be unique")
     ##     return v
 
 
+class AuthEvent(Base, IdMixin):
+    __tablename__ = "auth_event"
+
+    time_stamp = Column(DateTime)
+    client_ip = Column(String(512))
+    user_id = Column(ForeignKey("auth_user.id", ondelete="CASCADE"))
+    origin = Column(String(512))
+    description = Column(Text)
+
+
 class AuthGroup(Base, IdMixin):
     __tablename__ = "auth_group"
 
     role = Column(String(512))
     description = Column(Text)
 
 
@@ -548,14 +560,17 @@
     nopause = Column(Web2PyBoolean)
     is_peer = Column(Web2PyBoolean, default=False)
     current_index = Column(Integer, default=0)
     enforce_due = Column(Web2PyBoolean)
     peer_async_visible = Column(Web2PyBoolean, default=False)
 
 
+AssignmentValidator = sqlalchemy_to_pydantic(Assignment)
+
+
 class AssignmentQuestion(Base, IdMixin):
     __tablename__ = "assignment_questions"
 
     assignment_id = Column(
         ForeignKey("assignments.id", ondelete="CASCADE"), nullable=False, index=True
     )
     question_id = Column(
@@ -627,14 +642,16 @@
     manual_total = Column(Web2PyBoolean, nullable=False)
     # Not all grades will be reportable via LTI.
     lis_result_sourcedid = Column(String(1024))
     lis_outcome_url = Column(String(1024))
     is_submit = Column(String(512))
 
 
+GradeValidator = sqlalchemy_to_pydantic(Grade)
+
 # Book Structure Tables
 # ---------------------
 class Chapter(Base, IdMixin):
     __tablename__ = "chapters"
 
     chapter_name = Column(String(512), nullable=False)
     course_id = Column(String(512), index=True, nullable=False)
@@ -967,7 +984,18 @@
     __tablename__ = "invoice_request"
 
     timestamp = Column(DateTime)
     sid = Column(String(512))
     course_name = Column(String(512))
     email = Column(String(512))
     processed = Column(Web2PyBoolean)
+
+
+class Web2pySessionRunestone(Base, IdMixin):
+    __tablename__ = "web2py_session_runestone"
+
+    locked = Column(CHAR(1))
+    client_ip = Column(String(64))
+    created_datetime = Column(DateTime)
+    modified_datetime = Column(DateTime)
+    unique_key = Column(String(64))
+    session_data = Column(LargeBinary)
```

### Comparing `rsmanage-0.1.0.dev5/rsptx/logging/applogger.py` & `rsmanage-2.0.0/rsptx/logging/applogger.py`

 * *Files identical despite different names*

### Comparing `rsmanage-0.1.0.dev5/rsptx/response_helpers/core.py` & `rsmanage-2.0.0/rsptx/response_helpers/core.py`

 * *Files identical despite different names*

### Comparing `rsmanage-0.1.0.dev5/rsptx/rsmanage/core.py` & `rsmanage-2.0.0/rsptx/rsmanage/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,21 +15,23 @@
 import csv
 import datetime
 import json
 import os
 import re
 import sys
 import subprocess
+from pathlib import Path
 
 # third party imports
 import redis
 from sqlalchemy import create_engine
 from sqlalchemy.exc import IntegrityError
 from pgcli.main import cli as clipg
 from psycopg2.errors import UniqueViolation
+from dotenv import load_dotenv
 
 # our own package imports
 
 from rsptx.db.crud import (
     create_initial_courses_users,
     create_book_author,
     create_course,
@@ -53,29 +55,39 @@
     is_author,
     is_editor,
     update_user,
 )
 from rsptx.db.models import CoursesValidator, AuthUserValidator
 from rsptx.db.async_session import init_models, term_models
 from rsptx.configuration import settings
-from runestone.server.utils import _build_runestone_book, _build_ptx_book
+from rsptx.build_tools.core import _build_runestone_book, _build_ptx_book
+from rsptx.cl_utils.core import load_project_dotenv
 
 import pdb
 
 
 class Config(object):
     def __init__(self):
         self.verbose = False
 
 
 pass_config = click.make_pass_decorator(Config, ensure=True)
 
 # configuration
-REQ_ENV = ["WEB2PY_CONFIG", "DBURL"]
-OPT_ENV = ["JWT_SECRET", "WEB2PY_PRIVATE_KEY"]
+REQ_ENV = [
+    "SERVER_CONFIG",
+    "DBURL",
+    "WEB2PY_PRIVATE_KEY",
+    "JWT_SECRET",
+    "BOOK_PATH",
+]
+OPT_ENV = [
+    "DC_DEV_DBURL",
+    "DC_DBURL",
+]
 APP = "runestone"
 APP_PATH = "applications/{}".format(APP)
 DBSDIR = "{}/databases".format(APP_PATH)
 BUILDDIR = "{}/build".format(APP_PATH)
 PRIVATEDIR = "{}/private".format(APP_PATH)
 
 
@@ -84,33 +96,28 @@
 @click.option("--if_clean", is_flag=True, help="only run if database is uninitialized")
 @pass_config
 async def cli(config, verbose, if_clean):
     """Type subcommand --help for help on any subcommand"""
     checkEnvironment()
 
     conf = settings.server_config
-
-    if conf == "production":
-        config.dburl = os.environ.get("DBURL")
-    elif conf == "development":
-        config.dburl = os.environ.get("DEV_DBURL")
-    elif conf == "test":
-        config.dburl = os.environ.get("TEST_DBURL")
-    else:
-        click.echo("Incorrect WEB2PY_CONFIG")
-        sys.exit(1)
+    config.dburl = settings.database_url
 
     # DAL uses "postgres:", while SQLAlchemy (and the PostgreSQL spec) uses "postgresql:". Fix.
     remove_prefix = "postgres://"
     if config.dburl.startswith(remove_prefix):
         config.dburl = "postgresql://" + config.dburl[len(remove_prefix) :]
 
     config.conf = conf
     config.dbname = re.match(r"postgres.*//.*?@.*?/(.*)", config.dburl).group(1)
     config.dbhost = re.match(r"postgres.*//.*?@(.*?)/(.*)", config.dburl).group(1)
+
+    click.echo(f"Using configuration: {conf}")
+    click.echo(f"Using database: {config.dbname}")
+
     if conf != "production":
         config.dbuser = re.match(
             r"postgres.*//(.*?)(:.*?)?@(.*?)/(.*)", config.dburl
         ).group(1)
     else:
         config.dbuser = re.match(
             r"postgres.*//(.*?):(.*?)@(.*?)/(.*)", config.dburl
@@ -132,40 +139,35 @@
 async def _initdb(config):
     # Because click won't natively support making commands async we can use this simple method
     # to call async functions.
     # Since we successfully dropped the database we need to initialize it here.
 
     await init_models()
     await create_initial_courses_users()
-    await term_models()
     await create_group("instructor")
     await create_group("editor")
     await create_group("author")
+    await term_models()  # dispose of the engine
 
 
 #
 #    initdb
 #
 @cli.command()
 @click.option(
     "--list_tables", is_flag=True, help="List all of the defined tables when done"
 )
 @click.option(
     "--reset", is_flag=True, help="drop database and delete all migration information"
 )
-@click.option("--fake", is_flag=True, help="perform a fake migration")
 @click.option("--force", is_flag=True, help="answer Yes to confirm questions")
 @pass_config
-async def initdb(config, list_tables, reset, fake, force):
+async def initdb(config, list_tables, reset, force):
     """Initialize and optionally reset the database"""
-    os.chdir(findProjectRoot())
-    if not os.path.exists(DBSDIR):
-        click.echo("Making databases folder")
-        os.mkdir(DBSDIR)
-
+    checkEnvironment()
     if reset:
         if not force:
             click.confirm(
                 "Resetting the database will delete the database and the contents of the databases folder.  Are you sure?",
                 default=False,
                 abort=True,
                 prompt_suffix=": ",
@@ -181,46 +183,21 @@
             f"createdb --host={config.dbhost} --username={config.dbuser} --owner={config.dbuser} {config.dbname}",
             shell=True,
         )
         if res != 0:
             click.echo("Failed to drop the database do you have permission?")
             sys.exit(1)
 
-        click.echo("Removing all files in databases/")
-        table_migrate_prefix = "runestone_"
-        if config.conf == "test":
-            table_migrate_prefix = "test_runestone_"
-        for the_file in os.listdir(DBSDIR):
-            file_path = os.path.join(DBSDIR, the_file)
-            try:
-                if os.path.isfile(file_path) and file_path.startswith(
-                    os.path.join(DBSDIR, table_migrate_prefix)
-                ):
-                    print(f"removing {file_path}")
-                    os.unlink(file_path)
-            except Exception as e:
-                print(e)
-
         # Because click won't natively support making commands async we can use this simple method
         # to call async functions.
         # Since we successfully dropped the database we need to initialize it here.
         settings.drop_tables = "Yes"
         await _initdb(config)
         click.echo("Created new tables")
 
-    if len(os.listdir("{}/databases".format(APP_PATH))) > 1 and not fake and not force:
-        click.confirm(
-            "It appears you already have database migration information do you want to proceed?",
-            default=False,
-            abort=True,
-            prompt_suffix=": ",
-            show_default=True,
-            err=False,
-        )
-
     click.echo(
         message="Initializing the database", file=None, nl=True, err=False, color=None
     )
 
     if not reset:
         await _initdb(config)
 
@@ -269,21 +246,26 @@
     host,
     newserver,
     allow_pairs,
 ):
     """Create a course in the database"""
 
     done = False
+    regex = r"^([\x30-\x39]|[\x41-\x5A]|[\x61-\x7A]|[_-])*$"
     if course_name:
         use_defaults = True
     else:
         use_defaults = False
     while not done:
         if not course_name:
             course_name = click.prompt("Course Name")
+        if not re.match(regex, course_name):
+            click.echo("Course name must be alphanumeric or underscore")
+            course_name = None
+            continue
         if not python3 and not use_defaults:
             python3 = (
                 "T" if click.confirm("Use Python3 style syntax?", default="T") else "F"
             )
         else:
             python3 = "T" if python3 else "F"
         if not basecourse and not use_defaults:
@@ -831,31 +813,35 @@
 
 @cli.command()
 @pass_config
 def db(config):
     """
     Connect to the database based on the current configuration
     """
-    # replace argv[1] which is 'db' with the url to connect to
-    sys.argv[1] = config.dburl
-    sys.exit(clipg())
+    sys.exit(subprocess.run(["pgcli", f"{config.dburl.replace('+asyncpg', '')}"]))
 
 
 #
 # Utility Functions Below here
 #
 
 
 def checkEnvironment():
     """
     Check the list of required and optional environment variables to be sure they are defined.
     """
     stop = False
-    assert os.environ["WEB2PY_CONFIG"]
-    config = os.environ["WEB2PY_CONFIG"]
+
+    load_project_dotenv()
+
+    if "SERVER_CONFIG" not in os.environ:
+        click.echo("You must set your SERVER_CONFIG environment variable")
+        sys.exit()
+
+    config = os.environ["SERVER_CONFIG"]
 
     if config == "production":
         for var in REQ_ENV:
             if var not in os.environ:
                 stop = True
                 click.echo("Missing definition for {} environment variable".format(var))
     elif config == "test":
@@ -867,23 +853,26 @@
             stop = True
             click.echo("Missing definition for DEV_DBURL environment variable")
 
     for var in OPT_ENV:
         if var not in os.environ:
             click.echo("You may want to define the {} environment variable".format(var))
 
+    if "DC_DBURL" in os.environ or "DC_DEV_DBURL" in os.environ:
+        click.echo("You have defined docker compose specific environment variables")
+
     if stop:
         sys.exit(1)
 
 
 def echoEnviron(config):
-    click.echo("WEB2PY_CONFIG is {}".format(config.conf))
-    click.echo("SERVER_CONFIG is {}".format(settings.server_config))
     click.echo("RUNESTONE_PATH is {}".format(settings.runestone_path))
     click.echo("BOOK_PATH is {}".format(settings.book_path))
+    click.echo("SERVER_CONFIG is {}".format(settings.server_config))
+    click.echo("WEB2PY_CONFIG is {}".format(config.conf))
     click.echo("The database URL is configured as {}".format(config.dburl))
     click.echo("DBNAME is {}".format(config.dbname))
 
 
 def findProjectRoot():
     start = os.getcwd()
     prevdir = ""
@@ -957,20 +946,20 @@
             github = f"https://github.com/RunestoneInteractive/{book}.git"
 
     # create an entry in book_author (author, book)
     try:
         vals = dict(title=f"Temporary title for {book}")
         await create_library_book(book, vals)
     except Exception as e:
-        click.echo(f"Warning Book already exists in library {e}")
+        click.echo(f"Warning: Book already exists in library")
 
     try:
         await create_book_author(author, book)
     except Exception as e:
-        click.echo(f"Warning setting book,author pair failed {e}")
+        click.echo(f"Warning: It appears that {author} is already an author of {book}")
 
     # create an entry in auth_membership (group_id, user_id)
     auth_row = await fetch_group("author")
     auth_group_id = auth_row.id
 
     if not await is_author(a_row.id):
         await create_membership(auth_group_id, a_row.id)
```

### Comparing `rsmanage-0.1.0.dev5/rsptx/validation/schemas.py` & `rsmanage-2.0.0/rsptx/validation/schemas.py`

 * *Files identical despite different names*

