# Comparing `tmp/wiggler-0.0.1.tar.gz` & `tmp/wiggler-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiggler-0.0.1.tar", last modified: Fri Jun 30 10:52:05 2023, max compression
+gzip compressed data, was "wiggler-0.0.2.tar", last modified: Fri Jun 30 12:45:30 2023, max compression
```

## Comparing `wiggler-0.0.1.tar` & `wiggler-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 10:52:05.589380 wiggler-0.0.1/
--rw-r--r--   0 vincent    (501) staff       (20)      298 2023-06-30 10:52:05.589227 wiggler-0.0.1/PKG-INFO
--rw-r--r--   0 vincent    (501) staff       (20)       38 2023-06-30 10:52:05.589425 wiggler-0.0.1/setup.cfg
--rw-r--r--   0 vincent    (501) staff       (20)      544 2023-06-30 10:37:33.000000 wiggler-0.0.1/setup.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 10:52:05.588219 wiggler-0.0.1/wiggler/
--rw-r--r--   0 vincent    (501) staff       (20)       38 2023-06-30 10:33:24.000000 wiggler-0.0.1/wiggler/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     4087 2023-06-30 10:51:18.000000 wiggler-0.0.1/wiggler/timelapse.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 10:52:05.589018 wiggler-0.0.1/wiggler.egg-info/
--rw-r--r--   0 vincent    (501) staff       (20)      298 2023-06-30 10:52:05.000000 wiggler-0.0.1/wiggler.egg-info/PKG-INFO
--rw-r--r--   0 vincent    (501) staff       (20)      173 2023-06-30 10:52:05.000000 wiggler-0.0.1/wiggler.egg-info/SOURCES.txt
--rw-r--r--   0 vincent    (501) staff       (20)        1 2023-06-30 10:52:05.000000 wiggler-0.0.1/wiggler.egg-info/dependency_links.txt
--rw-r--r--   0 vincent    (501) staff       (20)        8 2023-06-30 10:52:05.000000 wiggler-0.0.1/wiggler.egg-info/top_level.txt
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 12:45:30.567372 wiggler-0.0.2/
+-rw-r--r--   0 vincent    (501) staff       (20)      298 2023-06-30 12:45:30.567237 wiggler-0.0.2/PKG-INFO
+-rw-r--r--   0 vincent    (501) staff       (20)       38 2023-06-30 12:45:30.567420 wiggler-0.0.2/setup.cfg
+-rw-r--r--   0 vincent    (501) staff       (20)      544 2023-06-30 10:53:15.000000 wiggler-0.0.2/setup.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 12:45:30.566188 wiggler-0.0.2/wiggler/
+-rw-r--r--   0 vincent    (501) staff       (20)       37 2023-06-30 12:45:16.000000 wiggler-0.0.2/wiggler/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     4087 2023-06-30 10:51:18.000000 wiggler-0.0.2/wiggler/timelapse.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 12:45:30.567040 wiggler-0.0.2/wiggler.egg-info/
+-rw-r--r--   0 vincent    (501) staff       (20)      298 2023-06-30 12:45:30.000000 wiggler-0.0.2/wiggler.egg-info/PKG-INFO
+-rw-r--r--   0 vincent    (501) staff       (20)      173 2023-06-30 12:45:30.000000 wiggler-0.0.2/wiggler.egg-info/SOURCES.txt
+-rw-r--r--   0 vincent    (501) staff       (20)        1 2023-06-30 12:45:30.000000 wiggler-0.0.2/wiggler.egg-info/dependency_links.txt
+-rw-r--r--   0 vincent    (501) staff       (20)        8 2023-06-30 12:45:30.000000 wiggler-0.0.2/wiggler.egg-info/top_level.txt
```

### Comparing `wiggler-0.0.1/setup.py` & `wiggler-0.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'WiggleR - Desktop research unit for making controlled experiments'
 LONG_DESCRIPTION = 'WiggleR is a desktop research unit for making controlled experiments with worms. WiggleR can also be used inside the WiggleBin'
 
 setup(
     name="wiggler",
     version=VERSION,
     author="Vincent Kranendonk",
```

### Comparing `wiggler-0.0.1/wiggler/timelapse.py` & `wiggler-0.0.2/wiggler/timelapse.py`

 * *Files identical despite different names*

