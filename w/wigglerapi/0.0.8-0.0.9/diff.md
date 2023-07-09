# Comparing `tmp/wigglerapi-0.0.8.tar.gz` & `tmp/wigglerapi-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wigglerapi-0.0.8.tar", last modified: Sun Jul  9 20:19:17 2023, max compression
+gzip compressed data, was "wigglerapi-0.0.9.tar", last modified: Sun Jul  9 20:24:28 2023, max compression
```

## Comparing `wigglerapi-0.0.8.tar` & `wigglerapi-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-09 20:19:17.636186 wigglerapi-0.0.8/
--rw-r--r--   0 vincent    (501) staff       (20)      301 2023-07-09 20:19:17.636051 wigglerapi-0.0.8/PKG-INFO
--rw-r--r--   0 vincent    (501) staff       (20)       38 2023-07-09 20:19:17.636356 wigglerapi-0.0.8/setup.cfg
--rw-r--r--   0 vincent    (501) staff       (20)      718 2023-07-09 20:18:58.000000 wigglerapi-0.0.8/setup.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-09 20:19:17.634699 wigglerapi-0.0.8/wigglerapi/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-07-09 16:41:51.000000 wigglerapi-0.0.8/wigglerapi/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)      310 2023-07-09 20:18:29.000000 wigglerapi-0.0.8/wigglerapi/cli.py
--rw-r--r--   0 vincent    (501) staff       (20)      698 2023-07-09 16:47:54.000000 wigglerapi-0.0.8/wigglerapi/main.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-09 20:19:17.635835 wigglerapi-0.0.8/wigglerapi.egg-info/
--rw-r--r--   0 vincent    (501) staff       (20)      301 2023-07-09 20:19:17.000000 wigglerapi-0.0.8/wigglerapi.egg-info/PKG-INFO
--rw-r--r--   0 vincent    (501) staff       (20)      274 2023-07-09 20:19:17.000000 wigglerapi-0.0.8/wigglerapi.egg-info/SOURCES.txt
--rw-r--r--   0 vincent    (501) staff       (20)        1 2023-07-09 20:19:17.000000 wigglerapi-0.0.8/wigglerapi.egg-info/dependency_links.txt
--rw-r--r--   0 vincent    (501) staff       (20)       48 2023-07-09 20:19:17.000000 wigglerapi-0.0.8/wigglerapi.egg-info/entry_points.txt
--rw-r--r--   0 vincent    (501) staff       (20)       25 2023-07-09 20:19:17.000000 wigglerapi-0.0.8/wigglerapi.egg-info/requires.txt
--rw-r--r--   0 vincent    (501) staff       (20)       11 2023-07-09 20:19:17.000000 wigglerapi-0.0.8/wigglerapi.egg-info/top_level.txt
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-09 20:24:28.676787 wigglerapi-0.0.9/
+-rw-r--r--   0 vincent    (501) staff       (20)      301 2023-07-09 20:24:28.676658 wigglerapi-0.0.9/PKG-INFO
+-rw-r--r--   0 vincent    (501) staff       (20)       38 2023-07-09 20:24:28.676821 wigglerapi-0.0.9/setup.cfg
+-rw-r--r--   0 vincent    (501) staff       (20)      718 2023-07-09 20:24:12.000000 wigglerapi-0.0.9/setup.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-09 20:24:28.675755 wigglerapi-0.0.9/wigglerapi/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-07-09 16:41:51.000000 wigglerapi-0.0.9/wigglerapi/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)      321 2023-07-09 20:24:07.000000 wigglerapi-0.0.9/wigglerapi/cli.py
+-rw-r--r--   0 vincent    (501) staff       (20)      698 2023-07-09 20:21:50.000000 wigglerapi-0.0.9/wigglerapi/main.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-09 20:24:28.676490 wigglerapi-0.0.9/wigglerapi.egg-info/
+-rw-r--r--   0 vincent    (501) staff       (20)      301 2023-07-09 20:24:28.000000 wigglerapi-0.0.9/wigglerapi.egg-info/PKG-INFO
+-rw-r--r--   0 vincent    (501) staff       (20)      274 2023-07-09 20:24:28.000000 wigglerapi-0.0.9/wigglerapi.egg-info/SOURCES.txt
+-rw-r--r--   0 vincent    (501) staff       (20)        1 2023-07-09 20:24:28.000000 wigglerapi-0.0.9/wigglerapi.egg-info/dependency_links.txt
+-rw-r--r--   0 vincent    (501) staff       (20)       48 2023-07-09 20:24:28.000000 wigglerapi-0.0.9/wigglerapi.egg-info/entry_points.txt
+-rw-r--r--   0 vincent    (501) staff       (20)       25 2023-07-09 20:24:28.000000 wigglerapi-0.0.9/wigglerapi.egg-info/requires.txt
+-rw-r--r--   0 vincent    (501) staff       (20)       11 2023-07-09 20:24:28.000000 wigglerapi-0.0.9/wigglerapi.egg-info/top_level.txt
```

### Comparing `wigglerapi-0.0.8/setup.py` & `wigglerapi-0.0.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'WiggleR - Desktop research unit for making controlled experiments'
 LONG_DESCRIPTION = 'WiggleR is a desktop research unit for making controlled experiments with worms. WiggleR can also be used inside the WiggleBin'
 
 setup(
     name="wigglerapi",
     version=VERSION,
     author="Vincent Kranendonk",
```

### Comparing `wigglerapi-0.0.8/wigglerapi/main.py` & `wigglerapi-0.0.9/wigglerapi/main.py`

 * *Files identical despite different names*

