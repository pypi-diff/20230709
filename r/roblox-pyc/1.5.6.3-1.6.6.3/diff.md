# Comparing `tmp/roblox-pyc-1.5.6.3.tar.gz` & `tmp/roblox-pyc-1.6.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roblox-pyc-1.5.6.3.tar", last modified: Sun Jul  9 15:43:38 2023, max compression
+gzip compressed data, was "roblox-pyc-1.6.6.3.tar", last modified: Sun Jul  9 17:44:42 2023, max compression
```

## Comparing `roblox-pyc-1.5.6.3.tar` & `roblox-pyc-1.6.6.3.tar`

### file list

```diff
@@ -1,34 +1,16 @@
-drwxr-xr-x   0 aaravs     (501) staff       (20)        0 2023-07-09 15:43:38.661939 roblox-pyc-1.5.6.3/
--rw-r--r--   0 aaravs     (501) staff       (20)    34525 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.3/LICENSE
--rw-r--r--   0 aaravs     (501) staff       (20)     2681 2023-07-09 15:43:38.662389 roblox-pyc-1.5.6.3/PKG-INFO
--rw-r--r--   0 aaravs     (501) staff       (20)     2457 2023-07-09 15:43:05.000000 roblox-pyc-1.5.6.3/README.md
--rw-r--r--   0 aaravs     (501) staff       (20)       89 2023-07-09 01:34:29.000000 roblox-pyc-1.5.6.3/pyproject.toml
-drwxr-xr-x   0 aaravs     (501) staff       (20)        0 2023-07-09 15:43:38.632840 roblox-pyc-1.5.6.3/roblox_pyc.egg-info/
--rw-r--r--   0 aaravs     (501) staff       (20)     2681 2023-07-09 15:43:38.000000 roblox-pyc-1.5.6.3/roblox_pyc.egg-info/PKG-INFO
--rw-r--r--   0 aaravs     (501) staff       (20)      586 2023-07-09 15:43:38.000000 roblox-pyc-1.5.6.3/roblox_pyc.egg-info/SOURCES.txt
--rw-r--r--   0 aaravs     (501) staff       (20)        1 2023-07-09 15:43:38.000000 roblox-pyc-1.5.6.3/roblox_pyc.egg-info/dependency_links.txt
--rw-r--r--   0 aaravs     (501) staff       (20)      122 2023-07-09 15:43:38.000000 roblox-pyc-1.5.6.3/roblox_pyc.egg-info/entry_points.txt
--rw-r--r--   0 aaravs     (501) staff       (20)       43 2023-07-09 15:43:38.000000 roblox-pyc-1.5.6.3/roblox_pyc.egg-info/requires.txt
--rw-r--r--   0 aaravs     (501) staff       (20)        4 2023-07-09 15:43:38.000000 roblox-pyc-1.5.6.3/roblox_pyc.egg-info/top_level.txt
--rw-r--r--   0 aaravs     (501) staff       (20)      262 2023-07-09 15:43:38.663881 roblox-pyc-1.5.6.3/setup.cfg
--rw-r--r--   0 aaravs     (501) staff       (20)      440 2023-07-09 15:41:08.000000 roblox-pyc-1.5.6.3/setup.py
-drwxr-xr-x   0 aaravs     (501) staff       (20)        0 2023-07-09 15:43:38.660236 roblox-pyc-1.5.6.3/src/
--rw-r--r--   0 aaravs     (501) staff       (20)       38 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.3/src/__init__.py
--rw-r--r--   0 aaravs     (501) staff       (20)     1464 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.3/src/binopdesc.py
--rw-r--r--   0 aaravs     (501) staff       (20)      382 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.3/src/boolopdesc.py
--rw-r--r--   0 aaravs     (501) staff       (20)      450 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.3/src/cmpopdesc.py
--rw-r--r--   0 aaravs     (501) staff       (20)      800 2023-07-09 03:44:33.000000 roblox-pyc-1.5.6.3/src/colortext.py
--rw-r--r--   0 aaravs     (501) staff       (20)      790 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.3/src/config.py
--rw-r--r--   0 aaravs     (501) staff       (20)     1050 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.3/src/context.py
--rw-r--r--   0 aaravs     (501) staff       (20)      447 2023-07-09 15:13:23.000000 roblox-pyc-1.5.6.3/src/cpAST.py
--rw-r--r--   0 aaravs     (501) staff       (20)      405 2023-07-09 15:15:08.000000 roblox-pyc-1.5.6.3/src/ctranslator.py
--rw-r--r--   0 aaravs     (501) staff       (20)      835 2023-07-09 04:51:27.000000 roblox-pyc-1.5.6.3/src/header.py
--rw-r--r--   0 aaravs     (501) staff       (20)      282 2023-07-09 01:58:37.000000 roblox-pyc-1.5.6.3/src/loopcounter.py
--rw-r--r--   0 aaravs     (501) staff       (20)    21563 2023-07-09 04:51:41.000000 roblox-pyc-1.5.6.3/src/luainit.py
--rw-r--r--   0 aaravs     (501) staff       (20)      181 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.3/src/nameconstdesc.py
--rw-r--r--   0 aaravs     (501) staff       (20)    27684 2023-07-09 01:59:38.000000 roblox-pyc-1.5.6.3/src/nodevisitor.py
--rw-r--r--   0 aaravs     (501) staff       (20)     1709 2023-07-09 03:36:47.000000 roblox-pyc-1.5.6.3/src/pytranslator.py
--rw-r--r--   0 aaravs     (501) staff       (20)     8426 2023-07-09 15:34:00.000000 roblox-pyc-1.5.6.3/src/robloxpy.py
--rw-r--r--   0 aaravs     (501) staff       (20)      642 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.3/src/symbolsstack.py
--rw-r--r--   0 aaravs     (501) staff       (20)      157 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6.3/src/tokenendmode.py
--rw-r--r--   0 aaravs     (501) staff       (20)      567 2023-07-08 14:04:57.000000 roblox-pyc-1.5.6.3/src/unaryopdesc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:44:42.058168 roblox-pyc-1.6.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    34525 2023-07-09 17:44:32.000000 roblox-pyc-1.6.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-09 17:44:42.058168 roblox-pyc-1.6.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-09 17:44:32.000000 roblox-pyc-1.6.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-09 17:44:32.000000 roblox-pyc-1.6.6.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:44:42.058168 roblox-pyc-1.6.6.3/roblox_pyc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-09 17:44:42.000000 roblox-pyc-1.6.6.3/roblox_pyc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-09 17:44:42.000000 roblox-pyc-1.6.6.3/roblox_pyc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 17:44:42.000000 roblox-pyc-1.6.6.3/roblox_pyc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-09 17:44:42.000000 roblox-pyc-1.6.6.3/roblox_pyc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-09 17:44:42.000000 roblox-pyc-1.6.6.3/roblox_pyc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-09 17:44:42.000000 roblox-pyc-1.6.6.3/roblox_pyc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-09 17:44:42.058168 roblox-pyc-1.6.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-09 17:44:32.000000 roblox-pyc-1.6.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:44:42.058168 roblox-pyc-1.6.6.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-07-09 17:44:32.000000 roblox-pyc-1.6.6.3/src/robloxpy.py
```

### Comparing `roblox-pyc-1.5.6.3/LICENSE` & `roblox-pyc-1.6.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.5.6.3/PKG-INFO` & `roblox-pyc-1.6.6.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-Metadata-Version: 2.1
-Name: roblox-pyc
-Version: 1.5.6.3
-Summary: A Python, C, C++ to Roblox Lua compiler
-Home-page: https://github.com/AsynchronousAI/roblox-pyc
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # roblox.pyc
 
 ## [Docs](https://robloxpydocs.vercel.app) | [Docs (github)](https://github.com/AsynchronousAI/robloxpydocs/tree/main) | [Devforum](https://devforum.roblox.com/t/roblox-py-python-luau/2457105?u=dev98799) | [Github](https://github.com/AsynchronousAI/roblox.py) | [Tests/Examples](https://github.com/AsynchronousAI/roblox.py/tree/main/test)
 Python, C, C++ Compiler for Roblox. 
 
 Python 3.13 (dev), C23, C++20 -> Lua(u)
 
+## Changelog:
+- Added C, C++ AST (abstract syntax tree), use the cli and it will output AST
+- Added automatic variable checking, check which builtin variables are needed
+- Added automatic function checking, check which builtin functions are needed
+- Reorganized code
+- Added more tests
+- Cleaned up code
+- Did this changelog
+
+
 ## Why did the name get changed to roblox.pyc?
 2 reasons:
 - It's a python compiler, so it should be named .py**c**
 - C, and C++ support.
 
 
 ## Credits
```

### Comparing `roblox-pyc-1.5.6.3/README.md` & `roblox-pyc-1.6.6.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,32 @@
+Metadata-Version: 2.1
+Name: roblox-pyc
+Version: 1.6.6.3
+Summary: A Python, C, C++ to Roblox Lua compiler
+Home-page: https://github.com/AsynchronousAI/roblox-pyc
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # roblox.pyc
 
 ## [Docs](https://robloxpydocs.vercel.app) | [Docs (github)](https://github.com/AsynchronousAI/robloxpydocs/tree/main) | [Devforum](https://devforum.roblox.com/t/roblox-py-python-luau/2457105?u=dev98799) | [Github](https://github.com/AsynchronousAI/roblox.py) | [Tests/Examples](https://github.com/AsynchronousAI/roblox.py/tree/main/test)
 Python, C, C++ Compiler for Roblox. 
 
 Python 3.13 (dev), C23, C++20 -> Lua(u)
 
+## Changelog:
+- Added C, C++ AST (abstract syntax tree), use the cli and it will output AST
+- Added automatic variable checking, check which builtin variables are needed
+- Added automatic function checking, check which builtin functions are needed
+- Reorganized code
+- Added more tests
+- Cleaned up code
+- Did this changelog
+
+
 ## Why did the name get changed to roblox.pyc?
 2 reasons:
 - It's a python compiler, so it should be named .py**c**
 - C, and C++ support.
 
 
 ## Credits
```

### Comparing `roblox-pyc-1.5.6.3/roblox_pyc.egg-info/PKG-INFO` & `roblox-pyc-1.6.6.3/roblox_pyc.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 Metadata-Version: 2.1
 Name: roblox-pyc
-Version: 1.5.6.3
+Version: 1.6.6.3
 Summary: A Python, C, C++ to Roblox Lua compiler
 Home-page: https://github.com/AsynchronousAI/roblox-pyc
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # roblox.pyc
 
 ## [Docs](https://robloxpydocs.vercel.app) | [Docs (github)](https://github.com/AsynchronousAI/robloxpydocs/tree/main) | [Devforum](https://devforum.roblox.com/t/roblox-py-python-luau/2457105?u=dev98799) | [Github](https://github.com/AsynchronousAI/roblox.py) | [Tests/Examples](https://github.com/AsynchronousAI/roblox.py/tree/main/test)
 Python, C, C++ Compiler for Roblox. 
 
 Python 3.13 (dev), C23, C++20 -> Lua(u)
 
+## Changelog:
+- Added C, C++ AST (abstract syntax tree), use the cli and it will output AST
+- Added automatic variable checking, check which builtin variables are needed
+- Added automatic function checking, check which builtin functions are needed
+- Reorganized code
+- Added more tests
+- Cleaned up code
+- Did this changelog
+
+
 ## Why did the name get changed to roblox.pyc?
 2 reasons:
 - It's a python compiler, so it should be named .py**c**
 - C, and C++ support.
 
 
 ## Credits
```

### Comparing `roblox-pyc-1.5.6.3/src/robloxpy.py` & `roblox-pyc-1.6.6.3/src/robloxpy.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 from flask import Flask, request
 from pyflakes import api
 import re
 import sys
 import typer 
 
 
-from . import colortext, pytranslator, ctranslator
+import compiler.colortext as colortext
+import compiler.pytranslator as pytranslator
+import compiler.ctranslator as ctranslator
 
 class Reporter:
     """
     Formats the results of pyflakes checks to users.
     """
     def __init__(self):
         self.diagnostics = []
@@ -81,29 +83,21 @@
 typerapp3 = typer.Typer() #cpp
 translator = pytranslator.Translator()
 
 def backwordreplace(s, old, new, occurrence):
   li = s.rsplit(old, occurrence)
   return new.join(li)
 
-@typerapp.command("p", help="Starts a server on port 5555 for the plugin (decreapted).")
 def p():
   print("The plugin is decreapted. Please use the CLI alongside a Studio+VSCode sync plugin.")
   @app.route('/', methods=["GET", "POST"]) 
   def base_page():
     code = (request.data).decode()
-    script_name = os.path.realpath(__file__)
-    folder = os.path.dirname(script_name)
-    luainit_path = os.path.join(folder, "src/header.lua")
-    header = ""
-    with open(luainit_path) as file:
-      header = file.read()
-        
     try:
-      lua_code = header+translator.translate(code)
+      lua_code = translator.translate(code)
     except Exception as e:
       return "CompileError!:"+str(e)
 
     return lua_code
 
   @app.route('/err', methods=["GET", "POST"]) 
   def debug():
@@ -117,40 +111,38 @@
   def library():
       return translator.getluainit()
   app.run(
   host='0.0.0.0', 
   port=5555 
   )
 
-@typerapp.command("w", help="Whenever enter is clicked in the terminal, compile all files, if exit is typed, exit the program.")
 def w():
   print(colortext.magenta("roblox-py: Ready to compile ", os.path.join(os.path.dirname(os.path.realpath(__file__)), "test")+" ...\n Type 'exit' to exit, Press enter to compile."))
   def incli():
     # NOTE: Since this isnt packaged yet, using this will only check files inside of the test folder
 
     # Get all the files inside of the path, look for all of them which are .py and even check inside of folders. If this is happening in the same directory as the script, do it in the sub directory test
     path = os.getcwd()
 
     for r, d, f in os.walk(path):
       for file in f:
           if '.py' in file:
             # compile the file to a file with the same name and path but .lua
             contents = ""
-            header = translator.get_luahead()
             
             try:
               with open(os.path.join(r, file)) as rf:
                 contents = rf.read()  
             except Exception as e:
               print(colortext.red(f"Failed to read {os.path.join(r, file)}!\n\n "+str(e)))
               # do not compile the file if it cannot be read
               continue
             
             try:
-              lua_code = header+translator.translate(contents)
+              lua_code = translator.translate(contents)
               print(colortext.green("roblox-py: Compiled "+os.path.join(r, file)))
               # get the relative path of the file and replace .py with .lua
               relative_path = backwordreplace(os.path.join(r, file),".py", ".lua", 1)
               if not os.path.exists(relative_path):
                 open(relative_path, "x").close()
               with open(relative_path, "w") as f:
                 f.write(lua_code)
@@ -161,15 +153,14 @@
     action = input("")
     if action == "exit":
       exit(0)
     else:
       incli()
   incli()
 
-@typerapp2.command("cw", help="Whenever enter is clicked in the terminal, compile all files, if exit is typed, exit the program.")
 def cw():
   print(colortext.magenta("roblox-c: Ready to compile ", os.path.join(os.path.dirname(os.path.realpath(__file__)), "test")+" ...\n Type 'exit' to exit, Press enter to compile."))
   def incli():
     # NOTE: Since this isnt packaged yet, using this will only check files inside of the test folder
 
     # Get all the files inside of the path, look for all of them which are .py and even check inside of folders. If this is happening in the same directory as the script, do it in the sub directory test
     path = os.getcwd()
@@ -188,15 +179,14 @@
     action = input("")
     if action == "exit":
       exit(0)
     else:
       incli()
   incli()
   
-@typerapp3.command("cpw", help="Whenever enter is clicked in the terminal, compile all files, if exit is typed, exit the program.")
 def cpw():
   print(colortext.magenta("roblox-cpp: Ready to compile ", os.path.join(os.path.dirname(os.path.realpath(__file__)), "test")+" ...\n Type 'exit' to exit, Press enter to compile."))
   def incli():
     # NOTE: Since this isnt packaged yet, using this will only check files inside of the test folder
 
     # Get all the files inside of the path, look for all of them which are .py and even check inside of folders. If this is happening in the same directory as the script, do it in the sub directory test
     path = os.getcwd()
@@ -221,12 +211,12 @@
   
   
 if __name__ == "__main__":
   print(colortext.blue("Test mode"))
   mode = input("Select which app to run (1, 2, 3): ")
   
   if mode == "1":
-    typerapp()
+    w()
   elif mode == "2":
-    typerapp2()
+    cw()
   elif mode == "3":
-    typerapp3()
+    cpw()
```

