# Comparing `tmp/anyconfig-configobj-backend-0.1.4.tar.gz` & `tmp/anyconfig-configobj-backend-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/anyconfig-configobj-backend-0.1.4.tar", last modified: Thu Apr 30 16:31:24 2020, max compression
+gzip compressed data, was "anyconfig-configobj-backend-0.2.0.tar", last modified: Sun Jul  9 06:02:55 2023, max compression
```

## Comparing `anyconfig-configobj-backend-0.1.4.tar` & `anyconfig-configobj-backend-0.2.0.tar`

### file list

```diff
@@ -1,46 +1,43 @@
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 16:31:24.000000 anyconfig-configobj-backend-0.1.4/
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      470 2020-04-30 16:02:43.000000 anyconfig-configobj-backend-0.1.4/.travis.yml
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1023 2018-01-08 04:39:55.000000 anyconfig-configobj-backend-0.1.4/LICENSE.MIT
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      219 2020-04-30 16:03:09.000000 anyconfig-configobj-backend-0.1.4/MANIFEST.in
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     2205 2020-04-30 16:17:44.000000 anyconfig-configobj-backend-0.1.4/NEWS
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1862 2020-04-30 16:31:24.000000 anyconfig-configobj-backend-0.1.4/PKG-INFO
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     2547 2019-09-21 04:57:01.000000 anyconfig-configobj-backend-0.1.4/README.rst
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 16:31:24.000000 anyconfig-configobj-backend-0.1.4/docs/
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     6201 2019-01-27 14:17:42.000000 anyconfig-configobj-backend-0.1.4/docs/Makefile
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      485 2019-01-27 14:36:51.000000 anyconfig-configobj-backend-0.1.4/docs/about.rst
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      266 2019-03-21 12:21:23.000000 anyconfig-configobj-backend-0.1.4/docs/anyconfig_configobj_backend.configobj.rst
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      111 2019-03-21 12:21:49.000000 anyconfig-configobj-backend-0.1.4/docs/api.rst
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      822 2019-03-21 12:06:48.000000 anyconfig-configobj-backend-0.1.4/docs/badges.rst
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1109 2019-09-21 04:56:27.000000 anyconfig-configobj-backend-0.1.4/docs/build_install.rst
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      526 2019-01-27 14:18:34.000000 anyconfig-configobj-backend-0.1.4/docs/conf.py
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      131 2019-01-27 14:38:00.000000 anyconfig-configobj-backend-0.1.4/docs/header.rst
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      121 2019-03-21 12:19:25.000000 anyconfig-configobj-backend-0.1.4/docs/index.rst
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 16:31:24.000000 anyconfig-configobj-backend-0.1.4/pkg/
--rwxrwxr-x   0 ssato     (1000) ssato     (1000)      475 2019-09-21 03:13:28.000000 anyconfig-configobj-backend-0.1.4/pkg/copr-build.sh
--rwxrwxr-x   0 ssato     (1000) ssato     (1000)      376 2019-01-27 14:51:13.000000 anyconfig-configobj-backend-0.1.4/pkg/gen-readme.sh
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       99 2018-01-08 05:59:55.000000 anyconfig-configobj-backend-0.1.4/pkg/nose.cfg
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     2221 2019-09-21 05:37:32.000000 anyconfig-configobj-backend-0.1.4/pkg/package.spec.in
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       20 2018-01-08 12:21:10.000000 anyconfig-configobj-backend-0.1.4/requirements.txt
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1928 2020-04-30 16:31:24.000000 anyconfig-configobj-backend-0.1.4/setup.cfg
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1501 2020-04-30 16:03:58.000000 anyconfig-configobj-backend-0.1.4/setup.py
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 16:31:24.000000 anyconfig-configobj-backend-0.1.4/src/
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 16:31:24.000000 anyconfig-configobj-backend-0.1.4/src/anyconfig_configobj_backend/
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      180 2020-04-30 16:17:12.000000 anyconfig-configobj-backend-0.1.4/src/anyconfig_configobj_backend/__init__.py
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     3421 2019-02-14 04:37:05.000000 anyconfig-configobj-backend-0.1.4/src/anyconfig_configobj_backend/configobj_.py
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 16:31:24.000000 anyconfig-configobj-backend-0.1.4/src/anyconfig_configobj_backend.egg-info/
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1862 2020-04-30 16:31:24.000000 anyconfig-configobj-backend-0.1.4/src/anyconfig_configobj_backend.egg-info/PKG-INFO
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      891 2020-04-30 16:31:24.000000 anyconfig-configobj-backend-0.1.4/src/anyconfig_configobj_backend.egg-info/SOURCES.txt
--rw-rw-r--   0 ssato     (1000) ssato     (1000)        1 2020-04-30 16:31:24.000000 anyconfig-configobj-backend-0.1.4/src/anyconfig_configobj_backend.egg-info/dependency_links.txt
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       69 2020-04-30 16:31:24.000000 anyconfig-configobj-backend-0.1.4/src/anyconfig_configobj_backend.egg-info/entry_points.txt
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       20 2020-04-30 16:31:24.000000 anyconfig-configobj-backend-0.1.4/src/anyconfig_configobj_backend.egg-info/requires.txt
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       28 2020-04-30 16:31:24.000000 anyconfig-configobj-backend-0.1.4/src/anyconfig_configobj_backend.egg-info/top_level.txt
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 16:31:24.000000 anyconfig-configobj-backend-0.1.4/tests/
--rw-rw-r--   0 ssato     (1000) ssato     (1000)        0 2018-01-08 04:39:55.000000 anyconfig-configobj-backend-0.1.4/tests/__init__.py
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     8891 2019-09-21 06:44:51.000000 anyconfig-configobj-backend-0.1.4/tests/common.py
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1484 2019-01-22 11:57:55.000000 anyconfig-configobj-backend-0.1.4/tests/configobj_.py
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1195 2019-01-22 11:57:55.000000 anyconfig-configobj-backend-0.1.4/tests/plugin.py
--rwxrwxr-x   0 ssato     (1000) ssato     (1000)     1545 2019-09-21 03:13:50.000000 anyconfig-configobj-backend-0.1.4/tests/releng.bats
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       41 2020-04-29 18:38:13.000000 anyconfig-configobj-backend-0.1.4/tests/requirements.txt
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 16:31:24.000000 anyconfig-configobj-backend-0.1.4/tests/res/
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      753 2019-01-22 11:57:55.000000 anyconfig-configobj-backend-0.1.4/tests/res/0.configobj
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      972 2020-04-30 16:02:43.000000 anyconfig-configobj-backend-0.1.4/tox.ini
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 06:02:55.129152 anyconfig-configobj-backend-0.2.0/
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)     1023 2018-01-08 04:39:55.000000 anyconfig-configobj-backend-0.2.0/LICENSE.MIT
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      224 2023-07-09 05:59:02.000000 anyconfig-configobj-backend-0.2.0/MANIFEST.in
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)     2205 2020-04-30 16:17:44.000000 anyconfig-configobj-backend-0.2.0/NEWS
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     1763 2023-07-09 06:02:55.129152 anyconfig-configobj-backend-0.2.0/PKG-INFO
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     2959 2023-07-09 05:59:02.000000 anyconfig-configobj-backend-0.2.0/README.rst
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 06:02:55.127152 anyconfig-configobj-backend-0.2.0/docs/
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)     6201 2019-01-27 14:17:42.000000 anyconfig-configobj-backend-0.2.0/docs/Makefile
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)      485 2019-01-27 14:36:51.000000 anyconfig-configobj-backend-0.2.0/docs/about.rst
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)      266 2019-03-21 12:21:23.000000 anyconfig-configobj-backend-0.2.0/docs/anyconfig_configobj_backend.configobj.rst
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)      111 2019-03-21 12:21:49.000000 anyconfig-configobj-backend-0.2.0/docs/api.rst
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     1234 2023-07-09 05:59:02.000000 anyconfig-configobj-backend-0.2.0/docs/badges.rst
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)     1109 2019-09-21 04:56:27.000000 anyconfig-configobj-backend-0.2.0/docs/build_install.rst
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)      526 2019-01-27 14:18:34.000000 anyconfig-configobj-backend-0.2.0/docs/conf.py
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)      131 2019-01-27 14:38:00.000000 anyconfig-configobj-backend-0.2.0/docs/header.rst
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)      121 2019-03-21 12:19:25.000000 anyconfig-configobj-backend-0.2.0/docs/index.rst
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 06:02:55.128152 anyconfig-configobj-backend-0.2.0/pkg/
+-rwxr-xr-x   0 ssato     (1000) ssato     (1000)      475 2021-05-18 02:14:48.000000 anyconfig-configobj-backend-0.2.0/pkg/copr-build.sh
+-rwxrwxr-x   0 ssato     (1000) ssato     (1000)      376 2019-01-27 14:51:13.000000 anyconfig-configobj-backend-0.2.0/pkg/gen-readme.sh
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     1688 2023-07-09 05:59:02.000000 anyconfig-configobj-backend-0.2.0/pkg/package.spec.in
+-rw-r--r--   0 ssato     (1000) ssato     (1000)       94 2023-07-09 05:59:02.000000 anyconfig-configobj-backend-0.2.0/requirements.txt
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     1906 2023-07-09 06:02:55.130152 anyconfig-configobj-backend-0.2.0/setup.cfg
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)     1501 2020-04-30 16:03:58.000000 anyconfig-configobj-backend-0.2.0/setup.py
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 06:02:55.125152 anyconfig-configobj-backend-0.2.0/src/
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 06:02:55.128152 anyconfig-configobj-backend-0.2.0/src/anyconfig_configobj_backend/
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)      180 2023-07-09 06:00:42.000000 anyconfig-configobj-backend-0.2.0/src/anyconfig_configobj_backend/__init__.py
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     3426 2023-07-09 05:59:02.000000 anyconfig-configobj-backend-0.2.0/src/anyconfig_configobj_backend/configobj_.py
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 06:02:55.129152 anyconfig-configobj-backend-0.2.0/src/anyconfig_configobj_backend.egg-info/
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)     1763 2023-07-09 06:02:55.000000 anyconfig-configobj-backend-0.2.0/src/anyconfig_configobj_backend.egg-info/PKG-INFO
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)      857 2023-07-09 06:02:55.000000 anyconfig-configobj-backend-0.2.0/src/anyconfig_configobj_backend.egg-info/SOURCES.txt
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)        1 2023-07-09 06:02:55.000000 anyconfig-configobj-backend-0.2.0/src/anyconfig_configobj_backend.egg-info/dependency_links.txt
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)       68 2023-07-09 06:02:55.000000 anyconfig-configobj-backend-0.2.0/src/anyconfig_configobj_backend.egg-info/entry_points.txt
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)       20 2023-07-09 06:02:55.000000 anyconfig-configobj-backend-0.2.0/src/anyconfig_configobj_backend.egg-info/requires.txt
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)       28 2023-07-09 06:02:55.000000 anyconfig-configobj-backend-0.2.0/src/anyconfig_configobj_backend.egg-info/top_level.txt
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 06:02:55.129152 anyconfig-configobj-backend-0.2.0/tests/
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)        0 2018-01-08 04:39:55.000000 anyconfig-configobj-backend-0.2.0/tests/__init__.py
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     8780 2023-07-09 05:59:02.000000 anyconfig-configobj-backend-0.2.0/tests/common.py
+-rw-r--r--   0 ssato     (1000) ssato     (1000)       70 2023-07-09 05:59:02.000000 anyconfig-configobj-backend-0.2.0/tests/requirements.txt
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 06:02:55.129152 anyconfig-configobj-backend-0.2.0/tests/res/
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)      753 2019-01-22 11:57:55.000000 anyconfig-configobj-backend-0.2.0/tests/res/0.configobj
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     1440 2023-07-09 05:59:02.000000 anyconfig-configobj-backend-0.2.0/tests/test_configobj.py
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     1195 2023-07-09 05:59:02.000000 anyconfig-configobj-backend-0.2.0/tests/test_plugin.py
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      829 2023-07-09 05:59:02.000000 anyconfig-configobj-backend-0.2.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `anyconfig-configobj-backend-0.1.4/LICENSE.MIT` & `anyconfig-configobj-backend-0.2.0/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `anyconfig-configobj-backend-0.1.4/NEWS` & `anyconfig-configobj-backend-0.2.0/NEWS`

 * *Files identical despite different names*

### Comparing `anyconfig-configobj-backend-0.1.4/PKG-INFO` & `anyconfig-configobj-backend-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,42 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: anyconfig-configobj-backend
-Version: 0.1.4
+Version: 0.2.0
 Summary: Backend module for python-anyconfig to load and dump configobj data
 Home-page: https://github.com/ssato/python-anyconfig-configobj-backend
 Author: Satoru SATOH
 Author-email: satoru.satoh@gmail.com
 Maintainer: Satoru SATOH
 Maintainer-email: satoru.satoh@gmail.com
 License: MIT
-Project-URL: CI: Travis, https://travis-ci.org/ssato/python-anyconfig-configobj-backend
+Project-URL: CI: Github Actions, https://github.com/ssato/python-anyconfig-configobj-backend/actions
 Project-URL: Download, https://pypi.python.org/pypi/anyconfig-configobj-backend
 Project-URL: Download RPMs, https://copr.fedoraproject.org/coprs/ssato/python-anyconfig/
 Project-URL: Bug Tracker, https://github.com/ssato/python-anyconfig-configobj-backend/issues
 Project-URL: Source, https://github.com/ssato/python-anyconfig-configobj-backend
-Description: 
-        This is a backend parser module for python-anyconfig to support to load and
-        dump configobj files using configobj.
-        
-        - Author: Satoru SATOH <ssato@redhat.com>
-        - License: MIT
-        
-        SEE ALSO:
-        
-        - python-anyconfig: https://github.com/ssato/python-anyconfig
-        - configobj: https://configobj.readthedocs.io
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
+License-File: LICENSE.MIT
+
+
+This is a backend parser module for python-anyconfig to support to load and
+dump configobj files using configobj.
+
+- Author: Satoru SATOH <ssato@redhat.com>
+- License: MIT
+
+SEE ALSO:
+
+- python-anyconfig: https://github.com/ssato/python-anyconfig
+- configobj: https://configobj.readthedocs.io
```

### Comparing `anyconfig-configobj-backend-0.1.4/README.rst` & `anyconfig-configobj-backend-0.2.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 ====================================
 python-anyconfig-configobj-backend
 ====================================
 
 .. vim:sw=2:ts=2:et:
 
-.. image:: https://img.shields.io/travis/ssato/python-anyconfig-configobj-backend.svg
-   :target: https://travis-ci.org/ssato/python-anyconfig-configobj-backend
-   :alt: Test status
+.. image:: https://img.shields.io/pypi/pyversions/anyconfig-configobj-backend.svg
+   :target: https://pypi.python.org/pypi/anyconfig-configobj-backend/
+   :alt: [Python versions]
+
+.. image:: https://img.shields.io/pypi/l/anyconfig-configobj-backend.svg
+   :target: https://pypi.python.org/pypi/anyconfig-configobj-backend/
+   :alt: MIT License
+
+.. image:: https://github.com/ssato/python-anyconfig-configobj-backend/workflows/Tests/badge.svg
+   :target: https://github.com/ssato/python-anyconfig-configobj-backend/actions?query=workflow%3ATests
+   :alt: [Github Actions: Test status]
 
 .. image:: https://img.shields.io/coveralls/ssato/python-anyconfig-configobj-backend.svg
    :target: https://coveralls.io/r/ssato/python-anyconfig-configobj-backend
    :alt: Coverage Status
 
-.. image:: https://landscape.io/github/ssato/python-anyconfig-configobj-backend/master/landscape.png
-   :target: https://landscape.io/github/ssato/python-anyconfig-configobj-backend/master
-   :alt: Code Health
+.. image:: https://codecov.io/gh/ssato/python-anyconfig-configobj-backend/branch/next/graph/badge.svg?token=CEHaIGm60z
+   :target: https://codecov.io/gh/ssato/python-anyconfig-configobj-backend
+   :alt: [Codecov Status]
 
 .. image:: https://readthedocs.org/projects/python-anyconfig-configobj-backend/badge/?version=latest
    :target: http://python-anyconfig-configobj-backend.readthedocs.io/en/latest/?badge=latest
    :alt: Doc Status
 
 .. vim:sw=2:ts=2:et:
```

### Comparing `anyconfig-configobj-backend-0.1.4/docs/Makefile` & `anyconfig-configobj-backend-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `anyconfig-configobj-backend-0.1.4/docs/badges.rst` & `anyconfig-configobj-backend-0.2.0/docs/badges.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 
-.. image:: https://img.shields.io/travis/ssato/python-anyconfig-configobj-backend.svg
-   :target: https://travis-ci.org/ssato/python-anyconfig-configobj-backend
-   :alt: Test status
+.. image:: https://img.shields.io/pypi/pyversions/anyconfig-configobj-backend.svg
+   :target: https://pypi.python.org/pypi/anyconfig-configobj-backend/
+   :alt: [Python versions]
+
+.. image:: https://img.shields.io/pypi/l/anyconfig-configobj-backend.svg
+   :target: https://pypi.python.org/pypi/anyconfig-configobj-backend/
+   :alt: MIT License
+
+.. image:: https://github.com/ssato/python-anyconfig-configobj-backend/workflows/Tests/badge.svg
+   :target: https://github.com/ssato/python-anyconfig-configobj-backend/actions?query=workflow%3ATests
+   :alt: [Github Actions: Test status]
 
 .. image:: https://img.shields.io/coveralls/ssato/python-anyconfig-configobj-backend.svg
    :target: https://coveralls.io/r/ssato/python-anyconfig-configobj-backend
    :alt: Coverage Status
 
-.. image:: https://landscape.io/github/ssato/python-anyconfig-configobj-backend/master/landscape.png
-   :target: https://landscape.io/github/ssato/python-anyconfig-configobj-backend/master
-   :alt: Code Health
+.. image:: https://codecov.io/gh/ssato/python-anyconfig-configobj-backend/branch/next/graph/badge.svg?token=CEHaIGm60z
+   :target: https://codecov.io/gh/ssato/python-anyconfig-configobj-backend
+   :alt: [Codecov Status]
 
 .. image:: https://readthedocs.org/projects/python-anyconfig-configobj-backend/badge/?version=latest
    :target: http://python-anyconfig-configobj-backend.readthedocs.io/en/latest/?badge=latest
    :alt: Doc Status
 
 .. vim:sw=2:ts=2:et:
```

### Comparing `anyconfig-configobj-backend-0.1.4/docs/build_install.rst` & `anyconfig-configobj-backend-0.2.0/docs/build_install.rst`

 * *Files identical despite different names*

### Comparing `anyconfig-configobj-backend-0.1.4/docs/conf.py` & `anyconfig-configobj-backend-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `anyconfig-configobj-backend-0.1.4/pkg/package.spec.in` & `anyconfig-configobj-backend-0.2.0/pkg/package.spec.in`

 * *Files 13% similar despite different names*

```diff
@@ -4,83 +4,54 @@
 %global desctxt \
 This is a python backend module for python-anyconfig to load and dump configobj\
 data.\
 \
 python-anyconfig is a python library to provide common APIs to load dump\
 various configuration files like INI, JSON and YAML.
 
-%if 0%{?rhel} == 7 || 0%{?epel} == 7
-%bcond_without python2
-%else
-%bcond_with python2
-%endif
-
 Name:           python-%{pkgname}
 Version:        @VERSION@
 Release:        @RELEASE@
 Summary:        Backend for python-anyconfig to load and dump configobj data
 Group:          Development/Libraries
 License:        MIT
 URL:            https://github.com/ssato/python-anyconfig-configobj-backend
 Source0:        %{url}/archive/RELEASE_%{version}.tar.gz
 BuildArch:      noarch
 
-%if %{with python2}
-BuildRequires:  python2-devel
-BuildRequires:  python2-setuptools
-%endif
 BuildRequires:  python3-devel
 BuildRequires:  python3-setuptools
 
 %description    %{desctxt}
 
-%if %{with python2}
-%package     -n python2-%{pkgname}
-Summary:        %{summary}
-Requires:       python2-anyconfig
-Requires:       python2-configobj
-%{?python_provide:%python_provide python2-%{pkgname}}
-
-%description -n python2-%{pkgname} %{desctxt}
-%endif
-
 %package     -n python3-%{pkgname}
 Summary:        %{summary}
 Requires:       python3-anyconfig
 Requires:       python3-configobj
 %{?python_provide:%python_provide python3-%{pkgname}}
 
 %description -n python3-%{pkgname} %{desctxt}
 
 %prep
 %autosetup   -n %{pkgname}-%{version}
 
 %build
-%if %{with python2}
-%py2_build
-%endif
 %py3_build
 
 %install
-%if %{with python2}
-%py2_install
-%endif
 %py3_install
 
-%if %{with python2}
-%files       -n python2-%{pkgname}
-%doc README.rst
-%{python2_sitelib}/*
-%endif
-
 %files       -n python3-%{pkgname}
 %doc README.rst
 %{python3_sitelib}/*
 
 %changelog
+* Tue May 18 2021 Satoru SATOH <satoru.satoh@gmail.com> - 0.2.0-1
+- new upstream release
+
 * Sat Sep 21 2019 Satoru SATOH <satoru.satoh@gmail.com> - 0.1.0-1
 - new upstream release
 
 * Tue Jan  9 2018 Satoru SATOH <ssato@redhat.com> - 0.0.4-1
 - new upstream release
 
 * Mon Jan  8 2018 Satoru SATOH <ssato@redhat.com> - 0.0.3-1
```

### Comparing `anyconfig-configobj-backend-0.1.4/setup.cfg` & `anyconfig-configobj-backend-0.2.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = anyconfig-configobj-backend
 description = Backend module for python-anyconfig to load and dump configobj data
 project_urls = 
-	CI: Travis = https://travis-ci.org/ssato/python-anyconfig-configobj-backend
+	CI: Github Actions = https://github.com/ssato/python-anyconfig-configobj-backend/actions
 	Download = https://pypi.python.org/pypi/anyconfig-configobj-backend
 	Download RPMs = https://copr.fedoraproject.org/coprs/ssato/python-anyconfig/
 	Bug Tracker = https://github.com/ssato/python-anyconfig-configobj-backend/issues
 	Source = https://github.com/ssato/python-anyconfig-configobj-backend
 long_description = 
 	This is a backend parser module for python-anyconfig to support to load and
 	dump configobj files using configobj.
@@ -29,20 +29,19 @@
 url = https://github.com/ssato/python-anyconfig-configobj-backend
 platforms = 
 	any
 classifiers = 
 	Development Status :: 4 - Beta
 	Intended Audience :: Developers
 	Programming Language :: Python
-	Programming Language :: Python :: 2
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 2.7
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Operating System :: OS Independent
 	Topic :: Software Development :: Libraries :: Python Modules
 	Topic :: Text Processing :: Markup
 	Topic :: Utilities
 	License :: OSI Approved :: MIT License
 
 [options]
```

### Comparing `anyconfig-configobj-backend-0.1.4/setup.py` & `anyconfig-configobj-backend-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `anyconfig-configobj-backend-0.1.4/src/anyconfig_configobj_backend/configobj_.py` & `anyconfig-configobj-backend-0.2.0/src/anyconfig_configobj_backend/configobj_.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2013 - 2019 Satoru SATOH <satoru.satoh @ gmail.com>
+# Copyright (C) 2013 - 2021 Satoru SATOH <satoru.satoh @ gmail.com>
 # License: MIT
 #
 r"""Configobj backend:
 
 - Format to support: configobj,
   https://bit.ly/2TgURnL (https://configobj.readthedocs.io)
 - Requirements: configobj (https://pypi.python.org/pypi/configobj/)
@@ -24,26 +24,27 @@
 
 .. versionchanged:: 0.5.0
 
    - Now loading and dumping options are detected automatically from inspection
      result if possible. Also these became not distinguished because these will
      be passed to configobj.Configuration anyway.
 """
-from __future__ import absolute_import
-
+import inspect
 import os
+
 import configobj
-import anyconfig.backend.base
 
-from anyconfig.compat import getargspec
+import anyconfig.backend.base
 
 
 try:
-    _LOAD_OPTS = [a for a in getargspec(configobj.ConfigObj).args
-                  if a not in "self infile".split()]
+    _LOAD_OPTS = [
+        a for a in inspect.getfullargspec(configobj.ConfigObj).args
+        if a not in {'self', 'infile'}
+    ]
 except (TypeError, AttributeError):
     _LOAD_OPTS = ("options configspec encoding interpolation raise_errors"
                   "list_values create_empty file_error stringify"
                   "indent_type default_encoding unrepr write_empty_values"
                   "_inspec").split()
 
 
@@ -70,15 +71,16 @@
 
     :return: Mapping object
     """
     return container(configobj.ConfigObj(path_or_strm, **opts))
 
 
 class Parser(anyconfig.backend.base.StreamParser,
-             anyconfig.backend.base.BinaryFilesMixin):
+             anyconfig.backend.base.BinaryLoaderMixin,
+             anyconfig.backend.base.BinaryDumperMixin):
     """
     Parser for Ini-like config files which configobj supports.
     """
     _cid = "configobj"
     _type = "configobj"
     _priority = 10
     _load_opts = _LOAD_OPTS  # options on dump will be just ignored.
```

### Comparing `anyconfig-configobj-backend-0.1.4/src/anyconfig_configobj_backend.egg-info/PKG-INFO` & `anyconfig-configobj-backend-0.2.0/src/anyconfig_configobj_backend.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,42 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: anyconfig-configobj-backend
-Version: 0.1.4
+Version: 0.2.0
 Summary: Backend module for python-anyconfig to load and dump configobj data
 Home-page: https://github.com/ssato/python-anyconfig-configobj-backend
 Author: Satoru SATOH
 Author-email: satoru.satoh@gmail.com
 Maintainer: Satoru SATOH
 Maintainer-email: satoru.satoh@gmail.com
 License: MIT
-Project-URL: CI: Travis, https://travis-ci.org/ssato/python-anyconfig-configobj-backend
+Project-URL: CI: Github Actions, https://github.com/ssato/python-anyconfig-configobj-backend/actions
 Project-URL: Download, https://pypi.python.org/pypi/anyconfig-configobj-backend
 Project-URL: Download RPMs, https://copr.fedoraproject.org/coprs/ssato/python-anyconfig/
 Project-URL: Bug Tracker, https://github.com/ssato/python-anyconfig-configobj-backend/issues
 Project-URL: Source, https://github.com/ssato/python-anyconfig-configobj-backend
-Description: 
-        This is a backend parser module for python-anyconfig to support to load and
-        dump configobj files using configobj.
-        
-        - Author: Satoru SATOH <ssato@redhat.com>
-        - License: MIT
-        
-        SEE ALSO:
-        
-        - python-anyconfig: https://github.com/ssato/python-anyconfig
-        - configobj: https://configobj.readthedocs.io
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
+License-File: LICENSE.MIT
+
+
+This is a backend parser module for python-anyconfig to support to load and
+dump configobj files using configobj.
+
+- Author: Satoru SATOH <ssato@redhat.com>
+- License: MIT
+
+SEE ALSO:
+
+- python-anyconfig: https://github.com/ssato/python-anyconfig
+- configobj: https://configobj.readthedocs.io
```

### Comparing `anyconfig-configobj-backend-0.1.4/src/anyconfig_configobj_backend.egg-info/SOURCES.txt` & `anyconfig-configobj-backend-0.2.0/src/anyconfig_configobj_backend.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.travis.yml
 LICENSE.MIT
 MANIFEST.in
 NEWS
 README.rst
 requirements.txt
 setup.cfg
 setup.py
@@ -14,24 +13,22 @@
 docs/badges.rst
 docs/build_install.rst
 docs/conf.py
 docs/header.rst
 docs/index.rst
 pkg/copr-build.sh
 pkg/gen-readme.sh
-pkg/nose.cfg
 pkg/package.spec.in
 src/anyconfig_configobj_backend/__init__.py
 src/anyconfig_configobj_backend/configobj_.py
 src/anyconfig_configobj_backend.egg-info/PKG-INFO
 src/anyconfig_configobj_backend.egg-info/SOURCES.txt
 src/anyconfig_configobj_backend.egg-info/dependency_links.txt
 src/anyconfig_configobj_backend.egg-info/entry_points.txt
 src/anyconfig_configobj_backend.egg-info/requires.txt
 src/anyconfig_configobj_backend.egg-info/top_level.txt
 tests/__init__.py
 tests/common.py
-tests/configobj_.py
-tests/plugin.py
-tests/releng.bats
 tests/requirements.txt
+tests/test_configobj.py
+tests/test_plugin.py
 tests/res/0.configobj
```

### Comparing `anyconfig-configobj-backend-0.1.4/tests/common.py` & `anyconfig-configobj-backend-0.2.0/tests/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 #
 # Copyright (C) 2011 - 2018 Satoru SATOH <ssato at redhat.com>
 #
 # pylint: disable=missing-docstring,invalid-name,too-few-public-methods
 # pylint: disable=ungrouped-imports
-from __future__ import absolute_import
-
 import copy
 import os.path
 import tempfile
 import unittest
 
 from os import linesep as lsep
+from collections import OrderedDict
 
-import anyconfig.compat
 import anyconfig.ioinfo
 
-from anyconfig.compat import OrderedDict
 from anyconfig.utils import is_dict_like
 
 
 CNF_0 = OrderedDict((("DEFAULT", OrderedDict((("a", "0"), ("b", "bbb"),
                                               ("c", "5")))),
                      ("sect0", OrderedDict((("a", "0"), ("b", "bbb"),
                                             ("c", "5"),
@@ -28,15 +25,15 @@
 CNF_1["sect0"]["d"] = CNF_1["sect0"]["d"].split()
 
 
 def _bytes(astr):
     """
     Convert a string to bytes. Do nothing in python 2.6.
     """
-    return bytes(astr, 'utf-8') if anyconfig.compat.IS_PYTHON_3 else astr
+    return bytes(astr, 'utf-8')
 
 
 CNF_2 = OrderedDict((("a", 0.1), ("b", _bytes("bbb")),
                      ("sect0", OrderedDict((("c", [_bytes("x"), _bytes("y"),
                                                    _bytes("z")]), )))))
```

### Comparing `anyconfig-configobj-backend-0.1.4/tests/configobj_.py` & `anyconfig-configobj-backend-0.2.0/tests/test_configobj.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 #
 # Copyright (C) 2013 - 2018 Satoru SATOH <ssato @ redhat.com>
 # License: MIT
 #
 # pylint: disable=missing-docstring,invalid-name,too-few-public-methods
 # pylint: disable=ungrouped-imports
-from __future__ import absolute_import
 import os.path
 
-from anyconfig.compat import OrderedDict as ODict
+from collections import OrderedDict as ODict
 
 import anyconfig_configobj_backend as TT
 import tests.common as TBC
 
 
 _ML_0 = """A multiline value,
 that spans more than one line :-)
```

### Comparing `anyconfig-configobj-backend-0.1.4/tests/plugin.py` & `anyconfig-configobj-backend-0.2.0/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `anyconfig-configobj-backend-0.1.4/tests/res/0.configobj` & `anyconfig-configobj-backend-0.2.0/tests/res/0.configobj`

 * *Files identical despite different names*

