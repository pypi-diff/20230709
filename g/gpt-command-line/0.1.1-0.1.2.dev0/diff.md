# Comparing `tmp/gpt-command-line-0.1.1.tar.gz` & `tmp/gpt-command-line-0.1.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-command-line-0.1.1.tar", last modified: Sun Jul  9 20:13:33 2023, max compression
+gzip compressed data, was "gpt-command-line-0.1.2.dev0.tar", last modified: Sun Jul  9 20:41:39 2023, max compression
```

## Comparing `gpt-command-line-0.1.1.tar` & `gpt-command-line-0.1.2.dev0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 demihalf   (501) staff       (20)        0 2023-07-09 20:13:33.982444 gpt-command-line-0.1.1/
--rw-r--r--   0 demihalf   (501) staff       (20)     1069 2023-03-12 03:56:07.000000 gpt-command-line-0.1.1/LICENSE
--rw-r--r--   0 demihalf   (501) staff       (20)    10120 2023-07-09 20:13:33.982261 gpt-command-line-0.1.1/PKG-INFO
--rw-r--r--   0 demihalf   (501) staff       (20)     8164 2023-07-09 20:12:31.000000 gpt-command-line-0.1.1/README.md
-drwxr-xr-x   0 demihalf   (501) staff       (20)        0 2023-07-09 20:13:33.978406 gpt-command-line-0.1.1/gpt_command_line.egg-info/
--rw-r--r--   0 demihalf   (501) staff       (20)    10120 2023-07-09 20:13:33.000000 gpt-command-line-0.1.1/gpt_command_line.egg-info/PKG-INFO
--rw-r--r--   0 demihalf   (501) staff       (20)      607 2023-07-09 20:13:33.000000 gpt-command-line-0.1.1/gpt_command_line.egg-info/SOURCES.txt
--rw-r--r--   0 demihalf   (501) staff       (20)        1 2023-07-09 20:13:33.000000 gpt-command-line-0.1.1/gpt_command_line.egg-info/dependency_links.txt
--rw-r--r--   0 demihalf   (501) staff       (20)       40 2023-07-09 20:13:33.000000 gpt-command-line-0.1.1/gpt_command_line.egg-info/entry_points.txt
--rw-r--r--   0 demihalf   (501) staff       (20)      229 2023-07-09 20:13:33.000000 gpt-command-line-0.1.1/gpt_command_line.egg-info/requires.txt
--rw-r--r--   0 demihalf   (501) staff       (20)        7 2023-07-09 20:13:33.000000 gpt-command-line-0.1.1/gpt_command_line.egg-info/top_level.txt
-drwxr-xr-x   0 demihalf   (501) staff       (20)        0 2023-07-09 20:13:33.981333 gpt-command-line-0.1.1/gptcli/
--rw-r--r--   0 demihalf   (501) staff       (20)        0 2023-03-23 04:43:55.000000 gpt-command-line-0.1.1/gptcli/__init__.py
--rw-r--r--   0 demihalf   (501) staff       (20)     2024 2023-07-09 18:14:55.000000 gpt-command-line-0.1.1/gptcli/anthropic.py
--rw-r--r--   0 demihalf   (501) staff       (20)     4964 2023-07-09 18:14:55.000000 gpt-command-line-0.1.1/gptcli/assistant.py
--rw-r--r--   0 demihalf   (501) staff       (20)     6263 2023-07-09 18:14:55.000000 gpt-command-line-0.1.1/gptcli/cli.py
--rw-r--r--   0 demihalf   (501) staff       (20)      413 2023-07-09 18:14:55.000000 gpt-command-line-0.1.1/gptcli/completion.py
--rw-r--r--   0 demihalf   (501) staff       (20)     1770 2023-07-09 18:14:55.000000 gpt-command-line-0.1.1/gptcli/composite.py
--rw-r--r--   0 demihalf   (501) staff       (20)     1296 2023-07-09 18:14:55.000000 gpt-command-line-0.1.1/gptcli/config.py
--rw-r--r--   0 demihalf   (501) staff       (20)     4885 2023-06-22 00:36:38.000000 gpt-command-line-0.1.1/gptcli/cost.py
--rw-r--r--   0 demihalf   (501) staff       (20)     1258 2023-07-09 18:14:55.000000 gpt-command-line-0.1.1/gptcli/google.py
--rwxr-xr-x   0 demihalf   (501) staff       (20)     7802 2023-07-09 20:10:39.000000 gpt-command-line-0.1.1/gptcli/gpt.py
--rw-r--r--   0 demihalf   (501) staff       (20)     3573 2023-07-09 20:10:41.000000 gpt-command-line-0.1.1/gptcli/llama.py
--rw-r--r--   0 demihalf   (501) staff       (20)      693 2023-07-09 18:14:55.000000 gpt-command-line-0.1.1/gptcli/logging.py
--rw-r--r--   0 demihalf   (501) staff       (20)     1984 2023-07-09 18:14:55.000000 gpt-command-line-0.1.1/gptcli/openai.py
--rw-r--r--   0 demihalf   (501) staff       (20)     5117 2023-07-09 18:14:55.000000 gpt-command-line-0.1.1/gptcli/session.py
--rw-r--r--   0 demihalf   (501) staff       (20)     1735 2023-07-09 18:14:55.000000 gpt-command-line-0.1.1/gptcli/shell.py
--rw-r--r--   0 demihalf   (501) staff       (20)     1375 2023-07-09 20:13:24.000000 gpt-command-line-0.1.1/pyproject.toml
--rw-r--r--   0 demihalf   (501) staff       (20)       38 2023-07-09 20:13:33.982478 gpt-command-line-0.1.1/setup.cfg
-drwxr-xr-x   0 demihalf   (501) staff       (20)        0 2023-07-09 20:13:33.981972 gpt-command-line-0.1.1/tests/
--rw-r--r--   0 demihalf   (501) staff       (20)     2120 2023-03-29 03:19:37.000000 gpt-command-line-0.1.1/tests/test_assistant.py
--rw-r--r--   0 demihalf   (501) staff       (20)     9105 2023-04-01 18:58:54.000000 gpt-command-line-0.1.1/tests/test_session.py
--rw-r--r--   0 demihalf   (501) staff       (20)      551 2023-05-08 02:55:30.000000 gpt-command-line-0.1.1/tests/test_term_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:39.726502 gpt-command-line-0.1.2.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10125 2023-07-09 20:41:39.726502 gpt-command-line-0.1.2.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:39.722502 gpt-command-line-0.1.2.dev0/gpt_command_line.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10125 2023-07-09 20:41:39.000000 gpt-command-line-0.1.2.dev0/gpt_command_line.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-09 20:41:39.000000 gpt-command-line-0.1.2.dev0/gpt_command_line.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 20:41:39.000000 gpt-command-line-0.1.2.dev0/gpt_command_line.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-09 20:41:39.000000 gpt-command-line-0.1.2.dev0/gpt_command_line.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-09 20:41:39.000000 gpt-command-line-0.1.2.dev0/gpt_command_line.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-09 20:41:39.000000 gpt-command-line-0.1.2.dev0/gpt_command_line.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:39.726502 gpt-command-line-0.1.2.dev0/gptcli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/gptcli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/gptcli/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/gptcli/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/gptcli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/gptcli/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/gptcli/composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/gptcli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/gptcli/cost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/gptcli/google.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7802 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/gptcli/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/gptcli/llama.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/gptcli/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/gptcli/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/gptcli/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/gptcli/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 20:41:39.726502 gpt-command-line-0.1.2.dev0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:39.726502 gpt-command-line-0.1.2.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/tests/test_assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/tests/test_term_utils.py
```

### Comparing `gpt-command-line-0.1.1/LICENSE` & `gpt-command-line-0.1.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.1/PKG-INFO` & `gpt-command-line-0.1.2.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-command-line
-Version: 0.1.1
+Version: 0.1.2.dev0
 Summary: Command-line interface for ChatGPT, Claude and Bard
 Author-email: Val Kharitonov <val@kharvd.com>
 License: Copyright (c) 2023 by Val Kharitonov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `gpt-command-line-0.1.1/README.md` & `gpt-command-line-0.1.2.dev0/README.md`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.1/gpt_command_line.egg-info/PKG-INFO` & `gpt-command-line-0.1.2.dev0/gpt_command_line.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-command-line
-Version: 0.1.1
+Version: 0.1.2.dev0
 Summary: Command-line interface for ChatGPT, Claude and Bard
 Author-email: Val Kharitonov <val@kharvd.com>
 License: Copyright (c) 2023 by Val Kharitonov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `gpt-command-line-0.1.1/gpt_command_line.egg-info/SOURCES.txt` & `gpt-command-line-0.1.2.dev0/gpt_command_line.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.1/gptcli/anthropic.py` & `gpt-command-line-0.1.2.dev0/gptcli/anthropic.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.1/gptcli/assistant.py` & `gpt-command-line-0.1.2.dev0/gptcli/assistant.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.1/gptcli/cli.py` & `gpt-command-line-0.1.2.dev0/gptcli/cli.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.1/gptcli/composite.py` & `gpt-command-line-0.1.2.dev0/gptcli/composite.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.1/gptcli/config.py` & `gpt-command-line-0.1.2.dev0/gptcli/config.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.1/gptcli/cost.py` & `gpt-command-line-0.1.2.dev0/gptcli/cost.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.1/gptcli/google.py` & `gpt-command-line-0.1.2.dev0/gptcli/google.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.1/gptcli/gpt.py` & `gpt-command-line-0.1.2.dev0/gptcli/gpt.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.1/gptcli/llama.py` & `gpt-command-line-0.1.2.dev0/gptcli/llama.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.1/gptcli/logging.py` & `gpt-command-line-0.1.2.dev0/gptcli/logging.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.1/gptcli/openai.py` & `gpt-command-line-0.1.2.dev0/gptcli/openai.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.1/gptcli/session.py` & `gpt-command-line-0.1.2.dev0/gptcli/session.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.1/gptcli/shell.py` & `gpt-command-line-0.1.2.dev0/gptcli/shell.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.1/pyproject.toml` & `gpt-command-line-0.1.2.dev0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gpt-command-line"
-version = "0.1.1"
+version = "0.1.2.dev0"
 description = "Command-line interface for ChatGPT, Claude and Bard"
 authors = [{name = "Val Kharitonov", email = "val@kharvd.com"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.9"
 keywords = ["cli", "command-line", "assistant", "openai", "claude", "bard", "gpt-3", "gpt-4", "llm", "chatgpt", "gpt-cli", "google-bard", "anthropic", "gpt-client", "anthropic-claude", "palm2"]
 classifiers = [
```

### Comparing `gpt-command-line-0.1.1/tests/test_assistant.py` & `gpt-command-line-0.1.2.dev0/tests/test_assistant.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.1/tests/test_session.py` & `gpt-command-line-0.1.2.dev0/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.1/tests/test_term_utils.py` & `gpt-command-line-0.1.2.dev0/tests/test_term_utils.py`

 * *Files identical despite different names*

