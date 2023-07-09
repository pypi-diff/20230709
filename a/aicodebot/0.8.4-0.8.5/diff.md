# Comparing `tmp/aicodebot-0.8.4.tar.gz` & `tmp/aicodebot-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aicodebot-0.8.4.tar", last modified: Fri Jul  7 01:54:06 2023, max compression
+gzip compressed data, was "aicodebot-0.8.5.tar", last modified: Sun Jul  9 16:52:58 2023, max compression
```

## Comparing `aicodebot-0.8.4.tar` & `aicodebot-0.8.5.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:54:06.340339 aicodebot-0.8.4/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-07 01:53:35.000000 aicodebot-0.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-07-07 01:54:06.340339 aicodebot-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11237 2023-07-07 01:53:35.000000 aicodebot-0.8.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:54:06.340339 aicodebot-0.8.4/aicodebot/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-07 01:53:35.000000 aicodebot-0.8.4/aicodebot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-07 01:53:35.000000 aicodebot-0.8.4/aicodebot/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)    17753 2023-07-07 01:53:35.000000 aicodebot-0.8.4/aicodebot/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-07-07 01:53:35.000000 aicodebot-0.8.4/aicodebot/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-07-07 01:53:35.000000 aicodebot-0.8.4/aicodebot/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:54:06.340339 aicodebot-0.8.4/aicodebot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-07-07 01:54:06.000000 aicodebot-0.8.4/aicodebot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-07 01:54:06.000000 aicodebot-0.8.4/aicodebot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 01:54:06.000000 aicodebot-0.8.4/aicodebot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-07 01:54:06.000000 aicodebot-0.8.4/aicodebot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-07 01:54:06.000000 aicodebot-0.8.4/aicodebot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 01:54:06.000000 aicodebot-0.8.4/aicodebot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-07 01:53:35.000000 aicodebot-0.8.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 01:54:06.340339 aicodebot-0.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-07 01:53:35.000000 aicodebot-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:52:58.189812 aicodebot-0.8.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-09 16:52:30.000000 aicodebot-0.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-07-09 16:52:58.189812 aicodebot-0.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11237 2023-07-09 16:52:30.000000 aicodebot-0.8.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:52:58.189812 aicodebot-0.8.5/aicodebot/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-09 16:52:30.000000 aicodebot-0.8.5/aicodebot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17753 2023-07-09 16:52:30.000000 aicodebot-0.8.5/aicodebot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-07-09 16:52:30.000000 aicodebot-0.8.5/aicodebot/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-07-09 16:52:30.000000 aicodebot-0.8.5/aicodebot/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:52:58.189812 aicodebot-0.8.5/aicodebot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-07-09 16:52:58.000000 aicodebot-0.8.5/aicodebot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-09 16:52:58.000000 aicodebot-0.8.5/aicodebot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 16:52:58.000000 aicodebot-0.8.5/aicodebot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-09 16:52:58.000000 aicodebot-0.8.5/aicodebot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-09 16:52:58.000000 aicodebot-0.8.5/aicodebot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-09 16:52:58.000000 aicodebot-0.8.5/aicodebot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-09 16:52:30.000000 aicodebot-0.8.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 16:52:58.189812 aicodebot-0.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-09 16:52:30.000000 aicodebot-0.8.5/setup.py
```

### Comparing `aicodebot-0.8.4/LICENSE` & `aicodebot-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aicodebot-0.8.4/PKG-INFO` & `aicodebot-0.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.8.4
+Version: 0.8.5
 Summary: Your AI-powered coding sidekick 🤖
 Home-page: https://github.com/gorillamania/AICodeBot
 Author: Nick Sullivan
 Keywords: AI,coding,assistant,pair-programming,automation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `aicodebot-0.8.4/README.md` & `aicodebot-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `aicodebot-0.8.4/aicodebot/cli.py` & `aicodebot-0.8.5/aicodebot/cli.py`

 * *Files identical despite different names*

### Comparing `aicodebot-0.8.4/aicodebot/helpers.py` & `aicodebot-0.8.5/aicodebot/helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from loguru import logger
 from pathlib import Path
-import os, subprocess, sys, tiktoken, yaml
+import fnmatch, os, subprocess, sys, tiktoken, yaml
 
 # ---------------------------------------------------------------------------- #
 #                    Global logging configuration for loguru                   #
 # ---------------------------------------------------------------------------- #
 
 
 logger.remove()
@@ -16,14 +16,39 @@
 logger = logger.opt(colors=True)
 
 # ---------------------------------------------------------------------------- #
 #                                Misc functions                                #
 # ---------------------------------------------------------------------------- #
 
 
+def generate_directory_structure(path, ignore_patterns=None, use_gitignore=True, indent=0):
+    """Generate a text representation of the directory structure of a path."""
+    ignore_patterns = ignore_patterns.copy() if ignore_patterns else []
+
+    base_path = Path(path)
+
+    if use_gitignore:
+        # Note: .gitignore files can exist in sub directories as well, such as * in __pycache__ directories
+        gitignore_file = base_path / ".gitignore"
+        if gitignore_file.exists():
+            with gitignore_file.open() as f:
+                ignore_patterns.extend(line.strip() for line in f if line.strip() and not line.startswith("#"))
+
+    structure = ""
+    if base_path.is_dir():
+        if not any(fnmatch.fnmatch(base_path.name, pattern) for pattern in ignore_patterns):
+            structure += "  " * indent + f"- [Directory] {base_path.name}\n"
+            for item in base_path.iterdir():
+                structure += generate_directory_structure(item, ignore_patterns, use_gitignore, indent + 1)
+    elif not any(fnmatch.fnmatch(base_path.name, pattern) for pattern in ignore_patterns):
+        structure += "  " * indent + f"- [File] {base_path.name}\n"
+
+    return structure
+
+
 def get_llm_model(token_size=0):
     # https://platform.openai.com/docs/models/gpt-3-5
     # We want to use GPT-4, if it is available for this OPENAI_API_KEY, otherwise GPT-3.5
     # We also want to use the largest model that supports the token size we need
     model_options = {
         "gpt-4": 8192,
         "gpt-4-32k": 32768,
```

### Comparing `aicodebot-0.8.4/aicodebot/prompts.py` & `aicodebot-0.8.5/aicodebot/prompts.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from aicodebot.helpers import get_token_length, logger, read_config
+from aicodebot.helpers import generate_directory_structure, get_token_length, logger, read_config
 from langchain import PromptTemplate
 from pathlib import Path
 from types import SimpleNamespace
 import os
 
 # ---------------------------------------------------------------------------- #
 #                              Personality helpers                             #
@@ -88,16 +88,26 @@
 Human: {task}
 AICodeBot:
 """
 )
 
 
 def generate_files_context(files):
-    """Generate the files context for the sidekick prompt."""
-    files_context = "Here are the relevant files we are working with in this session:\n"
+    """Generate the files context for the sidekick prompt.
+
+    This includes a directory structure and the contents of $files
+
+    """
+    files_context = "\nHere is the directory structure we are working with in this session:\n"
+    files_context += generate_directory_structure(".", ignore_patterns=[".git"], use_gitignore=True)
+
+    if not files:
+        return files_context
+
+    files_context += "Here are the relevant files we are working with in this session:\n"
     for file_name in files:
         contents = Path(file_name).read_text()
         token_length = get_token_length(contents)
         if token_length > 2_000:
             logger.warning(f"File {file_name} is large, using {token_length} tokens")
         else:
             logger.debug(f"File {file_name} is {token_length} tokens")
@@ -108,17 +118,15 @@
 
 
 # ---------------------------------------------------------------------------- #
 #                                 Other prompts                                #
 # ---------------------------------------------------------------------------- #
 
 ALIGNMENT_TEMPLATE = (
-    """
-    You're an advocate for aligned AI.
-    """
+    """You're an advocate for aligned AI."""
     + get_personality_prompt()
     + """
     You don't subscribe to the idea that AI is a black box or follow the
     Hollywood narrative of AI.
     You believe that AI should be explainable, fair, and full of heart-centered empathy.
     You're a champion for AI ethics and you're not afraid to speak up when
     you see something that's not right.
```

### Comparing `aicodebot-0.8.4/aicodebot.egg-info/PKG-INFO` & `aicodebot-0.8.5/aicodebot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.8.4
+Version: 0.8.5
 Summary: Your AI-powered coding sidekick 🤖
 Home-page: https://github.com/gorillamania/AICodeBot
 Author: Nick Sullivan
 Keywords: AI,coding,assistant,pair-programming,automation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `aicodebot-0.8.4/pyproject.toml` & `aicodebot-0.8.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.8.4/setup.py` & `aicodebot-0.8.5/setup.py`

 * *Files identical despite different names*

