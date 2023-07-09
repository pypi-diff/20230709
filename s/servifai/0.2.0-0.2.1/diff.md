# Comparing `tmp/servifai-0.2.0.tar.gz` & `tmp/servifai-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servifai-0.2.0.tar", max compression
+gzip compressed data, was "servifai-0.2.1.tar", max compression
```

## Comparing `servifai-0.2.0.tar` & `servifai-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1067 2023-06-29 08:21:05.500102 servifai-0.2.0/LICENSE
--rw-r--r--   0        0        0     4273 2023-07-07 16:02:37.891863 servifai-0.2.0/README.md
--rw-r--r--   0        0        0      773 2023-07-07 16:03:13.607863 servifai-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       53 2023-07-07 16:03:00.447863 servifai-0.2.0/servifai/__init__.py
--rw-r--r--   0        0        0      243 2023-07-07 16:02:37.899863 servifai-0.2.0/servifai/default_config.yaml
--rw-r--r--   0        0        0       26 2023-07-07 16:02:37.899863 servifai-0.2.0/servifai/llm/__init__.py
--rw-r--r--   0        0        0      389 2023-07-07 16:02:37.899863 servifai-0.2.0/servifai/llm/base.py
--rw-r--r--   0        0        0     1343 2023-07-07 16:02:37.899863 servifai-0.2.0/servifai/llm/openai.py
--rw-r--r--   0        0        0       29 2023-07-07 16:02:37.899863 servifai-0.2.0/servifai/memory/__init__.py
--rw-r--r--   0        0        0     1780 2023-07-07 16:02:37.899863 servifai-0.2.0/servifai/memory/chroma.py
--rw-r--r--   0        0        0       34 2023-07-07 16:02:37.899863 servifai-0.2.0/servifai/planning/__init__.py
--rw-r--r--   0        0        0      891 2023-07-07 16:02:37.899863 servifai-0.2.0/servifai/planning/react.py
--rw-r--r--   0        0        0     2090 2023-07-07 16:02:37.899863 servifai-0.2.0/servifai/servifai.py
--rw-r--r--   0        0        0       30 2023-07-07 16:02:37.899863 servifai-0.2.0/servifai/toolbox/__init__.py
--rw-r--r--   0        0        0      864 2023-07-07 16:02:37.899863 servifai-0.2.0/servifai/toolbox/base.py
--rw-r--r--   0        0        0     1285 2023-07-07 16:02:37.899863 servifai-0.2.0/servifai/toolbox/default.py
--rw-r--r--   0        0        0     6645 2023-07-07 16:02:37.899863 servifai-0.2.0/servifai/toolbox/knowledge_base.py
--rw-r--r--   0        0        0     5193 1970-01-01 00:00:00.000000 servifai-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-29 08:21:05.500102 servifai-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4278 2023-07-07 16:08:24.619863 servifai-0.2.1/README.md
+-rw-r--r--   0        0        0      773 2023-07-08 16:05:56.780199 servifai-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       53 2023-07-08 16:05:46.156199 servifai-0.2.1/servifai/__init__.py
+-rw-r--r--   0        0        0      243 2023-07-07 16:02:37.899863 servifai-0.2.1/servifai/default_config.yaml
+-rw-r--r--   0        0        0       26 2023-07-07 16:02:37.899863 servifai-0.2.1/servifai/llm/__init__.py
+-rw-r--r--   0        0        0      389 2023-07-07 16:02:37.899863 servifai-0.2.1/servifai/llm/base.py
+-rw-r--r--   0        0        0     1371 2023-07-08 16:06:18.140199 servifai-0.2.1/servifai/llm/openai.py
+-rw-r--r--   0        0        0       29 2023-07-07 16:02:37.899863 servifai-0.2.1/servifai/memory/__init__.py
+-rw-r--r--   0        0        0     1812 2023-07-08 16:06:17.516199 servifai-0.2.1/servifai/memory/chroma.py
+-rw-r--r--   0        0        0       34 2023-07-07 16:02:37.899863 servifai-0.2.1/servifai/planning/__init__.py
+-rw-r--r--   0        0        0     1071 2023-07-08 16:06:17.544199 servifai-0.2.1/servifai/planning/react.py
+-rw-r--r--   0        0        0     2011 2023-07-08 16:06:17.644199 servifai-0.2.1/servifai/servifai.py
+-rw-r--r--   0        0        0       30 2023-07-07 16:02:37.899863 servifai-0.2.1/servifai/toolbox/__init__.py
+-rw-r--r--   0        0        0      864 2023-07-08 16:06:17.600199 servifai-0.2.1/servifai/toolbox/base.py
+-rw-r--r--   0        0        0     1417 2023-07-08 16:06:17.676199 servifai-0.2.1/servifai/toolbox/default.py
+-rw-r--r--   0        0        0     7265 2023-07-08 16:06:17.908199 servifai-0.2.1/servifai/toolbox/knowledge_base.py
+-rw-r--r--   0        0        0     5198 1970-01-01 00:00:00.000000 servifai-0.2.1/PKG-INFO
```

### Comparing `servifai-0.2.0/LICENSE` & `servifai-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `servifai-0.2.0/README.md` & `servifai-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 Me: Hi, How are you?
 ServifAI: Hi, I'm an AI language model, so I don't have feelings, but I'm here to help you with any questions or tasks you have!
 
 Me: What is the current weather of Bengaluru?
 ServifAI: The current weather in Bengaluru is mostly cloudy with a temperature of 81°F (27°C). The wind is coming from the north at 3 mph (5 km/h). Tomorrow's temperature is expected to be nearly the same as today.
 
 ```
-## Data Creation Recipe for Local Knowledge Extraction Tasks
+## Data Creation Recipe for Local Docs Knowledge Extraction Tasks
 Consider the example of [Uber 10Q filings](https://investor.uber.com/financials/default.aspx). 
 - Download the quaterly reports for year 2022 and 2023 as pdf and save it locally in a directory (here `reports`).
 - Create a config YAML file `uber10q.yaml` inside a `configs` dir and fill details as:
 ```yaml
 task: qna_local_docs
 
 llm:
```

### Comparing `servifai-0.2.0/pyproject.toml` & `servifai-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "servifai"
-version = "0.2.0"
+version = "0.2.1"
 description = "A mini framework built on top of Langchain and Llamaindex to provide LLM powered Autonomous Agents as a simplified service to assist users with their tasks"
 authors = ["Zoheb Abai <zohebabai@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `servifai-0.2.0/servifai/llm/openai.py` & `servifai-0.2.1/servifai/llm/openai.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from dotenv import load_dotenv
 from langchain.chat_models import AzureChatOpenAI, ChatOpenAI
 
 load_dotenv()
 
 
 class OpenAI:
+    """OpenAI LLM Class"""
+
     def __init__(self, llmconfigs):
         self._name = llmconfigs["model"]
         self._temp = int(llmconfigs["temperature"])
         self._max_tokens = int(llmconfigs["max_tokens"])
         self.model = self._get_openai_model()
 
     def _get_openai_model(self):
```

### Comparing `servifai-0.2.0/servifai/memory/chroma.py` & `servifai-0.2.1/servifai/memory/chroma.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from langchain.embeddings import OpenAIEmbeddings
 from llama_index import LangchainEmbedding
 
 load_dotenv()
 
 
 class ChromaDB:
+    """ChromaDB vectorstore"""
+
     def __init__(self, db_dir):
         self._path = db_dir
         self._oai_org = os.getenv("OPENAI_API_TYPE")
         self._client_settings = chromadb.config.Settings(
             chroma_db_impl="duckdb+parquet",
             persist_directory=str(self._path),
             anonymized_telemetry=False,
```

### Comparing `servifai-0.2.0/servifai/planning/react.py` & `servifai-0.2.1/servifai/planning/react.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 from langchain.agents import initialize_agent
 from langchain.chains.conversation.memory import ConversationBufferMemory
 
 from servifai.toolbox import BaseToolBox
 
 
 class ReactChatAgent:
+    """React Chat Agent"""
+
     def __init__(self, task, llm, dbdir, datadir, dataconfigs, memoryconfigs):
         self.llm = llm
         self.toolbox = BaseToolBox(
             task, llm, dbdir, datadir, dataconfigs, memoryconfigs
         ).toolbox
         self.memory = ConversationBufferMemory(
             memory_key="chat_history", return_messages=True
         )
 
-    def query(self, query: str):
+    def query(self, query: str) -> str:
+        """agent query response
+
+        Args:
+            query (str): user query
+
+        Returns:
+            str: agent response
+        """
         agent = initialize_agent(
             self.toolbox,
             self.llm.model,
             agent="chat-conversational-react-description",
             verbose=True,
             memory=self.memory,
             max_iterations=3,
```

### Comparing `servifai-0.2.0/servifai/servifai.py` & `servifai-0.2.1/servifai/servifai.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,20 +13,17 @@
 
 BASE_DIR = Path(__file__).parent.parent.absolute()
 LOGS_DIR = Path(BASE_DIR, "logs")
 DEFAULT_CONFIG = Path(BASE_DIR, "servifai/default_config.yaml")
 
 
 class ServifAI:
-    def __init__(self, config_file=None):
-        """Initializes a ServifAI instance with specific config for a given task
+    """Initializes a ServifAI instance with specific config for a given task"""
 
-        Args:
-            cfg (DictConfig): specific constants for a particular data
-        """
+    def __init__(self, config_file=None):
         self.cfg = self._load_config(config_file)
         self.task = self.cfg["task"]
         self.llm = BaseLLM(self.cfg["llm"]).llm
         self.agent = ReactChatAgent(
             self.task,
             self.llm,
             Path(BASE_DIR, self.cfg["memory"]["dir"]),
@@ -44,24 +41,24 @@
             logging.warning(
                 "No Config file provided by user, hence switching to default!"
             )
             with open(DEFAULT_CONFIG, "r") as file:
                 config = yaml.safe_load(file)
         return config
 
-    def chat(self, question: str):
+    def chat(self, question: str) -> str:
         """Responds to user query as chat conversation
 
         Args:
             question (str): user query
 
         Returns:
             str: Response
         """
         try:
             if not question:
                 logging.warning("No input text provided by user")
-                return "No input provided by user"
+                return "No input provided by user. Try Again."
             logging.info("Generating response:")
             return self.agent.query(question)
         except Exception as e:
             logging.error(f"Error: {e}")
```

### Comparing `servifai-0.2.0/servifai/toolbox/base.py` & `servifai-0.2.1/servifai/toolbox/base.py`

 * *Files identical despite different names*

### Comparing `servifai-0.2.0/servifai/toolbox/default.py` & `servifai-0.2.1/servifai/toolbox/default.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from langchain.agents import Tool
 from langchain.chains import LLMMathChain, PALChain
 from langchain.tools import DuckDuckGoSearchRun
 
 
 class DefaultTools:
+    """ServifAI Default Toolbox"""
+
     def __init__(self, llm):
         self.llm = llm
         self.palmath_tool = self._get_pal_math()
         self.llmmath_tool = self._get_llm_math()
         self.web_search = self._get_ddg_search()
 
     def _get_pal_math(self):
@@ -28,8 +30,13 @@
         return Tool(
             name="Web Search",
             description="A search engine. Useful for when you need to answer questions about current events from internet. Input should be a search query.",
             func=DuckDuckGoSearchRun().run,
         )
 
     def as_tool(self):
+        """access default toolbox
+
+        Returns:
+            list: list of tools
+        """
         return [self.palmath_tool, self.llmmath_tool, self.web_search]
```

### Comparing `servifai-0.2.0/servifai/toolbox/knowledge_base.py` & `servifai-0.2.1/servifai/toolbox/knowledge_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,34 +15,46 @@
 from llama_index.query_engine.transform_query_engine import TransformQueryEngine
 from llama_index.vector_stores import ChromaVectorStore
 
 from servifai.memory import ChromaDB
 
 
 class VectorKnowledgeBase:
+    """Vector Index Knowledge Base"""
+
     def __init__(self, vector_indices, index_summaries, service_context):
         self._indices = vector_indices
         self._summaries = index_summaries
         self._service_context = service_context
 
-    def as_tool(self, title):
+    def as_tool(self, title: str) -> Tool:
+        """access vector index as a tool
+
+        Args:
+            title (str): index title
+
+        Returns:
+            Tool: index as tool
+        """
         index = self._indices[title]
         summary = self._summaries[title]
         query_engine = index.as_query_engine(
             service_context=self._service_context, similarity_top_k=3
         )
         return Tool(
             name=f"Knowledge Vector Index {title}",
             func=lambda q: str(query_engine.query(q)),
             description=f"useful for answering queries only regarding {summary}",
             return_direct=True,
         )
 
 
 class KnowledgeGraphs:
+    """Graph Knowledge Base"""
+
     def __init__(self, vector_indices, index_summaries, service_context, llm_predictor):
         self._indices = vector_indices
         self._summaries = index_summaries
         self._service_context = service_context
         self._llm_pred = llm_predictor
         self._graph = None
         self._custom_query_engines = {}
@@ -74,24 +86,34 @@
             response_mode="tree_summarize",
             service_context=self._service_context,
         )
         return self._graph.as_query_engine(
             custom_query_engines=self._custom_query_engines
         )
 
-    def as_tool(self, about):
+    def as_tool(self, about: str) -> Tool:
+        """access knowledge graph as tool
+
+        Args:
+            about (str): about the data
+
+        Returns:
+            Tool: graph as tool
+        """
         return Tool(
             name="Knowledge Graph Index",
             func=lambda q: str(self._query_engine.query(q)),
             description=f"useful for answering queries that require comparing/contrasting or analyzing over multiple sources about {about}",
             return_direct=True,
         )
 
 
 class KnowledgeBase:
+    """Combined Knowledge Base including vector and graph indices"""
+
     def __init__(self, vdb_dir, data_dir, about, memoryconfigs, oaillm):
         self.vdb_dir = vdb_dir
         self.data_dir = data_dir
         self.about = about
         self.max_input_size = int(memoryconfigs["max_input_size"])
         self.num_outputs = int(memoryconfigs["num_outputs"])
         self.max_chunk_overlap = float(memoryconfigs["max_chunk_overlap"])
@@ -169,8 +191,13 @@
         kg_tool = KnowledgeGraphs(
             self.indices, self.index_summaries, self.service_context, self.llm_predictor
         ).as_tool(self.about)
         qe_tools.append(kg_tool)
         return qe_tools
 
     def as_tool(self):
+        """access the combined knowledge base as a tool
+
+        Returns:
+            list: list of knowledge indices as tools
+        """
         return self.qe_tools
```

### Comparing `servifai-0.2.0/PKG-INFO` & `servifai-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servifai
-Version: 0.2.0
+Version: 0.2.1
 Summary: A mini framework built on top of Langchain and Llamaindex to provide LLM powered Autonomous Agents as a simplified service to assist users with their tasks
 License: MIT
 Author: Zoheb Abai
 Author-email: zohebabai@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -78,15 +78,15 @@
 Me: Hi, How are you?
 ServifAI: Hi, I'm an AI language model, so I don't have feelings, but I'm here to help you with any questions or tasks you have!
 
 Me: What is the current weather of Bengaluru?
 ServifAI: The current weather in Bengaluru is mostly cloudy with a temperature of 81°F (27°C). The wind is coming from the north at 3 mph (5 km/h). Tomorrow's temperature is expected to be nearly the same as today.
 
 ```
-## Data Creation Recipe for Local Knowledge Extraction Tasks
+## Data Creation Recipe for Local Docs Knowledge Extraction Tasks
 Consider the example of [Uber 10Q filings](https://investor.uber.com/financials/default.aspx). 
 - Download the quaterly reports for year 2022 and 2023 as pdf and save it locally in a directory (here `reports`).
 - Create a config YAML file `uber10q.yaml` inside a `configs` dir and fill details as:
 ```yaml
 task: qna_local_docs
 
 llm:
```

