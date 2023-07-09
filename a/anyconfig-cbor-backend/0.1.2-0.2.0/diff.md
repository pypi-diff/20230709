# Comparing `tmp/anyconfig-cbor-backend-0.1.2.tar.gz` & `tmp/anyconfig-cbor-backend-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/anyconfig-cbor-backend-0.1.2.tar", last modified: Thu Apr 30 15:31:03 2020, max compression
+gzip compressed data, was "anyconfig-cbor-backend-0.2.0.tar", last modified: Sun Jul  9 17:13:58 2023, max compression
```

## Comparing `anyconfig-cbor-backend-0.1.2.tar` & `anyconfig-cbor-backend-0.2.0.tar`

### file list

```diff
@@ -1,35 +1,33 @@
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 15:31:03.000000 anyconfig-cbor-backend-0.1.2/
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      470 2020-04-29 17:42:43.000000 anyconfig-cbor-backend-0.1.2/.travis.yml
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1069 2018-01-05 16:33:29.000000 anyconfig-cbor-backend-0.1.2/LICENSE.MIT
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      206 2020-04-30 14:12:25.000000 anyconfig-cbor-backend-0.1.2/MANIFEST.in
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      366 2020-04-30 15:01:53.000000 anyconfig-cbor-backend-0.1.2/NEWS.txt
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1807 2020-04-30 15:31:03.000000 anyconfig-cbor-backend-0.1.2/PKG-INFO
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1723 2020-04-30 15:02:03.000000 anyconfig-cbor-backend-0.1.2/README.rst
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 15:31:03.000000 anyconfig-cbor-backend-0.1.2/pkg/
--rwxrwxr-x   0 ssato     (1000) ssato     (1000)      494 2018-01-01 13:54:49.000000 anyconfig-cbor-backend-0.1.2/pkg/copr-build.sh
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      106 2018-01-05 16:44:03.000000 anyconfig-cbor-backend-0.1.2/pkg/nose.cfg
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     2457 2020-04-30 14:35:51.000000 anyconfig-cbor-backend-0.1.2/pkg/package.spec.in
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       15 2018-01-08 12:51:09.000000 anyconfig-cbor-backend-0.1.2/requirements.txt
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1905 2020-04-30 15:31:03.000000 anyconfig-cbor-backend-0.1.2/setup.cfg
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1493 2020-04-30 14:12:25.000000 anyconfig-cbor-backend-0.1.2/setup.py
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 15:31:03.000000 anyconfig-cbor-backend-0.1.2/src/
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 15:31:03.000000 anyconfig-cbor-backend-0.1.2/src/anyconfig_cbor_backend/
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      157 2020-04-30 14:35:09.000000 anyconfig-cbor-backend-0.1.2/src/anyconfig_cbor_backend/__init__.py
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1201 2020-04-29 17:37:56.000000 anyconfig-cbor-backend-0.1.2/src/anyconfig_cbor_backend/cbor_.py
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 15:31:03.000000 anyconfig-cbor-backend-0.1.2/src/anyconfig_cbor_backend.egg-info/
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1807 2020-04-30 15:31:03.000000 anyconfig-cbor-backend-0.1.2/src/anyconfig_cbor_backend.egg-info/PKG-INFO
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      650 2020-04-30 15:31:03.000000 anyconfig-cbor-backend-0.1.2/src/anyconfig_cbor_backend.egg-info/SOURCES.txt
--rw-rw-r--   0 ssato     (1000) ssato     (1000)        1 2020-04-30 15:31:03.000000 anyconfig-cbor-backend-0.1.2/src/anyconfig_cbor_backend.egg-info/dependency_links.txt
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       59 2020-04-30 15:31:03.000000 anyconfig-cbor-backend-0.1.2/src/anyconfig_cbor_backend.egg-info/entry_points.txt
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       70 2020-04-30 15:31:03.000000 anyconfig-cbor-backend-0.1.2/src/anyconfig_cbor_backend.egg-info/requires.txt
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       23 2020-04-30 15:31:03.000000 anyconfig-cbor-backend-0.1.2/src/anyconfig_cbor_backend.egg-info/top_level.txt
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 15:31:03.000000 anyconfig-cbor-backend-0.1.2/tests/
--rw-rw-r--   0 ssato     (1000) ssato     (1000)        0 2018-07-02 10:47:14.000000 anyconfig-cbor-backend-0.1.2/tests/__init__.py
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      637 2020-04-29 17:14:56.000000 anyconfig-cbor-backend-0.1.2/tests/cbor_.py
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     8891 2020-04-30 15:01:11.000000 anyconfig-cbor-backend-0.1.2/tests/common.py
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      864 2020-04-30 14:11:24.000000 anyconfig-cbor-backend-0.1.2/tests/plugin.py
--rwxrwxr-x   0 ssato     (1000) ssato     (1000)     1545 2019-09-23 12:42:10.000000 anyconfig-cbor-backend-0.1.2/tests/releng.bats
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       46 2020-04-29 17:09:19.000000 anyconfig-cbor-backend-0.1.2/tests/requirements.txt
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 15:31:03.000000 anyconfig-cbor-backend-0.1.2/tests/res/
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       29 2018-01-07 00:53:01.000000 anyconfig-cbor-backend-0.1.2/tests/res/0.cbor
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      972 2020-04-30 15:01:11.000000 anyconfig-cbor-backend-0.1.2/tox.ini
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 17:13:58.646381 anyconfig-cbor-backend-0.2.0/
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)     1069 2018-01-05 16:33:29.000000 anyconfig-cbor-backend-0.2.0/LICENSE.MIT
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      206 2023-07-09 17:11:31.000000 anyconfig-cbor-backend-0.2.0/MANIFEST.in
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)      366 2020-04-30 15:01:53.000000 anyconfig-cbor-backend-0.2.0/NEWS.txt
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     1685 2023-07-09 17:13:58.646381 anyconfig-cbor-backend-0.2.0/PKG-INFO
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     1780 2023-07-09 17:11:31.000000 anyconfig-cbor-backend-0.2.0/README.rst
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 17:13:58.645381 anyconfig-cbor-backend-0.2.0/pkg/
+-rwxrwxr-x   0 ssato     (1000) ssato     (1000)      494 2018-01-01 13:54:49.000000 anyconfig-cbor-backend-0.2.0/pkg/copr-build.sh
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)      106 2018-01-05 16:44:03.000000 anyconfig-cbor-backend-0.2.0/pkg/nose.cfg
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     1933 2023-07-09 17:11:31.000000 anyconfig-cbor-backend-0.2.0/pkg/package.spec.in
+-rw-r--r--   0 ssato     (1000) ssato     (1000)       89 2023-07-09 17:11:31.000000 anyconfig-cbor-backend-0.2.0/requirements.txt
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     1847 2023-07-09 17:13:58.647381 anyconfig-cbor-backend-0.2.0/setup.cfg
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)     1493 2020-04-30 14:12:25.000000 anyconfig-cbor-backend-0.2.0/setup.py
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 17:13:58.643381 anyconfig-cbor-backend-0.2.0/src/
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 17:13:58.645381 anyconfig-cbor-backend-0.2.0/src/anyconfig_cbor_backend/
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      157 2023-07-09 17:11:31.000000 anyconfig-cbor-backend-0.2.0/src/anyconfig_cbor_backend/__init__.py
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     1186 2023-07-09 17:11:31.000000 anyconfig-cbor-backend-0.2.0/src/anyconfig_cbor_backend/cbor_.py
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 17:13:58.646381 anyconfig-cbor-backend-0.2.0/src/anyconfig_cbor_backend.egg-info/
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)     1685 2023-07-09 17:13:58.000000 anyconfig-cbor-backend-0.2.0/src/anyconfig_cbor_backend.egg-info/PKG-INFO
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)      629 2023-07-09 17:13:58.000000 anyconfig-cbor-backend-0.2.0/src/anyconfig_cbor_backend.egg-info/SOURCES.txt
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)        1 2023-07-09 17:13:58.000000 anyconfig-cbor-backend-0.2.0/src/anyconfig_cbor_backend.egg-info/dependency_links.txt
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)       58 2023-07-09 17:13:58.000000 anyconfig-cbor-backend-0.2.0/src/anyconfig_cbor_backend.egg-info/entry_points.txt
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)       70 2023-07-09 17:13:58.000000 anyconfig-cbor-backend-0.2.0/src/anyconfig_cbor_backend.egg-info/requires.txt
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)       23 2023-07-09 17:13:58.000000 anyconfig-cbor-backend-0.2.0/src/anyconfig_cbor_backend.egg-info/top_level.txt
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 17:13:58.646381 anyconfig-cbor-backend-0.2.0/tests/
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)        0 2018-07-02 10:47:14.000000 anyconfig-cbor-backend-0.2.0/tests/__init__.py
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     8780 2023-07-09 17:11:31.000000 anyconfig-cbor-backend-0.2.0/tests/common.py
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      113 2023-07-09 17:11:31.000000 anyconfig-cbor-backend-0.2.0/tests/requirements.txt
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 17:13:58.646381 anyconfig-cbor-backend-0.2.0/tests/res/
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)       29 2018-01-07 00:53:01.000000 anyconfig-cbor-backend-0.2.0/tests/res/0.cbor
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      637 2023-07-09 17:11:31.000000 anyconfig-cbor-backend-0.2.0/tests/test_cbor.py
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      864 2023-07-09 17:11:31.000000 anyconfig-cbor-backend-0.2.0/tests/test_plugin.py
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      829 2023-07-09 17:11:31.000000 anyconfig-cbor-backend-0.2.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `anyconfig-cbor-backend-0.1.2/LICENSE.MIT` & `anyconfig-cbor-backend-0.2.0/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `anyconfig-cbor-backend-0.1.2/README.rst` & `anyconfig-cbor-backend-0.2.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 python-anyconfig-cbor-backend
 ================================
 
 .. image:: https://img.shields.io/pypi/v/anyconfig-cbor-backend.svg
    :target: https://pypi.python.org/pypi/anyconfig-cbor-backend/
    :alt: [Latest Version]
 
-.. image:: https://img.shields.io/travis/ssato/python-anyconfig-cbor-backend.svg
-   :target: https://travis-ci.org/ssato/python-anyconfig-cbor-backend
-   :alt: Test status
+.. image:: https://github.com/ssato/python-anyconfig-cbor-backend/workflows/Tests/badge.svg
+   :target: https://github.com/ssato/python-anyconfig-cbor-backend/actions?query=workflow%3ATests
+   :alt: [Github Actions: Test status]
 
 .. image:: https://img.shields.io/coveralls/ssato/python-anyconfig-cbor-backend.svg
    :target: https://coveralls.io/r/ssato/python-anyconfig-cbor-backend
    :alt: Coverage Status
 
 .. image:: https://scrutinizer-ci.com/g/ssato/python-anyconfig-cbor-backend/badges/quality-score.png
    :target: https://scrutinizer-ci.com/g/ssato/python-anyconfig-cbor-backend
```

### Comparing `anyconfig-cbor-backend-0.1.2/pkg/package.spec.in` & `anyconfig-cbor-backend-0.2.0/pkg/package.spec.in`

 * *Files 16% similar despite different names*

```diff
@@ -4,83 +4,54 @@
 %global desctxt \
 This is a backend module for python-anyconfig to load and dump CBOR data with\
 using cbor.\
 \
 python-anyconfig is a python library to provide common APIs to load dump\
 various configuration files like INI, JSON and YAML.
 
-%if 0%{?fedora} || 0%{?rhel} > 7
-%bcond_without python2
-%else
-%bcond_with python2
-%endif
-
 Name:           python-%{pkgname}
 Version:        @VERSION@
 Release:        @RELEASE@%{?dist}
 Summary:        Backend module for python-anyconfig to load and dump CBOR data
 Group:          Development/Libraries
 License:        MIT
 URL:            https://github.com/ssato/%{name}
 Source0:        %{url}/archive/RELEASE_%{version}.tar.gz
 BuildArch:      noarch
 
-%if %{with python2}
-BuildRequires:  python2-devel
-BuildRequires:  python2-setuptools
-%endif
 BuildRequires:  python3-devel
 BuildRequires:  python3-setuptools
 
 %description %{desctxt}
 
-%if %{with python2}
-%package     -n python2-%{pkgname}
-Summary:        %{summary}
-Requires:       python2-anyconfig
-Requires:       python2-cbor
-%{?python_provide:%python_provide python2-%{pkgname}}
-
-%description -n python2-%{pkgname} %{desctxt}
-%endif
-
 %package     -n python3-%{pkgname}
 Summary:        %{summary}
 Requires:       python3-anyconfig
 Requires:       python3-cbor
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
+- New upstream release
+
 * Thu Apr 30 2020 Satoru SATOH <satoru.satoh@gmail.com> - 0.1.2-1
 - New upstream release
 
 * Thu Apr 30 2020 Satoru SATOH <satoru.satoh@gmail.com> - 0.1.1-1
 - New upstream release
 
 * Mon Sep 23 2019 Satoru SATOH <satoru.satoh@gmail.com> - 0.1.0-1
```

### Comparing `anyconfig-cbor-backend-0.1.2/setup.cfg` & `anyconfig-cbor-backend-0.2.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = anyconfig-cbor-backend
 description = Backend module for python-anyconfig to load and dump CBOR data
 project_urls = 
-	CI: Travis = https://travis-ci.org/ssato/python-anyconfig-cbor-backend
+	CI: Github Actions = https://github.com/ssato/python-anyconfig-cbor-backend/actions
 	Download = https://pypi.python.org/pypi/anyconfig-cbor-backend
 	Download RPMs = https://copr.fedoraproject.org/coprs/ssato/python-anyconfig/
 	Bug Tracker = https://github.com/ssato/python-anyconfig-cbor-backend/issues
 	Source = https://github.com/ssato/python-anyconfig-cbor-backend
 long_description = 
 	This is a backend module for python-anyconfig to support to load and dump
 	CBOR files with using cbor, https://pypi.python.org/pypi/cbor.
@@ -26,24 +26,22 @@
 url = https://github.com/ssato/python-anyconfig-cbor-backend
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
 	Environment :: Console
 	Operating System :: OS Independent
 	Topic :: Software Development :: Libraries :: Python Modules
-	Topic :: Text Processing :: Markup
 	Topic :: Utilities
 	License :: OSI Approved :: MIT License
 
 [options]
 packages = find:
 install_requires = 
 	anyconfig
```

### Comparing `anyconfig-cbor-backend-0.1.2/setup.py` & `anyconfig-cbor-backend-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `anyconfig-cbor-backend-0.1.2/src/anyconfig_cbor_backend/cbor_.py` & `anyconfig-cbor-backend-0.2.0/src/anyconfig_cbor_backend/cbor_.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 #
-# Copyright (C) 2017 - 2018 Satoru SATOH <ssato @ redhat.com>
+# Copyright (C) 2017 - 2021 Satoru SATOH <satoru.satoh@gmail.com>
 # License: MIT
 #
-# pylint: disable=too-many-ancestors
 r"""CBOR backend:
 
 - Format to support: CBOR, http://cbor.io, https://tools.ietf.org/html/rfc7049
 - Requirements: cbor, https://pypi.python.org/pypi/cbor
 - Development Status :: 4 - Beta
 - Limitations: None obvious
 - Special options:
@@ -14,21 +13,22 @@
   - All options of cbor.load{s,} and cbor.dump{s,} should work.
   - See also: https://github.com/brianolson/cbor_py/blob/master/cbor/cbor.py
 
 Changelog:
 
     .. versionadded:: 0.8.3
 """
-from __future__ import absolute_import
-import anyconfig.backend.base
 import cbor
 
+import anyconfig.backend.base
+
 
 class Parser(anyconfig.backend.base.StringStreamFnParser,
-             anyconfig.backend.base.BinaryFilesMixin):
+             anyconfig.backend.base.BinaryLoaderMixin,
+             anyconfig.backend.base.BinaryDumperMixin):
     """Parser for CBOR files.
     """
     _cid = "cbor"
     _type = "cbor"
     _extensions = ["cbor"]
     _dump_opts = ["sort_keys"]
     _allow_primitives = True
```

### Comparing `anyconfig-cbor-backend-0.1.2/src/anyconfig_cbor_backend.egg-info/SOURCES.txt` & `anyconfig-cbor-backend-0.2.0/src/anyconfig_cbor_backend.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.travis.yml
 LICENSE.MIT
 MANIFEST.in
 NEWS.txt
 README.rst
 requirements.txt
 setup.cfg
 setup.py
@@ -15,13 +14,12 @@
 src/anyconfig_cbor_backend.egg-info/PKG-INFO
 src/anyconfig_cbor_backend.egg-info/SOURCES.txt
 src/anyconfig_cbor_backend.egg-info/dependency_links.txt
 src/anyconfig_cbor_backend.egg-info/entry_points.txt
 src/anyconfig_cbor_backend.egg-info/requires.txt
 src/anyconfig_cbor_backend.egg-info/top_level.txt
 tests/__init__.py
-tests/cbor_.py
 tests/common.py
-tests/plugin.py
-tests/releng.bats
 tests/requirements.txt
+tests/test_cbor.py
+tests/test_plugin.py
 tests/res/0.cbor
```

### Comparing `anyconfig-cbor-backend-0.1.2/tests/cbor_.py` & `anyconfig-cbor-backend-0.2.0/tests/test_cbor.py`

 * *Files identical despite different names*

### Comparing `anyconfig-cbor-backend-0.1.2/tests/common.py` & `anyconfig-cbor-backend-0.2.0/tests/common.py`

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

### Comparing `anyconfig-cbor-backend-0.1.2/tests/plugin.py` & `anyconfig-cbor-backend-0.2.0/tests/test_plugin.py`

 * *Files identical despite different names*

