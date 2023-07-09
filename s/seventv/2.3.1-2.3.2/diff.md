# Comparing `tmp/seventv-2.3.1.tar.gz` & `tmp/seventv-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seventv-2.3.1.tar", last modified: Sun Jul  9 20:53:43 2023, max compression
+gzip compressed data, was "seventv-2.3.2.tar", last modified: Sun Jul  9 21:15:01 2023, max compression
```

## Comparing `seventv-2.3.1.tar` & `seventv-2.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:53:43.199640 seventv-2.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-07-09 20:53:26.000000 seventv-2.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-09 20:53:43.199640 seventv-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-09 20:53:26.000000 seventv-2.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 20:53:43.203640 seventv-2.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-09 20:53:26.000000 seventv-2.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:53:43.195640 seventv-2.3.1/seventv/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-09 20:53:26.000000 seventv-2.3.1/seventv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-09 20:53:26.000000 seventv-2.3.1/seventv/seventv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:53:43.199640 seventv-2.3.1/seventv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-09 20:53:43.000000 seventv-2.3.1/seventv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-09 20:53:43.000000 seventv-2.3.1/seventv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 20:53:43.000000 seventv-2.3.1/seventv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-09 20:53:43.000000 seventv-2.3.1/seventv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-09 20:53:43.000000 seventv-2.3.1/seventv.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:53:43.199640 seventv-2.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-09 20:53:26.000000 seventv-2.3.1/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:15:01.190548 seventv-2.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-07-09 21:14:48.000000 seventv-2.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-09 21:15:01.190548 seventv-2.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-09 21:14:48.000000 seventv-2.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 21:15:01.190548 seventv-2.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-09 21:14:48.000000 seventv-2.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:15:01.190548 seventv-2.3.2/seventv/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-09 21:14:48.000000 seventv-2.3.2/seventv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-07-09 21:14:48.000000 seventv-2.3.2/seventv/seventv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:15:01.190548 seventv-2.3.2/seventv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-09 21:15:01.000000 seventv-2.3.2/seventv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-09 21:15:01.000000 seventv-2.3.2/seventv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 21:15:01.000000 seventv-2.3.2/seventv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-09 21:15:01.000000 seventv-2.3.2/seventv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-09 21:15:01.000000 seventv-2.3.2/seventv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:15:01.190548 seventv-2.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-09 21:14:48.000000 seventv-2.3.2/tests/test.py
```

### Comparing `seventv-2.3.1/LICENSE` & `seventv-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `seventv-2.3.1/PKG-INFO` & `seventv-2.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seventv
-Version: 2.3.1
+Version: 2.3.2
 Summary: An asynchronous API-wrapper for 7tv.app
 Home-page: https://github.com/probablyjassin/seventv.py
 Author: Jässin Aouani
 Author-email: jassin@aouani.de
 License: GPL
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `seventv-2.3.1/README.md` & `seventv-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `seventv-2.3.1/setup.py` & `seventv-2.3.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='seventv',
-    version="2.3.1",
+    version="2.3.2",
     author='Jässin Aouani',
     author_email='jassin@aouani.de',
     description='An asynchronous API-wrapper for 7tv.app',
     long_description = """
         An asynchronous Python API-wrapper for 7tv.app. 
         It makes use of the 7tv API (v3) to make it possible to get emotes, details about them, and soon some more things the API supports.
         To get emotes by search query, the wrapper uses the GraphQL endpoint
```

### Comparing `seventv-2.3.1/seventv/seventv.py` & `seventv-2.3.2/seventv/seventv.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,10 +92,13 @@
                 }
             },
             "query": f"{queries.get(query)}"
         }
         async with self.session.post(url, json=payload, headers=headers) as response:
             response_data = await response.json()
             if response_data.get('errors', {}):
-                raise Exception(response_data.get('errors', {})[0].get('message', {}))
+                raise seventvException(response_data.get('errors', {})[0].get('message', {}))
             emote_objects = create_emote_objects(response_data)
             return emote_objects
+
+class seventvException(Exception):
+        pass
```

### Comparing `seventv-2.3.1/seventv.egg-info/PKG-INFO` & `seventv-2.3.2/seventv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seventv
-Version: 2.3.1
+Version: 2.3.2
 Summary: An asynchronous API-wrapper for 7tv.app
 Home-page: https://github.com/probablyjassin/seventv.py
 Author: Jässin Aouani
 Author-email: jassin@aouani.de
 License: GPL
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

