# Comparing `tmp/BlitzChain-0.4.0.tar.gz` & `tmp/BlitzChain-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BlitzChain-0.4.0.tar", last modified: Fri Jul  7 08:07:33 2023, max compression
+gzip compressed data, was "BlitzChain-0.5.0.tar", last modified: Sun Jul  9 07:26:53 2023, max compression
```

## Comparing `BlitzChain-0.4.0.tar` & `BlitzChain-0.5.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-07 08:07:33.092063 BlitzChain-0.4.0/
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-07 08:07:33.088495 BlitzChain-0.4.0/BlitzChain.egg-info/
--rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-07-07 08:07:33.000000 BlitzChain-0.4.0/BlitzChain.egg-info/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)      361 2023-07-07 08:07:33.000000 BlitzChain-0.4.0/BlitzChain.egg-info/SOURCES.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-07-07 08:07:33.000000 BlitzChain-0.4.0/BlitzChain.egg-info/dependency_links.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        9 2023-07-07 08:07:33.000000 BlitzChain-0.4.0/BlitzChain.egg-info/requires.txt
--rw-r--r--   0 jackywong   (501) staff       (20)       15 2023-07-07 08:07:33.000000 BlitzChain-0.4.0/BlitzChain.egg-info/top_level.txt
--rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-06-25 04:01:50.000000 BlitzChain-0.4.0/LICENSE
--rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-07-07 08:07:33.091754 BlitzChain-0.4.0/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)     3488 2023-07-07 08:06:07.000000 BlitzChain-0.4.0/README.md
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-07 08:07:33.089844 BlitzChain-0.4.0/blitzchain/
--rw-r--r--   0 jackywong   (501) staff       (20)       42 2023-07-07 08:06:26.000000 BlitzChain-0.4.0/blitzchain/__init__.py
--rw-r--r--   0 jackywong   (501) staff       (20)     5898 2023-07-07 08:06:27.000000 BlitzChain-0.4.0/blitzchain/api.py
--rw-r--r--   0 jackywong   (501) staff       (20)     2138 2023-07-03 10:04:06.000000 BlitzChain-0.4.0/blitzchain/splitter.py
--rw-r--r--   0 jackywong   (501) staff       (20)      763 2023-06-28 00:10:27.000000 BlitzChain-0.4.0/blitzchain/utils.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-07 08:07:33.090437 BlitzChain-0.4.0/cli/
--rw-r--r--   0 jackywong   (501) staff       (20)        0 2023-06-28 03:39:00.000000 BlitzChain-0.4.0/cli/__init__.py
--rw-r--r--   0 jackywong   (501) staff       (20)      430 2023-06-28 13:19:06.000000 BlitzChain-0.4.0/cli/main.py
--rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-07-07 08:07:33.092154 BlitzChain-0.4.0/setup.cfg
--rw-r--r--   0 jackywong   (501) staff       (20)      485 2023-06-28 05:27:42.000000 BlitzChain-0.4.0/setup.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-07 08:07:33.091343 BlitzChain-0.4.0/tests/
--rw-r--r--   0 jackywong   (501) staff       (20)      216 2023-06-25 05:27:46.000000 BlitzChain-0.4.0/tests/test_crud.py
--rw-r--r--   0 jackywong   (501) staff       (20)      715 2023-06-25 05:08:57.000000 BlitzChain-0.4.0/tests/test_pdf.py
--rw-r--r--   0 jackywong   (501) staff       (20)      621 2023-06-25 07:10:23.000000 BlitzChain-0.4.0/tests/test_qa.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-09 07:26:53.543023 BlitzChain-0.5.0/
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-09 07:26:53.538142 BlitzChain-0.5.0/BlitzChain.egg-info/
+-rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-07-09 07:26:53.000000 BlitzChain-0.5.0/BlitzChain.egg-info/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)      361 2023-07-09 07:26:53.000000 BlitzChain-0.5.0/BlitzChain.egg-info/SOURCES.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-07-09 07:26:53.000000 BlitzChain-0.5.0/BlitzChain.egg-info/dependency_links.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        9 2023-07-09 07:26:53.000000 BlitzChain-0.5.0/BlitzChain.egg-info/requires.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)       15 2023-07-09 07:26:53.000000 BlitzChain-0.5.0/BlitzChain.egg-info/top_level.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-06-25 04:01:50.000000 BlitzChain-0.5.0/LICENSE
+-rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-07-09 07:26:53.542751 BlitzChain-0.5.0/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)     3488 2023-07-07 08:06:07.000000 BlitzChain-0.5.0/README.md
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-09 07:26:53.539815 BlitzChain-0.5.0/blitzchain/
+-rw-r--r--   0 jackywong   (501) staff       (20)       42 2023-07-09 07:26:39.000000 BlitzChain-0.5.0/blitzchain/__init__.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     6424 2023-07-09 07:26:30.000000 BlitzChain-0.5.0/blitzchain/api.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     2138 2023-07-03 10:04:06.000000 BlitzChain-0.5.0/blitzchain/splitter.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      763 2023-06-28 00:10:27.000000 BlitzChain-0.5.0/blitzchain/utils.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-09 07:26:53.540696 BlitzChain-0.5.0/cli/
+-rw-r--r--   0 jackywong   (501) staff       (20)        0 2023-06-28 03:39:00.000000 BlitzChain-0.5.0/cli/__init__.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      430 2023-06-28 13:19:06.000000 BlitzChain-0.5.0/cli/main.py
+-rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-07-09 07:26:53.543110 BlitzChain-0.5.0/setup.cfg
+-rw-r--r--   0 jackywong   (501) staff       (20)      485 2023-06-28 05:27:42.000000 BlitzChain-0.5.0/setup.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-09 07:26:53.542097 BlitzChain-0.5.0/tests/
+-rw-r--r--   0 jackywong   (501) staff       (20)      216 2023-06-25 05:27:46.000000 BlitzChain-0.5.0/tests/test_crud.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      715 2023-06-25 05:08:57.000000 BlitzChain-0.5.0/tests/test_pdf.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      621 2023-06-25 07:10:23.000000 BlitzChain-0.5.0/tests/test_qa.py
```

### Comparing `BlitzChain-0.4.0/LICENSE` & `BlitzChain-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.4.0/README.md` & `BlitzChain-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.4.0/blitzchain/api.py` & `BlitzChain-0.5.0/blitzchain/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,14 +74,30 @@
             },
             json={
                 "collection": self.collection_name,
                 "url": url
             }
         )
         return get_json_response(response)
+
+    def insert_html(self, html: str, metadata: dict=None):
+        api_url = self.base_url + "collection/insert-html"
+        response = requests.post(
+            api_url,
+            headers={
+                "Content-Type": "application/json",
+                "Authorization": "Bearer " + self.api_key
+            },
+            json={
+                "collection": self.collection_name,
+                "html": html,
+                "metadata": metadata
+            }
+        )
+        return get_json_response(response)
     
     def generative_qa(self, user_input: str, prompt_fields: list,
         conversation_id: str=None, limit: int=5, fields: list=None,
         include_rerank: bool=False, minimum_rerank_score: float=0.7,
         include_moderation: bool=False
     ):
         """Get an answer based on a question that you ask.
```

### Comparing `BlitzChain-0.4.0/blitzchain/splitter.py` & `BlitzChain-0.5.0/blitzchain/splitter.py`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.4.0/blitzchain/utils.py` & `BlitzChain-0.5.0/blitzchain/utils.py`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.4.0/tests/test_pdf.py` & `BlitzChain-0.5.0/tests/test_pdf.py`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.4.0/tests/test_qa.py` & `BlitzChain-0.5.0/tests/test_qa.py`

 * *Files identical despite different names*

