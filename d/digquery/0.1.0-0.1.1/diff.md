# Comparing `tmp/digquery-0.1.0.tar.gz` & `tmp/digquery-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digquery-0.1.0.tar", last modified: Sun Jul  9 14:42:30 2023, max compression
+gzip compressed data, was "digquery-0.1.1.tar", last modified: Sun Jul  9 14:56:41 2023, max compression
```

## Comparing `digquery-0.1.0.tar` & `digquery-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 14:42:30.174419 digquery-0.1.0/
--rw-r--r--   0 root         (0) root         (0)      549 2023-07-09 14:42:30.174419 digquery-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-09 14:26:52.000000 digquery-0.1.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 14:42:30.174419 digquery-0.1.0/digquery/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-09 14:25:25.000000 digquery-0.1.0/digquery/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1595 2023-07-09 14:31:20.000000 digquery-0.1.0/digquery/dig_query_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 14:42:30.174419 digquery-0.1.0/digquery.egg-info/
--rw-r--r--   0 root         (0) root         (0)      549 2023-07-09 14:42:30.000000 digquery-0.1.0/digquery.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      231 2023-07-09 14:42:30.000000 digquery-0.1.0/digquery.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 14:42:30.000000 digquery-0.1.0/digquery.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      135 2023-07-09 14:42:30.000000 digquery-0.1.0/digquery.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-09 14:42:30.000000 digquery-0.1.0/digquery.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-09 14:42:30.174419 digquery-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      830 2023-07-09 14:39:11.000000 digquery-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 14:56:41.264432 digquery-0.1.1/
+-rw-r--r--   0 root         (0) root         (0)      589 2023-07-09 14:56:41.264432 digquery-0.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-09 14:26:52.000000 digquery-0.1.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 14:56:41.264432 digquery-0.1.1/digquery/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-09 14:25:25.000000 digquery-0.1.1/digquery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-07-09 14:31:20.000000 digquery-0.1.1/digquery/dig_query_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 14:56:41.264432 digquery-0.1.1/digquery.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      589 2023-07-09 14:56:41.000000 digquery-0.1.1/digquery.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      231 2023-07-09 14:56:41.000000 digquery-0.1.1/digquery.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 14:56:41.000000 digquery-0.1.1/digquery.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      135 2023-07-09 14:56:41.000000 digquery-0.1.1/digquery.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-09 14:56:41.000000 digquery-0.1.1/digquery.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-09 14:56:41.264432 digquery-0.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      987 2023-07-09 14:56:31.000000 digquery-0.1.1/setup.py
```

### Comparing `digquery-0.1.0/PKG-INFO` & `digquery-0.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: digquery
-Version: 0.1.0
+Version: 0.1.1
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
+Description-Content-Type: text/markdown
```

### Comparing `digquery-0.1.0/digquery/dig_query_types.py` & `digquery-0.1.1/digquery/dig_query_types.py`

 * *Files identical despite different names*

### Comparing `digquery-0.1.0/digquery.egg-info/PKG-INFO` & `digquery-0.1.1/digquery.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: digquery
-Version: 0.1.0
+Version: 0.1.1
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
+Description-Content-Type: text/markdown
```

### Comparing `digquery-0.1.0/setup.py` & `digquery-0.1.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from setuptools import setup
 
+with open('README.md', 'r') as f:
+    long_description = f.read()
+
 setup(
     name='digquery',
-    version='0.1.0',
+    version='0.1.1',
     author='Jay',
     author_email='techdjay@gmail.com',
     description='A Python package for querying DNS information using dig',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     packages=['digquery'],
     	entry_points={
 		'console_scripts': [
 			'digquery = digquery.dig_query_types:main',
 			'pydig = digquery.dig_query_types:main',
 			'mydig = digquery.dig_query_types:main',
 		]
```

