# Comparing `tmp/sydeploy-0.2.1rc6.tar.gz` & `tmp/sydeploy-0.2.1rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sydeploy-0.2.1rc6.tar", last modified: Sun Jul  9 14:10:07 2023, max compression
+gzip compressed data, was "sydeploy-0.2.1rc7.tar", last modified: Sun Jul  9 14:18:28 2023, max compression
```

## Comparing `sydeploy-0.2.1rc6.tar` & `sydeploy-0.2.1rc7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:10:07.412795 sydeploy-0.2.1rc6/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-09 14:09:45.000000 sydeploy-0.2.1rc6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-09 14:10:07.412795 sydeploy-0.2.1rc6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-09 14:09:45.000000 sydeploy-0.2.1rc6/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 14:10:07.412795 sydeploy-0.2.1rc6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-09 14:09:45.000000 sydeploy-0.2.1rc6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:10:07.412795 sydeploy-0.2.1rc6/syd/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-09 14:09:45.000000 sydeploy-0.2.1rc6/syd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-09 14:09:45.000000 sydeploy-0.2.1rc6/syd/run.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-09 14:09:45.000000 sydeploy-0.2.1rc6/syd/syd_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:10:07.412795 sydeploy-0.2.1rc6/syd/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-09 14:09:45.000000 sydeploy-0.2.1rc6/syd/templates/meta.yaml.dist
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-09 14:09:45.000000 sydeploy-0.2.1rc6/syd/templates/setup.py.dist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:10:07.412795 sydeploy-0.2.1rc6/syd/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-09 14:09:45.000000 sydeploy-0.2.1rc6/syd/utils/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:10:07.412795 sydeploy-0.2.1rc6/sydeploy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-09 14:10:07.000000 sydeploy-0.2.1rc6/sydeploy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-09 14:10:07.000000 sydeploy-0.2.1rc6/sydeploy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 14:10:07.000000 sydeploy-0.2.1rc6/sydeploy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-09 14:10:07.000000 sydeploy-0.2.1rc6/sydeploy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-09 14:10:07.000000 sydeploy-0.2.1rc6/sydeploy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-09 14:10:07.000000 sydeploy-0.2.1rc6/sydeploy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:18:28.351464 sydeploy-0.2.1rc7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-09 14:18:08.000000 sydeploy-0.2.1rc7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-09 14:18:28.351464 sydeploy-0.2.1rc7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-09 14:18:08.000000 sydeploy-0.2.1rc7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 14:18:28.351464 sydeploy-0.2.1rc7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-09 14:18:08.000000 sydeploy-0.2.1rc7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:18:28.351464 sydeploy-0.2.1rc7/syd/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-09 14:18:08.000000 sydeploy-0.2.1rc7/syd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-09 14:18:08.000000 sydeploy-0.2.1rc7/syd/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-09 14:18:08.000000 sydeploy-0.2.1rc7/syd/syd_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:18:28.351464 sydeploy-0.2.1rc7/syd/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-09 14:18:08.000000 sydeploy-0.2.1rc7/syd/templates/meta.yaml.dist
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-09 14:18:08.000000 sydeploy-0.2.1rc7/syd/templates/setup.py.dist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:18:28.351464 sydeploy-0.2.1rc7/syd/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-09 14:18:08.000000 sydeploy-0.2.1rc7/syd/utils/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:18:28.351464 sydeploy-0.2.1rc7/sydeploy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-09 14:18:28.000000 sydeploy-0.2.1rc7/sydeploy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-09 14:18:28.000000 sydeploy-0.2.1rc7/sydeploy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 14:18:28.000000 sydeploy-0.2.1rc7/sydeploy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-09 14:18:28.000000 sydeploy-0.2.1rc7/sydeploy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-09 14:18:28.000000 sydeploy-0.2.1rc7/sydeploy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-09 14:18:28.000000 sydeploy-0.2.1rc7/sydeploy.egg-info/top_level.txt
```

### Comparing `sydeploy-0.2.1rc6/LICENSE` & `sydeploy-0.2.1rc7/LICENSE`

 * *Files identical despite different names*

### Comparing `sydeploy-0.2.1rc6/README.rst` & `sydeploy-0.2.1rc7/README.rst`

 * *Files identical despite different names*

### Comparing `sydeploy-0.2.1rc6/syd/utils/simple.py` & `sydeploy-0.2.1rc7/syd/utils/simple.py`

 * *Files identical despite different names*

