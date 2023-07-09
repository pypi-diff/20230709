# Comparing `tmp/roblox-pyc-1.5.6.2.tar.gz` & `tmp/roblox-pyc-1.5.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roblox-pyc-1.5.6.2.tar", last modified: Sun Jul  9 15:41:26 2023, max compression
+gzip compressed data, was "roblox-pyc-1.5.6.3.tar", last modified: Sun Jul  9 15:43:38 2023, max compression
```

## Comparing `roblox-pyc-1.5.6.2.tar` & `roblox-pyc-1.5.6.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 aaravs     (501) staff       (20)        0 2023-07-09 15:41:26.200435 roblox-pyc-1.5.6.2/
--rw-r--r--   0 aaravs     (501) staff       (20)    34525 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.2/LICENSE
--rw-r--r--   0 aaravs     (501) staff       (20)     2836 2023-07-09 15:41:26.201165 roblox-pyc-1.5.6.2/PKG-INFO
--rw-r--r--   0 aaravs     (501) staff       (20)     2612 2023-07-09 06:19:09.000000 roblox-pyc-1.5.6.2/README.md
--rw-r--r--   0 aaravs     (501) staff       (20)       89 2023-07-09 01:34:29.000000 roblox-pyc-1.5.6.2/pyproject.toml
-drwxr-xr-x   0 aaravs     (501) staff       (20)        0 2023-07-09 15:41:26.174898 roblox-pyc-1.5.6.2/roblox_pyc.egg-info/
--rw-r--r--   0 aaravs     (501) staff       (20)     2836 2023-07-09 15:41:26.000000 roblox-pyc-1.5.6.2/roblox_pyc.egg-info/PKG-INFO
--rw-r--r--   0 aaravs     (501) staff       (20)      586 2023-07-09 15:41:26.000000 roblox-pyc-1.5.6.2/roblox_pyc.egg-info/SOURCES.txt
--rw-r--r--   0 aaravs     (501) staff       (20)        1 2023-07-09 15:41:26.000000 roblox-pyc-1.5.6.2/roblox_pyc.egg-info/dependency_links.txt
--rw-r--r--   0 aaravs     (501) staff       (20)      122 2023-07-09 15:41:26.000000 roblox-pyc-1.5.6.2/roblox_pyc.egg-info/entry_points.txt
--rw-r--r--   0 aaravs     (501) staff       (20)       43 2023-07-09 15:41:26.000000 roblox-pyc-1.5.6.2/roblox_pyc.egg-info/requires.txt
--rw-r--r--   0 aaravs     (501) staff       (20)        4 2023-07-09 15:41:26.000000 roblox-pyc-1.5.6.2/roblox_pyc.egg-info/top_level.txt
--rw-r--r--   0 aaravs     (501) staff       (20)      262 2023-07-09 15:41:26.202872 roblox-pyc-1.5.6.2/setup.cfg
--rw-r--r--   0 aaravs     (501) staff       (20)      440 2023-07-09 15:41:08.000000 roblox-pyc-1.5.6.2/setup.py
-drwxr-xr-x   0 aaravs     (501) staff       (20)        0 2023-07-09 15:41:26.197998 roblox-pyc-1.5.6.2/src/
--rw-r--r--   0 aaravs     (501) staff       (20)       38 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.2/src/__init__.py
--rw-r--r--   0 aaravs     (501) staff       (20)     1464 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.2/src/binopdesc.py
--rw-r--r--   0 aaravs     (501) staff       (20)      382 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.2/src/boolopdesc.py
--rw-r--r--   0 aaravs     (501) staff       (20)      450 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.2/src/cmpopdesc.py
--rw-r--r--   0 aaravs     (501) staff       (20)      800 2023-07-09 03:44:33.000000 roblox-pyc-1.5.6.2/src/colortext.py
--rw-r--r--   0 aaravs     (501) staff       (20)      790 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.2/src/config.py
--rw-r--r--   0 aaravs     (501) staff       (20)     1050 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.2/src/context.py
--rw-r--r--   0 aaravs     (501) staff       (20)      447 2023-07-09 15:13:23.000000 roblox-pyc-1.5.6.2/src/cpAST.py
--rw-r--r--   0 aaravs     (501) staff       (20)      405 2023-07-09 15:15:08.000000 roblox-pyc-1.5.6.2/src/ctranslator.py
--rw-r--r--   0 aaravs     (501) staff       (20)      835 2023-07-09 04:51:27.000000 roblox-pyc-1.5.6.2/src/header.py
--rw-r--r--   0 aaravs     (501) staff       (20)      282 2023-07-09 01:58:37.000000 roblox-pyc-1.5.6.2/src/loopcounter.py
--rw-r--r--   0 aaravs     (501) staff       (20)    21563 2023-07-09 04:51:41.000000 roblox-pyc-1.5.6.2/src/luainit.py
--rw-r--r--   0 aaravs     (501) staff       (20)      181 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.2/src/nameconstdesc.py
--rw-r--r--   0 aaravs     (501) staff       (20)    27684 2023-07-09 01:59:38.000000 roblox-pyc-1.5.6.2/src/nodevisitor.py
--rw-r--r--   0 aaravs     (501) staff       (20)     1709 2023-07-09 03:36:47.000000 roblox-pyc-1.5.6.2/src/pytranslator.py
--rw-r--r--   0 aaravs     (501) staff       (20)     8426 2023-07-09 15:34:00.000000 roblox-pyc-1.5.6.2/src/robloxpy.py
--rw-r--r--   0 aaravs     (501) staff       (20)      642 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.2/src/symbolsstack.py
--rw-r--r--   0 aaravs     (501) staff       (20)      157 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.2/src/tokenendmode.py
--rw-r--r--   0 aaravs     (501) staff       (20)      567 2023-07-08 14:04:57.000000 roblox-pyc-1.5.6.2/src/unaryopdesc.py
+drwxr-xr-x   0 aaravs     (501) staff       (20)        0 2023-07-09 15:43:38.661939 roblox-pyc-1.5.6.3/
+-rw-r--r--   0 aaravs     (501) staff       (20)    34525 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.3/LICENSE
+-rw-r--r--   0 aaravs     (501) staff       (20)     2681 2023-07-09 15:43:38.662389 roblox-pyc-1.5.6.3/PKG-INFO
+-rw-r--r--   0 aaravs     (501) staff       (20)     2457 2023-07-09 15:43:05.000000 roblox-pyc-1.5.6.3/README.md
+-rw-r--r--   0 aaravs     (501) staff       (20)       89 2023-07-09 01:34:29.000000 roblox-pyc-1.5.6.3/pyproject.toml
+drwxr-xr-x   0 aaravs     (501) staff       (20)        0 2023-07-09 15:43:38.632840 roblox-pyc-1.5.6.3/roblox_pyc.egg-info/
+-rw-r--r--   0 aaravs     (501) staff       (20)     2681 2023-07-09 15:43:38.000000 roblox-pyc-1.5.6.3/roblox_pyc.egg-info/PKG-INFO
+-rw-r--r--   0 aaravs     (501) staff       (20)      586 2023-07-09 15:43:38.000000 roblox-pyc-1.5.6.3/roblox_pyc.egg-info/SOURCES.txt
+-rw-r--r--   0 aaravs     (501) staff       (20)        1 2023-07-09 15:43:38.000000 roblox-pyc-1.5.6.3/roblox_pyc.egg-info/dependency_links.txt
+-rw-r--r--   0 aaravs     (501) staff       (20)      122 2023-07-09 15:43:38.000000 roblox-pyc-1.5.6.3/roblox_pyc.egg-info/entry_points.txt
+-rw-r--r--   0 aaravs     (501) staff       (20)       43 2023-07-09 15:43:38.000000 roblox-pyc-1.5.6.3/roblox_pyc.egg-info/requires.txt
+-rw-r--r--   0 aaravs     (501) staff       (20)        4 2023-07-09 15:43:38.000000 roblox-pyc-1.5.6.3/roblox_pyc.egg-info/top_level.txt
+-rw-r--r--   0 aaravs     (501) staff       (20)      262 2023-07-09 15:43:38.663881 roblox-pyc-1.5.6.3/setup.cfg
+-rw-r--r--   0 aaravs     (501) staff       (20)      440 2023-07-09 15:41:08.000000 roblox-pyc-1.5.6.3/setup.py
+drwxr-xr-x   0 aaravs     (501) staff       (20)        0 2023-07-09 15:43:38.660236 roblox-pyc-1.5.6.3/src/
+-rw-r--r--   0 aaravs     (501) staff       (20)       38 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.3/src/__init__.py
+-rw-r--r--   0 aaravs     (501) staff       (20)     1464 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.3/src/binopdesc.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      382 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.3/src/boolopdesc.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      450 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.3/src/cmpopdesc.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      800 2023-07-09 03:44:33.000000 roblox-pyc-1.5.6.3/src/colortext.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      790 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.3/src/config.py
+-rw-r--r--   0 aaravs     (501) staff       (20)     1050 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.3/src/context.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      447 2023-07-09 15:13:23.000000 roblox-pyc-1.5.6.3/src/cpAST.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      405 2023-07-09 15:15:08.000000 roblox-pyc-1.5.6.3/src/ctranslator.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      835 2023-07-09 04:51:27.000000 roblox-pyc-1.5.6.3/src/header.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      282 2023-07-09 01:58:37.000000 roblox-pyc-1.5.6.3/src/loopcounter.py
+-rw-r--r--   0 aaravs     (501) staff       (20)    21563 2023-07-09 04:51:41.000000 roblox-pyc-1.5.6.3/src/luainit.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      181 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.3/src/nameconstdesc.py
+-rw-r--r--   0 aaravs     (501) staff       (20)    27684 2023-07-09 01:59:38.000000 roblox-pyc-1.5.6.3/src/nodevisitor.py
+-rw-r--r--   0 aaravs     (501) staff       (20)     1709 2023-07-09 03:36:47.000000 roblox-pyc-1.5.6.3/src/pytranslator.py
+-rw-r--r--   0 aaravs     (501) staff       (20)     8426 2023-07-09 15:34:00.000000 roblox-pyc-1.5.6.3/src/robloxpy.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      642 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.3/src/symbolsstack.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      157 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.3/src/tokenendmode.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      567 2023-07-08 14:04:57.000000 roblox-pyc-1.5.6.3/src/unaryopdesc.py
```

### Comparing `roblox-pyc-1.5.6.2/LICENSE` & `roblox-pyc-1.5.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.5.6.2/PKG-INFO` & `roblox-pyc-1.5.6.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,24 @@
-Metadata-Version: 2.1
-Name: roblox-pyc
-Version: 1.5.6.2
-Summary: A Python, C, C++ to Roblox Lua compiler
-Home-page: https://github.com/AsynchronousAI/roblox-pyc
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # roblox.pyc
 
 ## [Docs](https://robloxpydocs.vercel.app) | [Docs (github)](https://github.com/AsynchronousAI/robloxpydocs/tree/main) | [Devforum](https://devforum.roblox.com/t/roblox-py-python-luau/2457105?u=dev98799) | [Github](https://github.com/AsynchronousAI/roblox.py) | [Tests/Examples](https://github.com/AsynchronousAI/roblox.py/tree/main/test)
-Python compiler for Roblox. 
+Python, C, C++ Compiler for Roblox. 
 
-Python 3.13 (dev) -> Lua(u)
+Python 3.13 (dev), C23, C++20 -> Lua(u)
 
 ## Why did the name get changed to roblox.pyc?
 2 reasons:
 - It's a python compiler, so it should be named .py**c**
-- Eventually I am planning on adding C support, so it would be confusing to have a compiler named roblox.py that supports C.
+- C, and C++ support.
 
 
 ## Credits
 - [Highlighter](https://github.com/boatbomber/Highlighter). modified to work with python
 - [TextBoxPlus](https://github.com/boatbomber/TextBoxPlus). uses a modified version with autocomplete
 - [pythonlua](https://github.com/dmitrii-eremin/python-lua). this is heavily modified version with flask implementation and compiler changes.
-- [pycparser](https://github.com/eliben/pycparser/). used for c support
   (read licenses in [copyright.txt](/COPYRIGHTS.txt))
   
 # Python:
 ## Plugin Guide
 ### #1 - Download and start server
 ```
 pip3 install roblox-pyc
```

### Comparing `roblox-pyc-1.5.6.2/README.md` & `roblox-pyc-1.5.6.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,32 @@
+Metadata-Version: 2.1
+Name: roblox-pyc
+Version: 1.5.6.3
+Summary: A Python, C, C++ to Roblox Lua compiler
+Home-page: https://github.com/AsynchronousAI/roblox-pyc
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # roblox.pyc
 
 ## [Docs](https://robloxpydocs.vercel.app) | [Docs (github)](https://github.com/AsynchronousAI/robloxpydocs/tree/main) | [Devforum](https://devforum.roblox.com/t/roblox-py-python-luau/2457105?u=dev98799) | [Github](https://github.com/AsynchronousAI/roblox.py) | [Tests/Examples](https://github.com/AsynchronousAI/roblox.py/tree/main/test)
-Python compiler for Roblox. 
+Python, C, C++ Compiler for Roblox. 
 
-Python 3.13 (dev) -> Lua(u)
+Python 3.13 (dev), C23, C++20 -> Lua(u)
 
 ## Why did the name get changed to roblox.pyc?
 2 reasons:
 - It's a python compiler, so it should be named .py**c**
-- Eventually I am planning on adding C support, so it would be confusing to have a compiler named roblox.py that supports C.
+- C, and C++ support.
 
 
 ## Credits
 - [Highlighter](https://github.com/boatbomber/Highlighter). modified to work with python
 - [TextBoxPlus](https://github.com/boatbomber/TextBoxPlus). uses a modified version with autocomplete
 - [pythonlua](https://github.com/dmitrii-eremin/python-lua). this is heavily modified version with flask implementation and compiler changes.
-- [pycparser](https://github.com/eliben/pycparser/). used for c support
   (read licenses in [copyright.txt](/COPYRIGHTS.txt))
   
 # Python:
 ## Plugin Guide
 ### #1 - Download and start server
 ```
 pip3 install roblox-pyc
```

### Comparing `roblox-pyc-1.5.6.2/roblox_pyc.egg-info/PKG-INFO` & `roblox-pyc-1.5.6.3/roblox_pyc.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: roblox-pyc
-Version: 1.5.6.2
+Version: 1.5.6.3
 Summary: A Python, C, C++ to Roblox Lua compiler
 Home-page: https://github.com/AsynchronousAI/roblox-pyc
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # roblox.pyc
 
 ## [Docs](https://robloxpydocs.vercel.app) | [Docs (github)](https://github.com/AsynchronousAI/robloxpydocs/tree/main) | [Devforum](https://devforum.roblox.com/t/roblox-py-python-luau/2457105?u=dev98799) | [Github](https://github.com/AsynchronousAI/roblox.py) | [Tests/Examples](https://github.com/AsynchronousAI/roblox.py/tree/main/test)
-Python compiler for Roblox. 
+Python, C, C++ Compiler for Roblox. 
 
-Python 3.13 (dev) -> Lua(u)
+Python 3.13 (dev), C23, C++20 -> Lua(u)
 
 ## Why did the name get changed to roblox.pyc?
 2 reasons:
 - It's a python compiler, so it should be named .py**c**
-- Eventually I am planning on adding C support, so it would be confusing to have a compiler named roblox.py that supports C.
+- C, and C++ support.
 
 
 ## Credits
 - [Highlighter](https://github.com/boatbomber/Highlighter). modified to work with python
 - [TextBoxPlus](https://github.com/boatbomber/TextBoxPlus). uses a modified version with autocomplete
 - [pythonlua](https://github.com/dmitrii-eremin/python-lua). this is heavily modified version with flask implementation and compiler changes.
-- [pycparser](https://github.com/eliben/pycparser/). used for c support
   (read licenses in [copyright.txt](/COPYRIGHTS.txt))
   
 # Python:
 ## Plugin Guide
 ### #1 - Download and start server
 ```
 pip3 install roblox-pyc
```

### Comparing `roblox-pyc-1.5.6.2/roblox_pyc.egg-info/SOURCES.txt` & `roblox-pyc-1.5.6.3/roblox_pyc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.5.6.2/src/binopdesc.py` & `roblox-pyc-1.5.6.3/src/binopdesc.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.5.6.2/src/colortext.py` & `roblox-pyc-1.5.6.3/src/colortext.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.5.6.2/src/config.py` & `roblox-pyc-1.5.6.3/src/config.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.5.6.2/src/context.py` & `roblox-pyc-1.5.6.3/src/context.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.5.6.2/src/header.py` & `roblox-pyc-1.5.6.3/src/header.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.5.6.2/src/luainit.py` & `roblox-pyc-1.5.6.3/src/luainit.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.5.6.2/src/nodevisitor.py` & `roblox-pyc-1.5.6.3/src/nodevisitor.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.5.6.2/src/pytranslator.py` & `roblox-pyc-1.5.6.3/src/pytranslator.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.5.6.2/src/robloxpy.py` & `roblox-pyc-1.5.6.3/src/robloxpy.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.5.6.2/src/symbolsstack.py` & `roblox-pyc-1.5.6.3/src/symbolsstack.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.5.6.2/src/unaryopdesc.py` & `roblox-pyc-1.5.6.3/src/unaryopdesc.py`

 * *Files identical despite different names*

