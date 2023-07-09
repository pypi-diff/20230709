# Comparing `tmp/process-twarc-0.12.1.tar.gz` & `tmp/process-twarc-0.12.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "process-twarc-0.12.1.tar", last modified: Sun Jul  9 11:45:18 2023, max compression
+gzip compressed data, was "process-twarc-0.12.2.tar", last modified: Sun Jul  9 11:52:30 2023, max compression
```

## Comparing `process-twarc-0.12.1.tar` & `process-twarc-0.12.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 11:45:18.491737 process-twarc-0.12.1/
--rw-rw-rw-   0        0        0     1077 2023-07-07 10:42:07.000000 process-twarc-0.12.1/LICENSE.txt
--rw-rw-rw-   0        0        0      693 2023-07-09 11:45:18.491737 process-twarc-0.12.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-07 10:42:22.000000 process-twarc-0.12.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-09 11:45:18.459708 process-twarc-0.12.1/process_twarc/
--rw-rw-rw-   0        0        0        0 2023-07-07 10:27:29.000000 process-twarc-0.12.1/process_twarc/__init__.py
--rw-rw-rw-   0        0        0     8471 2023-07-09 11:42:16.000000 process-twarc-0.12.1/process_twarc/util.py
-drwxrwxrwx   0        0        0        0 2023-07-09 11:45:18.490739 process-twarc-0.12.1/process_twarc.egg-info/
--rw-rw-rw-   0        0        0      693 2023-07-09 11:45:18.000000 process-twarc-0.12.1/process_twarc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-07-09 11:45:18.000000 process-twarc-0.12.1/process_twarc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 11:45:18.000000 process-twarc-0.12.1/process_twarc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-07-09 11:45:18.000000 process-twarc-0.12.1/process_twarc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-09 11:45:18.000000 process-twarc-0.12.1/process_twarc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       56 2023-07-09 11:45:18.492745 process-twarc-0.12.1/setup.cfg
--rw-rw-rw-   0        0        0      976 2023-07-09 11:44:56.000000 process-twarc-0.12.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 11:52:30.488215 process-twarc-0.12.2/
+-rw-rw-rw-   0        0        0     1077 2023-07-07 10:42:07.000000 process-twarc-0.12.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      693 2023-07-09 11:52:30.488215 process-twarc-0.12.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-07 10:42:22.000000 process-twarc-0.12.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 11:52:30.481276 process-twarc-0.12.2/process_twarc/
+-rw-rw-rw-   0        0        0        0 2023-07-07 10:27:29.000000 process-twarc-0.12.2/process_twarc/__init__.py
+-rw-rw-rw-   0        0        0     8471 2023-07-09 11:42:16.000000 process-twarc-0.12.2/process_twarc/util.py
+drwxrwxrwx   0        0        0        0 2023-07-09 11:52:30.487211 process-twarc-0.12.2/process_twarc.egg-info/
+-rw-rw-rw-   0        0        0      693 2023-07-09 11:52:30.000000 process-twarc-0.12.2/process_twarc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-07-09 11:52:30.000000 process-twarc-0.12.2/process_twarc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 11:52:30.000000 process-twarc-0.12.2/process_twarc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-07-09 11:52:30.000000 process-twarc-0.12.2/process_twarc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-09 11:52:30.000000 process-twarc-0.12.2/process_twarc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       56 2023-07-09 11:52:30.489720 process-twarc-0.12.2/setup.cfg
+-rw-rw-rw-   0        0        0      976 2023-07-09 11:51:47.000000 process-twarc-0.12.2/setup.py
```

### Comparing `process-twarc-0.12.1/LICENSE.txt` & `process-twarc-0.12.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `process-twarc-0.12.1/PKG-INFO` & `process-twarc-0.12.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: process-twarc
-Version: 0.12.1
+Version: 0.12.2
 Summary: Tools for tranforming raw data from Twarc2 to structured data for Masked Language Modeling.
 Home-page: https://github.com/user/Lone-Wolfgang
 Author: Jordan Wolfgang Klein
 Author-email: jordan.klein.21@um.edu.mt
 License: MIT
 Keywords: Twitter,Deduplication,Tokenization,Language Modeling
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `process-twarc-0.12.1/process_twarc/util.py` & `process-twarc-0.12.2/process_twarc/util.py`

 * *Files identical despite different names*

### Comparing `process-twarc-0.12.1/process_twarc.egg-info/PKG-INFO` & `process-twarc-0.12.2/process_twarc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: process-twarc
-Version: 0.12.1
+Version: 0.12.2
 Summary: Tools for tranforming raw data from Twarc2 to structured data for Masked Language Modeling.
 Home-page: https://github.com/user/Lone-Wolfgang
 Author: Jordan Wolfgang Klein
 Author-email: jordan.klein.21@um.edu.mt
 License: MIT
 Keywords: Twitter,Deduplication,Tokenization,Language Modeling
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `process-twarc-0.12.1/setup.py` & `process-twarc-0.12.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'process-twarc',         
   packages = ['process_twarc'],   
-  version = '0.12.1',
+  version = '0.12.2',
   license='MIT',
   description = 'Tools for tranforming raw data from Twarc2 to structured data for Masked Language Modeling.',   # Give a short description about your library
   author = 'Jordan Wolfgang Klein',
   author_email = 'jordan.klein.21@um.edu.mt',
   url = 'https://github.com/user/Lone-Wolfgang',
   keywords = ['Twitter', 'Deduplication', "Tokenization", "Language Modeling"],
   install_requires=[
```

