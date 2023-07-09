# Comparing `tmp/anyconfig-cbor2-backend-0.1.2.tar.gz` & `tmp/anyconfig-cbor2-backend-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/anyconfig-cbor2-backend-0.1.2.tar", last modified: Thu Apr 30 15:54:03 2020, max compression
+gzip compressed data, was "anyconfig-cbor2-backend-0.2.0.tar", last modified: Sun Jul  9 17:27:45 2023, max compression
```

## Comparing `anyconfig-cbor2-backend-0.1.2.tar` & `anyconfig-cbor2-backend-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,41 @@
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 15:54:03.000000 anyconfig-cbor2-backend-0.1.2/
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      522 2020-04-30 15:42:02.000000 anyconfig-cbor2-backend-0.1.2/.travis.yml
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1069 2018-01-05 16:33:29.000000 anyconfig-cbor2-backend-0.1.2/LICENSE.MIT
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      206 2020-04-30 15:33:44.000000 anyconfig-cbor2-backend-0.1.2/MANIFEST.in
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1385 2020-04-30 15:45:34.000000 anyconfig-cbor2-backend-0.1.2/NEWS
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1761 2020-04-30 15:54:03.000000 anyconfig-cbor2-backend-0.1.2/PKG-INFO
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1999 2019-09-21 07:04:07.000000 anyconfig-cbor2-backend-0.1.2/README.rst
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 15:54:03.000000 anyconfig-cbor2-backend-0.1.2/extras/
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      494 2018-07-02 16:10:45.000000 anyconfig-cbor2-backend-0.1.2/extras/cbor2-hardcode-version.patch
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 15:54:03.000000 anyconfig-cbor2-backend-0.1.2/pkg/
--rwxrwxr-x   0 ssato     (1000) ssato     (1000)      494 2018-01-01 13:54:49.000000 anyconfig-cbor2-backend-0.1.2/pkg/copr-build.sh
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      107 2018-01-07 11:55:49.000000 anyconfig-cbor2-backend-0.1.2/pkg/nose.cfg
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     2363 2019-09-23 05:08:31.000000 anyconfig-cbor2-backend-0.1.2/pkg/package.spec.in
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       16 2019-09-21 06:55:54.000000 anyconfig-cbor2-backend-0.1.2/requirements.txt
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1836 2020-04-30 15:54:03.000000 anyconfig-cbor2-backend-0.1.2/setup.cfg
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1493 2020-04-30 15:33:44.000000 anyconfig-cbor2-backend-0.1.2/setup.py
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 15:54:03.000000 anyconfig-cbor2-backend-0.1.2/src/
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 15:54:03.000000 anyconfig-cbor2-backend-0.1.2/src/anyconfig_cbor2_backend/
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      158 2020-04-30 15:44:47.000000 anyconfig-cbor2-backend-0.1.2/src/anyconfig_cbor2_backend/__init__.py
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1562 2019-09-21 06:32:40.000000 anyconfig-cbor2-backend-0.1.2/src/anyconfig_cbor2_backend/cbor2_.py
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 15:54:03.000000 anyconfig-cbor2-backend-0.1.2/src/anyconfig_cbor2_backend.egg-info/
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1761 2020-04-30 15:54:03.000000 anyconfig-cbor2-backend-0.1.2/src/anyconfig_cbor2_backend.egg-info/PKG-INFO
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      692 2020-04-30 15:54:03.000000 anyconfig-cbor2-backend-0.1.2/src/anyconfig_cbor2_backend.egg-info/SOURCES.txt
--rw-rw-r--   0 ssato     (1000) ssato     (1000)        1 2020-04-30 15:54:03.000000 anyconfig-cbor2-backend-0.1.2/src/anyconfig_cbor2_backend.egg-info/dependency_links.txt
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       61 2020-04-30 15:54:03.000000 anyconfig-cbor2-backend-0.1.2/src/anyconfig_cbor2_backend.egg-info/entry_points.txt
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       16 2020-04-30 15:54:03.000000 anyconfig-cbor2-backend-0.1.2/src/anyconfig_cbor2_backend.egg-info/requires.txt
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       24 2020-04-30 15:54:03.000000 anyconfig-cbor2-backend-0.1.2/src/anyconfig_cbor2_backend.egg-info/top_level.txt
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 15:54:03.000000 anyconfig-cbor2-backend-0.1.2/tests/
--rw-rw-r--   0 ssato     (1000) ssato     (1000)        0 2018-01-14 04:56:17.000000 anyconfig-cbor2-backend-0.1.2/tests/__init__.py
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      656 2020-04-29 18:00:17.000000 anyconfig-cbor2-backend-0.1.2/tests/cbor2_.py
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     8891 2019-09-21 06:44:11.000000 anyconfig-cbor2-backend-0.1.2/tests/common.py
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1463 2020-04-30 15:34:32.000000 anyconfig-cbor2-backend-0.1.2/tests/plugin.py
--rwxrwxr-x   0 ssato     (1000) ssato     (1000)     1545 2019-09-23 02:47:46.000000 anyconfig-cbor2-backend-0.1.2/tests/releng.bats
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       41 2020-04-29 17:56:31.000000 anyconfig-cbor2-backend-0.1.2/tests/requirements.txt
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 15:54:03.000000 anyconfig-cbor2-backend-0.1.2/tests/res/
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       29 2018-01-14 04:56:17.000000 anyconfig-cbor2-backend-0.1.2/tests/res/0.cbor
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      972 2020-04-30 15:33:44.000000 anyconfig-cbor2-backend-0.1.2/tox.ini
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 17:27:45.155047 anyconfig-cbor2-backend-0.2.0/
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 17:27:45.151047 anyconfig-cbor2-backend-0.2.0/.github/
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 17:27:45.153047 anyconfig-cbor2-backend-0.2.0/.github/workflows/
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      956 2023-07-09 17:26:42.000000 anyconfig-cbor2-backend-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      858 2023-07-09 17:26:42.000000 anyconfig-cbor2-backend-0.2.0/.github/workflows/tests.yml
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)      522 2020-04-30 15:42:02.000000 anyconfig-cbor2-backend-0.2.0/.travis.yml
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)     1069 2018-01-05 16:33:29.000000 anyconfig-cbor2-backend-0.2.0/LICENSE.MIT
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      206 2023-07-09 17:26:42.000000 anyconfig-cbor2-backend-0.2.0/MANIFEST.in
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)     1385 2020-04-30 15:45:34.000000 anyconfig-cbor2-backend-0.2.0/NEWS
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     1639 2023-07-09 17:27:45.155047 anyconfig-cbor2-backend-0.2.0/PKG-INFO
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     2056 2023-07-09 17:26:42.000000 anyconfig-cbor2-backend-0.2.0/README.rst
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 17:27:45.153047 anyconfig-cbor2-backend-0.2.0/extras/
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)      494 2018-07-02 16:10:45.000000 anyconfig-cbor2-backend-0.2.0/extras/cbor2-hardcode-version.patch
+-rw-r--r--   0 ssato     (1000) ssato     (1000)       66 2023-07-09 17:26:42.000000 anyconfig-cbor2-backend-0.2.0/mypy.ini
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 17:27:45.153047 anyconfig-cbor2-backend-0.2.0/pkg/
+-rwxrwxr-x   0 ssato     (1000) ssato     (1000)      494 2018-01-01 13:54:49.000000 anyconfig-cbor2-backend-0.2.0/pkg/copr-build.sh
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)      107 2018-01-07 11:55:49.000000 anyconfig-cbor2-backend-0.2.0/pkg/nose.cfg
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     1757 2023-07-09 17:26:42.000000 anyconfig-cbor2-backend-0.2.0/pkg/package.spec.in
+-rw-r--r--   0 ssato     (1000) ssato     (1000)       90 2023-07-09 17:26:42.000000 anyconfig-cbor2-backend-0.2.0/requirements.txt
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     1778 2023-07-09 17:27:45.156047 anyconfig-cbor2-backend-0.2.0/setup.cfg
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)     1493 2020-04-30 15:33:44.000000 anyconfig-cbor2-backend-0.2.0/setup.py
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 17:27:45.151047 anyconfig-cbor2-backend-0.2.0/src/
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 17:27:45.153047 anyconfig-cbor2-backend-0.2.0/src/anyconfig_cbor2_backend/
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      158 2023-07-09 17:26:42.000000 anyconfig-cbor2-backend-0.2.0/src/anyconfig_cbor2_backend/__init__.py
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     1578 2023-07-09 17:26:42.000000 anyconfig-cbor2-backend-0.2.0/src/anyconfig_cbor2_backend/cbor2_.py
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 17:27:45.154047 anyconfig-cbor2-backend-0.2.0/src/anyconfig_cbor2_backend.egg-info/
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)     1639 2023-07-09 17:27:45.000000 anyconfig-cbor2-backend-0.2.0/src/anyconfig_cbor2_backend.egg-info/PKG-INFO
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)      750 2023-07-09 17:27:45.000000 anyconfig-cbor2-backend-0.2.0/src/anyconfig_cbor2_backend.egg-info/SOURCES.txt
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)        1 2023-07-09 17:27:45.000000 anyconfig-cbor2-backend-0.2.0/src/anyconfig_cbor2_backend.egg-info/dependency_links.txt
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)       60 2023-07-09 17:27:45.000000 anyconfig-cbor2-backend-0.2.0/src/anyconfig_cbor2_backend.egg-info/entry_points.txt
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)       16 2023-07-09 17:27:45.000000 anyconfig-cbor2-backend-0.2.0/src/anyconfig_cbor2_backend.egg-info/requires.txt
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)       24 2023-07-09 17:27:45.000000 anyconfig-cbor2-backend-0.2.0/src/anyconfig_cbor2_backend.egg-info/top_level.txt
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 17:27:45.155047 anyconfig-cbor2-backend-0.2.0/tests/
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)        0 2018-01-14 04:56:17.000000 anyconfig-cbor2-backend-0.2.0/tests/__init__.py
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     8780 2023-07-09 17:26:42.000000 anyconfig-cbor2-backend-0.2.0/tests/common.py
+-rw-r--r--   0 ssato     (1000) ssato     (1000)       87 2023-07-09 17:26:42.000000 anyconfig-cbor2-backend-0.2.0/tests/requirements.txt
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 17:27:45.155047 anyconfig-cbor2-backend-0.2.0/tests/res/
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)       29 2018-01-14 04:56:17.000000 anyconfig-cbor2-backend-0.2.0/tests/res/0.cbor
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      656 2023-07-09 17:26:42.000000 anyconfig-cbor2-backend-0.2.0/tests/test_cbor2.py
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     1463 2023-07-09 17:26:42.000000 anyconfig-cbor2-backend-0.2.0/tests/test_plugin.py
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      829 2023-07-09 17:26:42.000000 anyconfig-cbor2-backend-0.2.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `anyconfig-cbor2-backend-0.1.2/.travis.yml` & `anyconfig-cbor2-backend-0.2.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `anyconfig-cbor2-backend-0.1.2/LICENSE.MIT` & `anyconfig-cbor2-backend-0.2.0/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `anyconfig-cbor2-backend-0.1.2/NEWS` & `anyconfig-cbor2-backend-0.2.0/NEWS`

 * *Files identical despite different names*

### Comparing `anyconfig-cbor2-backend-0.1.2/PKG-INFO` & `anyconfig-cbor2-backend-0.2.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: anyconfig-cbor2-backend
-Version: 0.1.2
+Version: 0.2.0
 Summary: Backend module for python-anyconfig to load and dump CBOR data
 Home-page: https://github.com/ssato/python-anyconfig-cbor2-backend
 Author: Satoru SATOH
 Author-email: satoru.satoh@gmail.com
 Maintainer: Satoru SATOH
 Maintainer-email: satoru.satoh@gmail.com
 License: MIT
-Project-URL: CI: Travis, https://travis-ci.org/ssato/python-anyconfig-cbor2-backend
+Project-URL: CI: Github Actions, https://github.com/ssato/python-anyconfig-cbor2-backend/actions
 Project-URL: Download, https://pypi.python.org/pypi/anyconfig-cbor2-backend
 Project-URL: Download RPMs, https://copr.fedoraproject.org/coprs/ssato/python-anyconfig/
 Project-URL: Bug Tracker, https://github.com/ssato/python-anyconfig-cbor2-backend/issues
 Project-URL: Source, https://github.com/ssato/python-anyconfig-cbor2-backend
-Description: 
-        This is a backend parser module for python-anyconfig to support to load and
-        dump CBOR files using cbor2, https://pypi.python.org/pypi/cbor2.
-        
-        SEE ALSO:
-        
-        - python-anyconfig: https://github.com/ssato/python-anyconfig
-        - CBOR spec: http://cbor.io
 Platform: any
 Classifier: Development Status :: 3 - Alpha
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
-Classifier: Topic :: Text Processing :: Markup
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
+License-File: LICENSE.MIT
+
+
+This is a backend parser module for python-anyconfig to support to load and
+dump CBOR files using cbor2, https://pypi.python.org/pypi/cbor2.
+
+SEE ALSO:
+
+- python-anyconfig: https://github.com/ssato/python-anyconfig
+- CBOR spec: http://cbor.io
```

### Comparing `anyconfig-cbor2-backend-0.1.2/README.rst` & `anyconfig-cbor2-backend-0.2.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 python-anyconfig-cbor2-backend
 ================================
 
 .. image:: https://img.shields.io/pypi/v/anyconfig-cbor2-backend.svg
    :target: https://pypi.python.org/pypi/anyconfig-cbor2-backend/
    :alt: [Latest Verscbor2]
 
-.. image:: https://img.shields.io/travis/ssato/python-anyconfig-cbor2-backend.svg
-   :target: https://travis-ci.org/ssato/python-anyconfig-cbor2-backend
-   :alt: Test status
+.. image:: https://github.com/ssato/python-anyconfig-cbor2-backend/workflows/Tests/badge.svg
+   :target: https://github.com/ssato/python-anyconfig-cbor2-backend/actions?query=workflow%3ATests
+   :alt: [Github Actions: Test status]
 
 .. image:: https://img.shields.io/coveralls/ssato/python-anyconfig-cbor2-backend.svg
    :target: https://coveralls.io/r/ssato/python-anyconfig-cbor2-backend
    :alt: Coverage Status
 
 .. image:: https://landscape.io/github/ssato/python-anyconfig-cbor2-backend/master/landscape.png
    :target: https://landscape.io/github/ssato/python-anyconfig-cbor2-backend/master
```

### Comparing `anyconfig-cbor2-backend-0.1.2/pkg/package.spec.in` & `anyconfig-cbor2-backend-0.2.0/pkg/package.spec.in`

 * *Files 16% similar despite different names*

```diff
@@ -3,83 +3,53 @@
 
 %global desctxt \
 This is a CBOR backend module for python-anyconfig with using cbor2.\
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
 License:        MIT
 URL:            https://github.com/ssato/python-anyconfig-cbor2-backend
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
-# Both python{2,3}-cbor2 are available from my copr repo, ssato/python-anyconfig.
-%package     -n python2-%{pkgname}
-Summary:        %{summary}
-Requires:       python2-anyconfig
-Requires:       python2-cbor2
-%{?python_provide:%python_provide python2-%{pkgname}}
-
-%description -n python2-%{pkgname} %{desctxt}
-%endif
-
 %package     -n python3-%{pkgname}
 Summary:        %{sumtxt}
 Requires:       python3-anyconfig
 Requires:       python3-cbor2
 %{?python_provide:%python_provide python3-%{pkgname}}
 
 %description -n python3-%{pkgname} %{desctxt}
 
 %prep
 %autosetup -n %{pkgname}-%{version}
 
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
-%files -n python2-%{pkgname}
-%doc README.rst NEWS
-%{python2_sitelib}/*
-%endif
-
 %files -n python3-%{pkgname}
 %doc README.rst NEWS
 %{python3_sitelib}/*
 
 %changelog
+* Tue May 18 2021 Satoru SATOH <satoru.satoh@gmail.com> - 0.2.0-1
+- new upstream release
+
 * Mon Sep 23 2019 Satoru SATOH <satoru.satoh@gmail.com> - 0.1.0-1
 - new upstream release
 
 * Thu Jan  3 2019 Satoru SATOH <ssato@redhat.com> - 0.0.4-1
 - new upstream release
 
 * Mon Jul  2 2018 Satoru SATOH <ssato@redhat.com> - 0.0.3-1
```

### Comparing `anyconfig-cbor2-backend-0.1.2/setup.cfg` & `anyconfig-cbor2-backend-0.2.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = anyconfig-cbor2-backend
 description = Backend module for python-anyconfig to load and dump CBOR data
 project_urls = 
-	CI: Travis = https://travis-ci.org/ssato/python-anyconfig-cbor2-backend
+	CI: Github Actions = https://github.com/ssato/python-anyconfig-cbor2-backend/actions
 	Download = https://pypi.python.org/pypi/anyconfig-cbor2-backend
 	Download RPMs = https://copr.fedoraproject.org/coprs/ssato/python-anyconfig/
 	Bug Tracker = https://github.com/ssato/python-anyconfig-cbor2-backend/issues
 	Source = https://github.com/ssato/python-anyconfig-cbor2-backend
 long_description = 
 	This is a backend parser module for python-anyconfig to support to load and
 	dump CBOR files using cbor2, https://pypi.python.org/pypi/cbor2.
@@ -26,23 +26,21 @@
 url = https://github.com/ssato/python-anyconfig-cbor2-backend
 platforms = 
 	any
 classifiers = 
 	Development Status :: 3 - Alpha
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
-	Topic :: Text Processing :: Markup
 	Topic :: Utilities
 	License :: OSI Approved :: MIT License
 
 [options]
 include_package_data = True
 packages = find:
 install_requires =
```

### Comparing `anyconfig-cbor2-backend-0.1.2/setup.py` & `anyconfig-cbor2-backend-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `anyconfig-cbor2-backend-0.1.2/src/anyconfig_cbor2_backend/cbor2_.py` & `anyconfig-cbor2-backend-0.2.0/src/anyconfig_cbor2_backend/cbor2_.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 #
-# Copyright (C) 2018 Satoru SATOH <ssato @ redhat.com>
-# Copyright (C) 2019 Satoru SATOH <satoru.satoh @ gmail.com>
+# Copyright (C) 2018 - 2021 Satoru SATOH <satoru.satoh @ gmail.com>
 # License: MIT
 #
 # pylint: disable=too-many-ancestors
 r"""CBOR backend:
 
 - Format to support: CBOR, http://cbor.io, https://tools.ietf.org/html/rfc7049
 - Requirements: cbor2, https://pypi.python.org/pypi/cbor2
@@ -22,32 +21,31 @@
 
 .. versionchanged:: 0.0.3
 
    - fix: follow internal API changes of the argument for load/dump functions
 
 .. versionadded:: 0.0.2
 """
-from __future__ import absolute_import
-
 import cbor2
+
 import anyconfig.backend.base
-from anyconfig.backend.base import to_method
 
 
 class Parser(anyconfig.backend.base.StringStreamFnParser,
-             anyconfig.backend.base.BinaryFilesMixin):
+             anyconfig.backend.base.BinaryLoaderMixin,
+             anyconfig.backend.base.BinaryDumperMixin):
     """Parser for CBOR files.
     """
     _type = "cbor"
     _cid = "cbor2"
     _priority = 10  # Gives higher precedence than cbor.
     _extensions = ["cbor"]
     _loads_opts = ["tag_hook", "object_hook"]
     _dump_opts = ["datetime_as_timestamp", "timezone", "value_sharing",
                   "default"]
 
-    _load_from_string_fn = to_method(cbor2.loads)
-    _load_from_stream_fn = to_method(cbor2.load)
-    _dump_to_string_fn = to_method(cbor2.dumps)
-    _dump_to_stream_fn = to_method(cbor2.dump)
+    _load_from_string_fn = anyconfig.backend.base.to_method(cbor2.loads)
+    _load_from_stream_fn = anyconfig.backend.base.to_method(cbor2.load)
+    _dump_to_string_fn = anyconfig.backend.base.to_method(cbor2.dumps)
+    _dump_to_stream_fn = anyconfig.backend.base.to_method(cbor2.dump)
 
 # vim:sw=4:ts=4:et:
```

### Comparing `anyconfig-cbor2-backend-0.1.2/src/anyconfig_cbor2_backend.egg-info/PKG-INFO` & `anyconfig-cbor2-backend-0.2.0/src/anyconfig_cbor2_backend.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: anyconfig-cbor2-backend
-Version: 0.1.2
+Version: 0.2.0
 Summary: Backend module for python-anyconfig to load and dump CBOR data
 Home-page: https://github.com/ssato/python-anyconfig-cbor2-backend
 Author: Satoru SATOH
 Author-email: satoru.satoh@gmail.com
 Maintainer: Satoru SATOH
 Maintainer-email: satoru.satoh@gmail.com
 License: MIT
-Project-URL: CI: Travis, https://travis-ci.org/ssato/python-anyconfig-cbor2-backend
+Project-URL: CI: Github Actions, https://github.com/ssato/python-anyconfig-cbor2-backend/actions
 Project-URL: Download, https://pypi.python.org/pypi/anyconfig-cbor2-backend
 Project-URL: Download RPMs, https://copr.fedoraproject.org/coprs/ssato/python-anyconfig/
 Project-URL: Bug Tracker, https://github.com/ssato/python-anyconfig-cbor2-backend/issues
 Project-URL: Source, https://github.com/ssato/python-anyconfig-cbor2-backend
-Description: 
-        This is a backend parser module for python-anyconfig to support to load and
-        dump CBOR files using cbor2, https://pypi.python.org/pypi/cbor2.
-        
-        SEE ALSO:
-        
-        - python-anyconfig: https://github.com/ssato/python-anyconfig
-        - CBOR spec: http://cbor.io
 Platform: any
 Classifier: Development Status :: 3 - Alpha
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
-Classifier: Topic :: Text Processing :: Markup
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
+License-File: LICENSE.MIT
+
+
+This is a backend parser module for python-anyconfig to support to load and
+dump CBOR files using cbor2, https://pypi.python.org/pypi/cbor2.
+
+SEE ALSO:
+
+- python-anyconfig: https://github.com/ssato/python-anyconfig
+- CBOR spec: http://cbor.io
```

### Comparing `anyconfig-cbor2-backend-0.1.2/src/anyconfig_cbor2_backend.egg-info/SOURCES.txt` & `anyconfig-cbor2-backend-0.2.0/src/anyconfig_cbor2_backend.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 .travis.yml
 LICENSE.MIT
 MANIFEST.in
 NEWS
 README.rst
+mypy.ini
 requirements.txt
 setup.cfg
 setup.py
 tox.ini
+.github/workflows/release.yml
+.github/workflows/tests.yml
 extras/cbor2-hardcode-version.patch
 pkg/copr-build.sh
 pkg/nose.cfg
 pkg/package.spec.in
 src/anyconfig_cbor2_backend/__init__.py
 src/anyconfig_cbor2_backend/cbor2_.py
 src/anyconfig_cbor2_backend.egg-info/PKG-INFO
 src/anyconfig_cbor2_backend.egg-info/SOURCES.txt
 src/anyconfig_cbor2_backend.egg-info/dependency_links.txt
 src/anyconfig_cbor2_backend.egg-info/entry_points.txt
 src/anyconfig_cbor2_backend.egg-info/requires.txt
 src/anyconfig_cbor2_backend.egg-info/top_level.txt
 tests/__init__.py
-tests/cbor2_.py
 tests/common.py
-tests/plugin.py
-tests/releng.bats
 tests/requirements.txt
+tests/test_cbor2.py
+tests/test_plugin.py
 tests/res/0.cbor
```

### Comparing `anyconfig-cbor2-backend-0.1.2/tests/cbor2_.py` & `anyconfig-cbor2-backend-0.2.0/tests/test_cbor2.py`

 * *Files identical despite different names*

### Comparing `anyconfig-cbor2-backend-0.1.2/tests/common.py` & `anyconfig-cbor2-backend-0.2.0/tests/common.py`

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

### Comparing `anyconfig-cbor2-backend-0.1.2/tests/plugin.py` & `anyconfig-cbor2-backend-0.2.0/tests/test_plugin.py`

 * *Files identical despite different names*

