# Comparing `tmp/ngmapi-0.0.32.tar.gz` & `tmp/ngmapi-0.0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngmapi-0.0.32.tar", last modified: Sun Jul  9 06:19:00 2023, max compression
+gzip compressed data, was "ngmapi-0.0.33.tar", last modified: Sun Jul  9 06:22:11 2023, max compression
```

## Comparing `ngmapi-0.0.32.tar` & `ngmapi-0.0.33.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:19:00.382103 ngmapi-0.0.32/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-09 06:19:00.382103 ngmapi-0.0.32/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:19:00.382103 ngmapi-0.0.32/ngmapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 06:18:12.000000 ngmapi-0.0.32/ngmapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-09 06:18:12.000000 ngmapi-0.0.32/ngmapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-09 06:18:12.000000 ngmapi-0.0.32/ngmapi/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-09 06:18:12.000000 ngmapi-0.0.32/ngmapi/func.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:19:00.382103 ngmapi-0.0.32/ngmapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-09 06:19:00.000000 ngmapi-0.0.32/ngmapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-09 06:19:00.000000 ngmapi-0.0.32/ngmapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 06:19:00.000000 ngmapi-0.0.32/ngmapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-09 06:19:00.000000 ngmapi-0.0.32/ngmapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-09 06:19:00.000000 ngmapi-0.0.32/ngmapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-09 06:19:00.000000 ngmapi-0.0.32/ngmapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-09 06:18:12.000000 ngmapi-0.0.32/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 06:19:00.382103 ngmapi-0.0.32/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:19:00.382103 ngmapi-0.0.32/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-09 06:18:12.000000 ngmapi-0.0.32/tests/test_add.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:22:11.899064 ngmapi-0.0.33/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-09 06:22:11.899064 ngmapi-0.0.33/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:22:11.899064 ngmapi-0.0.33/ngmapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 06:21:24.000000 ngmapi-0.0.33/ngmapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-09 06:21:24.000000 ngmapi-0.0.33/ngmapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-09 06:21:24.000000 ngmapi-0.0.33/ngmapi/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-09 06:21:24.000000 ngmapi-0.0.33/ngmapi/func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:22:11.899064 ngmapi-0.0.33/ngmapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-09 06:22:11.000000 ngmapi-0.0.33/ngmapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-09 06:22:11.000000 ngmapi-0.0.33/ngmapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 06:22:11.000000 ngmapi-0.0.33/ngmapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-09 06:22:11.000000 ngmapi-0.0.33/ngmapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-09 06:22:11.000000 ngmapi-0.0.33/ngmapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-09 06:22:11.000000 ngmapi-0.0.33/ngmapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-09 06:21:24.000000 ngmapi-0.0.33/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 06:22:11.899064 ngmapi-0.0.33/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:22:11.899064 ngmapi-0.0.33/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-09 06:21:24.000000 ngmapi-0.0.33/tests/test_add.py
```

### Comparing `ngmapi-0.0.32/pyproject.toml` & `ngmapi-0.0.33/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ngmapi"
-version = "0.0.32"
+version = "0.0.33"
 description = "Just a demo project"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["flask", "project"]
 dependencies = [
     "Flask",
     "Jinja2",
```

