# Comparing `tmp/anyconfig-json5-backend-0.2.0.tar.gz` & `tmp/anyconfig-json5-backend-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anyconfig-json5-backend-0.2.0.tar", last modified: Sun Feb 28 08:28:43 2021, max compression
+gzip compressed data, was "anyconfig-json5-backend-0.2.1.tar", last modified: Sun Jul  9 17:47:27 2023, max compression
```

## Comparing `anyconfig-json5-backend-0.2.0.tar` & `anyconfig-json5-backend-0.2.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2021-02-28 08:28:43.476314 anyconfig-json5-backend-0.2.0/
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2021-02-28 08:28:43.474314 anyconfig-json5-backend-0.2.0/.github/
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2021-02-28 08:28:43.475314 anyconfig-json5-backend-0.2.0/.github/workflows/
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      662 2021-02-28 06:00:53.000000 anyconfig-json5-backend-0.2.0/.github/workflows/tests.yml
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1069 2021-02-27 14:24:36.000000 anyconfig-json5-backend-0.2.0/LICENSE.MIT
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      219 2020-04-30 17:05:50.000000 anyconfig-json5-backend-0.2.0/MANIFEST.in
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       52 2021-02-28 05:54:47.000000 anyconfig-json5-backend-0.2.0/NEWS
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     3936 2021-02-28 08:28:43.477314 anyconfig-json5-backend-0.2.0/PKG-INFO
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     2071 2021-02-28 08:11:50.000000 anyconfig-json5-backend-0.2.0/README.rst
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1345 2021-02-28 08:11:50.000000 anyconfig-json5-backend-0.2.0/azure-pipelines.yml
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2021-02-28 08:28:43.475314 anyconfig-json5-backend-0.2.0/pkg/
--rwxrwxr-x   0 ssato     (1000) ssato     (1000)      494 2018-01-01 13:54:49.000000 anyconfig-json5-backend-0.2.0/pkg/copr-build.sh
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1214 2021-02-28 06:03:24.000000 anyconfig-json5-backend-0.2.0/pkg/package.spec.in
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       16 2021-02-28 05:34:27.000000 anyconfig-json5-backend-0.2.0/requirements.txt
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1700 2021-02-28 08:28:43.477314 anyconfig-json5-backend-0.2.0/setup.cfg
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1501 2020-04-30 17:05:50.000000 anyconfig-json5-backend-0.2.0/setup.py
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2021-02-28 08:28:43.474314 anyconfig-json5-backend-0.2.0/src/
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2021-02-28 08:28:43.475314 anyconfig-json5-backend-0.2.0/src/anyconfig_json5_backend/
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      125 2021-02-28 08:28:34.000000 anyconfig-json5-backend-0.2.0/src/anyconfig_json5_backend/__init__.py
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1232 2021-02-27 14:43:03.000000 anyconfig-json5-backend-0.2.0/src/anyconfig_json5_backend/json5_.py
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2021-02-28 08:28:43.476314 anyconfig-json5-backend-0.2.0/src/anyconfig_json5_backend.egg-info/
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     3936 2021-02-28 08:28:43.000000 anyconfig-json5-backend-0.2.0/src/anyconfig_json5_backend.egg-info/PKG-INFO
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      702 2021-02-28 08:28:43.000000 anyconfig-json5-backend-0.2.0/src/anyconfig_json5_backend.egg-info/SOURCES.txt
--rw-rw-r--   0 ssato     (1000) ssato     (1000)        1 2021-02-28 08:28:43.000000 anyconfig-json5-backend-0.2.0/src/anyconfig_json5_backend.egg-info/dependency_links.txt
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       61 2021-02-28 08:28:43.000000 anyconfig-json5-backend-0.2.0/src/anyconfig_json5_backend.egg-info/entry_points.txt
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       10 2021-02-28 08:28:43.000000 anyconfig-json5-backend-0.2.0/src/anyconfig_json5_backend.egg-info/requires.txt
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       24 2021-02-28 08:28:43.000000 anyconfig-json5-backend-0.2.0/src/anyconfig_json5_backend.egg-info/top_level.txt
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2021-02-28 08:28:43.476314 anyconfig-json5-backend-0.2.0/tests/
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      116 2021-02-28 05:27:09.000000 anyconfig-json5-backend-0.2.0/tests/__init__.py
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       43 2021-02-28 05:36:40.000000 anyconfig-json5-backend-0.2.0/tests/requirements.txt
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2021-02-28 08:28:43.476314 anyconfig-json5-backend-0.2.0/tests/res/
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      356 2021-02-28 05:46:16.000000 anyconfig-json5-backend-0.2.0/tests/res/10_short_example.json
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      341 2021-02-28 05:46:44.000000 anyconfig-json5-backend-0.2.0/tests/res/10_short_example.json5
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1601 2021-02-28 05:54:09.000000 anyconfig-json5-backend-0.2.0/tests/test_json5.py
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      898 2021-02-28 05:29:26.000000 anyconfig-json5-backend-0.2.0/tests/test_plugin.py
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      841 2021-02-28 08:11:50.000000 anyconfig-json5-backend-0.2.0/tox.ini
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 17:47:27.175977 anyconfig-json5-backend-0.2.1/
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 17:47:27.172977 anyconfig-json5-backend-0.2.1/.github/
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 17:47:27.173977 anyconfig-json5-backend-0.2.1/.github/workflows/
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      858 2023-07-09 17:46:52.000000 anyconfig-json5-backend-0.2.1/.github/workflows/tests.yml
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)     1069 2021-02-27 14:24:36.000000 anyconfig-json5-backend-0.2.1/LICENSE.MIT
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)      219 2020-04-30 17:05:50.000000 anyconfig-json5-backend-0.2.1/MANIFEST.in
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)       52 2021-02-28 05:54:47.000000 anyconfig-json5-backend-0.2.1/NEWS
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     3084 2023-07-09 17:47:27.175977 anyconfig-json5-backend-0.2.1/PKG-INFO
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     1644 2023-07-09 17:46:52.000000 anyconfig-json5-backend-0.2.1/README.rst
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)     1345 2021-02-28 08:11:50.000000 anyconfig-json5-backend-0.2.1/azure-pipelines.yml
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 17:47:27.174977 anyconfig-json5-backend-0.2.1/pkg/
+-rwxrwxr-x   0 ssato     (1000) ssato     (1000)      494 2018-01-01 13:54:49.000000 anyconfig-json5-backend-0.2.1/pkg/copr-build.sh
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)     1214 2021-02-28 06:03:24.000000 anyconfig-json5-backend-0.2.1/pkg/package.spec.in
+-rw-r--r--   0 ssato     (1000) ssato     (1000)       90 2023-07-09 17:46:52.000000 anyconfig-json5-backend-0.2.1/requirements.txt
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     1702 2023-07-09 17:47:27.176977 anyconfig-json5-backend-0.2.1/setup.cfg
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)     1501 2020-04-30 17:05:50.000000 anyconfig-json5-backend-0.2.1/setup.py
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 17:47:27.172977 anyconfig-json5-backend-0.2.1/src/
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 17:47:27.174977 anyconfig-json5-backend-0.2.1/src/anyconfig_json5_backend/
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      125 2023-07-09 17:46:52.000000 anyconfig-json5-backend-0.2.1/src/anyconfig_json5_backend/__init__.py
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     1302 2023-07-09 17:46:52.000000 anyconfig-json5-backend-0.2.1/src/anyconfig_json5_backend/json5_.py
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 17:47:27.175977 anyconfig-json5-backend-0.2.1/src/anyconfig_json5_backend.egg-info/
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)     3084 2023-07-09 17:47:27.000000 anyconfig-json5-backend-0.2.1/src/anyconfig_json5_backend.egg-info/PKG-INFO
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)      702 2023-07-09 17:47:27.000000 anyconfig-json5-backend-0.2.1/src/anyconfig_json5_backend.egg-info/SOURCES.txt
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)        1 2023-07-09 17:47:27.000000 anyconfig-json5-backend-0.2.1/src/anyconfig_json5_backend.egg-info/dependency_links.txt
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)       60 2023-07-09 17:47:27.000000 anyconfig-json5-backend-0.2.1/src/anyconfig_json5_backend.egg-info/entry_points.txt
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)       10 2023-07-09 17:47:27.000000 anyconfig-json5-backend-0.2.1/src/anyconfig_json5_backend.egg-info/requires.txt
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)       24 2023-07-09 17:47:27.000000 anyconfig-json5-backend-0.2.1/src/anyconfig_json5_backend.egg-info/top_level.txt
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 17:47:27.175977 anyconfig-json5-backend-0.2.1/tests/
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)      116 2021-02-28 05:27:09.000000 anyconfig-json5-backend-0.2.1/tests/__init__.py
+-rw-r--r--   0 ssato     (1000) ssato     (1000)       87 2023-07-09 17:46:52.000000 anyconfig-json5-backend-0.2.1/tests/requirements.txt
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 17:47:27.175977 anyconfig-json5-backend-0.2.1/tests/res/
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)      356 2021-02-28 05:46:16.000000 anyconfig-json5-backend-0.2.1/tests/res/10_short_example.json
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)      341 2021-02-28 05:46:44.000000 anyconfig-json5-backend-0.2.1/tests/res/10_short_example.json5
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     1476 2023-07-09 17:46:52.000000 anyconfig-json5-backend-0.2.1/tests/test_json5.py
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      643 2023-07-09 17:46:52.000000 anyconfig-json5-backend-0.2.1/tests/test_plugin.py
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      829 2023-07-09 17:46:52.000000 anyconfig-json5-backend-0.2.1/tox.ini
```

### Comparing `anyconfig-json5-backend-0.2.0/.github/workflows/tests.yml` & `anyconfig-json5-backend-0.2.1/.github/workflows/tests.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 ---
 # .. seealso:: https://github.com/ymyzk/tox-gh-actions
 #
 name: Tests
 # yamllint disable-line rule:truthy
 on:
   - push
+
 jobs:
   build:
-    runs-on: ubuntu-latest
+    runs-on: ${{ matrix.platform }}
     strategy:
       max-parallel: 5
       matrix:
-        python-version: [3.7, 3.8]
+        platform:
+          - ubuntu-latest
+          # - macos-latest
+        python-version:
+          - 3.8
+          - 3.9
+          - "3.10"
+          - "3.11"
 
     steps:
       - uses: actions/checkout@v1
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install tox tox-gh-actions
       - name: Test with tox
         run: tox
+        env:
+          PLATFORM: ${{ matrix.platform }}
 
 # vim:sw=2:ts=2:et:
```

### Comparing `anyconfig-json5-backend-0.2.0/LICENSE.MIT` & `anyconfig-json5-backend-0.2.1/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `anyconfig-json5-backend-0.2.0/PKG-INFO` & `anyconfig-json5-backend-0.2.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,85 +1,78 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: anyconfig-json5-backend
-Version: 0.2.0
+Version: 0.2.1
 Summary: Backend module for python-anyconfig to load and dump json5 files
 Home-page: https://github.com/ssato/python-anyconfig-json5-backend
 Author: Satoru SATOH
 Author-email: satoru.satoh@gmail.com
 Maintainer: Satoru SATOH
 Maintainer-email: satoru.satoh@gmail.com
 License: MIT
 Project-URL: CI: Github Actions, https://github.com/ssato/python-anyconfig-json5-backend/actions
 Project-URL: Download, https://pypi.org/project/anyconfig-json5-backend/
 Project-URL: Download RPMs, https://copr.fedoraproject.org/coprs/ssato/python-anyconfig/
 Project-URL: Bug Tracker, https://github.com/ssato/python-anyconfig-json5-backend/issues
 Project-URL: Source, https://github.com/ssato/python-anyconfig-json5-backend
-Description: ==================================
-        python-anyconfig-json5-backend
-        ==================================
-        
-        .. image:: https://img.shields.io/pypi/v/anyconfig-json5-backend.svg
-           :target: https://pypi.python.org/pypi/anyconfig-json5-backend/
-           :alt: [Latest Version]
-        
-        .. image:: https://img.shields.io/pypi/pyversions/anyconfig-json5-backend.svg
-           :target: https://pypi.python.org/pypi/anyconfig-json5-backend/
-           :alt: [Python versions]
-        
-        .. image:: https://img.shields.io/pypi/l/anyconfig-json5-backend.svg
-           :target: https://pypi.python.org/pypi/anyconfig-json5-backend/
-           :alt: MIT License
-        
-        .. image:: https://github.com/ssato/python-anyconfig-json5-backend/workflows/Tests/badge.svg
-           :target: https://github.com/ssato/python-anyconfig-json5-backend/actions?query=workflow%3ATests
-           :alt: GitHub Actions Test status
-        
-        .. image:: https://dev.azure.com/satorusatoh0471/python-anyconfig-json5-backend/_apis/build/status/ssato.python-anyconfig-json5-backend?branchName=master
-           :target: https://dev.azure.com/satorusatoh0471/python-anyconfig-json5-backend/_build/latest?definitionId=1
-           :alt: [Azure Pipelines Status]
-        
-        .. .. image:: https://img.shields.io/coveralls/ssato/python-anyconfig-json5-backend.svg
-           :target: https://coveralls.io/r/ssato/python-anyconfig-json5-backend
-           :alt: Coverage Status
-        
-        .. image:: https://img.shields.io/lgtm/alerts/g/ssato/python-anyconfig-json5-backend.svg
-           :target: https://lgtm.com/projects/g/ssato/python-anyconfig-json5-backend/alerts/
-           :alt: [Total Alerts by LGTM]
-        
-        .. image:: https://img.shields.io/lgtm/grade/python/g/ssato/python-anyconfig-json5-backend.svg
-           :target: https://lgtm.com/projects/g/ssato/python-anyconfig-json5-backend/context:python
-           :alt: [Code Quality by LGTM]
-        
-        This is a backend module for python-anyconfig to support to load and dump
-        json5' data files.
-        
-        - Author: Satoru SATOH <satoru.satoh@gmail.com>
-        - License: MIT
-        
-        SEE ALSO:
-        
-        - python-anyconfig: https://pypi.python.org/pypi/anyconfig
-        - JSON5: https://json5.org
-        
-        Build packages
-        ================
-        
-        Try::
-        
-          $ tox -e dists
-          
-        .. vim:sw=2:ts=2:et:
-        
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
+License-File: LICENSE.MIT
+
+==================================
+python-anyconfig-json5-backend
+==================================
+
+.. image:: https://img.shields.io/pypi/v/anyconfig-json5-backend.svg
+   :target: https://pypi.python.org/pypi/anyconfig-json5-backend/
+   :alt: [Latest Version]
+
+.. image:: https://img.shields.io/pypi/pyversions/anyconfig-json5-backend.svg
+   :target: https://pypi.python.org/pypi/anyconfig-json5-backend/
+   :alt: [Python versions]
+
+.. image:: https://img.shields.io/pypi/l/anyconfig-json5-backend.svg
+   :target: https://pypi.python.org/pypi/anyconfig-json5-backend/
+   :alt: MIT License
+
+.. image:: https://github.com/ssato/python-anyconfig-json5-backend/workflows/Tests/badge.svg
+   :target: https://github.com/ssato/python-anyconfig-json5-backend/actions?query=workflow%3ATests
+   :alt: GitHub Actions Test status
+
+.. image:: https://dev.azure.com/satorusatoh0471/python-anyconfig-json5-backend/_apis/build/status/ssato.python-anyconfig-json5-backend?branchName=master
+   :target: https://dev.azure.com/satorusatoh0471/python-anyconfig-json5-backend/_build/latest?definitionId=1
+   :alt: [Azure Pipelines Status]
+
+.. .. image:: https://img.shields.io/coveralls/ssato/python-anyconfig-json5-backend.svg
+   :target: https://coveralls.io/r/ssato/python-anyconfig-json5-backend
+   :alt: Coverage Status
+
+This is a backend module for python-anyconfig to support to load and dump
+json5' data files.
+
+- Author: Satoru SATOH <satoru.satoh@gmail.com>
+- License: MIT
+
+SEE ALSO:
+
+- python-anyconfig: https://pypi.python.org/pypi/anyconfig
+- JSON5: https://json5.org
+
+Build packages
+================
+
+Try::
+
+  $ tox -e dists
+  
+.. vim:sw=2:ts=2:et:
```

### Comparing `anyconfig-json5-backend-0.2.0/README.rst` & `anyconfig-json5-backend-0.2.1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -22,22 +22,14 @@
    :target: https://dev.azure.com/satorusatoh0471/python-anyconfig-json5-backend/_build/latest?definitionId=1
    :alt: [Azure Pipelines Status]
 
 .. .. image:: https://img.shields.io/coveralls/ssato/python-anyconfig-json5-backend.svg
    :target: https://coveralls.io/r/ssato/python-anyconfig-json5-backend
    :alt: Coverage Status
 
-.. image:: https://img.shields.io/lgtm/alerts/g/ssato/python-anyconfig-json5-backend.svg
-   :target: https://lgtm.com/projects/g/ssato/python-anyconfig-json5-backend/alerts/
-   :alt: [Total Alerts by LGTM]
-
-.. image:: https://img.shields.io/lgtm/grade/python/g/ssato/python-anyconfig-json5-backend.svg
-   :target: https://lgtm.com/projects/g/ssato/python-anyconfig-json5-backend/context:python
-   :alt: [Code Quality by LGTM]
-
 This is a backend module for python-anyconfig to support to load and dump
 json5' data files.
 
 - Author: Satoru SATOH <satoru.satoh@gmail.com>
 - License: MIT
 
 SEE ALSO:
```

### Comparing `anyconfig-json5-backend-0.2.0/azure-pipelines.yml` & `anyconfig-json5-backend-0.2.1/azure-pipelines.yml`

 * *Files identical despite different names*

### Comparing `anyconfig-json5-backend-0.2.0/pkg/package.spec.in` & `anyconfig-json5-backend-0.2.1/pkg/package.spec.in`

 * *Files identical despite different names*

### Comparing `anyconfig-json5-backend-0.2.0/setup.cfg` & `anyconfig-json5-backend-0.2.1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -23,18 +23,18 @@
 platforms = 
 	any
 classifiers = 
 	Development Status :: 4 - Beta
 	Intended Audience :: Developers
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Operating System :: OS Independent
 	Topic :: Software Development :: Libraries :: Python Modules
 	Topic :: Text Processing :: Markup
 	Topic :: Utilities
 	License :: OSI Approved :: MIT License
 
 [options]
```

### Comparing `anyconfig-json5-backend-0.2.0/setup.py` & `anyconfig-json5-backend-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `anyconfig-json5-backend-0.2.0/src/anyconfig_json5_backend/json5_.py` & `anyconfig-json5-backend-0.2.1/src/anyconfig_json5_backend/json5_.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2019 - 2020 Satoru SATOH <satoru.satoh@gmail.com>
+# Copyright (C) 2019 - 2023 Satoru SATOH <satoru.satoh@gmail.com>
 # SPDX-License-Identifier: MIT
 #
 # Ref. python -c "import json; help(json)"
 #
 """JSON5 Backend.
 
 - Format to support: JSON5, https://json5.org/
@@ -10,25 +10,28 @@
 - Development Status :: 3 - Alpha
 - Limitations: None obvious
 
 Changelog:
 
 .. versionadded:: 0.0.1
 """
+import typing
+
 import json5
+
 import anyconfig.backend.base
 
 
-_LOAD_OPTS = """object_hook parse_float parse_int
+_LOAD_OPTS: typing.List[str] = """object_hook parse_float parse_int
 parse_constant object_pairs_hook""".split()
 
-_DUMP_OPTS = """skipkeys ensure_ascii check_circular allow_nan
-indent separators default sort_keys""".split()
+_DUMP_OPTS: typing.List[str] = """skipkeys ensure_ascii check_circular
+allow_nan indent separators default sort_keys""".split()
 
-_DICT_OPTS = 'object_pairs_hook object_hook'.split()
+_DICT_OPTS: typing.List[str] = 'object_pairs_hook object_hook'.split()
 
 
 class Parser(anyconfig.backend.base.StringStreamFnParser):
     """
     Parser for JSON5 data files.
     """
     _cid = 'json5'
```

### Comparing `anyconfig-json5-backend-0.2.0/src/anyconfig_json5_backend.egg-info/PKG-INFO` & `anyconfig-json5-backend-0.2.1/src/anyconfig_json5_backend.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,85 +1,78 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: anyconfig-json5-backend
-Version: 0.2.0
+Version: 0.2.1
 Summary: Backend module for python-anyconfig to load and dump json5 files
 Home-page: https://github.com/ssato/python-anyconfig-json5-backend
 Author: Satoru SATOH
 Author-email: satoru.satoh@gmail.com
 Maintainer: Satoru SATOH
 Maintainer-email: satoru.satoh@gmail.com
 License: MIT
 Project-URL: CI: Github Actions, https://github.com/ssato/python-anyconfig-json5-backend/actions
 Project-URL: Download, https://pypi.org/project/anyconfig-json5-backend/
 Project-URL: Download RPMs, https://copr.fedoraproject.org/coprs/ssato/python-anyconfig/
 Project-URL: Bug Tracker, https://github.com/ssato/python-anyconfig-json5-backend/issues
 Project-URL: Source, https://github.com/ssato/python-anyconfig-json5-backend
-Description: ==================================
-        python-anyconfig-json5-backend
-        ==================================
-        
-        .. image:: https://img.shields.io/pypi/v/anyconfig-json5-backend.svg
-           :target: https://pypi.python.org/pypi/anyconfig-json5-backend/
-           :alt: [Latest Version]
-        
-        .. image:: https://img.shields.io/pypi/pyversions/anyconfig-json5-backend.svg
-           :target: https://pypi.python.org/pypi/anyconfig-json5-backend/
-           :alt: [Python versions]
-        
-        .. image:: https://img.shields.io/pypi/l/anyconfig-json5-backend.svg
-           :target: https://pypi.python.org/pypi/anyconfig-json5-backend/
-           :alt: MIT License
-        
-        .. image:: https://github.com/ssato/python-anyconfig-json5-backend/workflows/Tests/badge.svg
-           :target: https://github.com/ssato/python-anyconfig-json5-backend/actions?query=workflow%3ATests
-           :alt: GitHub Actions Test status
-        
-        .. image:: https://dev.azure.com/satorusatoh0471/python-anyconfig-json5-backend/_apis/build/status/ssato.python-anyconfig-json5-backend?branchName=master
-           :target: https://dev.azure.com/satorusatoh0471/python-anyconfig-json5-backend/_build/latest?definitionId=1
-           :alt: [Azure Pipelines Status]
-        
-        .. .. image:: https://img.shields.io/coveralls/ssato/python-anyconfig-json5-backend.svg
-           :target: https://coveralls.io/r/ssato/python-anyconfig-json5-backend
-           :alt: Coverage Status
-        
-        .. image:: https://img.shields.io/lgtm/alerts/g/ssato/python-anyconfig-json5-backend.svg
-           :target: https://lgtm.com/projects/g/ssato/python-anyconfig-json5-backend/alerts/
-           :alt: [Total Alerts by LGTM]
-        
-        .. image:: https://img.shields.io/lgtm/grade/python/g/ssato/python-anyconfig-json5-backend.svg
-           :target: https://lgtm.com/projects/g/ssato/python-anyconfig-json5-backend/context:python
-           :alt: [Code Quality by LGTM]
-        
-        This is a backend module for python-anyconfig to support to load and dump
-        json5' data files.
-        
-        - Author: Satoru SATOH <satoru.satoh@gmail.com>
-        - License: MIT
-        
-        SEE ALSO:
-        
-        - python-anyconfig: https://pypi.python.org/pypi/anyconfig
-        - JSON5: https://json5.org
-        
-        Build packages
-        ================
-        
-        Try::
-        
-          $ tox -e dists
-          
-        .. vim:sw=2:ts=2:et:
-        
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
+License-File: LICENSE.MIT
+
+==================================
+python-anyconfig-json5-backend
+==================================
+
+.. image:: https://img.shields.io/pypi/v/anyconfig-json5-backend.svg
+   :target: https://pypi.python.org/pypi/anyconfig-json5-backend/
+   :alt: [Latest Version]
+
+.. image:: https://img.shields.io/pypi/pyversions/anyconfig-json5-backend.svg
+   :target: https://pypi.python.org/pypi/anyconfig-json5-backend/
+   :alt: [Python versions]
+
+.. image:: https://img.shields.io/pypi/l/anyconfig-json5-backend.svg
+   :target: https://pypi.python.org/pypi/anyconfig-json5-backend/
+   :alt: MIT License
+
+.. image:: https://github.com/ssato/python-anyconfig-json5-backend/workflows/Tests/badge.svg
+   :target: https://github.com/ssato/python-anyconfig-json5-backend/actions?query=workflow%3ATests
+   :alt: GitHub Actions Test status
+
+.. image:: https://dev.azure.com/satorusatoh0471/python-anyconfig-json5-backend/_apis/build/status/ssato.python-anyconfig-json5-backend?branchName=master
+   :target: https://dev.azure.com/satorusatoh0471/python-anyconfig-json5-backend/_build/latest?definitionId=1
+   :alt: [Azure Pipelines Status]
+
+.. .. image:: https://img.shields.io/coveralls/ssato/python-anyconfig-json5-backend.svg
+   :target: https://coveralls.io/r/ssato/python-anyconfig-json5-backend
+   :alt: Coverage Status
+
+This is a backend module for python-anyconfig to support to load and dump
+json5' data files.
+
+- Author: Satoru SATOH <satoru.satoh@gmail.com>
+- License: MIT
+
+SEE ALSO:
+
+- python-anyconfig: https://pypi.python.org/pypi/anyconfig
+- JSON5: https://json5.org
+
+Build packages
+================
+
+Try::
+
+  $ tox -e dists
+  
+.. vim:sw=2:ts=2:et:
```

### Comparing `anyconfig-json5-backend-0.2.0/src/anyconfig_json5_backend.egg-info/SOURCES.txt` & `anyconfig-json5-backend-0.2.1/src/anyconfig_json5_backend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anyconfig-json5-backend-0.2.0/tests/test_json5.py` & `anyconfig-json5-backend-0.2.1/tests/test_json5.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,16 +34,15 @@
                 try:
                     cnf = TT.Parser().load(anyconfig.ioinfo.make(in_path),
                                            ac_ordered=True)
                     self.assertTrue(cnf)
                     self.assertTrue(isinstance(cnf, collections.OrderedDict))
 
                     anyconfig.dump(cnf, out_path)
-                    self.assertEqual(anyconfig.load(out_path,
-                                                    ac_ordered=False),
-                                     anyconfig.load(exp_path,
-                                                    ac_ordered=False))
+                    self.assertEqual(
+                        anyconfig.load(out_path, ac_ordered=False),
+                        anyconfig.load(exp_path, ac_ordered=False)
+                    )
                 except AssertionError as exc:
-                    raise AssertionError("file: {}, "
-                                         "exc={!s}".format(in_path, exc))
+                    raise AssertionError(f'file: {in_path}, exc={exc!s}')
 
 # vim:sw=4:ts=4:et:
```

### Comparing `anyconfig-json5-backend-0.2.0/tests/test_plugin.py` & `anyconfig-json5-backend-0.2.1/tests/test_plugin.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 #
 # Copyright (C) 2021 Satoru SATOH <satoru.satoh@gmail.com>
 # SPDX-License-Identifier: MIT
 #
-# pylint: disable=missing-docstring,invalid-name
+# pylint: disable=missing-docstring
 import unittest
+
 import anyconfig
+
 from . import CNF_FILES
 
 
-class Test_90(unittest.TestCase):
+class TestCase(unittest.TestCase):
 
     def _try_loads(self, files):
-        for filepath in files:
-            try:
-                cnf = anyconfig.load(filepath, ac_parser='json5')
-                self.assertTrue(cnf)
-
-                exp_path = filepath.parent / filepath.name.replace('.json5',
-                                                                   '.json')
-                ref = anyconfig.load(exp_path, ordered=True)
-
-            except anyconfig.UnknownFileTypeError:
-                print('all types=%r' % anyconfig.list_types())
-                raise
+        for path in files:
+            cnf = anyconfig.load(path, ac_parser='json5')
+            self.assertTrue(cnf)
 
+            exp_path = path.parent / path.name.replace('.json5', '.json')
+            ref = anyconfig.load(exp_path, ordered=True)
             self.assertEqual(cnf, ref)
 
-    def test_10_load(self):
+    def test_load_with_plugin(self):
         self._try_loads(CNF_FILES)
 
 # vim:sw=4:ts=4:et:
```

