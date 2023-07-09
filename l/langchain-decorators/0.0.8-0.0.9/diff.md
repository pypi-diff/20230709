# Comparing `tmp/langchain-decorators-0.0.8.tar.gz` & `tmp/langchain-decorators-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain-decorators-0.0.8.tar", last modified: Fri Jun 16 23:04:47 2023, max compression
+gzip compressed data, was "langchain-decorators-0.0.9.tar", last modified: Sat Jun 17 14:23:10 2023, max compression
```

## Comparing `langchain-decorators-0.0.8.tar` & `langchain-decorators-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-16 23:04:47.480293 langchain-decorators-0.0.8/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1066 2023-06-09 22:30:45.000000 langchain-decorators-0.0.8/LICENSE
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    17654 2023-06-16 23:04:47.479292 langchain-decorators-0.0.8/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    17299 2023-06-16 23:01:41.000000 langchain-decorators-0.0.8/README.md
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 langchain-decorators-0.0.8/pyproject.toml
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-06-16 23:04:47.480361 langchain-decorators-0.0.8/setup.cfg
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1117 2023-06-11 12:35:54.000000 langchain-decorators-0.0.8/setup.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-16 23:04:47.472641 langchain-decorators-0.0.8/src/
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-16 23:04:47.477703 langchain-decorators-0.0.8/src/langchain_decorators/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      365 2023-06-16 22:26:59.000000 langchain-decorators-0.0.8/src/langchain_decorators/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     7431 2023-06-16 22:48:34.000000 langchain-decorators-0.0.8/src/langchain_decorators/chains.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     7738 2023-06-16 22:36:28.000000 langchain-decorators-0.0.8/src/langchain_decorators/common.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    14968 2023-06-16 22:33:40.000000 langchain-decorators-0.0.8/src/langchain_decorators/function_decorator.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    18570 2023-06-16 21:45:20.000000 langchain-decorators-0.0.8/src/langchain_decorators/output_parsers.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    21194 2023-06-16 22:50:18.000000 langchain-decorators-0.0.8/src/langchain_decorators/prompt_decorator.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    15906 2023-06-16 19:41:06.000000 langchain-decorators-0.0.8/src/langchain_decorators/prompt_template.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     4023 2023-06-16 21:33:53.000000 langchain-decorators-0.0.8/src/langchain_decorators/pydantic_helpers.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     2836 2023-06-16 22:52:56.000000 langchain-decorators-0.0.8/src/langchain_decorators/schema.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1624 2023-06-15 12:53:20.000000 langchain-decorators-0.0.8/src/langchain_decorators/streaming_context.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-16 23:04:47.478994 langchain-decorators-0.0.8/src/langchain_decorators.egg-info/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    17654 2023-06-16 23:04:47.000000 langchain-decorators-0.0.8/src/langchain_decorators.egg-info/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      739 2023-06-16 23:04:47.000000 langchain-decorators-0.0.8/src/langchain_decorators.egg-info/SOURCES.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-06-16 23:04:47.000000 langchain-decorators-0.0.8/src/langchain_decorators.egg-info/dependency_links.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-06-08 20:09:02.000000 langchain-decorators-0.0.8/src/langchain_decorators.egg-info/not-zip-safe
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       22 2023-06-16 23:04:47.000000 langchain-decorators-0.0.8/src/langchain_decorators.egg-info/requires.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       21 2023-06-16 23:04:47.000000 langchain-decorators-0.0.8/src/langchain_decorators.egg-info/top_level.txt
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-17 14:23:10.297776 langchain-decorators-0.0.9/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1066 2023-06-09 22:30:45.000000 langchain-decorators-0.0.9/LICENSE
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    17654 2023-06-17 14:23:10.297177 langchain-decorators-0.0.9/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    17299 2023-06-16 23:01:41.000000 langchain-decorators-0.0.9/README.md
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 langchain-decorators-0.0.9/pyproject.toml
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-06-17 14:23:10.297837 langchain-decorators-0.0.9/setup.cfg
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1117 2023-06-11 12:35:54.000000 langchain-decorators-0.0.9/setup.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-17 14:23:10.290137 langchain-decorators-0.0.9/src/
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-17 14:23:10.295472 langchain-decorators-0.0.9/src/langchain_decorators/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      365 2023-06-17 14:22:36.000000 langchain-decorators-0.0.9/src/langchain_decorators/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     7706 2023-06-17 14:06:30.000000 langchain-decorators-0.0.9/src/langchain_decorators/chains.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     7738 2023-06-16 22:36:28.000000 langchain-decorators-0.0.9/src/langchain_decorators/common.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    14968 2023-06-16 22:33:40.000000 langchain-decorators-0.0.9/src/langchain_decorators/function_decorator.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    18570 2023-06-16 21:45:20.000000 langchain-decorators-0.0.9/src/langchain_decorators/output_parsers.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    21324 2023-06-17 14:08:51.000000 langchain-decorators-0.0.9/src/langchain_decorators/prompt_decorator.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    15906 2023-06-16 19:41:06.000000 langchain-decorators-0.0.9/src/langchain_decorators/prompt_template.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     4023 2023-06-16 21:33:53.000000 langchain-decorators-0.0.9/src/langchain_decorators/pydantic_helpers.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3081 2023-06-17 14:12:19.000000 langchain-decorators-0.0.9/src/langchain_decorators/schema.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1624 2023-06-15 12:53:20.000000 langchain-decorators-0.0.9/src/langchain_decorators/streaming_context.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-17 14:23:10.296924 langchain-decorators-0.0.9/src/langchain_decorators.egg-info/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    17654 2023-06-17 14:23:10.000000 langchain-decorators-0.0.9/src/langchain_decorators.egg-info/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      739 2023-06-17 14:23:10.000000 langchain-decorators-0.0.9/src/langchain_decorators.egg-info/SOURCES.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-06-17 14:23:10.000000 langchain-decorators-0.0.9/src/langchain_decorators.egg-info/dependency_links.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-06-08 20:09:02.000000 langchain-decorators-0.0.9/src/langchain_decorators.egg-info/not-zip-safe
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       22 2023-06-17 14:23:10.000000 langchain-decorators-0.0.9/src/langchain_decorators.egg-info/requires.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       21 2023-06-17 14:23:10.000000 langchain-decorators-0.0.9/src/langchain_decorators.egg-info/top_level.txt
```

### Comparing `langchain-decorators-0.0.8/LICENSE` & `langchain-decorators-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.0.8/PKG-INFO` & `langchain-decorators-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-decorators
-Version: 0.0.8
+Version: 0.0.9
 Summary: syntactic sugar for langchain
 Home-page: https://github.com/ju-bezdek/langchain-decorators
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: langchain
 Requires-Python: >=3.9
```

### Comparing `langchain-decorators-0.0.8/README.md` & `langchain-decorators-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.0.8/setup.py` & `langchain-decorators-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.0.8/src/langchain_decorators/chains.py` & `langchain-decorators-0.0.9/src/langchain_decorators/chains.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from email.mime import message
 import json
 import logging
 from multiprocessing import Value
 from pyexpat.errors import messages
 from typing import Any, Callable, Dict, List, Optional, Union
 from langchain import LLMChain
 from langchain.schema import LLMResult
@@ -25,14 +26,15 @@
 class LLMChainWithFunctionSupport(LLMChain):
 
 
     functions:Optional[List[Union[Callable, BaseTool]]] = []
     function_schemas:List[dict]=None
     function_call_output_key:str="function_call_info"
     function_output_key:str="function"
+    message_output_key:str="message"
 
     @property
     def output_keys(self) -> List[str]:
         """Will always return text key.
 
         :meta private:
         """
@@ -141,18 +143,20 @@
                 prompts, stop, callbacks=run_manager.get_child() if run_manager else None
             )
         
     def _create_output(self,generation):
         res = {
                 self.output_key: generation.text,
                 self.function_call_output_key: None,
-                self.function_output_key: None
+                self.function_output_key: None,
              }
         if isinstance(generation, ChatGeneration):
-            function_call = generation.message.additional_kwargs.get("function_call")
+            res[self.message_output_key] = generation.message
+            # let's make a copy of the function call so that we don't modify the original
+            function_call = dict(generation.message.additional_kwargs.get("function_call")) if generation.message.additional_kwargs else {}
             if function_call:
                 if isinstance(function_call["arguments"],str):
                     function_call["arguments"]=json.loads(function_call["arguments"])
             if generation.message.additional_kwargs and generation.message.additional_kwargs.get("function_call"):
                 res[self.function_call_output_key] = function_call
                 res[self.function_output_key] = self.find_func(function_call["name"]) if function_call else None
         return res
```

### Comparing `langchain-decorators-0.0.8/src/langchain_decorators/common.py` & `langchain-decorators-0.0.9/src/langchain_decorators/common.py`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.0.8/src/langchain_decorators/function_decorator.py` & `langchain-decorators-0.0.9/src/langchain_decorators/function_decorator.py`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.0.8/src/langchain_decorators/output_parsers.py` & `langchain-decorators-0.0.9/src/langchain_decorators/output_parsers.py`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.0.8/src/langchain_decorators/prompt_decorator.py` & `langchain-decorators-0.0.9/src/langchain_decorators/prompt_decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
                 
                 
        
 
         def prepare_call_args(*args, **kwargs):
             global_settings = GlobalSettings.get_current_settings()
 
-            if not StreamingContext.get_context():
+            if _capture_stream and not StreamingContext.get_context():
                 print_log(f"INFO: Not inside StreamingContext. Ignoring capture_stream for {full_name}", logging.DEBUG, LogColors.WHITE)
                 capture_stream=False
             else:
                 capture_stream=_capture_stream
            
             if not llm:
                 if capture_stream:
@@ -382,23 +382,25 @@
                 _async_function = None
         else:
             raise TypeError(f"Invalid function type: {_function} of type {type(_function)}")
 
         return OutputWithFunctionCall(
                 output=result,
                 output_text=result_data["text"],
+                output_message=result_data["message"],
                 function=_sync_function,
                 function_async=_async_function,
                 function_name=result_data["function_call_info"]["name"],
                 function_args=result_data["function_call_info"]["arguments"],
                 function_arguments=_tool_arguments
             )
     else:
         return OutputWithFunctionCall(
                 output=result,
+                output_message=result_data["message"],
                 output_text=result_data["text"],
             )
 
 def log_results(result_data, result, is_function_call, verbose, prompt_type=None):
     if verbose or prompt_type:
         print_log(log_object=f"\nResult:\n{result}", log_level=prompt_type.log_level if verbose else 100,color=prompt_type.color if prompt_type else LogColors.BLUE)
         if is_function_call:
```

### Comparing `langchain-decorators-0.0.8/src/langchain_decorators/prompt_template.py` & `langchain-decorators-0.0.9/src/langchain_decorators/prompt_template.py`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.0.8/src/langchain_decorators/pydantic_helpers.py` & `langchain-decorators-0.0.9/src/langchain_decorators/pydantic_helpers.py`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.0.8/src/langchain_decorators/schema.py` & `langchain-decorators-0.0.9/src/langchain_decorators/schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 import asyncio
 import re
 from typing import Any, Callable, Dict, Generic, Optional, TypeVar, Union
 from pydantic import BaseModel
+from langchain.schema import AIMessage
 from langchain.schema import FunctionMessage
 import json
 
 
 
 T = TypeVar("T")
 
 class OutputWithFunctionCall(Generic[T],BaseModel):
     output_text:str
+    output_message:AIMessage
     output:T
     function_name:str =None
     function_arguments:Union[Dict[str,Any],str,None]
     function:Callable = None
     function_async:Callable = None
     result: Any = None
     
     @property
     def is_function_call(self):
-        return (self.function or self.function_async)
+        return bool(self.function or self.function_async)
     
     @property
     def support_async(self):
         return bool(self.function_async)
     
     @property
     def support_sync(self):
@@ -38,14 +40,17 @@
             if isinstance(self.function_arguments, dict):
                 result= await self.function_async(**self.function_arguments)
             else:
                 result= await self.function_async(self.function_arguments)
         else:
             await asyncio.sleep(0)
             result= self.function(**self.function_arguments)
+            if result and asyncio.iscoroutine(result):
+                # this handles special scenario when fake @llm_function is used
+                result = await result
         return result
         
     def execute(self):
         """ Executes the function synchronously. 
         If the function is async, it will be executed in a event loop.
         """
         if not (self.function or self.function_async):
```

### Comparing `langchain-decorators-0.0.8/src/langchain_decorators/streaming_context.py` & `langchain-decorators-0.0.9/src/langchain_decorators/streaming_context.py`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.0.8/src/langchain_decorators.egg-info/PKG-INFO` & `langchain-decorators-0.0.9/src/langchain_decorators.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-decorators
-Version: 0.0.8
+Version: 0.0.9
 Summary: syntactic sugar for langchain
 Home-page: https://github.com/ju-bezdek/langchain-decorators
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: langchain
 Requires-Python: >=3.9
```

### Comparing `langchain-decorators-0.0.8/src/langchain_decorators.egg-info/SOURCES.txt` & `langchain-decorators-0.0.9/src/langchain_decorators.egg-info/SOURCES.txt`

 * *Files identical despite different names*

