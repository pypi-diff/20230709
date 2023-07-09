# Comparing `tmp/ngmapi-0.0.41.tar.gz` & `tmp/ngmapi-0.0.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngmapi-0.0.41.tar", last modified: Sun Jul  9 09:17:57 2023, max compression
+gzip compressed data, was "ngmapi-0.0.42.tar", last modified: Sun Jul  9 09:23:46 2023, max compression
```

## Comparing `ngmapi-0.0.41.tar` & `ngmapi-0.0.42.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:17:57.730729 ngmapi-0.0.41/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-09 09:17:57.730729 ngmapi-0.0.41/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:17:57.726729 ngmapi-0.0.41/ngmapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 09:17:10.000000 ngmapi-0.0.41/ngmapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-09 09:17:10.000000 ngmapi-0.0.41/ngmapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-09 09:17:10.000000 ngmapi-0.0.41/ngmapi/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-09 09:17:10.000000 ngmapi-0.0.41/ngmapi/func.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:17:57.730729 ngmapi-0.0.41/ngmapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-09 09:17:57.000000 ngmapi-0.0.41/ngmapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-09 09:17:57.000000 ngmapi-0.0.41/ngmapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 09:17:57.000000 ngmapi-0.0.41/ngmapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-09 09:17:57.000000 ngmapi-0.0.41/ngmapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-09 09:17:57.000000 ngmapi-0.0.41/ngmapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-09 09:17:57.000000 ngmapi-0.0.41/ngmapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-09 09:17:10.000000 ngmapi-0.0.41/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 09:17:57.730729 ngmapi-0.0.41/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:17:57.730729 ngmapi-0.0.41/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-09 09:17:10.000000 ngmapi-0.0.41/tests/test_add.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:23:46.466412 ngmapi-0.0.42/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-09 09:23:46.466412 ngmapi-0.0.42/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:23:46.466412 ngmapi-0.0.42/ngmapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 09:23:04.000000 ngmapi-0.0.42/ngmapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-09 09:23:04.000000 ngmapi-0.0.42/ngmapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-09 09:23:04.000000 ngmapi-0.0.42/ngmapi/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-09 09:23:04.000000 ngmapi-0.0.42/ngmapi/func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:23:46.466412 ngmapi-0.0.42/ngmapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-09 09:23:46.000000 ngmapi-0.0.42/ngmapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-09 09:23:46.000000 ngmapi-0.0.42/ngmapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 09:23:46.000000 ngmapi-0.0.42/ngmapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-09 09:23:46.000000 ngmapi-0.0.42/ngmapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-09 09:23:46.000000 ngmapi-0.0.42/ngmapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-09 09:23:46.000000 ngmapi-0.0.42/ngmapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-09 09:23:04.000000 ngmapi-0.0.42/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 09:23:46.466412 ngmapi-0.0.42/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:23:46.466412 ngmapi-0.0.42/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-09 09:23:04.000000 ngmapi-0.0.42/tests/test_add.py
```

### Comparing `ngmapi-0.0.41/pyproject.toml` & `ngmapi-0.0.42/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ngmapi"
-version = "0.0.41"
+version = "0.0.42"
 description = "Just a demo project"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["flask", "project"]
 dependencies = [
     "Flask",
     "Jinja2",
```

