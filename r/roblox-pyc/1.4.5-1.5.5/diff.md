# Comparing `tmp/roblox-pyc-1.4.5.tar.gz` & `tmp/roblox-pyc-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roblox-pyc-1.4.5.tar", last modified: Sun Jul  9 05:03:28 2023, max compression
+gzip compressed data, was "roblox-pyc-1.5.5.tar", last modified: Sun Jul  9 05:13:21 2023, max compression
```

## Comparing `roblox-pyc-1.4.5.tar` & `roblox-pyc-1.5.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 aaravs     (501) staff       (20)        0 2023-07-09 05:03:28.570218 roblox-pyc-1.4.5/
--rw-r--r--   0 aaravs     (501) staff       (20)    34525 2023-07-07 21:26:51.000000 roblox-pyc-1.4.5/LICENSE
--rw-r--r--   0 aaravs     (501) staff       (20)       76 2023-07-09 05:03:28.570466 roblox-pyc-1.4.5/PKG-INFO
--rw-r--r--   0 aaravs     (501) staff       (20)     2387 2023-07-09 04:50:22.000000 roblox-pyc-1.4.5/README.md
--rw-r--r--   0 aaravs     (501) staff       (20)       89 2023-07-09 01:34:29.000000 roblox-pyc-1.4.5/pyproject.toml
-drwxr-xr-x   0 aaravs     (501) staff       (20)        0 2023-07-09 05:03:28.520766 roblox-pyc-1.4.5/roblox_pyc.egg-info/
--rw-r--r--   0 aaravs     (501) staff       (20)       76 2023-07-09 05:03:28.000000 roblox-pyc-1.4.5/roblox_pyc.egg-info/PKG-INFO
--rw-r--r--   0 aaravs     (501) staff       (20)      519 2023-07-09 05:03:28.000000 roblox-pyc-1.4.5/roblox_pyc.egg-info/SOURCES.txt
--rw-r--r--   0 aaravs     (501) staff       (20)        1 2023-07-09 05:03:28.000000 roblox-pyc-1.4.5/roblox_pyc.egg-info/dependency_links.txt
--rw-r--r--   0 aaravs     (501) staff       (20)      122 2023-07-09 05:03:28.000000 roblox-pyc-1.4.5/roblox_pyc.egg-info/entry_points.txt
--rw-r--r--   0 aaravs     (501) staff       (20)        4 2023-07-09 05:03:28.000000 roblox-pyc-1.4.5/roblox_pyc.egg-info/top_level.txt
--rw-r--r--   0 aaravs     (501) staff       (20)      260 2023-07-09 05:03:28.571494 roblox-pyc-1.4.5/setup.cfg
--rw-r--r--   0 aaravs     (501) staff       (20)       37 2023-07-09 02:02:48.000000 roblox-pyc-1.4.5/setup.py
-drwxr-xr-x   0 aaravs     (501) staff       (20)        0 2023-07-09 05:03:28.569242 roblox-pyc-1.4.5/src/
--rw-r--r--   0 aaravs     (501) staff       (20)       38 2023-07-07 21:26:51.000000 roblox-pyc-1.4.5/src/__init__.py
--rw-r--r--   0 aaravs     (501) staff       (20)     1464 2023-07-07 21:26:51.000000 roblox-pyc-1.4.5/src/binopdesc.py
--rw-r--r--   0 aaravs     (501) staff       (20)      382 2023-07-07 21:26:51.000000 roblox-pyc-1.4.5/src/boolopdesc.py
--rw-r--r--   0 aaravs     (501) staff       (20)      450 2023-07-07 21:26:51.000000 roblox-pyc-1.4.5/src/cmpopdesc.py
--rw-r--r--   0 aaravs     (501) staff       (20)      800 2023-07-09 03:44:33.000000 roblox-pyc-1.4.5/src/colortext.py
--rw-r--r--   0 aaravs     (501) staff       (20)      790 2023-07-07 21:26:51.000000 roblox-pyc-1.4.5/src/config.py
--rw-r--r--   0 aaravs     (501) staff       (20)     1050 2023-07-07 21:26:51.000000 roblox-pyc-1.4.5/src/context.py
--rw-r--r--   0 aaravs     (501) staff       (20)      835 2023-07-09 04:51:27.000000 roblox-pyc-1.4.5/src/header.py
--rw-r--r--   0 aaravs     (501) staff       (20)      282 2023-07-09 01:58:37.000000 roblox-pyc-1.4.5/src/loopcounter.py
--rw-r--r--   0 aaravs     (501) staff       (20)    21563 2023-07-09 04:51:41.000000 roblox-pyc-1.4.5/src/luainit.py
--rw-r--r--   0 aaravs     (501) staff       (20)      181 2023-07-07 21:26:51.000000 roblox-pyc-1.4.5/src/nameconstdesc.py
--rw-r--r--   0 aaravs     (501) staff       (20)    27684 2023-07-09 01:59:38.000000 roblox-pyc-1.4.5/src/nodevisitor.py
--rw-r--r--   0 aaravs     (501) staff       (20)     5957 2023-07-09 05:02:43.000000 roblox-pyc-1.4.5/src/robloxpy.py
--rw-r--r--   0 aaravs     (501) staff       (20)      642 2023-07-07 21:26:51.000000 roblox-pyc-1.4.5/src/symbolsstack.py
--rw-r--r--   0 aaravs     (501) staff       (20)      157 2023-07-07 21:26:51.000000 roblox-pyc-1.4.5/src/tokenendmode.py
--rw-r--r--   0 aaravs     (501) staff       (20)     1709 2023-07-09 03:36:47.000000 roblox-pyc-1.4.5/src/translator.py
--rw-r--r--   0 aaravs     (501) staff       (20)      567 2023-07-08 14:04:57.000000 roblox-pyc-1.4.5/src/unaryopdesc.py
+drwxr-xr-x   0 aaravs     (501) staff       (20)        0 2023-07-09 05:13:21.185545 roblox-pyc-1.5.5/
+-rw-r--r--   0 aaravs     (501) staff       (20)    34525 2023-07-07 21:26:51.000000 roblox-pyc-1.5.5/LICENSE
+-rw-r--r--   0 aaravs     (501) staff       (20)      124 2023-07-09 05:13:21.185876 roblox-pyc-1.5.5/PKG-INFO
+-rw-r--r--   0 aaravs     (501) staff       (20)     2387 2023-07-09 04:50:22.000000 roblox-pyc-1.5.5/README.md
+-rw-r--r--   0 aaravs     (501) staff       (20)       89 2023-07-09 01:34:29.000000 roblox-pyc-1.5.5/pyproject.toml
+drwxr-xr-x   0 aaravs     (501) staff       (20)        0 2023-07-09 05:13:21.160530 roblox-pyc-1.5.5/roblox_pyc.egg-info/
+-rw-r--r--   0 aaravs     (501) staff       (20)      124 2023-07-09 05:13:21.000000 roblox-pyc-1.5.5/roblox_pyc.egg-info/PKG-INFO
+-rw-r--r--   0 aaravs     (501) staff       (20)      519 2023-07-09 05:13:21.000000 roblox-pyc-1.5.5/roblox_pyc.egg-info/SOURCES.txt
+-rw-r--r--   0 aaravs     (501) staff       (20)        1 2023-07-09 05:13:21.000000 roblox-pyc-1.5.5/roblox_pyc.egg-info/dependency_links.txt
+-rw-r--r--   0 aaravs     (501) staff       (20)      122 2023-07-09 05:13:21.000000 roblox-pyc-1.5.5/roblox_pyc.egg-info/entry_points.txt
+-rw-r--r--   0 aaravs     (501) staff       (20)        4 2023-07-09 05:13:21.000000 roblox-pyc-1.5.5/roblox_pyc.egg-info/top_level.txt
+-rw-r--r--   0 aaravs     (501) staff       (20)      367 2023-07-09 05:13:21.187306 roblox-pyc-1.5.5/setup.cfg
+-rw-r--r--   0 aaravs     (501) staff       (20)       37 2023-07-09 02:02:48.000000 roblox-pyc-1.5.5/setup.py
+drwxr-xr-x   0 aaravs     (501) staff       (20)        0 2023-07-09 05:13:21.184125 roblox-pyc-1.5.5/src/
+-rw-r--r--   0 aaravs     (501) staff       (20)       38 2023-07-07 21:26:51.000000 roblox-pyc-1.5.5/src/__init__.py
+-rw-r--r--   0 aaravs     (501) staff       (20)     1464 2023-07-07 21:26:51.000000 roblox-pyc-1.5.5/src/binopdesc.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      382 2023-07-07 21:26:51.000000 roblox-pyc-1.5.5/src/boolopdesc.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      450 2023-07-07 21:26:51.000000 roblox-pyc-1.5.5/src/cmpopdesc.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      800 2023-07-09 03:44:33.000000 roblox-pyc-1.5.5/src/colortext.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      790 2023-07-07 21:26:51.000000 roblox-pyc-1.5.5/src/config.py
+-rw-r--r--   0 aaravs     (501) staff       (20)     1050 2023-07-07 21:26:51.000000 roblox-pyc-1.5.5/src/context.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      835 2023-07-09 04:51:27.000000 roblox-pyc-1.5.5/src/header.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      282 2023-07-09 01:58:37.000000 roblox-pyc-1.5.5/src/loopcounter.py
+-rw-r--r--   0 aaravs     (501) staff       (20)    21563 2023-07-09 04:51:41.000000 roblox-pyc-1.5.5/src/luainit.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      181 2023-07-07 21:26:51.000000 roblox-pyc-1.5.5/src/nameconstdesc.py
+-rw-r--r--   0 aaravs     (501) staff       (20)    27684 2023-07-09 01:59:38.000000 roblox-pyc-1.5.5/src/nodevisitor.py
+-rw-r--r--   0 aaravs     (501) staff       (20)     5957 2023-07-09 05:02:43.000000 roblox-pyc-1.5.5/src/robloxpy.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      642 2023-07-07 21:26:51.000000 roblox-pyc-1.5.5/src/symbolsstack.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      157 2023-07-07 21:26:51.000000 roblox-pyc-1.5.5/src/tokenendmode.py
+-rw-r--r--   0 aaravs     (501) staff       (20)     1709 2023-07-09 03:36:47.000000 roblox-pyc-1.5.5/src/translator.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      567 2023-07-08 14:04:57.000000 roblox-pyc-1.5.5/src/unaryopdesc.py
```

### Comparing `roblox-pyc-1.4.5/LICENSE` & `roblox-pyc-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.4.5/README.md` & `roblox-pyc-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.4.5/roblox_pyc.egg-info/SOURCES.txt` & `roblox-pyc-1.5.5/roblox_pyc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.4.5/src/binopdesc.py` & `roblox-pyc-1.5.5/src/binopdesc.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.4.5/src/colortext.py` & `roblox-pyc-1.5.5/src/colortext.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.4.5/src/config.py` & `roblox-pyc-1.5.5/src/config.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.4.5/src/context.py` & `roblox-pyc-1.5.5/src/context.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.4.5/src/header.py` & `roblox-pyc-1.5.5/src/header.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.4.5/src/luainit.py` & `roblox-pyc-1.5.5/src/luainit.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.4.5/src/nodevisitor.py` & `roblox-pyc-1.5.5/src/nodevisitor.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.4.5/src/robloxpy.py` & `roblox-pyc-1.5.5/src/robloxpy.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.4.5/src/symbolsstack.py` & `roblox-pyc-1.5.5/src/symbolsstack.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.4.5/src/translator.py` & `roblox-pyc-1.5.5/src/translator.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.4.5/src/unaryopdesc.py` & `roblox-pyc-1.5.5/src/unaryopdesc.py`

 * *Files identical despite different names*

