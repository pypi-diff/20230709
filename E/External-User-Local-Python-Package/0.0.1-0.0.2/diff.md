# Comparing `tmp/External-User-Local-Python-Package-0.0.1.tar.gz` & `tmp/External-User-Local-Python-Package-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "External-User-Local-Python-Package-0.0.1.tar", last modified: Sun Jul  9 17:44:53 2023, max compression
+gzip compressed data, was "External-User-Local-Python-Package-0.0.2.tar", last modified: Sun Jul  9 18:04:02 2023, max compression
```

## Comparing `External-User-Local-Python-Package-0.0.1.tar` & `External-User-Local-Python-Package-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:44:53.688438 External-User-Local-Python-Package-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:44:53.688438 External-User-Local-Python-Package-0.0.1/External_User_Local_Python_Package.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-09 17:44:53.000000 External-User-Local-Python-Package-0.0.1/External_User_Local_Python_Package.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-09 17:44:53.000000 External-User-Local-Python-Package-0.0.1/External_User_Local_Python_Package.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 17:44:53.000000 External-User-Local-Python-Package-0.0.1/External_User_Local_Python_Package.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 17:44:53.000000 External-User-Local-Python-Package-0.0.1/External_User_Local_Python_Package.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-09 17:44:53.688438 External-User-Local-Python-Package-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-09 17:44:32.000000 External-User-Local-Python-Package-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 17:44:53.688438 External-User-Local-Python-Package-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-09 17:44:32.000000 External-User-Local-Python-Package-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:44:53.688438 External-User-Local-Python-Package-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-09 17:44:32.000000 External-User-Local-Python-Package-0.0.1/tests/test_insertExternal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:04:02.141837 External-User-Local-Python-Package-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:04:02.141837 External-User-Local-Python-Package-0.0.2/External_User_Local_Python_Package.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-09 18:04:02.000000 External-User-Local-Python-Package-0.0.2/External_User_Local_Python_Package.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-09 18:04:02.000000 External-User-Local-Python-Package-0.0.2/External_User_Local_Python_Package.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 18:04:02.000000 External-User-Local-Python-Package-0.0.2/External_User_Local_Python_Package.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 18:04:02.000000 External-User-Local-Python-Package-0.0.2/External_User_Local_Python_Package.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-09 18:04:02.141837 External-User-Local-Python-Package-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-09 18:03:45.000000 External-User-Local-Python-Package-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 18:04:02.141837 External-User-Local-Python-Package-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-09 18:03:45.000000 External-User-Local-Python-Package-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:04:02.141837 External-User-Local-Python-Package-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-09 18:03:45.000000 External-User-Local-Python-Package-0.0.2/tests/test_insertExternal.py
```

### Comparing `External-User-Local-Python-Package-0.0.1/README.md` & `External-User-Local-Python-Package-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `External-User-Local-Python-Package-0.0.1/setup.py` & `External-User-Local-Python-Package-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 # used by python -m build
 # python -m build needs pyproject.toml or setup.py
 setuptools.setup(
      # TODO: Please update the name and delete this line i.e. XXX-local or XXX-remote (without the -python-package suffix)
      name='External-User-Local-Python-Package',  
-     version='0.0.1',
+     version='0.0.2',
      author="Circles",
      author_email="info@circles.life",
      # TODO: Please update the description and delete this line
      description="PyPI Package for Circles <project-name> Local/Remote Python",
      # TODO: Please update the long description and delete this line    
      long_description="This is a package for sharing common XXX function used in different repositories",
      long_description_content_type="text/markdown",
```

### Comparing `External-User-Local-Python-Package-0.0.1/tests/test_insertExternal.py` & `External-User-Local-Python-Package-0.0.2/tests/test_insertExternal.py`

 * *Files identical despite different names*

