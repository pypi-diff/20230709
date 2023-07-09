# Comparing `tmp/anyconfig-msgpack-backend-0.1.1.tar.gz` & `tmp/anyconfig-msgpack-backend-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/anyconfig-msgpack-backend-0.1.1.tar", last modified: Thu Apr 30 18:38:53 2020, max compression
+gzip compressed data, was "anyconfig-msgpack-backend-0.2.0.tar", last modified: Sun Jul  9 13:17:49 2023, max compression
```

## Comparing `anyconfig-msgpack-backend-0.1.1.tar` & `anyconfig-msgpack-backend-0.2.0.tar`

### file list

```diff
@@ -1,36 +1,34 @@
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 18:38:53.000000 anyconfig-msgpack-backend-0.1.1/
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      470 2020-04-30 18:08:58.000000 anyconfig-msgpack-backend-0.1.1/.travis.yml
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1069 2018-01-05 16:33:29.000000 anyconfig-msgpack-backend-0.1.1/LICENSE.MIT
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      219 2020-04-30 18:08:58.000000 anyconfig-msgpack-backend-0.1.1/MANIFEST.in
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      339 2020-04-30 18:36:19.000000 anyconfig-msgpack-backend-0.1.1/NEWS
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     3506 2020-04-30 18:38:53.000000 anyconfig-msgpack-backend-0.1.1/PKG-INFO
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1613 2018-01-14 12:23:40.000000 anyconfig-msgpack-backend-0.1.1/README.rst
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 18:38:53.000000 anyconfig-msgpack-backend-0.1.1/pkg/
--rwxrwxr-x   0 ssato     (1000) ssato     (1000)      494 2018-01-01 13:54:49.000000 anyconfig-msgpack-backend-0.1.1/pkg/copr-build.sh
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      109 2018-01-14 12:24:55.000000 anyconfig-msgpack-backend-0.1.1/pkg/nose.cfg
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1963 2019-10-01 11:29:52.000000 anyconfig-msgpack-backend-0.1.1/pkg/package.spec.in
--rwxrwxr-x   0 ssato     (1000) ssato     (1000)     1957 2015-05-31 14:02:48.000000 anyconfig-msgpack-backend-0.1.1/pkg/rpmbuild-wrapper.sh
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       18 2018-01-14 12:37:22.000000 anyconfig-msgpack-backend-0.1.1/requirements.txt
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1666 2020-04-30 18:38:53.000000 anyconfig-msgpack-backend-0.1.1/setup.cfg
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1501 2020-04-30 18:08:58.000000 anyconfig-msgpack-backend-0.1.1/setup.py
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 18:38:53.000000 anyconfig-msgpack-backend-0.1.1/src/
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 18:38:53.000000 anyconfig-msgpack-backend-0.1.1/src/anyconfig_msgpack_backend/
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      171 2020-04-30 18:37:37.000000 anyconfig-msgpack-backend-0.1.1/src/anyconfig_msgpack_backend/__init__.py
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1733 2018-01-14 13:53:49.000000 anyconfig-msgpack-backend-0.1.1/src/anyconfig_msgpack_backend/msgpack_.py
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 18:38:53.000000 anyconfig-msgpack-backend-0.1.1/src/anyconfig_msgpack_backend.egg-info/
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     3506 2020-04-30 18:38:53.000000 anyconfig-msgpack-backend-0.1.1/src/anyconfig_msgpack_backend.egg-info/PKG-INFO
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      703 2020-04-30 18:38:53.000000 anyconfig-msgpack-backend-0.1.1/src/anyconfig_msgpack_backend.egg-info/SOURCES.txt
--rw-rw-r--   0 ssato     (1000) ssato     (1000)        1 2020-04-30 18:38:53.000000 anyconfig-msgpack-backend-0.1.1/src/anyconfig_msgpack_backend.egg-info/dependency_links.txt
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       65 2020-04-30 18:38:53.000000 anyconfig-msgpack-backend-0.1.1/src/anyconfig_msgpack_backend.egg-info/entry_points.txt
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       18 2020-04-30 18:38:53.000000 anyconfig-msgpack-backend-0.1.1/src/anyconfig_msgpack_backend.egg-info/requires.txt
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       26 2020-04-30 18:38:53.000000 anyconfig-msgpack-backend-0.1.1/src/anyconfig_msgpack_backend.egg-info/top_level.txt
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 18:38:53.000000 anyconfig-msgpack-backend-0.1.1/tests/
--rw-rw-r--   0 ssato     (1000) ssato     (1000)        0 2015-05-31 04:08:11.000000 anyconfig-msgpack-backend-0.1.1/tests/__init__.py
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     8428 2020-04-30 18:32:14.000000 anyconfig-msgpack-backend-0.1.1/tests/common.py
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1962 2019-10-01 11:59:07.000000 anyconfig-msgpack-backend-0.1.1/tests/msgpack_.py
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      931 2020-04-30 18:09:40.000000 anyconfig-msgpack-backend-0.1.1/tests/plugin.py
--rwxrwxr-x   0 ssato     (1000) ssato     (1000)     1545 2019-10-01 11:30:01.000000 anyconfig-msgpack-backend-0.1.1/tests/releng.bats
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       41 2020-04-30 18:10:13.000000 anyconfig-msgpack-backend-0.1.1/tests/requirements.txt
-drwxrwxr-x   0 ssato     (1000) ssato     (1000)        0 2020-04-30 18:38:53.000000 anyconfig-msgpack-backend-0.1.1/tests/res/
--rw-rw-r--   0 ssato     (1000) ssato     (1000)       53 2018-01-14 12:16:47.000000 anyconfig-msgpack-backend-0.1.1/tests/res/0.msgpack
--rw-rw-r--   0 ssato     (1000) ssato     (1000)      972 2020-04-30 18:08:58.000000 anyconfig-msgpack-backend-0.1.1/tox.ini
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 13:17:49.294580 anyconfig-msgpack-backend-0.2.0/
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)     1069 2018-01-05 16:33:29.000000 anyconfig-msgpack-backend-0.2.0/LICENSE.MIT
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      222 2023-07-09 13:12:45.000000 anyconfig-msgpack-backend-0.2.0/MANIFEST.in
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)      339 2020-04-30 18:36:19.000000 anyconfig-msgpack-backend-0.2.0/NEWS
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     3080 2023-07-09 13:17:49.294580 anyconfig-msgpack-backend-0.2.0/PKG-INFO
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     1670 2023-07-09 13:12:45.000000 anyconfig-msgpack-backend-0.2.0/README.rst
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 13:17:49.292580 anyconfig-msgpack-backend-0.2.0/pkg/
+-rwxrwxr-x   0 ssato     (1000) ssato     (1000)      494 2018-01-01 13:54:49.000000 anyconfig-msgpack-backend-0.2.0/pkg/copr-build.sh
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)      109 2018-01-14 12:24:55.000000 anyconfig-msgpack-backend-0.2.0/pkg/nose.cfg
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     1436 2023-07-09 13:12:45.000000 anyconfig-msgpack-backend-0.2.0/pkg/package.spec.in
+-rwxrwxr-x   0 ssato     (1000) ssato     (1000)     1957 2015-05-31 14:02:48.000000 anyconfig-msgpack-backend-0.2.0/pkg/rpmbuild-wrapper.sh
+-rw-r--r--   0 ssato     (1000) ssato     (1000)       92 2023-07-09 13:12:45.000000 anyconfig-msgpack-backend-0.2.0/requirements.txt
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     1608 2023-07-09 13:17:49.294580 anyconfig-msgpack-backend-0.2.0/setup.cfg
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)     1501 2020-04-30 18:08:58.000000 anyconfig-msgpack-backend-0.2.0/setup.py
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 13:17:49.291580 anyconfig-msgpack-backend-0.2.0/src/
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 13:17:49.292580 anyconfig-msgpack-backend-0.2.0/src/anyconfig_msgpack_backend/
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      171 2023-07-09 13:16:41.000000 anyconfig-msgpack-backend-0.2.0/src/anyconfig_msgpack_backend/__init__.py
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     1804 2023-07-09 13:12:45.000000 anyconfig-msgpack-backend-0.2.0/src/anyconfig_msgpack_backend/msgpack_.py
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 13:17:49.293580 anyconfig-msgpack-backend-0.2.0/src/anyconfig_msgpack_backend.egg-info/
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     3080 2023-07-09 13:17:49.000000 anyconfig-msgpack-backend-0.2.0/src/anyconfig_msgpack_backend.egg-info/PKG-INFO
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      682 2023-07-09 13:17:49.000000 anyconfig-msgpack-backend-0.2.0/src/anyconfig_msgpack_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 ssato     (1000) ssato     (1000)        1 2023-07-09 13:17:49.000000 anyconfig-msgpack-backend-0.2.0/src/anyconfig_msgpack_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 ssato     (1000) ssato     (1000)       64 2023-07-09 13:17:49.000000 anyconfig-msgpack-backend-0.2.0/src/anyconfig_msgpack_backend.egg-info/entry_points.txt
+-rw-r--r--   0 ssato     (1000) ssato     (1000)       18 2023-07-09 13:17:49.000000 anyconfig-msgpack-backend-0.2.0/src/anyconfig_msgpack_backend.egg-info/requires.txt
+-rw-r--r--   0 ssato     (1000) ssato     (1000)       26 2023-07-09 13:17:49.000000 anyconfig-msgpack-backend-0.2.0/src/anyconfig_msgpack_backend.egg-info/top_level.txt
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 13:17:49.293580 anyconfig-msgpack-backend-0.2.0/tests/
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)        0 2015-05-31 04:08:11.000000 anyconfig-msgpack-backend-0.2.0/tests/__init__.py
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     8780 2023-07-09 13:12:45.000000 anyconfig-msgpack-backend-0.2.0/tests/common.py
+-rw-r--r--   0 ssato     (1000) ssato     (1000)       70 2023-07-09 13:12:45.000000 anyconfig-msgpack-backend-0.2.0/tests/requirements.txt
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 13:17:49.294580 anyconfig-msgpack-backend-0.2.0/tests/res/
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)       53 2018-01-14 12:16:47.000000 anyconfig-msgpack-backend-0.2.0/tests/res/0.msgpack
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     1922 2023-07-09 13:12:45.000000 anyconfig-msgpack-backend-0.2.0/tests/test_msgpack.py
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      931 2023-07-09 13:12:45.000000 anyconfig-msgpack-backend-0.2.0/tests/test_plugin.py
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      828 2023-07-09 13:12:45.000000 anyconfig-msgpack-backend-0.2.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `anyconfig-msgpack-backend-0.1.1/LICENSE.MIT` & `anyconfig-msgpack-backend-0.2.0/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `anyconfig-msgpack-backend-0.1.1/README.rst` & `anyconfig-msgpack-backend-0.2.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 python-anyconfig-msgpack-backend
 ==================================
 
 .. .. image:: https://img.shields.io/pypi/v/anyconfig-msgpack-backend.svg
    :target: https://pypi.python.org/pypi/anyconfig-msgpack-backend/
    :alt: [Latest Version]
 
-.. image:: https://img.shields.io/travis/ssato/python-anyconfig-msgpack-backend.svg
-   :target: https://travis-ci.org/ssato/python-anyconfig-msgpack-backend
-   :alt: Test status
+.. image:: https://github.com/ssato/python-anyconfig-msgpack-backend/workflows/Tests/badge.svg
+   :target: https://github.com/ssato/python-anyconfig-msgpack-backend/actions?query=workflow%3ATests
+   :alt: [Github Actions: Test status]
 
 .. image:: https://img.shields.io/coveralls/ssato/python-anyconfig-msgpack-backend.svg
    :target: https://coveralls.io/r/ssato/python-anyconfig-msgpack-backend
    :alt: Coverage Status
 
 .. image:: https://landscape.io/github/ssato/python-anyconfig-msgpack-backend/master/landscape.png
    :target: https://landscape.io/github/ssato/python-anyconfig-msgpack-backend/master
```

### Comparing `anyconfig-msgpack-backend-0.1.1/pkg/rpmbuild-wrapper.sh` & `anyconfig-msgpack-backend-0.2.0/pkg/rpmbuild-wrapper.sh`

 * *Files identical despite different names*

### Comparing `anyconfig-msgpack-backend-0.1.1/setup.cfg` & `anyconfig-msgpack-backend-0.2.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -11,34 +11,32 @@
 author = Satoru SATOH
 author_email = satoru.satoh@gmail.com
 maintainer = Satoru SATOH
 maintainer_email = satoru.satoh@gmail.com
 license = MIT
 url = https://github.com/ssato/python-anyconfig-msgpack-backend
 project_urls = 
-	CI: Travis = https://travis-ci.org/ssato/python-anyconfig-msgpack-backend
+	CI: Github Actions = https://github.com/ssato/python-anyconfig-msgpack-backend/actions
 	Download = https://pypi.org/project/anyconfig-msgpack-backend/
 	Download RPMs = https://copr.fedoraproject.org/coprs/ssato/python-anyconfig/
 	Bug Tracker = https://github.com/ssato/python-anyconfig-msgpack-backend/issues
 	Source = https://github.com/ssato/python-anyconfig-msgpack-backend
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
-	Topic :: Text Processing :: Markup
 	Topic :: Utilities
 	License :: OSI Approved :: MIT License
 
 [options]
 include_package_data = True
 packages = find:
 install_requires =
```

### Comparing `anyconfig-msgpack-backend-0.1.1/setup.py` & `anyconfig-msgpack-backend-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `anyconfig-msgpack-backend-0.1.1/src/anyconfig_msgpack_backend/msgpack_.py` & `anyconfig-msgpack-backend-0.2.0/src/anyconfig_msgpack_backend/msgpack_.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2015 - 2017 Satoru SATOH <ssato @ redhat.com>
+# Copyright (C) 2015 - 2019 Satoru SATOH <satoru.satoh@gmail.com>
 # License: MIT
 #
 # Ref. python -c "import msgpack; help(msgpack.Unpacker); help(msgpack.Packer)"
 #
 r"""MessagePack backend:
 
 - Format to support: MessagePack, http://msgpack.org
@@ -17,38 +17,41 @@
 
   - See also: https://pypi.python.org/pypi/msgpack/
 
 Changelog:
 
     .. versionadded:: 0.0.11
 """
-from __future__ import absolute_import
+import typing
 
 import msgpack
-import anyconfig.backend.base
-import anyconfig.compat
 
-from anyconfig.backend.base import to_method
+import anyconfig.backend.base
 
 
 class Parser(anyconfig.backend.base.StringStreamFnParser,
-             anyconfig.backend.base.BinaryFilesMixin):
+             anyconfig.backend.base.BinaryLoaderMixin,
+             anyconfig.backend.base.BinaryDumperMixin):
     """
     Loader/Dumper for MessagePack files.
     """
-    _type = "msgpack"
-    _extensions = []
-    _load_opts = ["read_size", "use_list", "object_hook", "list_hook",
-                  "encoding", "unicode_errors", "max_buffer_size", "ext_hook",
-                  "max_str_len", "max_bin_len", "max_array_len", "max_map_len",
-                  "max_ext_len", "object_pairs_hook"]
-    _dump_opts = ["default", "encoding", "unicode_errors", "use_single_float",
-                  "autoreset", "use_bin_type"]
-    _ordered = not anyconfig.compat.IS_PYTHON_3  # TODO.
-    _dict_opts = ["object_pairs_hook"]  # Exclusive with object_hook
-
-    _load_from_string_fn = to_method(msgpack.unpackb)
-    _load_from_stream_fn = to_method(msgpack.unpack)
-    _dump_to_string_fn = to_method(msgpack.packb)
-    _dump_to_stream_fn = to_method(msgpack.pack)
+    _type: [str] = 'msgpack'
+    _extensions: typing.List[str] = []
+    _load_opts: typing.List[str] = [
+        'read_size', 'use_list', 'object_hook', 'list_hook',
+        'encoding', 'unicode_errors', 'max_buffer_size', 'ext_hook',
+        'max_str_len', 'max_bin_len', 'max_array_len', 'max_map_len',
+        'max_ext_len', 'object_pairs_hook'
+    ]
+    _dump_opts: typing.List[str] = [
+        'default', 'encoding', 'unicode_errors', 'use_single_float',
+        'autoreset', 'use_bin_type'
+    ]
+    # Exclusive with object_hook
+    _dict_opts: typing.List[str] = ['object_pairs_hook']
+
+    _load_from_string_fn = anyconfig.backend.base.to_method(msgpack.unpackb)
+    _load_from_stream_fn = anyconfig.backend.base.to_method(msgpack.unpack)
+    _dump_to_string_fn = anyconfig.backend.base.to_method(msgpack.packb)
+    _dump_to_stream_fn = anyconfig.backend.base.to_method(msgpack.pack)
 
 # vim:sw=4:ts=4:et:
```

### Comparing `anyconfig-msgpack-backend-0.1.1/src/anyconfig_msgpack_backend.egg-info/SOURCES.txt` & `anyconfig-msgpack-backend-0.2.0/src/anyconfig_msgpack_backend.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

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
@@ -17,12 +16,11 @@
 src/anyconfig_msgpack_backend.egg-info/SOURCES.txt
 src/anyconfig_msgpack_backend.egg-info/dependency_links.txt
 src/anyconfig_msgpack_backend.egg-info/entry_points.txt
 src/anyconfig_msgpack_backend.egg-info/requires.txt
 src/anyconfig_msgpack_backend.egg-info/top_level.txt
 tests/__init__.py
 tests/common.py
-tests/msgpack_.py
-tests/plugin.py
-tests/releng.bats
 tests/requirements.txt
+tests/test_msgpack.py
+tests/test_plugin.py
 tests/res/0.msgpack
```

### Comparing `anyconfig-msgpack-backend-0.1.1/tests/common.py` & `anyconfig-msgpack-backend-0.2.0/tests/common.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,44 @@
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
+import anyconfig.ioinfo
 
 from anyconfig.utils import is_dict_like
 
 
-OrderedDict = anyconfig.compat.OrderedDict
-CNF_0 = dict(((u"DEFAULT",
-               dict(((u"a", u"0"),
-                     (u"b", u"bbb"),
-                     (u"c", u"5")))),
-              (u"sect0",
-               dict(((u"a", u"0"),
-                     (u"b", u"bbb"),
-                     (u"c", u"5"),
-                     (u"d", u"x,y,z"))))))
+CNF_0 = OrderedDict((("DEFAULT", OrderedDict((("a", "0"), ("b", "bbb"),
+                                              ("c", "5")))),
+                     ("sect0", OrderedDict((("a", "0"), ("b", "bbb"),
+                                            ("c", "5"),
+                                            ("d", "x,y,z"))))))
 CNF_1 = copy.deepcopy(CNF_0)
-CNF_1[u"sect0"][u"d"] = u"x,y,z".split()
+CNF_1["sect0"]["d"] = CNF_1["sect0"]["d"].split()
+
 
-CNF_2 = dict(((u"a", 0.1),
-              (u"b", u"bbb"),
-              (u"sect0",
-               dict(((u"c", [u"x", u"y", u"z"]), )))))
+def _bytes(astr):
+    """
+    Convert a string to bytes. Do nothing in python 2.6.
+    """
+    return bytes(astr, 'utf-8')
+
+
+CNF_2 = OrderedDict((("a", 0.1), ("b", _bytes("bbb")),
+                     ("sect0", OrderedDict((("c", [_bytes("x"), _bytes("y"),
+                                                   _bytes("z")]), )))))
 
 
 def selfdir():
     """
     >>> os.path.exists(selfdir())
     True
     """
@@ -129,14 +130,17 @@
 
     def is_ready(self):
         return self.psr is not None
 
 
 class TestBase(unittest.TestCase, HasParserTrait):
 
+    def _to_ioinfo(self, path):
+        return anyconfig.ioinfo.make(path)
+
     def _assert_dicts_equal(self, cnf, ordered=False, cls=None, ref=None):
         if ref is None:
             ref = self.cnf
         self.assertTrue(dicts_equal(cnf, ref, ordered=ordered),
                         "%s %r%svs.%s %r" % (lsep, cnf, lsep, lsep, ref))
         # .. note::
         #    `cnf` may not be an instance of `cls` even if ac_dict option was
@@ -222,61 +226,64 @@
         super(TestBaseWithIO, self).setUp()
         if self.is_ready():
             self.workdir = setup_workdir()
 
             exts = self.psr.extensions()
             ext = exts[0] if exts else "conf"
             self.cnf_path = os.path.join(self.workdir, "cnf_0." + ext)
+            self.ioi = self._to_ioinfo(self.cnf_path)
 
             with self.psr.wopen(self.cnf_path) as out:
                 out.write(self.cnf_s)
 
     def tearDown(self):
         if self.is_ready():
             cleanup_workdir(self.workdir)
 
 
 class Test_20_dump_and_load(TestBaseWithIO):
 
     def test_10_load(self):
         if self.is_ready():
-            cnf = self.psr.load(self.cnf_path)
+            cnf = self.psr.load(self.ioi)
             self.assertTrue(cnf)
             self._assert_dicts_equal(cnf)
 
     def test_12_load_from_stream(self):
         if self.is_ready():
             with self.psr.ropen(self.cnf_path) as strm:
-                cnf = self.psr.load(strm)
+                ioi = self._to_ioinfo(strm)
+                cnf = self.psr.load(ioi)
 
             self.assertTrue(cnf)
             self._assert_dicts_equal(cnf)
 
     def test_14_load_with_ac_ordered_option(self):
         if self.is_ready():
-            cnf = self.psr.load(self.cnf_path, ac_ordered=True)
+            cnf = self.psr.load(self.ioi, ac_ordered=True)
             self.assertTrue(cnf)
             self._assert_dicts_equal(cnf, ordered=self.psr.ordered())
 
     def test_16_load_with_ac_dict_option(self):
         if self.is_ready():
-            cnf = self.psr.load(self.cnf_path, ac_dict=MyDict)
+            cnf = self.psr.load(self.ioi, ac_dict=MyDict)
             self.assertTrue(cnf)
             self._assert_dicts_equal(cnf, cls=MyDict)
 
     def test_30_dump(self):
         if self.is_ready():
-            self.psr.dump(self.cnf, self.cnf_path)
-            cnf = self.psr.load(self.cnf_path)
+            self.psr.dump(self.cnf, self.ioi)
+            cnf = self.psr.load(self.ioi)
             self.assertTrue(cnf)
             self._assert_dicts_equal(cnf)
 
     def test_32_dump_to_stream(self):
         if self.is_ready():
             with self.psr.wopen(self.cnf_path) as strm:
-                self.psr.dump(self.cnf, strm)
+                ioi = self._to_ioinfo(strm)
+                self.psr.dump(self.cnf, ioi)
 
-            cnf = self.psr.load(self.cnf_path)
+            cnf = self.psr.load(self.ioi)
             self.assertTrue(cnf)
             self._assert_dicts_equal(cnf)
 
 # vim:sw=4:ts=4:et:
```

### Comparing `anyconfig-msgpack-backend-0.1.1/tests/msgpack_.py` & `anyconfig-msgpack-backend-0.2.0/tests/test_msgpack.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 #
 # Copyright (C) 2018 - 2019 Satoru SATOH <satoru.satoh @ gmail.com>
 # Copyright (C) 2015 - 2018 Satoru SATOH <ssato @ redhat.com>
 # Copyright (C) 2017 Red Hat, Inc.
 # License: MIT
 #
 # pylint: disable=missing-docstring,invalid-name,too-few-public-methods
-from __future__ import absolute_import
-
 import msgpack
 
 # import copy
 import anyconfig_msgpack_backend as TT
 import tests.common as TBC
```

### Comparing `anyconfig-msgpack-backend-0.1.1/tests/plugin.py` & `anyconfig-msgpack-backend-0.2.0/tests/test_plugin.py`

 * *Files identical despite different names*

