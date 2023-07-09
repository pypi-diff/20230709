# Comparing `tmp/event_dispatching-0.1.5.tar.gz` & `tmp/event_dispatching-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "event_dispatching-0.1.5.tar", max compression
+gzip compressed data, was "event_dispatching-0.2.0.tar", max compression
```

## Comparing `event_dispatching-0.1.5.tar` & `event_dispatching-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-07-09 07:43:47.089984 event_dispatching-0.1.5/LICENSE
--rw-r--r--   0        0        0     1627 2023-07-09 07:43:47.089984 event_dispatching-0.1.5/README.md
--rw-r--r--   0        0        0      238 2023-07-09 07:43:47.089984 event_dispatching-0.1.5/event_dispatcher/__init__.py
--rw-r--r--   0        0        0     1895 2023-07-09 07:43:47.089984 event_dispatching-0.1.5/event_dispatcher/_dispatcher.py
--rw-r--r--   0        0        0      953 2023-07-09 07:43:47.089984 event_dispatching-0.1.5/event_dispatcher/async_dispatcher.py
--rw-r--r--   0        0        0      817 2023-07-09 07:43:47.089984 event_dispatching-0.1.5/event_dispatcher/sync_dispatcher.py
--rw-r--r--   0        0        0      193 2023-07-09 07:43:47.089984 event_dispatching-0.1.5/event_dispatcher/types.py
--rw-r--r--   0        0        0     1717 2023-07-09 07:43:47.089984 event_dispatching-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2631 1970-01-01 00:00:00.000000 event_dispatching-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-09 15:53:37.754876 event_dispatching-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1627 2023-07-09 15:53:37.754876 event_dispatching-0.2.0/README.md
+-rw-r--r--   0        0        0      238 2023-07-09 15:53:37.754876 event_dispatching-0.2.0/event_dispatcher/__init__.py
+-rw-r--r--   0        0        0     2381 2023-07-09 15:53:37.754876 event_dispatching-0.2.0/event_dispatcher/_dispatcher.py
+-rw-r--r--   0        0        0      953 2023-07-09 15:53:37.754876 event_dispatching-0.2.0/event_dispatcher/async_dispatcher.py
+-rw-r--r--   0        0        0      817 2023-07-09 15:53:37.754876 event_dispatching-0.2.0/event_dispatcher/sync_dispatcher.py
+-rw-r--r--   0        0        0      193 2023-07-09 15:53:37.754876 event_dispatching-0.2.0/event_dispatcher/types.py
+-rw-r--r--   0        0        0     1702 2023-07-09 15:53:37.754876 event_dispatching-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2631 1970-01-01 00:00:00.000000 event_dispatching-0.2.0/PKG-INFO
```

### Comparing `event_dispatching-0.1.5/LICENSE` & `event_dispatching-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `event_dispatching-0.1.5/README.md` & `event_dispatching-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `event_dispatching-0.1.5/event_dispatcher/async_dispatcher.py` & `event_dispatching-0.2.0/event_dispatcher/async_dispatcher.py`

 * *Files identical despite different names*

### Comparing `event_dispatching-0.1.5/event_dispatcher/sync_dispatcher.py` & `event_dispatching-0.2.0/event_dispatcher/sync_dispatcher.py`

 * *Files identical despite different names*

### Comparing `event_dispatching-0.1.5/pyproject.toml` & `event_dispatching-0.2.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "event-dispatching"
-version = "0.1.5"
+version = "0.2.0"
 description = "Pure python implementation of event dispatcher"
 authors = ["Ruslan Saiko <ruslan.saiko.dev@gmail.com>"]
 repository = "https://github.com/trabem/event-dispatcher"
 readme = "README.md"
 packages = [{ include = "event_dispatcher" }]
 license = "MIT"
 classifiers = [
@@ -29,15 +29,14 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.0"
-pytest-cov = "^4.1.0"
 pytest-asyncio = "^0.21.0"
 coverage = "^7.2.7"
 ruff = "^0.0.275"
 black = "^23.3.0"
 
 
 [tool.poetry.group.dev.dependencies]
@@ -48,22 +47,24 @@
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 xfail_strict = true
 junit_family = "xunit2"
-addopts = [
-    "--cov=event_dispatcher",
-    "--cov-branch",
-]
 testpaths = [
     "tests"
 ]
 
+[tool.coverage.run]
+branch = true
+source = [
+    "event_dispatcher"
+]
+
 [tool.ruff]
 line-length = 100
 src = ["event_dispatcher", "tests", "examples"]
 select = [
     "E", # pycodestyle errors
     "W", # pycodestyle warnings
     "F", # pyflakes
```

### Comparing `event_dispatching-0.1.5/PKG-INFO` & `event_dispatching-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: event-dispatching
-Version: 0.1.5
+Version: 0.2.0
 Summary: Pure python implementation of event dispatcher
 Home-page: https://github.com/trabem/event-dispatcher
 License: MIT
 Keywords: event-dispatcher,event-dispatching,events,event handling,python,asynchronous,event-driven,event management
 Author: Ruslan Saiko
 Author-email: ruslan.saiko.dev@gmail.com
 Requires-Python: >=3.8,<4.0
```

