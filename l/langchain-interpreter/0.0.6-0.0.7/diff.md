# Comparing `tmp/langchain_interpreter-0.0.6.tar.gz` & `tmp/langchain_interpreter-0.0.7.tar.gz`

## Comparing `langchain_interpreter-0.0.6.tar` & `langchain_interpreter-0.0.7.tar`

### file list

```diff
@@ -1,25 +1,32 @@
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/.readthedocs.yaml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/requirements.txt
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/docs/Makefile
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/docs/conf.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/docs/index.rst
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/docs/langchain_interpreter.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/docs/make.bat
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/docs/modules.rst
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/docs/requirements.txt
--rw-r--r--   0        0        0    17907 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/src/examples/chains_from_json.ipynb
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/src/examples/json_from_chains.ipynb
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/src/examples/validation.ipynb
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/src/json/conv_buffer_memory.json
--rwxr-xr-x   0        0        0      403 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/src/json/llmchain.json
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/src/json/seq_chain.json
--rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/src/json/seq_chain_memory.json
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/src/json/simple_seq_chain.json
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/src/langchain_interpreter/__init__.py
--rwxr-xr-x   0        0        0     4785 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/src/langchain_interpreter/main.py
--rw-r--r--   0        0        0     5609 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/src/langchain_interpreter/validation.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/LICENSE
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/README.md
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.7/.readthedocs.yaml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.7/requirements.txt
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.7/docs/Makefile
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.7/docs/chromadb_example.md
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.7/docs/conf.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.7/docs/index.rst
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.7/docs/langchain_interpreter.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.7/docs/make.bat
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.7/docs/modules.rst
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.7/docs/mongodb_example.md
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.7/docs/requirements.txt
+-rw-r--r--   0        0        0    18054 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.7/src/examples/chains_from_json.ipynb
+-rw-r--r--   0        0        0     8651 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.7/src/examples/chromadb_example.ipynb
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.7/src/examples/json_from_chains.ipynb
+-rw-r--r--   0        0        0    18605 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.7/src/examples/mongodbvector_example.ipynb
+-rw-r--r--   0        0        0    39027 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.7/src/examples/state_of_the_union.txt
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.7/src/examples/validation.ipynb
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.7/src/json/chromadb_chain.json
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.7/src/json/conv_buffer_memory.json
+-rwxr-xr-x   0        0        0      403 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.7/src/json/llmchain.json
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.7/src/json/mongodbvector_chain.json
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.7/src/json/seq_chain.json
+-rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.7/src/json/seq_chain_memory.json
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.7/src/json/simple_seq_chain.json
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.7/src/langchain_interpreter/__init__.py
+-rwxr-xr-x   0        0        0     6626 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.7/src/langchain_interpreter/main.py
+-rw-r--r--   0        0        0     7079 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.7/src/langchain_interpreter/validation.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.7/LICENSE
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.7/README.md
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.7/PKG-INFO
```

### Comparing `langchain_interpreter-0.0.6/.readthedocs.yaml` & `langchain_interpreter-0.0.7/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.6/docs/Makefile` & `langchain_interpreter-0.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.6/docs/conf.py` & `langchain_interpreter-0.0.7/docs/conf.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,33 +5,36 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = "LangChain Interpreter"
 copyright = "2023, Elijah Tarr"
 author = "Elijah Tarr"
-release = "0.0.4"
+release = "0.0.7"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.napoleon",
     "sphinx.ext.todo",
     "sphinx.ext.coverage",
+    "myst_parser",
 ]
 
 templates_path = ["_templates"]
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = "furo"
 html_static_path = ["_static"]
 
+source_suffix = [".rst", ".md"]
+
 import os
 import sys
 
 sys.path.insert(0, os.path.abspath("../src"))
```

### Comparing `langchain_interpreter-0.0.6/docs/index.rst` & `langchain_interpreter-0.0.7/docs/index.rst`

 * *Files 20% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 .. toctree::
    :maxdepth: 2
    :caption: Contents:
 
    langchain_interpreter
    modules
+   mongodb_example.md
+   chromadb_example.md
 
 
 Indices and tables
 ==================
 
 * :ref:`genindex`
 * :ref:`modindex`
```

### Comparing `langchain_interpreter-0.0.6/docs/langchain_interpreter.rst` & `langchain_interpreter-0.0.7/docs/langchain_interpreter.rst`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.6/docs/make.bat` & `langchain_interpreter-0.0.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.6/src/examples/chains_from_json.ipynb` & `langchain_interpreter-0.0.7/src/examples/chains_from_json.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9824999999999999%*

 * *Differences: {"'cells'": "{0: {'execution_count': 2, 'outputs': [], 'source': {insert: [(2, '\\n'), (3, 'import "*

 * *            'sys\\n\'), (4, \'sys.path.append("..")\')]}}, insert: [(8, '*

 * *            "OrderedDict([('cell_type', 'code'), ('execution_count', 6), ('metadata', "*

 * *            "OrderedDict()), ('outputs', []), ('source', ['from langchain_interpreter import "*

 * *            "chain_from_file\\n', '\\n', 'chroma_chain = "*

 * *            'chain_from_file("../json/chromadb_chain.json")\'])]))]}'}*

```diff
@@ -1,28 +1,20 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": 2,
             "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "True"
-                        ]
-                    },
-                    "execution_count": 1,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
+            "outputs": [],
             "source": [
                 "from dotenv import load_dotenv\n",
-                "load_dotenv()\n"
+                "load_dotenv()\n",
+                "\n",
+                "import sys\n",
+                "sys.path.append(\"..\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [
@@ -254,14 +246,25 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "conversation.predict(input=\"not much. what about you?\")"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "from langchain_interpreter import chain_from_file\n",
+                "\n",
+                "chroma_chain = chain_from_file(\"../json/chromadb_chain.json\")"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "langchain",
             "language": "python",
             "name": "python3"
```

### Comparing `langchain_interpreter-0.0.6/src/examples/json_from_chains.ipynb` & `langchain_interpreter-0.0.7/src/examples/json_from_chains.ipynb`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.6/src/examples/validation.ipynb` & `langchain_interpreter-0.0.7/src/examples/validation.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9642857142857143%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'code'), ('execution_count', 2), "*

 * *            "('metadata', OrderedDict()), ('outputs', []), ('source', ['import sys\\n', "*

 * *            '\'sys.path.append("..")\'])])), (6, OrderedDict([(\'cell_type\', \'code\'), '*

 * *            "('execution_count', 4), ('metadata', OrderedDict()), ('outputs', []), ('source', "*

 * *            "['from langchain_interpreter import validate_file\\n', '\\n', "*

 * *            '\'validate_file("../json/chromadb_chain.json")\'])]))]}' […]*

```diff
@@ -1,11 +1,21 @@
 {
     "cells": [
         {
             "cell_type": "code",
+            "execution_count": 2,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "import sys\n",
+                "sys.path.append(\"..\")"
+            ]
+        },
+        {
+            "cell_type": "code",
             "execution_count": 27,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from langchain_interpreter import validate_file\n",
                 "\n",
                 "validate_file(\"../json/llmchain.json\")"
@@ -50,14 +60,25 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "from langchain_interpreter import validate_file\n",
                 "\n",
                 "validate_file(\"../json/conv_buffer_memory.json\")"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "from langchain_interpreter import validate_file\n",
+                "\n",
+                "validate_file(\"../json/chromadb_chain.json\")"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "lci",
             "language": "python",
             "name": "python3"
```

### Comparing `langchain_interpreter-0.0.6/src/json/seq_chain.json` & `langchain_interpreter-0.0.7/src/json/seq_chain.json`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.6/src/json/seq_chain_memory.json` & `langchain_interpreter-0.0.7/src/json/seq_chain_memory.json`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.6/src/json/simple_seq_chain.json` & `langchain_interpreter-0.0.7/src/json/simple_seq_chain.json`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.6/src/langchain_interpreter/main.py` & `langchain_interpreter-0.0.7/src/langchain_interpreter/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 from langchain.chains import (
     LLMChain,
     SimpleSequentialChain,
     SequentialChain,
     ConversationChain,
+    RetrievalQA,
 )
 from langchain import PromptTemplate, OpenAI, LLMChain
 from langchain.memory import SimpleMemory, ConversationBufferMemory
 from langchain.llms import type_to_cls_dict
 from langchain_interpreter import validate_chain
 import json
+import chromadb
+from langchain.vectorstores import Chroma
+from pymongo import MongoClient
+from langchain.vectorstores import MongoDBAtlasVectorSearch
+from langchain.embeddings.openai import OpenAIEmbeddings
 
 
 def chain_from_file(filename, **kwargs):
     """Generate a LangChain Chain from a json file.
 
     Args:
         filename (str): the path to the file containing json template.
@@ -44,20 +50,74 @@
     validate_chain(cfg)
     return get_chain(cfg["chain"], **kwargs)
 
 
 def get_chain(cfg, **kwargs):
     if cfg["type"] == "LLMChain":
         return get_llm_chain(cfg, **kwargs)
-    if cfg["type"] == "SimpleSequentialChain":
+    elif cfg["type"] == "SimpleSequentialChain":
         return get_simple_sequential_chain(cfg, **kwargs)
-    if cfg["type"] == "SequentialChain":
+    elif cfg["type"] == "SequentialChain":
         return get_sequential_chain(cfg, **kwargs)
-    if cfg["type"] == "ConversationChain":
+    elif cfg["type"] == "ConversationChain":
         return get_conversation_chain(cfg, **kwargs)
+    elif cfg["type"] == "RetrievalQA":
+        return get_retrieval_qa(cfg, **kwargs)
+    else:
+        raise NotImplementedError(f"{cfg['type']} isn't supported yet!")
+
+
+def get_retrieval_qa(cfg, **kwargs):
+    llm = get_llm(cfg["llm"], **kwargs)
+    chain_type = cfg["chain_type"]
+
+    retriever = get_retriever(cfg["retriever"], **kwargs)
+    return RetrievalQA.from_chain_type(
+        llm=llm, chain_type=chain_type, retriever=retriever
+    )
+
+
+def get_retriever(cfg, **kwargs):
+    if cfg["type"] == "vectorstore":
+        vectorstore = get_vectorstore(cfg["vectorstore"], **kwargs)
+        return vectorstore.as_retriever()
+
+
+def get_vectorstore(cfg, **kwargs):
+    if cfg["type"] == "ChromaDB":
+        return get_chromadb(cfg, **kwargs)
+    elif cfg["type"] == "MongoDB":
+        return get_mongodb(cfg, **kwargs)
+    else:
+        raise NotImplementedError(cfg["type"])
+
+
+def get_mongodb(cfg, **kwargs):
+    cluster = cfg["host"]
+    client = MongoClient(cluster)
+
+    # TODO: make these inputs
+    db_name = "langchain_db"
+    collection_name = "langchain_col"
+    collection = client[db_name][collection_name]
+    # index_name = "langchain_demo"
+
+    docsearch = MongoDBAtlasVectorSearch(collection, OpenAIEmbeddings())
+
+    return docsearch
+
+
+def get_chromadb(cfg, **kwargs) -> Chroma:
+    settings = chromadb.Settings(
+        chroma_api_impl="rest",
+        chroma_server_host=cfg["host"],
+        chroma_server_http_port=cfg["port"],
+    )
+    db = Chroma(client_settings=settings, embedding_function=OpenAIEmbeddings())
+    return db
 
 
 def get_conversation_chain(cfg, **kwargs):
     llm = get_llm(cfg["llm"], **kwargs)
     memory = try_memory(cfg, **kwargs)
 
     conv_chain = ConversationChain(llm=llm, memory=memory)
```

### Comparing `langchain_interpreter-0.0.6/src/langchain_interpreter/validation.py` & `langchain_interpreter-0.0.7/src/langchain_interpreter/validation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 from referencing import Registry, Resource
 from jsonschema import Draft202012Validator
 import json
 
 
 def get_validator():
-    template_resource = Resource.from_contents(template_schema)
-    chain_resource = Resource.from_contents(chain_schema)
-    llm_resource = Resource.from_contents(llm_schema)
-    prompt_resource = Resource.from_contents(prompt_schema)
-    memory_resource = Resource.from_contents(memory_schema)
-
-    registry = chain_resource @ (
-        llm_resource
-        @ (prompt_resource @ (memory_resource @ (template_resource @ Registry())))
-    )
+    registry = Resource.from_contents(template_schema) @ Registry()
+    registry = Resource.from_contents(chain_schema) @ registry
+    registry = Resource.from_contents(llm_schema) @ registry
+    registry = Resource.from_contents(prompt_schema) @ registry
+    registry = Resource.from_contents(memory_schema) @ registry
+    registry = Resource.from_contents(retriever_schema) @ registry
+    registry = Resource.from_contents(vectorstore_schema) @ registry
 
     validator = Draft202012Validator(template_schema, registry=registry)
 
     return validator
 
 
 def validate_chain(json):
@@ -98,14 +95,19 @@
             "description": "List of output variables for the chain",
             "items": {"type": "string"},
         },
         "output_key": {
             "type": "string",
             "description": "The key for the output of this specific chain.",
         },
+        "chain_type": {
+            "type": "string",
+            "description": "For retrieverqa, the chaintype",
+        },
+        "retriever": {"$ref": "https://example.com/retriever.schema.json"},
     },
     "additionalProperties": False,
     "required": ["type"],
 }
 
 llm_schema = {
     "$id": "https://example.com/llm.schema.json",
@@ -173,7 +175,49 @@
             "type": "string",
             "description": "String of previous conversation.",
         },
     },
     "additionalProperties": False,
     "required": ["type"],
 }
+
+retriever_schema = {
+    "$id": "https://example.com/retriever.schema.json",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
+    "title": "LangChain Retriever",
+    "description": "A langchain retriever object",
+    "type": "object",
+    "properties": {
+        "type": {
+            "type": "string",
+            "description": "The type of retriever.",
+        },
+        "vectorstore": {"$ref": "https://example.com/vectorstore.schema.json"},
+    },
+    "additionalProperties": False,
+    "required": ["type"],
+}
+
+
+vectorstore_schema = {
+    "$id": "https://example.com/vectorstore.schema.json",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
+    "title": "LangChain Vector Store",
+    "description": "A langchain vector store object",
+    "type": "object",
+    "properties": {
+        "type": {
+            "type": "string",
+            "description": "The type of vector store.",
+        },
+        "host": {
+            "type": "string",
+            "description": "The host for the vector store service.",
+        },
+        "port": {
+            "type": "string",
+            "description": "The port of the vector store service.",
+        },
+    },
+    "additionalProperties": False,
+    "required": ["type"],
+}
```

### Comparing `langchain_interpreter-0.0.6/.gitignore` & `langchain_interpreter-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.6/LICENSE` & `langchain_interpreter-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.6/README.md` & `langchain_interpreter-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.6/pyproject.toml` & `langchain_interpreter-0.0.7/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "langchain_interpreter"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Elijah Tarr", email="elijahotarr@gmail.com" },
 ]
 description = "A way to turn json into langchain pipelines."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `langchain_interpreter-0.0.6/PKG-INFO` & `langchain_interpreter-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain_interpreter
-Version: 0.0.6
+Version: 0.0.7
 Summary: A way to turn json into langchain pipelines.
 Project-URL: Homepage, https://github.com/eoriont/langchain_interpreter
 Project-URL: Bug Tracker, https://github.com/eoriont/langchain_interpreter/issues
 Author-email: Elijah Tarr <elijahotarr@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

