# Comparing `tmp/llmflows-0.0.5.tar.gz` & `tmp/llmflows-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmflows-0.0.5.tar", last modified: Thu Jul  6 06:02:36 2023, max compression
+gzip compressed data, was "llmflows-0.0.6.tar", last modified: Sun Jul  9 17:56:16 2023, max compression
```

## Comparing `llmflows-0.0.5.tar` & `llmflows-0.0.6.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:02:36.152041 llmflows-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-06 06:02:25.000000 llmflows-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-07-06 06:02:36.152041 llmflows-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-07-06 06:02:25.000000 llmflows-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:02:36.144041 llmflows-0.0.5/llmflows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:02:36.148041 llmflows-0.0.5/llmflows/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/callbacks/async_base_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/callbacks/async_functional_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/callbacks/base_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/callbacks/functional_callback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:02:36.148041 llmflows-0.0.5/llmflows/flows/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/flows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/flows/async_base_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/flows/async_base_flowstep.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/flows/async_chat_flowstep.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/flows/async_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/flows/async_flowstep.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/flows/base_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/flows/base_flowstep.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/flows/chat_flowstep.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/flows/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/flows/flowstep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/flows/functional_flowstep.py
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/flows/vectorstore_flowstep.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:02:36.152041 llmflows-0.0.5/llmflows/llms/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/llms/llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/llms/llm_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/llms/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/llms/openai_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/llms/openai_embeddings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:02:36.152041 llmflows-0.0.5/llmflows/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/prompts/prompt_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:02:36.152041 llmflows-0.0.5/llmflows/vectorstores/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/vectorstores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/vectorstores/pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/vectorstores/vector_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-06 06:02:25.000000 llmflows-0.0.5/llmflows/vectorstores/vector_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:02:36.148041 llmflows-0.0.5/llmflows.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-07-06 06:02:36.000000 llmflows-0.0.5/llmflows.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-06 06:02:36.000000 llmflows-0.0.5/llmflows.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 06:02:36.000000 llmflows-0.0.5/llmflows.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-06 06:02:36.000000 llmflows-0.0.5/llmflows.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 06:02:36.000000 llmflows-0.0.5/llmflows.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-06 06:02:25.000000 llmflows-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 06:02:36.152041 llmflows-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:56:16.303363 llmflows-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-09 17:56:06.000000 llmflows-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-07-09 17:56:16.303363 llmflows-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-07-09 17:56:06.000000 llmflows-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:56:16.299363 llmflows-0.0.6/llmflows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:56:16.299363 llmflows-0.0.6/llmflows/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/callbacks/async_base_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/callbacks/async_functional_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/callbacks/base_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/callbacks/functional_callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:56:16.299363 llmflows-0.0.6/llmflows/flows/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/flows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/flows/async_base_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/flows/async_base_flowstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/flows/async_chat_flowstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/flows/async_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/flows/async_flowstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/flows/base_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/flows/base_flowstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/flows/chat_flowstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/flows/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/flows/flowstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/flows/functional_flowstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/flows/vectorstore_flowstep.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:56:16.303363 llmflows-0.0.6/llmflows/llms/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/llms/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/llms/llm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/llms/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/llms/openai_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/llms/openai_embeddings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:56:16.303363 llmflows-0.0.6/llmflows/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/prompts/prompt_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:56:16.303363 llmflows-0.0.6/llmflows/vectorstores/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/vectorstores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/vectorstores/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/vectorstores/vector_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-09 17:56:06.000000 llmflows-0.0.6/llmflows/vectorstores/vector_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:56:16.299363 llmflows-0.0.6/llmflows.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-07-09 17:56:16.000000 llmflows-0.0.6/llmflows.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-09 17:56:16.000000 llmflows-0.0.6/llmflows.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 17:56:16.000000 llmflows-0.0.6/llmflows.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-09 17:56:16.000000 llmflows-0.0.6/llmflows.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-09 17:56:16.000000 llmflows-0.0.6/llmflows.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-09 17:56:06.000000 llmflows-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 17:56:16.303363 llmflows-0.0.6/setup.cfg
```

### Comparing `llmflows-0.0.5/LICENSE` & `llmflows-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.5/PKG-INFO` & `llmflows-0.0.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,60 +1,52 @@
-Metadata-Version: 2.1
-Name: llmflows
-Version: 0.0.5
-Summary: LLMFlows - Simple, Explicit and Transparent LLM Apps
-Author: Stoyan Stoyanov
-Project-URL: Homepage, https://github.com/stoyan-stoyanov/llmflows
-Project-URL: github, https://github.com/stoyan-stoyanov/llmflows
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # LLMFlows - Simple, Explicit, and Transparent LLM Apps
 
 <p align="center">
   <img style="width: 80%" src="docs/llmflows_last_logo.png" />
 </p>
 
 [![Twitter](https://img.shields.io/twitter/follow/LLMFlows?style=social)](https://twitter.com/LLMFlows)
 ![Pylint workflow](https://github.com/stoyan-stoyanov/llmflow/actions/workflows/pylint.yml/badge.svg)
 ![License](https://img.shields.io/github/license/stoyan-stoyanov/llmflow)
 ![PyPi](https://img.shields.io/pypi/v/llmflows)
 ![Stars](https://img.shields.io/github/stars/stoyan-stoyanov/llmflow?style=social)
 ![Release date](https://img.shields.io/github/release-date/stoyan-stoyanov/llmflow?style=social)
 
+Documentation: [https://readthedocs.org](https://readthedocs.org/)<br/>
+PyPI: [https://pypi.org/project/llmflows](https://pypi.org/project/llmflows/)</br>
+Twitter: [https://twitter.com/LLMFlows](https://twitter.com/LLMFlows)<br/>
+Substack: [https://llmflows.substack.com](https://llmflows.substack.com/)<br/>
+
 ## About
-LLMFlows is a simple and lightweight framework for building LLM-powered applications.
+LLMFlows is a framework for building simple, explicit, and transparent LLM applications.
 
 ## Installation
-You can quickly install LLMFlows with pip
 ```
 pip install llmflows
 ```
 
-## Documentation
-The full documentation including user guides and api reference can be found at readthedocs.
-
 ## Philosophy
 
 ### Simple
-Our goal is to build a simple, well documented framework with a minimal set of classes and abstractions that allow users to build flexible LLM-powered apps without compromising on capabilities.
+Our goal is to build a simple, well-documented framework with minimal abstractions that 
+allow users to build flexible LLM-powered apps without compromising on capabilities.
 
 ### Explicit
-We want to create an explicit API enabling users to write clean, and readable code while being able to easily create complex flows of LLMs interacting with each other.
+We want to create an explicit API enabling users to write clean and readable code while 
+easily creating complex flows of LLMs interacting with each other.
 
 ### Transparent
-We aim helping users have full transparency on their LLM-powered apps by providing traceable flows, and complete information for each component of the app making it easy to monitor, maintain, and debug.
+We aim to help users have full transparency on their LLM-powered apps by providing 
+traceable flows and complete information for each app component, making it easy to 
+monitor, maintain, and debug.
 
 
 ## Usage
-Here is a minimal example of an LLM with a PromptTemplate:
+You can quickly build a simple application with LLMFlows' `LLM` and `PrompTemplate` 
+classes:
 
 ```python
 
 from llmflows.llms.openai import OpenAI
 from llmflows.prompts.prompt_template import PromptTemplate
 
 prompt_template = PromptTemplate(
@@ -63,34 +55,39 @@
 llm_prompt = prompt_template.get_prompt(topic="friendship")
 
 llm = OpenAI()
 song_title = llm.generate(llm_prompt)
 
 ```
 
-While this is a good example on how easy it is to use LLMFlows, real-world applications are more complex and have dependencies between prompts, and LLMs outputs. Let's take a look at such example. 
+However, real-world applications are often more complex and have dependencies between 
+prompts and LLM calls. For example:
+
 ![Complex flow](docs/complex_flow.png)
-With LLMFlows it's quite easy to reproduce this flow by utilizing the Flow and Flowstep classes. LLMFlows will figure out the dependencies and make sure each flowstep is executed only when the flowsteps it depends on are complete:
+
+You can build such flow using the `Flow` and `Flowstep` classes. LLMFlows will figure 
+out the dependencies and make sure each flowstep runs only when all its dependencies 
+are met:
 
 ```python
-from llmflows.flows import Flow, Flowstep
+from llmflows.flows import Flow, FlowStep
 from llmflows.llms import OpenAI
 from llmflows.prompts import PromptTemplate
 
 # Create prompt templates
 title_template = PromptTemplate("What is a good title of a movie about {topic}?")
 song_template = PromptTemplate(
     "What is a good song title of a soundtrack for a movie called {movie_title}?"
 )
 characters_template = PromptTemplate(
     "What are two main characters for a movie called {movie_title}?"
 )
 lyrics_template = PromptTemplate(
-    "Write lyrics of a movie song called {song_title}. The main characters are"
-    " {main_characters}"
+    "Write lyrics of a movie song called {song_title}. The main characters are "
+    "{main_characters}"
 )
 
 # Create flowsteps
 flowstep1 = FlowStep(
     name="Flowstep 1",
     llm=OpenAI(),
     prompt_template=title_template,
@@ -121,45 +118,55 @@
 # Connect flowsteps
 flowstep1.connect(flowstep2, flowstep3, flowstep4)
 flowstep2.connect(flowstep4)
 flowstep3.connect(flowstep4)
 
 # Create and run Flow
 soundtrack_flow = Flow(flowstep1)
-soundtrack_flow.execute(topic="friendship")
-
+results = soundtrack_flow.start(topic="friendship", verbose=True)
 ```
-In fact, LLMFlows provides async, and threaded classes so any complex DAG can be executed in parallel.
-For more examples such as how to create question answering apps and web applications with Flask and FastAPI check our documentation.
+
+In addition, LLMFlows provides async classes to improve the runtime of any complex flow 
+by running flow steps that already have all their required inputs in parallel.
+Check our documentation for more examples, such as creating question-answering apps and 
+web applications with Flask and FastAPI.
 
 ## FAQ
 
 ### How is this different than langchain?
-Langchain is a great library and LLMFlows has been been certainly inspired by it. However, our philosophy is a bit different. Langchian has a "chain for everything" philosophy and provides many classes that come with multiple LLM calls, logic, and built-in default prompts. While this is great for beginners and default use-cases, we feel this can be a bit overwhelming if users want to do anything "out of the ordinary". In contrast, we are focusing on providing as few building blocks as possible and having an easy to understand API while matching (and in some cases exceeding) the capabilities of langchain.
-
-### You only have OpenAI wrappers but I want to use AcmeLLM?
-We decided to release the library initially supporting only OpenAI LLMs but we have a roadmap and we will slowly add new wrappers around the most popular models. If you are willing to spend some time we are looking for contributors and maintainers
-
-### You only support Pinecone and Redis vector DBs do you have plans to extend the list?
-Yes! We will also add Redis, Elastic Search and other popular solutions over time. If you want to help us out check out our contribution section.
+Langchain is a great library, and LLMFlows has undoubtedly been inspired by it. 
+However, our philosophy is a bit different. Langchian has a "chain for everything" 
+philosophy and provides many classes with multiple LLM calls, logic, and built-in 
+default prompts. While this is great for beginners and default use cases, we feel this 
+can be overwhelming if users want to do anything "out of the ordinary." In contrast, 
+we are focusing on providing as few building blocks as possible and having an 
+easy-to-understand API while matching (and in some cases exceeding) the capabilities 
+of langchain.
+
+### You only have OpenAI wrappers, but I want to use AcmeLLM.
+We decided to release the library initially supporting only OpenAI LLMs, but we have a 
+roadmap and will slowly add new wrappers around the most popular models. If you are 
+willing to spend some time, we are looking for contributors and maintainers.
+
+### You only support Pinecone. Do you have plans to extend the list?
+Yes! Over time, we will also add Chroma, Weaviate, Redis, Elastic Search, and other 
+popular solutions. If you want to help us out, check out our contribution section.
 
 ### Why can't I find any info related to document loaders?
-For the time being we have decided not to implement document loaders for few reasons:
-1. There are plenty of capable libraries like Llama-index and langchain that have tons of loaders.
-2. We think it is awkward to mix document loaders together with LLM and prompt management libraries since usually document loading happens in separate pipelines and are not part of the LLM-powered app.
-3. Real-life documents are messy. In our experience, no matter how many loaders are out there they will never cover all the specific use-cases.
+For the time being, we have decided not to implement document loaders for a few reasons:
 
-While we are not going to invest time into document loaders we might decide to change direction if we get significant interest and contributors.
+1. plenty of capable libraries like Llama-index and langchain have tons of loaders.
+2. We think mixing document loaders with LLM and prompt management libraries is awkward 
+3. since document loading usually happens in separate pipelines and is not part of the 
+4. LLM-powered app.
+5. Real-life documents are messy. In our experience, no matter how many loaders are out 
+6. there, they will never cover all the specific use cases.
 
-### What about agents?
-We believe agents are the future of LLM-powered apps and we have a few basic examples in the repo. However, we are working on a agent-focused library built on top of llmflow.
+While we will not invest time into document loaders, we might change direction if we 
+get significant interest and contributors.
 
 ## License
-LLMFlows is covered by the MIT license. For more information check `LICENCE.md`.
+LLMFlows is covered by the MIT license. For more information, check `LICENCE.md`.
 
 ## Contributing
-Thank you for spending the time to read our README! If you like what you saw and are considering contributing please check CONTRIBUTING.md
-
-## Links
-Twitter
-
-Documentation
+Thank you for spending the time to read our README! If you like what you saw and are 
+considering contributing, please check `CONTRIBUTING.md`
```

### Comparing `llmflows-0.0.5/README.md` & `llmflows-0.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,66 @@
+Metadata-Version: 2.1
+Name: llmflows
+Version: 0.0.6
+Summary: LLMFlows - Simple, Explicit and Transparent LLM Apps
+Author: Stoyan Stoyanov
+Project-URL: Homepage, https://github.com/stoyan-stoyanov/llmflows
+Project-URL: github, https://github.com/stoyan-stoyanov/llmflows
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # LLMFlows - Simple, Explicit, and Transparent LLM Apps
 
 <p align="center">
   <img style="width: 80%" src="docs/llmflows_last_logo.png" />
 </p>
 
 [![Twitter](https://img.shields.io/twitter/follow/LLMFlows?style=social)](https://twitter.com/LLMFlows)
 ![Pylint workflow](https://github.com/stoyan-stoyanov/llmflow/actions/workflows/pylint.yml/badge.svg)
 ![License](https://img.shields.io/github/license/stoyan-stoyanov/llmflow)
 ![PyPi](https://img.shields.io/pypi/v/llmflows)
 ![Stars](https://img.shields.io/github/stars/stoyan-stoyanov/llmflow?style=social)
 ![Release date](https://img.shields.io/github/release-date/stoyan-stoyanov/llmflow?style=social)
 
+Documentation: [https://readthedocs.org](https://readthedocs.org/)<br/>
+PyPI: [https://pypi.org/project/llmflows](https://pypi.org/project/llmflows/)</br>
+Twitter: [https://twitter.com/LLMFlows](https://twitter.com/LLMFlows)<br/>
+Substack: [https://llmflows.substack.com](https://llmflows.substack.com/)<br/>
+
 ## About
-LLMFlows is a simple and lightweight framework for building LLM-powered applications.
+LLMFlows is a framework for building simple, explicit, and transparent LLM applications.
 
 ## Installation
-You can quickly install LLMFlows with pip
 ```
 pip install llmflows
 ```
 
-## Documentation
-The full documentation including user guides and api reference can be found at readthedocs.
-
 ## Philosophy
 
 ### Simple
-Our goal is to build a simple, well documented framework with a minimal set of classes and abstractions that allow users to build flexible LLM-powered apps without compromising on capabilities.
+Our goal is to build a simple, well-documented framework with minimal abstractions that 
+allow users to build flexible LLM-powered apps without compromising on capabilities.
 
 ### Explicit
-We want to create an explicit API enabling users to write clean, and readable code while being able to easily create complex flows of LLMs interacting with each other.
+We want to create an explicit API enabling users to write clean and readable code while 
+easily creating complex flows of LLMs interacting with each other.
 
 ### Transparent
-We aim helping users have full transparency on their LLM-powered apps by providing traceable flows, and complete information for each component of the app making it easy to monitor, maintain, and debug.
+We aim to help users have full transparency on their LLM-powered apps by providing 
+traceable flows and complete information for each app component, making it easy to 
+monitor, maintain, and debug.
 
 
 ## Usage
-Here is a minimal example of an LLM with a PromptTemplate:
+You can quickly build a simple application with LLMFlows' `LLM` and `PrompTemplate` 
+classes:
 
 ```python
 
 from llmflows.llms.openai import OpenAI
 from llmflows.prompts.prompt_template import PromptTemplate
 
 prompt_template = PromptTemplate(
@@ -49,34 +69,39 @@
 llm_prompt = prompt_template.get_prompt(topic="friendship")
 
 llm = OpenAI()
 song_title = llm.generate(llm_prompt)
 
 ```
 
-While this is a good example on how easy it is to use LLMFlows, real-world applications are more complex and have dependencies between prompts, and LLMs outputs. Let's take a look at such example. 
+However, real-world applications are often more complex and have dependencies between 
+prompts and LLM calls. For example:
+
 ![Complex flow](docs/complex_flow.png)
-With LLMFlows it's quite easy to reproduce this flow by utilizing the Flow and Flowstep classes. LLMFlows will figure out the dependencies and make sure each flowstep is executed only when the flowsteps it depends on are complete:
+
+You can build such flow using the `Flow` and `Flowstep` classes. LLMFlows will figure 
+out the dependencies and make sure each flowstep runs only when all its dependencies 
+are met:
 
 ```python
-from llmflows.flows import Flow, Flowstep
+from llmflows.flows import Flow, FlowStep
 from llmflows.llms import OpenAI
 from llmflows.prompts import PromptTemplate
 
 # Create prompt templates
 title_template = PromptTemplate("What is a good title of a movie about {topic}?")
 song_template = PromptTemplate(
     "What is a good song title of a soundtrack for a movie called {movie_title}?"
 )
 characters_template = PromptTemplate(
     "What are two main characters for a movie called {movie_title}?"
 )
 lyrics_template = PromptTemplate(
-    "Write lyrics of a movie song called {song_title}. The main characters are"
-    " {main_characters}"
+    "Write lyrics of a movie song called {song_title}. The main characters are "
+    "{main_characters}"
 )
 
 # Create flowsteps
 flowstep1 = FlowStep(
     name="Flowstep 1",
     llm=OpenAI(),
     prompt_template=title_template,
@@ -107,45 +132,55 @@
 # Connect flowsteps
 flowstep1.connect(flowstep2, flowstep3, flowstep4)
 flowstep2.connect(flowstep4)
 flowstep3.connect(flowstep4)
 
 # Create and run Flow
 soundtrack_flow = Flow(flowstep1)
-soundtrack_flow.execute(topic="friendship")
-
+results = soundtrack_flow.start(topic="friendship", verbose=True)
 ```
-In fact, LLMFlows provides async, and threaded classes so any complex DAG can be executed in parallel.
-For more examples such as how to create question answering apps and web applications with Flask and FastAPI check our documentation.
+
+In addition, LLMFlows provides async classes to improve the runtime of any complex flow 
+by running flow steps that already have all their required inputs in parallel.
+Check our documentation for more examples, such as creating question-answering apps and 
+web applications with Flask and FastAPI.
 
 ## FAQ
 
 ### How is this different than langchain?
-Langchain is a great library and LLMFlows has been been certainly inspired by it. However, our philosophy is a bit different. Langchian has a "chain for everything" philosophy and provides many classes that come with multiple LLM calls, logic, and built-in default prompts. While this is great for beginners and default use-cases, we feel this can be a bit overwhelming if users want to do anything "out of the ordinary". In contrast, we are focusing on providing as few building blocks as possible and having an easy to understand API while matching (and in some cases exceeding) the capabilities of langchain.
-
-### You only have OpenAI wrappers but I want to use AcmeLLM?
-We decided to release the library initially supporting only OpenAI LLMs but we have a roadmap and we will slowly add new wrappers around the most popular models. If you are willing to spend some time we are looking for contributors and maintainers
-
-### You only support Pinecone and Redis vector DBs do you have plans to extend the list?
-Yes! We will also add Redis, Elastic Search and other popular solutions over time. If you want to help us out check out our contribution section.
+Langchain is a great library, and LLMFlows has undoubtedly been inspired by it. 
+However, our philosophy is a bit different. Langchian has a "chain for everything" 
+philosophy and provides many classes with multiple LLM calls, logic, and built-in 
+default prompts. While this is great for beginners and default use cases, we feel this 
+can be overwhelming if users want to do anything "out of the ordinary." In contrast, 
+we are focusing on providing as few building blocks as possible and having an 
+easy-to-understand API while matching (and in some cases exceeding) the capabilities 
+of langchain.
+
+### You only have OpenAI wrappers, but I want to use AcmeLLM.
+We decided to release the library initially supporting only OpenAI LLMs, but we have a 
+roadmap and will slowly add new wrappers around the most popular models. If you are 
+willing to spend some time, we are looking for contributors and maintainers.
+
+### You only support Pinecone. Do you have plans to extend the list?
+Yes! Over time, we will also add Chroma, Weaviate, Redis, Elastic Search, and other 
+popular solutions. If you want to help us out, check out our contribution section.
 
 ### Why can't I find any info related to document loaders?
-For the time being we have decided not to implement document loaders for few reasons:
-1. There are plenty of capable libraries like Llama-index and langchain that have tons of loaders.
-2. We think it is awkward to mix document loaders together with LLM and prompt management libraries since usually document loading happens in separate pipelines and are not part of the LLM-powered app.
-3. Real-life documents are messy. In our experience, no matter how many loaders are out there they will never cover all the specific use-cases.
+For the time being, we have decided not to implement document loaders for a few reasons:
 
-While we are not going to invest time into document loaders we might decide to change direction if we get significant interest and contributors.
+1. plenty of capable libraries like Llama-index and langchain have tons of loaders.
+2. We think mixing document loaders with LLM and prompt management libraries is awkward 
+3. since document loading usually happens in separate pipelines and is not part of the 
+4. LLM-powered app.
+5. Real-life documents are messy. In our experience, no matter how many loaders are out 
+6. there, they will never cover all the specific use cases.
 
-### What about agents?
-We believe agents are the future of LLM-powered apps and we have a few basic examples in the repo. However, we are working on a agent-focused library built on top of llmflow.
+While we will not invest time into document loaders, we might change direction if we 
+get significant interest and contributors.
 
 ## License
-LLMFlows is covered by the MIT license. For more information check `LICENCE.md`.
+LLMFlows is covered by the MIT license. For more information, check `LICENCE.md`.
 
 ## Contributing
-Thank you for spending the time to read our README! If you like what you saw and are considering contributing please check CONTRIBUTING.md
-
-## Links
-Twitter
-
-Documentation
+Thank you for spending the time to read our README! If you like what you saw and are 
+considering contributing, please check `CONTRIBUTING.md`
```

### Comparing `llmflows-0.0.5/llmflows/callbacks/async_base_callback.py` & `llmflows-0.0.6/llmflows/callbacks/async_base_callback.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.5/llmflows/callbacks/async_functional_callback.py` & `llmflows-0.0.6/llmflows/callbacks/async_functional_callback.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.5/llmflows/callbacks/base_callback.py` & `llmflows-0.0.6/llmflows/callbacks/base_callback.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.5/llmflows/callbacks/functional_callback.py` & `llmflows-0.0.6/llmflows/callbacks/functional_callback.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.5/llmflows/flows/async_base_flow.py` & `llmflows-0.0.6/llmflows/flows/async_base_flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,17 +104,17 @@
 
         Raises:
             ValueError: If not all required input keys are covered.
         """
         if not self.input_keys.issubset(self.output_keys.union(user_inputs.keys())):
             raise ValueError("Some flowsteps have missing inputs")
 
-    async def execute(self, **inputs: str):
+    async def start(self, **inputs: str):
         """
-        Placeholder for flow execution method. To be overridden in subclasses.
+        Placeholder starting the flow. To be overridden in subclasses.
 
         Args:
             **inputs (str): Inputs to the flow.
 
         Raises:
             NotImplementedError: If not implemented in subclass.
         """
```

### Comparing `llmflows-0.0.5/llmflows/flows/async_base_flowstep.py` & `llmflows-0.0.6/llmflows/flows/async_base_flowstep.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pylint: disable=R0801, R0913
 
 """
 This module contains the AsyncBaseFlowStep used as a base class by all async
-FlowStep classes. Each async flowstep can execute a task, record
-execution times, and optionally invoke callbacks on the results.
+FlowStep classes. Each async flowstep can run a task, record
+run times, and optionally invoke callbacks on the results.
 
-The async implementation allows async flowsteps to be executed in parallel if
+The async implementation allows async flowsteps to be run in parallel if
 multiple flowsteps have all the required inputs available.
 """
 
 import time
 import datetime
 from abc import ABC, abstractmethod
 from typing import Any, Union
@@ -86,33 +86,33 @@
             inputs (dict[str, Any]): The inputs to the flow step.
 
         Returns:
             tuple: result, call data and model configuration.
         """
         pass
 
-    async def execute(
+    async def run(
         self, inputs: dict[str, str], verbose: bool = False
     ) -> dict[str, str]:
         """
-        Executes the flow step with the provided inputs and returns a dictionary with
-        execution details.
+        Runs the flow step with the provided inputs and returns a dictionary with
+        runtime details.
 
         This includes the start and end times, the prompts and the input to the
         language model, the output from the language model, details about the model
-        configuration and the result of the step. Callback functions can be executed
+        configuration and the result of the step. Callback functions can be run
         with the result as well.
 
         Args:
             inputs (dict[str, str]): The inputs to the flow step.
             verbose (bool, optional): If true, the output of the step
-                and callback executions are printed.
+                and callbacks are printed.
 
         Returns:
-            dict[str, str]: A dictionary with various execution details and results.
+            dict[str, str]: A dictionary with various runtime details and results.
         """
         execution_info = {}
         start_time = datetime.datetime.now().isoformat()
         start_perf_time = time.perf_counter()
         execution_info["start_time"] = start_time
         execution_info["prompt_inputs"] = inputs
```

### Comparing `llmflows-0.0.5/llmflows/flows/async_chat_flowstep.py` & `llmflows-0.0.6/llmflows/flows/async_chat_flowstep.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 # pylint: disable=R0801, R0913
 
 """
 This file contains the AsyncChatFlowStep class, which represents a step in an AsyncFlow
 that is using a chat LLM. The async implementation allows async flowsteps to be 
-executed in parallel if multiple flowsteps have all the required inputs available.
+run in parallel if multiple flowsteps have all the required inputs available.
 """
 
 import logging
 from typing import Any, Union
 from llmflows.llms.llm import BaseLLM
 from llmflows.prompts.prompt_template import PromptTemplate
 from llmflows.callbacks.async_base_callback import AsyncBaseCallback
 from llmflows.flows.async_base_flowstep import AsyncBaseFlowStep
 
 
 class AsyncChatFlowStep(AsyncBaseFlowStep):
     """
     Represents an async step in a Flow that is utilizing a chat LLM.
 
-    An AsyncChatFlowStep executes a language model using two prompt templates, namely
-    a system prompt and a message prompt, records the execution time, and optionally
+    An AsyncChatFlowStep calls a language model using two prompt templates, namely
+    a system prompt and a message prompt, records the run time, and optionally
     invokes callback functions on the results.
 
     Args:
         name (str): The name of the flow step.
         llm (BaseLLM): The language model to be used in the flow step.
         output_key (str): The key for the output of the flow step.
         system_prompt_template (PromptTemplate): Prompt tempalte for the system prompt
             to be used with the language model.
         message_key (str): Key used to extract message from inputs.
         message_prompt_template (PromptTemplate): Prompt template for the message used
             with the language model.
         callbacks (Union[list[AsyncBaseCallback], None]): Callbacks to be invoked
-            during the flowstep execution.
+            during the flowstep run.
 
     Attributes:
         llm (BaseLLM): The language model to be used in the flow step.
         message_key (str): Key used to extract message from inputs.
         system_prompt_template (PromptTemplate): Prompt tempalte for the system prompt
             to be used with the language model.
         message_prompt_template (PromptTemplate): Prompt template for the message used
             with the language model.
-        required_keys (set[str]): The keys required for the flow step to execute.
+        required_keys (set[str]): The keys required for the flow step to run.
     """
 
     def __init__(
         self,
         name: str,
         llm: BaseLLM,
         output_key: str,
```

### Comparing `llmflows-0.0.5/llmflows/flows/async_flow.py` & `llmflows-0.0.6/llmflows/flows/async_flow.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,80 +1,80 @@
 # pylint: disable=R0801
 
 """
-LLMFlow module for the AsyncFlow class used for defining and executing flows, which are 
-digraphs of steps. The async implementation of this class allows for the parallel
-execution of async flowsteps that have all their required inputs available.
+LLMFlow module for the AsyncFlow class used for defining and running flows, which are
+digraphs of steps. The async implementation of this class allows running
+async flowsteps that have all their required inputs available in parallel.
 """
 
 import asyncio
 from llmflows.flows.async_flowstep import AsyncFlowStep
 from llmflows.flows.async_base_flow import AsyncBaseFlow
 
 
 class AsyncFlow(AsyncBaseFlow):
     """
-    Async implementation of BaseFlow that executes a series of FlowSteps in a Directed
+    Async implementation of BaseFlow that runs a series of FlowSteps in a Directed
     Acyclic Graph (DAG) structure.
 
     Args:
         first_step (AsyncFlowStep): The first step of the flow.
 
     Attributes:
         _first_step (AsyncFlowStep): The first step in the flow.
-        results (dict): Stores the results of the executed flow steps.
-        executed_steps (set): Keeps track of the steps that have been executed.
+        results (dict): Stores the results of the completed flow steps.
+        completed_steps (set): Keeps track of the steps that have been completed.
     """
 
     def __init__(self, first_step: AsyncFlowStep):
         super().__init__(first_step)
         self.results = {}
-        self.executed_steps = set()
+        self.completed_steps = set()
 
-    async def execute(self, verbose=False, **inputs) -> dict:
+    async def start(self, verbose=False, **inputs) -> dict:
         """
         Executes the flow with the provided inputs.
 
         Args:
             verbose (bool): Specifies if the flow step should print their output.
             **inputs (dict): The inputs to the flow.
 
         Returns:
             A dictionary of the results from each flow step.
 
         Raises:
             ValueError: If any required inputs are missing.
         """
         self._check_all_input_keys_available(inputs)
-        await self._execute_step(self._first_step, inputs, verbose)
+        await self._run_step(self._first_step, inputs, verbose)
         return self.results
 
-    async def _execute_step(self, step, inputs, verbose):
+    async def _run_step(self, step, inputs, verbose):
         """
         Executes the given step and its next steps in a DFS-like manner.
 
         Args:
-            step (AsyncFlowStep): The step to execute.
+            step (AsyncFlowStep): The step to run.
             inputs (dict): The inputs to the step.
             verbose (bool): Specifies if the flow step should print its output.
 
         Returns:
             Any: The output of the step.
         """
         if not step or any(parent.output_key not in inputs for parent in step.parents):
             return
 
         required_inputs = {key: inputs[key] for key in step.required_keys}
 
-        if step not in self.executed_steps:
-            flow_data = await step.execute(required_inputs, verbose)
-            self.executed_steps.add(step)
+        if step not in self.completed_steps:
+            flow_data = await step.run(required_inputs, verbose)
+            self.completed_steps.add(step)
 
             if flow_data:
                 self.results[step.name] = flow_data
                 inputs.update(flow_data["result"])
 
         tasks = [
-            self._execute_step(next_step, inputs, verbose)
+            self._run_step(next_step, inputs, verbose)
             for next_step in step.next_steps
         ]
         await asyncio.gather(*tasks)
```

### Comparing `llmflows-0.0.5/llmflows/flows/async_flowstep.py` & `llmflows-0.0.6/llmflows/flows/async_flowstep.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,32 +14,32 @@
 from llmflows.flows.async_base_flowstep import AsyncBaseFlowStep
 
 
 class AsyncFlowStep(AsyncBaseFlowStep):
     """
     Represents a specific async step in an async Flow.
 
-    An AsyncFlowStep executes a language model using a prompt template, records the 
-    execution time, and optionally invokes callback functions on the results.
-    Async Flowsteps can be executed in parallel in an AsyncFlow if all the required 
+    An AsyncFlowStep calls a language model using a prompt template, records the
+    run time, and optionally invokes callback functions on the results.
+    Async Flowsteps can be run in parallel in an AsyncFlow if all the required
     inputs are available.
 
     Args:
         name (str): The name of the flow step.
         llm (BaseLLM): The language model to be used in the flow step.
         prompt_template (PromptTemplate): Template for the prompt to be used with the 
             language model.
-        callbacks Union[list[AsyncBaseCallback], None]: Callbacks to be invoked during 
-            the flowstep execution.
+        callbacks Union[list[AsyncBaseCallback], None]: Callbacks to be invoked
+            when running the flow
 
     Attributes:
         llm (BaseLLM): The language model to be used in the flow step.
         prompt_template (PromptTemplate): Template for the prompt to be used with the 
             language model.
-        required_keys (set[str]): The keys required for the flow step to execute.
+        required_keys (set[str]): The keys required for the flow step to run.
     """
 
     def __init__(
         self,
         name: str,
         llm: BaseLLM,
         prompt_template: PromptTemplate,
```

### Comparing `llmflows-0.0.5/llmflows/flows/base_flow.py` & `llmflows-0.0.6/llmflows/flows/base_flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,16 @@
                 self.input_keys.update(step.prompt_template.variables)
             elif flowstep_class == "ChatFlowStep":
                 self.input_keys.update(
                     step.system_prompt_template.variables,
                     step.message_prompt_template.variables,
                     {step.message_key},
                 )
+            elif flowstep_class == "FunctionalFlowStep":
+                self.input_keys.update(step.required_keys)
 
     def _check_all_input_keys_available(self, user_inputs):
         """
         Checks that all required input keys are available.
 
         Args:
             user_inputs (dict): The set of input keys provided by the user.
@@ -104,19 +106,22 @@
         Raises:
             ValueError: If not all required input keys are covered.
         """
 
         print(self.output_keys.union(user_inputs.keys()))
         print(self.input_keys)
         if not self.input_keys.issubset(self.output_keys.union(user_inputs.keys())):
-            raise ValueError("Some flowsteps have missing inputs")
+            missing_inputs = self.input_keys.difference(
+                self.output_keys.union(user_inputs.keys())
+            )
+            raise ValueError(f"Some flowsteps have missing inputs: {missing_inputs}")
 
-    def execute(self, **inputs):
+    def start(self, **inputs):
         """
-        Placeholder method for executing the flow.
+        Placeholder method for starting the flow.
 
         Args:
             inputs (dict): Inputs to the flow.
 
         Raises:
             NotImplementedError: If not implemented in a subclass of BaseFlow.
         """
```

### Comparing `llmflows-0.0.5/llmflows/flows/base_flowstep.py` & `llmflows-0.0.6/llmflows/flows/base_flowstep.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,15 @@
             inputs (dict[str, Any]): The inputs to the flow step.
 
         Returns:
             tuple: result, call data and model configuration.
         """
         pass
 
-    def execute(self, inputs: dict[str, str], verbose: bool = False) -> dict[str, str]:
+    def run(self, inputs: dict[str, str], verbose: bool = False) -> dict[str, str]:
         """
         Executes the flow step with the provided inputs and returns a dictionary with
         execution details.
 
         This includes the start and end times, the prompts and the input to the
         language model, the output from the language model, details about the model
         configuration and the result of the step. Callback functions can be executed
@@ -117,15 +117,15 @@
 
         Args:
             inputs (dict[str, str]): The inputs to the flow step.
             verbose (bool, optional): If true, the output of the step
                 and callback executions are printed.
 
         Returns:
-            dict[str, str]: A dictionary with various execution details and results.
+            dict[str, str]: A dictionary with various runtime details and results.
         """
         execution_info = {}
         start_time = datetime.datetime.now().isoformat()
         start_perf_time = time.perf_counter()
         execution_info["start_time"] = start_time
         execution_info["prompt_inputs"] = inputs
```

### Comparing `llmflows-0.0.5/llmflows/flows/chat_flowstep.py` & `llmflows-0.0.6/llmflows/flows/chat_flowstep.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,38 +11,38 @@
 from llmflows.flows.flowstep import BaseFlowStep
 
 
 class ChatFlowStep(BaseFlowStep):
     """
     Represents a step in a Flow that is utilizing a chat Language Learning Model (LLM).
 
-    A ChatFlowStep executes a language model using two prompt templates, namely a 
-    system prompt and a message prompt, records the execution time, and optionally 
-    invokes callback functions on the results.
+    A ChatFlowStep calls a language model using a system prompt and a message prompt,
+    records the run time, and optionally invokes callback functions on the
+    results.
 
     Args:
         name (str): The name of the flow step.
         llm (BaseLLM): The language model to be used in the flow step.
         output_key (str): The key for the output of the flow step.
         system_prompt_template (PromptTemplate): Prompt tempalte for the system prompt
             to be used with the language model.
         message_key (str): Key used to extract message from inputs.
         message_prompt_template (PromptTemplate): Prompt template for the message used
             with the language model.
         callbacks (Union[list[AsyncBaseCallback], None]): Callbacks to be invoked
-            during the flowstep execution.
+            within the flowstep
 
     Attributes:
         llm (BaseLLM): The language model to be used in the flow step.
         message_key (str): Key used to extract message from inputs.
         system_prompt_template (PromptTemplate): Prompt tempalte for the system prompt
             to be used with the language model.
         message_prompt_template (PromptTemplate): Prompt template for the message used
             with the language model.
-        required_keys (set[str]): The keys required for the flow step to execute.
+        required_keys (set[str]): The keys required for the flow step to run.
     """
 
     def __init__(
         self,
         name: str,
         llm: BaseLLM,
         output_key: str,
```

### Comparing `llmflows-0.0.5/llmflows/flows/flow.py` & `llmflows-0.0.6/llmflows/flows/flow.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,78 +1,78 @@
 # pylint: disable=R0801
 
 """
 LLMFlow module for the Flow class used for defining and executing flows, which are 
 digraphs of steps. Each step is represented by a `FlowStep` instance.
 """
 
-from llmflows.flows.flowstep import FlowStep
+from llmflows.flows.flowstep import BaseFlowStep
 from llmflows.flows.base_flow import BaseFlow
 
 
 class Flow(BaseFlow):
     """
     Base class for all flows. Each flow is a digraph of steps, represented by FlowStep
     instances.
 
     Args:
-        first_step (FlowStep): The first step of the flow.
+        first_step (BaseFlowStep): The first step of the flow.
 
     Attributes:
-        _first_step (FlowStep): The first step in the flow.
+        _first_step (BaseFlowStep): The first step in the flow.
         results (dict): Stores the results of the executed flow steps.
-        executed_steps (set): Keeps track of the steps that have been executed.
+        completed_steps (set): Keeps track of the steps that have been executed.
     """
 
-    def __init__(self, first_step: FlowStep):
+    def __init__(self, first_step: BaseFlowStep):
         super().__init__(first_step)
         self.results = {}
-        self.executed_steps = set()
+        self.completed_steps = set()
 
-    def execute(self, verbose=False, **inputs) -> dict:
+    def start(self, verbose=False, **inputs) -> dict:
         """
         Executes the flow with the provided inputs.
 
         Args:
             verbose (bool): Specifies if the flow step should print their output.
             **inputs (dict): The inputs to the flow.
 
         Returns:
             A dictionary of the results from each flow step.
 
         Raises:
             ValueError: If any required inputs are missing.
         """
         self._check_all_input_keys_available(inputs)
-        self._execute_step(self._first_step, inputs, verbose)
+        self._run_step(self._first_step, inputs, verbose)
         return self.results
 
-    def _execute_step(self, step, inputs, verbose):
+    def _run_step(self, step, inputs, verbose):
         """
         Executes the given step and its next steps in a DFS-like manner.
 
         Args:
-            step (FlowStep): The step to execute.
+            step (FlowStep): The step to run.
             inputs (dict): The inputs to the step.
             verbose (bool): Specifies if the flow step should print its output.
 
         Returns:
             Any: The output of the step.
         """
 
         if not step or any(parent.output_key not in inputs for parent in step.parents):
             return
 
         required_inputs = {
             key: inputs[key] for key in step.required_keys
         }
 
-        if step not in self.executed_steps:
-            flow_data = step.execute(required_inputs, verbose)
-            self.executed_steps.add(step)
+        if step not in self.completed_steps:
+            flow_data = step.run(required_inputs, verbose)
+            self.completed_steps.add(step)
 
             if flow_data:
                 self.results[step.name] = flow_data
                 inputs.update(flow_data["result"])
 
         for next_step in step.next_steps:
-            self._execute_step(next_step, inputs, verbose)
+            self._run_step(next_step, inputs, verbose)
```

### Comparing `llmflows-0.0.5/llmflows/flows/flowstep.py` & `llmflows-0.0.6/llmflows/flows/flowstep.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 # pylint: disable=R0801, R0913
 
 """
-This module the FlowStep class, which can execute a language model, record
-execution times, and optionally invoke callbacks on the results.
+This module the FlowStep class, which can call a language model, record
+run times, and optionally invoke callbacks on the results.
 """
 
 from typing import Any, Union
 from llmflows.llms.llm import BaseLLM
 from llmflows.prompts.prompt_template import PromptTemplate
 from llmflows.callbacks.base_callback import BaseCallback
 from llmflows.flows.base_flowstep import BaseFlowStep
 
 
 class FlowStep(BaseFlowStep):
     """
     Represents a specific step in a Flow.
 
-    A FlowStep executes a language model using a prompt template, records the execution
+    A FlowStep calls a language model using a prompt template, records the run
     time, and optionally invokes callback functions on the results.
 
     Args:
         name (str): The name of the flow step.
         llm (BaseLLM): The language model to be used in the flow step.
         prompt_template (PromptTemplate): Template for the prompt to be used with the 
             language model.
-        callbacks (list[BaseCallback]): Callbacks to be invoked during the flowstep 
-            execution.
+        callbacks (list[BaseCallback]): Callbacks to be invoked within the flowstep
 
     Attributes:
         llm (BaseLLM): The language model to be used in the flow step.
         prompt_template (PromptTemplate): Template for the prompt to be used with the 
             language model.
-        required_keys (set[str]): The keys required for the flow step to execute.
+        required_keys (set[str]): The keys required for the flow step to run.
     """
 
     def __init__(
         self,
         name: str,
         llm: BaseLLM,
         prompt_template: PromptTemplate,
```

### Comparing `llmflows-0.0.5/llmflows/flows/functional_flowstep.py` & `llmflows-0.0.6/llmflows/flows/functional_flowstep.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,62 @@
 """
-LLMFlow module for the `FunctionalFlowstep` class that can be used to execute a given
+LLMFlow module for the `FunctionalFlowstep` class that can be used to run a given
 function within a flow.
 """
 
+import inspect
 from llmflows.flows.flowstep import BaseFlowStep
 from llmflows.callbacks.base_callback import BaseCallback
 from typing import Callable, Any, Union
 
 
 class FunctionalFlowStep(BaseFlowStep):
     """
-    Represents a functional flow step that executes a function. The function must take
-        a dictionary of strings as input and return a string(like regular flow steps) 
+    Represents a functional flow step that runs a function. The function must take
+        a dictionary of strings as input and return a string(like regular flow steps)
 
     Args:
         name (str): The name of the flow step.
-        fn (Callable): The function to execute.
+        fn (Callable): The function to run.
         required_keys (list[str]): A list of required keys.
         output_key (str): The key to use for the output.
-        callbacks (list[Callback], optional): List of callback instances. Defaults to 
+        callbacks (list[Callback], optional): List of callback instances. Defaults to
             None.
-    
+
     Attributes:
-        required_keys (set[str]): The keys required for the flow step to execute.
-        fn (Callable[[dict[str, str]], str]): The function to be executed.
+        required_keys (set[str]): The keys required for the flow step to run.
+        fn (Callable[[dict[str, str]], str]): The function to be run.
     """
+
     def __init__(
         self,
         name: str,
-        fn: Callable[[dict[str, str]], str],
-        required_keys: list[str],
+        flowstep_fn: Callable[..., str],
         output_key: str,
         callbacks: Union[list[BaseCallback], None] = None,
     ):
         super().__init__(name, output_key, callbacks)
-        self.required_keys = set(required_keys)
-        self.fn = fn
+        self.flowstep_fn = flowstep_fn
+        self.required_keys = inspect.getfullargspec(self.flowstep_fn).args
 
     def generate(
         self, inputs: dict[str, Any]
     ) -> tuple[Any, Union[dict, None], Union[dict, None]]:
         """
         Executes the function with the provided inputs.
 
         Args:
             inputs (dict[str, Any]): Input parameters as a dictionary.
 
         Returns:
-            The result of the function call, followed by two None values (for call 
+            The result of the function call, followed by two None values (for call
                 data and config, which are not applicable in this case).
         """
-        return self.fn(inputs), None, None
+        # Get the argument names of fn
+        fn_args = inspect.getfullargspec(self.flowstep_fn).args
+
+        # Create a new dictionary from inputs containing only the keys that fn requires
+        filtered_inputs = {
+            key: value for key, value in inputs.items() if key in fn_args
+        }
+
+        return self.flowstep_fn(**filtered_inputs), None, None
```

### Comparing `llmflows-0.0.5/llmflows/flows/vectorstore_flowstep.py` & `llmflows-0.0.6/llmflows/flows/vectorstore_flowstep.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         prompt_template (PromptTemplate): Optional prompt template to be used with the 
             required keys to create a search prompt.
         output_key (str): The dict key to use for the output.
         top_k (int, optional): The number of top results to return. Defaults to 1.
         append_top_k (bool, optional): Whether to append top_k results. Defaults to
             False.
         callbacks (Union[list[BaseCallback], None]): Callbacks to be invoked during 
-            the flowstep execution.
+            while the flow is running.
 
     Attributes:
         embeddings_model (BaseLLM): The embeddings model instance to use.
         prompt_template (PromptTemplate): Optional prompt template to be used with the 
             required keys to create a search prompt.
         required_keys (list[str]): A list of required keys.
         vector_store (VectorStore): The vector store instance to use.
```

### Comparing `llmflows-0.0.5/llmflows/llms/llm.py` & `llmflows-0.0.6/llmflows/llms/llm.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.5/llmflows/llms/llm_utils.py` & `llmflows-0.0.6/llmflows/llms/llm_utils.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.5/llmflows/llms/openai.py` & `llmflows-0.0.6/llmflows/llms/openai.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.5/llmflows/llms/openai_chat.py` & `llmflows-0.0.6/llmflows/llms/openai_chat.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.5/llmflows/llms/openai_embeddings.py` & `llmflows-0.0.6/llmflows/llms/openai_embeddings.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.5/llmflows/prompts/prompt_template.py` & `llmflows-0.0.6/llmflows/prompts/prompt_template.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.5/llmflows/vectorstores/pinecone.py` & `llmflows-0.0.6/llmflows/vectorstores/pinecone.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,17 +24,15 @@
     
     Attributes:
         index_name (str): The name of the index to use.
         environment (str): The pinecone environment to use.
     """
 
     def __init__(self, index_name: str, api_key: str, environment: str):
-        self.index_name = index_name
-        self._api_key = api_key
-        self.environment = environment
+        super().__init__(index_name, api_key, environment)
         self._init_client()
 
     def _prepare_results(self, search_result) -> tuple[list, dict, dict]:
         """
         Format the search results for the Pinecone vector store client.
 
         Args:
@@ -47,23 +45,23 @@
         search_results = search_result["matches"]
 
         call_data = {
             "raw_outputs": search_result,
         }
 
         config = {
-            "environment": self.environment,
-            "index_name": self.index_name
+            "environment": self.region,
+            "index_name": self.storage_entity
         }
 
         return search_results, call_data, config
 
     def _init_client(self):
-        pinecone.init(api_key=self._api_key, environment=self.environment)
-        self.index = pinecone.Index(self.index_name)
+        pinecone.init(api_key=self._api_key, environment=self.region)
+        self.index = pinecone.Index(self.storage_entity)
         self.describe()
 
     def describe(self):
         """Describe the index."""
         print(self.index.describe_index_stats())
 
     def search(self, query: VectorDoc, top_k: int) -> tuple[list, dict, dict]:
```

### Comparing `llmflows-0.0.5/llmflows/vectorstores/vector_doc.py` & `llmflows-0.0.6/llmflows/vectorstores/vector_doc.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.5/llmflows/vectorstores/vector_store.py` & `llmflows-0.0.6/llmflows/vectorstores/vector_store.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,17 +17,18 @@
 class VectorStore(ABC):
     """
     Abstract base class for vector store services.
 
     This class defines the interface that all vector store services must provide.
     """
 
-    @abstractmethod
-    def __init__(self, index_name: str, api_key: str, environment: str):
-        pass
+    def __init__(self, storage_entity: str, api_key: str, region: str):
+        self.storage_entity = storage_entity
+        self._api_key = api_key
+        self.region = region
 
     @abstractmethod
     def describe(self) -> None:
         """Describe the index."""
         pass
 
     @abstractmethod
```

### Comparing `llmflows-0.0.5/llmflows.egg-info/PKG-INFO` & `llmflows-0.0.6/llmflows.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmflows
-Version: 0.0.5
+Version: 0.0.6
 Summary: LLMFlows - Simple, Explicit and Transparent LLM Apps
 Author: Stoyan Stoyanov
 Project-URL: Homepage, https://github.com/stoyan-stoyanov/llmflows
 Project-URL: github, https://github.com/stoyan-stoyanov/llmflows
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,40 +21,46 @@
 [![Twitter](https://img.shields.io/twitter/follow/LLMFlows?style=social)](https://twitter.com/LLMFlows)
 ![Pylint workflow](https://github.com/stoyan-stoyanov/llmflow/actions/workflows/pylint.yml/badge.svg)
 ![License](https://img.shields.io/github/license/stoyan-stoyanov/llmflow)
 ![PyPi](https://img.shields.io/pypi/v/llmflows)
 ![Stars](https://img.shields.io/github/stars/stoyan-stoyanov/llmflow?style=social)
 ![Release date](https://img.shields.io/github/release-date/stoyan-stoyanov/llmflow?style=social)
 
+Documentation: [https://readthedocs.org](https://readthedocs.org/)<br/>
+PyPI: [https://pypi.org/project/llmflows](https://pypi.org/project/llmflows/)</br>
+Twitter: [https://twitter.com/LLMFlows](https://twitter.com/LLMFlows)<br/>
+Substack: [https://llmflows.substack.com](https://llmflows.substack.com/)<br/>
+
 ## About
-LLMFlows is a simple and lightweight framework for building LLM-powered applications.
+LLMFlows is a framework for building simple, explicit, and transparent LLM applications.
 
 ## Installation
-You can quickly install LLMFlows with pip
 ```
 pip install llmflows
 ```
 
-## Documentation
-The full documentation including user guides and api reference can be found at readthedocs.
-
 ## Philosophy
 
 ### Simple
-Our goal is to build a simple, well documented framework with a minimal set of classes and abstractions that allow users to build flexible LLM-powered apps without compromising on capabilities.
+Our goal is to build a simple, well-documented framework with minimal abstractions that 
+allow users to build flexible LLM-powered apps without compromising on capabilities.
 
 ### Explicit
-We want to create an explicit API enabling users to write clean, and readable code while being able to easily create complex flows of LLMs interacting with each other.
+We want to create an explicit API enabling users to write clean and readable code while 
+easily creating complex flows of LLMs interacting with each other.
 
 ### Transparent
-We aim helping users have full transparency on their LLM-powered apps by providing traceable flows, and complete information for each component of the app making it easy to monitor, maintain, and debug.
+We aim to help users have full transparency on their LLM-powered apps by providing 
+traceable flows and complete information for each app component, making it easy to 
+monitor, maintain, and debug.
 
 
 ## Usage
-Here is a minimal example of an LLM with a PromptTemplate:
+You can quickly build a simple application with LLMFlows' `LLM` and `PrompTemplate` 
+classes:
 
 ```python
 
 from llmflows.llms.openai import OpenAI
 from llmflows.prompts.prompt_template import PromptTemplate
 
 prompt_template = PromptTemplate(
@@ -63,34 +69,39 @@
 llm_prompt = prompt_template.get_prompt(topic="friendship")
 
 llm = OpenAI()
 song_title = llm.generate(llm_prompt)
 
 ```
 
-While this is a good example on how easy it is to use LLMFlows, real-world applications are more complex and have dependencies between prompts, and LLMs outputs. Let's take a look at such example. 
+However, real-world applications are often more complex and have dependencies between 
+prompts and LLM calls. For example:
+
 ![Complex flow](docs/complex_flow.png)
-With LLMFlows it's quite easy to reproduce this flow by utilizing the Flow and Flowstep classes. LLMFlows will figure out the dependencies and make sure each flowstep is executed only when the flowsteps it depends on are complete:
+
+You can build such flow using the `Flow` and `Flowstep` classes. LLMFlows will figure 
+out the dependencies and make sure each flowstep runs only when all its dependencies 
+are met:
 
 ```python
-from llmflows.flows import Flow, Flowstep
+from llmflows.flows import Flow, FlowStep
 from llmflows.llms import OpenAI
 from llmflows.prompts import PromptTemplate
 
 # Create prompt templates
 title_template = PromptTemplate("What is a good title of a movie about {topic}?")
 song_template = PromptTemplate(
     "What is a good song title of a soundtrack for a movie called {movie_title}?"
 )
 characters_template = PromptTemplate(
     "What are two main characters for a movie called {movie_title}?"
 )
 lyrics_template = PromptTemplate(
-    "Write lyrics of a movie song called {song_title}. The main characters are"
-    " {main_characters}"
+    "Write lyrics of a movie song called {song_title}. The main characters are "
+    "{main_characters}"
 )
 
 # Create flowsteps
 flowstep1 = FlowStep(
     name="Flowstep 1",
     llm=OpenAI(),
     prompt_template=title_template,
@@ -121,45 +132,55 @@
 # Connect flowsteps
 flowstep1.connect(flowstep2, flowstep3, flowstep4)
 flowstep2.connect(flowstep4)
 flowstep3.connect(flowstep4)
 
 # Create and run Flow
 soundtrack_flow = Flow(flowstep1)
-soundtrack_flow.execute(topic="friendship")
-
+results = soundtrack_flow.start(topic="friendship", verbose=True)
 ```
-In fact, LLMFlows provides async, and threaded classes so any complex DAG can be executed in parallel.
-For more examples such as how to create question answering apps and web applications with Flask and FastAPI check our documentation.
+
+In addition, LLMFlows provides async classes to improve the runtime of any complex flow 
+by running flow steps that already have all their required inputs in parallel.
+Check our documentation for more examples, such as creating question-answering apps and 
+web applications with Flask and FastAPI.
 
 ## FAQ
 
 ### How is this different than langchain?
-Langchain is a great library and LLMFlows has been been certainly inspired by it. However, our philosophy is a bit different. Langchian has a "chain for everything" philosophy and provides many classes that come with multiple LLM calls, logic, and built-in default prompts. While this is great for beginners and default use-cases, we feel this can be a bit overwhelming if users want to do anything "out of the ordinary". In contrast, we are focusing on providing as few building blocks as possible and having an easy to understand API while matching (and in some cases exceeding) the capabilities of langchain.
-
-### You only have OpenAI wrappers but I want to use AcmeLLM?
-We decided to release the library initially supporting only OpenAI LLMs but we have a roadmap and we will slowly add new wrappers around the most popular models. If you are willing to spend some time we are looking for contributors and maintainers
-
-### You only support Pinecone and Redis vector DBs do you have plans to extend the list?
-Yes! We will also add Redis, Elastic Search and other popular solutions over time. If you want to help us out check out our contribution section.
+Langchain is a great library, and LLMFlows has undoubtedly been inspired by it. 
+However, our philosophy is a bit different. Langchian has a "chain for everything" 
+philosophy and provides many classes with multiple LLM calls, logic, and built-in 
+default prompts. While this is great for beginners and default use cases, we feel this 
+can be overwhelming if users want to do anything "out of the ordinary." In contrast, 
+we are focusing on providing as few building blocks as possible and having an 
+easy-to-understand API while matching (and in some cases exceeding) the capabilities 
+of langchain.
+
+### You only have OpenAI wrappers, but I want to use AcmeLLM.
+We decided to release the library initially supporting only OpenAI LLMs, but we have a 
+roadmap and will slowly add new wrappers around the most popular models. If you are 
+willing to spend some time, we are looking for contributors and maintainers.
+
+### You only support Pinecone. Do you have plans to extend the list?
+Yes! Over time, we will also add Chroma, Weaviate, Redis, Elastic Search, and other 
+popular solutions. If you want to help us out, check out our contribution section.
 
 ### Why can't I find any info related to document loaders?
-For the time being we have decided not to implement document loaders for few reasons:
-1. There are plenty of capable libraries like Llama-index and langchain that have tons of loaders.
-2. We think it is awkward to mix document loaders together with LLM and prompt management libraries since usually document loading happens in separate pipelines and are not part of the LLM-powered app.
-3. Real-life documents are messy. In our experience, no matter how many loaders are out there they will never cover all the specific use-cases.
+For the time being, we have decided not to implement document loaders for a few reasons:
 
-While we are not going to invest time into document loaders we might decide to change direction if we get significant interest and contributors.
+1. plenty of capable libraries like Llama-index and langchain have tons of loaders.
+2. We think mixing document loaders with LLM and prompt management libraries is awkward 
+3. since document loading usually happens in separate pipelines and is not part of the 
+4. LLM-powered app.
+5. Real-life documents are messy. In our experience, no matter how many loaders are out 
+6. there, they will never cover all the specific use cases.
 
-### What about agents?
-We believe agents are the future of LLM-powered apps and we have a few basic examples in the repo. However, we are working on a agent-focused library built on top of llmflow.
+While we will not invest time into document loaders, we might change direction if we 
+get significant interest and contributors.
 
 ## License
-LLMFlows is covered by the MIT license. For more information check `LICENCE.md`.
+LLMFlows is covered by the MIT license. For more information, check `LICENCE.md`.
 
 ## Contributing
-Thank you for spending the time to read our README! If you like what you saw and are considering contributing please check CONTRIBUTING.md
-
-## Links
-Twitter
-
-Documentation
+Thank you for spending the time to read our README! If you like what you saw and are 
+considering contributing, please check `CONTRIBUTING.md`
```

### Comparing `llmflows-0.0.5/llmflows.egg-info/SOURCES.txt` & `llmflows-0.0.6/llmflows.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.5/pyproject.toml` & `llmflows-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "llmflows"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Stoyan Stoyanov"},
 ]
 description = "LLMFlows - Simple, Explicit and Transparent LLM Apps"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

