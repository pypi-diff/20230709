# Comparing `tmp/sicdeploy-0.2.1rc2.tar.gz` & `tmp/sicdeploy-0.2.1rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sicdeploy-0.2.1rc2.tar", last modified: Sun Jul  9 13:27:33 2023, max compression
+gzip compressed data, was "sicdeploy-0.2.1rc3.tar", last modified: Sun Jul  9 13:42:51 2023, max compression
```

## Comparing `sicdeploy-0.2.1rc2.tar` & `sicdeploy-0.2.1rc3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:27:33.788912 sicdeploy-0.2.1rc2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-09 13:27:15.000000 sicdeploy-0.2.1rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-09 13:27:33.788912 sicdeploy-0.2.1rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-09 13:27:15.000000 sicdeploy-0.2.1rc2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 13:27:33.788912 sicdeploy-0.2.1rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-09 13:27:15.000000 sicdeploy-0.2.1rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:27:33.788912 sicdeploy-0.2.1rc2/sicd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 13:27:15.000000 sicdeploy-0.2.1rc2/sicd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-09 13:27:15.000000 sicdeploy-0.2.1rc2/sicd/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-09 13:27:15.000000 sicdeploy-0.2.1rc2/sicd/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:27:33.788912 sicdeploy-0.2.1rc2/sicdeploy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-09 13:27:33.000000 sicdeploy-0.2.1rc2/sicdeploy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-09 13:27:33.000000 sicdeploy-0.2.1rc2/sicdeploy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 13:27:33.000000 sicdeploy-0.2.1rc2/sicdeploy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-09 13:27:33.000000 sicdeploy-0.2.1rc2/sicdeploy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-09 13:27:33.000000 sicdeploy-0.2.1rc2/sicdeploy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-09 13:27:33.000000 sicdeploy-0.2.1rc2/sicdeploy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:42:51.274788 sicdeploy-0.2.1rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-09 13:42:31.000000 sicdeploy-0.2.1rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-09 13:42:51.274788 sicdeploy-0.2.1rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-09 13:42:31.000000 sicdeploy-0.2.1rc3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 13:42:51.274788 sicdeploy-0.2.1rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-09 13:42:31.000000 sicdeploy-0.2.1rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:42:51.274788 sicdeploy-0.2.1rc3/sicd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 13:42:31.000000 sicdeploy-0.2.1rc3/sicd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-09 13:42:31.000000 sicdeploy-0.2.1rc3/sicd/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-09 13:42:31.000000 sicdeploy-0.2.1rc3/sicd/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:42:51.274788 sicdeploy-0.2.1rc3/sicdeploy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-09 13:42:51.000000 sicdeploy-0.2.1rc3/sicdeploy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-09 13:42:51.000000 sicdeploy-0.2.1rc3/sicdeploy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 13:42:51.000000 sicdeploy-0.2.1rc3/sicdeploy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-09 13:42:51.000000 sicdeploy-0.2.1rc3/sicdeploy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-09 13:42:51.000000 sicdeploy-0.2.1rc3/sicdeploy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-09 13:42:51.000000 sicdeploy-0.2.1rc3/sicdeploy.egg-info/top_level.txt
```

### Comparing `sicdeploy-0.2.1rc2/LICENSE` & `sicdeploy-0.2.1rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `sicdeploy-0.2.1rc2/README.rst` & `sicdeploy-0.2.1rc3/README.rst`

 * *Files identical despite different names*

