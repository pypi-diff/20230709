# Comparing `tmp/sydeploy-0.2.1rc9.tar.gz` & `tmp/sydeploy-0.2.2rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sydeploy-0.2.1rc9.tar", last modified: Sun Jul  9 14:34:47 2023, max compression
+gzip compressed data, was "sydeploy-0.2.2rc0.tar", last modified: Sun Jul  9 17:06:11 2023, max compression
```

## Comparing `sydeploy-0.2.1rc9.tar` & `sydeploy-0.2.2rc0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:34:47.177923 sydeploy-0.2.1rc9/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-09 14:34:28.000000 sydeploy-0.2.1rc9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-09 14:34:47.177923 sydeploy-0.2.1rc9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-09 14:34:28.000000 sydeploy-0.2.1rc9/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 14:34:47.177923 sydeploy-0.2.1rc9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-09 14:34:28.000000 sydeploy-0.2.1rc9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:34:47.177923 sydeploy-0.2.1rc9/sydeploy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-09 14:34:47.000000 sydeploy-0.2.1rc9/sydeploy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-09 14:34:47.000000 sydeploy-0.2.1rc9/sydeploy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 14:34:47.000000 sydeploy-0.2.1rc9/sydeploy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-09 14:34:47.000000 sydeploy-0.2.1rc9/sydeploy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-09 14:34:47.000000 sydeploy-0.2.1rc9/sydeploy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 14:34:47.000000 sydeploy-0.2.1rc9/sydeploy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:06:11.829573 sydeploy-0.2.2rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-09 17:05:53.000000 sydeploy-0.2.2rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-09 17:06:11.825573 sydeploy-0.2.2rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-09 17:05:53.000000 sydeploy-0.2.2rc0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 17:06:11.829573 sydeploy-0.2.2rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-09 17:05:53.000000 sydeploy-0.2.2rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:06:11.825573 sydeploy-0.2.2rc0/sydeploy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-09 17:06:11.000000 sydeploy-0.2.2rc0/sydeploy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-09 17:06:11.000000 sydeploy-0.2.2rc0/sydeploy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 17:06:11.000000 sydeploy-0.2.2rc0/sydeploy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-09 17:06:11.000000 sydeploy-0.2.2rc0/sydeploy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 17:06:11.000000 sydeploy-0.2.2rc0/sydeploy.egg-info/top_level.txt
```

### Comparing `sydeploy-0.2.1rc9/LICENSE` & `sydeploy-0.2.2rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `sydeploy-0.2.1rc9/README.rst` & `sydeploy-0.2.2rc0/README.rst`

 * *Files identical despite different names*

