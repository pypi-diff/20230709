# Comparing `tmp/gpt-command-line-0.1.0.tar.gz` & `tmp/gpt-command-line-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-command-line-0.1.0.tar", last modified: Sun Jul  9 20:07:28 2023, max compression
+gzip compressed data, was "gpt-command-line-0.1.1.tar", last modified: Sun Jul  9 20:13:33 2023, max compression
```

## Comparing `gpt-command-line-0.1.0.tar` & `gpt-command-line-0.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 demihalf   (501) staff       (20)        0 2023-07-09 20:07:28.942861 gpt-command-line-0.1.0/
--rw-r--r--   0 demihalf   (501) staff       (20)     1069 2023-03-12 03:56:07.000000 gpt-command-line-0.1.0/LICENSE
--rw-r--r--   0 demihalf   (501) staff       (20)     9979 2023-07-09 20:07:28.942687 gpt-command-line-0.1.0/PKG-INFO
--rw-r--r--   0 demihalf   (501) staff       (20)     8023 2023-07-09 19:49:10.000000 gpt-command-line-0.1.0/README.md
-drwxr-xr-x   0 demihalf   (501) staff       (20)        0 2023-07-09 20:07:28.938839 gpt-command-line-0.1.0/gpt_command_line.egg-info/
--rw-r--r--   0 demihalf   (501) staff       (20)     9979 2023-07-09 20:07:28.000000 gpt-command-line-0.1.0/gpt_command_line.egg-info/PKG-INFO
--rw-r--r--   0 demihalf   (501) staff       (20)      607 2023-07-09 20:07:28.000000 gpt-command-line-0.1.0/gpt_command_line.egg-info/SOURCES.txt
--rw-r--r--   0 demihalf   (501) staff       (20)        1 2023-07-09 20:07:28.000000 gpt-command-line-0.1.0/gpt_command_line.egg-info/dependency_links.txt
--rw-r--r--   0 demihalf   (501) staff       (20)       40 2023-07-09 20:07:28.000000 gpt-command-line-0.1.0/gpt_command_line.egg-info/entry_points.txt
--rw-r--r--   0 demihalf   (501) staff       (20)      229 2023-07-09 20:07:28.000000 gpt-command-line-0.1.0/gpt_command_line.egg-info/requires.txt
--rw-r--r--   0 demihalf   (501) staff       (20)        7 2023-07-09 20:07:28.000000 gpt-command-line-0.1.0/gpt_command_line.egg-info/top_level.txt
-drwxr-xr-x   0 demihalf   (501) staff       (20)        0 2023-07-09 20:07:28.941691 gpt-command-line-0.1.0/gptcli/
--rw-r--r--   0 demihalf   (501) staff       (20)        0 2023-03-23 04:43:55.000000 gpt-command-line-0.1.0/gptcli/__init__.py
--rw-r--r--   0 demihalf   (501) staff       (20)     2024 2023-07-09 18:14:55.000000 gpt-command-line-0.1.0/gptcli/anthropic.py
--rw-r--r--   0 demihalf   (501) staff       (20)     4964 2023-07-09 18:14:55.000000 gpt-command-line-0.1.0/gptcli/assistant.py
--rw-r--r--   0 demihalf   (501) staff       (20)     6263 2023-07-09 18:14:55.000000 gpt-command-line-0.1.0/gptcli/cli.py
--rw-r--r--   0 demihalf   (501) staff       (20)      413 2023-07-09 18:14:55.000000 gpt-command-line-0.1.0/gptcli/completion.py
--rw-r--r--   0 demihalf   (501) staff       (20)     1770 2023-07-09 18:14:55.000000 gpt-command-line-0.1.0/gptcli/composite.py
--rw-r--r--   0 demihalf   (501) staff       (20)     1296 2023-07-09 18:14:55.000000 gpt-command-line-0.1.0/gptcli/config.py
--rw-r--r--   0 demihalf   (501) staff       (20)     4885 2023-06-22 00:36:38.000000 gpt-command-line-0.1.0/gptcli/cost.py
--rw-r--r--   0 demihalf   (501) staff       (20)     1258 2023-07-09 18:14:55.000000 gpt-command-line-0.1.0/gptcli/google.py
--rwxr-xr-x   0 demihalf   (501) staff       (20)     7802 2023-07-09 19:19:09.000000 gpt-command-line-0.1.0/gptcli/gpt.py
--rw-r--r--   0 demihalf   (501) staff       (20)     3573 2023-07-09 20:07:11.000000 gpt-command-line-0.1.0/gptcli/llama.py
--rw-r--r--   0 demihalf   (501) staff       (20)      693 2023-07-09 18:14:55.000000 gpt-command-line-0.1.0/gptcli/logging.py
--rw-r--r--   0 demihalf   (501) staff       (20)     1984 2023-07-09 18:14:55.000000 gpt-command-line-0.1.0/gptcli/openai.py
--rw-r--r--   0 demihalf   (501) staff       (20)     5117 2023-07-09 18:14:55.000000 gpt-command-line-0.1.0/gptcli/session.py
--rw-r--r--   0 demihalf   (501) staff       (20)     1735 2023-07-09 18:14:55.000000 gpt-command-line-0.1.0/gptcli/shell.py
--rw-r--r--   0 demihalf   (501) staff       (20)     1375 2023-07-09 20:05:36.000000 gpt-command-line-0.1.0/pyproject.toml
--rw-r--r--   0 demihalf   (501) staff       (20)       38 2023-07-09 20:07:28.942901 gpt-command-line-0.1.0/setup.cfg
-drwxr-xr-x   0 demihalf   (501) staff       (20)        0 2023-07-09 20:07:28.942371 gpt-command-line-0.1.0/tests/
--rw-r--r--   0 demihalf   (501) staff       (20)     2120 2023-03-29 03:19:37.000000 gpt-command-line-0.1.0/tests/test_assistant.py
--rw-r--r--   0 demihalf   (501) staff       (20)     9105 2023-04-01 18:58:54.000000 gpt-command-line-0.1.0/tests/test_session.py
--rw-r--r--   0 demihalf   (501) staff       (20)      551 2023-05-08 02:55:30.000000 gpt-command-line-0.1.0/tests/test_term_utils.py
+drwxr-xr-x   0 demihalf   (501) staff       (20)        0 2023-07-09 20:13:33.982444 gpt-command-line-0.1.1/
+-rw-r--r--   0 demihalf   (501) staff       (20)     1069 2023-03-12 03:56:07.000000 gpt-command-line-0.1.1/LICENSE
+-rw-r--r--   0 demihalf   (501) staff       (20)    10120 2023-07-09 20:13:33.982261 gpt-command-line-0.1.1/PKG-INFO
+-rw-r--r--   0 demihalf   (501) staff       (20)     8164 2023-07-09 20:12:31.000000 gpt-command-line-0.1.1/README.md
+drwxr-xr-x   0 demihalf   (501) staff       (20)        0 2023-07-09 20:13:33.978406 gpt-command-line-0.1.1/gpt_command_line.egg-info/
+-rw-r--r--   0 demihalf   (501) staff       (20)    10120 2023-07-09 20:13:33.000000 gpt-command-line-0.1.1/gpt_command_line.egg-info/PKG-INFO
+-rw-r--r--   0 demihalf   (501) staff       (20)      607 2023-07-09 20:13:33.000000 gpt-command-line-0.1.1/gpt_command_line.egg-info/SOURCES.txt
+-rw-r--r--   0 demihalf   (501) staff       (20)        1 2023-07-09 20:13:33.000000 gpt-command-line-0.1.1/gpt_command_line.egg-info/dependency_links.txt
+-rw-r--r--   0 demihalf   (501) staff       (20)       40 2023-07-09 20:13:33.000000 gpt-command-line-0.1.1/gpt_command_line.egg-info/entry_points.txt
+-rw-r--r--   0 demihalf   (501) staff       (20)      229 2023-07-09 20:13:33.000000 gpt-command-line-0.1.1/gpt_command_line.egg-info/requires.txt
+-rw-r--r--   0 demihalf   (501) staff       (20)        7 2023-07-09 20:13:33.000000 gpt-command-line-0.1.1/gpt_command_line.egg-info/top_level.txt
+drwxr-xr-x   0 demihalf   (501) staff       (20)        0 2023-07-09 20:13:33.981333 gpt-command-line-0.1.1/gptcli/
+-rw-r--r--   0 demihalf   (501) staff       (20)        0 2023-03-23 04:43:55.000000 gpt-command-line-0.1.1/gptcli/__init__.py
+-rw-r--r--   0 demihalf   (501) staff       (20)     2024 2023-07-09 18:14:55.000000 gpt-command-line-0.1.1/gptcli/anthropic.py
+-rw-r--r--   0 demihalf   (501) staff       (20)     4964 2023-07-09 18:14:55.000000 gpt-command-line-0.1.1/gptcli/assistant.py
+-rw-r--r--   0 demihalf   (501) staff       (20)     6263 2023-07-09 18:14:55.000000 gpt-command-line-0.1.1/gptcli/cli.py
+-rw-r--r--   0 demihalf   (501) staff       (20)      413 2023-07-09 18:14:55.000000 gpt-command-line-0.1.1/gptcli/completion.py
+-rw-r--r--   0 demihalf   (501) staff       (20)     1770 2023-07-09 18:14:55.000000 gpt-command-line-0.1.1/gptcli/composite.py
+-rw-r--r--   0 demihalf   (501) staff       (20)     1296 2023-07-09 18:14:55.000000 gpt-command-line-0.1.1/gptcli/config.py
+-rw-r--r--   0 demihalf   (501) staff       (20)     4885 2023-06-22 00:36:38.000000 gpt-command-line-0.1.1/gptcli/cost.py
+-rw-r--r--   0 demihalf   (501) staff       (20)     1258 2023-07-09 18:14:55.000000 gpt-command-line-0.1.1/gptcli/google.py
+-rwxr-xr-x   0 demihalf   (501) staff       (20)     7802 2023-07-09 20:10:39.000000 gpt-command-line-0.1.1/gptcli/gpt.py
+-rw-r--r--   0 demihalf   (501) staff       (20)     3573 2023-07-09 20:10:41.000000 gpt-command-line-0.1.1/gptcli/llama.py
+-rw-r--r--   0 demihalf   (501) staff       (20)      693 2023-07-09 18:14:55.000000 gpt-command-line-0.1.1/gptcli/logging.py
+-rw-r--r--   0 demihalf   (501) staff       (20)     1984 2023-07-09 18:14:55.000000 gpt-command-line-0.1.1/gptcli/openai.py
+-rw-r--r--   0 demihalf   (501) staff       (20)     5117 2023-07-09 18:14:55.000000 gpt-command-line-0.1.1/gptcli/session.py
+-rw-r--r--   0 demihalf   (501) staff       (20)     1735 2023-07-09 18:14:55.000000 gpt-command-line-0.1.1/gptcli/shell.py
+-rw-r--r--   0 demihalf   (501) staff       (20)     1375 2023-07-09 20:13:24.000000 gpt-command-line-0.1.1/pyproject.toml
+-rw-r--r--   0 demihalf   (501) staff       (20)       38 2023-07-09 20:13:33.982478 gpt-command-line-0.1.1/setup.cfg
+drwxr-xr-x   0 demihalf   (501) staff       (20)        0 2023-07-09 20:13:33.981972 gpt-command-line-0.1.1/tests/
+-rw-r--r--   0 demihalf   (501) staff       (20)     2120 2023-03-29 03:19:37.000000 gpt-command-line-0.1.1/tests/test_assistant.py
+-rw-r--r--   0 demihalf   (501) staff       (20)     9105 2023-04-01 18:58:54.000000 gpt-command-line-0.1.1/tests/test_session.py
+-rw-r--r--   0 demihalf   (501) staff       (20)      551 2023-05-08 02:55:30.000000 gpt-command-line-0.1.1/tests/test_term_utils.py
```

### Comparing `gpt-command-line-0.1.0/LICENSE` & `gpt-command-line-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.0/PKG-INFO` & `gpt-command-line-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-command-line
-Version: 0.1.0
+Version: 0.1.1
 Summary: Command-line interface for ChatGPT, Claude and Bard
 Author-email: Val Kharitonov <val@kharvd.com>
 License: Copyright (c) 2023 by Val Kharitonov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -25,15 +25,15 @@
 Provides-Extra: llama
 License-File: LICENSE
 
 # gpt-cli
 
 Command-line interface for ChatGPT Claude and Bard.
 
-![screenshot](./screenshot.png)
+![screenshot](https://github.com/kharvd/gpt-cli/assets/466920/ecbcccc4-7cfa-4c04-83c3-a822b6596f01)
 
 ## Features
 
 ### **Coming soon** - Code Interpreter support https://github.com/kharvd/gpt-cli/pull/37
 
 - **Command-Line Interface**: Interact with ChatGPT or Claude directly from your terminal.
 - **Model Customization**: Override the default model, temperature, and top_p values for each assistant, giving you fine-grained control over the AI's behavior.
@@ -43,15 +43,20 @@
 - **Markdown Support**: Enable or disable markdown formatting for chat sessions to tailor the output to your preferences.
 - **Predefined Messages**: Set up predefined messages for your custom assistants to establish context or role-play scenarios.
 - **Multiple Assistants**: Easily switch between different assistants, including general, dev, and custom assistants defined in the config file.
 - **Flexible Configuration**: Define your assistants, model parameters, and API key in a YAML configuration file, allowing for easy customization and management.
 
 ## Installation
 
-This install assumes a Linux/OSX machine with Git, Python and pip available.
+This install assumes a Linux/OSX machine with Python and pip available.
+```bash
+pip install gpt-command-line
+```
+
+Install latest version from source:
 ```bash
 pip install git+https://github.com/kharvd/gpt-cli.git
 ```
 
 Or install by cloning the repository manually:
 ```bash
 git clone https://github.com/kharvd/gpt-cli.git
```

### Comparing `gpt-command-line-0.1.0/README.md` & `gpt-command-line-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # gpt-cli
 
 Command-line interface for ChatGPT Claude and Bard.
 
-![screenshot](./screenshot.png)
+![screenshot](https://github.com/kharvd/gpt-cli/assets/466920/ecbcccc4-7cfa-4c04-83c3-a822b6596f01)
 
 ## Features
 
 ### **Coming soon** - Code Interpreter support https://github.com/kharvd/gpt-cli/pull/37
 
 - **Command-Line Interface**: Interact with ChatGPT or Claude directly from your terminal.
 - **Model Customization**: Override the default model, temperature, and top_p values for each assistant, giving you fine-grained control over the AI's behavior.
@@ -16,15 +16,20 @@
 - **Markdown Support**: Enable or disable markdown formatting for chat sessions to tailor the output to your preferences.
 - **Predefined Messages**: Set up predefined messages for your custom assistants to establish context or role-play scenarios.
 - **Multiple Assistants**: Easily switch between different assistants, including general, dev, and custom assistants defined in the config file.
 - **Flexible Configuration**: Define your assistants, model parameters, and API key in a YAML configuration file, allowing for easy customization and management.
 
 ## Installation
 
-This install assumes a Linux/OSX machine with Git, Python and pip available.
+This install assumes a Linux/OSX machine with Python and pip available.
+```bash
+pip install gpt-command-line
+```
+
+Install latest version from source:
 ```bash
 pip install git+https://github.com/kharvd/gpt-cli.git
 ```
 
 Or install by cloning the repository manually:
 ```bash
 git clone https://github.com/kharvd/gpt-cli.git
```

### Comparing `gpt-command-line-0.1.0/gpt_command_line.egg-info/PKG-INFO` & `gpt-command-line-0.1.1/gpt_command_line.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-command-line
-Version: 0.1.0
+Version: 0.1.1
 Summary: Command-line interface for ChatGPT, Claude and Bard
 Author-email: Val Kharitonov <val@kharvd.com>
 License: Copyright (c) 2023 by Val Kharitonov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -25,15 +25,15 @@
 Provides-Extra: llama
 License-File: LICENSE
 
 # gpt-cli
 
 Command-line interface for ChatGPT Claude and Bard.
 
-![screenshot](./screenshot.png)
+![screenshot](https://github.com/kharvd/gpt-cli/assets/466920/ecbcccc4-7cfa-4c04-83c3-a822b6596f01)
 
 ## Features
 
 ### **Coming soon** - Code Interpreter support https://github.com/kharvd/gpt-cli/pull/37
 
 - **Command-Line Interface**: Interact with ChatGPT or Claude directly from your terminal.
 - **Model Customization**: Override the default model, temperature, and top_p values for each assistant, giving you fine-grained control over the AI's behavior.
@@ -43,15 +43,20 @@
 - **Markdown Support**: Enable or disable markdown formatting for chat sessions to tailor the output to your preferences.
 - **Predefined Messages**: Set up predefined messages for your custom assistants to establish context or role-play scenarios.
 - **Multiple Assistants**: Easily switch between different assistants, including general, dev, and custom assistants defined in the config file.
 - **Flexible Configuration**: Define your assistants, model parameters, and API key in a YAML configuration file, allowing for easy customization and management.
 
 ## Installation
 
-This install assumes a Linux/OSX machine with Git, Python and pip available.
+This install assumes a Linux/OSX machine with Python and pip available.
+```bash
+pip install gpt-command-line
+```
+
+Install latest version from source:
 ```bash
 pip install git+https://github.com/kharvd/gpt-cli.git
 ```
 
 Or install by cloning the repository manually:
 ```bash
 git clone https://github.com/kharvd/gpt-cli.git
```

### Comparing `gpt-command-line-0.1.0/gpt_command_line.egg-info/SOURCES.txt` & `gpt-command-line-0.1.1/gpt_command_line.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.0/gptcli/anthropic.py` & `gpt-command-line-0.1.1/gptcli/anthropic.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.0/gptcli/assistant.py` & `gpt-command-line-0.1.1/gptcli/assistant.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.0/gptcli/cli.py` & `gpt-command-line-0.1.1/gptcli/cli.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.0/gptcli/composite.py` & `gpt-command-line-0.1.1/gptcli/composite.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.0/gptcli/config.py` & `gpt-command-line-0.1.1/gptcli/config.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.0/gptcli/cost.py` & `gpt-command-line-0.1.1/gptcli/cost.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.0/gptcli/google.py` & `gpt-command-line-0.1.1/gptcli/google.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.0/gptcli/gpt.py` & `gpt-command-line-0.1.1/gptcli/gpt.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.0/gptcli/llama.py` & `gpt-command-line-0.1.1/gptcli/llama.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.0/gptcli/logging.py` & `gpt-command-line-0.1.1/gptcli/logging.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.0/gptcli/openai.py` & `gpt-command-line-0.1.1/gptcli/openai.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.0/gptcli/session.py` & `gpt-command-line-0.1.1/gptcli/session.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.0/gptcli/shell.py` & `gpt-command-line-0.1.1/gptcli/shell.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.0/pyproject.toml` & `gpt-command-line-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gpt-command-line"
-version = "0.1.0"
+version = "0.1.1"
 description = "Command-line interface for ChatGPT, Claude and Bard"
 authors = [{name = "Val Kharitonov", email = "val@kharvd.com"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.9"
 keywords = ["cli", "command-line", "assistant", "openai", "claude", "bard", "gpt-3", "gpt-4", "llm", "chatgpt", "gpt-cli", "google-bard", "anthropic", "gpt-client", "anthropic-claude", "palm2"]
 classifiers = [
```

### Comparing `gpt-command-line-0.1.0/tests/test_assistant.py` & `gpt-command-line-0.1.1/tests/test_assistant.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.0/tests/test_session.py` & `gpt-command-line-0.1.1/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.0/tests/test_term_utils.py` & `gpt-command-line-0.1.1/tests/test_term_utils.py`

 * *Files identical despite different names*

