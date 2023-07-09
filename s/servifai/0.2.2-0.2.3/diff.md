# Comparing `tmp/servifai-0.2.2.tar.gz` & `tmp/servifai-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servifai-0.2.2.tar", max compression
+gzip compressed data, was "servifai-0.2.3.tar", max compression
```

## Comparing `servifai-0.2.2.tar` & `servifai-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1067 2023-06-29 08:21:05.500102 servifai-0.2.2/LICENSE
--rw-r--r--   0        0        0     2712 2023-07-09 05:19:26.420188 servifai-0.2.2/README.md
--rw-r--r--   0        0        0      791 2023-07-09 05:17:00.916188 servifai-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       53 2023-07-09 05:16:05.568188 servifai-0.2.2/servifai/__init__.py
--rw-r--r--   0        0        0      243 2023-07-07 16:02:37.899863 servifai-0.2.2/servifai/default_config.yaml
--rw-r--r--   0        0        0       26 2023-07-07 16:02:37.899863 servifai-0.2.2/servifai/llm/__init__.py
--rw-r--r--   0        0        0      389 2023-07-07 16:02:37.899863 servifai-0.2.2/servifai/llm/base.py
--rw-r--r--   0        0        0     1371 2023-07-08 16:06:18.140199 servifai-0.2.2/servifai/llm/openai.py
--rw-r--r--   0        0        0       29 2023-07-07 16:02:37.899863 servifai-0.2.2/servifai/memory/__init__.py
--rw-r--r--   0        0        0     1812 2023-07-08 16:06:17.516199 servifai-0.2.2/servifai/memory/chroma.py
--rw-r--r--   0        0        0       34 2023-07-07 16:02:37.899863 servifai-0.2.2/servifai/planning/__init__.py
--rw-r--r--   0        0        0     1071 2023-07-08 16:06:17.544199 servifai-0.2.2/servifai/planning/react.py
--rw-r--r--   0        0        0     2011 2023-07-08 16:06:17.644199 servifai-0.2.2/servifai/servifai.py
--rw-r--r--   0        0        0       30 2023-07-07 16:02:37.899863 servifai-0.2.2/servifai/toolbox/__init__.py
--rw-r--r--   0        0        0      864 2023-07-08 16:06:17.600199 servifai-0.2.2/servifai/toolbox/base.py
--rw-r--r--   0        0        0     1417 2023-07-08 16:06:17.676199 servifai-0.2.2/servifai/toolbox/default.py
--rw-r--r--   0        0        0     7500 2023-07-09 05:16:05.568188 servifai-0.2.2/servifai/toolbox/knowledge_base.py
--rw-r--r--   0        0        0     3669 1970-01-01 00:00:00.000000 servifai-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-29 08:21:05.500102 servifai-0.2.3/LICENSE
+-rw-r--r--   0        0        0     3929 2023-07-09 06:21:26.524188 servifai-0.2.3/README.md
+-rw-r--r--   0        0        0      791 2023-07-09 06:05:24.892188 servifai-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0       53 2023-07-09 06:06:10.204188 servifai-0.2.3/servifai/__init__.py
+-rw-r--r--   0        0        0      243 2023-07-09 06:05:09.660188 servifai-0.2.3/servifai/default_config.yaml
+-rw-r--r--   0        0        0       26 2023-07-07 16:02:37.899863 servifai-0.2.3/servifai/llm/__init__.py
+-rw-r--r--   0        0        0      389 2023-07-07 16:02:37.899863 servifai-0.2.3/servifai/llm/base.py
+-rw-r--r--   0        0        0     1371 2023-07-08 16:06:18.140199 servifai-0.2.3/servifai/llm/openai.py
+-rw-r--r--   0        0        0       29 2023-07-07 16:02:37.899863 servifai-0.2.3/servifai/memory/__init__.py
+-rw-r--r--   0        0        0     1812 2023-07-08 16:06:17.516199 servifai-0.2.3/servifai/memory/chroma.py
+-rw-r--r--   0        0        0       34 2023-07-07 16:02:37.899863 servifai-0.2.3/servifai/planning/__init__.py
+-rw-r--r--   0        0        0     1071 2023-07-08 16:06:17.544199 servifai-0.2.3/servifai/planning/react.py
+-rw-r--r--   0        0        0     2011 2023-07-08 16:06:17.644199 servifai-0.2.3/servifai/servifai.py
+-rw-r--r--   0        0        0       30 2023-07-07 16:02:37.899863 servifai-0.2.3/servifai/toolbox/__init__.py
+-rw-r--r--   0        0        0      864 2023-07-08 16:06:17.600199 servifai-0.2.3/servifai/toolbox/base.py
+-rw-r--r--   0        0        0     1417 2023-07-08 16:06:17.676199 servifai-0.2.3/servifai/toolbox/default.py
+-rw-r--r--   0        0        0     7500 2023-07-09 05:16:05.568188 servifai-0.2.3/servifai/toolbox/knowledge_base.py
+-rw-r--r--   0        0        0     4886 1970-01-01 00:00:00.000000 servifai-0.2.3/PKG-INFO
```

### Comparing `servifai-0.2.2/LICENSE` & `servifai-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `servifai-0.2.2/pyproject.toml` & `servifai-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "servifai"
-version = "0.2.2"
+version = "0.2.3"
 description = "A mini framework built on top of Langchain and Llamaindex to provide LLM powered Autonomous Agents as a simplified service to assist users with their tasks"
 authors = ["Zoheb Abai <zohebabai@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `servifai-0.2.2/servifai/llm/openai.py` & `servifai-0.2.3/servifai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `servifai-0.2.2/servifai/memory/chroma.py` & `servifai-0.2.3/servifai/memory/chroma.py`

 * *Files identical despite different names*

### Comparing `servifai-0.2.2/servifai/planning/react.py` & `servifai-0.2.3/servifai/planning/react.py`

 * *Files identical despite different names*

### Comparing `servifai-0.2.2/servifai/servifai.py` & `servifai-0.2.3/servifai/servifai.py`

 * *Files identical despite different names*

### Comparing `servifai-0.2.2/servifai/toolbox/base.py` & `servifai-0.2.3/servifai/toolbox/base.py`

 * *Files identical despite different names*

### Comparing `servifai-0.2.2/servifai/toolbox/default.py` & `servifai-0.2.3/servifai/toolbox/default.py`

 * *Files identical despite different names*

### Comparing `servifai-0.2.2/servifai/toolbox/knowledge_base.py` & `servifai-0.2.3/servifai/toolbox/knowledge_base.py`

 * *Files identical despite different names*

### Comparing `servifai-0.2.2/PKG-INFO` & `servifai-0.2.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: servifai
-Version: 0.2.2
-Summary: A mini framework built on top of Langchain and Llamaindex to provide LLM powered Autonomous Agents as a simplified service to assist users with their tasks
-License: MIT
-Author: Zoheb Abai
-Author-email: zohebabai@gmail.com
-Requires-Python: >=3.10,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: chromadb (>=0.3.26,<0.4.0)
-Requires-Dist: docx2txt (>=0.8,<0.9)
-Requires-Dist: duckduckgo-search (>=3.8.3,<4.0.0)
-Requires-Dist: langchain (==0.0.220)
-Requires-Dist: llama-index (==0.6.38)
-Requires-Dist: nltk (>=3.8.1,<4.0.0)
-Requires-Dist: openai (>=0.27.8,<0.28.0)
-Requires-Dist: pypdf (>=3.11.0,<4.0.0)
-Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
-Requires-Dist: pyyaml (>=6.0,<7.0)
-Description-Content-Type: text/markdown
-
 # ServifAI
 
 *A mini framework built on top of Langchain and Llamaindex to provide LLM powered Autonomous Agents as a simplified service to assist users with their tasks.*
 
 ![PyPI](https://img.shields.io/github/license/zohebabai/servifai)
 ![PyPI](https://img.shields.io/pypi/v/servifai)
 
@@ -76,24 +52,52 @@
     if text_input == "exit":
         break
     response = myagent.chat(text_input)
     print(f'ServifAI: {response}\n')
 ```
 Output
 ```
-Me: Hi, How are you?
-ServifAI: Hi, I'm an AI language model, so I don't have feelings, but I'm here to help you with any questions or tasks you have!
+Me: I am feeling bored at home, provide me a list of places in bengaluru to chill out on a sunday.
+ServifAI: Here is a list of places in Bengaluru to chill out on a Sunday:
+
+1. Cubbon Park
+2. Rasta Cafe
+3. Skandagiri
+4. Uttari Betta Sunrise
+5. Ranganathaswamy Betta
+6. Adventure Camping at Nandi Hills
+7. Riverside Manchanabele
+8. Caving at AntaraGange
+9. Clubbing at Hard Rock Café
+10. High Ultra lounge
+11. Toit
+12. Dinning at Empire Hotel
+
+These are just a few options, and there are many more places in Bengaluru where you can relax and have a good time on a Sunday.
+
+Me: Too many options for a day. Provide a itinerary instead for one day
+ServifAI: Based on the search results, here is a suggested one-day itinerary for Bengaluru:
+
+Morning: Start your day with a visit to Cubbon Park and enjoy the greenery. Join the locals on their early morning walk.
 
-Me: What is the current weather of Bengaluru?
-ServifAI: The current weather in Bengaluru is mostly cloudy with a temperature of 81°F (27°C). The wind is coming from the north at 3 mph (5 km/h). Tomorrow's temperature is expected to be nearly the same as today.
+Afternoon: Indulge in a classic South Indian breakfast and then head to Savandurga, a famous place known for its temples and rock climbing.
 
+Evening: Explore the vibrant streets of Bengaluru and visit popular spots like MG Road or Brigade Road for shopping and dining.
+
+Night: End your day by experiencing the nightlife of Bengaluru at one of the city's popular clubs or lounges.
+
+Please note that this is just a suggested itinerary and you can customize it based on your preferences and interests.
+
+Me: Do you think this would be possible to complete based on today's weather?
+ServifAI: Based on the weather forecast, it is possible to complete the activity you mentioned. The maximum temperature in Bengaluru is expected to be around 32 degrees Celsius today.
+
+Me: exit
 ```
 
 **Check [Examples](https://github.com/ZohebAbai/servifai/tree/main/examples) for more.**
 
 # TODO:
 - [x] Add support for popular unstructured data formats
 - [ ] Add support for other VectorDBs
 - [ ] Add other task based tools
 - [ ] Add support for structured data formats
 - [ ] Support for OpenAI funcs
-
```

