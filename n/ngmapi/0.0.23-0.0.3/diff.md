# Comparing `tmp/ngmapi-0.0.23.tar.gz` & `tmp/ngmapi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngmapi-0.0.23.tar", last modified: Sun Jul  9 05:44:23 2023, max compression
+gzip compressed data, was "ngmapi-0.0.3.tar", last modified: Fri Jul  7 10:16:13 2023, max compression
```

## Comparing `ngmapi-0.0.23.tar` & `ngmapi-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 05:44:23.079969 ngmapi-0.0.23/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-09 05:44:23.079969 ngmapi-0.0.23/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 05:44:23.079969 ngmapi-0.0.23/ngmapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 05:43:32.000000 ngmapi-0.0.23/ngmapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-09 05:43:32.000000 ngmapi-0.0.23/ngmapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-09 05:43:32.000000 ngmapi-0.0.23/ngmapi/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-09 05:43:32.000000 ngmapi-0.0.23/ngmapi/func.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 05:44:23.079969 ngmapi-0.0.23/ngmapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-09 05:44:23.000000 ngmapi-0.0.23/ngmapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-09 05:44:23.000000 ngmapi-0.0.23/ngmapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 05:44:23.000000 ngmapi-0.0.23/ngmapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-09 05:44:23.000000 ngmapi-0.0.23/ngmapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-09 05:44:23.000000 ngmapi-0.0.23/ngmapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-09 05:44:23.000000 ngmapi-0.0.23/ngmapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-09 05:43:32.000000 ngmapi-0.0.23/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 05:44:23.079969 ngmapi-0.0.23/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 05:44:23.079969 ngmapi-0.0.23/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-09 05:43:32.000000 ngmapi-0.0.23/tests/test_add.py
+drwxr-xr-x   0 ngmaibulat   (502) staff       (20)        0 2023-07-07 10:16:13.081674 ngmapi-0.0.3/
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)      375 2023-07-07 10:16:13.081168 ngmapi-0.0.3/PKG-INFO
+drwxr-xr-x   0 ngmaibulat   (502) staff       (20)        0 2023-07-07 10:16:13.075989 ngmapi-0.0.3/ngmapi/
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)        0 2023-07-07 06:42:48.000000 ngmapi-0.0.3/ngmapi/__init__.py
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)       95 2023-07-07 10:11:21.000000 ngmapi-0.0.3/ngmapi/__main__.py
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)      258 2023-07-07 09:46:14.000000 ngmapi-0.0.3/ngmapi/app.py
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)       32 2023-07-07 09:46:31.000000 ngmapi-0.0.3/ngmapi/func.py
+drwxr-xr-x   0 ngmaibulat   (502) staff       (20)        0 2023-07-07 10:16:13.079543 ngmapi-0.0.3/ngmapi.egg-info/
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)      375 2023-07-07 10:16:13.000000 ngmapi-0.0.3/ngmapi.egg-info/PKG-INFO
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)      281 2023-07-07 10:16:13.000000 ngmapi-0.0.3/ngmapi.egg-info/SOURCES.txt
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)        1 2023-07-07 10:16:13.000000 ngmapi-0.0.3/ngmapi.egg-info/dependency_links.txt
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)       48 2023-07-07 10:16:13.000000 ngmapi-0.0.3/ngmapi.egg-info/entry_points.txt
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)       24 2023-07-07 10:16:13.000000 ngmapi-0.0.3/ngmapi.egg-info/requires.txt
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)        7 2023-07-07 10:16:13.000000 ngmapi-0.0.3/ngmapi.egg-info/top_level.txt
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)      550 2023-07-07 10:13:40.000000 ngmapi-0.0.3/pyproject.toml
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)       38 2023-07-07 10:16:13.081836 ngmapi-0.0.3/setup.cfg
+drwxr-xr-x   0 ngmaibulat   (502) staff       (20)        0 2023-07-07 10:16:13.080107 ngmapi-0.0.3/tests/
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)      285 2023-07-07 09:46:42.000000 ngmapi-0.0.3/tests/test_add.py
```

