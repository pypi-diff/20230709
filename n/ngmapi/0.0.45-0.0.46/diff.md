# Comparing `tmp/ngmapi-0.0.45.tar.gz` & `tmp/ngmapi-0.0.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngmapi-0.0.45.tar", last modified: Sun Jul  9 18:09:04 2023, max compression
+gzip compressed data, was "ngmapi-0.0.46.tar", last modified: Sun Jul  9 19:56:28 2023, max compression
```

## Comparing `ngmapi-0.0.45.tar` & `ngmapi-0.0.46.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:09:04.613569 ngmapi-0.0.45/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-09 18:09:04.613569 ngmapi-0.0.45/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:09:04.613569 ngmapi-0.0.45/ngmapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 18:08:18.000000 ngmapi-0.0.45/ngmapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-09 18:08:18.000000 ngmapi-0.0.45/ngmapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-09 18:08:18.000000 ngmapi-0.0.45/ngmapi/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-09 18:08:18.000000 ngmapi-0.0.45/ngmapi/func.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:09:04.613569 ngmapi-0.0.45/ngmapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-09 18:09:04.000000 ngmapi-0.0.45/ngmapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-09 18:09:04.000000 ngmapi-0.0.45/ngmapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 18:09:04.000000 ngmapi-0.0.45/ngmapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-09 18:09:04.000000 ngmapi-0.0.45/ngmapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-09 18:09:04.000000 ngmapi-0.0.45/ngmapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-09 18:09:04.000000 ngmapi-0.0.45/ngmapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-09 18:08:18.000000 ngmapi-0.0.45/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 18:09:04.613569 ngmapi-0.0.45/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:09:04.613569 ngmapi-0.0.45/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-09 18:08:18.000000 ngmapi-0.0.45/tests/test_add.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 19:56:28.960928 ngmapi-0.0.46/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-09 19:56:28.960928 ngmapi-0.0.46/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 19:56:28.960928 ngmapi-0.0.46/ngmapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 19:55:49.000000 ngmapi-0.0.46/ngmapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-09 19:55:49.000000 ngmapi-0.0.46/ngmapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-09 19:55:49.000000 ngmapi-0.0.46/ngmapi/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-09 19:55:49.000000 ngmapi-0.0.46/ngmapi/func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 19:56:28.960928 ngmapi-0.0.46/ngmapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-09 19:56:28.000000 ngmapi-0.0.46/ngmapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-09 19:56:28.000000 ngmapi-0.0.46/ngmapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 19:56:28.000000 ngmapi-0.0.46/ngmapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-09 19:56:28.000000 ngmapi-0.0.46/ngmapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-09 19:56:28.000000 ngmapi-0.0.46/ngmapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-09 19:56:28.000000 ngmapi-0.0.46/ngmapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-09 19:55:49.000000 ngmapi-0.0.46/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 19:56:28.960928 ngmapi-0.0.46/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 19:56:28.960928 ngmapi-0.0.46/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-09 19:55:49.000000 ngmapi-0.0.46/tests/test_add.py
```

### Comparing `ngmapi-0.0.45/pyproject.toml` & `ngmapi-0.0.46/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ngmapi"
-version = "0.0.45"
+version = "0.0.46"
 description = "Just a demo project"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["flask", "project"]
 dependencies = [
     "Flask",
     "Jinja2",
```

