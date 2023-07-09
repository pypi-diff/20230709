# Comparing `tmp/actionai-0.0.3.tar.gz` & `tmp/actionai-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "actionai-0.0.3.tar", max compression
+gzip compressed data, was "actionai-0.0.4.tar", max compression
```

## Comparing `actionai-0.0.3.tar` & `actionai-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1067 2023-07-08 15:41:43.483740 actionai-0.0.3/LICENSE
--rw-r--r--   0        0        0     1623 2023-07-08 16:57:44.038115 actionai-0.0.3/README.md
--rw-r--r--   0        0        0      536 2023-07-08 16:59:30.685499 actionai-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3176 2023-07-08 16:57:44.038797 actionai-0.0.3/src/actionai/__init__.py
--rw-r--r--   0        0        0      910 2023-07-08 16:57:44.039116 actionai-0.0.3/src/actionai/json_schema.py
--rw-r--r--   0        0        0      906 2023-07-08 16:57:44.039563 actionai-0.0.3/src/actionai/types.py
--rw-r--r--   0        0        0     2431 1970-01-01 00:00:00.000000 actionai-0.0.3/setup.py
--rw-r--r--   0        0        0     2060 1970-01-01 00:00:00.000000 actionai-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-08 15:41:43.483740 actionai-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2152 2023-07-09 15:29:10.860733 actionai-0.0.4/README.md
+-rw-r--r--   0        0        0      594 2023-07-09 15:30:56.251362 actionai-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3798 2023-07-09 15:29:10.861088 actionai-0.0.4/src/actionai/__init__.py
+-rw-r--r--   0        0        0       45 2023-07-09 14:31:10.412650 actionai-0.0.4/src/actionai/exceptions.py
+-rw-r--r--   0        0        0     1269 2023-07-09 14:31:10.412909 actionai-0.0.4/src/actionai/json_schema.py
+-rw-r--r--   0        0        0     1116 2023-07-09 15:29:10.861426 actionai-0.0.4/src/actionai/types.py
+-rw-r--r--   0        0        0     2979 1970-01-01 00:00:00.000000 actionai-0.0.4/setup.py
+-rw-r--r--   0        0        0     2589 1970-01-01 00:00:00.000000 actionai-0.0.4/PKG-INFO
```

### Comparing `actionai-0.0.3/LICENSE` & `actionai-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `actionai-0.0.3/README.md` & `actionai-0.0.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 pip install actionai
 ```
 
 ## Usage
 
 ```python
 # define a new function
-# example from openai functions examples
 def get_current_weather(location: str, unit: str = "fahrenheit"):
     """Function to get current weather for the given location"""
     weather_info = {
         "location": location,
         "temperature": "72",
         "unit": unit,
         "forecast": ["sunny", "windy"],
@@ -31,14 +30,22 @@
 
 response = action.prompt("What is the current weather in the north pole?")
 
 print(response["choices"][0]["message"]["content"])
 # The current weather at the North Pole is 72°F. It is sunny and windy.
 ```
 
+The openai api key will be read automatically from the `OPENAI_API_KEY` environment variable. You can pass it manually as,
+
+```python
+import actionai
+
+action = actionai.ActionAI(openai_api_key="YOUR_KEY")
+```
+
 ### Adding context
 
 Sometimes your function will have variables that needs to be set by the program.
 
 ```python
 def list_todos(user: str):
     """Function to list all todos"""
@@ -48,14 +55,26 @@
 ```
 
 The context keys are skipped when creating json schema. The values are directly passed at the time of function calling.
 
 > **Warning**
 > A function must be fully typed and must have a docstring(one liner explanation of the function is enough)
 
+### Choosing a model
+
+By default, the completion run on the `gpt-3.5-turbo-0613` model. You can change the model using the `model` argument.
+
+```python
+import actionai
+
+action = actionai.ActionAI(model="gpt-4")
+```
+
+You can see the complete list of supported chat completion models [here](https://platform.openai.com/docs/models/model-endpoint-compatibility)
+
 ## Demo
 
 Running [todo example](https://github.com/amalshaji/actionai/blob/main/examples/todo.py) 👇🏻
 
 ![todo demo](https://raw.githubusercontent.com/amalshaji/actionai/main/examples/demo.svg)
 
 For more examples, checkout the [examples](https://github.com/amalshaji/actionai/tree/main/examples) directory.
```

### Comparing `actionai-0.0.3/pyproject.toml` & `actionai-0.0.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "actionai"
-version = "0.0.3"
+version = "0.0.4"
 description = "A small library to call local functions using openai function calling"
 authors = ["Amal Shaji <amalshajid@gmail.com>"]
 readme = "README.md"
 packages = [{include = "actionai", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -14,10 +14,14 @@
 
 [tool.poetry.group.cq.dependencies]
 black = "^23.3.0"
 mypy = "^1.4.1"
 pre-commit = "^3.3.3"
 ruff = "^0.0.277"
 
+
+[tool.poetry.group.test.dependencies]
+pytest = "^7.4.0"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `actionai-0.0.3/src/actionai/__init__.py` & `actionai-0.0.4/src/actionai/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import json
 from typing import Any, Callable, cast
 
 import openai
 from attr import dataclass
 
+from actionai.exceptions import ActionAIException
 from actionai.json_schema import create_json_schema_for_function_input
-from actionai.types import ChatResponse, ChatResponseMessage, Message, OpenAIFunction
-
-
-class ActionAIException(Exception):
-    pass
+from actionai.types import (
+    OPENAI_MODELS,
+    ChatResponse,
+    ChatResponseMessage,
+    Message,
+    OpenAIFunction,
+)
 
 
 @dataclass
 class ActionAIFunction:
     fn: Callable
     name: str
     description: str
@@ -21,22 +24,36 @@
 
 
 class ActionAI:
     def __init__(
         self,
         openai_api_key: str | None = None,
         context: dict[str, Any] | None = None,
+        model: OPENAI_MODELS = "gpt-3.5-turbo-0613",
     ) -> None:
+        """
+        Args:
+            openai_api_key (str | None, optional): If not set, defaults \
+                to `OPENAI_API_KEY` environment variable.
+
+            context (dict[str, Any] | None, optional): These keys will be skipped \
+                when creating json schema for the function's input. The values \
+                    will be directly passed during function call.
+
+            model (optional): The chat completion model to use. Defaults to \
+                "gpt-3.5-turbo-0613".
+        """
         if openai_api_key is not None:
             openai.api_key = openai_api_key
 
         self.functions: dict[str, ActionAIFunction] = {}
         self.messages: list[Message | ChatResponseMessage] = []
         self.openai_functions: list[OpenAIFunction] = []
         self.context = context or {}
+        self.model = model
 
     def register(self, fn: Callable):
         if fn.__name__ in self.functions:
             raise ActionAIException("function with the same name already registered")
 
         if fn.__doc__ is None:
             raise ActionAIException("function must have a docstring")
@@ -64,15 +81,15 @@
             )
 
     def prompt(self, query: str) -> ChatResponse:
         self._set_openai_functions()
         self.messages.append({"role": "user", "content": query})
 
         response = openai.ChatCompletion.create(
-            model="gpt-3.5-turbo-0613",
+            model=self.model,
             messages=self.messages,
             functions=self.openai_functions,
             function_call="auto",
         )
 
         response = cast(ChatResponse, response)
 
@@ -91,12 +108,12 @@
             {
                 "role": "function",
                 "name": function_name,
                 "content": json.dumps(function_response, default=str),
             }
         )
         second_response = openai.ChatCompletion.create(
-            model="gpt-3.5-turbo-0613",
+            model=self.model,
             messages=self.messages,
         )
         second_response = cast(ChatResponse, second_response)
         return second_response
```

### Comparing `actionai-0.0.3/setup.py` & `actionai-0.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 {'': ['*']}
 
 install_requires = \
 ['openai>=0.27.8,<0.28.0', 'pydantic>=2.0.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'actionai',
-    'version': '0.0.3',
+    'version': '0.0.4',
     'description': 'A small library to call local functions using openai function calling',
-    'long_description': '# ActionAI\n\nA small library to run local functions using openai function calling\n\n## Install\n\n```shell\npip install actionai\n```\n\n## Usage\n\n```python\n# define a new function\n# example from openai functions examples\ndef get_current_weather(location: str, unit: str = "fahrenheit"):\n    """Function to get current weather for the given location"""\n    weather_info = {\n        "location": location,\n        "temperature": "72",\n        "unit": unit,\n        "forecast": ["sunny", "windy"],\n    }\n    return weather_info\n\n\nimport actionai\n\naction = actionai.ActionAI()\naction.register(get_current_weather)\n\nresponse = action.prompt("What is the current weather in the north pole?")\n\nprint(response["choices"][0]["message"]["content"])\n# The current weather at the North Pole is 72°F. It is sunny and windy.\n```\n\n### Adding context\n\nSometimes your function will have variables that needs to be set by the program.\n\n```python\ndef list_todos(user: str):\n    """Function to list all todos"""\n    return todos[user]\n\naction = actionai.ActionAI(context={"user": "jason"})\n```\n\nThe context keys are skipped when creating json schema. The values are directly passed at the time of function calling.\n\n> **Warning**\n> A function must be fully typed and must have a docstring(one liner explanation of the function is enough)\n\n## Demo\n\nRunning [todo example](https://github.com/amalshaji/actionai/blob/main/examples/todo.py) 👇🏻\n\n![todo demo](https://raw.githubusercontent.com/amalshaji/actionai/main/examples/demo.svg)\n\nFor more examples, checkout the [examples](https://github.com/amalshaji/actionai/tree/main/examples) directory.\n',
+    'long_description': '# ActionAI\n\nA small library to run local functions using openai function calling\n\n## Install\n\n```shell\npip install actionai\n```\n\n## Usage\n\n```python\n# define a new function\ndef get_current_weather(location: str, unit: str = "fahrenheit"):\n    """Function to get current weather for the given location"""\n    weather_info = {\n        "location": location,\n        "temperature": "72",\n        "unit": unit,\n        "forecast": ["sunny", "windy"],\n    }\n    return weather_info\n\n\nimport actionai\n\naction = actionai.ActionAI()\naction.register(get_current_weather)\n\nresponse = action.prompt("What is the current weather in the north pole?")\n\nprint(response["choices"][0]["message"]["content"])\n# The current weather at the North Pole is 72°F. It is sunny and windy.\n```\n\nThe openai api key will be read automatically from the `OPENAI_API_KEY` environment variable. You can pass it manually as,\n\n```python\nimport actionai\n\naction = actionai.ActionAI(openai_api_key="YOUR_KEY")\n```\n\n### Adding context\n\nSometimes your function will have variables that needs to be set by the program.\n\n```python\ndef list_todos(user: str):\n    """Function to list all todos"""\n    return todos[user]\n\naction = actionai.ActionAI(context={"user": "jason"})\n```\n\nThe context keys are skipped when creating json schema. The values are directly passed at the time of function calling.\n\n> **Warning**\n> A function must be fully typed and must have a docstring(one liner explanation of the function is enough)\n\n### Choosing a model\n\nBy default, the completion run on the `gpt-3.5-turbo-0613` model. You can change the model using the `model` argument.\n\n```python\nimport actionai\n\naction = actionai.ActionAI(model="gpt-4")\n```\n\nYou can see the complete list of supported chat completion models [here](https://platform.openai.com/docs/models/model-endpoint-compatibility)\n\n## Demo\n\nRunning [todo example](https://github.com/amalshaji/actionai/blob/main/examples/todo.py) 👇🏻\n\n![todo demo](https://raw.githubusercontent.com/amalshaji/actionai/main/examples/demo.svg)\n\nFor more examples, checkout the [examples](https://github.com/amalshaji/actionai/tree/main/examples) directory.\n',
     'author': 'Amal Shaji',
     'author_email': 'amalshajid@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `actionai-0.0.3/PKG-INFO` & `actionai-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: actionai
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small library to call local functions using openai function calling
 Author: Amal Shaji
 Author-email: amalshajid@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: openai (>=0.27.8,<0.28.0)
@@ -21,15 +21,14 @@
 pip install actionai
 ```
 
 ## Usage
 
 ```python
 # define a new function
-# example from openai functions examples
 def get_current_weather(location: str, unit: str = "fahrenheit"):
     """Function to get current weather for the given location"""
     weather_info = {
         "location": location,
         "temperature": "72",
         "unit": unit,
         "forecast": ["sunny", "windy"],
@@ -44,14 +43,22 @@
 
 response = action.prompt("What is the current weather in the north pole?")
 
 print(response["choices"][0]["message"]["content"])
 # The current weather at the North Pole is 72°F. It is sunny and windy.
 ```
 
+The openai api key will be read automatically from the `OPENAI_API_KEY` environment variable. You can pass it manually as,
+
+```python
+import actionai
+
+action = actionai.ActionAI(openai_api_key="YOUR_KEY")
+```
+
 ### Adding context
 
 Sometimes your function will have variables that needs to be set by the program.
 
 ```python
 def list_todos(user: str):
     """Function to list all todos"""
@@ -61,14 +68,26 @@
 ```
 
 The context keys are skipped when creating json schema. The values are directly passed at the time of function calling.
 
 > **Warning**
 > A function must be fully typed and must have a docstring(one liner explanation of the function is enough)
 
+### Choosing a model
+
+By default, the completion run on the `gpt-3.5-turbo-0613` model. You can change the model using the `model` argument.
+
+```python
+import actionai
+
+action = actionai.ActionAI(model="gpt-4")
+```
+
+You can see the complete list of supported chat completion models [here](https://platform.openai.com/docs/models/model-endpoint-compatibility)
+
 ## Demo
 
 Running [todo example](https://github.com/amalshaji/actionai/blob/main/examples/todo.py) 👇🏻
 
 ![todo demo](https://raw.githubusercontent.com/amalshaji/actionai/main/examples/demo.svg)
 
 For more examples, checkout the [examples](https://github.com/amalshaji/actionai/tree/main/examples) directory.
```

