# Comparing `tmp/sydeploy-0.2.1rc4.tar.gz` & `tmp/sydeploy-0.2.1rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sydeploy-0.2.1rc4.tar", last modified: Sun Jul  9 13:55:13 2023, max compression
+gzip compressed data, was "sydeploy-0.2.1rc5.tar", last modified: Sun Jul  9 13:59:40 2023, max compression
```

## Comparing `sydeploy-0.2.1rc4.tar` & `sydeploy-0.2.1rc5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:55:13.539614 sydeploy-0.2.1rc4/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-09 13:54:55.000000 sydeploy-0.2.1rc4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-09 13:55:13.539614 sydeploy-0.2.1rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-09 13:54:55.000000 sydeploy-0.2.1rc4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 13:55:13.539614 sydeploy-0.2.1rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-09 13:54:55.000000 sydeploy-0.2.1rc4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:55:13.535614 sydeploy-0.2.1rc4/syd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 13:54:55.000000 sydeploy-0.2.1rc4/syd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-09 13:54:55.000000 sydeploy-0.2.1rc4/syd/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-09 13:54:55.000000 sydeploy-0.2.1rc4/syd/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:55:13.535614 sydeploy-0.2.1rc4/syd/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-09 13:54:55.000000 sydeploy-0.2.1rc4/syd/templates/meta.yaml.dist
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-09 13:54:55.000000 sydeploy-0.2.1rc4/syd/templates/setup.py.dist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:55:13.535614 sydeploy-0.2.1rc4/syd/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-09 13:54:55.000000 sydeploy-0.2.1rc4/syd/utils/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:55:13.539614 sydeploy-0.2.1rc4/sydeploy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-09 13:55:13.000000 sydeploy-0.2.1rc4/sydeploy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-09 13:55:13.000000 sydeploy-0.2.1rc4/sydeploy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 13:55:13.000000 sydeploy-0.2.1rc4/sydeploy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 13:55:13.000000 sydeploy-0.2.1rc4/sydeploy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-09 13:55:13.000000 sydeploy-0.2.1rc4/sydeploy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-09 13:55:13.000000 sydeploy-0.2.1rc4/sydeploy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:59:40.690702 sydeploy-0.2.1rc5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-09 13:59:19.000000 sydeploy-0.2.1rc5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-09 13:59:40.690702 sydeploy-0.2.1rc5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-09 13:59:19.000000 sydeploy-0.2.1rc5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 13:59:40.690702 sydeploy-0.2.1rc5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-09 13:59:19.000000 sydeploy-0.2.1rc5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:59:40.690702 sydeploy-0.2.1rc5/syd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 13:59:19.000000 sydeploy-0.2.1rc5/syd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-09 13:59:19.000000 sydeploy-0.2.1rc5/syd/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-09 13:59:19.000000 sydeploy-0.2.1rc5/syd/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:59:40.690702 sydeploy-0.2.1rc5/syd/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-09 13:59:19.000000 sydeploy-0.2.1rc5/syd/templates/meta.yaml.dist
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-09 13:59:19.000000 sydeploy-0.2.1rc5/syd/templates/setup.py.dist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:59:40.690702 sydeploy-0.2.1rc5/syd/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-09 13:59:19.000000 sydeploy-0.2.1rc5/syd/utils/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:59:40.690702 sydeploy-0.2.1rc5/sydeploy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-09 13:59:40.000000 sydeploy-0.2.1rc5/sydeploy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-09 13:59:40.000000 sydeploy-0.2.1rc5/sydeploy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 13:59:40.000000 sydeploy-0.2.1rc5/sydeploy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 13:59:40.000000 sydeploy-0.2.1rc5/sydeploy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-09 13:59:40.000000 sydeploy-0.2.1rc5/sydeploy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-09 13:59:40.000000 sydeploy-0.2.1rc5/sydeploy.egg-info/top_level.txt
```

### Comparing `sydeploy-0.2.1rc4/LICENSE` & `sydeploy-0.2.1rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `sydeploy-0.2.1rc4/README.rst` & `sydeploy-0.2.1rc5/README.rst`

 * *Files identical despite different names*

### Comparing `sydeploy-0.2.1rc4/syd/utils/simple.py` & `sydeploy-0.2.1rc5/syd/utils/simple.py`

 * *Files identical despite different names*

