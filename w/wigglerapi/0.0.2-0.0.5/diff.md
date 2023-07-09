# Comparing `tmp/wigglerapi-0.0.2.tar.gz` & `tmp/wigglerapi-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wigglerapi-0.0.2.tar", last modified: Sun Jul  9 19:51:00 2023, max compression
+gzip compressed data, was "wigglerapi-0.0.5.tar", last modified: Sun Jul  9 20:03:17 2023, max compression
```

## Comparing `wigglerapi-0.0.2.tar` & `wigglerapi-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-09 19:51:00.425168 wigglerapi-0.0.2/
--rw-r--r--   0 vincent    (501) staff       (20)      301 2023-07-09 19:51:00.424986 wigglerapi-0.0.2/PKG-INFO
--rw-r--r--   0 vincent    (501) staff       (20)       38 2023-07-09 19:51:00.425224 wigglerapi-0.0.2/setup.cfg
--rw-r--r--   0 vincent    (501) staff       (20)      722 2023-07-09 19:50:09.000000 wigglerapi-0.0.2/setup.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-09 19:51:00.423792 wigglerapi-0.0.2/wigglerapi/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-07-09 16:41:51.000000 wigglerapi-0.0.2/wigglerapi/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)      319 2023-07-09 19:49:49.000000 wigglerapi-0.0.2/wigglerapi/cli.py
--rw-r--r--   0 vincent    (501) staff       (20)      698 2023-07-09 16:47:54.000000 wigglerapi-0.0.2/wigglerapi/main.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-09 19:51:00.424785 wigglerapi-0.0.2/wigglerapi.egg-info/
--rw-r--r--   0 vincent    (501) staff       (20)      301 2023-07-09 19:51:00.000000 wigglerapi-0.0.2/wigglerapi.egg-info/PKG-INFO
--rw-r--r--   0 vincent    (501) staff       (20)      274 2023-07-09 19:51:00.000000 wigglerapi-0.0.2/wigglerapi.egg-info/SOURCES.txt
--rw-r--r--   0 vincent    (501) staff       (20)        1 2023-07-09 19:51:00.000000 wigglerapi-0.0.2/wigglerapi.egg-info/dependency_links.txt
--rw-r--r--   0 vincent    (501) staff       (20)       52 2023-07-09 19:51:00.000000 wigglerapi-0.0.2/wigglerapi.egg-info/entry_points.txt
--rw-r--r--   0 vincent    (501) staff       (20)       25 2023-07-09 19:51:00.000000 wigglerapi-0.0.2/wigglerapi.egg-info/requires.txt
--rw-r--r--   0 vincent    (501) staff       (20)       11 2023-07-09 19:51:00.000000 wigglerapi-0.0.2/wigglerapi.egg-info/top_level.txt
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-09 20:03:17.783080 wigglerapi-0.0.5/
+-rw-r--r--   0 vincent    (501) staff       (20)      301 2023-07-09 20:03:17.782947 wigglerapi-0.0.5/PKG-INFO
+-rw-r--r--   0 vincent    (501) staff       (20)       38 2023-07-09 20:03:17.783115 wigglerapi-0.0.5/setup.cfg
+-rw-r--r--   0 vincent    (501) staff       (20)      718 2023-07-09 20:02:01.000000 wigglerapi-0.0.5/setup.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-09 20:03:17.781650 wigglerapi-0.0.5/wigglerapi/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-07-09 16:41:51.000000 wigglerapi-0.0.5/wigglerapi/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)      319 2023-07-09 19:49:49.000000 wigglerapi-0.0.5/wigglerapi/cli.py
+-rw-r--r--   0 vincent    (501) staff       (20)      698 2023-07-09 16:47:54.000000 wigglerapi-0.0.5/wigglerapi/main.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-09 20:03:17.782650 wigglerapi-0.0.5/wigglerapi.egg-info/
+-rw-r--r--   0 vincent    (501) staff       (20)      301 2023-07-09 20:03:17.000000 wigglerapi-0.0.5/wigglerapi.egg-info/PKG-INFO
+-rw-r--r--   0 vincent    (501) staff       (20)      274 2023-07-09 20:03:17.000000 wigglerapi-0.0.5/wigglerapi.egg-info/SOURCES.txt
+-rw-r--r--   0 vincent    (501) staff       (20)        1 2023-07-09 20:03:17.000000 wigglerapi-0.0.5/wigglerapi.egg-info/dependency_links.txt
+-rw-r--r--   0 vincent    (501) staff       (20)       48 2023-07-09 20:03:17.000000 wigglerapi-0.0.5/wigglerapi.egg-info/entry_points.txt
+-rw-r--r--   0 vincent    (501) staff       (20)       25 2023-07-09 20:03:17.000000 wigglerapi-0.0.5/wigglerapi.egg-info/requires.txt
+-rw-r--r--   0 vincent    (501) staff       (20)       11 2023-07-09 20:03:17.000000 wigglerapi-0.0.5/wigglerapi.egg-info/top_level.txt
```

### Comparing `wigglerapi-0.0.2/setup.py` & `wigglerapi-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.5'
 DESCRIPTION = 'WiggleR - Desktop research unit for making controlled experiments'
 LONG_DESCRIPTION = 'WiggleR is a desktop research unit for making controlled experiments with worms. WiggleR can also be used inside the WiggleBin'
 
 setup(
     name="wigglerapi",
     version=VERSION,
     author="Vincent Kranendonk",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     entry_points={
         'console_scripts': [
-            'wiggler = wigglerapi.wiggler:main'
+            'wiggler = wigglerapi.cli:main'
         ]
     },
     install_requires=[
         'fastapi',
         'pydantic',
         'uvicorn'
     ],
```

### Comparing `wigglerapi-0.0.2/wigglerapi/main.py` & `wigglerapi-0.0.5/wigglerapi/main.py`

 * *Files identical despite different names*

