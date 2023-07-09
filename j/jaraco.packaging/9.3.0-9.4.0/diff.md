# Comparing `tmp/jaraco.packaging-9.3.0.tar.gz` & `tmp/jaraco.packaging-9.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.packaging-9.3.0.tar", last modified: Thu Jul  6 02:21:55 2023, max compression
+gzip compressed data, was "jaraco.packaging-9.4.0.tar", last modified: Sun Jul  9 01:09:23 2023, max compression
```

## Comparing `jaraco.packaging-9.3.0.tar` & `jaraco.packaging-9.4.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:21:55.443220 jaraco.packaging-9.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:21:55.439220 jaraco.packaging-9.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:21:55.439220 jaraco.packaging-9.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-07-06 02:21:55.443220 jaraco.packaging-9.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:21:55.439220 jaraco.packaging-9.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:21:55.439220 jaraco.packaging-9.3.0/jaraco/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:21:55.439220 jaraco.packaging-9.3.0/jaraco/packaging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/jaraco/packaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/jaraco/packaging/make-tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/jaraco/packaging/sphinx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:21:55.439220 jaraco.packaging-9.3.0/jaraco.packaging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-07-06 02:21:55.000000 jaraco.packaging-9.3.0/jaraco.packaging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-06 02:21:55.000000 jaraco.packaging-9.3.0/jaraco.packaging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 02:21:55.000000 jaraco.packaging-9.3.0/jaraco.packaging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-06 02:21:55.000000 jaraco.packaging-9.3.0/jaraco.packaging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-06 02:21:55.000000 jaraco.packaging-9.3.0/jaraco.packaging.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-06 02:21:55.443220 jaraco.packaging-9.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-06 02:21:32.000000 jaraco.packaging-9.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:09:23.081488 jaraco.packaging-9.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-09 01:08:59.000000 jaraco.packaging-9.4.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-09 01:08:59.000000 jaraco.packaging-9.4.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:09:23.081488 jaraco.packaging-9.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-09 01:08:59.000000 jaraco.packaging-9.4.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:09:23.081488 jaraco.packaging-9.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-09 01:08:59.000000 jaraco.packaging-9.4.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-09 01:08:59.000000 jaraco.packaging-9.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-09 01:08:59.000000 jaraco.packaging-9.4.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-09 01:08:59.000000 jaraco.packaging-9.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-07-09 01:08:59.000000 jaraco.packaging-9.4.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-07-09 01:09:23.081488 jaraco.packaging-9.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-09 01:08:59.000000 jaraco.packaging-9.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-09 01:08:59.000000 jaraco.packaging-9.4.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:09:23.081488 jaraco.packaging-9.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-09 01:08:59.000000 jaraco.packaging-9.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-09 01:08:59.000000 jaraco.packaging-9.4.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-09 01:08:59.000000 jaraco.packaging-9.4.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:09:23.081488 jaraco.packaging-9.4.0/jaraco/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:09:23.081488 jaraco.packaging-9.4.0/jaraco/packaging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 01:08:59.000000 jaraco.packaging-9.4.0/jaraco/packaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-09 01:08:59.000000 jaraco.packaging-9.4.0/jaraco/packaging/make-tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-07-09 01:08:59.000000 jaraco.packaging-9.4.0/jaraco/packaging/sphinx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:09:23.081488 jaraco.packaging-9.4.0/jaraco.packaging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-07-09 01:09:23.000000 jaraco.packaging-9.4.0/jaraco.packaging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-09 01:09:23.000000 jaraco.packaging-9.4.0/jaraco.packaging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 01:09:23.000000 jaraco.packaging-9.4.0/jaraco.packaging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-09 01:09:23.000000 jaraco.packaging-9.4.0/jaraco.packaging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-09 01:09:23.000000 jaraco.packaging-9.4.0/jaraco.packaging.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-09 01:08:59.000000 jaraco.packaging-9.4.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-09 01:08:59.000000 jaraco.packaging-9.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-09 01:08:59.000000 jaraco.packaging-9.4.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-09 01:09:23.081488 jaraco.packaging-9.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-09 01:08:59.000000 jaraco.packaging-9.4.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-09 01:08:59.000000 jaraco.packaging-9.4.0/tox.ini
```

### Comparing `jaraco.packaging-9.3.0/.github/workflows/main.yml` & `jaraco.packaging-9.4.0/.github/workflows/main.yml`

 * *Files 1% similar despite different names*

```diff
@@ -64,29 +64,29 @@
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
           allow-prereleases: true
       - name: Install tox
         run: |
           python -m pip install tox
-      - name: Run tests
+      - name: Run
         run: tox
 
   docs:
     runs-on: ubuntu-latest
     env:
       TOXENV: docs
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
       - name: Install tox
         run: |
           python -m pip install tox
-      - name: Run tests
+      - name: Run
         run: tox
 
   check:  # This job does nothing and is only used for the branch protection
     if: always()
 
     needs:
     - test
@@ -113,12 +113,12 @@
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: 3.x
       - name: Install tox
         run: |
           python -m pip install tox
-      - name: Release
+      - name: Run
         run: tox -e release
         env:
           TWINE_PASSWORD: ${{ secrets.PYPI_TOKEN }}
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `jaraco.packaging-9.3.0/LICENSE` & `jaraco.packaging-9.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jaraco.packaging-9.3.0/NEWS.rst` & `jaraco.packaging-9.4.0/NEWS.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v9.4.0
+======
+
+Features
+--------
+
+- Deprecated use of environment variable for isolated builds. The workaround is in the wrong place and should be dealt with upstream. (#11)
+
+
 v9.3.0
 ======
 
 Features
 --------
 
 - Add sidebar-links directive.
```

### Comparing `jaraco.packaging-9.3.0/PKG-INFO` & `jaraco.packaging-9.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.packaging
-Version: 9.3.0
+Version: 9.4.0
 Summary: tools to supplement packaging Python releases
 Home-page: https://github.com/jaraco/jaraco.packaging
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jaraco.packaging-9.3.0/README.rst` & `jaraco.packaging-9.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `jaraco.packaging-9.3.0/docs/conf.py` & `jaraco.packaging-9.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaraco.packaging-9.3.0/jaraco/packaging/make-tree.py` & `jaraco.packaging-9.4.0/jaraco/packaging/make-tree.py`

 * *Files identical despite different names*

### Comparing `jaraco.packaging-9.3.0/jaraco/packaging/sphinx.py` & `jaraco.packaging-9.4.0/jaraco/packaging/sphinx.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 to conf.py, and the setup hook does the rest.
 
 >>> 'setup' in globals()
 True
 """
 
 import os
+import warnings
 from importlib import metadata
 
 from build.util import project_wheel_metadata as load_metadata
 from jaraco.context import suppress
 import sphinx.util.docutils
 from docutils.parsers.rst import directives
 import docutils.statemachine
@@ -91,14 +92,18 @@
     >>> _load_metadata_from_wheel()
     >>> getfixture('static_wheel')
     >>> meta = _load_metadata_from_wheel()
     >>> meta['Name']
     'sampleproject'
     """
     wheel = os.environ['JARACO_PACKAGING_SPHINX_WHEEL']
+    warnings.warn(
+        "JARACO_PACKAGING_SPHINX_WHEEL is deprecated; fix pypa/build#556 instead",
+        DeprecationWarning,
+    )
     (dist,) = metadata.distributions(path=[wheel])
     return dist.metadata
 
 
 def load_config_from_setup(app):
     """
     Replace values in app.config from package metadata
```

### Comparing `jaraco.packaging-9.3.0/jaraco.packaging.egg-info/PKG-INFO` & `jaraco.packaging-9.4.0/jaraco.packaging.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.packaging
-Version: 9.3.0
+Version: 9.4.0
 Summary: tools to supplement packaging Python releases
 Home-page: https://github.com/jaraco/jaraco.packaging
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jaraco.packaging-9.3.0/jaraco.packaging.egg-info/SOURCES.txt` & `jaraco.packaging-9.4.0/jaraco.packaging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaraco.packaging-9.3.0/pytest.ini` & `jaraco.packaging-9.4.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `jaraco.packaging-9.3.0/setup.cfg` & `jaraco.packaging-9.4.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 	python_implementation != "PyPy"
 	pytest-enabler >= 2.2
 	pytest-ruff
 	
 	types-docutils
 docs = 
 	sphinx >= 3.5
-	jaraco.packaging >= 9
+	jaraco.packaging >= 9.3
 	rst.linker >= 1.9
 	furo
 	sphinx-lint
 
 [options.entry_points]
 
 [egg_info]
```

### Comparing `jaraco.packaging-9.3.0/tox.ini` & `jaraco.packaging-9.4.0/tox.ini`

 * *Files identical despite different names*

