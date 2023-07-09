# Comparing `tmp/wajig-4.1.0.tar.gz` & `tmp/wajig-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wajig-4.1.0.tar", last modified: Sun Jul  9 05:59:13 2023, max compression
+gzip compressed data, was "wajig-4.1.1.tar", last modified: Sun Jul  9 06:02:46 2023, max compression
```

## Comparing `wajig-4.1.0.tar` & `wajig-4.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-x---   0 gjw       (1000) gjw       (1000)        0 2023-07-09 05:59:13.019310 wajig-4.1.0/
--rw-r-----   0 gjw       (1000) gjw       (1000)    35149 2020-07-07 02:15:20.000000 wajig-4.1.0/LICENSE
--rw-r-----   0 gjw       (1000) gjw       (1000)       82 2020-07-25 22:22:49.000000 wajig-4.1.0/MANIFEST.in
--rw-r-----   0 gjw       (1000) gjw       (1000)    32921 2023-07-09 05:59:13.019310 wajig-4.1.0/PKG-INFO
--rw-r-----   0 gjw       (1000) gjw       (1000)    32815 2023-07-09 03:06:21.000000 wajig-4.1.0/README.rst
-drwxr-x---   0 gjw       (1000) gjw       (1000)        0 2023-07-09 05:59:13.015310 wajig-4.1.0/docs/
--rw-r-----   0 gjw       (1000) gjw       (1000)    32372 2020-08-02 08:52:34.000000 wajig-4.1.0/docs/README.md
--rw-r-----   0 gjw       (1000) gjw       (1000)       50 2023-07-09 05:59:13.019310 wajig-4.1.0/setup.cfg
--rw-r-----   0 gjw       (1000) gjw       (1000)     2498 2023-07-09 05:59:12.000000 wajig-4.1.0/setup.py
-drwxr-x---   0 gjw       (1000) gjw       (1000)        0 2023-07-09 05:59:13.015310 wajig-4.1.0/wajig/
--rwxr-x---   0 gjw       (1000) gjw       (1000)    40230 2023-07-09 02:54:05.000000 wajig-4.1.0/wajig/__init__.py
-drwxr-x---   0 gjw       (1000) gjw       (1000)        0 2023-07-09 05:59:13.015310 wajig-4.1.0/wajig/bash_completion.d/
--rw-r-----   0 gjw       (1000) gjw       (1000)     4972 2022-09-09 01:07:27.000000 wajig-4.1.0/wajig/bash_completion.d/wajig.bash
--rw-r-----   0 gjw       (1000) gjw       (1000)    53078 2023-07-09 02:55:03.000000 wajig-4.1.0/wajig/commands.py
--rw-r-----   0 gjw       (1000) gjw       (1000)      289 2023-07-09 05:59:12.000000 wajig-4.1.0/wajig/constants.py
--rw-r-----   0 gjw       (1000) gjw       (1000)     1586 2020-06-11 00:25:18.000000 wajig-4.1.0/wajig/debfile-deps.py
--rw-r-----   0 gjw       (1000) gjw       (1000)     1224 2020-07-26 06:53:41.000000 wajig-4.1.0/wajig/debfile.py
--rw-r-----   0 gjw       (1000) gjw       (1000)     4429 2021-10-24 21:34:57.000000 wajig-4.1.0/wajig/perform.py
--rwxr-x---   0 gjw       (1000) gjw       (1000)     2990 2022-11-06 19:20:40.000000 wajig-4.1.0/wajig/shell.py
--rw-r-----   0 gjw       (1000) gjw       (1000)    22441 2022-11-06 19:20:40.000000 wajig-4.1.0/wajig/util.py
-drwxr-x---   0 gjw       (1000) gjw       (1000)        0 2023-07-09 05:59:13.015310 wajig-4.1.0/wajig.egg-info/
--rw-r-----   0 gjw       (1000) gjw       (1000)    32921 2023-07-09 05:59:12.000000 wajig-4.1.0/wajig.egg-info/PKG-INFO
--rw-r-----   0 gjw       (1000) gjw       (1000)      415 2023-07-09 05:59:12.000000 wajig-4.1.0/wajig.egg-info/SOURCES.txt
--rw-r-----   0 gjw       (1000) gjw       (1000)        1 2023-07-09 05:59:12.000000 wajig-4.1.0/wajig.egg-info/dependency_links.txt
--rw-r-----   0 gjw       (1000) gjw       (1000)       37 2023-07-09 05:59:12.000000 wajig-4.1.0/wajig.egg-info/entry_points.txt
--rw-r-----   0 gjw       (1000) gjw       (1000)       36 2023-07-09 05:59:12.000000 wajig-4.1.0/wajig.egg-info/requires.txt
--rw-r-----   0 gjw       (1000) gjw       (1000)        6 2023-07-09 05:59:12.000000 wajig-4.1.0/wajig.egg-info/top_level.txt
+drwxr-x---   0 gjw       (1000) gjw       (1000)        0 2023-07-09 06:02:46.071511 wajig-4.1.1/
+-rw-r-----   0 gjw       (1000) gjw       (1000)    35149 2020-07-07 02:15:20.000000 wajig-4.1.1/LICENSE
+-rw-r-----   0 gjw       (1000) gjw       (1000)       82 2020-07-25 22:22:49.000000 wajig-4.1.1/MANIFEST.in
+-rw-r-----   0 gjw       (1000) gjw       (1000)    32921 2023-07-09 06:02:46.071511 wajig-4.1.1/PKG-INFO
+-rw-r-----   0 gjw       (1000) gjw       (1000)    32815 2023-07-09 03:06:21.000000 wajig-4.1.1/README.rst
+drwxr-x---   0 gjw       (1000) gjw       (1000)        0 2023-07-09 06:02:46.067511 wajig-4.1.1/docs/
+-rw-r-----   0 gjw       (1000) gjw       (1000)    32372 2020-08-02 08:52:34.000000 wajig-4.1.1/docs/README.md
+-rw-r-----   0 gjw       (1000) gjw       (1000)       50 2023-07-09 06:02:46.071511 wajig-4.1.1/setup.cfg
+-rw-r-----   0 gjw       (1000) gjw       (1000)     2498 2023-07-09 06:02:45.000000 wajig-4.1.1/setup.py
+drwxr-x---   0 gjw       (1000) gjw       (1000)        0 2023-07-09 06:02:46.071511 wajig-4.1.1/wajig/
+-rwxr-x---   0 gjw       (1000) gjw       (1000)    40230 2023-07-09 02:54:05.000000 wajig-4.1.1/wajig/__init__.py
+drwxr-x---   0 gjw       (1000) gjw       (1000)        0 2023-07-09 06:02:46.071511 wajig-4.1.1/wajig/bash_completion.d/
+-rw-r-----   0 gjw       (1000) gjw       (1000)     4972 2022-09-09 01:07:27.000000 wajig-4.1.1/wajig/bash_completion.d/wajig.bash
+-rw-r-----   0 gjw       (1000) gjw       (1000)    53078 2023-07-09 02:55:03.000000 wajig-4.1.1/wajig/commands.py
+-rw-r-----   0 gjw       (1000) gjw       (1000)      289 2023-07-09 06:02:45.000000 wajig-4.1.1/wajig/constants.py
+-rw-r-----   0 gjw       (1000) gjw       (1000)     1586 2020-06-11 00:25:18.000000 wajig-4.1.1/wajig/debfile-deps.py
+-rw-r-----   0 gjw       (1000) gjw       (1000)     1224 2020-07-26 06:53:41.000000 wajig-4.1.1/wajig/debfile.py
+-rw-r-----   0 gjw       (1000) gjw       (1000)     4429 2021-10-24 21:34:57.000000 wajig-4.1.1/wajig/perform.py
+-rwxr-x---   0 gjw       (1000) gjw       (1000)     2990 2022-11-06 19:20:40.000000 wajig-4.1.1/wajig/shell.py
+-rw-r-----   0 gjw       (1000) gjw       (1000)    22441 2022-11-06 19:20:40.000000 wajig-4.1.1/wajig/util.py
+drwxr-x---   0 gjw       (1000) gjw       (1000)        0 2023-07-09 06:02:46.071511 wajig-4.1.1/wajig.egg-info/
+-rw-r-----   0 gjw       (1000) gjw       (1000)    32921 2023-07-09 06:02:45.000000 wajig-4.1.1/wajig.egg-info/PKG-INFO
+-rw-r-----   0 gjw       (1000) gjw       (1000)      415 2023-07-09 06:02:46.000000 wajig-4.1.1/wajig.egg-info/SOURCES.txt
+-rw-r-----   0 gjw       (1000) gjw       (1000)        1 2023-07-09 06:02:45.000000 wajig-4.1.1/wajig.egg-info/dependency_links.txt
+-rw-r-----   0 gjw       (1000) gjw       (1000)       37 2023-07-09 06:02:45.000000 wajig-4.1.1/wajig.egg-info/entry_points.txt
+-rw-r-----   0 gjw       (1000) gjw       (1000)       36 2023-07-09 06:02:45.000000 wajig-4.1.1/wajig.egg-info/requires.txt
+-rw-r-----   0 gjw       (1000) gjw       (1000)        6 2023-07-09 06:02:45.000000 wajig-4.1.1/wajig.egg-info/top_level.txt
```

### Comparing `wajig-4.1.0/LICENSE` & `wajig-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wajig-4.1.0/PKG-INFO` & `wajig-4.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wajig
-Version: 4.1.0
+Version: 4.1.1
 Summary: Debian/Ubuntu admin management tool
 Home-page: https://wajig.togaware.com
 Author: Graham Williams
 Author-email: wajig@togaware.com
 Keywords: debian ubuntu admin
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `wajig-4.1.0/README.rst` & `wajig-4.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `wajig-4.1.0/docs/README.md` & `wajig-4.1.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `wajig-4.1.0/setup.py` & `wajig-4.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # Get the long description from the README file.
 
 with open(path.join(here, 'docs/README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='wajig',
-    version='4.1.0',  # DO NOT MODIFY. Managed from Makefile.
+    version='4.1.1',  # DO NOT MODIFY. Managed from Makefile.
     description='Debian/Ubuntu admin management tool',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Graham Williams',
     author_email='wajig@togaware.com',
     url='https://wajig.togaware.com',
     classifiers=[
```

### Comparing `wajig-4.1.0/wajig/__init__.py` & `wajig-4.1.1/wajig/__init__.py`

 * *Files identical despite different names*

### Comparing `wajig-4.1.0/wajig/bash_completion.d/wajig.bash` & `wajig-4.1.1/wajig/bash_completion.d/wajig.bash`

 * *Files identical despite different names*

### Comparing `wajig-4.1.0/wajig/commands.py` & `wajig-4.1.1/wajig/commands.py`

 * *Files identical despite different names*

### Comparing `wajig-4.1.0/wajig/debfile-deps.py` & `wajig-4.1.1/wajig/debfile-deps.py`

 * *Files identical despite different names*

### Comparing `wajig-4.1.0/wajig/debfile.py` & `wajig-4.1.1/wajig/debfile.py`

 * *Files identical despite different names*

### Comparing `wajig-4.1.0/wajig/perform.py` & `wajig-4.1.1/wajig/perform.py`

 * *Files identical despite different names*

### Comparing `wajig-4.1.0/wajig/shell.py` & `wajig-4.1.1/wajig/shell.py`

 * *Files identical despite different names*

### Comparing `wajig-4.1.0/wajig/util.py` & `wajig-4.1.1/wajig/util.py`

 * *Files identical despite different names*

### Comparing `wajig-4.1.0/wajig.egg-info/PKG-INFO` & `wajig-4.1.1/wajig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wajig
-Version: 4.1.0
+Version: 4.1.1
 Summary: Debian/Ubuntu admin management tool
 Home-page: https://wajig.togaware.com
 Author: Graham Williams
 Author-email: wajig@togaware.com
 Keywords: debian ubuntu admin
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

