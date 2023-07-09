# Comparing `tmp/wizlib-0.2.7.tar.gz` & `tmp/wizlib-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizlib-0.2.7.tar", last modified: Sun Jul  9 03:40:44 2023, max compression
+gzip compressed data, was "wizlib-0.3.0.tar", last modified: Sat Jul  8 17:25:39 2023, max compression
```

## Comparing `wizlib-0.2.7.tar` & `wizlib-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 03:40:44.627268 wizlib-0.2.7/
--rw-rw-rw-   0 root         (0) root         (0)        5 2023-07-09 03:39:54.000000 wizlib-0.2.7/.version
--rw-r--r--   0 root         (0) root         (0)     1771 2023-07-09 03:40:44.627268 wizlib-0.2.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1506 2023-07-09 03:40:36.000000 wizlib-0.2.7/README.md
--rw-rw-rw-   0 root         (0) root         (0)      541 2023-07-09 03:40:36.000000 wizlib-0.2.7/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-09 03:40:44.627268 wizlib-0.2.7/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 03:40:44.625268 wizlib-0.2.7/test/
--rw-rw-rw-   0 root         (0) root         (0)     1099 2023-07-09 03:40:36.000000 wizlib-0.2.7/test/test_super_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 03:40:44.626268 wizlib-0.2.7/wizlib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-09 03:40:36.000000 wizlib-0.2.7/wizlib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1626 2023-07-09 03:40:36.000000 wizlib-0.2.7/wizlib/rlinput.py
--rw-rw-rw-   0 root         (0) root         (0)      973 2023-07-09 03:40:36.000000 wizlib-0.2.7/wizlib/super_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 03:40:44.627268 wizlib-0.2.7/wizlib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1771 2023-07-09 03:40:44.000000 wizlib-0.2.7/wizlib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      270 2023-07-09 03:40:44.000000 wizlib-0.2.7/wizlib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 03:40:44.000000 wizlib-0.2.7/wizlib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       89 2023-07-09 03:40:44.000000 wizlib-0.2.7/wizlib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-09 03:40:44.000000 wizlib-0.2.7/wizlib.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:25:39.706326 wizlib-0.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)        5 2023-07-08 17:24:50.000000 wizlib-0.3.0/.version
+-rw-r--r--   0 root         (0) root         (0)     1771 2023-07-08 17:25:39.706326 wizlib-0.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1506 2023-07-08 17:25:31.000000 wizlib-0.3.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      541 2023-07-08 17:25:31.000000 wizlib-0.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-08 17:25:39.706326 wizlib-0.3.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:25:39.704326 wizlib-0.3.0/test/
+-rw-rw-rw-   0 root         (0) root         (0)     1099 2023-07-08 17:25:31.000000 wizlib-0.3.0/test/test_super_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:25:39.704326 wizlib-0.3.0/wizlib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-08 17:25:31.000000 wizlib-0.3.0/wizlib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1626 2023-07-08 17:25:31.000000 wizlib-0.3.0/wizlib/rlinput.py
+-rw-rw-rw-   0 root         (0) root         (0)      973 2023-07-08 17:25:31.000000 wizlib-0.3.0/wizlib/super_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 17:25:39.705326 wizlib-0.3.0/wizlib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1771 2023-07-08 17:25:39.000000 wizlib-0.3.0/wizlib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      270 2023-07-08 17:25:39.000000 wizlib-0.3.0/wizlib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-08 17:25:39.000000 wizlib-0.3.0/wizlib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       89 2023-07-08 17:25:39.000000 wizlib-0.3.0/wizlib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-08 17:25:39.000000 wizlib-0.3.0/wizlib.egg-info/top_level.txt
```

### Comparing `wizlib-0.2.7/PKG-INFO` & `wizlib-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wizlib
-Version: 0.2.7
+Version: 0.3.0
 Summary: A collection of Python modules that are useful across multiple projects
 Author-email: Francis Potter <wizlib@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # WizLib
```

### Comparing `wizlib-0.2.7/README.md` & `wizlib-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `wizlib-0.2.7/pyproject.toml` & `wizlib-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wizlib-0.2.7/test/test_super_wrapper.py` & `wizlib-0.3.0/test/test_super_wrapper.py`

 * *Files identical despite different names*

### Comparing `wizlib-0.2.7/wizlib/rlinput.py` & `wizlib-0.3.0/wizlib/rlinput.py`

 * *Files identical despite different names*

### Comparing `wizlib-0.2.7/wizlib/super_wrapper.py` & `wizlib-0.3.0/wizlib/super_wrapper.py`

 * *Files identical despite different names*

### Comparing `wizlib-0.2.7/wizlib.egg-info/PKG-INFO` & `wizlib-0.3.0/wizlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wizlib
-Version: 0.2.7
+Version: 0.3.0
 Summary: A collection of Python modules that are useful across multiple projects
 Author-email: Francis Potter <wizlib@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # WizLib
```

