# Comparing `tmp/ngmapi-0.0.30.tar.gz` & `tmp/ngmapi-0.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngmapi-0.0.30.tar", last modified: Sun Jul  9 06:02:50 2023, max compression
+gzip compressed data, was "ngmapi-0.0.31.tar", last modified: Sun Jul  9 06:07:38 2023, max compression
```

## Comparing `ngmapi-0.0.30.tar` & `ngmapi-0.0.31.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:02:50.706648 ngmapi-0.0.30/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-09 06:02:50.706648 ngmapi-0.0.30/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:02:50.706648 ngmapi-0.0.30/ngmapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 06:02:05.000000 ngmapi-0.0.30/ngmapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-09 06:02:05.000000 ngmapi-0.0.30/ngmapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-09 06:02:05.000000 ngmapi-0.0.30/ngmapi/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-09 06:02:05.000000 ngmapi-0.0.30/ngmapi/func.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:02:50.706648 ngmapi-0.0.30/ngmapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-09 06:02:50.000000 ngmapi-0.0.30/ngmapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-09 06:02:50.000000 ngmapi-0.0.30/ngmapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 06:02:50.000000 ngmapi-0.0.30/ngmapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-09 06:02:50.000000 ngmapi-0.0.30/ngmapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-09 06:02:50.000000 ngmapi-0.0.30/ngmapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-09 06:02:50.000000 ngmapi-0.0.30/ngmapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-09 06:02:05.000000 ngmapi-0.0.30/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 06:02:50.706648 ngmapi-0.0.30/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:02:50.706648 ngmapi-0.0.30/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-09 06:02:05.000000 ngmapi-0.0.30/tests/test_add.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:07:38.929437 ngmapi-0.0.31/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-09 06:07:38.929437 ngmapi-0.0.31/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:07:38.925438 ngmapi-0.0.31/ngmapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 06:06:53.000000 ngmapi-0.0.31/ngmapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-09 06:06:53.000000 ngmapi-0.0.31/ngmapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-09 06:06:53.000000 ngmapi-0.0.31/ngmapi/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-09 06:06:53.000000 ngmapi-0.0.31/ngmapi/func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:07:38.925438 ngmapi-0.0.31/ngmapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-09 06:07:38.000000 ngmapi-0.0.31/ngmapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-09 06:07:38.000000 ngmapi-0.0.31/ngmapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 06:07:38.000000 ngmapi-0.0.31/ngmapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-09 06:07:38.000000 ngmapi-0.0.31/ngmapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-09 06:07:38.000000 ngmapi-0.0.31/ngmapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-09 06:07:38.000000 ngmapi-0.0.31/ngmapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-09 06:06:53.000000 ngmapi-0.0.31/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 06:07:38.929437 ngmapi-0.0.31/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:07:38.925438 ngmapi-0.0.31/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-09 06:06:53.000000 ngmapi-0.0.31/tests/test_add.py
```

### Comparing `ngmapi-0.0.30/pyproject.toml` & `ngmapi-0.0.31/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ngmapi"
-version = "0.0.30"
+version = "0.0.31"
 description = "Just a demo project"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["flask", "project"]
 dependencies = [
     "Flask",
     "Jinja2",
```

