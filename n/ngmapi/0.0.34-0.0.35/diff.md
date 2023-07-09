# Comparing `tmp/ngmapi-0.0.34.tar.gz` & `tmp/ngmapi-0.0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngmapi-0.0.34.tar", last modified: Sun Jul  9 06:25:34 2023, max compression
+gzip compressed data, was "ngmapi-0.0.35.tar", last modified: Sun Jul  9 06:31:44 2023, max compression
```

## Comparing `ngmapi-0.0.34.tar` & `ngmapi-0.0.35.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:25:34.907031 ngmapi-0.0.34/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-09 06:25:34.907031 ngmapi-0.0.34/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:25:34.907031 ngmapi-0.0.34/ngmapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 06:24:48.000000 ngmapi-0.0.34/ngmapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-09 06:24:48.000000 ngmapi-0.0.34/ngmapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-09 06:24:48.000000 ngmapi-0.0.34/ngmapi/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-09 06:24:48.000000 ngmapi-0.0.34/ngmapi/func.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:25:34.907031 ngmapi-0.0.34/ngmapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-09 06:25:34.000000 ngmapi-0.0.34/ngmapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-09 06:25:34.000000 ngmapi-0.0.34/ngmapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 06:25:34.000000 ngmapi-0.0.34/ngmapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-09 06:25:34.000000 ngmapi-0.0.34/ngmapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-09 06:25:34.000000 ngmapi-0.0.34/ngmapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-09 06:25:34.000000 ngmapi-0.0.34/ngmapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-09 06:24:48.000000 ngmapi-0.0.34/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 06:25:34.907031 ngmapi-0.0.34/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:25:34.907031 ngmapi-0.0.34/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-09 06:24:48.000000 ngmapi-0.0.34/tests/test_add.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:31:44.670313 ngmapi-0.0.35/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-09 06:31:44.670313 ngmapi-0.0.35/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:31:44.666313 ngmapi-0.0.35/ngmapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 06:30:59.000000 ngmapi-0.0.35/ngmapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-09 06:30:59.000000 ngmapi-0.0.35/ngmapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-09 06:30:59.000000 ngmapi-0.0.35/ngmapi/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-09 06:30:59.000000 ngmapi-0.0.35/ngmapi/func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:31:44.670313 ngmapi-0.0.35/ngmapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-09 06:31:44.000000 ngmapi-0.0.35/ngmapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-09 06:31:44.000000 ngmapi-0.0.35/ngmapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 06:31:44.000000 ngmapi-0.0.35/ngmapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-09 06:31:44.000000 ngmapi-0.0.35/ngmapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-09 06:31:44.000000 ngmapi-0.0.35/ngmapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-09 06:31:44.000000 ngmapi-0.0.35/ngmapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-09 06:30:59.000000 ngmapi-0.0.35/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 06:31:44.670313 ngmapi-0.0.35/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:31:44.670313 ngmapi-0.0.35/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-09 06:30:59.000000 ngmapi-0.0.35/tests/test_add.py
```

