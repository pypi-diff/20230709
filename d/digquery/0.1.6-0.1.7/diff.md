# Comparing `tmp/digquery-0.1.6.tar.gz` & `tmp/digquery-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digquery-0.1.6.tar", last modified: Sun Jul  9 16:19:55 2023, max compression
+gzip compressed data, was "digquery-0.1.7.tar", last modified: Sun Jul  9 16:53:10 2023, max compression
```

## Comparing `digquery-0.1.6.tar` & `digquery-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 16:19:55.404509 digquery-0.1.6/
--rw-r--r--   0 root         (0) root         (0)     1610 2023-07-09 16:19:55.404509 digquery-0.1.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1012 2023-07-09 16:12:31.000000 digquery-0.1.6/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 16:19:55.404509 digquery-0.1.6/digquery/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-09 14:25:25.000000 digquery-0.1.6/digquery/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1595 2023-07-09 14:31:20.000000 digquery-0.1.6/digquery/dig_query_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 16:19:55.404509 digquery-0.1.6/digquery.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1610 2023-07-09 16:19:55.000000 digquery-0.1.6/digquery.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      231 2023-07-09 16:19:55.000000 digquery-0.1.6/digquery.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 16:19:55.000000 digquery-0.1.6/digquery.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      135 2023-07-09 16:19:55.000000 digquery-0.1.6/digquery.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-09 16:19:55.000000 digquery-0.1.6/digquery.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-09 16:19:55.404509 digquery-0.1.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1020 2023-07-09 16:19:44.000000 digquery-0.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 16:53:10.124540 digquery-0.1.7/
+-rw-r--r--   0 root         (0) root         (0)     3893 2023-07-09 16:53:10.124540 digquery-0.1.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3295 2023-07-09 16:49:08.000000 digquery-0.1.7/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 16:53:10.124540 digquery-0.1.7/digquery/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-09 14:25:25.000000 digquery-0.1.7/digquery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-07-09 14:31:20.000000 digquery-0.1.7/digquery/dig_query_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 16:53:10.124540 digquery-0.1.7/digquery.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3893 2023-07-09 16:53:10.000000 digquery-0.1.7/digquery.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      231 2023-07-09 16:53:10.000000 digquery-0.1.7/digquery.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 16:53:10.000000 digquery-0.1.7/digquery.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      135 2023-07-09 16:53:10.000000 digquery-0.1.7/digquery.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-09 16:53:10.000000 digquery-0.1.7/digquery.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-09 16:53:10.124540 digquery-0.1.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-07-09 16:52:44.000000 digquery-0.1.7/setup.py
```

### Comparing `digquery-0.1.6/digquery/dig_query_types.py` & `digquery-0.1.7/digquery/dig_query_types.py`

 * *Files identical despite different names*

### Comparing `digquery-0.1.6/setup.py` & `digquery-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import setup
 
 with open(os.path.join(os.path.dirname(__file__), 'README.rst')) as readme:
     README = readme.read()
 setup(
     name='digquery',
-    version='0.1.6',
+    version='0.1.7',
     author='Jay',
     url='https://github.com/techdjay/digquery',
     author_email='techdjay@gmail.com',
     description='A Python package for querying DNS information using dig',
     long_description=README,
     packages=['digquery'],
     	entry_points={
```

