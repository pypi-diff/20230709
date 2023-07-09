# Comparing `tmp/gpttrace-0.1.1.tar.gz` & `tmp/gpttrace-0.1.2.tar.gz`

## Comparing `gpttrace-0.1.1.tar` & `gpttrace-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 gpttrace-0.1.1/LICENSE
--rw-r--r--   0        0        0     8129 2020-02-02 00:00:00.000000 gpttrace-0.1.1/README.md
--rw-r--r--   0        0        0   127304 2020-02-02 00:00:00.000000 gpttrace-0.1.1/data_save/funcs.json
--rw-r--r--   0        0        0  1254913 2020-02-02 00:00:00.000000 gpttrace-0.1.1/data_save/vector_database/docstore.json
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 gpttrace-0.1.1/data_save/vector_database/graph_store.json
--rw-r--r--   0        0        0    49891 2020-02-02 00:00:00.000000 gpttrace-0.1.1/data_save/vector_database/index_store.json
--rw-r--r--   0        0        0 20395238 2020-02-02 00:00:00.000000 gpttrace-0.1.1/data_save/vector_database/vector_store.json
--rw-r--r--   0        0        0    59144 2020-02-02 00:00:00.000000 gpttrace-0.1.1/doc/api-key.png
--rw-r--r--   0        0        0    47700 2020-02-02 00:00:00.000000 gpttrace-0.1.1/doc/generate.png
--rw-r--r--   0        0        0   311412 2020-02-02 00:00:00.000000 gpttrace-0.1.1/doc/result.gif
--rw-r--r--   0        0        0    33423 2020-02-02 00:00:00.000000 gpttrace-0.1.1/doc/result.png
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 gpttrace-0.1.1/doc/talk.md
--rwxr-xr-x   0        0        0     2637 2020-02-02 00:00:00.000000 gpttrace-0.1.1/gpttrace/GPTtrace.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 gpttrace-0.1.1/gpttrace/__init__.py
--rw-r--r--   0        0        0     8720 2020-02-02 00:00:00.000000 gpttrace-0.1.1/gpttrace/cmd.py
--rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 gpttrace-0.1.1/gpttrace/config.py
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 gpttrace-0.1.1/gpttrace/execute.py
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 gpttrace-0.1.1/gpttrace/generate.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 gpttrace-0.1.1/gpttrace/utils/__init__.py
--rw-r--r--   0        0        0     4086 2020-02-02 00:00:00.000000 gpttrace-0.1.1/gpttrace/utils/common.py
--rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 gpttrace-0.1.1/gpttrace/utils/prompt.py
--rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 gpttrace-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 gpttrace-0.1.1/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 gpttrace-0.1.1/LICENSE
--rw-r--r--   0        0        0     8129 2020-02-02 00:00:00.000000 gpttrace-0.1.1/README.md
--rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 gpttrace-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     9577 2020-02-02 00:00:00.000000 gpttrace-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 gpttrace-0.1.2/LICENSE
+-rw-r--r--   0        0        0     8129 2020-02-02 00:00:00.000000 gpttrace-0.1.2/README.md
+-rw-r--r--   0        0        0   127304 2020-02-02 00:00:00.000000 gpttrace-0.1.2/data_save/funcs.json
+-rw-r--r--   0        0        0  1254913 2020-02-02 00:00:00.000000 gpttrace-0.1.2/data_save/vector_database/docstore.json
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 gpttrace-0.1.2/data_save/vector_database/graph_store.json
+-rw-r--r--   0        0        0    49891 2020-02-02 00:00:00.000000 gpttrace-0.1.2/data_save/vector_database/index_store.json
+-rw-r--r--   0        0        0 20395238 2020-02-02 00:00:00.000000 gpttrace-0.1.2/data_save/vector_database/vector_store.json
+-rw-r--r--   0        0        0    59144 2020-02-02 00:00:00.000000 gpttrace-0.1.2/doc/api-key.png
+-rw-r--r--   0        0        0    47700 2020-02-02 00:00:00.000000 gpttrace-0.1.2/doc/generate.png
+-rw-r--r--   0        0        0   311412 2020-02-02 00:00:00.000000 gpttrace-0.1.2/doc/result.gif
+-rw-r--r--   0        0        0    33423 2020-02-02 00:00:00.000000 gpttrace-0.1.2/doc/result.png
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 gpttrace-0.1.2/doc/talk.md
+-rwxr-xr-x   0        0        0     2637 2020-02-02 00:00:00.000000 gpttrace-0.1.2/gpttrace/GPTtrace.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 gpttrace-0.1.2/gpttrace/__init__.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 gpttrace-0.1.2/gpttrace/__main__.py
+-rw-r--r--   0        0        0     8720 2020-02-02 00:00:00.000000 gpttrace-0.1.2/gpttrace/cmd.py
+-rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 gpttrace-0.1.2/gpttrace/config.py
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 gpttrace-0.1.2/gpttrace/execute.py
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 gpttrace-0.1.2/gpttrace/generate.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 gpttrace-0.1.2/gpttrace/utils/__init__.py
+-rw-r--r--   0        0        0     4086 2020-02-02 00:00:00.000000 gpttrace-0.1.2/gpttrace/utils/common.py
+-rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 gpttrace-0.1.2/gpttrace/utils/prompt.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 gpttrace-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 gpttrace-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 gpttrace-0.1.2/LICENSE
+-rw-r--r--   0        0        0     8129 2020-02-02 00:00:00.000000 gpttrace-0.1.2/README.md
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 gpttrace-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 gpttrace-0.1.2/PKG-INFO
```

### Comparing `gpttrace-0.1.1/LICENSE` & `gpttrace-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gpttrace-0.1.1/README.md` & `gpttrace-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `gpttrace-0.1.1/data_save/funcs.json` & `gpttrace-0.1.2/data_save/funcs.json`

 * *Files identical despite different names*

### Comparing `gpttrace-0.1.1/data_save/vector_database/docstore.json` & `gpttrace-0.1.2/data_save/vector_database/docstore.json`

 * *Files identical despite different names*

### Comparing `gpttrace-0.1.1/data_save/vector_database/index_store.json` & `gpttrace-0.1.2/data_save/vector_database/index_store.json`

 * *Files identical despite different names*

### Comparing `gpttrace-0.1.1/data_save/vector_database/vector_store.json` & `gpttrace-0.1.2/data_save/vector_database/vector_store.json`

 * *Files identical despite different names*

### Comparing `gpttrace-0.1.1/doc/api-key.png` & `gpttrace-0.1.2/doc/api-key.png`

 * *Files identical despite different names*

### Comparing `gpttrace-0.1.1/doc/generate.png` & `gpttrace-0.1.2/doc/generate.png`

 * *Files identical despite different names*

### Comparing `gpttrace-0.1.1/doc/result.gif` & `gpttrace-0.1.2/doc/result.gif`

 * *Files identical despite different names*

### Comparing `gpttrace-0.1.1/doc/result.png` & `gpttrace-0.1.2/doc/result.png`

 * *Files identical despite different names*

### Comparing `gpttrace-0.1.1/doc/talk.md` & `gpttrace-0.1.2/doc/talk.md`

 * *Files identical despite different names*

### Comparing `gpttrace-0.1.1/gpttrace/GPTtrace.py` & `gpttrace-0.1.2/gpttrace/GPTtrace.py`

 * *Files identical despite different names*

### Comparing `gpttrace-0.1.1/gpttrace/cmd.py` & `gpttrace-0.1.2/gpttrace/cmd.py`

 * *Files identical despite different names*

### Comparing `gpttrace-0.1.1/gpttrace/config.py` & `gpttrace-0.1.2/gpttrace/config.py`

 * *Files identical despite different names*

### Comparing `gpttrace-0.1.1/gpttrace/execute.py` & `gpttrace-0.1.2/gpttrace/execute.py`

 * *Files identical despite different names*

### Comparing `gpttrace-0.1.1/gpttrace/generate.py` & `gpttrace-0.1.2/gpttrace/generate.py`

 * *Files identical despite different names*

### Comparing `gpttrace-0.1.1/gpttrace/utils/common.py` & `gpttrace-0.1.2/gpttrace/utils/common.py`

 * *Files identical despite different names*

### Comparing `gpttrace-0.1.1/gpttrace/utils/prompt.py` & `gpttrace-0.1.2/gpttrace/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `gpttrace-0.1.1/pyproject.toml` & `gpttrace-0.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
-
 [project]
 name = "gpttrace"
 description = "Generate eBPF programs and tracing with ChatGPT and natural language."
 keywords = ["shell", "gpt", "openai", "cli", "productivity"]
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.6"
@@ -31,33 +30,36 @@
     "langchain>=0.0.227",
     "llama_index>=0.7.3",
     "marko>=2.0.0",
     "openai>=0.27.8",
     "prompt_toolkit>=3.0.38",
     "Pygments>=2.15.1",
     "pygments_markdown_lexer>=0.1.0.dev39",
+    "click>=8.1.4"
 ]
 
+# Program entry function of gpttrace.
 [project.scripts]
-sgpt = "gpttrace:cli"
+gpttrace = "gpttrace:main"
 
 [project.urls]
 homepage = "https://github.com/eunomia-bpf/GPTtrace"
 repository = "https://github.com/eunomia-bpf/GPTtrace"
 documentation = "https://github.com/eunomia-bpf/GPTtrace/blob/main/README.md"
 
 [tool.hatch.version]
 path = "gpttrace/__init__.py"
 
+# Generate the .whl file, which is installed when the user use `pip install package`
 [tool.hatch.build.targets.wheel]
 only-include = [
     "gpttrace",
     "data_save",
 ]
-
+# This will be uploaded to pypi.
 [tool.hatch.build.targets.sdist]
 only-include = [
     "gpttrace",
     "doc",
     "data_save",
     "README.md",
     "LICENSE",
```

### Comparing `gpttrace-0.1.1/.gitignore` & `gpttrace-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `gpttrace-0.1.1/PKG-INFO` & `gpttrace-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpttrace
-Version: 0.1.1
+Version: 0.1.2
 Summary: Generate eBPF programs and tracing with ChatGPT and natural language.
 Project-URL: homepage, https://github.com/eunomia-bpf/GPTtrace
 Project-URL: repository, https://github.com/eunomia-bpf/GPTtrace
 Project-URL: documentation, https://github.com/eunomia-bpf/GPTtrace/blob/main/README.md
 Author-email: eunomia-bpf <2629757717@qq.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Requires-Python: >=3.6
+Requires-Dist: click>=8.1.4
 Requires-Dist: langchain>=0.0.227
 Requires-Dist: llama-index>=0.7.3
 Requires-Dist: marko>=2.0.0
 Requires-Dist: openai>=0.27.8
 Requires-Dist: prompt-toolkit>=3.0.38
 Requires-Dist: pygments-markdown-lexer>=0.1.0.dev39
 Requires-Dist: pygments>=2.15.1
```

