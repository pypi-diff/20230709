# Comparing `tmp/roblox-pyc-1.5.6.tar.gz` & `tmp/roblox-pyc-1.5.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roblox-pyc-1.5.6.tar", last modified: Sun Jul  9 15:06:14 2023, max compression
+gzip compressed data, was "roblox-pyc-1.5.6.1.tar", last modified: Sun Jul  9 15:35:51 2023, max compression
```

## Comparing `roblox-pyc-1.5.6.tar` & `roblox-pyc-1.5.6.1.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 aaravs     (501) staff       (20)        0 2023-07-09 15:06:14.627478 roblox-pyc-1.5.6/
--rw-r--r--   0 aaravs     (501) staff       (20)    34525 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6/LICENSE
--rw-r--r--   0 aaravs     (501) staff       (20)      181 2023-07-09 15:06:14.627771 roblox-pyc-1.5.6/PKG-INFO
--rw-r--r--   0 aaravs     (501) staff       (20)     2612 2023-07-09 06:19:09.000000 roblox-pyc-1.5.6/README.md
--rw-r--r--   0 aaravs     (501) staff       (20)       89 2023-07-09 01:34:29.000000 roblox-pyc-1.5.6/pyproject.toml
-drwxr-xr-x   0 aaravs     (501) staff       (20)        0 2023-07-09 15:06:14.604673 roblox-pyc-1.5.6/roblox_pyc.egg-info/
--rw-r--r--   0 aaravs     (501) staff       (20)      181 2023-07-09 15:06:14.000000 roblox-pyc-1.5.6/roblox_pyc.egg-info/PKG-INFO
--rw-r--r--   0 aaravs     (501) staff       (20)      565 2023-07-09 15:06:14.000000 roblox-pyc-1.5.6/roblox_pyc.egg-info/SOURCES.txt
--rw-r--r--   0 aaravs     (501) staff       (20)        1 2023-07-09 15:06:14.000000 roblox-pyc-1.5.6/roblox_pyc.egg-info/dependency_links.txt
--rw-r--r--   0 aaravs     (501) staff       (20)      122 2023-07-09 15:06:14.000000 roblox-pyc-1.5.6/roblox_pyc.egg-info/entry_points.txt
--rw-r--r--   0 aaravs     (501) staff       (20)       43 2023-07-09 15:06:14.000000 roblox-pyc-1.5.6/roblox_pyc.egg-info/requires.txt
--rw-r--r--   0 aaravs     (501) staff       (20)        4 2023-07-09 15:06:14.000000 roblox-pyc-1.5.6/roblox_pyc.egg-info/top_level.txt
--rw-r--r--   0 aaravs     (501) staff       (20)      260 2023-07-09 15:06:14.628952 roblox-pyc-1.5.6/setup.cfg
--rw-r--r--   0 aaravs     (501) staff       (20)      334 2023-07-09 15:03:29.000000 roblox-pyc-1.5.6/setup.py
-drwxr-xr-x   0 aaravs     (501) staff       (20)        0 2023-07-09 15:06:14.626453 roblox-pyc-1.5.6/src/
--rw-r--r--   0 aaravs     (501) staff       (20)       38 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6/src/__init__.py
--rw-r--r--   0 aaravs     (501) staff       (20)     1464 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6/src/binopdesc.py
--rw-r--r--   0 aaravs     (501) staff       (20)      382 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6/src/boolopdesc.py
--rw-r--r--   0 aaravs     (501) staff       (20)      450 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6/src/cmpopdesc.py
--rw-r--r--   0 aaravs     (501) staff       (20)      800 2023-07-09 03:44:33.000000 roblox-pyc-1.5.6/src/colortext.py
--rw-r--r--   0 aaravs     (501) staff       (20)      790 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6/src/config.py
--rw-r--r--   0 aaravs     (501) staff       (20)     1050 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6/src/context.py
--rw-r--r--   0 aaravs     (501) staff       (20)      647 2023-07-09 14:56:33.000000 roblox-pyc-1.5.6/src/cpAST.py
--rw-r--r--   0 aaravs     (501) staff       (20)      835 2023-07-09 04:51:27.000000 roblox-pyc-1.5.6/src/header.py
--rw-r--r--   0 aaravs     (501) staff       (20)      282 2023-07-09 01:58:37.000000 roblox-pyc-1.5.6/src/loopcounter.py
--rw-r--r--   0 aaravs     (501) staff       (20)    21563 2023-07-09 04:51:41.000000 roblox-pyc-1.5.6/src/luainit.py
--rw-r--r--   0 aaravs     (501) staff       (20)      181 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6/src/nameconstdesc.py
--rw-r--r--   0 aaravs     (501) staff       (20)    27684 2023-07-09 01:59:38.000000 roblox-pyc-1.5.6/src/nodevisitor.py
--rw-r--r--   0 aaravs     (501) staff       (20)     6360 2023-07-09 06:05:53.000000 roblox-pyc-1.5.6/src/robloxpy.py
--rw-r--r--   0 aaravs     (501) staff       (20)      642 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6/src/symbolsstack.py
--rw-r--r--   0 aaravs     (501) staff       (20)      157 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6/src/tokenendmode.py
--rw-r--r--   0 aaravs     (501) staff       (20)     1709 2023-07-09 03:36:47.000000 roblox-pyc-1.5.6/src/translator.py
--rw-r--r--   0 aaravs     (501) staff       (20)      567 2023-07-08 14:04:57.000000 roblox-pyc-1.5.6/src/unaryopdesc.py
+drwxr-xr-x   0 aaravs     (501) staff       (20)        0 2023-07-09 15:35:51.394789 roblox-pyc-1.5.6.1/
+-rw-r--r--   0 aaravs     (501) staff       (20)    34525 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.1/LICENSE
+-rw-r--r--   0 aaravs     (501) staff       (20)      183 2023-07-09 15:35:51.395004 roblox-pyc-1.5.6.1/PKG-INFO
+-rw-r--r--   0 aaravs     (501) staff       (20)     2612 2023-07-09 06:19:09.000000 roblox-pyc-1.5.6.1/README.md
+-rw-r--r--   0 aaravs     (501) staff       (20)       89 2023-07-09 01:34:29.000000 roblox-pyc-1.5.6.1/pyproject.toml
+drwxr-xr-x   0 aaravs     (501) staff       (20)        0 2023-07-09 15:35:51.368376 roblox-pyc-1.5.6.1/roblox_pyc.egg-info/
+-rw-r--r--   0 aaravs     (501) staff       (20)      183 2023-07-09 15:35:51.000000 roblox-pyc-1.5.6.1/roblox_pyc.egg-info/PKG-INFO
+-rw-r--r--   0 aaravs     (501) staff       (20)      586 2023-07-09 15:35:51.000000 roblox-pyc-1.5.6.1/roblox_pyc.egg-info/SOURCES.txt
+-rw-r--r--   0 aaravs     (501) staff       (20)        1 2023-07-09 15:35:51.000000 roblox-pyc-1.5.6.1/roblox_pyc.egg-info/dependency_links.txt
+-rw-r--r--   0 aaravs     (501) staff       (20)      122 2023-07-09 15:35:51.000000 roblox-pyc-1.5.6.1/roblox_pyc.egg-info/entry_points.txt
+-rw-r--r--   0 aaravs     (501) staff       (20)       43 2023-07-09 15:35:51.000000 roblox-pyc-1.5.6.1/roblox_pyc.egg-info/requires.txt
+-rw-r--r--   0 aaravs     (501) staff       (20)        4 2023-07-09 15:35:51.000000 roblox-pyc-1.5.6.1/roblox_pyc.egg-info/top_level.txt
+-rw-r--r--   0 aaravs     (501) staff       (20)      262 2023-07-09 15:35:51.395721 roblox-pyc-1.5.6.1/setup.cfg
+-rw-r--r--   0 aaravs     (501) staff       (20)      334 2023-07-09 15:03:29.000000 roblox-pyc-1.5.6.1/setup.py
+drwxr-xr-x   0 aaravs     (501) staff       (20)        0 2023-07-09 15:35:51.393836 roblox-pyc-1.5.6.1/src/
+-rw-r--r--   0 aaravs     (501) staff       (20)       38 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.1/src/__init__.py
+-rw-r--r--   0 aaravs     (501) staff       (20)     1464 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.1/src/binopdesc.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      382 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.1/src/boolopdesc.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      450 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.1/src/cmpopdesc.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      800 2023-07-09 03:44:33.000000 roblox-pyc-1.5.6.1/src/colortext.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      790 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.1/src/config.py
+-rw-r--r--   0 aaravs     (501) staff       (20)     1050 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.1/src/context.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      447 2023-07-09 15:13:23.000000 roblox-pyc-1.5.6.1/src/cpAST.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      405 2023-07-09 15:15:08.000000 roblox-pyc-1.5.6.1/src/ctranslator.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      835 2023-07-09 04:51:27.000000 roblox-pyc-1.5.6.1/src/header.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      282 2023-07-09 01:58:37.000000 roblox-pyc-1.5.6.1/src/loopcounter.py
+-rw-r--r--   0 aaravs     (501) staff       (20)    21563 2023-07-09 04:51:41.000000 roblox-pyc-1.5.6.1/src/luainit.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      181 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.1/src/nameconstdesc.py
+-rw-r--r--   0 aaravs     (501) staff       (20)    27684 2023-07-09 01:59:38.000000 roblox-pyc-1.5.6.1/src/nodevisitor.py
+-rw-r--r--   0 aaravs     (501) staff       (20)     1709 2023-07-09 03:36:47.000000 roblox-pyc-1.5.6.1/src/pytranslator.py
+-rw-r--r--   0 aaravs     (501) staff       (20)     8426 2023-07-09 15:34:00.000000 roblox-pyc-1.5.6.1/src/robloxpy.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      642 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.1/src/symbolsstack.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      157 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.1/src/tokenendmode.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      567 2023-07-08 14:04:57.000000 roblox-pyc-1.5.6.1/src/unaryopdesc.py
```

### Comparing `roblox-pyc-1.5.6/LICENSE` & `roblox-pyc-1.5.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.5.6/README.md` & `roblox-pyc-1.5.6.1/README.md`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.5.6/roblox_pyc.egg-info/SOURCES.txt` & `roblox-pyc-1.5.6.1/roblox_pyc.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,18 @@
 src/binopdesc.py
 src/boolopdesc.py
 src/cmpopdesc.py
 src/colortext.py
 src/config.py
 src/context.py
 src/cpAST.py
+src/ctranslator.py
 src/header.py
 src/loopcounter.py
 src/luainit.py
 src/nameconstdesc.py
 src/nodevisitor.py
+src/pytranslator.py
 src/robloxpy.py
 src/symbolsstack.py
 src/tokenendmode.py
-src/translator.py
 src/unaryopdesc.py
```

### Comparing `roblox-pyc-1.5.6/src/binopdesc.py` & `roblox-pyc-1.5.6.1/src/binopdesc.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.5.6/src/colortext.py` & `roblox-pyc-1.5.6.1/src/colortext.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.5.6/src/config.py` & `roblox-pyc-1.5.6.1/src/config.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.5.6/src/context.py` & `roblox-pyc-1.5.6.1/src/context.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.5.6/src/header.py` & `roblox-pyc-1.5.6.1/src/header.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.5.6/src/luainit.py` & `roblox-pyc-1.5.6.1/src/luainit.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.5.6/src/nodevisitor.py` & `roblox-pyc-1.5.6.1/src/nodevisitor.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.5.6/src/robloxpy.py` & `roblox-pyc-1.5.6.1/src/robloxpy.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import os
 from flask import Flask, request
-from .translator import Translator
 from pyflakes import api
 import re
 import sys
 import typer 
-from .colortext import red, green, yellow, blue, magenta, cyan, white, color
+
+
+from . import colortext, pytranslator, ctranslator
 
 class Reporter:
     """
     Formats the results of pyflakes checks to users.
     """
     def __init__(self):
         self.diagnostics = []
@@ -74,15 +75,15 @@
         self.diagnostics.append('\n')
 
 
 app = Flask(__name__)
 typerapp = typer.Typer() #py
 typerapp2 = typer.Typer() #c
 typerapp3 = typer.Typer() #cpp
-translator = Translator()
+translator = pytranslator.Translator()
 
 def backwordreplace(s, old, new, occurrence):
   li = s.rsplit(old, occurrence)
   return new.join(li)
 
 @typerapp.command("p", help="Starts a server on port 5555 for the plugin (decreapted).")
 def p():
@@ -118,15 +119,15 @@
   app.run(
   host='0.0.0.0', 
   port=5555 
   )
 
 @typerapp.command("w", help="Whenever enter is clicked in the terminal, compile all files, if exit is typed, exit the program.")
 def w():
-  print(magenta("roblox-py: Ready to compile ", os.path.join(os.path.dirname(os.path.realpath(__file__)), "test")+" ...\n Type 'exit' to exit, Press enter to compile."))
+  print(colortext.magenta("roblox-py: Ready to compile ", os.path.join(os.path.dirname(os.path.realpath(__file__)), "test")+" ...\n Type 'exit' to exit, Press enter to compile."))
   def incli():
     # NOTE: Since this isnt packaged yet, using this will only check files inside of the test folder
 
     # Get all the files inside of the path, look for all of them which are .py and even check inside of folders. If this is happening in the same directory as the script, do it in the sub directory test
     path = os.getcwd()
 
     for r, d, f in os.walk(path):
@@ -136,49 +137,95 @@
             contents = ""
             header = translator.get_luahead()
             
             try:
               with open(os.path.join(r, file)) as rf:
                 contents = rf.read()  
             except Exception as e:
-              print(red(f"Failed to read {os.path.join(r, file)}!\n\n "+str(e)))
+              print(colortext.red(f"Failed to read {os.path.join(r, file)}!\n\n "+str(e)))
               # do not compile the file if it cannot be read
               continue
             
             try:
               lua_code = header+translator.translate(contents)
-              print(green("roblox-py: Compiled "+os.path.join(r, file)))
+              print(colortext.green("roblox-py: Compiled "+os.path.join(r, file)))
               # get the relative path of the file and replace .py with .lua
               relative_path = backwordreplace(os.path.join(r, file),".py", ".lua", 1)
               if not os.path.exists(relative_path):
                 open(relative_path, "x").close()
               with open(relative_path, "w") as f:
                 f.write(lua_code)
             except Exception as e:
-              print(red(f"Compile Error for {os.path.join(r, file)}!\n\n "+str(e)))
+              print(colortext.red(f"Compile Error for {os.path.join(r, file)}!\n\n "+str(e)))
             
 
     action = input("")
     if action == "exit":
       exit(0)
     else:
       incli()
   incli()
 
 @typerapp2.command("cw", help="Whenever enter is clicked in the terminal, compile all files, if exit is typed, exit the program.")
 def cw():
-  print(red("Version does not support roblox-c"))
+  print(colortext.magenta("roblox-c: Ready to compile ", os.path.join(os.path.dirname(os.path.realpath(__file__)), "test")+" ...\n Type 'exit' to exit, Press enter to compile."))
+  def incli():
+    # NOTE: Since this isnt packaged yet, using this will only check files inside of the test folder
+
+    # Get all the files inside of the path, look for all of them which are .py and even check inside of folders. If this is happening in the same directory as the script, do it in the sub directory test
+    path = os.getcwd()
+
+    for r, d, f in os.walk(path):
+      for file in f:
+          if '.c' in file:
+            # compile the file to a file with the same name and path but .lua
+            try:
+              ctranslator.translate(os.path.join(r, file))
+              print(colortext.green("roblox-c: Compiled "+os.path.join(r, file)))
+            except Exception as e:
+              print(colortext.red(f"Compile Error for {os.path.join(r, file)}!\n\n "+str(e)))
+            
+
+    action = input("")
+    if action == "exit":
+      exit(0)
+    else:
+      incli()
+  incli()
   
 @typerapp3.command("cpw", help="Whenever enter is clicked in the terminal, compile all files, if exit is typed, exit the program.")
 def cpw():
-  print(red("Version does not support roblox-cpp"))
+  print(colortext.magenta("roblox-cpp: Ready to compile ", os.path.join(os.path.dirname(os.path.realpath(__file__)), "test")+" ...\n Type 'exit' to exit, Press enter to compile."))
+  def incli():
+    # NOTE: Since this isnt packaged yet, using this will only check files inside of the test folder
+
+    # Get all the files inside of the path, look for all of them which are .py and even check inside of folders. If this is happening in the same directory as the script, do it in the sub directory test
+    path = os.getcwd()
+
+    for r, d, f in os.walk(path):
+      for file in f:
+          if '.c' in file:
+            # compile the file to a file with the same name and path but .lua
+            try:
+              ctranslator.translate(os.path.join(r, file))
+              print(colortext.green("roblox-cpp: Compiled "+os.path.join(r, file)))
+            except Exception as e:
+              print(colortext.red(f"Compile Error for {os.path.join(r, file)}!\n\n "+str(e)))
+            
+
+    action = input("")
+    if action == "exit":
+      exit(0)
+    else:
+      incli()
+  incli()
   
   
 if __name__ == "__main__":
-  print(blue("Test mode"))
+  print(colortext.blue("Test mode"))
   mode = input("Select which app to run (1, 2, 3): ")
   
   if mode == "1":
     typerapp()
   elif mode == "2":
     typerapp2()
   elif mode == "3":
```

### Comparing `roblox-pyc-1.5.6/src/symbolsstack.py` & `roblox-pyc-1.5.6.1/src/symbolsstack.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.5.6/src/translator.py` & `roblox-pyc-1.5.6.1/src/pytranslator.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.5.6/src/unaryopdesc.py` & `roblox-pyc-1.5.6.1/src/unaryopdesc.py`

 * *Files identical despite different names*

