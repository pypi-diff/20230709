# Comparing `tmp/roblox-pyc-1.6.6.4.tar.gz` & `tmp/roblox-pyc-1.6.6.4b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roblox-pyc-1.6.6.4.tar", last modified: Sun Jul  9 18:01:04 2023, max compression
+gzip compressed data, was "roblox-pyc-1.6.6.4b0.tar", last modified: Sun Jul  9 18:18:47 2023, max compression
```

## Comparing `roblox-pyc-1.6.6.4.tar` & `roblox-pyc-1.6.6.4b0.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:01:04.829112 roblox-pyc-1.6.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)    34525 2023-07-09 18:00:54.000000 roblox-pyc-1.6.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-09 18:01:04.833112 roblox-pyc-1.6.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-09 18:00:54.000000 roblox-pyc-1.6.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-09 18:00:54.000000 roblox-pyc-1.6.6.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:01:04.825112 roblox-pyc-1.6.6.4/roblox_pyc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-09 18:01:04.000000 roblox-pyc-1.6.6.4/roblox_pyc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-09 18:01:04.000000 roblox-pyc-1.6.6.4/roblox_pyc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 18:01:04.000000 roblox-pyc-1.6.6.4/roblox_pyc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-09 18:01:04.000000 roblox-pyc-1.6.6.4/roblox_pyc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-09 18:01:04.000000 roblox-pyc-1.6.6.4/roblox_pyc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-09 18:01:04.000000 roblox-pyc-1.6.6.4/roblox_pyc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-09 18:01:04.833112 roblox-pyc-1.6.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-09 18:00:54.000000 roblox-pyc-1.6.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:01:04.825112 roblox-pyc-1.6.6.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:01:04.829112 roblox-pyc-1.6.6.4/src/compiler/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 18:00:54.000000 roblox-pyc-1.6.6.4/src/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-09 18:00:54.000000 roblox-pyc-1.6.6.4/src/compiler/binopdesc.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-09 18:00:54.000000 roblox-pyc-1.6.6.4/src/compiler/boolopdesc.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-09 18:00:54.000000 roblox-pyc-1.6.6.4/src/compiler/cmpopdesc.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-09 18:00:54.000000 roblox-pyc-1.6.6.4/src/compiler/colortext.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-09 18:00:54.000000 roblox-pyc-1.6.6.4/src/compiler/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-09 18:00:54.000000 roblox-pyc-1.6.6.4/src/compiler/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-09 18:00:54.000000 roblox-pyc-1.6.6.4/src/compiler/cpAST.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-09 18:00:54.000000 roblox-pyc-1.6.6.4/src/compiler/ctranslator.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-09 18:00:54.000000 roblox-pyc-1.6.6.4/src/compiler/header.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-09 18:00:54.000000 roblox-pyc-1.6.6.4/src/compiler/loopcounter.py
--rw-r--r--   0 runner    (1001) docker     (123)    21165 2023-07-09 18:00:54.000000 roblox-pyc-1.6.6.4/src/compiler/luainit.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-09 18:00:54.000000 roblox-pyc-1.6.6.4/src/compiler/nameconstdesc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27684 2023-07-09 18:00:54.000000 roblox-pyc-1.6.6.4/src/compiler/nodevisitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-09 18:00:54.000000 roblox-pyc-1.6.6.4/src/compiler/pytranslator.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-09 18:00:54.000000 roblox-pyc-1.6.6.4/src/compiler/symbolsstack.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-09 18:00:54.000000 roblox-pyc-1.6.6.4/src/compiler/tokenendmode.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-09 18:00:54.000000 roblox-pyc-1.6.6.4/src/compiler/unaryopdesc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-07-09 18:00:54.000000 roblox-pyc-1.6.6.4/src/robloxpy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:18:47.339972 roblox-pyc-1.6.6.4b0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34525 2023-07-09 18:18:37.000000 roblox-pyc-1.6.6.4b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-09 18:18:47.339972 roblox-pyc-1.6.6.4b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-09 18:18:37.000000 roblox-pyc-1.6.6.4b0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-09 18:18:37.000000 roblox-pyc-1.6.6.4b0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:18:47.339972 roblox-pyc-1.6.6.4b0/roblox_pyc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-09 18:18:47.000000 roblox-pyc-1.6.6.4b0/roblox_pyc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-09 18:18:47.000000 roblox-pyc-1.6.6.4b0/roblox_pyc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 18:18:47.000000 roblox-pyc-1.6.6.4b0/roblox_pyc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-09 18:18:47.000000 roblox-pyc-1.6.6.4b0/roblox_pyc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-09 18:18:47.000000 roblox-pyc-1.6.6.4b0/roblox_pyc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-09 18:18:47.000000 roblox-pyc-1.6.6.4b0/roblox_pyc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-09 18:18:47.339972 roblox-pyc-1.6.6.4b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-09 18:18:37.000000 roblox-pyc-1.6.6.4b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:18:47.339972 roblox-pyc-1.6.6.4b0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 18:18:37.000000 roblox-pyc-1.6.6.4b0/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-09 18:18:37.000000 roblox-pyc-1.6.6.4b0/src/binopdesc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-09 18:18:37.000000 roblox-pyc-1.6.6.4b0/src/boolopdesc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-09 18:18:37.000000 roblox-pyc-1.6.6.4b0/src/cmpopdesc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-09 18:18:37.000000 roblox-pyc-1.6.6.4b0/src/colortext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-09 18:18:37.000000 roblox-pyc-1.6.6.4b0/src/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-09 18:18:37.000000 roblox-pyc-1.6.6.4b0/src/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-09 18:18:37.000000 roblox-pyc-1.6.6.4b0/src/cpAST.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-09 18:18:37.000000 roblox-pyc-1.6.6.4b0/src/ctranslator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-09 18:18:37.000000 roblox-pyc-1.6.6.4b0/src/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-09 18:18:37.000000 roblox-pyc-1.6.6.4b0/src/loopcounter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21165 2023-07-09 18:18:37.000000 roblox-pyc-1.6.6.4b0/src/luainit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-09 18:18:37.000000 roblox-pyc-1.6.6.4b0/src/nameconstdesc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27684 2023-07-09 18:18:37.000000 roblox-pyc-1.6.6.4b0/src/nodevisitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-09 18:18:37.000000 roblox-pyc-1.6.6.4b0/src/pytranslator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-07-09 18:18:37.000000 roblox-pyc-1.6.6.4b0/src/robloxpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-09 18:18:37.000000 roblox-pyc-1.6.6.4b0/src/symbolsstack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-09 18:18:37.000000 roblox-pyc-1.6.6.4b0/src/tokenendmode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-09 18:18:37.000000 roblox-pyc-1.6.6.4b0/src/unaryopdesc.py
```

### Comparing `roblox-pyc-1.6.6.4/LICENSE` & `roblox-pyc-1.6.6.4b0/LICENSE`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.6.6.4/PKG-INFO` & `roblox-pyc-1.6.6.4b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roblox-pyc
-Version: 1.6.6.4
+Version: 1.6.6.4b0
 Summary: A Python, C, C++ to Roblox Lua compiler
 Home-page: https://github.com/AsynchronousAI/roblox-pyc
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # roblox.pyc
```

### Comparing `roblox-pyc-1.6.6.4/README.md` & `roblox-pyc-1.6.6.4b0/README.md`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.6.6.4/roblox_pyc.egg-info/PKG-INFO` & `roblox-pyc-1.6.6.4b0/roblox_pyc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roblox-pyc
-Version: 1.6.6.4
+Version: 1.6.6.4b0
 Summary: A Python, C, C++ to Roblox Lua compiler
 Home-page: https://github.com/AsynchronousAI/roblox-pyc
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # roblox.pyc
```

### Comparing `roblox-pyc-1.6.6.4/src/compiler/binopdesc.py` & `roblox-pyc-1.6.6.4b0/src/binopdesc.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.6.6.4/src/compiler/colortext.py` & `roblox-pyc-1.6.6.4b0/src/colortext.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.6.6.4/src/compiler/config.py` & `roblox-pyc-1.6.6.4b0/src/config.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.6.6.4/src/compiler/context.py` & `roblox-pyc-1.6.6.4b0/src/context.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.6.6.4/src/compiler/luainit.py` & `roblox-pyc-1.6.6.4b0/src/luainit.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.6.6.4/src/compiler/nodevisitor.py` & `roblox-pyc-1.6.6.4b0/src/nodevisitor.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.6.6.4/src/compiler/pytranslator.py` & `roblox-pyc-1.6.6.4b0/src/pytranslator.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.6.6.4/src/compiler/symbolsstack.py` & `roblox-pyc-1.6.6.4b0/src/symbolsstack.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.6.6.4/src/compiler/unaryopdesc.py` & `roblox-pyc-1.6.6.4b0/src/unaryopdesc.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.6.6.4/src/robloxpy.py` & `roblox-pyc-1.6.6.4b0/src/robloxpy.py`

 * *Files identical despite different names*

