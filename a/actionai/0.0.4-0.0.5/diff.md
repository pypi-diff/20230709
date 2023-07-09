# Comparing `tmp/actionai-0.0.4.tar.gz` & `tmp/actionai-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "actionai-0.0.4.tar", max compression
+gzip compressed data, was "actionai-0.0.5.tar", max compression
```

## Comparing `actionai-0.0.4.tar` & `actionai-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1067 2023-07-08 15:41:43.483740 actionai-0.0.4/LICENSE
--rw-r--r--   0        0        0     2152 2023-07-09 15:29:10.860733 actionai-0.0.4/README.md
--rw-r--r--   0        0        0      594 2023-07-09 15:30:56.251362 actionai-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3798 2023-07-09 15:29:10.861088 actionai-0.0.4/src/actionai/__init__.py
--rw-r--r--   0        0        0       45 2023-07-09 14:31:10.412650 actionai-0.0.4/src/actionai/exceptions.py
--rw-r--r--   0        0        0     1269 2023-07-09 14:31:10.412909 actionai-0.0.4/src/actionai/json_schema.py
--rw-r--r--   0        0        0     1116 2023-07-09 15:29:10.861426 actionai-0.0.4/src/actionai/types.py
--rw-r--r--   0        0        0     2979 1970-01-01 00:00:00.000000 actionai-0.0.4/setup.py
--rw-r--r--   0        0        0     2589 1970-01-01 00:00:00.000000 actionai-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-08 15:41:43.483740 actionai-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2152 2023-07-09 15:29:10.860733 actionai-0.0.5/README.md
+-rw-r--r--   0        0        0      594 2023-07-09 16:47:48.056335 actionai-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3739 2023-07-09 16:47:48.056545 actionai-0.0.5/src/actionai/__init__.py
+-rw-r--r--   0        0        0       45 2023-07-09 14:31:10.412650 actionai-0.0.5/src/actionai/exceptions.py
+-rw-r--r--   0        0        0     1269 2023-07-09 14:31:10.412909 actionai-0.0.5/src/actionai/json_schema.py
+-rw-r--r--   0        0        0     1116 2023-07-09 15:29:10.861426 actionai-0.0.5/src/actionai/types.py
+-rw-r--r--   0        0        0     2979 1970-01-01 00:00:00.000000 actionai-0.0.5/setup.py
+-rw-r--r--   0        0        0     2589 1970-01-01 00:00:00.000000 actionai-0.0.5/PKG-INFO
```

### Comparing `actionai-0.0.4/LICENSE` & `actionai-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `actionai-0.0.4/README.md` & `actionai-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `actionai-0.0.4/pyproject.toml` & `actionai-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "actionai"
-version = "0.0.4"
+version = "0.0.5"
 description = "A small library to call local functions using openai function calling"
 authors = ["Amal Shaji <amalshajid@gmail.com>"]
 readme = "README.md"
 packages = [{include = "actionai", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `actionai-0.0.4/src/actionai/__init__.py` & `actionai-0.0.5/src/actionai/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
+from dataclasses import dataclass
 from typing import Any, Callable, cast
 
 import openai
-from attr import dataclass
 
 from actionai.exceptions import ActionAIException
 from actionai.json_schema import create_json_schema_for_function_input
 from actionai.types import (
     OPENAI_MODELS,
     ChatResponse,
     ChatResponseMessage,
@@ -18,14 +18,21 @@
 @dataclass
 class ActionAIFunction:
     fn: Callable
     name: str
     description: str
     input_schema: Any
 
+    def to_openai_function(self) -> OpenAIFunction:
+        return {
+            "name": self.name,
+            "description": self.description,
+            "parameters": self.input_schema,
+        }
+
 
 class ActionAI:
     def __init__(
         self,
         openai_api_key: str | None = None,
         context: dict[str, Any] | None = None,
         model: OPENAI_MODELS = "gpt-3.5-turbo-0613",
@@ -41,69 +48,59 @@
 
             model (optional): The chat completion model to use. Defaults to \
                 "gpt-3.5-turbo-0613".
         """
         if openai_api_key is not None:
             openai.api_key = openai_api_key
 
-        self.functions: dict[str, ActionAIFunction] = {}
         self.messages: list[Message | ChatResponseMessage] = []
-        self.openai_functions: list[OpenAIFunction] = []
         self.context = context or {}
         self.model = model
 
+        # Do not update these attributes directly
+        self._functions: dict[str, ActionAIFunction] = {}
+        self._openai_functions: list[OpenAIFunction] = []
+
     def register(self, fn: Callable):
-        if fn.__name__ in self.functions:
+        if fn.__name__ in self._functions:
             raise ActionAIException("function with the same name already registered")
 
         if fn.__doc__ is None:
             raise ActionAIException("function must have a docstring")
 
-        self.functions[fn.__name__] = ActionAIFunction(  # type: ignore #TODO: Fix this
+        action_function = ActionAIFunction(
             fn=fn,
             name=fn.__name__,
             description=fn.__doc__,
             input_schema=create_json_schema_for_function_input(
                 fn=fn, skip_keys=list(self.context.keys())
             ),
         )
-
-    def _set_openai_functions(self):
-        if len(self.functions) == 0:
-            return
-
-        for fun in self.functions.values():
-            self.openai_functions.append(
-                {
-                    "name": fun.name,
-                    "description": fun.description,
-                    "parameters": fun.input_schema,
-                }
-            )
+        self._functions[fn.__name__] = action_function
+        self._openai_functions.append(action_function.to_openai_function())
 
     def prompt(self, query: str) -> ChatResponse:
-        self._set_openai_functions()
         self.messages.append({"role": "user", "content": query})
 
         response = openai.ChatCompletion.create(
             model=self.model,
             messages=self.messages,
-            functions=self.openai_functions,
+            functions=self._openai_functions,
             function_call="auto",
         )
 
         response = cast(ChatResponse, response)
 
         response_message = response["choices"][0]["message"]
 
         if response_message.get("function_call") is None:
             return response
 
         function_name = response_message["function_call"]["name"]
-        fuction_to_call = self.functions[function_name].fn
+        fuction_to_call = self._functions[function_name].fn
         function_args = json.loads(response_message["function_call"]["arguments"])
         function_response = fuction_to_call(**function_args, **self.context)
 
         self.messages.append(response_message)
         self.messages.append(
             {
                 "role": "function",
```

### Comparing `actionai-0.0.4/src/actionai/json_schema.py` & `actionai-0.0.5/src/actionai/json_schema.py`

 * *Files identical despite different names*

### Comparing `actionai-0.0.4/src/actionai/types.py` & `actionai-0.0.5/src/actionai/types.py`

 * *Files identical despite different names*

### Comparing `actionai-0.0.4/setup.py` & `actionai-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['openai>=0.27.8,<0.28.0', 'pydantic>=2.0.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'actionai',
-    'version': '0.0.4',
+    'version': '0.0.5',
     'description': 'A small library to call local functions using openai function calling',
     'long_description': '# ActionAI\n\nA small library to run local functions using openai function calling\n\n## Install\n\n```shell\npip install actionai\n```\n\n## Usage\n\n```python\n# define a new function\ndef get_current_weather(location: str, unit: str = "fahrenheit"):\n    """Function to get current weather for the given location"""\n    weather_info = {\n        "location": location,\n        "temperature": "72",\n        "unit": unit,\n        "forecast": ["sunny", "windy"],\n    }\n    return weather_info\n\n\nimport actionai\n\naction = actionai.ActionAI()\naction.register(get_current_weather)\n\nresponse = action.prompt("What is the current weather in the north pole?")\n\nprint(response["choices"][0]["message"]["content"])\n# The current weather at the North Pole is 72°F. It is sunny and windy.\n```\n\nThe openai api key will be read automatically from the `OPENAI_API_KEY` environment variable. You can pass it manually as,\n\n```python\nimport actionai\n\naction = actionai.ActionAI(openai_api_key="YOUR_KEY")\n```\n\n### Adding context\n\nSometimes your function will have variables that needs to be set by the program.\n\n```python\ndef list_todos(user: str):\n    """Function to list all todos"""\n    return todos[user]\n\naction = actionai.ActionAI(context={"user": "jason"})\n```\n\nThe context keys are skipped when creating json schema. The values are directly passed at the time of function calling.\n\n> **Warning**\n> A function must be fully typed and must have a docstring(one liner explanation of the function is enough)\n\n### Choosing a model\n\nBy default, the completion run on the `gpt-3.5-turbo-0613` model. You can change the model using the `model` argument.\n\n```python\nimport actionai\n\naction = actionai.ActionAI(model="gpt-4")\n```\n\nYou can see the complete list of supported chat completion models [here](https://platform.openai.com/docs/models/model-endpoint-compatibility)\n\n## Demo\n\nRunning [todo example](https://github.com/amalshaji/actionai/blob/main/examples/todo.py) 👇🏻\n\n![todo demo](https://raw.githubusercontent.com/amalshaji/actionai/main/examples/demo.svg)\n\nFor more examples, checkout the [examples](https://github.com/amalshaji/actionai/tree/main/examples) directory.\n',
     'author': 'Amal Shaji',
     'author_email': 'amalshajid@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `actionai-0.0.4/PKG-INFO` & `actionai-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: actionai
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small library to call local functions using openai function calling
 Author: Amal Shaji
 Author-email: amalshajid@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: openai (>=0.27.8,<0.28.0)
```

