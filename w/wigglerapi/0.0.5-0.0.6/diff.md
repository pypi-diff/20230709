# Comparing `tmp/wigglerapi-0.0.5.tar.gz` & `tmp/wigglerapi-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wigglerapi-0.0.5.tar", last modified: Sun Jul  9 20:03:17 2023, max compression
+gzip compressed data, was "wigglerapi-0.0.6.tar", last modified: Sun Jul  9 20:08:30 2023, max compression
```

## Comparing `wigglerapi-0.0.5.tar` & `wigglerapi-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-09 20:03:17.783080 wigglerapi-0.0.5/
--rw-r--r--   0 vincent    (501) staff       (20)      301 2023-07-09 20:03:17.782947 wigglerapi-0.0.5/PKG-INFO
--rw-r--r--   0 vincent    (501) staff       (20)       38 2023-07-09 20:03:17.783115 wigglerapi-0.0.5/setup.cfg
--rw-r--r--   0 vincent    (501) staff       (20)      718 2023-07-09 20:02:01.000000 wigglerapi-0.0.5/setup.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-09 20:03:17.781650 wigglerapi-0.0.5/wigglerapi/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-07-09 16:41:51.000000 wigglerapi-0.0.5/wigglerapi/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)      319 2023-07-09 19:49:49.000000 wigglerapi-0.0.5/wigglerapi/cli.py
--rw-r--r--   0 vincent    (501) staff       (20)      698 2023-07-09 16:47:54.000000 wigglerapi-0.0.5/wigglerapi/main.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-09 20:03:17.782650 wigglerapi-0.0.5/wigglerapi.egg-info/
--rw-r--r--   0 vincent    (501) staff       (20)      301 2023-07-09 20:03:17.000000 wigglerapi-0.0.5/wigglerapi.egg-info/PKG-INFO
--rw-r--r--   0 vincent    (501) staff       (20)      274 2023-07-09 20:03:17.000000 wigglerapi-0.0.5/wigglerapi.egg-info/SOURCES.txt
--rw-r--r--   0 vincent    (501) staff       (20)        1 2023-07-09 20:03:17.000000 wigglerapi-0.0.5/wigglerapi.egg-info/dependency_links.txt
--rw-r--r--   0 vincent    (501) staff       (20)       48 2023-07-09 20:03:17.000000 wigglerapi-0.0.5/wigglerapi.egg-info/entry_points.txt
--rw-r--r--   0 vincent    (501) staff       (20)       25 2023-07-09 20:03:17.000000 wigglerapi-0.0.5/wigglerapi.egg-info/requires.txt
--rw-r--r--   0 vincent    (501) staff       (20)       11 2023-07-09 20:03:17.000000 wigglerapi-0.0.5/wigglerapi.egg-info/top_level.txt
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-09 20:08:30.097316 wigglerapi-0.0.6/
+-rw-r--r--   0 vincent    (501) staff       (20)      301 2023-07-09 20:08:30.097172 wigglerapi-0.0.6/PKG-INFO
+-rw-r--r--   0 vincent    (501) staff       (20)       38 2023-07-09 20:08:30.097354 wigglerapi-0.0.6/setup.cfg
+-rw-r--r--   0 vincent    (501) staff       (20)      718 2023-07-09 20:08:20.000000 wigglerapi-0.0.6/setup.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-09 20:08:30.095826 wigglerapi-0.0.6/wigglerapi/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-07-09 16:41:51.000000 wigglerapi-0.0.6/wigglerapi/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)      306 2023-07-09 20:07:36.000000 wigglerapi-0.0.6/wigglerapi/cli.py
+-rw-r--r--   0 vincent    (501) staff       (20)      698 2023-07-09 16:47:54.000000 wigglerapi-0.0.6/wigglerapi/main.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-09 20:08:30.096998 wigglerapi-0.0.6/wigglerapi.egg-info/
+-rw-r--r--   0 vincent    (501) staff       (20)      301 2023-07-09 20:08:30.000000 wigglerapi-0.0.6/wigglerapi.egg-info/PKG-INFO
+-rw-r--r--   0 vincent    (501) staff       (20)      274 2023-07-09 20:08:30.000000 wigglerapi-0.0.6/wigglerapi.egg-info/SOURCES.txt
+-rw-r--r--   0 vincent    (501) staff       (20)        1 2023-07-09 20:08:30.000000 wigglerapi-0.0.6/wigglerapi.egg-info/dependency_links.txt
+-rw-r--r--   0 vincent    (501) staff       (20)       48 2023-07-09 20:08:30.000000 wigglerapi-0.0.6/wigglerapi.egg-info/entry_points.txt
+-rw-r--r--   0 vincent    (501) staff       (20)       25 2023-07-09 20:08:30.000000 wigglerapi-0.0.6/wigglerapi.egg-info/requires.txt
+-rw-r--r--   0 vincent    (501) staff       (20)       11 2023-07-09 20:08:30.000000 wigglerapi-0.0.6/wigglerapi.egg-info/top_level.txt
```

### Comparing `wigglerapi-0.0.5/setup.py` & `wigglerapi-0.0.6/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'WiggleR - Desktop research unit for making controlled experiments'
 LONG_DESCRIPTION = 'WiggleR is a desktop research unit for making controlled experiments with worms. WiggleR can also be used inside the WiggleBin'
 
 setup(
     name="wigglerapi",
     version=VERSION,
     author="Vincent Kranendonk",
```

### Comparing `wigglerapi-0.0.5/wigglerapi/main.py` & `wigglerapi-0.0.6/wigglerapi/main.py`

 * *Files identical despite different names*

