# Comparing `tmp/digquery-0.1.3.tar.gz` & `tmp/digquery-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digquery-0.1.3.tar", last modified: Sun Jul  9 15:13:59 2023, max compression
+gzip compressed data, was "digquery-0.1.5.tar", last modified: Sun Jul  9 16:13:25 2023, max compression
```

## Comparing `digquery-0.1.3.tar` & `digquery-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:13:59.224448 digquery-0.1.3/
--rw-r--r--   0 root         (0) root         (0)     1486 2023-07-09 15:13:59.224448 digquery-0.1.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      936 2023-07-09 15:13:09.000000 digquery-0.1.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:13:59.224448 digquery-0.1.3/digquery/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-09 14:25:25.000000 digquery-0.1.3/digquery/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1595 2023-07-09 14:31:20.000000 digquery-0.1.3/digquery/dig_query_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:13:59.224448 digquery-0.1.3/digquery.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1486 2023-07-09 15:13:59.000000 digquery-0.1.3/digquery.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      231 2023-07-09 15:13:59.000000 digquery-0.1.3/digquery.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 15:13:59.000000 digquery-0.1.3/digquery.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      135 2023-07-09 15:13:59.000000 digquery-0.1.3/digquery.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-09 15:13:59.000000 digquery-0.1.3/digquery.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-09 15:13:59.224448 digquery-0.1.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      972 2023-07-09 15:09:59.000000 digquery-0.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 16:13:25.224503 digquery-0.1.5/
+-rw-r--r--   0 root         (0) root         (0)     1562 2023-07-09 16:13:25.224503 digquery-0.1.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-07-09 16:12:31.000000 digquery-0.1.5/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 16:13:25.224503 digquery-0.1.5/digquery/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-09 14:25:25.000000 digquery-0.1.5/digquery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-07-09 14:31:20.000000 digquery-0.1.5/digquery/dig_query_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 16:13:25.224503 digquery-0.1.5/digquery.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1562 2023-07-09 16:13:25.000000 digquery-0.1.5/digquery.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      231 2023-07-09 16:13:25.000000 digquery-0.1.5/digquery.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 16:13:25.000000 digquery-0.1.5/digquery.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      135 2023-07-09 16:13:25.000000 digquery-0.1.5/digquery.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-09 16:13:25.000000 digquery-0.1.5/digquery.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-09 16:13:25.224503 digquery-0.1.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      972 2023-07-09 16:12:49.000000 digquery-0.1.5/setup.py
```

### Comparing `digquery-0.1.3/PKG-INFO` & `digquery-0.1.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digquery
-Version: 0.1.3
+Version: 0.1.5
 Summary: A Python package for querying DNS information using dig
 Author: Jay
 Author-email: techdjay@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -36,22 +36,23 @@
 
 .. code-block:: bash
 
     digquery example.com 
     pydig example.com 
     mydig example.com
 
-This will execute separate `dig` commands for each query type (`TXT` and `A`) and display the results.
+This will execute separate `dig` commands for each query type (`A` , `TXT` , `MX`, `NS`) and display the results in clear and crisp format.
 
 Contributing
 ------------
 
 Contributions are welcome! Here are some ways you can contribute:
 
 - Report bugs or suggest improvements by creating a new issue on the `digquery` GitHub repository.
+  https://github.com/techdjay/digquery
 - Fork the repository, make changes, and submit a pull request.
 
 License
 -------
 
 This project is licensed under the MIT License. See the `LICENSE` file for more information.
```

### Comparing `digquery-0.1.3/README.rst` & `digquery-0.1.5/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -21,22 +21,23 @@
 
 .. code-block:: bash
 
     digquery example.com 
     pydig example.com 
     mydig example.com
 
-This will execute separate `dig` commands for each query type (`TXT` and `A`) and display the results.
+This will execute separate `dig` commands for each query type (`A` , `TXT` , `MX`, `NS`) and display the results in clear and crisp format.
 
 Contributing
 ------------
 
 Contributions are welcome! Here are some ways you can contribute:
 
 - Report bugs or suggest improvements by creating a new issue on the `digquery` GitHub repository.
+  https://github.com/techdjay/digquery
 - Fork the repository, make changes, and submit a pull request.
 
 License
 -------
 
 This project is licensed under the MIT License. See the `LICENSE` file for more information.
```

### Comparing `digquery-0.1.3/digquery/dig_query_types.py` & `digquery-0.1.5/digquery/dig_query_types.py`

 * *Files identical despite different names*

### Comparing `digquery-0.1.3/digquery.egg-info/PKG-INFO` & `digquery-0.1.5/digquery.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digquery
-Version: 0.1.3
+Version: 0.1.5
 Summary: A Python package for querying DNS information using dig
 Author: Jay
 Author-email: techdjay@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -36,22 +36,23 @@
 
 .. code-block:: bash
 
     digquery example.com 
     pydig example.com 
     mydig example.com
 
-This will execute separate `dig` commands for each query type (`TXT` and `A`) and display the results.
+This will execute separate `dig` commands for each query type (`A` , `TXT` , `MX`, `NS`) and display the results in clear and crisp format.
 
 Contributing
 ------------
 
 Contributions are welcome! Here are some ways you can contribute:
 
 - Report bugs or suggest improvements by creating a new issue on the `digquery` GitHub repository.
+  https://github.com/techdjay/digquery
 - Fork the repository, make changes, and submit a pull request.
 
 License
 -------
 
 This project is licensed under the MIT License. See the `LICENSE` file for more information.
```

### Comparing `digquery-0.1.3/setup.py` & `digquery-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import setup
 
 with open(os.path.join(os.path.dirname(__file__), 'README.rst')) as readme:
     README = readme.read()
 setup(
     name='digquery',
-    version='0.1.3',
+    version='0.1.5',
     author='Jay',
     author_email='techdjay@gmail.com',
     description='A Python package for querying DNS information using dig',
     long_description=README,
     packages=['digquery'],
     	entry_points={
 		'console_scripts': [
```

