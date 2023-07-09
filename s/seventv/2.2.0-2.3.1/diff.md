# Comparing `tmp/seventv-2.2.0.tar.gz` & `tmp/seventv-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seventv-2.2.0.tar", last modified: Sun Jul  9 13:43:22 2023, max compression
+gzip compressed data, was "seventv-2.3.1.tar", last modified: Sun Jul  9 20:53:43 2023, max compression
```

## Comparing `seventv-2.2.0.tar` & `seventv-2.3.1.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:22.006310 seventv-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-07-09 13:43:09.000000 seventv-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-09 13:43:22.006310 seventv-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-09 13:43:09.000000 seventv-2.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 13:43:22.006310 seventv-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-09 13:43:09.000000 seventv-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:22.006310 seventv-2.2.0/seventv/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-09 13:43:09.000000 seventv-2.2.0/seventv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-07-09 13:43:09.000000 seventv-2.2.0/seventv/seventv.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:09.000000 seventv-2.2.0/seventv/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:22.006310 seventv-2.2.0/seventv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-09 13:43:21.000000 seventv-2.2.0/seventv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-09 13:43:22.000000 seventv-2.2.0/seventv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 13:43:21.000000 seventv-2.2.0/seventv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-09 13:43:21.000000 seventv-2.2.0/seventv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-09 13:43:21.000000 seventv-2.2.0/seventv.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:22.006310 seventv-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-09 13:43:09.000000 seventv-2.2.0/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:53:43.199640 seventv-2.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-07-09 20:53:26.000000 seventv-2.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-09 20:53:43.199640 seventv-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-09 20:53:26.000000 seventv-2.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 20:53:43.203640 seventv-2.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-09 20:53:26.000000 seventv-2.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:53:43.195640 seventv-2.3.1/seventv/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-09 20:53:26.000000 seventv-2.3.1/seventv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-09 20:53:26.000000 seventv-2.3.1/seventv/seventv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:53:43.199640 seventv-2.3.1/seventv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-09 20:53:43.000000 seventv-2.3.1/seventv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-09 20:53:43.000000 seventv-2.3.1/seventv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 20:53:43.000000 seventv-2.3.1/seventv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-09 20:53:43.000000 seventv-2.3.1/seventv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-09 20:53:43.000000 seventv-2.3.1/seventv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:53:43.199640 seventv-2.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-09 20:53:26.000000 seventv-2.3.1/tests/test.py
```

### Comparing `seventv-2.2.0/LICENSE` & `seventv-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `seventv-2.2.0/PKG-INFO` & `seventv-2.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seventv
-Version: 2.2.0
+Version: 2.3.1
 Summary: An asynchronous API-wrapper for 7tv.app
 Home-page: https://github.com/probablyjassin/seventv.py
 Author: Jässin Aouani
 Author-email: jassin@aouani.de
 License: GPL
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `seventv-2.2.0/README.md` & `seventv-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `seventv-2.2.0/setup.py` & `seventv-2.3.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='seventv',
-    version="2.2.0",
+    version="2.3.1",
     author='Jässin Aouani',
     author_email='jassin@aouani.de',
     description='An asynchronous API-wrapper for 7tv.app',
     long_description = """
         An asynchronous Python API-wrapper for 7tv.app. 
         It makes use of the 7tv API (v3) to make it possible to get emotes, details about them, and soon some more things the API supports.
         To get emotes by search query, the wrapper uses the GraphQL endpoint
```

### Comparing `seventv-2.2.0/seventv/seventv.py` & `seventv-2.3.1/seventv/seventv.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from __future__ import annotations
-import aiohttp
+import aiohttp, json
 from typing import Literal
 
 class Emote:
     def __init__(self, id = None, name = None, owner_username = None, host_url = None):
         self.id = id
         self.name = name
         self.owner_username = owner_username
@@ -41,14 +41,15 @@
         host_url = host.get('url')
 
         emote_objects.append(Emote(emote_id, emote_name, owner_username, host_url))
 
     return emote_objects
 
 class seventv:
+    """The seventv instance that contains an aiohttp session and the methods for interacting with the API"""
     def __init__(self):
         self.endpoint = "https://7tv.io/v3/gql"
         self.session = aiohttp.ClientSession()
 
     async def close(self):
         await self.session.close()
 
@@ -57,26 +58,27 @@
                            limit: int = 12,
                            page: int = 1,
                            case_sensitive: bool = False, 
                            animated: bool = False,
                            exact_match: bool = False, 
                            query: Literal["all", "url"] = "all",
                            ):
+        """Search for emotes using a text string (searchterm)"""
         url = self.endpoint
         queries = {
         "all": 'query SearchEmotes($query: String!, $page: Int, $sort: Sort, $limit: Int, $filter: EmoteSearchFilter) {\n emotes(query: $query, page: $page, sort: $sort, limit: $limit, filter: $filter) {\nitems{\n id\n name\n owner{\n username\n }\n host{\n url}}\n}\n}',
         "url": 'query SearchEmotes($query: String!, $page: Int, $sort: Sort, $limit: Int, $filter: EmoteSearchFilter) {\n emotes(query: $query, page: $page, sort: $sort, limit: $limit, filter: $filter) {\nitems{host{\n url}}\n}\n}'
         }
         headers = {
             "Content-Type": "application/json"
         }
         payload = {
             "operationName": "SearchEmotes",
             "variables": {
-                "query": searchterm,
+                "query": json.dumps(searchterm),
                 "limit": limit,
                 "page": page,
                 "sort": {
                     "value": "popularity",
                     "order": "DESCENDING"
                 },
                 "filter": {
@@ -88,12 +90,12 @@
                     "animated": animated,
                     "aspect_ratio": ""
                 }
             },
             "query": f"{queries.get(query)}"
         }
         async with self.session.post(url, json=payload, headers=headers) as response:
-            if response.status != 200:
-                raise Exception(response.get('errors', {})[0].get('message', {}))
             response_data = await response.json()
+            if response_data.get('errors', {}):
+                raise Exception(response_data.get('errors', {})[0].get('message', {}))
             emote_objects = create_emote_objects(response_data)
             return emote_objects
```

### Comparing `seventv-2.2.0/seventv.egg-info/PKG-INFO` & `seventv-2.3.1/seventv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seventv
-Version: 2.2.0
+Version: 2.3.1
 Summary: An asynchronous API-wrapper for 7tv.app
 Home-page: https://github.com/probablyjassin/seventv.py
 Author: Jässin Aouani
 Author-email: jassin@aouani.de
 License: GPL
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

