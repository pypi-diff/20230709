# Comparing `tmp/BlitzChain-0.5.0.tar.gz` & `tmp/BlitzChain-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BlitzChain-0.5.0.tar", last modified: Sun Jul  9 07:26:53 2023, max compression
+gzip compressed data, was "BlitzChain-0.5.1.tar", last modified: Sun Jul  9 13:27:45 2023, max compression
```

## Comparing `BlitzChain-0.5.0.tar` & `BlitzChain-0.5.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-09 07:26:53.543023 BlitzChain-0.5.0/
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-09 07:26:53.538142 BlitzChain-0.5.0/BlitzChain.egg-info/
--rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-07-09 07:26:53.000000 BlitzChain-0.5.0/BlitzChain.egg-info/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)      361 2023-07-09 07:26:53.000000 BlitzChain-0.5.0/BlitzChain.egg-info/SOURCES.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-07-09 07:26:53.000000 BlitzChain-0.5.0/BlitzChain.egg-info/dependency_links.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        9 2023-07-09 07:26:53.000000 BlitzChain-0.5.0/BlitzChain.egg-info/requires.txt
--rw-r--r--   0 jackywong   (501) staff       (20)       15 2023-07-09 07:26:53.000000 BlitzChain-0.5.0/BlitzChain.egg-info/top_level.txt
--rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-06-25 04:01:50.000000 BlitzChain-0.5.0/LICENSE
--rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-07-09 07:26:53.542751 BlitzChain-0.5.0/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)     3488 2023-07-07 08:06:07.000000 BlitzChain-0.5.0/README.md
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-09 07:26:53.539815 BlitzChain-0.5.0/blitzchain/
--rw-r--r--   0 jackywong   (501) staff       (20)       42 2023-07-09 07:26:39.000000 BlitzChain-0.5.0/blitzchain/__init__.py
--rw-r--r--   0 jackywong   (501) staff       (20)     6424 2023-07-09 07:26:30.000000 BlitzChain-0.5.0/blitzchain/api.py
--rw-r--r--   0 jackywong   (501) staff       (20)     2138 2023-07-03 10:04:06.000000 BlitzChain-0.5.0/blitzchain/splitter.py
--rw-r--r--   0 jackywong   (501) staff       (20)      763 2023-06-28 00:10:27.000000 BlitzChain-0.5.0/blitzchain/utils.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-09 07:26:53.540696 BlitzChain-0.5.0/cli/
--rw-r--r--   0 jackywong   (501) staff       (20)        0 2023-06-28 03:39:00.000000 BlitzChain-0.5.0/cli/__init__.py
--rw-r--r--   0 jackywong   (501) staff       (20)      430 2023-06-28 13:19:06.000000 BlitzChain-0.5.0/cli/main.py
--rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-07-09 07:26:53.543110 BlitzChain-0.5.0/setup.cfg
--rw-r--r--   0 jackywong   (501) staff       (20)      485 2023-06-28 05:27:42.000000 BlitzChain-0.5.0/setup.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-09 07:26:53.542097 BlitzChain-0.5.0/tests/
--rw-r--r--   0 jackywong   (501) staff       (20)      216 2023-06-25 05:27:46.000000 BlitzChain-0.5.0/tests/test_crud.py
--rw-r--r--   0 jackywong   (501) staff       (20)      715 2023-06-25 05:08:57.000000 BlitzChain-0.5.0/tests/test_pdf.py
--rw-r--r--   0 jackywong   (501) staff       (20)      621 2023-06-25 07:10:23.000000 BlitzChain-0.5.0/tests/test_qa.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-09 13:27:45.887178 BlitzChain-0.5.1/
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-09 13:27:45.882551 BlitzChain-0.5.1/BlitzChain.egg-info/
+-rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-07-09 13:27:45.000000 BlitzChain-0.5.1/BlitzChain.egg-info/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)      361 2023-07-09 13:27:45.000000 BlitzChain-0.5.1/BlitzChain.egg-info/SOURCES.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-07-09 13:27:45.000000 BlitzChain-0.5.1/BlitzChain.egg-info/dependency_links.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        9 2023-07-09 13:27:45.000000 BlitzChain-0.5.1/BlitzChain.egg-info/requires.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)       15 2023-07-09 13:27:45.000000 BlitzChain-0.5.1/BlitzChain.egg-info/top_level.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-06-25 04:01:50.000000 BlitzChain-0.5.1/LICENSE
+-rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-07-09 13:27:45.886882 BlitzChain-0.5.1/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)     3488 2023-07-07 08:06:07.000000 BlitzChain-0.5.1/README.md
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-09 13:27:45.883931 BlitzChain-0.5.1/blitzchain/
+-rw-r--r--   0 jackywong   (501) staff       (20)       42 2023-07-09 13:27:33.000000 BlitzChain-0.5.1/blitzchain/__init__.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     6471 2023-07-09 13:27:28.000000 BlitzChain-0.5.1/blitzchain/api.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     2138 2023-07-03 10:04:06.000000 BlitzChain-0.5.1/blitzchain/splitter.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      763 2023-06-28 00:10:27.000000 BlitzChain-0.5.1/blitzchain/utils.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-09 13:27:45.884631 BlitzChain-0.5.1/cli/
+-rw-r--r--   0 jackywong   (501) staff       (20)        0 2023-06-28 03:39:00.000000 BlitzChain-0.5.1/cli/__init__.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      430 2023-06-28 13:19:06.000000 BlitzChain-0.5.1/cli/main.py
+-rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-07-09 13:27:45.887283 BlitzChain-0.5.1/setup.cfg
+-rw-r--r--   0 jackywong   (501) staff       (20)      485 2023-06-28 05:27:42.000000 BlitzChain-0.5.1/setup.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-09 13:27:45.886296 BlitzChain-0.5.1/tests/
+-rw-r--r--   0 jackywong   (501) staff       (20)      216 2023-06-25 05:27:46.000000 BlitzChain-0.5.1/tests/test_crud.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      715 2023-06-25 05:08:57.000000 BlitzChain-0.5.1/tests/test_pdf.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      621 2023-06-25 07:10:23.000000 BlitzChain-0.5.1/tests/test_qa.py
```

### Comparing `BlitzChain-0.5.0/LICENSE` & `BlitzChain-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.5.0/README.md` & `BlitzChain-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.5.0/blitzchain/api.py` & `BlitzChain-0.5.1/blitzchain/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,21 +15,22 @@
         self.api_key = api_key
         self.base_url = "https://app.twilix.io/api/v1/"
     
     def Collection(self, collection_name: str):
         return Collection(api_key=self.api_key, collection_name=collection_name)
     
     def list_collections(self):
-        return requests.get(
+        response = requests.get(
             url=self.base_url + "collection/list",
             headers={
                 "Content-Type": "application/json", 
                 "Authorization": "Bearer " + self.api_key
             }
         )
+        return get_json_response(response)
 
 class Collection:
     def __init__(self, api_key: str, collection_name: str):
         self.collection_name = collection_name
         self.api_key = api_key
         self.base_url = "https://app.twilix.io/api/v1/"
```

### Comparing `BlitzChain-0.5.0/blitzchain/splitter.py` & `BlitzChain-0.5.1/blitzchain/splitter.py`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.5.0/blitzchain/utils.py` & `BlitzChain-0.5.1/blitzchain/utils.py`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.5.0/tests/test_pdf.py` & `BlitzChain-0.5.1/tests/test_pdf.py`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.5.0/tests/test_qa.py` & `BlitzChain-0.5.1/tests/test_qa.py`

 * *Files identical despite different names*

