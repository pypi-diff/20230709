# Comparing `tmp/anyconfig-bson-backend-0.1.2.tar.gz` & `tmp/anyconfig-bson-backend-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/anyconfig-bson-backend-0.1.2.tar", last modified: Thu Apr 30 14:04:44 2020, max compression
+gzip compressed data, was "anyconfig-bson-backend-0.2.0.tar", last modified: Sun Jul  9 15:49:48 2023, max compression
```

## Comparing `anyconfig-bson-backend-0.1.2.tar` & `anyconfig-bson-backend-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,36 @@
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 14:04:44.000000 anyconfig-bson-backend-0.1.2/
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      470 2020-04-29 11:46:21.000000 anyconfig-bson-backend-0.1.2/.travis.yml
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1069 2018-01-14 05:09:46.000000 anyconfig-bson-backend-0.1.2/LICENSE.MIT
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      206 2020-04-30 01:40:50.000000 anyconfig-bson-backend-0.1.2/MANIFEST.in
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1908 2020-04-30 14:04:44.000000 anyconfig-bson-backend-0.1.2/PKG-INFO
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     2189 2020-04-30 13:58:29.000000 anyconfig-bson-backend-0.1.2/README.rst
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 14:04:44.000000 anyconfig-bson-backend-0.1.2/pkg/
--rwxrwxr-x   0 ssato     (1000) ssato     (1000)      494 2018-01-01 13:54:49.000000 anyconfig-bson-backend-0.1.2/pkg/copr-build.sh
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       56 2018-01-14 05:37:19.000000 anyconfig-bson-backend-0.1.2/pkg/entry_points.txt
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      106 2018-01-14 05:28:23.000000 anyconfig-bson-backend-0.1.2/pkg/nose.cfg
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     2170 2020-04-30 14:00:29.000000 anyconfig-bson-backend-0.1.2/pkg/package.spec.in
--rwxrwxr-x   0 ssato     (1000) ssato     (1000)     1957 2015-05-31 14:02:48.000000 anyconfig-bson-backend-0.1.2/pkg/rpmbuild-wrapper.sh
--rwxrwxr-x   0 ssato     (1000) ssato     (1000)      575 2018-01-11 10:20:02.000000 anyconfig-bson-backend-0.1.2/pkg/run-backend-tests.sh
--rwxrwxr-x   0 ssato     (1000) ssato     (1000)     1853 2018-01-07 13:43:59.000000 anyconfig-bson-backend-0.1.2/pkg/runtest.sh
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       18 2019-09-23 07:13:37.000000 anyconfig-bson-backend-0.1.2/requirements.txt
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1955 2020-04-30 14:04:44.000000 anyconfig-bson-backend-0.1.2/setup.cfg
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1493 2020-04-30 00:55:53.000000 anyconfig-bson-backend-0.1.2/setup.py
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 14:04:44.000000 anyconfig-bson-backend-0.1.2/src/
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 14:04:44.000000 anyconfig-bson-backend-0.1.2/src/anyconfig_bson_backend/
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      162 2020-04-30 00:52:29.000000 anyconfig-bson-backend-0.1.2/src/anyconfig_bson_backend/__init__.py
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     4415 2020-04-29 16:45:21.000000 anyconfig-bson-backend-0.1.2/src/anyconfig_bson_backend/bson_.py
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 14:04:44.000000 anyconfig-bson-backend-0.1.2/src/anyconfig_bson_backend.egg-info/
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1908 2020-04-30 14:04:44.000000 anyconfig-bson-backend-0.1.2/src/anyconfig_bson_backend.egg-info/PKG-INFO
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      726 2020-04-30 14:04:44.000000 anyconfig-bson-backend-0.1.2/src/anyconfig_bson_backend.egg-info/SOURCES.txt
--rw-rw-r--   0 ssato     (1000) ssato     (1000)        1 2020-04-30 14:04:44.000000 anyconfig-bson-backend-0.1.2/src/anyconfig_bson_backend.egg-info/dependency_links.txt
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       59 2020-04-30 14:04:44.000000 anyconfig-bson-backend-0.1.2/src/anyconfig_bson_backend.egg-info/entry_points.txt
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       18 2020-04-30 14:04:44.000000 anyconfig-bson-backend-0.1.2/src/anyconfig_bson_backend.egg-info/requires.txt
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       23 2020-04-30 14:04:44.000000 anyconfig-bson-backend-0.1.2/src/anyconfig_bson_backend.egg-info/top_level.txt
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 14:04:44.000000 anyconfig-bson-backend-0.1.2/tests/
--rw-rw-r--   0 ssato     (1000) ssato     (1000)        0 2015-05-31 04:08:11.000000 anyconfig-bson-backend-0.1.2/tests/__init__.py
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      750 2020-04-29 16:46:26.000000 anyconfig-bson-backend-0.1.2/tests/bson_.py
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     8891 2019-09-23 06:54:50.000000 anyconfig-bson-backend-0.1.2/tests/common.py
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1114 2020-04-30 01:39:59.000000 anyconfig-bson-backend-0.1.2/tests/plugin.py
--rwxrwxr-x   0 ssato     (1000) ssato     (1000)     1760 2020-04-30 01:31:00.000000 anyconfig-bson-backend-0.1.2/tests/releng.bats
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       46 2020-04-29 11:47:34.000000 anyconfig-bson-backend-0.1.2/tests/requirements.txt
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 14:04:44.000000 anyconfig-bson-backend-0.1.2/tests/res/
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       77 2018-01-14 05:33:56.000000 anyconfig-bson-backend-0.1.2/tests/res/0.bson
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      972 2020-04-30 13:08:34.000000 anyconfig-bson-backend-0.1.2/tox.ini
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 15:49:48.822525 anyconfig-bson-backend-0.2.0/
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)     1069 2018-01-14 05:09:46.000000 anyconfig-bson-backend-0.2.0/LICENSE.MIT
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      219 2023-07-09 15:49:08.000000 anyconfig-bson-backend-0.2.0/MANIFEST.in
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     1801 2023-07-09 15:49:48.822525 anyconfig-bson-backend-0.2.0/PKG-INFO
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     2246 2023-07-09 15:49:08.000000 anyconfig-bson-backend-0.2.0/README.rst
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 15:49:48.821525 anyconfig-bson-backend-0.2.0/pkg/
+-rwxrwxr-x   0 ssato     (1000) ssato     (1000)      494 2018-01-01 13:54:49.000000 anyconfig-bson-backend-0.2.0/pkg/copr-build.sh
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)       56 2018-01-14 05:37:19.000000 anyconfig-bson-backend-0.2.0/pkg/entry_points.txt
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)      106 2018-01-14 05:28:23.000000 anyconfig-bson-backend-0.2.0/pkg/nose.cfg
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)     2170 2020-04-30 14:00:29.000000 anyconfig-bson-backend-0.2.0/pkg/package.spec.in
+-rwxrwxr-x   0 ssato     (1000) ssato     (1000)     1957 2015-05-31 14:02:48.000000 anyconfig-bson-backend-0.2.0/pkg/rpmbuild-wrapper.sh
+-rwxrwxr-x   0 ssato     (1000) ssato     (1000)      575 2018-01-11 10:20:02.000000 anyconfig-bson-backend-0.2.0/pkg/run-backend-tests.sh
+-rwxrwxr-x   0 ssato     (1000) ssato     (1000)     1853 2018-01-07 13:43:59.000000 anyconfig-bson-backend-0.2.0/pkg/runtest.sh
+-rw-r--r--   0 ssato     (1000) ssato     (1000)       92 2023-07-09 15:49:08.000000 anyconfig-bson-backend-0.2.0/requirements.txt
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     1933 2023-07-09 15:49:48.823525 anyconfig-bson-backend-0.2.0/setup.cfg
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)     1501 2020-04-30 16:04:13.000000 anyconfig-bson-backend-0.2.0/setup.py
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 15:49:48.820525 anyconfig-bson-backend-0.2.0/src/
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 15:49:48.821525 anyconfig-bson-backend-0.2.0/src/anyconfig_bson_backend/
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      162 2023-07-09 15:49:08.000000 anyconfig-bson-backend-0.2.0/src/anyconfig_bson_backend/__init__.py
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     4431 2023-07-09 15:49:08.000000 anyconfig-bson-backend-0.2.0/src/anyconfig_bson_backend/bson_.py
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 15:49:48.822525 anyconfig-bson-backend-0.2.0/src/anyconfig_bson_backend.egg-info/
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)     1801 2023-07-09 15:49:48.000000 anyconfig-bson-backend-0.2.0/src/anyconfig_bson_backend.egg-info/PKG-INFO
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)      705 2023-07-09 15:49:48.000000 anyconfig-bson-backend-0.2.0/src/anyconfig_bson_backend.egg-info/SOURCES.txt
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)        1 2023-07-09 15:49:48.000000 anyconfig-bson-backend-0.2.0/src/anyconfig_bson_backend.egg-info/dependency_links.txt
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)       58 2023-07-09 15:49:48.000000 anyconfig-bson-backend-0.2.0/src/anyconfig_bson_backend.egg-info/entry_points.txt
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)       18 2023-07-09 15:49:48.000000 anyconfig-bson-backend-0.2.0/src/anyconfig_bson_backend.egg-info/requires.txt
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)       23 2023-07-09 15:49:48.000000 anyconfig-bson-backend-0.2.0/src/anyconfig_bson_backend.egg-info/top_level.txt
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 15:49:48.822525 anyconfig-bson-backend-0.2.0/tests/
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)        0 2015-05-31 04:08:11.000000 anyconfig-bson-backend-0.2.0/tests/__init__.py
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     8780 2023-07-09 15:49:08.000000 anyconfig-bson-backend-0.2.0/tests/common.py
+-rw-r--r--   0 ssato     (1000) ssato     (1000)       75 2023-07-09 15:49:08.000000 anyconfig-bson-backend-0.2.0/tests/requirements.txt
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 15:49:48.822525 anyconfig-bson-backend-0.2.0/tests/res/
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)       77 2018-01-14 05:33:56.000000 anyconfig-bson-backend-0.2.0/tests/res/0.bson
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      750 2023-07-09 15:49:08.000000 anyconfig-bson-backend-0.2.0/tests/test_bson.py
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     1088 2023-07-09 15:49:08.000000 anyconfig-bson-backend-0.2.0/tests/test_plugin.py
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      829 2023-07-09 15:49:08.000000 anyconfig-bson-backend-0.2.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `anyconfig-bson-backend-0.1.2/LICENSE.MIT` & `anyconfig-bson-backend-0.2.0/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `anyconfig-bson-backend-0.1.2/PKG-INFO` & `anyconfig-bson-backend-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,43 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: anyconfig-bson-backend
-Version: 0.1.2
+Version: 0.2.0
 Summary: Backend module for python-anyconfig to load and dump CBOR data
 Home-page: https://github.com/ssato/python-anyconfig-bson-backend
 Author: Satoru SATOH
 Author-email: satoru.satoh@gmail.com
 Maintainer: Satoru SATOH
 Maintainer-email: satoru.satoh@gmail.com
 License: MIT
-Project-URL: CI: Travis, https://travis-ci.org/ssato/python-anyconfig-bson-backend
+Project-URL: CI: Github Actions, https://github.com/ssato/python-anyconfig-bson-backend/actions
 Project-URL: Download, https://pypi.python.org/pypi/anyconfig-bson-backend
 Project-URL: Download RPMs, https://copr.fedoraproject.org/coprs/ssato/python-anyconfig/
 Project-URL: Bug Tracker, https://github.com/ssato/python-anyconfig-bson-backend/issues
 Project-URL: Source, https://github.com/ssato/python-anyconfig-bson-backend
-Description: 
-        This is a parser backend module for python-anyconfig to load and dump BSON
-        files using pymongo.
-        
-        NOTE: bson from pymongo package may work with this package but bson
-        (https://pypi.python.org/pypi/bson/) does not.
-        
-        SEE ALSO:
-        
-        - python-anyconfig: https://github.com/ssato/python-anyconfig
-        - pymongo: https://pypi.org/project/pymongo/
-        - BSON spec: http://bsonspec.org
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
 Classifier: Topic :: Text Processing :: Markup
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
+License-File: LICENSE.MIT
+
+
+This is a parser backend module for python-anyconfig to load and dump BSON
+files using pymongo.
+
+NOTE: bson from pymongo package may work with this package but bson
+(https://pypi.python.org/pypi/bson/) does not.
+
+SEE ALSO:
+
+- python-anyconfig: https://github.com/ssato/python-anyconfig
+- pymongo: https://pypi.org/project/pymongo/
+- BSON spec: http://bsonspec.org
```

### Comparing `anyconfig-bson-backend-0.1.2/README.rst` & `anyconfig-bson-backend-0.2.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 python-anyconfig-bson-backend
 ================================
 
 .. image:: https://img.shields.io/pypi/v/anyconfig-bson-backend.svg
    :target: https://pypi.python.org/pypi/anyconfig-bson-backend/
    :alt: [Latest Versbson]
 
-.. image:: https://img.shields.io/travis/ssato/python-anyconfig-bson-backend.svg
-   :target: https://travis-ci.org/ssato/python-anyconfig-bson-backend
-   :alt: Test status
+.. image:: https://github.com/ssato/python-anyconfig-bson-backend/workflows/Tests/badge.svg
+   :target: https://github.com/ssato/python-anyconfig-bson-backend/actions?query=workflow%3ATests
+   :alt: [Github Actions: Test status]
 
 .. image:: https://img.shields.io/coveralls/ssato/python-anyconfig-bson-backend.svg
    :target: https://coveralls.io/r/ssato/python-anyconfig-bson-backend
    :alt: Coverage Status
 
 .. image:: https://scrutinizer-ci.com/g/ssato/python-anyconfig-bson-backend/badges/quality-score.png
    :target: https://scrutinizer-ci.com/g/ssato/python-anyconfig-bson-backend
```

### Comparing `anyconfig-bson-backend-0.1.2/pkg/package.spec.in` & `anyconfig-bson-backend-0.2.0/pkg/package.spec.in`

 * *Files identical despite different names*

### Comparing `anyconfig-bson-backend-0.1.2/pkg/rpmbuild-wrapper.sh` & `anyconfig-bson-backend-0.2.0/pkg/rpmbuild-wrapper.sh`

 * *Files identical despite different names*

### Comparing `anyconfig-bson-backend-0.1.2/pkg/run-backend-tests.sh` & `anyconfig-bson-backend-0.2.0/pkg/run-backend-tests.sh`

 * *Files identical despite different names*

### Comparing `anyconfig-bson-backend-0.1.2/pkg/runtest.sh` & `anyconfig-bson-backend-0.2.0/pkg/runtest.sh`

 * *Files identical despite different names*

### Comparing `anyconfig-bson-backend-0.1.2/setup.cfg` & `anyconfig-bson-backend-0.2.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = anyconfig-bson-backend
 description = Backend module for python-anyconfig to load and dump CBOR data
 project_urls = 
-	CI: Travis = https://travis-ci.org/ssato/python-anyconfig-bson-backend
+	CI: Github Actions = https://github.com/ssato/python-anyconfig-bson-backend/actions
 	Download = https://pypi.python.org/pypi/anyconfig-bson-backend
 	Download RPMs = https://copr.fedoraproject.org/coprs/ssato/python-anyconfig/
 	Bug Tracker = https://github.com/ssato/python-anyconfig-bson-backend/issues
 	Source = https://github.com/ssato/python-anyconfig-bson-backend
 long_description = 
 	This is a parser backend module for python-anyconfig to load and dump BSON
 	files using pymongo.
@@ -30,20 +30,19 @@
 url = https://github.com/ssato/python-anyconfig-bson-backend
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
 	Topic :: Text Processing :: Markup
 	Topic :: Utilities
 	License :: OSI Approved :: MIT License
 
 [options]
```

### Comparing `anyconfig-bson-backend-0.1.2/setup.py` & `anyconfig-bson-backend-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     if matches:
         VERSION = matches[0][0]
         break
 
 assert VERSION
 
 # For daily snapshot versioning mode:
-RELEASE = "1"
+RELEASE = "1%{?dist}"
 if os.environ.get("_SNAPSHOT_BUILD", None) is not None:
     import datetime
     RELEASE = datetime.datetime.now().strftime("%Y%m%d%H%M%S")
 
 
 def _replace(line):
     """Replace some strings in the RPM SPEC template"""
```

### Comparing `anyconfig-bson-backend-0.1.2/src/anyconfig_bson_backend/bson_.py` & `anyconfig-bson-backend-0.2.0/src/anyconfig_bson_backend/bson_.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2015 - 2020 Satoru SATOH <satoru.satoh @ gmail.com>
+# Copyright (C) 2015 - 2021 Satoru SATOH <satoru.satoh @ gmail.com>
 # License: MIT
 #
 # Ref. python -c "import bson; help(bson)"
 #
 r"""BSON backend:
 
 - Format to support: BSON, http://bsonspec.org
@@ -38,16 +38,14 @@
 
    - _load_opts() was removed because C extension looks forced to be enalbed if
      bson.has_c() == True, that is, C extension was built, installed and used.
      see also: https://jira.mongodb.org/browse/PYTHON-379
 
     .. versionadded:: anyconfig-0.1.0
 """
-from __future__ import absolute_import
-
 import bson
 import anyconfig.backend.base
 import anyconfig.utils
 
 
 _CO_OPTIONS = ("document_class", "tz_aware", "uuid_representation",
                "unicode_decode_error_handler", "tzinfo")
@@ -60,15 +58,16 @@
     :return: :class:`~bson.CodecOptions`
     """
     opts = anyconfig.utils.filter_options(_CO_OPTIONS, options)
     return bson.CodecOptions(**opts)
 
 
 class Parser(anyconfig.backend.base.StringParser,
-             anyconfig.backend.base.BinaryFilesMixin):
+             anyconfig.backend.base.BinaryLoaderMixin,
+             anyconfig.backend.base.BinaryDumperMixin):
     """
     Loader/Dumper of BSON files.
     """
     _cid = "bson"
     _type = "bson"
     _extensions = ["bson", "bsn"]  # Temporary.
     _load_opts = [] if bson.has_c() else ["codec_options"]
```

### Comparing `anyconfig-bson-backend-0.1.2/src/anyconfig_bson_backend.egg-info/PKG-INFO` & `anyconfig-bson-backend-0.2.0/src/anyconfig_bson_backend.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,43 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: anyconfig-bson-backend
-Version: 0.1.2
+Version: 0.2.0
 Summary: Backend module for python-anyconfig to load and dump CBOR data
 Home-page: https://github.com/ssato/python-anyconfig-bson-backend
 Author: Satoru SATOH
 Author-email: satoru.satoh@gmail.com
 Maintainer: Satoru SATOH
 Maintainer-email: satoru.satoh@gmail.com
 License: MIT
-Project-URL: CI: Travis, https://travis-ci.org/ssato/python-anyconfig-bson-backend
+Project-URL: CI: Github Actions, https://github.com/ssato/python-anyconfig-bson-backend/actions
 Project-URL: Download, https://pypi.python.org/pypi/anyconfig-bson-backend
 Project-URL: Download RPMs, https://copr.fedoraproject.org/coprs/ssato/python-anyconfig/
 Project-URL: Bug Tracker, https://github.com/ssato/python-anyconfig-bson-backend/issues
 Project-URL: Source, https://github.com/ssato/python-anyconfig-bson-backend
-Description: 
-        This is a parser backend module for python-anyconfig to load and dump BSON
-        files using pymongo.
-        
-        NOTE: bson from pymongo package may work with this package but bson
-        (https://pypi.python.org/pypi/bson/) does not.
-        
-        SEE ALSO:
-        
-        - python-anyconfig: https://github.com/ssato/python-anyconfig
-        - pymongo: https://pypi.org/project/pymongo/
-        - BSON spec: http://bsonspec.org
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
 Classifier: Topic :: Text Processing :: Markup
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
+License-File: LICENSE.MIT
+
+
+This is a parser backend module for python-anyconfig to load and dump BSON
+files using pymongo.
+
+NOTE: bson from pymongo package may work with this package but bson
+(https://pypi.python.org/pypi/bson/) does not.
+
+SEE ALSO:
+
+- python-anyconfig: https://github.com/ssato/python-anyconfig
+- pymongo: https://pypi.org/project/pymongo/
+- BSON spec: http://bsonspec.org
```

### Comparing `anyconfig-bson-backend-0.1.2/src/anyconfig_bson_backend.egg-info/SOURCES.txt` & `anyconfig-bson-backend-0.2.0/src/anyconfig_bson_backend.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.travis.yml
 LICENSE.MIT
 MANIFEST.in
 README.rst
 requirements.txt
 setup.cfg
 setup.py
 tox.ini
@@ -18,13 +17,12 @@
 src/anyconfig_bson_backend.egg-info/PKG-INFO
 src/anyconfig_bson_backend.egg-info/SOURCES.txt
 src/anyconfig_bson_backend.egg-info/dependency_links.txt
 src/anyconfig_bson_backend.egg-info/entry_points.txt
 src/anyconfig_bson_backend.egg-info/requires.txt
 src/anyconfig_bson_backend.egg-info/top_level.txt
 tests/__init__.py
-tests/bson_.py
 tests/common.py
-tests/plugin.py
-tests/releng.bats
 tests/requirements.txt
+tests/test_bson.py
+tests/test_plugin.py
 tests/res/0.bson
```

### Comparing `anyconfig-bson-backend-0.1.2/tests/bson_.py` & `anyconfig-bson-backend-0.2.0/tests/test_bson.py`

 * *Files identical despite different names*

### Comparing `anyconfig-bson-backend-0.1.2/tests/common.py` & `anyconfig-bson-backend-0.2.0/tests/common.py`

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

### Comparing `anyconfig-bson-backend-0.1.2/tests/plugin.py` & `anyconfig-bson-backend-0.2.0/tests/test_plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 import os.path
 import os
 import pkg_resources
 import unittest
 
 import anyconfig
-import anyconfig.backends
 
 from tests.common import dicts_equal
 
 
 _CURDIR = os.path.dirname(__file__)
 _CNF_0 = {u'a': 0,
           u'b': u'bbb',
```

