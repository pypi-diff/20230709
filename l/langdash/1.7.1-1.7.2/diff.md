# Comparing `tmp/langdash-1.7.1.tar.gz` & `tmp/langdash-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langdash-1.7.1.tar", last modified: Fri Jul  7 17:44:09 2023, max compression
+gzip compressed data, was "langdash-1.7.2.tar", last modified: Sat Jul  8 23:55:09 2023, max compression
```

## Comparing `langdash-1.7.1.tar` & `langdash-1.7.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-07 17:44:09.181198 langdash-1.7.1/
--rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-1.7.1/LICENSE.txt
--rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-1.7.1/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)     3724 2023-07-07 17:44:09.181198 langdash-1.7.1/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     2788 2023-06-23 20:18:20.000000 langdash-1.7.1/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-07 17:44:09.177197 langdash-1.7.1/langdash/
--rw-rw-r--   0 user      (1000) user      (1000)       76 2023-07-07 17:41:14.000000 langdash-1.7.1/langdash/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-07 17:44:09.177197 langdash-1.7.1/langdash/chains/
--rw-rw-r--   0 user      (1000) user      (1000)      177 2023-06-27 17:54:15.000000 langdash-1.7.1/langdash/chains/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    14903 2023-06-28 07:18:05.000000 langdash-1.7.1/langdash/chains/chains.py
--rw-rw-r--   0 user      (1000) user      (1000)     9394 2023-06-28 07:12:18.000000 langdash-1.7.1/langdash/chains/nodes.py
--rw-rw-r--   0 user      (1000) user      (1000)      253 2023-06-11 03:43:22.000000 langdash-1.7.1/langdash/chains/typing.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-07 17:44:09.173197 langdash-1.7.1/langdash/classify/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-1.7.1/langdash/classify/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2032 2023-06-12 18:40:51.000000 langdash-1.7.1/langdash/classify/token_qa.py
--rw-rw-r--   0 user      (1000) user      (1000)     6738 2023-06-28 07:20:44.000000 langdash-1.7.1/langdash/core.py
--rw-rw-r--   0 user      (1000) user      (1000)     1341 2023-06-28 07:36:19.000000 langdash-1.7.1/langdash/infer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1661 2023-06-28 07:07:44.000000 langdash-1.7.1/langdash/llm.py
--rw-rw-r--   0 user      (1000) user      (1000)     9137 2023-06-28 07:27:22.000000 langdash-1.7.1/langdash/llm_session.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-07 17:44:09.181198 langdash-1.7.1/langdash/models/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-04 22:40:10.000000 langdash-1.7.1/langdash/models/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-07 17:44:09.181198 langdash-1.7.1/langdash/models/_mixins/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.7.1/langdash/models/_mixins/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3412 2023-06-21 10:26:00.000000 langdash-1.7.1/langdash/models/_mixins/tensor_based_infer_mixin.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-07 17:44:09.181198 langdash-1.7.1/langdash/models/_tokenizer/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.7.1/langdash/models/_tokenizer/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1886 2023-06-12 18:40:51.000000 langdash-1.7.1/langdash/models/_tokenizer/_bpe.py
--rw-rw-r--   0 user      (1000) user      (1000)     1532 2023-06-13 05:07:37.000000 langdash-1.7.1/langdash/models/_tokenizer/bytes_dict_tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)     2269 2023-06-21 10:26:00.000000 langdash-1.7.1/langdash/models/_tokenizer/hf_tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1546 2023-06-22 00:31:04.000000 langdash-1.7.1/langdash/models/_tokenizer/rwkv_tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)      664 2023-06-13 05:07:37.000000 langdash-1.7.1/langdash/models/_tokenizer/tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)     5280 2023-06-27 18:43:45.000000 langdash-1.7.1/langdash/models/ctransformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     4932 2023-06-27 18:24:11.000000 langdash-1.7.1/langdash/models/llama_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)      689 2023-06-06 03:06:05.000000 langdash-1.7.1/langdash/models/mock.py
--rw-rw-r--   0 user      (1000) user      (1000)     9063 2023-07-06 10:32:23.000000 langdash-1.7.1/langdash/models/rwkv_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)     1005 2023-06-12 18:40:51.000000 langdash-1.7.1/langdash/models/sentence_transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     5632 2023-06-27 18:22:06.000000 langdash-1.7.1/langdash/models/transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)      837 2023-06-06 03:06:05.000000 langdash-1.7.1/langdash/response.py
--rw-rw-r--   0 user      (1000) user      (1000)     3450 2023-06-14 22:44:24.000000 langdash-1.7.1/langdash/sampling.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-07 17:44:09.177197 langdash-1.7.1/langdash/search/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-1.7.1/langdash/search/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1135 2023-06-12 18:40:51.000000 langdash-1.7.1/langdash/search/embedding_search.py
--rw-rw-r--   0 user      (1000) user      (1000)     1118 2023-06-09 18:58:51.000000 langdash-1.7.1/langdash/search/engine.py
--rw-rw-r--   0 user      (1000) user      (1000)     2861 2023-06-19 07:37:15.000000 langdash-1.7.1/langdash/search/multichoice_search.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-07 17:44:09.177197 langdash-1.7.1/langdash.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     3724 2023-07-07 17:44:09.000000 langdash-1.7.1/langdash.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1654 2023-07-07 17:44:09.000000 langdash-1.7.1/langdash.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-07 17:44:09.000000 langdash-1.7.1/langdash.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      199 2023-07-07 17:44:09.000000 langdash-1.7.1/langdash.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        9 2023-07-07 17:44:09.000000 langdash-1.7.1/langdash.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-07 17:44:09.181198 langdash-1.7.1/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1604 2023-06-23 20:18:20.000000 langdash-1.7.1/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-08 23:55:09.778844 langdash-1.7.2/
+-rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-1.7.2/LICENSE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-1.7.2/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)     3647 2023-07-08 23:55:09.778844 langdash-1.7.2/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     2712 2023-07-08 22:51:09.000000 langdash-1.7.2/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-08 23:55:09.774843 langdash-1.7.2/langdash/
+-rw-rw-r--   0 user      (1000) user      (1000)       76 2023-07-08 22:57:58.000000 langdash-1.7.2/langdash/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-08 23:55:09.774843 langdash-1.7.2/langdash/chains/
+-rw-rw-r--   0 user      (1000) user      (1000)      177 2023-06-27 17:54:15.000000 langdash-1.7.2/langdash/chains/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    14903 2023-06-28 07:18:05.000000 langdash-1.7.2/langdash/chains/chains.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9394 2023-06-28 07:12:18.000000 langdash-1.7.2/langdash/chains/nodes.py
+-rw-rw-r--   0 user      (1000) user      (1000)      253 2023-06-11 03:43:22.000000 langdash-1.7.2/langdash/chains/typing.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-08 23:55:09.770842 langdash-1.7.2/langdash/classify/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-1.7.2/langdash/classify/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2032 2023-06-12 18:40:51.000000 langdash-1.7.2/langdash/classify/token_qa.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6738 2023-06-28 07:20:44.000000 langdash-1.7.2/langdash/core.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1341 2023-06-28 07:36:19.000000 langdash-1.7.2/langdash/infer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1661 2023-06-28 07:07:44.000000 langdash-1.7.2/langdash/llm.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9137 2023-06-28 07:27:22.000000 langdash-1.7.2/langdash/llm_session.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-08 23:55:09.774843 langdash-1.7.2/langdash/models/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-04 22:40:10.000000 langdash-1.7.2/langdash/models/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-08 23:55:09.774843 langdash-1.7.2/langdash/models/_mixins/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.7.2/langdash/models/_mixins/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3412 2023-06-21 10:26:00.000000 langdash-1.7.2/langdash/models/_mixins/tensor_based_infer_mixin.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-08 23:55:09.778844 langdash-1.7.2/langdash/models/_tokenizer/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.7.2/langdash/models/_tokenizer/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1886 2023-06-12 18:40:51.000000 langdash-1.7.2/langdash/models/_tokenizer/_bpe.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1532 2023-06-13 05:07:37.000000 langdash-1.7.2/langdash/models/_tokenizer/bytes_dict_tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2269 2023-06-21 10:26:00.000000 langdash-1.7.2/langdash/models/_tokenizer/hf_tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1546 2023-06-22 00:31:04.000000 langdash-1.7.2/langdash/models/_tokenizer/rwkv_tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)      664 2023-06-13 05:07:37.000000 langdash-1.7.2/langdash/models/_tokenizer/tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5280 2023-06-27 18:43:45.000000 langdash-1.7.2/langdash/models/ctransformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4932 2023-06-27 18:24:11.000000 langdash-1.7.2/langdash/models/llama_cpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)      689 2023-06-06 03:06:05.000000 langdash-1.7.2/langdash/models/mock.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10945 2023-07-08 23:00:42.000000 langdash-1.7.2/langdash/models/rwkv_cpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1005 2023-06-12 18:40:51.000000 langdash-1.7.2/langdash/models/sentence_transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5632 2023-06-27 18:22:06.000000 langdash-1.7.2/langdash/models/transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)      837 2023-06-06 03:06:05.000000 langdash-1.7.2/langdash/response.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3450 2023-06-14 22:44:24.000000 langdash-1.7.2/langdash/sampling.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-08 23:55:09.770842 langdash-1.7.2/langdash/search/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-1.7.2/langdash/search/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1135 2023-06-12 18:40:51.000000 langdash-1.7.2/langdash/search/embedding_search.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1118 2023-06-09 18:58:51.000000 langdash-1.7.2/langdash/search/engine.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2861 2023-06-19 07:37:15.000000 langdash-1.7.2/langdash/search/multichoice_search.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-08 23:55:09.774843 langdash-1.7.2/langdash.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     3647 2023-07-08 23:55:09.000000 langdash-1.7.2/langdash.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1654 2023-07-08 23:55:09.000000 langdash-1.7.2/langdash.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-08 23:55:09.000000 langdash-1.7.2/langdash.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      199 2023-07-08 23:55:09.000000 langdash-1.7.2/langdash.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        9 2023-07-08 23:55:09.000000 langdash-1.7.2/langdash.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-08 23:55:09.778844 langdash-1.7.2/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1604 2023-06-23 20:18:20.000000 langdash-1.7.2/setup.py
```

### Comparing `langdash-1.7.1/LICENSE.txt` & `langdash-1.7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langdash-1.7.1/PKG-INFO` & `langdash-1.7.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 1.7.1
+Version: 1.7.2
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 4 - Beta
@@ -21,16 +21,14 @@
 Provides-Extra: transformers
 Provides-Extra: ctransformers
 Provides-Extra: sentence_transformers
 License-File: LICENSE.txt
 
 # langdash
 
-[**Announcement post**](https://mysymphony.jp.net/a/langdash-announcement/)
-
 A simple library for interfacing with language models.
 
 **Currently in beta!**
 
 **Features:**
   
   * Support for text generation, text classification (through prompting) and vector-based document searching.
```

### Comparing `langdash-1.7.1/README.md` & `langdash-1.7.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # langdash
 
-[**Announcement post**](https://mysymphony.jp.net/a/langdash-announcement/)
-
 A simple library for interfacing with language models.
 
 **Currently in beta!**
 
 **Features:**
   
   * Support for text generation, text classification (through prompting) and vector-based document searching.
@@ -64,8 +62,8 @@
 ```
 python examples/instruct.py llama_cpp /path/to/ggml-wizardlm.bin -ae n_ctx 4096 --prompt-format wizardlm
 ```
 
 
 ## License
 
-Apache 2.0
+Apache 2.0
```

### Comparing `langdash-1.7.1/langdash/chains/chains.py` & `langdash-1.7.2/langdash/chains/chains.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.1/langdash/chains/nodes.py` & `langdash-1.7.2/langdash/chains/nodes.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.1/langdash/classify/token_qa.py` & `langdash-1.7.2/langdash/classify/token_qa.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.1/langdash/core.py` & `langdash-1.7.2/langdash/core.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.1/langdash/infer.py` & `langdash-1.7.2/langdash/infer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.1/langdash/llm.py` & `langdash-1.7.2/langdash/llm.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.1/langdash/llm_session.py` & `langdash-1.7.2/langdash/llm_session.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.1/langdash/models/_mixins/tensor_based_infer_mixin.py` & `langdash-1.7.2/langdash/models/_mixins/tensor_based_infer_mixin.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.1/langdash/models/_tokenizer/_bpe.py` & `langdash-1.7.2/langdash/models/_tokenizer/_bpe.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.1/langdash/models/_tokenizer/bytes_dict_tokenizer.py` & `langdash-1.7.2/langdash/models/_tokenizer/bytes_dict_tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.1/langdash/models/_tokenizer/hf_tokenizer.py` & `langdash-1.7.2/langdash/models/_tokenizer/hf_tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.1/langdash/models/_tokenizer/rwkv_tokenizer.py` & `langdash-1.7.2/langdash/models/_tokenizer/rwkv_tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.1/langdash/models/_tokenizer/tokenizer.py` & `langdash-1.7.2/langdash/models/_tokenizer/tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.1/langdash/models/ctransformers.py` & `langdash-1.7.2/langdash/models/ctransformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.1/langdash/models/llama_cpp.py` & `langdash-1.7.2/langdash/models/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.1/langdash/models/mock.py` & `langdash-1.7.2/langdash/models/mock.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.1/langdash/models/rwkv_cpp.py` & `langdash-1.7.2/langdash/models/rwkv_cpp.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import sys
 import torch
 import tokenizers  # type: ignore
 
 from langdash.llm import LLM
 from langdash.llm_session import LLMGenerationSessionForRawText, LLMState
 import langdash.sampling as sampling
-from ._tokenizer.rwkv_tokenizer import RwkvTokenizer
 from ._mixins.tensor_based_infer_mixin import TensorBasedInferMixin
 
 _rwkv_lib: Optional[str] = None
 _rwkv_cpp_folder: Optional[str] = None
 
 RWKV_CPP_COMMIT_DEFAULT = "84634c047a9831b16cdf1cc3f2626e0ef0b2373b"
 RWKV_CPP_COMMIT = os.environ.get(
@@ -90,14 +89,34 @@
     file_name = "librwkv.dylib"
   else:
     file_name = "librwkv.so"
 
   _rwkv_lib = os.path.join(_rwkv_cpp_folder, file_name)
 
   if force_recompile or not os.path.isfile(_rwkv_lib):
+
+    if os.environ.get("LANGDASH_RWKV_CPP_PATCH_MAX_NODES", "") == "1":
+      print("Patching rwkv.cpp's ggml...")
+      patch = shutil.which("patch")
+      if patch is None:
+        raise ImportError("patch is needed for compiling rwkv.cpp")
+      with open(
+        os.path.join(
+          os.path.dirname(langdash.__file__),
+          "extern/rwkv-cpp-ggml-max-nodes.patch"
+        ), "r"
+      ) as patch_file:
+        subprocess.run(
+          [patch, "-r", "-", "-N", "-p1"],
+          input=patch_file.read(),
+          text=True,
+          cwd=os.path.join(_rwkv_cpp_folder, "ggml"),
+          check=False
+        )
+
     cmake = shutil.which("cmake")
     if cmake is None:
       raise ImportError("cmake is needed for compiling rwkv.cpp")
     subprocess.check_call([cmake, "."], cwd=_rwkv_cpp_folder)
     subprocess.check_call(
       [cmake, "--build", ".", "--config", "Release"], cwd=_rwkv_cpp_folder
     )
@@ -127,48 +146,69 @@
 
 
 class RwkvCppWrapper:
 
   def __init__(self, llm: "RwkvCppModel"):
     assert _rwkv_lib is not None
     self.model = rwkv_cpp_model.RWKVModel(
-      rwkv_cpp_shared_library.RWKVSharedLibrary(_rwkv_lib), llm._model_path
+      rwkv_cpp_shared_library.RWKVSharedLibrary(_rwkv_lib), llm._model_path,
+      **llm._model_kwargs
     )
-    self.batch_size = llm.batch_size
+    self.batch_size = llm._batch_size
     if self.batch_size == 1:
       self.do_eval_sequence = False
     elif RWKV_CPP_ENABLE_EVAL_SEQUENCE:
       self.do_eval_sequence = hasattr(self.model, "eval_sequence")
     else:
       self.do_eval_sequence = False
     if llm._tokenizer_type == "20B":
+      from ._tokenizer.rwkv_tokenizer import RwkvTokenizer
       tokenizer = tokenizers.Tokenizer.from_file(llm._tokenizer_path)
+      self.tokenizer = RwkvTokenizer(tokenizer)
     elif llm._tokenizer_type == "world":
-      tokenizer = rwkv_tokenizer.TRIE_TOKENIZER(llm._tokenizer_path)
+      from ._tokenizer.bytes_dict_tokenizer import BytesDictTokenizer
+      tokenizer = rwkv_tokenizer.WorldTokenizer(llm._tokenizer_path)
+      mapping = [b""] * (len(tokenizer.index_to_token) + 1)
+      for k, v in tokenizer.index_to_token.items():
+        mapping[k] = v
+      self.tokenizer = BytesDictTokenizer(
+        encode_func=(lambda text, **_: tokenizer.encode(text)),
+        decode_func=(
+          lambda tokens, **_: tokenizer.decode_bytes(tokens).
+          decode("utf-8", errors="strict")
+        ),
+        mapping=mapping
+      )
     else:
       raise ValueError(f"unknown tokenizer type {llm._tokenizer_type}")
-    self.tokenizer = RwkvTokenizer(tokenizer)
     self.eos_token = 0
 
   def eval(self, tokid: int, state: torch.Tensor,
            logits_out: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor]:
     return self.model.eval(tokid, state, state, logits_out)
 
   def eval_mult(
     self, tokens: List[int], state: torch.Tensor, logits_out: torch.Tensor
   ) -> Tuple[torch.Tensor, torch.Tensor]:
+    try:
+      from tqdm import tqdm as progress
+    except ImportError:
+
+      def progress(v):
+        return v
+
     if self.do_eval_sequence:
       batch_size = self.batch_size
-      for i in range(0, len(tokens), batch_size):
+      for i in progress(range(0, len(tokens), batch_size)):
         logits_out, state = self.model.eval_sequence(
           tokens[i:i + batch_size], state, state, logits_out
         )
       return logits_out, state
     else:
-      for tokid in tokens[:-1]:
+      for tokid in progress(tokens[:-1]):
         _, state = self.model.eval(tokid, state, state, None)
       logits_out, state = self.model.eval(tokens[-1], state, state, logits_out)
       return logits_out, state
 
 
 class RwkvCppSession(
   TensorBasedInferMixin,
@@ -253,37 +293,54 @@
   Session = RwkvCppSession
 
   def __init__(
     self,
     model_path: str,
     tokenizer_path: Optional[str] = None,
     tokenizer_type: str = "20B",
-    batch_size: int = 2,
+    batch_size: int = 32,
+    **model_kwargs
   ):
     """
     Creates a template for the RWKV language model (using the rwkv.cpp library).
+  
+    You can pass the following environment variables to set compile flags:
+  
+    * LANGDASH_RWKV_CPP_COMMIT: hash of the commit to compile
+    * LANGDASH_RWKV_CPP_FORCE_RECOMPILE: '1' to force recompilation
+    * LANGDASH_RWKV_CPP_PATCH_MAX_NODES: '1' to patch the ggml library in rwkv.cpp
+    so that large batch_size works (> 1)
     
     Args:
       model_path (str): Path to the model file.
       tokenizer_path (Optional[str]):
         Path to the tokenizer file.
         Defaults to `None`. If not set, the built-in tokenizer will be used.
       tokenizer_type (str):
-        The type of tokenizer to use. Either `"world"` for world models or `"20B"` for anything else.
+        The type of tokenizer to use. Either `"world"` for world models
+        or `"20B"` for anything else.
+      batch_size (int):
+        The batch size for sequence evaluation.
+        Must be a positive integer (more than 0). If set to 1, serial evaluation
+        will always be used.
     """
+    
+    if not _rwkv_tokenizer_available and tokenizer_type != "20B":
+      raise ValueError("old RWKV tokenizer only supports '20B'")
+    if batch_size < 1:
+      raise ValueError("batch_size must be >= 1")
+    
     self._model_path = model_path
     self._tokenizer_type = tokenizer_type
-    if not _rwkv_tokenizer_available and self._tokenizer_type != "20B":
-      raise ValueError("old RWKV tokenizer only supports 20B")
     if tokenizer_path is None:
       builtin_tokenizer_paths = {
         "world": "rwkv/rwkv_vocab_v20230424.txt",
         "20B": "rwkv/20B_tokenizer.json",
       }
       assert _rwkv_cpp_folder is not None
       self._tokenizer_path = os.path.join(
         _rwkv_cpp_folder, builtin_tokenizer_paths[self._tokenizer_type]
       )
     else:
       self._tokenizer_path = tokenizer_path
-    self.batch_size = batch_size
-    assert self.batch_size >= 1, "batch_size must be >= 1"
+    self._batch_size = batch_size
+    self._model_kwargs = model_kwargs
```

### Comparing `langdash-1.7.1/langdash/models/sentence_transformers.py` & `langdash-1.7.2/langdash/models/sentence_transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.1/langdash/models/transformers.py` & `langdash-1.7.2/langdash/models/transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.1/langdash/response.py` & `langdash-1.7.2/langdash/response.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.1/langdash/sampling.py` & `langdash-1.7.2/langdash/sampling.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.1/langdash/search/embedding_search.py` & `langdash-1.7.2/langdash/search/embedding_search.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.1/langdash/search/engine.py` & `langdash-1.7.2/langdash/search/engine.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.1/langdash/search/multichoice_search.py` & `langdash-1.7.2/langdash/search/multichoice_search.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.1/langdash.egg-info/PKG-INFO` & `langdash-1.7.2/langdash.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 1.7.1
+Version: 1.7.2
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 4 - Beta
@@ -21,16 +21,14 @@
 Provides-Extra: transformers
 Provides-Extra: ctransformers
 Provides-Extra: sentence_transformers
 License-File: LICENSE.txt
 
 # langdash
 
-[**Announcement post**](https://mysymphony.jp.net/a/langdash-announcement/)
-
 A simple library for interfacing with language models.
 
 **Currently in beta!**
 
 **Features:**
   
   * Support for text generation, text classification (through prompting) and vector-based document searching.
```

### Comparing `langdash-1.7.1/langdash.egg-info/SOURCES.txt` & `langdash-1.7.2/langdash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langdash-1.7.1/setup.py` & `langdash-1.7.2/setup.py`

 * *Files identical despite different names*

