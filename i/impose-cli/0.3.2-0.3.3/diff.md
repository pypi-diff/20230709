# Comparing `tmp/impose-cli-0.3.2.tar.gz` & `tmp/impose-cli-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impose-cli-0.3.2.tar", last modified: Sun Jul  9 13:38:02 2023, max compression
+gzip compressed data, was "impose-cli-0.3.3.tar", last modified: Sun Jul  9 18:10:58 2023, max compression
```

## Comparing `impose-cli-0.3.2.tar` & `impose-cli-0.3.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:38:02.610403 impose-cli-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-09 13:37:38.000000 impose-cli-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-09 13:38:02.610403 impose-cli-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-09 13:37:38.000000 impose-cli-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:38:02.610403 impose-cli-0.3.2/impose_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 13:37:38.000000 impose-cli-0.3.2/impose_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11373 2023-07-09 13:37:38.000000 impose-cli-0.3.2/impose_cli/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-09 13:37:38.000000 impose-cli-0.3.2/impose_cli/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-09 13:37:38.000000 impose-cli-0.3.2/impose_cli/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-09 13:37:38.000000 impose-cli-0.3.2/impose_cli/impose_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:38:02.610403 impose-cli-0.3.2/impose_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-09 13:38:02.000000 impose-cli-0.3.2/impose_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-09 13:38:02.000000 impose-cli-0.3.2/impose_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 13:38:02.000000 impose-cli-0.3.2/impose_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-09 13:38:02.000000 impose-cli-0.3.2/impose_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-09 13:38:02.000000 impose-cli-0.3.2/impose_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 13:38:02.610403 impose-cli-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-09 13:37:38.000000 impose-cli-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:38:02.610403 impose-cli-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 13:37:38.000000 impose-cli-0.3.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-09 13:37:38.000000 impose-cli-0.3.2/tests/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:10:58.396620 impose-cli-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-09 18:10:35.000000 impose-cli-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-09 18:10:58.396620 impose-cli-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-09 18:10:35.000000 impose-cli-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:10:58.396620 impose-cli-0.3.3/impose_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 18:10:35.000000 impose-cli-0.3.3/impose_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11393 2023-07-09 18:10:35.000000 impose-cli-0.3.3/impose_cli/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-09 18:10:35.000000 impose-cli-0.3.3/impose_cli/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-09 18:10:35.000000 impose-cli-0.3.3/impose_cli/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-09 18:10:35.000000 impose-cli-0.3.3/impose_cli/impose_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:10:58.396620 impose-cli-0.3.3/impose_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-09 18:10:58.000000 impose-cli-0.3.3/impose_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-09 18:10:58.000000 impose-cli-0.3.3/impose_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 18:10:58.000000 impose-cli-0.3.3/impose_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-09 18:10:58.000000 impose-cli-0.3.3/impose_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-09 18:10:58.000000 impose-cli-0.3.3/impose_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 18:10:58.396620 impose-cli-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-09 18:10:35.000000 impose-cli-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:10:58.396620 impose-cli-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 18:10:35.000000 impose-cli-0.3.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-09 18:10:35.000000 impose-cli-0.3.3/tests/simple.py
```

### Comparing `impose-cli-0.3.2/LICENSE` & `impose-cli-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `impose-cli-0.3.2/README.md` & `impose-cli-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `impose-cli-0.3.2/impose_cli/_utils.py` & `impose-cli-0.3.3/impose_cli/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import os
 import inspect
 import builtins
+import astor
 import click
 from .errors import InterfaceNotImplementedError
 from docstring_parser import parse as docparse
 from inspect import signature as sig
-from ast import parse, FunctionDef, Import, ImportFrom, unparse
+from ast import parse, FunctionDef, Import, ImportFrom
 from importlib.util import spec_from_file_location, module_from_spec
 from os.path import dirname, join, exists, abspath, splitext, basename, relpath
 from . import decorators as imposedecorators
 
 
 def parse_nodes(entry: str, target: str):
     class Function(object):
@@ -81,15 +82,15 @@
                 doc_meta[param.arg_name] = param.description
         if hasattr(node, "args") and getattr(node, "args") is not None and len(getattr(node, "args").args) > 0:
             args_object = getattr(node, "args")
             arg_list = args_object.args
             for arg in arg_list:
                 parameter_meta[arg.arg] = {}
                 if hasattr(arg, "annotation") and getattr(arg, "annotation") is not None:
-                    parameter_meta[arg.arg]["type"] = unparse(getattr(arg, "annotation"))
+                    parameter_meta[arg.arg]["type"] = astor.to_source(getattr(arg, "annotation")).strip()
                 else:
                     parameter_meta[arg.arg]["type"] = "Any"
                 parameter_settings = sig(getattr(module, node.name)).parameters.get(arg.arg)
                 if hasattr(parameter_settings, "default") and \
                         str(getattr(parameter_settings, "default")) != "<class 'inspect._empty'>":
                     parameter_meta[arg.arg]["default"] = parameter_settings.default
                 if arg.arg in doc_meta:
```

### Comparing `impose-cli-0.3.2/impose_cli/impose_cli.py` & `impose-cli-0.3.3/impose_cli/impose_cli.py`

 * *Files identical despite different names*

