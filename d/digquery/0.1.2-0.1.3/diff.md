# Comparing `tmp/digquery-0.1.2.tar.gz` & `tmp/digquery-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digquery-0.1.2.tar", last modified: Sun Jul  9 15:03:02 2023, max compression
+gzip compressed data, was "digquery-0.1.3.tar", last modified: Sun Jul  9 15:13:59 2023, max compression
```

## Comparing `digquery-0.1.2.tar` & `digquery-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:03:02.604438 digquery-0.1.2/
--rw-r--r--   0 root         (0) root         (0)      549 2023-07-09 15:03:02.604438 digquery-0.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-09 14:26:52.000000 digquery-0.1.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:03:02.594438 digquery-0.1.2/digquery/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-09 14:25:25.000000 digquery-0.1.2/digquery/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1595 2023-07-09 14:31:20.000000 digquery-0.1.2/digquery/dig_query_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:03:02.604438 digquery-0.1.2/digquery.egg-info/
--rw-r--r--   0 root         (0) root         (0)      549 2023-07-09 15:03:02.000000 digquery-0.1.2/digquery.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      231 2023-07-09 15:03:02.000000 digquery-0.1.2/digquery.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 15:03:02.000000 digquery-0.1.2/digquery.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      135 2023-07-09 15:03:02.000000 digquery-0.1.2/digquery.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-09 15:03:02.000000 digquery-0.1.2/digquery.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-09 15:03:02.604438 digquery-0.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      972 2023-07-09 15:02:50.000000 digquery-0.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:13:59.224448 digquery-0.1.3/
+-rw-r--r--   0 root         (0) root         (0)     1486 2023-07-09 15:13:59.224448 digquery-0.1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      936 2023-07-09 15:13:09.000000 digquery-0.1.3/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:13:59.224448 digquery-0.1.3/digquery/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-09 14:25:25.000000 digquery-0.1.3/digquery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-07-09 14:31:20.000000 digquery-0.1.3/digquery/dig_query_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:13:59.224448 digquery-0.1.3/digquery.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1486 2023-07-09 15:13:59.000000 digquery-0.1.3/digquery.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      231 2023-07-09 15:13:59.000000 digquery-0.1.3/digquery.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 15:13:59.000000 digquery-0.1.3/digquery.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      135 2023-07-09 15:13:59.000000 digquery-0.1.3/digquery.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-09 15:13:59.000000 digquery-0.1.3/digquery.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-09 15:13:59.224448 digquery-0.1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      972 2023-07-09 15:09:59.000000 digquery-0.1.3/setup.py
```

### Comparing `digquery-0.1.2/digquery/dig_query_types.py` & `digquery-0.1.3/digquery/dig_query_types.py`

 * *Files identical despite different names*

### Comparing `digquery-0.1.2/setup.py` & `digquery-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import setup
 
 with open(os.path.join(os.path.dirname(__file__), 'README.rst')) as readme:
     README = readme.read()
 setup(
     name='digquery',
-    version='0.1.2',
+    version='0.1.3',
     author='Jay',
     author_email='techdjay@gmail.com',
     description='A Python package for querying DNS information using dig',
     long_description=README,
     packages=['digquery'],
     	entry_points={
 		'console_scripts': [
```

