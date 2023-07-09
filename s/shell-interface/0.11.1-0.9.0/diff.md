# Comparing `tmp/shell_interface-0.11.1.tar.gz` & `tmp/shell_interface-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shell_interface-0.11.1.tar", max compression
+gzip compressed data, was "shell_interface-0.9.0.tar", max compression
```

## Comparing `shell_interface-0.11.1.tar` & `shell_interface-0.9.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35106 2023-07-09 00:27:20.538171 shell_interface-0.11.1/LICENSE
--rw-r--r--   0        0        0     1270 2023-07-09 00:27:20.538171 shell_interface-0.11.1/pyproject.toml
--rw-r--r--   0        0        0      363 2023-07-09 00:27:20.538171 shell_interface-0.11.1/src/shell_interface/__init__.py
--rw-r--r--   0        0        0        0 2023-07-09 00:27:20.538171 shell_interface-0.11.1/src/shell_interface/py.typed
--rw-r--r--   0        0        0     4458 2023-07-09 00:27:20.538171 shell_interface-0.11.1/src/shell_interface/shell_interface.py
--rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 shell_interface-0.11.1/PKG-INFO
+-rw-r--r--   0        0        0    35106 2023-06-15 09:18:53.630323 shell_interface-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1197 2023-06-15 10:28:46.770111 shell_interface-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      282 2023-06-15 10:21:50.909541 shell_interface-0.9.0/src/shell_interface/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 09:30:30.916346 shell_interface-0.9.0/src/shell_interface/py.typed
+-rw-r--r--   0        0        0     1851 2023-06-15 09:30:30.916346 shell_interface-0.9.0/src/shell_interface/shell_interface.py
+-rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 shell_interface-0.9.0/PKG-INFO
```

### Comparing `shell_interface-0.11.1/LICENSE` & `shell_interface-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shell_interface-0.11.1/PKG-INFO` & `shell_interface-0.9.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: shell-interface
-Version: 0.11.1
+Version: 0.9.0
 Summary: Helpful and convenient utilities to interact with UNIX shells
 License: GPL-3.0-or-later
 Author: Max Görner
 Author-email: max@familie-goerner.eu
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: logging
-Requires-Dist: loguru (>=0.7.0,<0.8.0) ; extra == "logging"
+Requires-Dist: loguru (>=0.7.0,<0.8.0)
```

