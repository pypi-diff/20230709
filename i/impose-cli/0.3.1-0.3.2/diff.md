# Comparing `tmp/impose-cli-0.3.1.tar.gz` & `tmp/impose-cli-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impose-cli-0.3.1.tar", last modified: Sun Jul  9 09:05:42 2023, max compression
+gzip compressed data, was "impose-cli-0.3.2.tar", last modified: Sun Jul  9 13:38:02 2023, max compression
```

## Comparing `impose-cli-0.3.1.tar` & `impose-cli-0.3.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:05:42.395167 impose-cli-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-09 09:05:19.000000 impose-cli-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-09 09:05:42.395167 impose-cli-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-09 09:05:19.000000 impose-cli-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:05:42.395167 impose-cli-0.3.1/impose_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 09:05:19.000000 impose-cli-0.3.1/impose_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11373 2023-07-09 09:05:19.000000 impose-cli-0.3.1/impose_cli/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-09 09:05:19.000000 impose-cli-0.3.1/impose_cli/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-09 09:05:19.000000 impose-cli-0.3.1/impose_cli/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-09 09:05:19.000000 impose-cli-0.3.1/impose_cli/impose_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:05:42.395167 impose-cli-0.3.1/impose_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-09 09:05:42.000000 impose-cli-0.3.1/impose_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-09 09:05:42.000000 impose-cli-0.3.1/impose_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 09:05:42.000000 impose-cli-0.3.1/impose_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-09 09:05:42.000000 impose-cli-0.3.1/impose_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-09 09:05:42.000000 impose-cli-0.3.1/impose_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 09:05:42.395167 impose-cli-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-09 09:05:19.000000 impose-cli-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:05:42.395167 impose-cli-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 09:05:19.000000 impose-cli-0.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-09 09:05:19.000000 impose-cli-0.3.1/tests/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:38:02.610403 impose-cli-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-09 13:37:38.000000 impose-cli-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-09 13:38:02.610403 impose-cli-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-09 13:37:38.000000 impose-cli-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:38:02.610403 impose-cli-0.3.2/impose_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 13:37:38.000000 impose-cli-0.3.2/impose_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11373 2023-07-09 13:37:38.000000 impose-cli-0.3.2/impose_cli/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-09 13:37:38.000000 impose-cli-0.3.2/impose_cli/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-09 13:37:38.000000 impose-cli-0.3.2/impose_cli/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-09 13:37:38.000000 impose-cli-0.3.2/impose_cli/impose_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:38:02.610403 impose-cli-0.3.2/impose_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-09 13:38:02.000000 impose-cli-0.3.2/impose_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-09 13:38:02.000000 impose-cli-0.3.2/impose_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 13:38:02.000000 impose-cli-0.3.2/impose_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-09 13:38:02.000000 impose-cli-0.3.2/impose_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-09 13:38:02.000000 impose-cli-0.3.2/impose_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 13:38:02.610403 impose-cli-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-09 13:37:38.000000 impose-cli-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:38:02.610403 impose-cli-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 13:37:38.000000 impose-cli-0.3.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-09 13:37:38.000000 impose-cli-0.3.2/tests/simple.py
```

### Comparing `impose-cli-0.3.1/LICENSE` & `impose-cli-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `impose-cli-0.3.1/README.md` & `impose-cli-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `impose-cli-0.3.1/impose_cli/_utils.py` & `impose-cli-0.3.2/impose_cli/_utils.py`

 * *Files identical despite different names*

### Comparing `impose-cli-0.3.1/impose_cli/impose_cli.py` & `impose-cli-0.3.2/impose_cli/impose_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from ._utils import parse_nodes, _get_interface_builder
-from inspect import currentframe, getframeinfo
+from inspect import stack
 
 
 def impose_cli(target: str = None, launch_type: str = "cli", launch_specific_configs: dict = {},
                return_before_executing: bool = False, root_name: str = "cli", build_cache: bool = True):
     """
     The entrypoint for building a suite of CLI commands / API endpoints.
     :param launch_specific_configs:
     :param target: Can be used to specify the relative path of a directory which will contain all commands / endpoints.
     :param launch_type: CLI or API.
     :param return_before_executing: Return the produced object before executing.
     :param build_cache: If cache should be built. This could be problematic for larger applications.
     :return:
     """
 
-    tree = parse_nodes(getframeinfo(currentframe().f_back)[0], target)
+    tree = parse_nodes(stack()[1].filename, target)
     return _get_interface_builder(tree, launch_type, root_name, launch_specific_configs, return_before_executing)
```

