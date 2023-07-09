# Comparing `tmp/tscratchapiget-0.3.8.tar.gz` & `tmp/tscratchapiget-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tscratchapiget-0.3.8.tar", last modified: Sat May 27 09:05:33 2023, max compression
+gzip compressed data, was "tscratchapiget-0.4.0.tar", last modified: Sun Jul  9 05:06:27 2023, max compression
```

## Comparing `tscratchapiget-0.3.8.tar` & `tscratchapiget-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 09:05:33.237279 tscratchapiget-0.3.8/
--rw-rw-rw-   0        0        0     1075 2023-05-21 08:00:32.000000 tscratchapiget-0.3.8/LICENSE
--rw-rw-rw-   0        0        0     4957 2023-05-27 09:05:33.234218 tscratchapiget-0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     3120 2023-05-27 08:59:31.000000 tscratchapiget-0.3.8/README.md
--rw-rw-rw-   0        0        0      639 2023-05-27 08:59:31.000000 tscratchapiget-0.3.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-27 09:05:33.237879 tscratchapiget-0.3.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-27 09:05:33.123844 tscratchapiget-0.3.8/src/
-drwxrwxrwx   0        0        0        0 2023-05-27 09:05:33.187005 tscratchapiget-0.3.8/src/tscratchapiget/
--rw-rw-rw-   0        0        0        0 2023-05-21 04:30:30.000000 tscratchapiget-0.3.8/src/tscratchapiget/__init__.py
--rw-rw-rw-   0        0        0     2303 2023-05-27 08:47:30.000000 tscratchapiget-0.3.8/src/tscratchapiget/project.py
--rw-rw-rw-   0        0        0     2405 2023-05-26 14:21:43.000000 tscratchapiget-0.3.8/src/tscratchapiget/user.py
-drwxrwxrwx   0        0        0        0 2023-05-27 09:05:33.213857 tscratchapiget-0.3.8/src/tscratchapiget.egg-info/
--rw-rw-rw-   0        0        0     4957 2023-05-27 09:05:33.000000 tscratchapiget-0.3.8/src/tscratchapiget.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-05-27 09:05:33.000000 tscratchapiget-0.3.8/src/tscratchapiget.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 09:05:33.000000 tscratchapiget-0.3.8/src/tscratchapiget.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-27 09:05:33.000000 tscratchapiget-0.3.8/src/tscratchapiget.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-27 09:05:33.224116 tscratchapiget-0.3.8/tests/
--rw-rw-rw-   0        0        0       42 2023-05-27 08:47:30.000000 tscratchapiget-0.3.8/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-07-09 05:06:27.246824 tscratchapiget-0.4.0/
+-rw-rw-rw-   0        0        0     1075 2023-05-21 08:00:32.000000 tscratchapiget-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0     5323 2023-07-09 05:06:27.238781 tscratchapiget-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3476 2023-07-09 05:04:42.000000 tscratchapiget-0.4.0/README.md
+-rw-rw-rw-   0        0        0      639 2023-07-09 05:04:42.000000 tscratchapiget-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-09 05:06:27.246824 tscratchapiget-0.4.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-09 05:06:27.150723 tscratchapiget-0.4.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-09 05:06:27.206779 tscratchapiget-0.4.0/src/tscratchapiget/
+-rw-rw-rw-   0        0        0        0 2023-07-09 02:53:38.000000 tscratchapiget-0.4.0/src/tscratchapiget/__init__.py
+-rw-rw-rw-   0        0        0      102 2023-07-09 05:04:42.000000 tscratchapiget-0.4.0/src/tscratchapiget/all.py
+-rw-rw-rw-   0        0        0     2633 2023-07-09 03:42:35.000000 tscratchapiget-0.4.0/src/tscratchapiget/project.py
+-rw-rw-rw-   0        0        0      614 2023-07-09 03:42:35.000000 tscratchapiget-0.4.0/src/tscratchapiget/studio.py
+-rw-rw-rw-   0        0        0     3920 2023-07-09 03:20:58.000000 tscratchapiget-0.4.0/src/tscratchapiget/user.py
+drwxrwxrwx   0        0        0        0 2023-07-09 05:06:27.230856 tscratchapiget-0.4.0/src/tscratchapiget.egg-info/
+-rw-rw-rw-   0        0        0     5323 2023-07-09 05:06:27.000000 tscratchapiget-0.4.0/src/tscratchapiget.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-07-09 05:06:27.000000 tscratchapiget-0.4.0/src/tscratchapiget.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 05:06:27.000000 tscratchapiget-0.4.0/src/tscratchapiget.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-09 05:06:27.000000 tscratchapiget-0.4.0/src/tscratchapiget.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-09 05:06:27.238781 tscratchapiget-0.4.0/tests/
+-rw-rw-rw-   0        0        0      111 2023-07-09 03:41:40.000000 tscratchapiget-0.4.0/tests/test.py
```

### Comparing `tscratchapiget-0.3.8/LICENSE` & `tscratchapiget-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tscratchapiget-0.3.8/PKG-INFO` & `tscratchapiget-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tscratchapiget
-Version: 0.3.8
+Version: 0.4.0
 Summary: A library can get scratch api
 Author-email: Tony <tonyvu4913@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Scratch_Tony_14261
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,33 +36,43 @@
 
 This project gets the scratch api. Everything in this project code by me (except some needed library). Big credit to TimMcCool(Scratcher) for example codes. (This project is not related to TimMcCool)<br>
 Install: `pip install tscratchapiget`<br>
 Change log: https://github.com/Tony14261/tscratchapiget/blob/main/changelog.md<br>
 Report bugs or request new features here: https://github.com/Tony14261/tscratchapiget/issues<br>
 Contact me (Discord): Tony14261#2089<br>
 <br>
-**Functions**<br>
-    **User features(v0.2.7)(Updated commands in v0.3.0)** (New commands are at the top):<br>
-        Note: Remeber to ```from tscratchapiget import user```<br>
-        - Get if a username exists  ```exists([username])```     EX: ```user.exists('Scratch_Tony_14261')``` if yes: Return 'User exists'     if not: Return 'User does not exist'<br>
-        - Get a user unread-message-count ```message_count('[user]')```     EX: ```user.message_count('TimMcCool')```<br>
-        - Get a user id ```id('[user]')```     EX: ```user.id('griffpatch')```<br>
-        - Get if a user is a scratchteam ```scratchteam('[user]')```     EX: ```user.scratchteam('ScratchCat')``` #Return 'True'<br>
-        - Get user join date ```join('[user]')```     EX: ```user.join('Will_Wam')```#Return '2013-11-25T19:52:29.000Z'<br>
-        - Get a user pfp(link) ```pfp_link('[user]')```     EX: ```user.pfp_link('Scratch_Tony_14261')```          +Bonus Feature: Open that pfp link in browser. Change that to ```pfp_link_open('[Username]')```<br>
-        - Get user About-Me section ```aboutme('[user]')``` EX: ```user.aboutme('WazzoTV')```<br>
-        - Get user What-I'm-Working-On section ```wiwo('[username]')```     EX: ```user.wiwo('ceebee')```<br>
-        - Get user country ```country(['user]')```     EX: ```user.country(['')```<br>
-        - Get user follower count ```followers('[user]')```     Ex: ```user.followers('sharkyshar')```<br>
-        - Get user following count ```following('[user]')```     EX: ```user.followers('atomicmagicnumber')```<br>
-        <br>
-    **Project features(v0.3.6)**<br>
-        Note: Remember to ```from tscratchapiget import project```<br>
-              ONLY FILL IN [PROJECT ID] NOT A FULL LINK<br>
-        - Get a project title ```title('[Project_ID]')```     EX: ```project.title('105500895')```<br>
-        - Get a project description ```description('[Project_ID]')```     EX: ```project.description('105500895')```<br>
-        - Get a project views ```views('[Project_ID]')```     EX: ```project.views('105500895')```<br>
-        - Get a project loves ```loves('[Project_ID]')```     EX: ```project.loves('105500895')```<br>
-        - Get a project favorites ```favorites('[Project_ID]')```    EX: ```project.favorites('105500895')```<br>
-        - Get a project remixes ```remixes('[Project_ID]')```     EX:   ```project.remixes('105500895')```<br>
-        - Get if a project exists ```exists('[Project_ID]')```     EX: ```project.exists('105500895')``` This check returns to your terminal<br>
-        - Open a project in a web browser ```open('[Project_ID]')```     EX: ```project.open('105500895')```<br>
+
+**New feature**(not tested): Tired of importing every single feature? Now, you can ```from tscratchapiget import all```. It will import everything for you.
+
+
+**User features(v0.2.7)(Updated commands in v0.3.0)** (New commands are at the top):<br>
+    Note: Remeber to ```from tscratchapiget import user```<br>
+    - Get if a username exists  ```exists([username])```     EX: ```user.exists('Scratch_Tony_14261')``` if yes: Return 'User exists'     if not: Return 'User does not exist'<br>
+    - Get a user unread-message-count ```message_count('[user]')```     EX: ```user.message_count('TimMcCool')```<br>
+    - Get a user id ```id('[user]')```     EX: ```user.id('griffpatch')```<br>
+    - Get if a user is a scratchteam ```scratchteam('[user]')```     EX: ```user.scratchteam('ScratchCat')``` #Return 'True'<br>
+    - Get user join date ```join('[user]')```     EX: ```user.join('Will_Wam')```#Return '2013-11-25T19:52:29.000Z'<br>
+    - Get a user pfp(link) ```pfp_link('[user]')```     EX: ```user.pfp_link('Scratch_Tony_14261')```          +Bonus Feature: Open that pfp link in browser. Change that to ```pfp_link_open('[Username]')```<br>
+    - Get user About-Me section ```aboutme('[user]')``` EX: ```user.aboutme('WazzoTV')```<br>
+    - Get user What-I'm-Working-On section ```wiwo('[username]')```     EX: ```user.wiwo('ceebee')```<br>
+    - Get user country ```country(['user]')```     EX: ```user.country(['')```<br>
+    - Get user follower count ```followers('[user]')```     Ex: ```user.followers('sharkyshar')```<br>
+    - Get user following count ```following('[user]')```     EX: ```user.followers('atomicmagicnumber')```<br>
+    <br>
+**Project features(v0.3.6)**<br>
+    Note: Remember to ```from tscratchapiget import project```<br>
+    ONLY FILL IN PROJECT ID NOT A FULL LINK<br>
+    - Get a project title ```title('[Project_ID]')```     EX: ```project.title('105500895')```<br>
+    - Get a project description ```description('[Project_ID]')```     EX: ```project.description('105500895')```<br>
+    - Get a project views ```views('[Project_ID]')```     EX: ```project.views('105500895')```<br>
+    - Get a project loves ```loves('[Project_ID]')```     EX: ```project.loves('105500895')```<br>
+    - Get a project favorites ```favorites('[Project_ID]')```    EX: ```project.favorites('105500895')```<br>
+    - Get a project remixes ```remixes('[Project_ID]')```     EX:   ```project.remixes('105500895')```<br>
+    - Get if a project exists ```exists('[Project_ID]')```     EX: ```project.exists('105500895')``` This check returns to your terminal<br>
+    - Open a project in a web browser ```open('[Project_ID]')```     EX: ```project.open('105500895')```<br>
+    <br>
+**Studio features(v0.4.1)**<br>
+    Note: Remeber to import all from tscratchapiget<br>
+    Fill in the [Studio ID] with the ID of a studio<br>
+    - Get a studio title ```studio.title("[Studio ID]")```<br>
+    - Get a studio description ```studio.description("[Studio ID]")```<br>
+    More comming **very soon**!
```

### Comparing `tscratchapiget-0.3.8/README.md` & `tscratchapiget-0.4.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,42 @@
 This project gets the scratch api. Everything in this project code by me (except some needed library). Big credit to TimMcCool(Scratcher) for example codes. (This project is not related to TimMcCool)<br>
 Install: `pip install tscratchapiget`<br>
 Change log: https://github.com/Tony14261/tscratchapiget/blob/main/changelog.md<br>
 Report bugs or request new features here: https://github.com/Tony14261/tscratchapiget/issues<br>
 Contact me (Discord): Tony14261#2089<br>
 <br>
-**Functions**<br>
-    **User features(v0.2.7)(Updated commands in v0.3.0)** (New commands are at the top):<br>
-        Note: Remeber to ```from tscratchapiget import user```<br>
-        - Get if a username exists  ```exists([username])```     EX: ```user.exists('Scratch_Tony_14261')``` if yes: Return 'User exists'     if not: Return 'User does not exist'<br>
-        - Get a user unread-message-count ```message_count('[user]')```     EX: ```user.message_count('TimMcCool')```<br>
-        - Get a user id ```id('[user]')```     EX: ```user.id('griffpatch')```<br>
-        - Get if a user is a scratchteam ```scratchteam('[user]')```     EX: ```user.scratchteam('ScratchCat')``` #Return 'True'<br>
-        - Get user join date ```join('[user]')```     EX: ```user.join('Will_Wam')```#Return '2013-11-25T19:52:29.000Z'<br>
-        - Get a user pfp(link) ```pfp_link('[user]')```     EX: ```user.pfp_link('Scratch_Tony_14261')```          +Bonus Feature: Open that pfp link in browser. Change that to ```pfp_link_open('[Username]')```<br>
-        - Get user About-Me section ```aboutme('[user]')``` EX: ```user.aboutme('WazzoTV')```<br>
-        - Get user What-I'm-Working-On section ```wiwo('[username]')```     EX: ```user.wiwo('ceebee')```<br>
-        - Get user country ```country(['user]')```     EX: ```user.country(['')```<br>
-        - Get user follower count ```followers('[user]')```     Ex: ```user.followers('sharkyshar')```<br>
-        - Get user following count ```following('[user]')```     EX: ```user.followers('atomicmagicnumber')```<br>
-        <br>
-    **Project features(v0.3.6)**<br>
-        Note: Remember to ```from tscratchapiget import project```<br>
-              ONLY FILL IN [PROJECT ID] NOT A FULL LINK<br>
-        - Get a project title ```title('[Project_ID]')```     EX: ```project.title('105500895')```<br>
-        - Get a project description ```description('[Project_ID]')```     EX: ```project.description('105500895')```<br>
-        - Get a project views ```views('[Project_ID]')```     EX: ```project.views('105500895')```<br>
-        - Get a project loves ```loves('[Project_ID]')```     EX: ```project.loves('105500895')```<br>
-        - Get a project favorites ```favorites('[Project_ID]')```    EX: ```project.favorites('105500895')```<br>
-        - Get a project remixes ```remixes('[Project_ID]')```     EX:   ```project.remixes('105500895')```<br>
-        - Get if a project exists ```exists('[Project_ID]')```     EX: ```project.exists('105500895')``` This check returns to your terminal<br>
-        - Open a project in a web browser ```open('[Project_ID]')```     EX: ```project.open('105500895')```<br>
+
+**New feature**(not tested): Tired of importing every single feature? Now, you can ```from tscratchapiget import all```. It will import everything for you.
+
+
+**User features(v0.2.7)(Updated commands in v0.3.0)** (New commands are at the top):<br>
+    Note: Remeber to ```from tscratchapiget import user```<br>
+    - Get if a username exists  ```exists([username])```     EX: ```user.exists('Scratch_Tony_14261')``` if yes: Return 'User exists'     if not: Return 'User does not exist'<br>
+    - Get a user unread-message-count ```message_count('[user]')```     EX: ```user.message_count('TimMcCool')```<br>
+    - Get a user id ```id('[user]')```     EX: ```user.id('griffpatch')```<br>
+    - Get if a user is a scratchteam ```scratchteam('[user]')```     EX: ```user.scratchteam('ScratchCat')``` #Return 'True'<br>
+    - Get user join date ```join('[user]')```     EX: ```user.join('Will_Wam')```#Return '2013-11-25T19:52:29.000Z'<br>
+    - Get a user pfp(link) ```pfp_link('[user]')```     EX: ```user.pfp_link('Scratch_Tony_14261')```          +Bonus Feature: Open that pfp link in browser. Change that to ```pfp_link_open('[Username]')```<br>
+    - Get user About-Me section ```aboutme('[user]')``` EX: ```user.aboutme('WazzoTV')```<br>
+    - Get user What-I'm-Working-On section ```wiwo('[username]')```     EX: ```user.wiwo('ceebee')```<br>
+    - Get user country ```country(['user]')```     EX: ```user.country(['')```<br>
+    - Get user follower count ```followers('[user]')```     Ex: ```user.followers('sharkyshar')```<br>
+    - Get user following count ```following('[user]')```     EX: ```user.followers('atomicmagicnumber')```<br>
+    <br>
+**Project features(v0.3.6)**<br>
+    Note: Remember to ```from tscratchapiget import project```<br>
+    ONLY FILL IN PROJECT ID NOT A FULL LINK<br>
+    - Get a project title ```title('[Project_ID]')```     EX: ```project.title('105500895')```<br>
+    - Get a project description ```description('[Project_ID]')```     EX: ```project.description('105500895')```<br>
+    - Get a project views ```views('[Project_ID]')```     EX: ```project.views('105500895')```<br>
+    - Get a project loves ```loves('[Project_ID]')```     EX: ```project.loves('105500895')```<br>
+    - Get a project favorites ```favorites('[Project_ID]')```    EX: ```project.favorites('105500895')```<br>
+    - Get a project remixes ```remixes('[Project_ID]')```     EX:   ```project.remixes('105500895')```<br>
+    - Get if a project exists ```exists('[Project_ID]')```     EX: ```project.exists('105500895')``` This check returns to your terminal<br>
+    - Open a project in a web browser ```open('[Project_ID]')```     EX: ```project.open('105500895')```<br>
+    <br>
+**Studio features(v0.4.1)**<br>
+    Note: Remeber to import all from tscratchapiget<br>
+    Fill in the [Studio ID] with the ID of a studio<br>
+    - Get a studio title ```studio.title("[Studio ID]")```<br>
+    - Get a studio description ```studio.description("[Studio ID]")```<br>
+    More comming **very soon**!
```

### Comparing `tscratchapiget-0.3.8/pyproject.toml` & `tscratchapiget-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tscratchapiget"
-version = "0.3.8"
+version = "0.4.0"
 authors = [
   { name="Tony", email="tonyvu4913@gmail.com" },
 ]
 description = "A library can get scratch api"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
```

### Comparing `tscratchapiget-0.3.8/src/tscratchapiget/project.py` & `tscratchapiget-0.4.0/src/tscratchapiget/project.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,58 +2,68 @@
 import requests
 import webbrowser
 
 def title(id):
     try:
         data = json.loads(requests.get(f"https://api.scratch.mit.edu/project/{id}/").text)
         return (data["title"])
-    except Exception:
-        return "There is a error. Maybe the project is not shared or it does not exists."
+    except Exception as e:
+        print("There is a error. Maybe the project is not shared or it does not exists.")
+        return e
 
 def description(id):
     try:
         data = json.loads(requests.get(f"https://api.scratch.mit.edu/project/{id}/").text)
         return (data["description"])
-    except Exception:
-        return "There is a error. Maybe the project is not shared or it does not exists."
+    except Exception as e:
+        print("There is a error. Maybe the project is not shared or it does not exists.")
+        return e
     
 def views(id):
     try:
         data = jsondata = json.loads(requests.get(f"https://api.scratch.mit.edu/project/{id}/").text)
         return (data["stats"]['views'])
-    except Exception:
-        return "There is a error. Maybe the project is not shared or it does not exists."
+    except Exception as e:
+        print("There is a error. Maybe the project is not shared or it does not exists.")
+        return e
     
 def loves(id):
     try:
         data = jsondata = json.loads(requests.get(f"https://api.scratch.mit.edu/project/{id}/").text)
         return (data["stats"]['loves'])
-    except Exception:
-        return "There is a error. Maybe the project is not shared or it does not exists."
+    except Exception as e:
+        print("There is a error. Maybe the project is not shared or it does not exists.")
+        return e
     
 def favorites(id):
     try:
         data = jsondata = json.loads(requests.get(f"https://api.scratch.mit.edu/project/{id}/").text)
         return (data['stats']['favorites'])
-    except Exception:
-        return "There is a error. Maybe the project is not shared or it does not exists."
+    except Exception as e:
+        print("There is a error. Maybe the project is not shared or it does not exists.")
+        return e
     
 def remixes(id):
     try:
         data = jsondata = json.loads(requests.get(f"https://api.scratch.mit.edu/project/{id}/").text)
         return (data["stats"]['remixes'])
-    except Exception:
-        return "There is a error. Maybe the project is not shared or it does not exists."    
+    except Exception as e:
+        print("There is a error. Maybe the project is not shared or it does not exists.")
+        return e
     
 def exists(id):
     try:
         data = jsondata = json.loads(requests.get(f"https://api.scratch.mit.edu/project/{id}/").text)
-        if data['code'] == 'NotFound':
+        if data['code'] == 'ResourceNotFound':
             return "Project is not shared or it does not exists."
+        else:
+            return 'There is a bad error. Please report to https://github.com/Tony14261/tscratchapiget/issues'
     except Exception:
             return 'Project exists'
     
 def open(id):
     try:
-        webbrowser.open_new('https://scratch.mit.edu/projects/{id}/')
+        url = 'https://scratch.mit.edu/projects/' + id
+        webbrowser.open_new(url=url)
+        return "Opened successfully"
     except Exception:
         return "There is a bad error. Please report to https://github.com/Tony14261/tscratchapiget/issues"
```

### Comparing `tscratchapiget-0.3.8/src/tscratchapiget.egg-info/PKG-INFO` & `tscratchapiget-0.4.0/src/tscratchapiget.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tscratchapiget
-Version: 0.3.8
+Version: 0.4.0
 Summary: A library can get scratch api
 Author-email: Tony <tonyvu4913@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Scratch_Tony_14261
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,33 +36,43 @@
 
 This project gets the scratch api. Everything in this project code by me (except some needed library). Big credit to TimMcCool(Scratcher) for example codes. (This project is not related to TimMcCool)<br>
 Install: `pip install tscratchapiget`<br>
 Change log: https://github.com/Tony14261/tscratchapiget/blob/main/changelog.md<br>
 Report bugs or request new features here: https://github.com/Tony14261/tscratchapiget/issues<br>
 Contact me (Discord): Tony14261#2089<br>
 <br>
-**Functions**<br>
-    **User features(v0.2.7)(Updated commands in v0.3.0)** (New commands are at the top):<br>
-        Note: Remeber to ```from tscratchapiget import user```<br>
-        - Get if a username exists  ```exists([username])```     EX: ```user.exists('Scratch_Tony_14261')``` if yes: Return 'User exists'     if not: Return 'User does not exist'<br>
-        - Get a user unread-message-count ```message_count('[user]')```     EX: ```user.message_count('TimMcCool')```<br>
-        - Get a user id ```id('[user]')```     EX: ```user.id('griffpatch')```<br>
-        - Get if a user is a scratchteam ```scratchteam('[user]')```     EX: ```user.scratchteam('ScratchCat')``` #Return 'True'<br>
-        - Get user join date ```join('[user]')```     EX: ```user.join('Will_Wam')```#Return '2013-11-25T19:52:29.000Z'<br>
-        - Get a user pfp(link) ```pfp_link('[user]')```     EX: ```user.pfp_link('Scratch_Tony_14261')```          +Bonus Feature: Open that pfp link in browser. Change that to ```pfp_link_open('[Username]')```<br>
-        - Get user About-Me section ```aboutme('[user]')``` EX: ```user.aboutme('WazzoTV')```<br>
-        - Get user What-I'm-Working-On section ```wiwo('[username]')```     EX: ```user.wiwo('ceebee')```<br>
-        - Get user country ```country(['user]')```     EX: ```user.country(['')```<br>
-        - Get user follower count ```followers('[user]')```     Ex: ```user.followers('sharkyshar')```<br>
-        - Get user following count ```following('[user]')```     EX: ```user.followers('atomicmagicnumber')```<br>
-        <br>
-    **Project features(v0.3.6)**<br>
-        Note: Remember to ```from tscratchapiget import project```<br>
-              ONLY FILL IN [PROJECT ID] NOT A FULL LINK<br>
-        - Get a project title ```title('[Project_ID]')```     EX: ```project.title('105500895')```<br>
-        - Get a project description ```description('[Project_ID]')```     EX: ```project.description('105500895')```<br>
-        - Get a project views ```views('[Project_ID]')```     EX: ```project.views('105500895')```<br>
-        - Get a project loves ```loves('[Project_ID]')```     EX: ```project.loves('105500895')```<br>
-        - Get a project favorites ```favorites('[Project_ID]')```    EX: ```project.favorites('105500895')```<br>
-        - Get a project remixes ```remixes('[Project_ID]')```     EX:   ```project.remixes('105500895')```<br>
-        - Get if a project exists ```exists('[Project_ID]')```     EX: ```project.exists('105500895')``` This check returns to your terminal<br>
-        - Open a project in a web browser ```open('[Project_ID]')```     EX: ```project.open('105500895')```<br>
+
+**New feature**(not tested): Tired of importing every single feature? Now, you can ```from tscratchapiget import all```. It will import everything for you.
+
+
+**User features(v0.2.7)(Updated commands in v0.3.0)** (New commands are at the top):<br>
+    Note: Remeber to ```from tscratchapiget import user```<br>
+    - Get if a username exists  ```exists([username])```     EX: ```user.exists('Scratch_Tony_14261')``` if yes: Return 'User exists'     if not: Return 'User does not exist'<br>
+    - Get a user unread-message-count ```message_count('[user]')```     EX: ```user.message_count('TimMcCool')```<br>
+    - Get a user id ```id('[user]')```     EX: ```user.id('griffpatch')```<br>
+    - Get if a user is a scratchteam ```scratchteam('[user]')```     EX: ```user.scratchteam('ScratchCat')``` #Return 'True'<br>
+    - Get user join date ```join('[user]')```     EX: ```user.join('Will_Wam')```#Return '2013-11-25T19:52:29.000Z'<br>
+    - Get a user pfp(link) ```pfp_link('[user]')```     EX: ```user.pfp_link('Scratch_Tony_14261')```          +Bonus Feature: Open that pfp link in browser. Change that to ```pfp_link_open('[Username]')```<br>
+    - Get user About-Me section ```aboutme('[user]')``` EX: ```user.aboutme('WazzoTV')```<br>
+    - Get user What-I'm-Working-On section ```wiwo('[username]')```     EX: ```user.wiwo('ceebee')```<br>
+    - Get user country ```country(['user]')```     EX: ```user.country(['')```<br>
+    - Get user follower count ```followers('[user]')```     Ex: ```user.followers('sharkyshar')```<br>
+    - Get user following count ```following('[user]')```     EX: ```user.followers('atomicmagicnumber')```<br>
+    <br>
+**Project features(v0.3.6)**<br>
+    Note: Remember to ```from tscratchapiget import project```<br>
+    ONLY FILL IN PROJECT ID NOT A FULL LINK<br>
+    - Get a project title ```title('[Project_ID]')```     EX: ```project.title('105500895')```<br>
+    - Get a project description ```description('[Project_ID]')```     EX: ```project.description('105500895')```<br>
+    - Get a project views ```views('[Project_ID]')```     EX: ```project.views('105500895')```<br>
+    - Get a project loves ```loves('[Project_ID]')```     EX: ```project.loves('105500895')```<br>
+    - Get a project favorites ```favorites('[Project_ID]')```    EX: ```project.favorites('105500895')```<br>
+    - Get a project remixes ```remixes('[Project_ID]')```     EX:   ```project.remixes('105500895')```<br>
+    - Get if a project exists ```exists('[Project_ID]')```     EX: ```project.exists('105500895')``` This check returns to your terminal<br>
+    - Open a project in a web browser ```open('[Project_ID]')```     EX: ```project.open('105500895')```<br>
+    <br>
+**Studio features(v0.4.1)**<br>
+    Note: Remeber to import all from tscratchapiget<br>
+    Fill in the [Studio ID] with the ID of a studio<br>
+    - Get a studio title ```studio.title("[Studio ID]")```<br>
+    - Get a studio description ```studio.description("[Studio ID]")```<br>
+    More comming **very soon**!
```

