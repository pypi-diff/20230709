# Comparing `tmp/anyconfig-ion-backend-0.1.1.tar.gz` & `tmp/anyconfig-ion-backend-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/anyconfig-ion-backend-0.1.1.tar", last modified: Thu Apr 30 17:48:10 2020, max compression
+gzip compressed data, was "anyconfig-ion-backend-0.2.0.tar", last modified: Sun Jul  9 06:40:32 2023, max compression
```

## Comparing `anyconfig-ion-backend-0.1.1.tar` & `anyconfig-ion-backend-0.2.0.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 17:48:10.000000 anyconfig-ion-backend-0.1.1/
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      470 2020-04-30 17:20:28.000000 anyconfig-ion-backend-0.1.1/.travis.yml
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1069 2018-01-05 16:33:29.000000 anyconfig-ion-backend-0.1.1/LICENSE.MIT
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      219 2020-04-30 17:20:28.000000 anyconfig-ion-backend-0.1.1/MANIFEST.in
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1812 2020-04-30 17:48:10.000000 anyconfig-ion-backend-0.1.1/PKG-INFO
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1791 2020-04-30 17:45:31.000000 anyconfig-ion-backend-0.1.1/README.rst
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 17:48:10.000000 anyconfig-ion-backend-0.1.1/pkg/
--rwxrwxr-x   0 ssato     (1000) ssato     (1000)      494 2018-01-01 13:54:49.000000 anyconfig-ion-backend-0.1.1/pkg/copr-build.sh
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      105 2018-01-08 16:42:40.000000 anyconfig-ion-backend-0.1.1/pkg/nose.cfg
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     2109 2020-04-30 17:46:57.000000 anyconfig-ion-backend-0.1.1/pkg/package.spec.in
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       21 2018-01-08 16:42:50.000000 anyconfig-ion-backend-0.1.1/requirements.txt
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1867 2020-04-30 17:48:10.000000 anyconfig-ion-backend-0.1.1/setup.cfg
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1501 2020-04-30 17:20:28.000000 anyconfig-ion-backend-0.1.1/setup.py
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 17:48:10.000000 anyconfig-ion-backend-0.1.1/src/
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 17:48:10.000000 anyconfig-ion-backend-0.1.1/src/anyconfig_ion_backend/
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      199 2020-04-30 17:46:28.000000 anyconfig-ion-backend-0.1.1/src/anyconfig_ion_backend/__init__.py
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     2499 2018-01-09 02:07:48.000000 anyconfig-ion-backend-0.1.1/src/anyconfig_ion_backend/ion_.py
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 17:48:10.000000 anyconfig-ion-backend-0.1.1/src/anyconfig_ion_backend.egg-info/
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1812 2020-04-30 17:48:10.000000 anyconfig-ion-backend-0.1.1/src/anyconfig_ion_backend.egg-info/PKG-INFO
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      660 2020-04-30 17:48:10.000000 anyconfig-ion-backend-0.1.1/src/anyconfig_ion_backend.egg-info/SOURCES.txt
--rw-rw-r--   0 ssato     (1000) ssato     (1000)        1 2020-04-30 17:48:10.000000 anyconfig-ion-backend-0.1.1/src/anyconfig_ion_backend.egg-info/dependency_links.txt
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       57 2020-04-30 17:48:10.000000 anyconfig-ion-backend-0.1.1/src/anyconfig_ion_backend.egg-info/entry_points.txt
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       21 2020-04-30 17:48:10.000000 anyconfig-ion-backend-0.1.1/src/anyconfig_ion_backend.egg-info/requires.txt
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       22 2020-04-30 17:48:10.000000 anyconfig-ion-backend-0.1.1/src/anyconfig_ion_backend.egg-info/top_level.txt
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 17:48:10.000000 anyconfig-ion-backend-0.1.1/tests/
--rw-rw-r--   0 ssato     (1000) ssato     (1000)        0 2015-05-31 04:08:11.000000 anyconfig-ion-backend-0.1.1/tests/__init__.py
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     8891 2019-09-23 23:38:47.000000 anyconfig-ion-backend-0.1.1/tests/common.py
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      728 2020-04-30 17:22:26.000000 anyconfig-ion-backend-0.1.1/tests/ion_.py
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1008 2020-04-30 17:21:28.000000 anyconfig-ion-backend-0.1.1/tests/plugin.py
--rwxrwxr-x   0 ssato     (1000) ssato     (1000)     1545 2019-09-23 23:38:52.000000 anyconfig-ion-backend-0.1.1/tests/releng.bats
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       41 2020-04-30 00:26:25.000000 anyconfig-ion-backend-0.1.1/tests/requirements.txt
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 17:48:10.000000 anyconfig-ion-backend-0.1.1/tests/res/
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       50 2018-01-08 17:09:11.000000 anyconfig-ion-backend-0.1.1/tests/res/ion.bin_data
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       60 2018-01-08 17:17:17.000000 anyconfig-ion-backend-0.1.1/tests/res/ion.txt_data
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      972 2020-04-30 17:20:28.000000 anyconfig-ion-backend-0.1.1/tox.ini
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 06:40:32.235907 anyconfig-ion-backend-0.2.0/
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 06:40:32.232907 anyconfig-ion-backend-0.2.0/.github/
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 06:40:32.233907 anyconfig-ion-backend-0.2.0/.github/workflows/
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      858 2023-07-09 06:30:13.000000 anyconfig-ion-backend-0.2.0/.github/workflows/tests.yml
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)     1069 2018-01-05 16:33:29.000000 anyconfig-ion-backend-0.2.0/LICENSE.MIT
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)      218 2021-05-18 06:45:43.000000 anyconfig-ion-backend-0.2.0/MANIFEST.in
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     1713 2023-07-09 06:40:32.235907 anyconfig-ion-backend-0.2.0/PKG-INFO
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)     1649 2023-07-09 06:35:03.000000 anyconfig-ion-backend-0.2.0/README.rst
+-rw-r--r--   0 ssato     (1000) ssato     (1000)       66 2021-05-18 06:44:53.000000 anyconfig-ion-backend-0.2.0/mypy.ini
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 06:40:32.233907 anyconfig-ion-backend-0.2.0/pkg/
+-rwxrwxr-x   0 ssato     (1000) ssato     (1000)      494 2018-01-01 13:54:49.000000 anyconfig-ion-backend-0.2.0/pkg/copr-build.sh
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)      105 2018-01-08 16:42:40.000000 anyconfig-ion-backend-0.2.0/pkg/nose.cfg
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)     2109 2020-04-30 17:46:57.000000 anyconfig-ion-backend-0.2.0/pkg/package.spec.in
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)       95 2021-05-18 06:48:10.000000 anyconfig-ion-backend-0.2.0/requirements.txt
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)     1845 2023-07-09 06:40:32.235907 anyconfig-ion-backend-0.2.0/setup.cfg
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)     1501 2020-04-30 17:20:28.000000 anyconfig-ion-backend-0.2.0/setup.py
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 06:40:32.232907 anyconfig-ion-backend-0.2.0/src/
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 06:40:32.234907 anyconfig-ion-backend-0.2.0/src/anyconfig_ion_backend/
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)      199 2023-07-09 06:38:23.000000 anyconfig-ion-backend-0.2.0/src/anyconfig_ion_backend/__init__.py
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)     2417 2021-05-18 06:52:23.000000 anyconfig-ion-backend-0.2.0/src/anyconfig_ion_backend/ion_.py
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 06:40:32.234907 anyconfig-ion-backend-0.2.0/src/anyconfig_ion_backend.egg-info/
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)     1713 2023-07-09 06:40:32.000000 anyconfig-ion-backend-0.2.0/src/anyconfig_ion_backend.egg-info/PKG-INFO
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)      677 2023-07-09 06:40:32.000000 anyconfig-ion-backend-0.2.0/src/anyconfig_ion_backend.egg-info/SOURCES.txt
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)        1 2023-07-09 06:40:32.000000 anyconfig-ion-backend-0.2.0/src/anyconfig_ion_backend.egg-info/dependency_links.txt
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)       56 2023-07-09 06:40:32.000000 anyconfig-ion-backend-0.2.0/src/anyconfig_ion_backend.egg-info/entry_points.txt
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)       21 2023-07-09 06:40:32.000000 anyconfig-ion-backend-0.2.0/src/anyconfig_ion_backend.egg-info/requires.txt
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)       22 2023-07-09 06:40:32.000000 anyconfig-ion-backend-0.2.0/src/anyconfig_ion_backend.egg-info/top_level.txt
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 06:40:32.234907 anyconfig-ion-backend-0.2.0/tests/
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)        0 2015-05-31 04:08:11.000000 anyconfig-ion-backend-0.2.0/tests/__init__.py
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)     8780 2021-05-18 06:46:18.000000 anyconfig-ion-backend-0.2.0/tests/common.py
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)       70 2023-07-09 06:24:08.000000 anyconfig-ion-backend-0.2.0/tests/requirements.txt
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 06:40:32.235907 anyconfig-ion-backend-0.2.0/tests/res/
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)       50 2018-01-08 17:09:11.000000 anyconfig-ion-backend-0.2.0/tests/res/ion.bin_data
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)       60 2018-01-08 17:17:17.000000 anyconfig-ion-backend-0.2.0/tests/res/ion.txt_data
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)      728 2020-04-30 17:22:26.000000 anyconfig-ion-backend-0.2.0/tests/test_ion_.py
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)     1008 2020-04-30 17:21:28.000000 anyconfig-ion-backend-0.2.0/tests/test_plugin.py
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)      829 2023-07-09 06:33:01.000000 anyconfig-ion-backend-0.2.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `anyconfig-ion-backend-0.1.1/LICENSE.MIT` & `anyconfig-ion-backend-0.2.0/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `anyconfig-ion-backend-0.1.1/PKG-INFO` & `anyconfig-ion-backend-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,42 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: anyconfig-ion-backend
-Version: 0.1.1
+Version: 0.2.0
 Summary: Backend module for python-anyconfig to load and dump CBOR data
 Home-page: https://github.com/ssato/python-anyconfig-ion-backend
 Author: Satoru SATOH
 Author-email: satoru.satoh@gmail.com
 Maintainer: Satoru SATOH
 Maintainer-email: satoru.satoh@gmail.com
 License: MIT
-Project-URL: CI: Travis, https://travis-ci.org/ssato/python-anyconfig-ion-backend
+Project-URL: CI: Github Actions, https://github.com/ssato/python-anyconfig-ion-backend/actions
 Project-URL: Download, https://pypi.python.org/pypi/anyconfig-ion-backend
 Project-URL: Download RPMs, https://copr.fedoraproject.org/coprs/ssato/python-anyconfig/
 Project-URL: Bug Tracker, https://github.com/ssato/python-anyconfig-ion-backend/issues
 Project-URL: Source, https://github.com/ssato/python-anyconfig-ion-backend
-Description: 
-        This is a backend module for python-anyconfig to support to load and dump
-        Amazon Ion data files.
-        
-        - Author: Satoru SATOH <satoru.satoh@gmail.com>
-        - License: MIT
-        
-        SEE ALSO:
-        
-        - python-anyconfig: https://github.com/ssato/python-anyconfig
-        - Amazon Ion: https://amzn.github.io/ion-docs/
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
+This is a backend module for python-anyconfig to support to load and dump
+Amazon Ion data files.
+
+- Author: Satoru SATOH <satoru.satoh@gmail.com>
+- License: MIT
+
+SEE ALSO:
+
+- python-anyconfig: https://github.com/ssato/python-anyconfig
+- Amazon Ion: https://amzn.github.io/ion-docs/
```

### Comparing `anyconfig-ion-backend-0.1.1/README.rst` & `anyconfig-ion-backend-0.2.0/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -2,26 +2,22 @@
 python-anyconfig-ion-backend
 ================================
 
 .. image:: https://img.shields.io/pypi/v/anyconfig-ion-backend.svg
    :target: https://pypi.python.org/pypi/anyconfig-ion-backend/
    :alt: [Latest Version]
 
-.. image:: https://img.shields.io/travis/ssato/python-anyconfig-ion-backend.svg
-   :target: https://travis-ci.org/ssato/python-anyconfig-ion-backend
-   :alt: Test status
+.. image:: https://github.com/ssato/python-anyconfig-ion-backend/workflows/Tests/badge.svg
+   :target: https://github.com/ssato/python-anyconfig-ion-backend/actions?query=workflow%3ATests
+   :alt: [Github Actions: Test status]
 
 .. image:: https://img.shields.io/coveralls/ssato/python-anyconfig-ion-backend.svg
    :target: https://coveralls.io/r/ssato/python-anyconfig-ion-backend
    :alt: Coverage Status
 
-.. image:: https://landscape.io/github/ssato/python-anyconfig-ion-backend/master/landscape.png
-   :target: https://landscape.io/github/ssato/python-anyconfig-ion-backend/master
-   :alt: Code Health
-
 This is a backend module for python-anyconfig to support to load and dump
 Amazon Ion data files.
 
 - Author: Satoru SATOH <satoru.satoh@gmail.com>
 - License: MIT
 
 SEE ALSO:
```

### Comparing `anyconfig-ion-backend-0.1.1/pkg/package.spec.in` & `anyconfig-ion-backend-0.2.0/pkg/package.spec.in`

 * *Files identical despite different names*

### Comparing `anyconfig-ion-backend-0.1.1/setup.cfg` & `anyconfig-ion-backend-0.2.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = anyconfig-ion-backend
 description = Backend module for python-anyconfig to load and dump CBOR data
 project_urls = 
-	CI: Travis = https://travis-ci.org/ssato/python-anyconfig-ion-backend
+	CI: Github Actions = https://github.com/ssato/python-anyconfig-ion-backend/actions
 	Download = https://pypi.python.org/pypi/anyconfig-ion-backend
 	Download RPMs = https://copr.fedoraproject.org/coprs/ssato/python-anyconfig/
 	Bug Tracker = https://github.com/ssato/python-anyconfig-ion-backend/issues
 	Source = https://github.com/ssato/python-anyconfig-ion-backend
 long_description = 
 	This is a backend module for python-anyconfig to support to load and dump
 	Amazon Ion data files.
@@ -29,20 +29,19 @@
 url = https://github.com/ssato/python-anyconfig-ion-backend
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

### Comparing `anyconfig-ion-backend-0.1.1/setup.py` & `anyconfig-ion-backend-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `anyconfig-ion-backend-0.1.1/src/anyconfig_ion_backend.egg-info/PKG-INFO` & `anyconfig-ion-backend-0.2.0/src/anyconfig_ion_backend.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,42 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: anyconfig-ion-backend
-Version: 0.1.1
+Version: 0.2.0
 Summary: Backend module for python-anyconfig to load and dump CBOR data
 Home-page: https://github.com/ssato/python-anyconfig-ion-backend
 Author: Satoru SATOH
 Author-email: satoru.satoh@gmail.com
 Maintainer: Satoru SATOH
 Maintainer-email: satoru.satoh@gmail.com
 License: MIT
-Project-URL: CI: Travis, https://travis-ci.org/ssato/python-anyconfig-ion-backend
+Project-URL: CI: Github Actions, https://github.com/ssato/python-anyconfig-ion-backend/actions
 Project-URL: Download, https://pypi.python.org/pypi/anyconfig-ion-backend
 Project-URL: Download RPMs, https://copr.fedoraproject.org/coprs/ssato/python-anyconfig/
 Project-URL: Bug Tracker, https://github.com/ssato/python-anyconfig-ion-backend/issues
 Project-URL: Source, https://github.com/ssato/python-anyconfig-ion-backend
-Description: 
-        This is a backend module for python-anyconfig to support to load and dump
-        Amazon Ion data files.
-        
-        - Author: Satoru SATOH <satoru.satoh@gmail.com>
-        - License: MIT
-        
-        SEE ALSO:
-        
-        - python-anyconfig: https://github.com/ssato/python-anyconfig
-        - Amazon Ion: https://amzn.github.io/ion-docs/
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
+This is a backend module for python-anyconfig to support to load and dump
+Amazon Ion data files.
+
+- Author: Satoru SATOH <satoru.satoh@gmail.com>
+- License: MIT
+
+SEE ALSO:
+
+- python-anyconfig: https://github.com/ssato/python-anyconfig
+- Amazon Ion: https://amzn.github.io/ion-docs/
```

### Comparing `anyconfig-ion-backend-0.1.1/src/anyconfig_ion_backend.egg-info/SOURCES.txt` & `anyconfig-ion-backend-0.2.0/src/anyconfig_ion_backend.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-.travis.yml
 LICENSE.MIT
 MANIFEST.in
 README.rst
+mypy.ini
 requirements.txt
 setup.cfg
 setup.py
 tox.ini
+.github/workflows/tests.yml
 pkg/copr-build.sh
 pkg/nose.cfg
 pkg/package.spec.in
 src/anyconfig_ion_backend/__init__.py
 src/anyconfig_ion_backend/ion_.py
 src/anyconfig_ion_backend.egg-info/PKG-INFO
 src/anyconfig_ion_backend.egg-info/SOURCES.txt
 src/anyconfig_ion_backend.egg-info/dependency_links.txt
 src/anyconfig_ion_backend.egg-info/entry_points.txt
 src/anyconfig_ion_backend.egg-info/requires.txt
 src/anyconfig_ion_backend.egg-info/top_level.txt
 tests/__init__.py
 tests/common.py
-tests/ion_.py
-tests/plugin.py
-tests/releng.bats
 tests/requirements.txt
+tests/test_ion_.py
+tests/test_plugin.py
 tests/res/ion.bin_data
 tests/res/ion.txt_data
```

### Comparing `anyconfig-ion-backend-0.1.1/tests/common.py` & `anyconfig-ion-backend-0.2.0/tests/common.py`

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

### Comparing `anyconfig-ion-backend-0.1.1/tests/ion_.py` & `anyconfig-ion-backend-0.2.0/tests/test_ion_.py`

 * *Files identical despite different names*

### Comparing `anyconfig-ion-backend-0.1.1/tests/plugin.py` & `anyconfig-ion-backend-0.2.0/tests/test_plugin.py`

 * *Files identical despite different names*

