# Comparing `tmp/jaraco.classes-3.2.3.tar.gz` & `tmp/jaraco.classes-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.classes-3.2.3.tar", last modified: Tue Sep 27 00:10:06 2022, max compression
+gzip compressed data, was "jaraco.classes-3.3.0.tar", last modified: Sun Jul  9 01:41:25 2023, max compression
```

## Comparing `jaraco.classes-3.2.3.tar` & `jaraco.classes-3.3.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 00:10:06.337881 jaraco.classes-3.2.3/
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-09-27 00:09:22.000000 jaraco.classes-3.2.3/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-09-27 00:09:22.000000 jaraco.classes-3.2.3/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-09-27 00:09:22.000000 jaraco.classes-3.2.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 00:10:06.333881 jaraco.classes-3.2.3/.github/
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-09-27 00:09:22.000000 jaraco.classes-3.2.3/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-09-27 00:09:22.000000 jaraco.classes-3.2.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 00:10:06.333881 jaraco.classes-3.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1586 2022-09-27 00:09:22.000000 jaraco.classes-3.2.3/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-09-27 00:09:22.000000 jaraco.classes-3.2.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-09-27 00:09:22.000000 jaraco.classes-3.2.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1500 2022-09-27 00:09:22.000000 jaraco.classes-3.2.3/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-09-27 00:09:22.000000 jaraco.classes-3.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2175 2022-09-27 00:10:06.337881 jaraco.classes-3.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1608 2022-09-27 00:09:22.000000 jaraco.classes-3.2.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 00:10:06.333881 jaraco.classes-3.2.3/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     1188 2022-09-27 00:09:22.000000 jaraco.classes-3.2.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-09-27 00:09:22.000000 jaraco.classes-3.2.3/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      531 2022-09-27 00:09:22.000000 jaraco.classes-3.2.3/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 00:10:06.333881 jaraco.classes-3.2.3/jaraco/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 00:10:06.337881 jaraco.classes-3.2.3/jaraco/classes/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-27 00:09:22.000000 jaraco.classes-3.2.3/jaraco/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1464 2022-09-27 00:09:22.000000 jaraco.classes-3.2.3/jaraco/classes/ancestry.py
--rw-r--r--   0 runner    (1001) docker     (121)     1853 2022-09-27 00:09:22.000000 jaraco.classes-3.2.3/jaraco/classes/meta.py
--rw-r--r--   0 runner    (1001) docker     (121)     3996 2022-09-27 00:09:22.000000 jaraco.classes-3.2.3/jaraco/classes/properties.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 00:10:06.333881 jaraco.classes-3.2.3/jaraco.classes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2175 2022-09-27 00:10:06.000000 jaraco.classes-3.2.3/jaraco.classes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      568 2022-09-27 00:10:06.000000 jaraco.classes-3.2.3/jaraco.classes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-27 00:10:06.000000 jaraco.classes-3.2.3/jaraco.classes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-09-27 00:10:06.000000 jaraco.classes-3.2.3/jaraco.classes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-09-27 00:10:06.000000 jaraco.classes-3.2.3/jaraco.classes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-09-27 00:09:22.000000 jaraco.classes-3.2.3/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-09-27 00:09:22.000000 jaraco.classes-3.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      910 2022-09-27 00:09:22.000000 jaraco.classes-3.2.3/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)     1046 2022-09-27 00:10:06.337881 jaraco.classes-3.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      732 2022-09-27 00:09:22.000000 jaraco.classes-3.2.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:41:25.651173 jaraco.classes-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-09 01:41:05.000000 jaraco.classes-3.3.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-09 01:41:05.000000 jaraco.classes-3.3.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:41:25.647173 jaraco.classes-3.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-09 01:41:05.000000 jaraco.classes-3.3.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-09 01:41:05.000000 jaraco.classes-3.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:41:25.647173 jaraco.classes-3.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-09 01:41:05.000000 jaraco.classes-3.3.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-09 01:41:05.000000 jaraco.classes-3.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-09 01:41:05.000000 jaraco.classes-3.3.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-09 01:41:05.000000 jaraco.classes-3.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-09 01:41:05.000000 jaraco.classes-3.3.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-09 01:41:25.651173 jaraco.classes-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-09 01:41:05.000000 jaraco.classes-3.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-09 01:41:05.000000 jaraco.classes-3.3.0/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:41:25.647173 jaraco.classes-3.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-09 01:41:05.000000 jaraco.classes-3.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-09 01:41:05.000000 jaraco.classes-3.3.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-09 01:41:05.000000 jaraco.classes-3.3.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:41:25.647173 jaraco.classes-3.3.0/jaraco/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:41:25.651173 jaraco.classes-3.3.0/jaraco/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 01:41:05.000000 jaraco.classes-3.3.0/jaraco/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-09 01:41:05.000000 jaraco.classes-3.3.0/jaraco/classes/ancestry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-09 01:41:05.000000 jaraco.classes-3.3.0/jaraco/classes/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-07-09 01:41:05.000000 jaraco.classes-3.3.0/jaraco/classes/properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:41:25.647173 jaraco.classes-3.3.0/jaraco.classes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-09 01:41:25.000000 jaraco.classes-3.3.0/jaraco.classes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-09 01:41:25.000000 jaraco.classes-3.3.0/jaraco.classes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 01:41:25.000000 jaraco.classes-3.3.0/jaraco.classes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-09 01:41:25.000000 jaraco.classes-3.3.0/jaraco.classes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-09 01:41:25.000000 jaraco.classes-3.3.0/jaraco.classes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-09 01:41:05.000000 jaraco.classes-3.3.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-09 01:41:05.000000 jaraco.classes-3.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-09 01:41:05.000000 jaraco.classes-3.3.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-09 01:41:25.651173 jaraco.classes-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-09 01:41:05.000000 jaraco.classes-3.3.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-09 01:41:05.000000 jaraco.classes-3.3.0/tox.ini
```

### Comparing `jaraco.classes-3.2.3/CHANGES.rst` & `jaraco.classes-3.3.0/NEWS.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v3.3.0
+======
+
+Features
+--------
+
+- Require Python 3.8 or later.
+
+
 v3.2.3
 ======
 
 #7: Enabled badge with link to docs in the readme.
 
 v3.2.2
 ======
```

### Comparing `jaraco.classes-3.2.3/LICENSE` & `jaraco.classes-3.3.0/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-Copyright Jason R. Coombs
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `jaraco.classes-3.2.3/PKG-INFO` & `jaraco.classes-3.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,51 @@
 Metadata-Version: 2.1
 Name: jaraco.classes
-Version: 3.2.3
+Version: 3.3.0
 Summary: Utility functions for Python class constructs
 Home-page: https://github.com/jaraco/jaraco.classes
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/jaraco.classes.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/jaraco.classes
 
 .. image:: https://img.shields.io/pypi/pyversions/jaraco.classes.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/jaraco.ui
 
 .. image:: https://github.com/jaraco/jaraco.classes/workflows/tests/badge.svg
    :target: https://github.com/jaraco/jaraco.classes/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/jaracoclasses/badge/?version=latest
    :target: https://jaracoclasses.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2022-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 .. image:: https://tidelift.com/badges/package/pypi/jaraco.classes
    :target: https://tidelift.com/subscription/pkg/pypi-jaraco.classes?utm_source=pypi-jaraco.classes&utm_medium=readme
 
 For Enterprise
 ==============
 
 Available as part of the Tidelift Subscription.
 
 This project and the maintainers of thousands of other packages are working with Tidelift to deliver one enterprise subscription that covers all of the open source you use.
 
 `Learn more <https://tidelift.com/subscription/pkg/pypi-jaraco.classes?utm_source=pypi-jaraco.classes&utm_medium=referral&utm_campaign=github>`_.
-
-Security Contact
-================
-
-To report a security vulnerability, please use the
-`Tidelift security contact <https://tidelift.com/security>`_.
-Tidelift will coordinate the fix and disclosure.
```

### Comparing `jaraco.classes-3.2.3/README.rst` & `jaraco.classes-3.3.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,34 @@
 .. image:: https://img.shields.io/pypi/v/jaraco.classes.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/jaraco.classes
 
 .. image:: https://img.shields.io/pypi/pyversions/jaraco.classes.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/jaraco.ui
 
 .. image:: https://github.com/jaraco/jaraco.classes/workflows/tests/badge.svg
    :target: https://github.com/jaraco/jaraco.classes/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/jaracoclasses/badge/?version=latest
    :target: https://jaracoclasses.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2022-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 .. image:: https://tidelift.com/badges/package/pypi/jaraco.classes
    :target: https://tidelift.com/subscription/pkg/pypi-jaraco.classes?utm_source=pypi-jaraco.classes&utm_medium=readme
 
 For Enterprise
 ==============
 
 Available as part of the Tidelift Subscription.
 
 This project and the maintainers of thousands of other packages are working with Tidelift to deliver one enterprise subscription that covers all of the open source you use.
 
 `Learn more <https://tidelift.com/subscription/pkg/pypi-jaraco.classes?utm_source=pypi-jaraco.classes&utm_medium=referral&utm_campaign=github>`_.
-
-Security Contact
-================
-
-To report a security vulnerability, please use the
-`Tidelift security contact <https://tidelift.com/security>`_.
-Tidelift will coordinate the fix and disclosure.
```

### Comparing `jaraco.classes-3.2.3/docs/conf.py` & `jaraco.classes-3.3.0/docs/conf.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
 extensions = [
     'sphinx.ext.autodoc',
     'jaraco.packaging.sphinx',
 ]
 
 master_doc = "index"
+html_theme = "furo"
 
 # Link dates and other references in the changelog
 extensions += ['rst.linker']
 link_files = {
-    '../CHANGES.rst': dict(
+    '../NEWS.rst': dict(
         using=dict(GH='https://github.com'),
         replace=[
             dict(
                 pattern=r'(Issue #|\B#)(?P<issue>\d+)',
                 url='{package_url}/issues/{issue}',
             ),
             dict(
```

### Comparing `jaraco.classes-3.2.3/docs/index.rst` & `jaraco.classes-3.3.0/docs/index.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Welcome to |project| documentation!
 ===================================
 
+.. sidebar-links::
+   :home:
+   :pypi:
+
 .. toctree::
    :maxdepth: 1
 
    history
 
 
 .. tidelift-referral-banner::
```

### Comparing `jaraco.classes-3.2.3/jaraco/classes/ancestry.py` & `jaraco.classes-3.3.0/jaraco/classes/ancestry.py`

 * *Files identical despite different names*

### Comparing `jaraco.classes-3.2.3/jaraco/classes/meta.py` & `jaraco.classes-3.3.0/jaraco/classes/meta.py`

 * *Files identical despite different names*

### Comparing `jaraco.classes-3.2.3/jaraco/classes/properties.py` & `jaraco.classes-3.3.0/jaraco/classes/properties.py`

 * *Files identical despite different names*

### Comparing `jaraco.classes-3.2.3/jaraco.classes.egg-info/PKG-INFO` & `jaraco.classes-3.3.0/jaraco.classes.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,51 @@
 Metadata-Version: 2.1
 Name: jaraco.classes
-Version: 3.2.3
+Version: 3.3.0
 Summary: Utility functions for Python class constructs
 Home-page: https://github.com/jaraco/jaraco.classes
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/jaraco.classes.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/jaraco.classes
 
 .. image:: https://img.shields.io/pypi/pyversions/jaraco.classes.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/jaraco.ui
 
 .. image:: https://github.com/jaraco/jaraco.classes/workflows/tests/badge.svg
    :target: https://github.com/jaraco/jaraco.classes/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/jaracoclasses/badge/?version=latest
    :target: https://jaracoclasses.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2022-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 .. image:: https://tidelift.com/badges/package/pypi/jaraco.classes
    :target: https://tidelift.com/subscription/pkg/pypi-jaraco.classes?utm_source=pypi-jaraco.classes&utm_medium=readme
 
 For Enterprise
 ==============
 
 Available as part of the Tidelift Subscription.
 
 This project and the maintainers of thousands of other packages are working with Tidelift to deliver one enterprise subscription that covers all of the open source you use.
 
 `Learn more <https://tidelift.com/subscription/pkg/pypi-jaraco.classes?utm_source=pypi-jaraco.classes&utm_medium=referral&utm_campaign=github>`_.
-
-Security Contact
-================
-
-To report a security vulnerability, please use the
-`Tidelift security contact <https://tidelift.com/security>`_.
-Tidelift will coordinate the fix and disclosure.
```

### Comparing `jaraco.classes-3.2.3/jaraco.classes.egg-info/SOURCES.txt` & `jaraco.classes-3.3.0/jaraco.classes.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 .coveragerc
 .editorconfig
-.flake8
 .pre-commit-config.yaml
-.readthedocs.yml
-CHANGES.rst
+.readthedocs.yaml
 LICENSE
+NEWS.rst
 README.rst
+SECURITY.md
 mypy.ini
 pyproject.toml
 pytest.ini
 setup.cfg
+towncrier.toml
 tox.ini
 .github/FUNDING.yml
 .github/dependabot.yml
 .github/workflows/main.yml
 docs/conf.py
 docs/history.rst
 docs/index.rst
```

### Comparing `jaraco.classes-3.2.3/setup.cfg` & `jaraco.classes-3.3.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -11,41 +11,43 @@
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 
 [options]
 packages = find_namespace:
 include_package_data = true
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
 	more_itertools
 
 [options.packages.find]
 exclude = 
 	build*
 	dist*
 	docs*
 	tests*
 
 [options.extras_require]
 testing = 
 	pytest >= 6
 	pytest-checkdocs >= 2.4
-	pytest-flake8
-	flake8 < 5
 	pytest-black >= 0.3.7; \
 	python_implementation != "PyPy"
 	pytest-cov
 	pytest-mypy >= 0.9.1; \
 	python_implementation != "PyPy"
-	pytest-enabler >= 1.3
+	pytest-enabler >= 2.2
+	pytest-ruff
 docs = 
 	sphinx >= 3.5
-	jaraco.packaging >= 9
+	jaraco.packaging >= 9.3
 	rst.linker >= 1.9
+	furo
+	sphinx-lint
+	
 	jaraco.tidelift >= 1.4
 
 [options.entry_points]
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

