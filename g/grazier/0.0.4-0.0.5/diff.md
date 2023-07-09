# Comparing `tmp/grazier-0.0.4.tar.gz` & `tmp/grazier-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grazier-0.0.4.tar", last modified: Tue Jun 27 19:48:59 2023, max compression
+gzip compressed data, was "grazier-0.0.5.tar", last modified: Sun Jul  9 20:20:43 2023, max compression
```

## Comparing `grazier-0.0.4.tar` & `grazier-0.0.5.tar`

### file list

```diff
@@ -1,47 +1,56 @@
-drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-06-27 19:48:59.257970 grazier-0.0.4/
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     1181 2023-06-26 20:44:22.000000 grazier-0.0.4/LICENSE
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     9422 2023-06-27 19:48:59.257970 grazier-0.0.4/PKG-INFO
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     7000 2023-06-27 18:10:53.000000 grazier-0.0.4/README.md
-drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-06-27 19:48:59.253971 grazier-0.0.4/grazier/
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      303 2023-06-27 18:28:08.000000 grazier-0.0.4/grazier/__init__.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      764 2023-06-27 17:58:59.000000 grazier-0.0.4/grazier/cli.py
-drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-06-27 19:48:59.253971 grazier-0.0.4/grazier/engines/
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)        0 2023-06-26 19:09:44.000000 grazier-0.0.4/grazier/engines/__init__.py
-drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-06-27 19:48:59.257970 grazier-0.0.4/grazier/engines/chat/
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     3980 2023-06-27 19:47:51.000000 grazier-0.0.4/grazier/engines/chat/__init__.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     3374 2023-06-27 19:05:09.000000 grazier-0.0.4/grazier/engines/chat/anthropic_engine.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      824 2023-06-27 00:23:55.000000 grazier-0.0.4/grazier/engines/chat/anthropic_engine_test.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)    11381 2023-06-27 18:34:58.000000 grazier-0.0.4/grazier/engines/chat/bard_engine.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      760 2023-06-27 00:23:55.000000 grazier-0.0.4/grazier/engines/chat/bard_engine_test.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     8413 2023-06-27 19:28:37.000000 grazier-0.0.4/grazier/engines/chat/llama_engine.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      818 2023-06-27 00:23:55.000000 grazier-0.0.4/grazier/engines/chat/llama_engine_test.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     2817 2023-06-27 18:52:28.000000 grazier-0.0.4/grazier/engines/chat/openai_engine.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     1014 2023-06-27 00:23:55.000000 grazier-0.0.4/grazier/engines/chat/openai_engine_test.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     4910 2023-06-27 18:32:40.000000 grazier-0.0.4/grazier/engines/chat/stable_lm_engine.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      824 2023-06-27 00:23:55.000000 grazier-0.0.4/grazier/engines/chat/stable_lm_engine_test.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     3541 2023-06-27 19:02:43.000000 grazier-0.0.4/grazier/engines/chat/vertex_engine.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      815 2023-06-27 00:23:55.000000 grazier-0.0.4/grazier/engines/chat/vertex_engine_test.py
-drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-06-27 19:48:59.257970 grazier-0.0.4/grazier/engines/llm/
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     2850 2023-06-27 19:38:32.000000 grazier-0.0.4/grazier/engines/llm/__init__.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     1097 2023-06-27 19:36:25.000000 grazier-0.0.4/grazier/engines/llm/chat_engine.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     6285 2023-06-27 19:34:33.000000 grazier-0.0.4/grazier/engines/llm/huggingface_engine.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      794 2023-06-27 19:39:57.000000 grazier-0.0.4/grazier/engines/llm/huggingface_engine_test.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     2659 2023-06-27 19:12:30.000000 grazier-0.0.4/grazier/engines/llm/llama_engine.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      777 2023-06-27 00:23:55.000000 grazier-0.0.4/grazier/engines/llm/llama_engine_test.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     2243 2023-06-27 18:51:49.000000 grazier-0.0.4/grazier/engines/llm/openai_engine.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      835 2023-06-27 00:23:55.000000 grazier-0.0.4/grazier/engines/llm/openai_engine_test.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     2202 2023-06-27 19:01:26.000000 grazier-0.0.4/grazier/engines/llm/vertex_engine.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      574 2023-06-27 00:23:55.000000 grazier-0.0.4/grazier/engines/llm/vertex_engine_test.py
-drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-06-27 19:48:59.257970 grazier-0.0.4/grazier/utils/
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)        0 2023-06-26 19:11:27.000000 grazier-0.0.4/grazier/utils/__init__.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     2253 2023-06-26 20:25:42.000000 grazier-0.0.4/grazier/utils/python.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     1123 2023-06-26 21:00:23.000000 grazier-0.0.4/grazier/utils/pytorch.py
-drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-06-27 19:48:59.253971 grazier-0.0.4/grazier.egg-info/
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     9422 2023-06-27 19:48:59.000000 grazier-0.0.4/grazier.egg-info/PKG-INFO
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     1274 2023-06-27 19:48:59.000000 grazier-0.0.4/grazier.egg-info/SOURCES.txt
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)        1 2023-06-27 19:48:59.000000 grazier-0.0.4/grazier.egg-info/dependency_links.txt
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)       45 2023-06-27 19:48:59.000000 grazier-0.0.4/grazier.egg-info/entry_points.txt
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      187 2023-06-27 19:48:59.000000 grazier-0.0.4/grazier.egg-info/requires.txt
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)        8 2023-06-27 19:48:59.000000 grazier-0.0.4/grazier.egg-info/top_level.txt
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     2781 2023-06-27 19:48:34.000000 grazier-0.0.4/pyproject.toml
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)       38 2023-06-27 19:48:59.257970 grazier-0.0.4/setup.cfg
+drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-07-09 20:20:43.581528 grazier-0.0.5/
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     1181 2023-06-26 20:44:22.000000 grazier-0.0.5/LICENSE
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)    10582 2023-07-09 20:20:43.581528 grazier-0.0.5/PKG-INFO
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     8160 2023-07-03 19:47:02.000000 grazier-0.0.5/README.md
+drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-07-09 20:20:43.577528 grazier-0.0.5/grazier/
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      303 2023-06-27 18:28:08.000000 grazier-0.0.5/grazier/__init__.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     1031 2023-07-03 19:52:15.000000 grazier-0.0.5/grazier/cli.py
+drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-07-09 20:20:43.577528 grazier-0.0.5/grazier/engines/
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)        0 2023-06-26 19:09:44.000000 grazier-0.0.5/grazier/engines/__init__.py
+drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-07-09 20:20:43.577528 grazier-0.0.5/grazier/engines/chat/
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     5675 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/chat/__init__.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     3364 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/chat/anthropic_engine.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      828 2023-07-03 18:01:05.000000 grazier-0.0.5/grazier/engines/chat/anthropic_engine_test.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)    11368 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/chat/bard_engine.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      782 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/chat/bard_engine_test.py
+drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-07-09 20:20:43.577528 grazier-0.0.5/grazier/engines/chat/dolly/
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     4163 2023-07-03 18:18:59.000000 grazier-0.0.5/grazier/engines/chat/dolly/__init__.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     1584 2023-07-03 18:01:37.000000 grazier-0.0.5/grazier/engines/chat/dolly/dolly_engine_test.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     9237 2023-07-03 18:03:53.000000 grazier-0.0.5/grazier/engines/chat/dolly/instruct_pipeline.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)    12590 2023-07-03 19:44:12.000000 grazier-0.0.5/grazier/engines/chat/llama_engine.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      817 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/chat/llama_engine_test.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     3025 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/chat/openai_engine.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     1013 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/chat/openai_engine_test.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     4967 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/chat/stable_lm_engine.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      823 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/chat/stable_lm_engine_test.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     3501 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/chat/vertex_engine.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      814 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/chat/vertex_engine_test.py
+drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-07-09 20:20:43.581528 grazier-0.0.5/grazier/engines/llm/
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     3016 2023-07-03 19:54:15.000000 grazier-0.0.5/grazier/engines/llm/__init__.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     2109 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/llm/ai21_engine.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      631 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/llm/ai21_engine_test.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     1027 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/llm/chat_engine.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     8363 2023-07-03 19:53:19.000000 grazier-0.0.5/grazier/engines/llm/huggingface_engine.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      897 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/llm/huggingface_engine_test.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     2610 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/llm/llama_engine.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      806 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/llm/llama_engine_test.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     2164 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/llm/openai_engine.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      834 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/llm/openai_engine_test.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     2159 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/llm/vertex_engine.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      571 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/llm/vertex_engine_test.py
+drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-07-09 20:20:43.581528 grazier-0.0.5/grazier/utils/
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)        0 2023-06-26 19:11:27.000000 grazier-0.0.5/grazier/utils/__init__.py
+drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-07-09 20:20:43.581528 grazier-0.0.5/grazier/utils/llama/
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)    10917 2023-07-03 18:25:09.000000 grazier-0.0.5/grazier/utils/llama/convert_llama_weights_to_hf.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     7286 2023-07-03 18:26:09.000000 grazier-0.0.5/grazier/utils/llama/weight_diff.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     2258 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/utils/python.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     1123 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/utils/pytorch.py
+drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-07-09 20:20:43.577528 grazier-0.0.5/grazier.egg-info/
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)    10582 2023-07-09 20:20:43.000000 grazier-0.0.5/grazier.egg-info/PKG-INFO
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     1570 2023-07-09 20:20:43.000000 grazier-0.0.5/grazier.egg-info/SOURCES.txt
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)        1 2023-07-09 20:20:43.000000 grazier-0.0.5/grazier.egg-info/dependency_links.txt
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)       45 2023-07-09 20:20:43.000000 grazier-0.0.5/grazier.egg-info/entry_points.txt
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      197 2023-07-09 20:20:43.000000 grazier-0.0.5/grazier.egg-info/requires.txt
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)        8 2023-07-09 20:20:43.000000 grazier-0.0.5/grazier.egg-info/top_level.txt
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     2865 2023-07-09 20:20:22.000000 grazier-0.0.5/pyproject.toml
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)       38 2023-07-09 20:20:43.581528 grazier-0.0.5/setup.cfg
```

### Comparing `grazier-0.0.4/LICENSE` & `grazier-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `grazier-0.0.4/PKG-INFO` & `grazier-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grazier
-Version: 0.0.4
+Version: 0.0.5
 Summary: A tool for calling (and calling out to) large language models.
 Author-email: David Chan <davidchan@berkeley.edu>
 License: 
         Copyright 2023, Regents of the University of California
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -37,44 +37,54 @@
 # Grazier: Easily call Large Language Models from a unified API
 
 Grazier is a Python library for easily calling large language models from a unified API.
 
 ## Supported Large Language Models
 
 From OpenAI:
-- GPT-4 (Base, 32K) (Chat Engine)
-- GPT-3.5 (ChatGPT) (Chat Engine)
+- GPT-4 (Base, 32K) (Chat and Completion Engines)
+- GPT-3.5 (ChatGPT) (Chat and Completion Engines)
 - GPT-3 (Davinci (v2,v3), Ada, Babbage, Curie) (Completion Engine)
 
 From Anthropic:
-- Claude (Base, 100K) (Chat Engine)
-- Claude Instant (Base, 100K) (Chat Engine)
+- Claude (Base, 100K) (Chat and Completion Engines)
+- Claude Instant (Base, 100K) (Chat and Completion Engines)
 
 From Google/GCP:
 - PaLM (Chat and Completion Engines)
 
 From Huggingface
 - GPT-2 (Base, Medium, Large, XL) (Completion Engine)
 - GPT-Neo (125M, 1.3B, 2.7B) (Completion Engine)
 - GPT-J (6B) (Completion Engine)
+- Falcon (7B, 40B, rw-1B, rw-7B) (Completion Engine)
+- Dolly (v1 - 6B, v2 - 3B, 7B, 12B) (Chat and Completion Engines)
+- MPT (Instruct - 7B, 30B) (Chat and Completion Engines)
 
 From Facebook (via Huggingface)
 - Llama (7B, 13B, 30B, 65B) (Completion Engine)
 - OPT (125M, 350M, 1.3B, 2.7B, 6.7B, 13B, 30B, 66B) (Completion Engine)
 
 From Stanford (via Huggingface)
-- Alpaca (7B) (Chat Engine)
+- Alpaca (7B) (Chat and Completion Engines)
 
 From Berkeley (via Huggingface)
-- Koala (7B, 13B_v1, 13B_v2) (Chat Engine)
-- Vicuna (7B, 13B) (Chat Engine)
+- Koala (7B, 13B_v1, 13B_v2) (Chat and Completion Engines)
+- Vicuna (7B, 13B) (Chat and Completion Engines)
 
 From StabilityAI (via Huggingface)
 - StableLM (7B, 13B) (Chat and Completion Engines)
 
+From AllenAI (via Huggingface)
+- Tulu (7B, 13B, 30B, 65B) (Chat and Completion Engines)
+- Open Instruct (ShareGPT) (7B, 13B, 30B, 65B) (Chat and Completion Engines)
+
+From AI21
+- Jurassic 2 (Light, Mid, Ultra) (Completion Engines)
+
 
 ## Installation
 
 Grazier can easily be installed using pip:
 ```bash
 pip install grazier
 ```
@@ -172,30 +182,44 @@
 ```
 
 ### Huggingface Engines
 Most of the huggingface engines require no additional setup, however, some of the larger models require a GPU to run
 with any kind of efficiency (and some require multiple GPUs with large amounts of memory). You can find more details
 about the requirements for each model on the [Huggingface model hub](https://huggingface.co/models).
 
-### Llama, Alpaca, Koala, and Vicuna Engines
+### Llama, Alpaca, Koala, Vicuna and AllenAI Engines
 For these engines, you will need to obtain and postprocess the weights yourself (due to Facebook's licensing). You can
 find the instructions for doing so on each model page:
 - Llama: https://huggingface.co/docs/transformers/main/model_doc/llama
 - Alpaca: https://github.com/tatsu-lab/stanford_alpaca#recovering-alpaca-weights
 - Koala: https://github.com/young-geng/EasyLM/blob/main/docs/koala.md
 - Vicuna: https://github.com/lm-sys/FastChat#vicuna-weights
+- AllenAI: https://huggingface.co/allenai/tulu-65b
 
 Once the weights have been downloaded and processed, you can set the following environment variables to the root
-directory containing a folder for each variant (for example, `root_dir/llama_7B/weights.bin`, the root directory would
-be `root_dir`):
+directory containing a folder for each variant (The format is, `{root_dir}/{model-prefix}/weights.bin`, the root directory would
+be `root_dir`, and the model-prefix is the name of the model, e.g. `tulu-65b`):
 ```bash
 LLAMA_WEIGHTS_ROOT=<path to the llama weights>
 ALPACA_WEIGHTS_ROOT=<path to the alpaca weights>
 KOALA_WEIGHTS_ROOT=<path to the koala weights>
 VICUNA_WEIGHTS_ROOT=<path to the vicuna weights>
+ALLENAI_WEIGHTS_ROOT=<path to the allenai weights>
+```
+
+### AI21 Models (Jurassic)
+For AI21 models, you will need to set the `AI21_API_KEY` environment variable. You can find your API key at
+the [AI21 Studio Dashboard](https://studio.ai21.com/account/api-key). You can set this environment variable in
+your shell or in a `.env` file in the root of your project. For example, in a `.env` file, you would have:
+```bash
+AI21_API_KEY=<your key>
+```
+or on the command line:
+```bash
+export AI21_API_KEY=<your key>
 ```
 
 ## Citation
 
 If you use grazier in your work, please cite:
 
 ```
```

### Comparing `grazier-0.0.4/README.md` & `grazier-0.0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,54 @@
 # Grazier: Easily call Large Language Models from a unified API
 
 Grazier is a Python library for easily calling large language models from a unified API.
 
 ## Supported Large Language Models
 
 From OpenAI:
-- GPT-4 (Base, 32K) (Chat Engine)
-- GPT-3.5 (ChatGPT) (Chat Engine)
+- GPT-4 (Base, 32K) (Chat and Completion Engines)
+- GPT-3.5 (ChatGPT) (Chat and Completion Engines)
 - GPT-3 (Davinci (v2,v3), Ada, Babbage, Curie) (Completion Engine)
 
 From Anthropic:
-- Claude (Base, 100K) (Chat Engine)
-- Claude Instant (Base, 100K) (Chat Engine)
+- Claude (Base, 100K) (Chat and Completion Engines)
+- Claude Instant (Base, 100K) (Chat and Completion Engines)
 
 From Google/GCP:
 - PaLM (Chat and Completion Engines)
 
 From Huggingface
 - GPT-2 (Base, Medium, Large, XL) (Completion Engine)
 - GPT-Neo (125M, 1.3B, 2.7B) (Completion Engine)
 - GPT-J (6B) (Completion Engine)
+- Falcon (7B, 40B, rw-1B, rw-7B) (Completion Engine)
+- Dolly (v1 - 6B, v2 - 3B, 7B, 12B) (Chat and Completion Engines)
+- MPT (Instruct - 7B, 30B) (Chat and Completion Engines)
 
 From Facebook (via Huggingface)
 - Llama (7B, 13B, 30B, 65B) (Completion Engine)
 - OPT (125M, 350M, 1.3B, 2.7B, 6.7B, 13B, 30B, 66B) (Completion Engine)
 
 From Stanford (via Huggingface)
-- Alpaca (7B) (Chat Engine)
+- Alpaca (7B) (Chat and Completion Engines)
 
 From Berkeley (via Huggingface)
-- Koala (7B, 13B_v1, 13B_v2) (Chat Engine)
-- Vicuna (7B, 13B) (Chat Engine)
+- Koala (7B, 13B_v1, 13B_v2) (Chat and Completion Engines)
+- Vicuna (7B, 13B) (Chat and Completion Engines)
 
 From StabilityAI (via Huggingface)
 - StableLM (7B, 13B) (Chat and Completion Engines)
 
+From AllenAI (via Huggingface)
+- Tulu (7B, 13B, 30B, 65B) (Chat and Completion Engines)
+- Open Instruct (ShareGPT) (7B, 13B, 30B, 65B) (Chat and Completion Engines)
+
+From AI21
+- Jurassic 2 (Light, Mid, Ultra) (Completion Engines)
+
 
 ## Installation
 
 Grazier can easily be installed using pip:
 ```bash
 pip install grazier
 ```
@@ -136,30 +146,44 @@
 ```
 
 ### Huggingface Engines
 Most of the huggingface engines require no additional setup, however, some of the larger models require a GPU to run
 with any kind of efficiency (and some require multiple GPUs with large amounts of memory). You can find more details
 about the requirements for each model on the [Huggingface model hub](https://huggingface.co/models).
 
-### Llama, Alpaca, Koala, and Vicuna Engines
+### Llama, Alpaca, Koala, Vicuna and AllenAI Engines
 For these engines, you will need to obtain and postprocess the weights yourself (due to Facebook's licensing). You can
 find the instructions for doing so on each model page:
 - Llama: https://huggingface.co/docs/transformers/main/model_doc/llama
 - Alpaca: https://github.com/tatsu-lab/stanford_alpaca#recovering-alpaca-weights
 - Koala: https://github.com/young-geng/EasyLM/blob/main/docs/koala.md
 - Vicuna: https://github.com/lm-sys/FastChat#vicuna-weights
+- AllenAI: https://huggingface.co/allenai/tulu-65b
 
 Once the weights have been downloaded and processed, you can set the following environment variables to the root
-directory containing a folder for each variant (for example, `root_dir/llama_7B/weights.bin`, the root directory would
-be `root_dir`):
+directory containing a folder for each variant (The format is, `{root_dir}/{model-prefix}/weights.bin`, the root directory would
+be `root_dir`, and the model-prefix is the name of the model, e.g. `tulu-65b`):
 ```bash
 LLAMA_WEIGHTS_ROOT=<path to the llama weights>
 ALPACA_WEIGHTS_ROOT=<path to the alpaca weights>
 KOALA_WEIGHTS_ROOT=<path to the koala weights>
 VICUNA_WEIGHTS_ROOT=<path to the vicuna weights>
+ALLENAI_WEIGHTS_ROOT=<path to the allenai weights>
+```
+
+### AI21 Models (Jurassic)
+For AI21 models, you will need to set the `AI21_API_KEY` environment variable. You can find your API key at
+the [AI21 Studio Dashboard](https://studio.ai21.com/account/api-key). You can set this environment variable in
+your shell or in a `.env` file in the root of your project. For example, in a `.env` file, you would have:
+```bash
+AI21_API_KEY=<your key>
+```
+or on the command line:
+```bash
+export AI21_API_KEY=<your key>
 ```
 
 ## Citation
 
 If you use grazier in your work, please cite:
 
 ```
```

### Comparing `grazier-0.0.4/grazier/engines/chat/anthropic_engine.py` & `grazier-0.0.5/grazier/engines/chat/anthropic_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import logging
 import os
 from typing import Any, List
 
 import anthropic
 
 from grazier.engines.chat import Conversation, ConversationTurn, LLMChat, Speaker, register_engine
@@ -24,18 +23,15 @@
             "prompt": prompt,
         } | kwargs
 
         return self._client.completion(
             **kwargs,
         )
 
-    def call(
-        self, conversation: Conversation, n_completions: int = 1, **kwargs: Any
-    ) -> List[ConversationTurn]:
-
+    def call(self, conversation: Conversation, n_completions: int = 1, **kwargs: Any) -> List[ConversationTurn]:
         # Some odd anthropic assertions
         if conversation.turns[-1].speaker != Speaker.USER:
             raise AssertionError("Last turn must be a user turn")
         # Assert that conversations altrenate between user and AI (anthropic doesn't support system turns)
         for idx, turn in enumerate([c for c in conversation.turns if c.speaker != Speaker.SYSTEM]):
             if idx % 2 == 0 and turn.speaker != Speaker.USER:
                 raise AssertionError("Conversations must alternate between user and AI turns")
@@ -67,31 +63,37 @@
         return [ConversationTurn(text=s.strip(), speaker=Speaker.AI) for s in samples]
 
 
 @register_engine
 @singleton
 class Claude(AnthropicLMEngine):
     name = ("Claude", "claude")
+
     def __init__(self) -> None:
         super().__init__("claude-1")
 
+
 @register_engine
 @singleton
 class Claude100K(AnthropicLMEngine):
     name = ("Claude 100K", "claude-100k")
+
     def __init__(self) -> None:
         super().__init__("claude-1-100k")
 
 
 @register_engine
 @singleton
 class ClaudeInstant(AnthropicLMEngine):
     name = ("Claude Instant", "claude-instant")
+
     def __init__(self) -> None:
         super().__init__("claude-instant-1")
 
+
 @register_engine
 @singleton
 class ClaudeInstant100K(AnthropicLMEngine):
     name = ("Claude Instant 100K", "claude-instant-100k")
+
     def __init__(self) -> None:
         super().__init__("claude-instant-1-100k")
```

### Comparing `grazier-0.0.4/grazier/engines/chat/anthropic_engine_test.py` & `grazier-0.0.5/grazier/engines/chat/bard_engine_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-
 import logging
 
 import pytest
 
 from grazier.engines.chat import Conversation, LLMChat, Speaker
 
 
-@pytest.mark.parametrize("engine", ["claude-instant"])
-def test_llama_llm_engine(engine: str) -> None:
+@pytest.mark.parametrize("engine", ["bard"])
+def test_bard_llm_engine(engine: str) -> None:
     # Construct a conversation
     conversation = Conversation()
-    conversation.add_turn("You are an intelligent AI named Jason.", speaker=Speaker.SYSTEM)
-    conversation.add_turn("Your name, followed by a colon with the number 42 is:", speaker=Speaker.USER)
+    conversation.add_turn(
+        "You are an intelligent AI named Jason. Your name, followed by a colon with the number 42 is:",
+        speaker=Speaker.USER,
+    )
 
     _engine = LLMChat.from_string(engine)
     responses = _engine(conversation)
     for r in responses:
-        assert r.text.strip() != ''
-        if 'Jason' not in r.text:
+        assert r.text.strip() != ""
+        if "Jason" not in r.text:
             logging.warning(f'Name "Jason" not found in response "{r.text}"')
-        if '42' not in r.text:
+        if "42" not in r.text:
             logging.warning(f'Number "42" not found in response "{r.text}"')
```

### Comparing `grazier-0.0.4/grazier/engines/chat/bard_engine.py` & `grazier-0.0.5/grazier/engines/chat/bard_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         self._reqid = int("".join(random.choices(string.digits, k=4)))
         self.proxy = proxy
         self.conversation_id = ""
         self.response_id = ""
         self.choice_id = ""
         self.session_id = session_id
         self.session = httpx.AsyncClient(proxies=self.proxy)
-        self.session.headers = headers # type: ignore
+        self.session.headers = headers  # type: ignore
         self.session.cookies.set("__Secure-1PSID", session_id)
         self.timeout = timeout
 
     @classmethod
     async def create(
         cls,
         session_id: str,
@@ -266,14 +266,15 @@
         }
         self.conversation_id = results["conversation_id"]
         self.response_id = results["response_id"]
         self.choice_id = results["choices"][0]["id"]
         self._reqid += 100000
         return results
 
+
 @register_engine
 @singleton
 class BardEngine(LLMChat):
     name = ("Bard", "bard")
 
     def __init__(
         self,
@@ -283,18 +284,15 @@
         session_id = os.environ.get("GOOGLE_BARD_SESSION_ID", None)
         if session_id is None:
             raise Exception(
                 "GOOGLE_BARD_SESSION_ID environment variable not found. Please add it to your environment variables.",
             )
         self._chatbot = Chatbot(session_id=session_id)
 
-    def call(
-        self, conversation: Conversation, n_completions: int = 1, **kwargs: Any
-    ) -> List[ConversationTurn]:
-
+    def call(self, conversation: Conversation, n_completions: int = 1, **kwargs: Any) -> List[ConversationTurn]:
         if len(conversation.turns) != 1:
             raise AssertionError("BARD conversations must have exactly one turn.")
 
         # Extract the last user turn from the conversation.
         user_turn = conversation.turns[-1]
         new_prompt = user_turn.text
         if user_turn.speaker in (Speaker.SYSTEM, Speaker.AI):
```

### Comparing `grazier-0.0.4/grazier/engines/chat/bard_engine_test.py` & `grazier-0.0.5/grazier/engines/chat/anthropic_engine_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-
 import logging
 
 import pytest
 
 from grazier.engines.chat import Conversation, LLMChat, Speaker
 
 
-@pytest.mark.parametrize("engine", ["bard"])
-def test_bard_llm_engine(engine: str) -> None:
+@pytest.mark.parametrize("engine", ["claude-instant"])
+def test_anthropic_chat_engine(engine: str) -> None:
     # Construct a conversation
     conversation = Conversation()
-    conversation.add_turn("You are an intelligent AI named Jason. Your name, followed by a colon with the number 42 is:", speaker=Speaker.USER)
+    conversation.add_turn("You are an intelligent AI named Jason.", speaker=Speaker.SYSTEM)
+    conversation.add_turn("Your name, followed by a colon with the number 42 is:", speaker=Speaker.USER)
 
     _engine = LLMChat.from_string(engine)
     responses = _engine(conversation)
     for r in responses:
-        assert r.text.strip() != ''
-        if 'Jason' not in r.text:
+        assert r.text.strip() != ""
+        if "Jason" not in r.text:
             logging.warning(f'Name "Jason" not found in response "{r.text}"')
-        if '42' not in r.text:
+        if "42" not in r.text:
             logging.warning(f'Number "42" not found in response "{r.text}"')
```

### Comparing `grazier-0.0.4/grazier/engines/chat/llama_engine_test.py` & `grazier-0.0.5/grazier/engines/chat/llama_engine_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import logging
 
 import pytest
 
 from grazier.engines.chat import Conversation, LLMChat, Speaker
 
 
@@ -12,12 +11,12 @@
     conversation = Conversation()
     conversation.add_turn("You are an intelligent AI named Jason.", speaker=Speaker.SYSTEM)
     conversation.add_turn("Your name, followed by a colon with the number 42 is:", speaker=Speaker.USER)
 
     _engine = LLMChat.from_string(engine)
     responses = _engine(conversation)
     for r in responses:
-        assert r.text.strip() != ''
-        if 'Jason' not in r.text:
+        assert r.text.strip() != ""
+        if "Jason" not in r.text:
             logging.warning(f'Name "Jason" not found in response "{r.text}"')
-        if '42' not in r.text:
+        if "42" not in r.text:
             logging.warning(f'Number "42" not found in response "{r.text}"')
```

### Comparing `grazier-0.0.4/grazier/engines/chat/openai_engine.py` & `grazier-0.0.5/grazier/engines/chat/openai_engine.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,95 +1,106 @@
-
 import os
 from abc import abstractmethod
 from typing import Any, List
 
 import openai
 
 from grazier.engines.chat import Conversation, ConversationTurn, LLMChat, Speaker, register_engine
 from grazier.engines.llm.openai_engine import OpenAI
 from grazier.utils.python import retry, singleton
 
 # Setup openai api keys
 openai.organization = os.getenv("OPENAI_API_ORG", None)
 openai.api_key = os.getenv("OPENAI_API_KEY", None)
 
+
 class OpenAIChatEngine(LLMChat):
     def __init__(self, model: str):
         super().__init__(device="api")
         self._model = model
 
     @property
     @abstractmethod
     def cost_per_token(self) -> float:
         raise NotImplementedError()
 
-    @retry(
-        no_retry_on=(
-            openai.error.AuthenticationError,
-        )
-    )
+    @retry(no_retry_on=(openai.error.AuthenticationError,))
     def _retry_call(self, *args: Any, **kwargs: Any) -> Any:
-        return openai.ChatCompletion.create(*args, **kwargs) # type: ignore
-
+        return openai.ChatCompletion.create(*args, **kwargs)  # type: ignore
 
     def call(
         self,
         conversation: Conversation,
         n_completions: int = 1,
         **kwargs: Any,
     ) -> List[ConversationTurn]:
-
         # Construct the messages list from the conversation
         messages = []
         for turn in conversation.turns:
-            messages.append({
-                "role": "user" if turn.speaker == Speaker.USER else "system" if turn.speaker == Speaker.SYSTEM else "assistant" if turn.speaker == Speaker.AI else "user",
-                "content": turn.text,
-            })
+            messages.append(
+                {
+                    "role": "user"
+                    if turn.speaker == Speaker.USER
+                    else "system"
+                    if turn.speaker == Speaker.SYSTEM
+                    else "assistant"
+                    if turn.speaker == Speaker.AI
+                    else "user",
+                    "content": turn.text,
+                }
+            )
 
         # Update temperature and max_tokens
         kwargs["temperature"] = kwargs.get("temperature", 0.9)
         kwargs["max_tokens"] = kwargs.get("max_tokens", 150)
 
         # Call the OpenAI API
         cp = self._retry_call(
-                model=self._model,
-                messages=messages,
-                n=n_completions,
-                **kwargs,
+            model=self._model,
+            messages=messages,
+            n=n_completions,
+            **kwargs,
         )  # type: ignore
         OpenAI.USAGE += int(cp.usage.total_tokens) * self.cost_per_token
 
         return [
             ConversationTurn(
                 text=i.message.content,
-                speaker=Speaker.USER if i.message.role == "user" else Speaker.SYSTEM if i.message.role == "system" else Speaker.AI if i.message.role == "assistant" else Speaker.USER,
+                speaker=Speaker.USER
+                if i.message.role == "user"
+                else Speaker.SYSTEM
+                if i.message.role == "system"
+                else Speaker.AI
+                if i.message.role == "assistant"
+                else Speaker.USER,
             )
             for i in cp.choices
         ]
 
+
 @register_engine
 @singleton
 class ChatGPT(OpenAIChatEngine):
     name = ("Chat GPT", "chat-gpt")
     cost_per_token = 0.002 / 1000
 
     def __init__(self) -> None:
         super().__init__("gpt-3.5-turbo")
 
+
 @register_engine
 @singleton
 class GPT4(OpenAIChatEngine):
     name = ("GPT-4", "gpt4")
     cost_per_token = 0.03 / 1000
 
     def __init__(self) -> None:
         super().__init__("gpt-4")
 
+
 @register_engine
 @singleton
 class GPT432K(OpenAIChatEngine):
     name = ("GPT-4 32K", "gpt4-32k")
     cost_per_token = 0.06 / 1000
 
     def __init__(self) -> None:
```

### Comparing `grazier-0.0.4/grazier/engines/chat/openai_engine_test.py` & `grazier-0.0.5/grazier/engines/chat/openai_engine_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import logging
 import os
 
 import pytest
 
 from grazier.engines.chat import Conversation, LLMChat, Speaker
 
@@ -18,12 +17,12 @@
     conversation = Conversation()
     conversation.add_turn("You are an intelligent AI named Jason.", speaker=Speaker.SYSTEM)
     conversation.add_turn("Your name, followed by a colon with the number 42 is:", speaker=Speaker.USER)
 
     _engine = LLMChat.from_string(engine)
     responses = _engine(conversation)
     for r in responses:
-        assert r.text.strip() != ''
-        if 'Jason' not in r.text:
+        assert r.text.strip() != ""
+        if "Jason" not in r.text:
             logging.warning(f'Name "Jason" not found in response "{r.text}"')
-        if '42' not in r.text:
+        if "42" not in r.text:
             logging.warning(f'Number "42" not found in response "{r.text}"')
```

### Comparing `grazier-0.0.4/grazier/engines/chat/stable_lm_engine.py` & `grazier-0.0.5/grazier/engines/chat/stable_lm_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,44 +33,43 @@
         self._device = device
 
     def _decode_tokens(self, tokens: torch.Tensor, last_turn_is_user: bool) -> str:
         output = self._tokenizer.decode(tokens).strip()
         if last_turn_is_user:
             output, _, _ = output.partition("<|ASSISTANT|>")
         else:
-            output, _, _  = output.partition("<|USER|>")
+            output, _, _ = output.partition("<|USER|>")
 
         output = (
             output.replace("<|USER|>", "")
             .replace("<|ASSISTANT|>", "")
             .replace("<|SYSTEM|>", "")
             .replace("<|endoftext|>", "")
             .strip()
         )
         return output
 
-    def call(
-        self, conversation: Conversation, n_completions: int = 1, **kwargs: Any
-    ) -> List[ConversationTurn]:
-
+    def call(self, conversation: Conversation, n_completions: int = 1, **kwargs: Any) -> List[ConversationTurn]:
         # Build the prompt
-        prompt = ''
+        prompt = ""
         for idx, turn in enumerate(conversation.turns):
             if idx == 0:
                 if turn.speaker != Speaker.SYSTEM:
                     # Use the default prompt if the first turn is not from the system
                     prompt += StableLMChatEngine.SYSTEM_PROMPT
                 else:
                     prompt += turn.text
             elif turn.speaker == Speaker.USER:
-                    prompt += f"<|USER|>{turn.text}"
+                prompt += f"<|USER|>{turn.text}"
             elif turn.speaker == Speaker.AI:
                 prompt += f"<|ASSISTANT|>{turn.text}"
             elif turn.speaker == Speaker.SYSTEM:
-                logging.warning(f"System turn detected at index {idx} in conversation {conversation}. This turn will be ignored.")
+                logging.warning(
+                    f"System turn detected at index {idx} in conversation {conversation}. This turn will be ignored."
+                )
 
         # Add the beginning of the last turn
         last_turn_is_user = True
         if conversation.turns[-1].speaker == Speaker.AI:
             prompt += "<|USER|>"
             last_turn_is_user = False
         else:
@@ -97,23 +96,30 @@
                 max_new_tokens=256,
                 min_new_tokens=5,
                 num_return_sequences=n_completions,
                 do_sample=False,
                 stopping_criteria=StoppingCriteriaList([StopOnTokens()]),
             )
 
-        outputs = [self._decode_tokens(t[inputs['input_ids'].shape[-1]:], last_turn_is_user) for t in tokens]  # type: ignore
-        return [ConversationTurn(text=output, speaker=Speaker.AI if last_turn_is_user else Speaker.USER) for output in outputs]
+        outputs = [self._decode_tokens(t[inputs["input_ids"].shape[-1] :], last_turn_is_user) for t in tokens]  # type: ignore
+        return [
+            ConversationTurn(text=output, speaker=Speaker.AI if last_turn_is_user else Speaker.USER)
+            for output in outputs
+        ]
+
 
 @register_engine
 @singleton
 class StableLM3B(StableLMChatEngine):
     name = ("Stable LM (3B)", "stablelm-3b")
+
     def __init__(self, device: Optional[str] = None) -> None:
         super().__init__("stabilityai/stablelm-tuned-alpha-3b", device=device)
 
+
 @register_engine
 @singleton
 class StableLM7B(StableLMChatEngine):
     name = ("Stable LM (7B)", "stablelm-7b")
+
     def __init__(self, device: Optional[str] = None) -> None:
         super().__init__("stabilityai/stablelm-tuned-alpha-7b", device=device)
```

### Comparing `grazier-0.0.4/grazier/engines/chat/stable_lm_engine_test.py` & `grazier-0.0.5/grazier/engines/chat/vertex_engine_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-
 import logging
 
 import pytest
 
 from grazier.engines.chat import Conversation, LLMChat, Speaker
 
 
-@pytest.mark.parametrize("engine", ["stablelm-3b"])
-def test_stablelm_llm_engine(engine: str) -> None:
+@pytest.mark.parametrize("engine", ["palm"])
+def test_vertex_llm_engine(engine: str) -> None:
     # Construct a conversation
     conversation = Conversation()
     conversation.add_turn("You are an intelligent AI named Jason.", speaker=Speaker.SYSTEM)
     conversation.add_turn("Your name, followed by a colon with the number 42 is:", speaker=Speaker.USER)
 
     _engine = LLMChat.from_string(engine)
     responses = _engine(conversation)
     for r in responses:
-        assert r.text.strip() != ''
-        if 'Jason' not in r.text:
+        assert r.text.strip() != ""
+        if "Jason" not in r.text:
             logging.warning(f'Name "Jason" not found in response "{r.text}"')
-        if '42' not in r.text:
+        if "42" not in r.text:
             logging.warning(f'Number "42" not found in response "{r.text}"')
```

### Comparing `grazier-0.0.4/grazier/engines/chat/vertex_engine.py` & `grazier-0.0.5/grazier/engines/chat/vertex_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 try:
     from vertexai.preview.language_models import ChatModel, InputOutputTextPair
 except ImportError:
     ChatModel = None
     InputOutputTextPair = None
 
 from typing import Any, Dict, List
@@ -23,71 +22,67 @@
         self._model = ChatModel.from_pretrained(model)
         self._parameters = {
             "max_output_tokens": 256,  # Token limit determines the maximum amount of text output.
             "top_p": 0.95,  # Tokens are selected from most probable to least until the sum of their probabilities equals the top_p value.
             "top_k": 40,  # A top_k of 1 means the selected token is the most probable among all tokens.
         } | kwargs
 
-    @sleep_and_retry # type: ignore
-    @limits( # type: ignore
+    @sleep_and_retry  # type: ignore
+    @limits(  # type: ignore
         calls=40, period=60
     )  # This is the default rate limit for Vertex AI (actual rate limit is 60 calls per minute, but we'll be conservative)
     def _rate_limited_model_predict(self, info, **kwargs: Any) -> Any:
         context, examples, prompt = info
-        chat = self._model.start_chat(
-            context=context,
-            examples=examples,
-            **kwargs
-        )
+        chat = self._model.start_chat(context=context, examples=examples, **kwargs)
         response = chat.send_message(prompt).text
 
         return response
 
-    def call(
-        self, conversation: Conversation, n_completions: int = 1, **kwargs: Any
-    ) -> List[ConversationTurn]:
-
+    def call(self, conversation: Conversation, n_completions: int = 1, **kwargs: Any) -> List[ConversationTurn]:
         # Start the chat
         system_turns = [c for c in conversation.turns if c.speaker == Speaker.SYSTEM]
-        context = system_turns[-1].text if system_turns else ''
+        context = system_turns[-1].text if system_turns else ""
         non_system_turns = [c for c in conversation.turns if c.speaker != Speaker.SYSTEM]
 
         # Assert that the non-system turns alternate between the user and the agent
         for idx, turn in enumerate(non_system_turns):
             if idx % 2 == 0:
                 assert turn.speaker == Speaker.USER
             else:
                 assert turn.speaker == Speaker.AI
         if len(non_system_turns) > 1:
             assert non_system_turns[-1].speaker == Speaker.USER
             assert InputOutputTextPair is not None
             # Build the examples
             examples = [
-                InputOutputTextPair(
-                    input_text=non_system_turns[i].text,
-                    output_text=non_system_turns[i + 1].text
-                ) for i in range(0, len(non_system_turns) - 1, 2)
+                InputOutputTextPair(input_text=non_system_turns[i].text, output_text=non_system_turns[i + 1].text)
+                for i in range(0, len(non_system_turns) - 1, 2)
             ]
         else:
             examples = []
 
         # Normalize kwargs from openai to vertexai (some common parameters are different)
-        kwargs = self._parameters | {
-            "max_output_tokens": kwargs.pop('max_output_tokens', kwargs.pop('max_tokens', 256)),
-            "temperature": kwargs.pop('temperature', 1.0),
-        } | kwargs
-
+        kwargs = (
+            self._parameters
+            | {
+                "max_output_tokens": kwargs.pop("max_output_tokens", kwargs.pop("max_tokens", 256)),
+                "temperature": kwargs.pop("temperature", 1.0),
+            }
+            | kwargs
+        )
 
         return [
-            ConversationTurn(self._rate_limited_model_predict(
-                (context, examples, non_system_turns[-1].text),
-                **kwargs
-            ), speaker=Speaker.AI)  # type: ignore
+            ConversationTurn(
+                self._rate_limited_model_predict((context, examples, non_system_turns[-1].text), **kwargs),
+                speaker=Speaker.AI,
+            )  # type: ignore
             for _ in range(n_completions)
         ]
 
+
 @register_engine
 @singleton
 class PaLMEngine(VertexLLMEngine):
     name = ("PaLM", "palm")
+
     def __init__(self) -> None:
         super().__init__("chat-bison@001")
```

### Comparing `grazier-0.0.4/grazier/engines/chat/vertex_engine_test.py` & `grazier-0.0.5/grazier/engines/chat/stable_lm_engine_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-
 import logging
 
 import pytest
 
 from grazier.engines.chat import Conversation, LLMChat, Speaker
 
 
-@pytest.mark.parametrize("engine", ["palm"])
-def test_vertex_llm_engine(engine: str) -> None:
+@pytest.mark.parametrize("engine", ["stablelm-3b"])
+def test_stablelm_llm_engine(engine: str) -> None:
     # Construct a conversation
     conversation = Conversation()
     conversation.add_turn("You are an intelligent AI named Jason.", speaker=Speaker.SYSTEM)
     conversation.add_turn("Your name, followed by a colon with the number 42 is:", speaker=Speaker.USER)
 
     _engine = LLMChat.from_string(engine)
     responses = _engine(conversation)
     for r in responses:
-        assert r.text.strip() != ''
-        if 'Jason' not in r.text:
+        assert r.text.strip() != ""
+        if "Jason" not in r.text:
             logging.warning(f'Name "Jason" not found in response "{r.text}"')
-        if '42' not in r.text:
+        if "42" not in r.text:
             logging.warning(f'Number "42" not found in response "{r.text}"')
```

### Comparing `grazier-0.0.4/grazier/engines/llm/__init__.py` & `grazier-0.0.5/grazier/engines/llm/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,95 +4,89 @@
 
 from huggingface_hub import HfApi, ModelFilter
 
 from grazier.utils.pytorch import select_device
 
 
 class LLMEngine(ABC):
-
     @property
     @abstractmethod
     def name(self) -> Tuple[str, str]:
-        """ Returns a tuple of (Pretty Name, CLI name) of the language model. """
+        """Returns a tuple of (Pretty Name, CLI name) of the language model."""
         raise NotImplementedError()
 
     def __init__(self, device: Optional[str] = None) -> None:
         self.device = select_device(device)
 
-
     @property
     def prompt_prefix(self) -> str:
         return ""
 
     @property
     def prompt_suffix(self) -> str:
         return ""
 
-    def __call__(
-        self,
-        prompt: str,
-        n_completions: int = 1,
-        **kwargs: Any
-    ) -> List[str]:
+    def __call__(self, prompt: str, n_completions: int = 1, **kwargs: Any) -> List[str]:
         prompt = self.prompt_prefix + prompt + self.prompt_suffix
         return self.call(prompt, n_completions, **kwargs)
 
-
     @abstractmethod
-    def call(
-        self,
-        prompt: str,
-        n_completions: int = 1,
-        **kwargs: Any
-    ) -> List[str]:
+    def call(self, prompt: str, n_completions: int = 1, **kwargs: Any) -> List[str]:
         raise NotImplementedError()
 
     def __repr__(
         self,
     ) -> str:
         return f"{self.__class__.__name__}({self.name[0]})"
 
+    @classmethod
+    def configure(cls, *args, **kwargs):
+        raise NotImplementedError("This engine does not support automated configuration.")
 
     @staticmethod
     def from_string(typestr: str, **kwargs: Any) -> "LLMEngine":
-
         if typestr in LM_ENGINES:
             return LM_ENGINES[typestr](**kwargs)  # type: ignore
         elif typestr in LM_ENGINES_CLI:
             return LM_ENGINES_CLI[typestr](**kwargs)  # type: ignore
 
         logging.info(f"Failed to find local LLM matching {typestr}. Fetching remote LLMs...")
         api = HfApi()
-        models = list(api.list_models(filter=ModelFilter(model_name=typestr, task='text-generation')))
+        models = list(api.list_models(filter=ModelFilter(model_name=typestr, task="text-generation")))
         if len(models) > 0:
             return HuggingFaceTextGenerationLMEngine.from_hub_model(typestr)(**kwargs)
 
         raise ValueError(f"Invalid language model type: {typestr}")
 
-
     @staticmethod
     def list_models() -> List[str]:
         return list(LM_ENGINES_CLI.keys())
 
+
 LM_ENGINES: Dict[str, Type[LLMEngine]] = {}
 LM_ENGINES_CLI: Dict[str, Type[LLMEngine]] = {}
 
 T = TypeVar("T")
-def register_engine(cls: T) -> T:
 
-    LM_ENGINES[cls.name[0]] = cls # type: ignore
-    LM_ENGINES_CLI[cls.name[1]] = cls # type: ignore
+
+def register_engine(cls: T) -> T:
+    LM_ENGINES[cls.name[0]] = cls  # type: ignore
+    LM_ENGINES_CLI[cls.name[1].lower()] = cls  # type: ignore
     return cls
 
+
 def register_chat_engine(cls: T) -> T:
-    LM_ENGINES[cls.name[0]] = cls # type: ignore
+    LM_ENGINES[cls.name[0]] = cls  # type: ignore
     if cls.name[1] not in LM_ENGINES_CLI:
-        LM_ENGINES_CLI[cls.name[1]] = cls # type: ignore
-    LM_ENGINES_CLI[f'{cls.name[1]}-chat'] = cls # type: ignore
+        LM_ENGINES_CLI[cls.name[1].lower()] = cls  # type: ignore
+
+    LM_ENGINES_CLI[f"{cls.name[1]}-chat".lower()] = cls  # type: ignore
 
     return cls
 
+
 # Imports for engine modules
+from grazier.engines.llm.ai21_engine import *  # noqa: F403, E402
 from grazier.engines.llm.huggingface_engine import *  # noqa: F403, E402
 from grazier.engines.llm.llama_engine import *  # noqa: F403, E402
 from grazier.engines.llm.openai_engine import *  # noqa: F403, E402
 from grazier.engines.llm.vertex_engine import *  # noqa: F403, E402
```

### Comparing `grazier-0.0.4/grazier/engines/llm/chat_engine.py` & `grazier-0.0.5/grazier/engines/llm/chat_engine.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,31 @@
-
-from typing import Any, List, Optional, Type
+from typing import Any, List, Type
 
 from grazier.engines.chat import Conversation, Speaker
 from grazier.engines.llm import LLMEngine
 
 
-def wrap_chat_llm_engine(cls) -> Type[LLMEngine]: # type: ignore
+def wrap_chat_llm_engine(cls) -> Type[LLMEngine]:  # type: ignore
     """
     Wrap an LLMChat engine to make it compatible with the LLMEngine interface.
 
     Args:
         cls (Type[LLMChat]): The LLMChat engine to wrap.
 
     Returns:
         Type[LLMEngine]: The wrapped LLMEngine.
     """
 
     class _WrappedEngine(LLMEngine):
-
-        name = (f'{cls.name[0]} (Chat)', f'{cls.name[1]}')
+        name = (f"{cls.name[0]} (Chat)", f"{cls.name[1]}")
 
         def __init__(self, **kwargs: Any) -> None:
             super().__init__(device="defer")
             self._engine = cls(**kwargs)
 
-        def call(
-            self,
-            prompt: str,
-            n_completions: int = 1,
-            **kwargs: Any
-        ) -> List[str]:
+        def call(self, prompt: str, n_completions: int = 1, **kwargs: Any) -> List[str]:
             # Build a conversation
             conversation = Conversation()
             conversation.add_turn(prompt, speaker=Speaker.USER)
             return [x.text for x in self._engine.call(conversation, n_completions=n_completions, **kwargs)]
 
-
     return _WrappedEngine
```

### Comparing `grazier-0.0.4/grazier/engines/llm/huggingface_engine_test.py` & `grazier-0.0.5/grazier/engines/llm/huggingface_engine_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,33 @@
-
 import logging
 import random
 
 import pytest
 
 from grazier.engines.llm import LLMEngine
 
 
-@pytest.mark.parametrize("engine", [
-    "gptj-6B",
-    "gpt2",
-    "gpt2-med",
-    "gpt2-lg",
-    "gpt2-xl",
-    "distilgpt2",
-    "gptneo-125M",
-    "gptneo-1.3B",
-    "gptneo-2.7B",
-    "stablelm-3B",
-    "stablelm-7B",
-])
+@pytest.mark.parametrize(
+    "engine",
+    [
+        "gptj-6B",
+        "gpt2",
+        "gpt2-med",
+        "gpt2-lg",
+        "gpt2-xl",
+        "distilgpt2",
+        "gptneo-125M",
+        "gptneo-1.3B",
+        "gptneo-2.7B",
+        "stablelm-3B",
+        "stablelm-7B",
+        "falcon-7b",
+        "falcon-rw-1b",
+    ],
+)
 def test_huggingface_llm_engine(engine: str) -> None:
     _engine = LLMEngine.from_string(engine)
     random_number = random.randint(0, 100)
     response = _engine(f"My name, followed by a colon with the number {random_number} is:")
 
     for r in response:
         if len(r.strip()) == 0:
```

### Comparing `grazier-0.0.4/grazier/engines/llm/llama_engine.py` & `grazier-0.0.5/grazier/engines/llm/llama_engine.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,80 +1,82 @@
-
 import os
 from typing import Any, List, Optional
 
 from transformers import LlamaForCausalLM, LlamaTokenizer
 
 from grazier.engines.llm import LLMEngine, register_engine
 from grazier.utils.python import singleton
 
 
 class HuggingFaceLlamaLMEngine(LLMEngine):
-    def __init__(self,
-                model: str,
-                weight_root: str,
-                max_new_tokens: int = 128,
-                device: Optional[str] = None,
+    def __init__(
+        self,
+        model: str,
+        weight_root: str,
+        max_new_tokens: int = 128,
+        device: Optional[str] = None,
     ) -> None:
         super().__init__(device=device)
         self._max_new_tokens = max_new_tokens
         self.tokenizer = LlamaTokenizer.from_pretrained(f"{os.environ.get(weight_root, '')}{model}")
         self._generator = LlamaForCausalLM.from_pretrained(
             f"{os.environ.get(weight_root, '')}{model}", device_map="auto"
         )
 
-    def call(
-        self, prompt: str, n_completions: int = 1, **kwargs: Any
-    ) -> List[str]:
+    def call(self, prompt: str, n_completions: int = 1, **kwargs: Any) -> List[str]:
         input = self.tokenizer(prompt, return_tensors="pt").input_ids.to(self._generator.device)
 
         # Handle the kwargs
         _params = {
-            'max_new_tokens': kwargs.get("max_new_tokens", kwargs.pop('max_tokens', self._max_new_tokens)),
-            'num_return_sequences': n_completions,
-            'temperature': kwargs.get("temperature", None),
+            "max_new_tokens": kwargs.get("max_new_tokens", kwargs.pop("max_tokens", self._max_new_tokens)),
+            "num_return_sequences": n_completions,
+            "temperature": kwargs.get("temperature", None),
         } | kwargs
 
         outputs = self._generator.generate(
-                input,
-                do_sample=n_completions > 1,
-                **_params,
-            )
+            input,
+            do_sample=n_completions > 1,
+            **_params,
+        )
 
         # Strip the prompt from the output
-        outputs = outputs[:, input.shape[-1]:]
+        outputs = outputs[:, input.shape[-1] :]
         # Decode and return the output
         outputs = self.tokenizer.batch_decode(outputs, skip_special_tokens=True, clean_up_tokenization_spaces=False)
 
         return outputs
 
+
 @register_engine
 @singleton
 class Llama7B(HuggingFaceLlamaLMEngine):
     name = ("LLAMA 7B", "llama-7B")
 
     def __init__(self, device: Optional[str] = "defer") -> None:
         super().__init__("7B", "LLAMA_WEIGHTS_ROOT", device=device)
 
+
 @register_engine
 @singleton
 class Llama13B(HuggingFaceLlamaLMEngine):
     name = ("LLAMA 13B", "llama-13B")
 
     def __init__(self, device: Optional[str] = "defer") -> None:
         super().__init__("13B", "LLAMA_WEIGHTS_ROOT", device=device)
 
+
 @register_engine
 @singleton
 class Llama30B(HuggingFaceLlamaLMEngine):
     name = ("LLAMA 30B", "llama-30B")
 
     def __init__(self, device: Optional[str] = "defer") -> None:
         super().__init__("30B", "LLAMA_WEIGHTS_ROOT", device=device)
 
+
 @register_engine
 @singleton
 class Llama65B(HuggingFaceLlamaLMEngine):
     name = ("LLAMA 65B", "llama-65B")
 
     def __init__(self, device: Optional[str] = "defer") -> None:
         super().__init__("65B", "LLAMA_WEIGHTS_ROOT", device=device)
```

### Comparing `grazier-0.0.4/grazier/engines/llm/llama_engine_test.py` & `grazier-0.0.5/grazier/engines/llm/llama_engine_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-
 import logging
 import random
 
 import pytest
 
 from grazier.engines.llm import LLMEngine
 
 
-@pytest.mark.parametrize("engine", [
-    "llama-7B",
-    "llama-13B",
-    "llama-30B",
-    "llama-60B",
-])
+@pytest.mark.parametrize(
+    "engine",
+    [
+        "llama-7B",
+        "llama-13B",
+        "llama-30B",
+        "llama-60B",
+    ],
+)
 def test_huggingface_llm_engine(engine: str) -> None:
-
     if engine in (
         "llama-13B",
         "llama-30B",
         "llama-60B",
     ):
         pytest.skip("Model too large for CI")
```

### Comparing `grazier-0.0.4/grazier/engines/llm/openai_engine.py` & `grazier-0.0.5/grazier/engines/llm/openai_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-
 import os
 from abc import abstractmethod
-from typing import Any, List, Optional
+from typing import Any, List
 
 import openai
 
 from grazier.engines.llm import LLMEngine, register_engine
 from grazier.utils.python import retry, singleton
 
 # Setup openai api keys
@@ -15,74 +14,70 @@
 
 @singleton
 class OpenAI:
     USAGE = 0.0
 
 
 class OpenAICompletionLLMEngine(LLMEngine):
-
     @property
     @abstractmethod
     def cost_per_token(self) -> float:
         raise NotImplementedError()
 
     def __init__(self, model: str):
         self._model = model
-        super().__init__(device='api')
+        super().__init__(device="api")
 
-    @retry(
-        no_retry_on=(
-            openai.error.AuthenticationError,
-        )
-    )
-    def call(
-        self, prompt: str, n_completions: int = 1, **kwargs: Any
-    ) -> List[str]:
-        cp = openai.Completion.create(
-            model=self._model, prompt=prompt, n=n_completions, **kwargs
-        )  # type: ignore
+    @retry(no_retry_on=(openai.error.AuthenticationError,))
+    def call(self, prompt: str, n_completions: int = 1, **kwargs: Any) -> List[str]:
+        cp = openai.Completion.create(model=self._model, prompt=prompt, n=n_completions, **kwargs)  # type: ignore
         OpenAI.USAGE += int(cp.usage.total_tokens) * self.cost_per_token
         return [i.text for i in cp.choices]  # type: ignore
 
+
 @register_engine
 @singleton
 class GPT3Davinci3(OpenAICompletionLLMEngine):
     cost_per_token = 0.02 / 1000
     name = ("GPT-3 Davinci", "gpt3-davinci3")
 
     def __init__(self) -> None:
         super().__init__("text-davinci-003")
 
+
 @register_engine
 @singleton
 class GPT3Davinci2(OpenAICompletionLLMEngine):
     cost_per_token = 0.03 / 1000
     name = ("GPT-3 Davinci", "gpt3-davinci2")
 
     def __init__(self) -> None:
         super().__init__("text-davinci-002")
 
+
 @register_engine
 @singleton
 class GPT3Curie(OpenAICompletionLLMEngine):
     cost_per_token = 0.002 / 1000
     name = ("GPT-3 Curie", "gpt3-curie")
 
     def __init__(self) -> None:
         super().__init__("text-curie-001")
 
+
 @register_engine
 @singleton
 class GPT3Babbage(OpenAICompletionLLMEngine):
     cost_per_token = 0.02 / 1000
     name = ("GPT-3 Babbage", "gpt3-babbage")
 
     def __init__(self) -> None:
         super().__init__("text-babbage-001")
 
+
 @register_engine
 @singleton
 class GPT3Ada(OpenAICompletionLLMEngine):
     cost_per_token = 0.02 / 1000
     name = ("GPT-3 Ada", "gpt3-ada")
 
     def __init__(self) -> None:
```

### Comparing `grazier-0.0.4/grazier/engines/llm/openai_engine_test.py` & `grazier-0.0.5/grazier/engines/llm/openai_engine_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import logging
 import os
 import random
 
 import pytest
 
 from grazier.engines.llm import LLMEngine
```

### Comparing `grazier-0.0.4/grazier/engines/llm/vertex_engine.py` & `grazier-0.0.5/grazier/engines/llm/vertex_engine.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-
 try:
     from vertexai.preview.language_models import TextGenerationModel
 except ImportError:
     TextGenerationModel = None
 
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List
 
 from ratelimit import limits, sleep_and_retry
 
 from grazier.engines.llm import LLMEngine, register_engine
 from grazier.utils.python import singleton
 
 
@@ -16,44 +15,40 @@
     def __init__(self, model: str, **kwargs: Dict[str, Any]) -> None:
         if TextGenerationModel is None:
             raise ImportError("Please install the Vertex AI SDK to use this LM engine.")
 
         self._model = TextGenerationModel.from_pretrained(model)
         self._parameters = {
             # Token limit determines the maximum amount of text output.
-            "max_output_tokens": kwargs.pop('max_output_tokens', kwargs.pop('max_tokens', 256)),
+            "max_output_tokens": kwargs.pop("max_output_tokens", kwargs.pop("max_tokens", 256)),
             "top_p": 0.95,  # Tokens are selected from most probable to least until the sum of their probabilities equals the top_p value.
             "top_k": 40,  # A top_k of 1 means the selected token is the most probable among all tokens.
         } | kwargs
 
-    @sleep_and_retry # type: ignore
-    @limits( # type: ignore
+    @sleep_and_retry  # type: ignore
+    @limits(  # type: ignore
         calls=40, period=60
     )  # This is the default rate limit for Vertex AI (actual rate limit is 60 calls per minute, but we'll be conservative)
     def _rate_limited_model_predict(self, *args: Any, **kwargs: Any) -> Any:
         return self._model.predict(*args, **kwargs)
 
-    def call(
-        self, prompt: str, n_completions: int = 1, **kwargs: Any
-    ) -> List[str]:
-
+    def call(self, prompt: str, n_completions: int = 1, **kwargs: Any) -> List[str]:
         # Normalize kwargs from openai to vertexai (some common parameters are different)
-        kwargs = self._parameters | {
-            "max_output_tokens": kwargs.pop('max_output_tokens', kwargs.pop('max_tokens', 256)),
-            "temperature": kwargs.pop('temperature', 1.0),
-        } | kwargs
+        kwargs = (
+            self._parameters
+            | {
+                "max_output_tokens": kwargs.pop("max_output_tokens", kwargs.pop("max_tokens", 256)),
+                "temperature": kwargs.pop("temperature", 1.0),
+            }
+            | kwargs
+        )
 
+        return [self._rate_limited_model_predict(prompt, **kwargs).text for _ in range(n_completions)]  # type: ignore
 
-        return [
-            self._rate_limited_model_predict(
-                prompt,
-                **kwargs
-            ).text  # type: ignore
-            for _ in range(n_completions)
-        ]
 
 @register_engine
 @singleton
 class PaLMEngine(VertexLLMEngine):
     name = ("PaLM", "palm")
+
     def __init__(self) -> None:
         super().__init__("text-bison@001")
```

### Comparing `grazier-0.0.4/grazier/utils/python.py` & `grazier-0.0.5/grazier/utils/python.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,18 +21,21 @@
     def __enter__(self) -> None:
         self._old_cwd.append(os.getcwd())
         os.chdir(self.path)
 
     def __exit__(self, *excinfo) -> None:  # type: ignore
         os.chdir(self._old_cwd.pop())
 
+
 Q = TypeVar("Q", bound=Callable[..., Any])
 
+
 def retry(no_retry_on: Optional[Collection[Type[Exception]]] = None) -> Callable[[Q], Q]:
     """Retry a function if it throws an exception."""
+
     def decorator(func: Q) -> Q:
         @functools.wraps(func)
         def wrapper(*args: Any, **kwargs: Any) -> Any:
             error = None
             for backoff in [0.1, 0.2, 0.5, 1.0, 2.0, 5.0, 10.0]:
                 try:
                     return func(*args, **kwargs)
@@ -42,17 +45,17 @@
 
                     # Backoff and try again
                     time.sleep(backoff)
                     error = e
                     continue
 
             if error is not None:
-                raise error # type: ignore
+                raise error  # type: ignore
 
-        return wrapper # type: ignore
+        return wrapper  # type: ignore
 
     return decorator
 
 
 T = TypeVar("T")
 S = TypeVar("S")
```

### Comparing `grazier-0.0.4/grazier/utils/pytorch.py` & `grazier-0.0.5/grazier/utils/pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
                 for i in range(torch.cuda.device_count())
             ]
             device = "cuda:" + str(torch.argmax(torch.tensor(free_memory)).item())
         elif device.startswith("cuda:"):
             # If the user specifies a specific GPU, make sure it exists
             if int(device[5:]) >= torch.cuda.device_count():
                 raise ValueError(f"Invalid device: {device}")
-        elif device == 'api' or device == 'defer':
+        elif device == "api" or device == "defer":
             return None
 
         return device
 
     elif isinstance(device, int):
         return f"cuda:{device}"
```

### Comparing `grazier-0.0.4/grazier.egg-info/PKG-INFO` & `grazier-0.0.5/grazier.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grazier
-Version: 0.0.4
+Version: 0.0.5
 Summary: A tool for calling (and calling out to) large language models.
 Author-email: David Chan <davidchan@berkeley.edu>
 License: 
         Copyright 2023, Regents of the University of California
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -37,44 +37,54 @@
 # Grazier: Easily call Large Language Models from a unified API
 
 Grazier is a Python library for easily calling large language models from a unified API.
 
 ## Supported Large Language Models
 
 From OpenAI:
-- GPT-4 (Base, 32K) (Chat Engine)
-- GPT-3.5 (ChatGPT) (Chat Engine)
+- GPT-4 (Base, 32K) (Chat and Completion Engines)
+- GPT-3.5 (ChatGPT) (Chat and Completion Engines)
 - GPT-3 (Davinci (v2,v3), Ada, Babbage, Curie) (Completion Engine)
 
 From Anthropic:
-- Claude (Base, 100K) (Chat Engine)
-- Claude Instant (Base, 100K) (Chat Engine)
+- Claude (Base, 100K) (Chat and Completion Engines)
+- Claude Instant (Base, 100K) (Chat and Completion Engines)
 
 From Google/GCP:
 - PaLM (Chat and Completion Engines)
 
 From Huggingface
 - GPT-2 (Base, Medium, Large, XL) (Completion Engine)
 - GPT-Neo (125M, 1.3B, 2.7B) (Completion Engine)
 - GPT-J (6B) (Completion Engine)
+- Falcon (7B, 40B, rw-1B, rw-7B) (Completion Engine)
+- Dolly (v1 - 6B, v2 - 3B, 7B, 12B) (Chat and Completion Engines)
+- MPT (Instruct - 7B, 30B) (Chat and Completion Engines)
 
 From Facebook (via Huggingface)
 - Llama (7B, 13B, 30B, 65B) (Completion Engine)
 - OPT (125M, 350M, 1.3B, 2.7B, 6.7B, 13B, 30B, 66B) (Completion Engine)
 
 From Stanford (via Huggingface)
-- Alpaca (7B) (Chat Engine)
+- Alpaca (7B) (Chat and Completion Engines)
 
 From Berkeley (via Huggingface)
-- Koala (7B, 13B_v1, 13B_v2) (Chat Engine)
-- Vicuna (7B, 13B) (Chat Engine)
+- Koala (7B, 13B_v1, 13B_v2) (Chat and Completion Engines)
+- Vicuna (7B, 13B) (Chat and Completion Engines)
 
 From StabilityAI (via Huggingface)
 - StableLM (7B, 13B) (Chat and Completion Engines)
 
+From AllenAI (via Huggingface)
+- Tulu (7B, 13B, 30B, 65B) (Chat and Completion Engines)
+- Open Instruct (ShareGPT) (7B, 13B, 30B, 65B) (Chat and Completion Engines)
+
+From AI21
+- Jurassic 2 (Light, Mid, Ultra) (Completion Engines)
+
 
 ## Installation
 
 Grazier can easily be installed using pip:
 ```bash
 pip install grazier
 ```
@@ -172,30 +182,44 @@
 ```
 
 ### Huggingface Engines
 Most of the huggingface engines require no additional setup, however, some of the larger models require a GPU to run
 with any kind of efficiency (and some require multiple GPUs with large amounts of memory). You can find more details
 about the requirements for each model on the [Huggingface model hub](https://huggingface.co/models).
 
-### Llama, Alpaca, Koala, and Vicuna Engines
+### Llama, Alpaca, Koala, Vicuna and AllenAI Engines
 For these engines, you will need to obtain and postprocess the weights yourself (due to Facebook's licensing). You can
 find the instructions for doing so on each model page:
 - Llama: https://huggingface.co/docs/transformers/main/model_doc/llama
 - Alpaca: https://github.com/tatsu-lab/stanford_alpaca#recovering-alpaca-weights
 - Koala: https://github.com/young-geng/EasyLM/blob/main/docs/koala.md
 - Vicuna: https://github.com/lm-sys/FastChat#vicuna-weights
+- AllenAI: https://huggingface.co/allenai/tulu-65b
 
 Once the weights have been downloaded and processed, you can set the following environment variables to the root
-directory containing a folder for each variant (for example, `root_dir/llama_7B/weights.bin`, the root directory would
-be `root_dir`):
+directory containing a folder for each variant (The format is, `{root_dir}/{model-prefix}/weights.bin`, the root directory would
+be `root_dir`, and the model-prefix is the name of the model, e.g. `tulu-65b`):
 ```bash
 LLAMA_WEIGHTS_ROOT=<path to the llama weights>
 ALPACA_WEIGHTS_ROOT=<path to the alpaca weights>
 KOALA_WEIGHTS_ROOT=<path to the koala weights>
 VICUNA_WEIGHTS_ROOT=<path to the vicuna weights>
+ALLENAI_WEIGHTS_ROOT=<path to the allenai weights>
+```
+
+### AI21 Models (Jurassic)
+For AI21 models, you will need to set the `AI21_API_KEY` environment variable. You can find your API key at
+the [AI21 Studio Dashboard](https://studio.ai21.com/account/api-key). You can set this environment variable in
+your shell or in a `.env` file in the root of your project. For example, in a `.env` file, you would have:
+```bash
+AI21_API_KEY=<your key>
+```
+or on the command line:
+```bash
+export AI21_API_KEY=<your key>
 ```
 
 ## Citation
 
 If you use grazier in your work, please cite:
 
 ```
```

### Comparing `grazier-0.0.4/grazier.egg-info/SOURCES.txt` & `grazier-0.0.5/grazier.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -19,20 +19,27 @@
 grazier/engines/chat/llama_engine_test.py
 grazier/engines/chat/openai_engine.py
 grazier/engines/chat/openai_engine_test.py
 grazier/engines/chat/stable_lm_engine.py
 grazier/engines/chat/stable_lm_engine_test.py
 grazier/engines/chat/vertex_engine.py
 grazier/engines/chat/vertex_engine_test.py
+grazier/engines/chat/dolly/__init__.py
+grazier/engines/chat/dolly/dolly_engine_test.py
+grazier/engines/chat/dolly/instruct_pipeline.py
 grazier/engines/llm/__init__.py
+grazier/engines/llm/ai21_engine.py
+grazier/engines/llm/ai21_engine_test.py
 grazier/engines/llm/chat_engine.py
 grazier/engines/llm/huggingface_engine.py
 grazier/engines/llm/huggingface_engine_test.py
 grazier/engines/llm/llama_engine.py
 grazier/engines/llm/llama_engine_test.py
 grazier/engines/llm/openai_engine.py
 grazier/engines/llm/openai_engine_test.py
 grazier/engines/llm/vertex_engine.py
 grazier/engines/llm/vertex_engine_test.py
 grazier/utils/__init__.py
 grazier/utils/python.py
-grazier/utils/pytorch.py
+grazier/utils/pytorch.py
+grazier/utils/llama/convert_llama_weights_to_hf.py
+grazier/utils/llama/weight_diff.py
```

### Comparing `grazier-0.0.4/pyproject.toml` & `grazier-0.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 [project]
 name = 'grazier'
-version = '0.0.4'
+version = '0.0.5'
 description = 'A tool for calling (and calling out to) large language models.'
 authors = [
     {name='David Chan', email='davidchan@berkeley.edu'}
 ]
 dependencies=[
     # Base dependencies
     "click",
     "rich",
     "python-dotenv",
     "ratelimit",
+    "fire", # For weight_diff.py. TODO: Remove this, replace with click
 
     # LM Engines
     "openai",
     "anthropic",
     "google-cloud-aiplatform[pipelines]",
+    "ai21",
 
     # Local LM Engines
     "torch>=1.13.0",
     "transformers>=4.30.2",
     "sentencepiece",
     "accelerate",
     "einops",
```

