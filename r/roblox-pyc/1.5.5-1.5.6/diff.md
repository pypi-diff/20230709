# Comparing `tmp/roblox-pyc-1.5.5.tar.gz` & `tmp/roblox-pyc-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roblox-pyc-1.5.5.tar", last modified: Sun Jul  9 05:13:21 2023, max compression
+gzip compressed data, was "roblox-pyc-1.5.6.tar", last modified: Sun Jul  9 15:06:14 2023, max compression
```

## Comparing `roblox-pyc-1.5.5.tar` & `roblox-pyc-1.5.6.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxr-xr-x   0 aaravs     (501) staff       (20)        0 2023-07-09 05:13:21.185545 roblox-pyc-1.5.5/
--rw-r--r--   0 aaravs     (501) staff       (20)    34525 2023-07-07 21:26:51.000000 roblox-pyc-1.5.5/LICENSE
--rw-r--r--   0 aaravs     (501) staff       (20)      124 2023-07-09 05:13:21.185876 roblox-pyc-1.5.5/PKG-INFO
--rw-r--r--   0 aaravs     (501) staff       (20)     2387 2023-07-09 04:50:22.000000 roblox-pyc-1.5.5/README.md
--rw-r--r--   0 aaravs     (501) staff       (20)       89 2023-07-09 01:34:29.000000 roblox-pyc-1.5.5/pyproject.toml
-drwxr-xr-x   0 aaravs     (501) staff       (20)        0 2023-07-09 05:13:21.160530 roblox-pyc-1.5.5/roblox_pyc.egg-info/
--rw-r--r--   0 aaravs     (501) staff       (20)      124 2023-07-09 05:13:21.000000 roblox-pyc-1.5.5/roblox_pyc.egg-info/PKG-INFO
--rw-r--r--   0 aaravs     (501) staff       (20)      519 2023-07-09 05:13:21.000000 roblox-pyc-1.5.5/roblox_pyc.egg-info/SOURCES.txt
--rw-r--r--   0 aaravs     (501) staff       (20)        1 2023-07-09 05:13:21.000000 roblox-pyc-1.5.5/roblox_pyc.egg-info/dependency_links.txt
--rw-r--r--   0 aaravs     (501) staff       (20)      122 2023-07-09 05:13:21.000000 roblox-pyc-1.5.5/roblox_pyc.egg-info/entry_points.txt
--rw-r--r--   0 aaravs     (501) staff       (20)        4 2023-07-09 05:13:21.000000 roblox-pyc-1.5.5/roblox_pyc.egg-info/top_level.txt
--rw-r--r--   0 aaravs     (501) staff       (20)      367 2023-07-09 05:13:21.187306 roblox-pyc-1.5.5/setup.cfg
--rw-r--r--   0 aaravs     (501) staff       (20)       37 2023-07-09 02:02:48.000000 roblox-pyc-1.5.5/setup.py
-drwxr-xr-x   0 aaravs     (501) staff       (20)        0 2023-07-09 05:13:21.184125 roblox-pyc-1.5.5/src/
--rw-r--r--   0 aaravs     (501) staff       (20)       38 2023-07-07 21:26:51.000000 roblox-pyc-1.5.5/src/__init__.py
--rw-r--r--   0 aaravs     (501) staff       (20)     1464 2023-07-07 21:26:51.000000 roblox-pyc-1.5.5/src/binopdesc.py
--rw-r--r--   0 aaravs     (501) staff       (20)      382 2023-07-07 21:26:51.000000 roblox-pyc-1.5.5/src/boolopdesc.py
--rw-r--r--   0 aaravs     (501) staff       (20)      450 2023-07-07 21:26:51.000000 roblox-pyc-1.5.5/src/cmpopdesc.py
--rw-r--r--   0 aaravs     (501) staff       (20)      800 2023-07-09 03:44:33.000000 roblox-pyc-1.5.5/src/colortext.py
--rw-r--r--   0 aaravs     (501) staff       (20)      790 2023-07-07 21:26:51.000000 roblox-pyc-1.5.5/src/config.py
--rw-r--r--   0 aaravs     (501) staff       (20)     1050 2023-07-07 21:26:51.000000 roblox-pyc-1.5.5/src/context.py
--rw-r--r--   0 aaravs     (501) staff       (20)      835 2023-07-09 04:51:27.000000 roblox-pyc-1.5.5/src/header.py
--rw-r--r--   0 aaravs     (501) staff       (20)      282 2023-07-09 01:58:37.000000 roblox-pyc-1.5.5/src/loopcounter.py
--rw-r--r--   0 aaravs     (501) staff       (20)    21563 2023-07-09 04:51:41.000000 roblox-pyc-1.5.5/src/luainit.py
--rw-r--r--   0 aaravs     (501) staff       (20)      181 2023-07-07 21:26:51.000000 roblox-pyc-1.5.5/src/nameconstdesc.py
--rw-r--r--   0 aaravs     (501) staff       (20)    27684 2023-07-09 01:59:38.000000 roblox-pyc-1.5.5/src/nodevisitor.py
--rw-r--r--   0 aaravs     (501) staff       (20)     5957 2023-07-09 05:02:43.000000 roblox-pyc-1.5.5/src/robloxpy.py
--rw-r--r--   0 aaravs     (501) staff       (20)      642 2023-07-07 21:26:51.000000 roblox-pyc-1.5.5/src/symbolsstack.py
--rw-r--r--   0 aaravs     (501) staff       (20)      157 2023-07-07 21:26:51.000000 roblox-pyc-1.5.5/src/tokenendmode.py
--rw-r--r--   0 aaravs     (501) staff       (20)     1709 2023-07-09 03:36:47.000000 roblox-pyc-1.5.5/src/translator.py
--rw-r--r--   0 aaravs     (501) staff       (20)      567 2023-07-08 14:04:57.000000 roblox-pyc-1.5.5/src/unaryopdesc.py
+drwxr-xr-x   0 aaravs     (501) staff       (20)        0 2023-07-09 15:06:14.627478 roblox-pyc-1.5.6/
+-rw-r--r--   0 aaravs     (501) staff       (20)    34525 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6/LICENSE
+-rw-r--r--   0 aaravs     (501) staff       (20)      181 2023-07-09 15:06:14.627771 roblox-pyc-1.5.6/PKG-INFO
+-rw-r--r--   0 aaravs     (501) staff       (20)     2612 2023-07-09 06:19:09.000000 roblox-pyc-1.5.6/README.md
+-rw-r--r--   0 aaravs     (501) staff       (20)       89 2023-07-09 01:34:29.000000 roblox-pyc-1.5.6/pyproject.toml
+drwxr-xr-x   0 aaravs     (501) staff       (20)        0 2023-07-09 15:06:14.604673 roblox-pyc-1.5.6/roblox_pyc.egg-info/
+-rw-r--r--   0 aaravs     (501) staff       (20)      181 2023-07-09 15:06:14.000000 roblox-pyc-1.5.6/roblox_pyc.egg-info/PKG-INFO
+-rw-r--r--   0 aaravs     (501) staff       (20)      565 2023-07-09 15:06:14.000000 roblox-pyc-1.5.6/roblox_pyc.egg-info/SOURCES.txt
+-rw-r--r--   0 aaravs     (501) staff       (20)        1 2023-07-09 15:06:14.000000 roblox-pyc-1.5.6/roblox_pyc.egg-info/dependency_links.txt
+-rw-r--r--   0 aaravs     (501) staff       (20)      122 2023-07-09 15:06:14.000000 roblox-pyc-1.5.6/roblox_pyc.egg-info/entry_points.txt
+-rw-r--r--   0 aaravs     (501) staff       (20)       43 2023-07-09 15:06:14.000000 roblox-pyc-1.5.6/roblox_pyc.egg-info/requires.txt
+-rw-r--r--   0 aaravs     (501) staff       (20)        4 2023-07-09 15:06:14.000000 roblox-pyc-1.5.6/roblox_pyc.egg-info/top_level.txt
+-rw-r--r--   0 aaravs     (501) staff       (20)      260 2023-07-09 15:06:14.628952 roblox-pyc-1.5.6/setup.cfg
+-rw-r--r--   0 aaravs     (501) staff       (20)      334 2023-07-09 15:03:29.000000 roblox-pyc-1.5.6/setup.py
+drwxr-xr-x   0 aaravs     (501) staff       (20)        0 2023-07-09 15:06:14.626453 roblox-pyc-1.5.6/src/
+-rw-r--r--   0 aaravs     (501) staff       (20)       38 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6/src/__init__.py
+-rw-r--r--   0 aaravs     (501) staff       (20)     1464 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6/src/binopdesc.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      382 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6/src/boolopdesc.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      450 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6/src/cmpopdesc.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      800 2023-07-09 03:44:33.000000 roblox-pyc-1.5.6/src/colortext.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      790 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6/src/config.py
+-rw-r--r--   0 aaravs     (501) staff       (20)     1050 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6/src/context.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      647 2023-07-09 14:56:33.000000 roblox-pyc-1.5.6/src/cpAST.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      835 2023-07-09 04:51:27.000000 roblox-pyc-1.5.6/src/header.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      282 2023-07-09 01:58:37.000000 roblox-pyc-1.5.6/src/loopcounter.py
+-rw-r--r--   0 aaravs     (501) staff       (20)    21563 2023-07-09 04:51:41.000000 roblox-pyc-1.5.6/src/luainit.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      181 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6/src/nameconstdesc.py
+-rw-r--r--   0 aaravs     (501) staff       (20)    27684 2023-07-09 01:59:38.000000 roblox-pyc-1.5.6/src/nodevisitor.py
+-rw-r--r--   0 aaravs     (501) staff       (20)     6360 2023-07-09 06:05:53.000000 roblox-pyc-1.5.6/src/robloxpy.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      642 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6/src/symbolsstack.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      157 2023-07-07 21:26:51.000000 roblox-pyc-1.5.6/src/tokenendmode.py
+-rw-r--r--   0 aaravs     (501) staff       (20)     1709 2023-07-09 03:36:47.000000 roblox-pyc-1.5.6/src/translator.py
+-rw-r--r--   0 aaravs     (501) staff       (20)      567 2023-07-08 14:04:57.000000 roblox-pyc-1.5.6/src/unaryopdesc.py
```

### Comparing `roblox-pyc-1.5.5/LICENSE` & `roblox-pyc-1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.5.5/README.md` & `roblox-pyc-1.5.6/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -6,31 +6,31 @@
 Python 3.13 (dev) -> Lua(u)
 
 ## Why did the name get changed to roblox.pyc?
 2 reasons:
 - It's a python compiler, so it should be named .py**c**
 - Eventually I am planning on adding C support, so it would be confusing to have a compiler named roblox.py that supports C.
 
-## Dependencies
-- ``pip3 install --upgrade pyflakes``
-- ``pip3 install flask``
-- ``pip3 install pyyaml``
 
 ## Credits
 - [Highlighter](https://github.com/boatbomber/Highlighter). modified to work with python
 - [TextBoxPlus](https://github.com/boatbomber/TextBoxPlus). uses a modified version with autocomplete
 - [pythonlua](https://github.com/dmitrii-eremin/python-lua). this is heavily modified version with flask implementation and compiler changes.
-
+- [pycparser](https://github.com/eliben/pycparser/). used for c support
   (read licenses in [copyright.txt](/COPYRIGHTS.txt))
+  
+# Python:
 ## Plugin Guide
-### #1 - Clone and start server
+### #1 - Download and start server
 ```
-git clone https://github.com/AsynchronousAI/roblox.py/; cd roblox.py; python3 .
+pip3 install roblox-pyc
+```
+```
+roblox-py p
 ```
-
 > Note: This process will end whenever you restart your computer or close the terminal. We recommend using Replit instead.
 
 If any issues occur here report it in github issues.
 
 ### #2 - Download client
 A download link is in the releases, download the file and place it in your plugins folder. 
 
@@ -43,11 +43,28 @@
 After installing the client open any place, make a new StringValue anywhere named "ROBLOXPY_CONFIG" with its value being the url and then press the roblox.py/Python icon in the plugins tab.
 
 > Note: If you are hosting on a personal computer this step may not be needed because the url is defaulted to localhost:5555
 
 ### #4 Open studio and test
 Open Roblox Studio, and select any location and click the roblox.py/Python icon in the plugins tab. A window for editing the plugin and a new script named "Script.py" should appear in the explorer.
 
-## CLI Coming soon
+## CLI
+### #1 - Download
+```
+pip3 install roblox-pyc
+```
+### #2 - cd to target directory
+```
+cd Desktop/mygame
+```
+When called, for every python script roblox-pyc finds it will make a duplicate in the same path with the same name but a .lua ending and with the python code.
+
+### #2 - start
+```
+roblox-py w
+```
+
+# C:
+coming soon
+# C++:
+coming soon
 
-### Learn more
-Learn more in the devforum post.
```

### Comparing `roblox-pyc-1.5.5/roblox_pyc.egg-info/SOURCES.txt` & `roblox-pyc-1.5.6/roblox_pyc.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 pyproject.toml
 setup.cfg
 setup.py
 roblox_pyc.egg-info/PKG-INFO
 roblox_pyc.egg-info/SOURCES.txt
 roblox_pyc.egg-info/dependency_links.txt
 roblox_pyc.egg-info/entry_points.txt
+roblox_pyc.egg-info/requires.txt
 roblox_pyc.egg-info/top_level.txt
 src/__init__.py
 src/binopdesc.py
 src/boolopdesc.py
 src/cmpopdesc.py
 src/colortext.py
 src/config.py
 src/context.py
+src/cpAST.py
 src/header.py
 src/loopcounter.py
 src/luainit.py
 src/nameconstdesc.py
 src/nodevisitor.py
 src/robloxpy.py
 src/symbolsstack.py
```

### Comparing `roblox-pyc-1.5.5/src/binopdesc.py` & `roblox-pyc-1.5.6/src/binopdesc.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.5.5/src/colortext.py` & `roblox-pyc-1.5.6/src/colortext.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.5.5/src/config.py` & `roblox-pyc-1.5.6/src/config.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.5.5/src/context.py` & `roblox-pyc-1.5.6/src/context.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.5.5/src/header.py` & `roblox-pyc-1.5.6/src/header.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.5.5/src/luainit.py` & `roblox-pyc-1.5.6/src/luainit.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.5.5/src/nodevisitor.py` & `roblox-pyc-1.5.6/src/nodevisitor.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.5.5/src/robloxpy.py` & `roblox-pyc-1.5.6/src/robloxpy.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,17 +71,17 @@
         @param: A L{pyflakes.messages.Message}.
         """
         self.diagnostics.append("2"+str(message))
         self.diagnostics.append('\n')
 
 
 app = Flask(__name__)
-typerapp = typer.Typer()
-typerapp2 = typer.Typer()
-typerapp3 = typer.Typer()
+typerapp = typer.Typer() #py
+typerapp2 = typer.Typer() #c
+typerapp3 = typer.Typer() #cpp
 translator = Translator()
 
 def backwordreplace(s, old, new, occurrence):
   li = s.rsplit(old, occurrence)
   return new.join(li)
 
 @typerapp.command("p", help="Starts a server on port 5555 for the plugin (decreapted).")
@@ -160,15 +160,22 @@
     action = input("")
     if action == "exit":
       exit(0)
     else:
       incli()
   incli()
 
-
+@typerapp2.command("cw", help="Whenever enter is clicked in the terminal, compile all files, if exit is typed, exit the program.")
+def cw():
+  print(red("Version does not support roblox-c"))
+  
+@typerapp3.command("cpw", help="Whenever enter is clicked in the terminal, compile all files, if exit is typed, exit the program.")
+def cpw():
+  print(red("Version does not support roblox-cpp"))
+  
   
 if __name__ == "__main__":
   print(blue("Test mode"))
   mode = input("Select which app to run (1, 2, 3): ")
   
   if mode == "1":
     typerapp()
```

### Comparing `roblox-pyc-1.5.5/src/symbolsstack.py` & `roblox-pyc-1.5.6/src/symbolsstack.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.5.5/src/translator.py` & `roblox-pyc-1.5.6/src/translator.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.5.5/src/unaryopdesc.py` & `roblox-pyc-1.5.6/src/unaryopdesc.py`

 * *Files identical despite different names*

