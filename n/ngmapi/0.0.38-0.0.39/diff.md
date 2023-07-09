# Comparing `tmp/ngmapi-0.0.38.tar.gz` & `tmp/ngmapi-0.0.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngmapi-0.0.38.tar", last modified: Sun Jul  9 07:32:43 2023, max compression
+gzip compressed data, was "ngmapi-0.0.39.tar", last modified: Sun Jul  9 07:35:47 2023, max compression
```

## Comparing `ngmapi-0.0.38.tar` & `ngmapi-0.0.39.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:32:43.170123 ngmapi-0.0.38/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-09 07:32:43.170123 ngmapi-0.0.38/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:32:43.170123 ngmapi-0.0.38/ngmapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 07:31:54.000000 ngmapi-0.0.38/ngmapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-09 07:31:54.000000 ngmapi-0.0.38/ngmapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-09 07:31:54.000000 ngmapi-0.0.38/ngmapi/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-09 07:31:54.000000 ngmapi-0.0.38/ngmapi/func.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:32:43.170123 ngmapi-0.0.38/ngmapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-09 07:32:43.000000 ngmapi-0.0.38/ngmapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-09 07:32:43.000000 ngmapi-0.0.38/ngmapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 07:32:43.000000 ngmapi-0.0.38/ngmapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-09 07:32:43.000000 ngmapi-0.0.38/ngmapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-09 07:32:43.000000 ngmapi-0.0.38/ngmapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-09 07:32:43.000000 ngmapi-0.0.38/ngmapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-09 07:31:54.000000 ngmapi-0.0.38/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 07:32:43.170123 ngmapi-0.0.38/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:32:43.170123 ngmapi-0.0.38/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-09 07:31:54.000000 ngmapi-0.0.38/tests/test_add.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:35:47.382094 ngmapi-0.0.39/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-09 07:35:47.382094 ngmapi-0.0.39/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:35:47.382094 ngmapi-0.0.39/ngmapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 07:35:07.000000 ngmapi-0.0.39/ngmapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-09 07:35:07.000000 ngmapi-0.0.39/ngmapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-09 07:35:07.000000 ngmapi-0.0.39/ngmapi/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-09 07:35:07.000000 ngmapi-0.0.39/ngmapi/func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:35:47.382094 ngmapi-0.0.39/ngmapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-09 07:35:47.000000 ngmapi-0.0.39/ngmapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-09 07:35:47.000000 ngmapi-0.0.39/ngmapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 07:35:47.000000 ngmapi-0.0.39/ngmapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-09 07:35:47.000000 ngmapi-0.0.39/ngmapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-09 07:35:47.000000 ngmapi-0.0.39/ngmapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-09 07:35:47.000000 ngmapi-0.0.39/ngmapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-09 07:35:07.000000 ngmapi-0.0.39/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 07:35:47.382094 ngmapi-0.0.39/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:35:47.382094 ngmapi-0.0.39/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-09 07:35:07.000000 ngmapi-0.0.39/tests/test_add.py
```

