# Comparing `tmp/pyosutools-0.2.0.tar.gz` & `tmp/pyosutools-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyosutools-0.2.0.tar", last modified: Sat Jul  8 19:18:40 2023, max compression
+gzip compressed data, was "pyosutools-0.2.1.tar", last modified: Sun Jul  9 13:26:57 2023, max compression
```

## Comparing `pyosutools-0.2.0.tar` & `pyosutools-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:18:40.564055 pyosutools-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-08 19:18:27.000000 pyosutools-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-08 19:18:40.564055 pyosutools-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 19:18:27.000000 pyosutools-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:18:40.560055 pyosutools-0.2.0/pyosutools/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-08 19:18:27.000000 pyosutools-0.2.0/pyosutools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-08 19:18:27.000000 pyosutools-0.2.0/pyosutools/datatypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:18:40.564055 pyosutools-0.2.0/pyosutools/db/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-08 19:18:27.000000 pyosutools-0.2.0/pyosutools/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-08 19:18:27.000000 pyosutools-0.2.0/pyosutools/db/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-08 19:18:27.000000 pyosutools-0.2.0/pyosutools/db/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-07-08 19:18:27.000000 pyosutools-0.2.0/pyosutools/db/osu.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-08 19:18:27.000000 pyosutools-0.2.0/pyosutools/db/presence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-07-08 19:18:27.000000 pyosutools-0.2.0/pyosutools/db/scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-08 19:18:27.000000 pyosutools-0.2.0/pyosutools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:18:40.564055 pyosutools-0.2.0/pyosutools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-08 19:18:40.000000 pyosutools-0.2.0/pyosutools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-08 19:18:40.000000 pyosutools-0.2.0/pyosutools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 19:18:40.000000 pyosutools-0.2.0/pyosutools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-08 19:18:40.000000 pyosutools-0.2.0/pyosutools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-08 19:18:40.000000 pyosutools-0.2.0/pyosutools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-08 19:18:27.000000 pyosutools-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 19:18:40.564055 pyosutools-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:26:57.829534 pyosutools-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-09 13:26:46.000000 pyosutools-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-09 13:26:57.829534 pyosutools-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 13:26:46.000000 pyosutools-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:26:57.825534 pyosutools-0.2.1/pyosutools/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-09 13:26:46.000000 pyosutools-0.2.1/pyosutools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:26:57.829534 pyosutools-0.2.1/pyosutools/beatmaps/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-09 13:26:46.000000 pyosutools-0.2.1/pyosutools/beatmaps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9191 2023-07-09 13:26:46.000000 pyosutools-0.2.1/pyosutools/beatmaps/beatmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-07-09 13:26:46.000000 pyosutools-0.2.1/pyosutools/beatmaps/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-09 13:26:46.000000 pyosutools-0.2.1/pyosutools/datatypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:26:57.829534 pyosutools-0.2.1/pyosutools/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-09 13:26:46.000000 pyosutools-0.2.1/pyosutools/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-09 13:26:46.000000 pyosutools-0.2.1/pyosutools/db/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-09 13:26:46.000000 pyosutools-0.2.1/pyosutools/db/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-07-09 13:26:46.000000 pyosutools-0.2.1/pyosutools/db/osu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-09 13:26:46.000000 pyosutools-0.2.1/pyosutools/db/presence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-07-09 13:26:46.000000 pyosutools-0.2.1/pyosutools/db/scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-09 13:26:46.000000 pyosutools-0.2.1/pyosutools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:26:57.829534 pyosutools-0.2.1/pyosutools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-09 13:26:57.000000 pyosutools-0.2.1/pyosutools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-09 13:26:57.000000 pyosutools-0.2.1/pyosutools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 13:26:57.000000 pyosutools-0.2.1/pyosutools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-09 13:26:57.000000 pyosutools-0.2.1/pyosutools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-09 13:26:57.000000 pyosutools-0.2.1/pyosutools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-09 13:26:46.000000 pyosutools-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 13:26:57.829534 pyosutools-0.2.1/setup.cfg
```

### Comparing `pyosutools-0.2.0/LICENSE` & `pyosutools-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyosutools-0.2.0/PKG-INFO` & `pyosutools-0.2.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyosutools
-Version: 0.2.0
+Version: 0.2.1
 Summary: Parsing osu! files for easier usage
 Author-email: OlegSuperBro <olegrakovic323@gmail.com>
 Project-URL: Homepage, https://github.com/OlegSuperBro/pyosutools
 Project-URL: Bug Tracker, https://github.com/OlegSuperBro/pyosutools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyosutools-0.2.0/pyosutools/datatypes.py` & `pyosutools-0.2.1/pyosutools/datatypes.py`

 * *Files identical despite different names*

### Comparing `pyosutools-0.2.0/pyosutools/db/collection.py` & `pyosutools-0.2.1/pyosutools/db/collection.py`

 * *Files identical despite different names*

### Comparing `pyosutools-0.2.0/pyosutools/db/datatypes.py` & `pyosutools-0.2.1/pyosutools/db/datatypes.py`

 * *Files identical despite different names*

### Comparing `pyosutools-0.2.0/pyosutools/db/osu.py` & `pyosutools-0.2.1/pyosutools/db/osu.py`

 * *Files identical despite different names*

### Comparing `pyosutools-0.2.0/pyosutools/db/presence.py` & `pyosutools-0.2.1/pyosutools/db/presence.py`

 * *Files identical despite different names*

### Comparing `pyosutools-0.2.0/pyosutools/db/scores.py` & `pyosutools-0.2.1/pyosutools/db/scores.py`

 * *Files identical despite different names*

### Comparing `pyosutools-0.2.0/pyosutools/utils.py` & `pyosutools-0.2.1/pyosutools/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,7 +67,15 @@
 
 def read_datetime(buffer) -> datetime.datetime:
     ticks = read_ulong(buffer)
     if ticks >= 621355968000000000:
         return datetime.datetime.fromtimestamp((ticks-621355968000000000)/10_000_000, tz=datetime.timezone.utc)
     else:
         return datetime.datetime.min
+
+
+def is_int(text) -> bool:
+    try:
+        assert int(text) == float(text)
+    except (ValueError, AssertionError):
+        return False
+    return True
```

### Comparing `pyosutools-0.2.0/pyosutools.egg-info/PKG-INFO` & `pyosutools-0.2.1/pyosutools.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyosutools
-Version: 0.2.0
+Version: 0.2.1
 Summary: Parsing osu! files for easier usage
 Author-email: OlegSuperBro <olegrakovic323@gmail.com>
 Project-URL: Homepage, https://github.com/OlegSuperBro/pyosutools
 Project-URL: Bug Tracker, https://github.com/OlegSuperBro/pyosutools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyosutools-0.2.0/pyproject.toml` & `pyosutools-0.2.1/pyproject.toml`

 * *Files identical despite different names*

