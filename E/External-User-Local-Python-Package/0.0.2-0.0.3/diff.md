# Comparing `tmp/External-User-Local-Python-Package-0.0.2.tar.gz` & `tmp/External-User-Local-Python-Package-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "External-User-Local-Python-Package-0.0.2.tar", last modified: Sun Jul  9 18:04:02 2023, max compression
+gzip compressed data, was "External-User-Local-Python-Package-0.0.3.tar", last modified: Sun Jul  9 18:39:45 2023, max compression
```

## Comparing `External-User-Local-Python-Package-0.0.2.tar` & `External-User-Local-Python-Package-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:04:02.141837 External-User-Local-Python-Package-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:04:02.141837 External-User-Local-Python-Package-0.0.2/External_User_Local_Python_Package.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-09 18:04:02.000000 External-User-Local-Python-Package-0.0.2/External_User_Local_Python_Package.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-09 18:04:02.000000 External-User-Local-Python-Package-0.0.2/External_User_Local_Python_Package.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 18:04:02.000000 External-User-Local-Python-Package-0.0.2/External_User_Local_Python_Package.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 18:04:02.000000 External-User-Local-Python-Package-0.0.2/External_User_Local_Python_Package.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-09 18:04:02.141837 External-User-Local-Python-Package-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-09 18:03:45.000000 External-User-Local-Python-Package-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 18:04:02.141837 External-User-Local-Python-Package-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-09 18:03:45.000000 External-User-Local-Python-Package-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:04:02.141837 External-User-Local-Python-Package-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-09 18:03:45.000000 External-User-Local-Python-Package-0.0.2/tests/test_insertExternal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:39:45.984478 External-User-Local-Python-Package-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:39:45.984478 External-User-Local-Python-Package-0.0.3/External_User_Local_Python_Package.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-09 18:39:45.000000 External-User-Local-Python-Package-0.0.3/External_User_Local_Python_Package.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-09 18:39:45.000000 External-User-Local-Python-Package-0.0.3/External_User_Local_Python_Package.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 18:39:45.000000 External-User-Local-Python-Package-0.0.3/External_User_Local_Python_Package.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 18:39:45.000000 External-User-Local-Python-Package-0.0.3/External_User_Local_Python_Package.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-09 18:39:45.984478 External-User-Local-Python-Package-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-09 18:39:28.000000 External-User-Local-Python-Package-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 18:39:45.984478 External-User-Local-Python-Package-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-09 18:39:28.000000 External-User-Local-Python-Package-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:39:45.984478 External-User-Local-Python-Package-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-09 18:39:28.000000 External-User-Local-Python-Package-0.0.3/tests/test_insertExternal.py
```

### Comparing `External-User-Local-Python-Package-0.0.2/setup.py` & `External-User-Local-Python-Package-0.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import setuptools
 # used by python -m build
 # python -m build needs pyproject.toml or setup.py
 setuptools.setup(
      # TODO: Please update the name and delete this line i.e. XXX-local or XXX-remote (without the -python-package suffix)
      name='External-User-Local-Python-Package',  
-     version='0.0.2',
+     version='0.0.3',
      author="Circles",
      author_email="info@circles.life",
      # TODO: Please update the description and delete this line
-     description="PyPI Package for Circles <project-name> Local/Remote Python",
+     description="PyPI Package for Circles access token library Local/Remote Python",
      # TODO: Please update the long description and delete this line    
-     long_description="This is a package for sharing common XXX function used in different repositories",
+     long_description="This is a package for sharing common access tokens function used in different repositories",
      long_description_content_type="text/markdown",
      url="https://github.com/circles",
      packages=setuptools.find_packages(),
      classifiers=[
          "Programming Language :: Python :: 3",
          "License :: Other/Proprietary License",
          "Operating System :: OS Independent",
```

### Comparing `External-User-Local-Python-Package-0.0.2/tests/test_insertExternal.py` & `External-User-Local-Python-Package-0.0.3/tests/test_insertExternal.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 import pytest
 import dotenv 
 
 
 
 sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '..', 'src')))
 sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '..', 'db')))
-from insert import insert
+from library import Accsess_Token_Library
 
 
 dotenv.load_dotenv()
 
 @pytest.mark.test
 def test_getProfiles_returns_name_and_email():
-    insert1 = insert()
+    insert1 = Accsess_Token_Library()
     insert1.insert_user_external("test",2,"test1")
 
     token=insert1.get_access_token_by_user_name("test")
     assert token[0]=="test1"
 
-test_getProfiles_returns_name_and_email() 
+
```

