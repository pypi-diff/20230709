# Comparing `tmp/pytest-checkdocs-2.8.1.tar.gz` & `tmp/pytest-checkdocs-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-checkdocs-2.8.1.tar", last modified: Tue Sep 27 01:46:30 2022, max compression
+gzip compressed data, was "pytest-checkdocs-2.9.0.tar", last modified: Sun Oct  9 02:00:08 2022, max compression
```

## Comparing `pytest-checkdocs-2.8.1.tar` & `pytest-checkdocs-2.9.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2022-09-27 01:46:30.850658 pytest-checkdocs-2.8.1/
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)      121 2022-09-11 16:31:31.000000 pytest-checkdocs-2.8.1/.coveragerc
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)      246 2022-09-11 16:31:31.000000 pytest-checkdocs-2.8.1/.editorconfig
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)      136 2022-09-11 16:31:31.000000 pytest-checkdocs-2.8.1/.flake8
-drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2022-09-27 01:46:30.848241 pytest-checkdocs-2.8.1/.github/
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)      148 2022-09-11 16:31:31.000000 pytest-checkdocs-2.8.1/.github/dependabot.yml
-drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2022-09-27 01:46:30.848442 pytest-checkdocs-2.8.1/.github/workflows/
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1732 2022-09-27 01:34:25.000000 pytest-checkdocs-2.8.1/.github/workflows/main.yml
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)       81 2022-09-11 16:31:31.000000 pytest-checkdocs-2.8.1/.pre-commit-config.yaml
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)       79 2022-09-11 16:31:31.000000 pytest-checkdocs-2.8.1/.readthedocs.yml
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)     2142 2022-09-27 01:46:13.000000 pytest-checkdocs-2.8.1/CHANGES.rst
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1050 2022-09-11 16:31:31.000000 pytest-checkdocs-2.8.1/LICENSE
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1532 2022-09-27 01:46:30.850768 pytest-checkdocs-2.8.1/PKG-INFO
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)      939 2022-09-27 01:45:18.000000 pytest-checkdocs-2.8.1/README.rst
-drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2022-09-27 01:46:30.849142 pytest-checkdocs-2.8.1/docs/
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1215 2022-09-27 01:34:25.000000 pytest-checkdocs-2.8.1/docs/conf.py
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)       81 2022-09-11 16:31:31.000000 pytest-checkdocs-2.8.1/docs/history.rst
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)      300 2022-09-11 16:31:31.000000 pytest-checkdocs-2.8.1/docs/index.rst
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)       37 2022-09-11 16:31:31.000000 pytest-checkdocs-2.8.1/mypy.ini
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)      378 2022-09-11 16:31:31.000000 pytest-checkdocs-2.8.1/pyproject.toml
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)      910 2022-09-11 16:31:31.000000 pytest-checkdocs-2.8.1/pytest.ini
-drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2022-09-27 01:46:30.849334 pytest-checkdocs-2.8.1/pytest_checkdocs/
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)     2735 2022-09-27 01:35:55.000000 pytest-checkdocs-2.8.1/pytest_checkdocs/__init__.py
-drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2022-09-27 01:46:30.850531 pytest-checkdocs-2.8.1/pytest_checkdocs.egg-info/
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1532 2022-09-27 01:46:30.000000 pytest-checkdocs-2.8.1/pytest_checkdocs.egg-info/PKG-INFO
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)      524 2022-09-27 01:46:30.000000 pytest-checkdocs-2.8.1/pytest_checkdocs.egg-info/SOURCES.txt
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)        1 2022-09-27 01:46:30.000000 pytest-checkdocs-2.8.1/pytest_checkdocs.egg-info/dependency_links.txt
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)       40 2022-09-27 01:46:30.000000 pytest-checkdocs-2.8.1/pytest_checkdocs.egg-info/entry_points.txt
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)      302 2022-09-27 01:46:30.000000 pytest-checkdocs-2.8.1/pytest_checkdocs.egg-info/requires.txt
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)       17 2022-09-27 01:46:30.000000 pytest-checkdocs-2.8.1/pytest_checkdocs.egg-info/top_level.txt
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1154 2022-09-27 01:46:30.851143 pytest-checkdocs-2.8.1/setup.cfg
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)      732 2022-09-11 16:31:31.000000 pytest-checkdocs-2.8.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-09 02:00:08.194766 pytest-checkdocs-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)      121 2022-10-09 01:59:35.000000 pytest-checkdocs-2.9.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (121)      246 2022-10-09 01:59:35.000000 pytest-checkdocs-2.9.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (121)      136 2022-10-09 01:59:35.000000 pytest-checkdocs-2.9.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-09 02:00:08.194766 pytest-checkdocs-2.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-09 01:59:35.000000 pytest-checkdocs-2.9.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-09 02:00:08.194766 pytest-checkdocs-2.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1732 2022-10-09 01:59:35.000000 pytest-checkdocs-2.9.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-10-09 01:59:35.000000 pytest-checkdocs-2.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      233 2022-10-09 01:59:35.000000 pytest-checkdocs-2.9.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2214 2022-10-09 01:59:35.000000 pytest-checkdocs-2.9.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-10-09 01:59:35.000000 pytest-checkdocs-2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1532 2022-10-09 02:00:08.194766 pytest-checkdocs-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      939 2022-10-09 01:59:35.000000 pytest-checkdocs-2.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-09 02:00:08.194766 pytest-checkdocs-2.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)     1235 2022-10-09 01:59:35.000000 pytest-checkdocs-2.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-10-09 01:59:35.000000 pytest-checkdocs-2.9.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      300 2022-10-09 01:59:35.000000 pytest-checkdocs-2.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-10-09 01:59:35.000000 pytest-checkdocs-2.9.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (121)      378 2022-10-09 01:59:35.000000 pytest-checkdocs-2.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      910 2022-10-09 01:59:35.000000 pytest-checkdocs-2.9.0/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-09 02:00:08.194766 pytest-checkdocs-2.9.0/pytest_checkdocs/
+-rw-r--r--   0 runner    (1001) docker     (121)     2734 2022-10-09 01:59:35.000000 pytest-checkdocs-2.9.0/pytest_checkdocs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      141 2022-10-09 01:59:35.000000 pytest-checkdocs-2.9.0/pytest_checkdocs/py310compat.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-09 02:00:08.194766 pytest-checkdocs-2.9.0/pytest_checkdocs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1532 2022-10-09 02:00:08.000000 pytest-checkdocs-2.9.0/pytest_checkdocs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      556 2022-10-09 02:00:08.000000 pytest-checkdocs-2.9.0/pytest_checkdocs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-09 02:00:08.000000 pytest-checkdocs-2.9.0/pytest_checkdocs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       40 2022-10-09 02:00:08.000000 pytest-checkdocs-2.9.0/pytest_checkdocs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      335 2022-10-09 02:00:08.000000 pytest-checkdocs-2.9.0/pytest_checkdocs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-09 02:00:08.000000 pytest-checkdocs-2.9.0/pytest_checkdocs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1185 2022-10-09 02:00:08.194766 pytest-checkdocs-2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      732 2022-10-09 01:59:35.000000 pytest-checkdocs-2.9.0/tox.ini
```

### Comparing `pytest-checkdocs-2.8.1/.github/workflows/main.yml` & `pytest-checkdocs-2.9.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pytest-checkdocs-2.8.1/CHANGES.rst` & `pytest-checkdocs-2.9.0/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+v2.9.0
+======
+
+Prefer ``importlib.metadata`` on Python 3.10 and later.
+
 v2.8.1
 ======
 
 In README, present badge/link to the docs.
 
 v2.8.0
 ======
```

### Comparing `pytest-checkdocs-2.8.1/LICENSE` & `pytest-checkdocs-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-checkdocs-2.8.1/PKG-INFO` & `pytest-checkdocs-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-checkdocs
-Version: 2.8.1
+Version: 2.9.0
 Summary: check the README when running tests
 Home-page: https://github.com/jaraco/pytest-checkdocs
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pytest-checkdocs-2.8.1/README.rst` & `pytest-checkdocs-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-checkdocs-2.8.1/docs/conf.py` & `pytest-checkdocs-2.9.0/docs/conf.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 extensions = [
     'sphinx.ext.autodoc',
     'jaraco.packaging.sphinx',
 ]
 
 master_doc = "index"
+html_theme = "furo"
 
 # Link dates and other references in the changelog
 extensions += ['rst.linker']
 link_files = {
     '../CHANGES.rst': dict(
         using=dict(GH='https://github.com'),
         replace=[
```

### Comparing `pytest-checkdocs-2.8.1/pytest.ini` & `pytest-checkdocs-2.9.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `pytest-checkdocs-2.8.1/pytest_checkdocs/__init__.py` & `pytest-checkdocs-2.9.0/pytest_checkdocs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import contextlib
 import re
 import warnings
 
 import pytest
 import docutils.core
-import importlib_metadata
 from build.util import project_wheel_metadata as load_metadata
 
+from .py310compat import metadata as md
+
 
 project_files = 'setup.py', 'setup.cfg', 'pyproject.toml'
 
 
 @contextlib.contextmanager
 def _suppress_deprecation():
     # pypa/pep517#122
@@ -85,9 +86,9 @@
     On Python 3.8 and later, pep517.meta returns a PathDistribution
     without clean metadata. Employ the adapter that comes with
     importlib_metadata 4 to get clean metadata.
     """
     try:
         metadata.json
     except AttributeError:
-        metadata = importlib_metadata._adapters.Message(metadata)
+        metadata = md._adapters.Message(metadata)
     return metadata
```

### Comparing `pytest-checkdocs-2.8.1/pytest_checkdocs.egg-info/PKG-INFO` & `pytest-checkdocs-2.9.0/pytest_checkdocs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-checkdocs
-Version: 2.8.1
+Version: 2.9.0
 Summary: check the README when running tests
 Home-page: https://github.com/jaraco/pytest-checkdocs
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pytest-checkdocs-2.8.1/setup.cfg` & `pytest-checkdocs-2.9.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 [options]
 packages = find_namespace:
 include_package_data = true
 python_requires = >=3.7
 install_requires = 
 	docutils >= 0.15
 	build
-	importlib_metadata >= 4
+	importlib_metadata >= 4; python_version < "3.10"
 
 [options.packages.find]
 exclude = 
 	build*
 	dist*
 	docs*
 	tests*
@@ -43,14 +43,15 @@
 	pytest-enabler >= 1.3
 	
 	types-docutils  # pytest-checkdocs#13
 docs = 
 	sphinx >= 3.5
 	jaraco.packaging >= 9
 	rst.linker >= 1.9
+	furo
 
 [options.entry_points]
 pytest11 = 
 	checkdocs = pytest_checkdocs
 
 [egg_info]
 tag_build =
```

### Comparing `pytest-checkdocs-2.8.1/tox.ini` & `pytest-checkdocs-2.9.0/tox.ini`

 * *Files identical despite different names*

