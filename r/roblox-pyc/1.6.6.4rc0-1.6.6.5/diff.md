# Comparing `tmp/roblox-pyc-1.6.6.4rc0.tar.gz` & `tmp/roblox-pyc-1.6.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roblox-pyc-1.6.6.4rc0.tar", last modified: Sun Jul  9 18:23:57 2023, max compression
+gzip compressed data, was "roblox-pyc-1.6.6.5.tar", last modified: Sun Jul  9 18:30:43 2023, max compression
```

## Comparing `roblox-pyc-1.6.6.4rc0.tar` & `roblox-pyc-1.6.6.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:23:57.341713 roblox-pyc-1.6.6.4rc0/
--rw-r--r--   0 runner    (1001) docker     (123)    34525 2023-07-09 18:23:47.000000 roblox-pyc-1.6.6.4rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-07-09 18:23:57.341713 roblox-pyc-1.6.6.4rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-09 18:23:47.000000 roblox-pyc-1.6.6.4rc0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-09 18:23:47.000000 roblox-pyc-1.6.6.4rc0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:23:57.337713 roblox-pyc-1.6.6.4rc0/roblox_pyc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-07-09 18:23:57.000000 roblox-pyc-1.6.6.4rc0/roblox_pyc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-09 18:23:57.000000 roblox-pyc-1.6.6.4rc0/roblox_pyc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 18:23:57.000000 roblox-pyc-1.6.6.4rc0/roblox_pyc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-09 18:23:57.000000 roblox-pyc-1.6.6.4rc0/roblox_pyc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-09 18:23:57.000000 roblox-pyc-1.6.6.4rc0/roblox_pyc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-09 18:23:57.000000 roblox-pyc-1.6.6.4rc0/roblox_pyc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-09 18:23:57.341713 roblox-pyc-1.6.6.4rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-09 18:23:47.000000 roblox-pyc-1.6.6.4rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:23:57.341713 roblox-pyc-1.6.6.4rc0/src/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 18:23:47.000000 roblox-pyc-1.6.6.4rc0/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-09 18:23:47.000000 roblox-pyc-1.6.6.4rc0/src/binopdesc.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-09 18:23:47.000000 roblox-pyc-1.6.6.4rc0/src/boolopdesc.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-09 18:23:47.000000 roblox-pyc-1.6.6.4rc0/src/cmpopdesc.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-09 18:23:47.000000 roblox-pyc-1.6.6.4rc0/src/colortext.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-09 18:23:47.000000 roblox-pyc-1.6.6.4rc0/src/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-09 18:23:47.000000 roblox-pyc-1.6.6.4rc0/src/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-09 18:23:47.000000 roblox-pyc-1.6.6.4rc0/src/cpAST.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-09 18:23:47.000000 roblox-pyc-1.6.6.4rc0/src/ctranslator.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-09 18:23:47.000000 roblox-pyc-1.6.6.4rc0/src/header.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-09 18:23:47.000000 roblox-pyc-1.6.6.4rc0/src/loopcounter.py
--rw-r--r--   0 runner    (1001) docker     (123)    21165 2023-07-09 18:23:47.000000 roblox-pyc-1.6.6.4rc0/src/luainit.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-09 18:23:47.000000 roblox-pyc-1.6.6.4rc0/src/nameconstdesc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27684 2023-07-09 18:23:47.000000 roblox-pyc-1.6.6.4rc0/src/nodevisitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-09 18:23:47.000000 roblox-pyc-1.6.6.4rc0/src/pytranslator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-07-09 18:23:47.000000 roblox-pyc-1.6.6.4rc0/src/robloxpy.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-09 18:23:47.000000 roblox-pyc-1.6.6.4rc0/src/symbolsstack.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-09 18:23:47.000000 roblox-pyc-1.6.6.4rc0/src/tokenendmode.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-09 18:23:47.000000 roblox-pyc-1.6.6.4rc0/src/unaryopdesc.py
+drwxr-xr-x   0 aaravs     (501) staff       (20)        0 2023-07-09 18:30:43.762433 roblox-pyc-1.6.6.5/
+-rw-r--r--   0 aaravs     (501) staff       (20)    34525 2023-07-07 21:26:51.000000 roblox-pyc-1.6.6.5/LICENSE
+-rw-r--r--   0 aaravs     (501) staff       (20)     3008 2023-07-09 18:30:43.762694 roblox-pyc-1.6.6.5/PKG-INFO
+-rw-r--r--   0 aaravs     (501) staff       (20)     2784 2023-07-09 17:36:20.000000 roblox-pyc-1.6.6.5/README.md
+-rw-r--r--   0 aaravs     (501) staff       (20)       89 2023-07-09 01:34:29.000000 roblox-pyc-1.6.6.5/pyproject.toml
+drwxr-xr-x   0 aaravs     (501) staff       (20)        0 2023-07-09 18:30:43.747477 roblox-pyc-1.6.6.5/roblox_pyc.egg-info/
+-rw-r--r--   0 aaravs     (501) staff       (20)     3008 2023-07-09 18:30:43.000000 roblox-pyc-1.6.6.5/roblox_pyc.egg-info/PKG-INFO
+-rw-r--r--   0 aaravs     (501) staff       (20)      586 2023-07-09 18:30:43.000000 roblox-pyc-1.6.6.5/roblox_pyc.egg-info/SOURCES.txt
+-rw-r--r--   0 aaravs     (501) staff       (20)        1 2023-07-09 18:30:43.000000 roblox-pyc-1.6.6.5/roblox_pyc.egg-info/dependency_links.txt
+-rw-r--r--   0 aaravs     (501) staff       (20)      102 2023-07-09 18:30:43.000000 roblox-pyc-1.6.6.5/roblox_pyc.egg-info/entry_points.txt
+-rw-r--r--   0 aaravs     (501) staff       (20)       43 2023-07-09 18:30:43.000000 roblox-pyc-1.6.6.5/roblox_pyc.egg-info/requires.txt
+-rw-r--r--   0 aaravs     (501) staff       (20)        4 2023-07-09 18:30:43.000000 roblox-pyc-1.6.6.5/roblox_pyc.egg-info/top_level.txt
+-rw-r--r--   0 aaravs     (501) staff       (20)      242 2023-07-09 18:30:43.763669 roblox-pyc-1.6.6.5/setup.cfg
+-rw-r--r--   0 aaravs     (501) staff       (20)      440 2023-07-09 15:41:08.000000 roblox-pyc-1.6.6.5/setup.py
+drwxr-xr-x   0 aaravs     (501) staff       (20)        0 2023-07-09 18:30:43.761639 roblox-pyc-1.6.6.5/src/
+-rw-r--r--   0 aaravs     (501) staff       (20)       38 2023-07-07 21:26:51.000000 roblox-pyc-1.6.6.5/src/__init__.py
+-rw-r--r--   0 aaravs     (501) staff       (20)     1464 2023-07-07 21:26:51.000000 roblox-pyc-1.6.6.5/src/binopdesc.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      382 2023-07-07 21:26:51.000000 roblox-pyc-1.6.6.5/src/boolopdesc.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      450 2023-07-07 21:26:51.000000 roblox-pyc-1.6.6.5/src/cmpopdesc.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      800 2023-07-09 03:44:33.000000 roblox-pyc-1.6.6.5/src/colortext.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      790 2023-07-07 21:26:51.000000 roblox-pyc-1.6.6.5/src/config.py
+-rw-r--r--   0 aaravs     (501) staff       (20)     1050 2023-07-07 21:26:51.000000 roblox-pyc-1.6.6.5/src/context.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      447 2023-07-09 15:13:23.000000 roblox-pyc-1.6.6.5/src/cpAST.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      405 2023-07-09 15:15:08.000000 roblox-pyc-1.6.6.5/src/ctranslator.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      482 2023-07-09 17:33:56.000000 roblox-pyc-1.6.6.5/src/header.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      282 2023-07-09 01:58:37.000000 roblox-pyc-1.6.6.5/src/loopcounter.py
+-rw-r--r--   0 aaravs     (501) staff       (20)    21165 2023-07-09 17:23:29.000000 roblox-pyc-1.6.6.5/src/luainit.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      181 2023-07-07 21:26:51.000000 roblox-pyc-1.6.6.5/src/nameconstdesc.py
+-rw-r--r--   0 aaravs     (501) staff       (20)    27684 2023-07-09 01:59:38.000000 roblox-pyc-1.6.6.5/src/nodevisitor.py
+-rw-r--r--   0 aaravs     (501) staff       (20)     2153 2023-07-09 17:33:27.000000 roblox-pyc-1.6.6.5/src/pytranslator.py
+-rw-r--r--   0 aaravs     (501) staff       (20)     7630 2023-07-09 18:22:04.000000 roblox-pyc-1.6.6.5/src/robloxpy.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      642 2023-07-07 21:26:51.000000 roblox-pyc-1.6.6.5/src/symbolsstack.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      157 2023-07-07 21:26:51.000000 roblox-pyc-1.6.6.5/src/tokenendmode.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      567 2023-07-08 14:04:57.000000 roblox-pyc-1.6.6.5/src/unaryopdesc.py
```

### Comparing `roblox-pyc-1.6.6.4rc0/LICENSE` & `roblox-pyc-1.6.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.6.6.4rc0/PKG-INFO` & `roblox-pyc-1.6.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roblox-pyc
-Version: 1.6.6.4rc0
+Version: 1.6.6.5
 Summary: A Python, C, C++ to Roblox Lua compiler
 Home-page: https://github.com/AsynchronousAI/roblox-pyc
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # roblox.pyc
```

### Comparing `roblox-pyc-1.6.6.4rc0/README.md` & `roblox-pyc-1.6.6.5/README.md`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.6.6.4rc0/roblox_pyc.egg-info/PKG-INFO` & `roblox-pyc-1.6.6.5/roblox_pyc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roblox-pyc
-Version: 1.6.6.4rc0
+Version: 1.6.6.5
 Summary: A Python, C, C++ to Roblox Lua compiler
 Home-page: https://github.com/AsynchronousAI/roblox-pyc
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # roblox.pyc
```

### Comparing `roblox-pyc-1.6.6.4rc0/roblox_pyc.egg-info/SOURCES.txt` & `roblox-pyc-1.6.6.5/roblox_pyc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.6.6.4rc0/src/binopdesc.py` & `roblox-pyc-1.6.6.5/src/binopdesc.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.6.6.4rc0/src/colortext.py` & `roblox-pyc-1.6.6.5/src/colortext.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.6.6.4rc0/src/config.py` & `roblox-pyc-1.6.6.5/src/config.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.6.6.4rc0/src/context.py` & `roblox-pyc-1.6.6.5/src/context.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.6.6.4rc0/src/luainit.py` & `roblox-pyc-1.6.6.5/src/luainit.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.6.6.4rc0/src/nodevisitor.py` & `roblox-pyc-1.6.6.5/src/nodevisitor.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.6.6.4rc0/src/pytranslator.py` & `roblox-pyc-1.6.6.5/src/pytranslator.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.6.6.4rc0/src/robloxpy.py` & `roblox-pyc-1.6.6.5/src/robloxpy.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.6.6.4rc0/src/symbolsstack.py` & `roblox-pyc-1.6.6.5/src/symbolsstack.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.6.6.4rc0/src/unaryopdesc.py` & `roblox-pyc-1.6.6.5/src/unaryopdesc.py`

 * *Files identical despite different names*

