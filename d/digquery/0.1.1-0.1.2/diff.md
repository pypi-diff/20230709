# Comparing `tmp/digquery-0.1.1.tar.gz` & `tmp/digquery-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digquery-0.1.1.tar", last modified: Sun Jul  9 14:56:41 2023, max compression
+gzip compressed data, was "digquery-0.1.2.tar", last modified: Sun Jul  9 15:03:02 2023, max compression
```

## Comparing `digquery-0.1.1.tar` & `digquery-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 14:56:41.264432 digquery-0.1.1/
--rw-r--r--   0 root         (0) root         (0)      589 2023-07-09 14:56:41.264432 digquery-0.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-09 14:26:52.000000 digquery-0.1.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 14:56:41.264432 digquery-0.1.1/digquery/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-09 14:25:25.000000 digquery-0.1.1/digquery/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1595 2023-07-09 14:31:20.000000 digquery-0.1.1/digquery/dig_query_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 14:56:41.264432 digquery-0.1.1/digquery.egg-info/
--rw-r--r--   0 root         (0) root         (0)      589 2023-07-09 14:56:41.000000 digquery-0.1.1/digquery.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      231 2023-07-09 14:56:41.000000 digquery-0.1.1/digquery.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 14:56:41.000000 digquery-0.1.1/digquery.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      135 2023-07-09 14:56:41.000000 digquery-0.1.1/digquery.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-09 14:56:41.000000 digquery-0.1.1/digquery.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-09 14:56:41.264432 digquery-0.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      987 2023-07-09 14:56:31.000000 digquery-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:03:02.604438 digquery-0.1.2/
+-rw-r--r--   0 root         (0) root         (0)      549 2023-07-09 15:03:02.604438 digquery-0.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-09 14:26:52.000000 digquery-0.1.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:03:02.594438 digquery-0.1.2/digquery/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-09 14:25:25.000000 digquery-0.1.2/digquery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-07-09 14:31:20.000000 digquery-0.1.2/digquery/dig_query_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:03:02.604438 digquery-0.1.2/digquery.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      549 2023-07-09 15:03:02.000000 digquery-0.1.2/digquery.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      231 2023-07-09 15:03:02.000000 digquery-0.1.2/digquery.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 15:03:02.000000 digquery-0.1.2/digquery.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      135 2023-07-09 15:03:02.000000 digquery-0.1.2/digquery.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-09 15:03:02.000000 digquery-0.1.2/digquery.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-09 15:03:02.604438 digquery-0.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      972 2023-07-09 15:02:50.000000 digquery-0.1.2/setup.py
```

### Comparing `digquery-0.1.1/PKG-INFO` & `digquery-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: digquery
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python package for querying DNS information using dig
 Author: Jay
 Author-email: techdjay@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
```

### Comparing `digquery-0.1.1/digquery/dig_query_types.py` & `digquery-0.1.2/digquery/dig_query_types.py`

 * *Files identical despite different names*

### Comparing `digquery-0.1.1/digquery.egg-info/PKG-INFO` & `digquery-0.1.2/digquery.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: digquery
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python package for querying DNS information using dig
 Author: Jay
 Author-email: techdjay@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
```

### Comparing `digquery-0.1.1/setup.py` & `digquery-0.1.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,19 @@
+import os
 from setuptools import setup
 
-with open('README.md', 'r') as f:
-    long_description = f.read()
-
+with open(os.path.join(os.path.dirname(__file__), 'README.rst')) as readme:
+    README = readme.read()
 setup(
     name='digquery',
-    version='0.1.1',
+    version='0.1.2',
     author='Jay',
     author_email='techdjay@gmail.com',
     description='A Python package for querying DNS information using dig',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
+    long_description=README,
     packages=['digquery'],
     	entry_points={
 		'console_scripts': [
 			'digquery = digquery.dig_query_types:main',
 			'pydig = digquery.dig_query_types:main',
 			'mydig = digquery.dig_query_types:main',
 		]
```

