# Comparing `tmp/seventv-2.1.0.tar.gz` & `tmp/seventv-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seventv-2.1.0.tar", last modified: Sat Jul  8 17:24:54 2023, max compression
+gzip compressed data, was "seventv-2.2.0.tar", last modified: Sun Jul  9 13:43:22 2023, max compression
```

## Comparing `seventv-2.1.0.tar` & `seventv-2.2.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:24:54.629298 seventv-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-07-08 17:24:44.000000 seventv-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-08 17:24:54.629298 seventv-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-08 17:24:44.000000 seventv-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 17:24:54.629298 seventv-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-08 17:24:44.000000 seventv-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:24:54.629298 seventv-2.1.0/seventv/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-08 17:24:44.000000 seventv-2.1.0/seventv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-07-08 17:24:44.000000 seventv-2.1.0/seventv/seventv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:24:54.629298 seventv-2.1.0/seventv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-08 17:24:54.000000 seventv-2.1.0/seventv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-08 17:24:54.000000 seventv-2.1.0/seventv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 17:24:54.000000 seventv-2.1.0/seventv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 17:24:54.000000 seventv-2.1.0/seventv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 17:24:54.000000 seventv-2.1.0/seventv.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:24:54.629298 seventv-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-08 17:24:44.000000 seventv-2.1.0/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:22.006310 seventv-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-07-09 13:43:09.000000 seventv-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-09 13:43:22.006310 seventv-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-09 13:43:09.000000 seventv-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 13:43:22.006310 seventv-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-09 13:43:09.000000 seventv-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:22.006310 seventv-2.2.0/seventv/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-09 13:43:09.000000 seventv-2.2.0/seventv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-07-09 13:43:09.000000 seventv-2.2.0/seventv/seventv.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:09.000000 seventv-2.2.0/seventv/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:22.006310 seventv-2.2.0/seventv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-09 13:43:21.000000 seventv-2.2.0/seventv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-09 13:43:22.000000 seventv-2.2.0/seventv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 13:43:21.000000 seventv-2.2.0/seventv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-09 13:43:21.000000 seventv-2.2.0/seventv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-09 13:43:21.000000 seventv-2.2.0/seventv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:22.006310 seventv-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-09 13:43:09.000000 seventv-2.2.0/tests/test.py
```

### Comparing `seventv-2.1.0/LICENSE` & `seventv-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seventv-2.1.0/PKG-INFO` & `seventv-2.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: seventv
-Version: 2.1.0
+Version: 2.2.0
 Summary: An asynchronous API-wrapper for 7tv.app
+Home-page: https://github.com/probablyjassin/seventv.py
 Author: Jässin Aouani
 Author-email: jassin@aouani.de
 License: GPL
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `seventv-2.1.0/README.md` & `seventv-2.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -31,44 +31,58 @@
 async def myFunctionSearchEmote():
     mySevenTvSession = seventv.seventv()
     # initialize an instance of the seventv() class. this must happen in an asynchronous context
 
     emotes = await mySevenTvSession.emote_search("pepe", case_sensitive=True)
     # searches for "pepe", using the optional filter "case_sensitive"
     
-    print(emotes[2]) # get the third emote from the search results
+    myEmote = emotes[2] # get the third emote from the search results
+    print(myEmote)
+    print(myEmote.host_url) # get the url from the emote object
+    
     await mySevenTvSession.close() # later close the session
 
 asyncio.run(getemote())
 ```
-_About closing sessions: initializing a session with seventv.sevent() creates an aiohttp session. This session should be closed by calling yourSession.close() at some point. Not doing so will cause a warning like this:_ 
+Sample output: third Emote object in results; host_url:
 ```
-Unclosed session
-client_session: <aiohttp.client.ClientSession object at 0x7fd2b06469b0>
+Emote(id: 60a304efac2bcb20ef20fa89, name: pepeMeltdown, owner_username: supernoahtv, host_url: //cdn.7tv.app/emote/60a304efac2bcb20ef20fa89)
+//cdn.7tv.app/emote/60a304efac2bcb20ef20fa89
 ```
-_Closing/reopening it after every request does avoid the warning, but is not very efficent. It would be optimal to close the session when the service/code that uses it stops._
-
-Sample output: third Emote object in the search results:
-```Emote(id: 60a304efac2bcb20ef20fa89, name: pepeMeltdown, owner_username: supernoahtv, host_url: //cdn.7tv.app/emote/60a304efac2bcb20ef20fa89)```
 
 The output from a search is an array with the Emote objects inside.
 Each emote contains the following properties:
 - id
 - name
 - owner_username
 - host_url
 
-_Sidenote: Keep in mind that to get the emote using the url, the file extension must be appended to the host_url. Emotes are stored on 7tv in different sizes, usually ranging from 1x.webp to 4x.webp. Not every emote might have every size though, so look it up or go with x2 or x3 which the majority of emotes have._
+_Sidenote: Keep in mind that to use the actual emote-image using the url, you must write it as url like this:_
+```
+host_url = //cdn.7tv.app/emote/60a304efac2bcb20ef20fa89 # url you get from the api
+https:host_url/2x.webp
+```
+_Emotes are stored on 7tv in different sizes, usually ranging from 1x.webp to 4x.webp. Not every emote might have every size though, so look it up or go with x2 or x3 which the majority of emotes have._
+
+_About closing sessions: initializing a session with seventv.sevent() creates an aiohttp session. This session should be closed by calling .close() at some point. Not doing so will cause a warning like this:_ 
+```
+Unclosed client session
+client_session: <aiohttp.client.ClientSession object at 0x7fd2b06469b0>
+```
+_Closing/reopening it after every request does avoid the warning, but is not very efficent. It would be optimal to close the session when the service/code that uses it stops._
 
 ### Currently available search filters (optional):
 
 | filter                         | meaning | default value |     
 | ---------------------------------------------- | -------- | --------------- | 
+| searchterm | search for specific emotes by text string      | empty string, which can be left this way and still works             |
 | limit (int) | how many emotes are contained in the response      | 12             |     
 | page (int) | which page from the search results to return      | 1             | 
 | case_sensitive (bool) | whether or not upper-/lowercase letters are treated differently or will not be distinguished   | False |     
 | animated (bool) |only return animated emotes in search results          | False                 |     
-| exact_match (bool) | only return emotes that exactly match the search query | False   |     |                                               |          |                 |     
+| exact_match (bool) | only return emotes that exactly match the search query | False   |
+| query     | you can chose what data exactly to request (WIP). options: "all", "url" for only the host_url | "all"         |
 
 
-soon to be added functionality: 
-- get an emote by it's id
+planned to be added functionality: 
+- get an emote by it's id
+- more options for the gql query
```

### Comparing `seventv-2.1.0/setup.py` & `seventv-2.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from setuptools import setup
 
 setup(
     name='seventv',
-    version='2.1.0',
+    version="2.2.0",
     author='Jässin Aouani',
     author_email='jassin@aouani.de',
     description='An asynchronous API-wrapper for 7tv.app',
     long_description = """
         An asynchronous Python API-wrapper for 7tv.app. 
         It makes use of the 7tv API (v3) to make it possible to get emotes, details about them, and soon some more things the API supports.
         To get emotes by search query, the wrapper uses the GraphQL endpoint 
         https://7tv.io/v3/gql because it seems to currently be the only working one for searching emotes.
     """,
     packages=['seventv'],
     install_requires=['aiohttp'],
+    url="https://github.com/probablyjassin/seventv.py",
     license='GPL',
     classifiers=[
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
```

### Comparing `seventv-2.1.0/seventv/seventv.py` & `seventv-2.2.0/seventv/seventv.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 import aiohttp
+from typing import Literal
 
 class Emote:
-    def __init__(self, id, name, owner_username, host_url):
+    def __init__(self, id = None, name = None, owner_username = None, host_url = None):
         self.id = id
         self.name = name
         self.owner_username = owner_username
         self.host_url = host_url
 
     def __repr__(self):
         return '' \
@@ -20,27 +21,31 @@
             "id": self.id,
             "name": self.name,
             "owner_username": self.owner_username,
             "host_url": self.host_url
         }
 
 def create_emote_objects(response: dict) -> list[Emote]:
-    emotes_data = response['data']['emotes']
-    emote_items = emotes_data['items']
-
+    if (response.get('errors', {})):
+        raise Exception(response.get('errors', {})[0].get('message', {}))
+    
     emote_objects = []
+    emotes_data = response.get('data', {}).get('emotes')
+    emote_items = emotes_data.get('items', [])
 
     for emote in emote_items:
-        emote_id = emote['id']
-        emote_name = emote['name']
-        owner = emote['owner']
-        owner_username = owner['username']
-        host = emote['host']
-        host_url = host['url']
+        emote_id = emote.get('id')
+        emote_name = emote.get('name')
+        owner = emote.get('owner', {})
+        owner_username = owner.get('username')
+        host = emote.get('host', {})
+        host_url = host.get('url')
+
         emote_objects.append(Emote(emote_id, emote_name, owner_username, host_url))
+
     return emote_objects
 
 class seventv:
     def __init__(self):
         self.endpoint = "https://7tv.io/v3/gql"
         self.session = aiohttp.ClientSession()
 
@@ -49,17 +54,22 @@
 
     async def emote_search(self, 
                            searchterm: str = "", 
                            limit: int = 12,
                            page: int = 1,
                            case_sensitive: bool = False, 
                            animated: bool = False,
-                           exact_match: bool = False
+                           exact_match: bool = False, 
+                           query: Literal["all", "url"] = "all",
                            ):
         url = self.endpoint
+        queries = {
+        "all": 'query SearchEmotes($query: String!, $page: Int, $sort: Sort, $limit: Int, $filter: EmoteSearchFilter) {\n emotes(query: $query, page: $page, sort: $sort, limit: $limit, filter: $filter) {\nitems{\n id\n name\n owner{\n username\n }\n host{\n url}}\n}\n}',
+        "url": 'query SearchEmotes($query: String!, $page: Int, $sort: Sort, $limit: Int, $filter: EmoteSearchFilter) {\n emotes(query: $query, page: $page, sort: $sort, limit: $limit, filter: $filter) {\nitems{host{\n url}}\n}\n}'
+        }
         headers = {
             "Content-Type": "application/json"
         }
         payload = {
             "operationName": "SearchEmotes",
             "variables": {
                 "query": searchterm,
@@ -75,17 +85,15 @@
                     "case_sensitive": case_sensitive,
                     "ignore_tags": False,
                     "zero_width": False,
                     "animated": animated,
                     "aspect_ratio": ""
                 }
             },
-            "query": "query SearchEmotes($query: String!, $page: Int, $sort: Sort, $limit: Int, $filter: EmoteSearchFilter) {\n  emotes(query: $query, page: $page, sort: $sort, limit: $limit, filter: $filter) {\n    count\n    items {\n      id\n      name\n      state\n      trending\n      owner {\n        id\n        username\n        display_name\n        style {\n          color\n          paint_id\n          __typename\n        }\n        __typename\n      }\n      flags\n      host {\n        url\n        files {\n          name\n          format\n          width\n          height\n          __typename\n        }\n        __typename\n      }\n      __typename\n    }\n    __typename\n  }\n}"
+            "query": f"{queries.get(query)}"
         }
-
         async with self.session.post(url, json=payload, headers=headers) as response:
             if response.status != 200:
-                raise Exception("HTTP request failed")
+                raise Exception(response.get('errors', {})[0].get('message', {}))
             response_data = await response.json()
             emote_objects = create_emote_objects(response_data)
             return emote_objects
-
```

### Comparing `seventv-2.1.0/seventv.egg-info/PKG-INFO` & `seventv-2.2.0/seventv.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: seventv
-Version: 2.1.0
+Version: 2.2.0
 Summary: An asynchronous API-wrapper for 7tv.app
+Home-page: https://github.com/probablyjassin/seventv.py
 Author: Jässin Aouani
 Author-email: jassin@aouani.de
 License: GPL
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

