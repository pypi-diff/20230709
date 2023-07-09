# Comparing `tmp/event_dispatching-0.1.4.tar.gz` & `tmp/event_dispatching-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "event_dispatching-0.1.4.tar", max compression
+gzip compressed data, was "event_dispatching-0.1.5.tar", max compression
```

## Comparing `event_dispatching-0.1.4.tar` & `event_dispatching-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-07-07 08:23:30.272583 event_dispatching-0.1.4/LICENSE
--rw-r--r--   0        0        0     1627 2023-07-07 08:23:30.272583 event_dispatching-0.1.4/README.md
--rw-r--r--   0        0        0      238 2023-07-07 08:23:30.272583 event_dispatching-0.1.4/event_dispatcher/__init__.py
--rw-r--r--   0        0        0     1895 2023-07-07 08:23:30.272583 event_dispatching-0.1.4/event_dispatcher/_dispatcher.py
--rw-r--r--   0        0        0      953 2023-07-07 08:23:30.272583 event_dispatching-0.1.4/event_dispatcher/async_dispatcher.py
--rw-r--r--   0        0        0      817 2023-07-07 08:23:30.272583 event_dispatching-0.1.4/event_dispatcher/sync_dispatcher.py
--rw-r--r--   0        0        0      237 2023-07-07 08:23:30.272583 event_dispatching-0.1.4/event_dispatcher/types.py
--rw-r--r--   0        0        0     1717 2023-07-07 08:23:30.272583 event_dispatching-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2631 1970-01-01 00:00:00.000000 event_dispatching-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-09 07:43:47.089984 event_dispatching-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1627 2023-07-09 07:43:47.089984 event_dispatching-0.1.5/README.md
+-rw-r--r--   0        0        0      238 2023-07-09 07:43:47.089984 event_dispatching-0.1.5/event_dispatcher/__init__.py
+-rw-r--r--   0        0        0     1895 2023-07-09 07:43:47.089984 event_dispatching-0.1.5/event_dispatcher/_dispatcher.py
+-rw-r--r--   0        0        0      953 2023-07-09 07:43:47.089984 event_dispatching-0.1.5/event_dispatcher/async_dispatcher.py
+-rw-r--r--   0        0        0      817 2023-07-09 07:43:47.089984 event_dispatching-0.1.5/event_dispatcher/sync_dispatcher.py
+-rw-r--r--   0        0        0      193 2023-07-09 07:43:47.089984 event_dispatching-0.1.5/event_dispatcher/types.py
+-rw-r--r--   0        0        0     1717 2023-07-09 07:43:47.089984 event_dispatching-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2631 1970-01-01 00:00:00.000000 event_dispatching-0.1.5/PKG-INFO
```

### Comparing `event_dispatching-0.1.4/LICENSE` & `event_dispatching-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `event_dispatching-0.1.4/README.md` & `event_dispatching-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `event_dispatching-0.1.4/event_dispatcher/_dispatcher.py` & `event_dispatching-0.1.5/event_dispatcher/_dispatcher.py`

 * *Files identical despite different names*

### Comparing `event_dispatching-0.1.4/event_dispatcher/async_dispatcher.py` & `event_dispatching-0.1.5/event_dispatcher/async_dispatcher.py`

 * *Files identical despite different names*

### Comparing `event_dispatching-0.1.4/event_dispatcher/sync_dispatcher.py` & `event_dispatching-0.1.5/event_dispatcher/sync_dispatcher.py`

 * *Files identical despite different names*

### Comparing `event_dispatching-0.1.4/pyproject.toml` & `event_dispatching-0.1.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "event-dispatching"
-version = "0.1.4"
+version = "0.1.5"
 description = "Pure python implementation of event dispatcher"
 authors = ["Ruslan Saiko <ruslan.saiko.dev@gmail.com>"]
 repository = "https://github.com/trabem/event-dispatcher"
 readme = "README.md"
 packages = [{ include = "event_dispatcher" }]
 license = "MIT"
 classifiers = [
```

### Comparing `event_dispatching-0.1.4/PKG-INFO` & `event_dispatching-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: event-dispatching
-Version: 0.1.4
+Version: 0.1.5
 Summary: Pure python implementation of event dispatcher
 Home-page: https://github.com/trabem/event-dispatcher
 License: MIT
 Keywords: event-dispatcher,event-dispatching,events,event handling,python,asynchronous,event-driven,event management
 Author: Ruslan Saiko
 Author-email: ruslan.saiko.dev@gmail.com
 Requires-Python: >=3.8,<4.0
```

