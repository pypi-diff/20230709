# Comparing `tmp/gptfunctionutil-0.1.6.tar.gz` & `tmp/gptfunctionutil-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptfunctionutil-0.1.6.tar", last modified: Thu Jul  6 19:21:19 2023, max compression
+gzip compressed data, was "gptfunctionutil-0.1.7.tar", last modified: Sun Jul  9 18:06:50 2023, max compression
```

## Comparing `gptfunctionutil-0.1.6.tar` & `gptfunctionutil-0.1.7.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:21:19.507264 gptfunctionutil-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-06 19:20:51.000000 gptfunctionutil-0.1.6/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:21:19.499263 gptfunctionutil-0.1.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:21:19.503263 gptfunctionutil-0.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-06 19:20:51.000000 gptfunctionutil-0.1.6/.github/workflows/publishpackage.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-07-06 19:20:51.000000 gptfunctionutil-0.1.6/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:21:19.503263 gptfunctionutil-0.1.6/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-06 19:20:51.000000 gptfunctionutil-0.1.6/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-06 19:20:51.000000 gptfunctionutil-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-07-06 19:21:19.503263 gptfunctionutil-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-07-06 19:20:51.000000 gptfunctionutil-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-06 19:20:51.000000 gptfunctionutil-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:20:51.000000 gptfunctionutil-0.1.6/pytest.local.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 19:21:19.507264 gptfunctionutil-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:21:19.503263 gptfunctionutil-0.1.6/src/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-06 19:20:51.000000 gptfunctionutil-0.1.6/src/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:21:19.503263 gptfunctionutil-0.1.6/src/gptfunctionutil/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-06 19:20:51.000000 gptfunctionutil-0.1.6/src/gptfunctionutil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-07-06 19:20:51.000000 gptfunctionutil-0.1.6/src/gptfunctionutil/functionlib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:21:19.503263 gptfunctionutil-0.1.6/src/gptfunctionutil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-07-06 19:21:19.000000 gptfunctionutil-0.1.6/src/gptfunctionutil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-06 19:21:19.000000 gptfunctionutil-0.1.6/src/gptfunctionutil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 19:21:19.000000 gptfunctionutil-0.1.6/src/gptfunctionutil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-06 19:21:19.000000 gptfunctionutil-0.1.6/src/gptfunctionutil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-06 19:21:19.000000 gptfunctionutil-0.1.6/src/gptfunctionutil.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:21:19.503263 gptfunctionutil-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-06 19:20:51.000000 gptfunctionutil-0.1.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-06 19:20:51.000000 gptfunctionutil-0.1.6/tests/test_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:06:50.687763 gptfunctionutil-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-09 18:06:27.000000 gptfunctionutil-0.1.7/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:06:50.683763 gptfunctionutil-0.1.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:06:50.683763 gptfunctionutil-0.1.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-09 18:06:27.000000 gptfunctionutil-0.1.7/.github/workflows/publishpackage.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-07-09 18:06:27.000000 gptfunctionutil-0.1.7/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:06:50.687763 gptfunctionutil-0.1.7/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-09 18:06:27.000000 gptfunctionutil-0.1.7/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-09 18:06:27.000000 gptfunctionutil-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-07-09 18:06:50.687763 gptfunctionutil-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-07-09 18:06:27.000000 gptfunctionutil-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-09 18:06:27.000000 gptfunctionutil-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 18:06:27.000000 gptfunctionutil-0.1.7/pytest.local.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 18:06:50.687763 gptfunctionutil-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:06:50.687763 gptfunctionutil-0.1.7/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-09 18:06:27.000000 gptfunctionutil-0.1.7/src/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:06:50.687763 gptfunctionutil-0.1.7/src/gptfunctionutil/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-09 18:06:27.000000 gptfunctionutil-0.1.7/src/gptfunctionutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14771 2023-07-09 18:06:27.000000 gptfunctionutil-0.1.7/src/gptfunctionutil/functionlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13063 2023-07-09 18:06:27.000000 gptfunctionutil-0.1.7/src/gptfunctionutil/functionlib_discord.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:06:50.687763 gptfunctionutil-0.1.7/src/gptfunctionutil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-07-09 18:06:50.000000 gptfunctionutil-0.1.7/src/gptfunctionutil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-09 18:06:50.000000 gptfunctionutil-0.1.7/src/gptfunctionutil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 18:06:50.000000 gptfunctionutil-0.1.7/src/gptfunctionutil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-09 18:06:50.000000 gptfunctionutil-0.1.7/src/gptfunctionutil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-09 18:06:50.000000 gptfunctionutil-0.1.7/src/gptfunctionutil.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:06:50.687763 gptfunctionutil-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-09 18:06:27.000000 gptfunctionutil-0.1.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-09 18:06:27.000000 gptfunctionutil-0.1.7/tests/test_methods.py
```

### Comparing `gptfunctionutil-0.1.6/.github/workflows/publishpackage.yaml` & `gptfunctionutil-0.1.7/.github/workflows/publishpackage.yaml`

 * *Files identical despite different names*

### Comparing `gptfunctionutil-0.1.6/.gitignore` & `gptfunctionutil-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `gptfunctionutil-0.1.6/.vscode/settings.json` & `gptfunctionutil-0.1.7/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gptfunctionutil-0.1.6/LICENSE` & `gptfunctionutil-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gptfunctionutil-0.1.6/PKG-INFO` & `gptfunctionutil-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptfunctionutil
-Version: 0.1.6
+Version: 0.1.7
 Summary: A simple package for the purpose of providing a set of utilities that make it easier to invoke python methods and discord.py commands with the OpenAI Function Calling API
 Author-email: Crosswave Omega <xtream2pro@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 CrosswaveOmega
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -25,14 +25,15 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/CrosswaveOmega/GPT-Function-Calling-Utility
 Keywords: discord.py,OpenAI,Function Calling API
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Provides-Extra: discord
 Provides-Extra: spark
 Provides-Extra: test
 License-File: LICENSE
 
 # GPT Function Calling Utility
 
 The GPT Function Calling Utility is a Python package designed to streamline the process of calling Python functions using OpenAI's Function Calling API.
```

### Comparing `gptfunctionutil-0.1.6/README.md` & `gptfunctionutil-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `gptfunctionutil-0.1.6/pyproject.toml` & `gptfunctionutil-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 [project]
 name = 'gptfunctionutil'
-version = "0.1.6"
+version = "0.1.7"
 license = {file = "LICENSE"}
 authors = [{name="Crosswave Omega",email= "xtream2pro@gmail.com"}]
 description = "A simple package for the purpose of providing a set of utilities that make it easier to invoke python methods and discord.py commands with the OpenAI Function Calling API"
 readme = 'README.md'
 
 keywords = ['discord.py', 'OpenAI', 'Function Calling API']
 requires-python = '>=3.10'
 
-dependencies = [
-    "discord>=2.1.0"
-]
 [project.urls]
 "Homepage"= "https://github.com/CrosswaveOmega/GPT-Function-Calling-Utility"
 
 
 [options.packages.find]
 exclude = ['tests',  'docs']
 
 
 
 [project.optional-dependencies]
+
+discord = [
+    "discord>=2.1.0"
+]
 spark = [
     "pyspark>=3.0.0"
 ]
 test = [
     "bandit[toml]==1.7.4",
     "black==23.1.0",
     "check-manifest==0.48",
```

### Comparing `gptfunctionutil-0.1.6/src/gptfunctionutil/functionlib.py` & `gptfunctionutil-0.1.7/src/gptfunctionutil/functionlib.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,21 +2,15 @@
 import json
 import re
 from typing import Any, Coroutine, Dict, List, Union
 
 from enum import Enum, EnumMeta
 
 from datetime import datetime
-from discord.ext.commands import (
-    Command,
-    Context,
-    Bot,
-    CommandNotFound,
-    CheckFailure
-)
+
 
 
 class CommandSingleton:
     _instance = None
     _commands = {}
 
     @classmethod
@@ -28,14 +22,149 @@
     @staticmethod
     def add_command(name, command):
         CommandSingleton._commands[name] = command
 
     @staticmethod
     def load_command(name):
         return CommandSingleton._commands.get(name, None)
+
+substitutions={
+    'str':'string',
+    'int':'integer',
+    'bool':'boolean',
+    'float':'number',
+    'datetime':'string',
+    'Literal':'string'
+}
+
+to_ignore=['_empty','Context']
+class LibCommand:
+    '''This class is a container for functions, coroutines, and discord.py Commands
+    that have been annotated with the LibParam and the AILibFunction decorators,
+    wrapping them up with attributes that help the GPTFunctionLibary invoke them.'''
+    def __init__(self, func: Union[callable,Coroutine], name: str, description: str, required:List[str]=[],force_words:List[str]=[], enabled=True):
+        '''
+        Description: This class represents a library command. It encapsulates a Discord bot command, along with its associated metadata and functionality.
+
+        Args:
+            func (Command): The Discord.py bot command object. (commands.command())
+            name (str): The name of the command.
+            description (str): The description of the command.
+            required (List[str], optional): A list of required parameter names. Defaults to an empty list.
+            force_words (List[str], optional): A list of force words. Defaults to an empty list.
+            enabled (bool, optional): Indicates whether the command is enabled. Defaults to True.
+        '''
+        self.command=func
+        self.internal_name=self.function_name=name
+        self.comm_type='callable'
+
+        if inspect.iscoroutinefunction(func):
+            self.comm_type='coroutine'
+        print(self.function_name,self.comm_type)
+        my_schema= {
+            'name': self.function_name,
+            'description': description,
+            'parameters':{'type': 'object','properties': {},'required': []}
+        }
+
+        self.function_schema=my_schema
+        self.required=required
+        #if 'parameter_decorators' in func.extras:
+        self.param_iterate()
+        self.enabled=enabled
+        self.force_words=force_words
+    def param_iterate(self):
+        '''
+        Iterates over the command's arguments and update the function_schema dictionary with parameter information.
+        Every parameter that isn't 'self' or ctx must be added!
+        '''
+        func=self.command
+        paramdict={}
+        param_decorators={}
+
+        sig = inspect.signature(func)
+        if hasattr(func,'parameter_decorators'):
+            paramdict=sig.parameters
+            param_decorators=func.parameter_decorators
+        print("THE type is",self.comm_type)
+        self.function_schema.update(
+            { 'parameters': {'type': 'object','properties': {},'required': []}}
+        )
+        for param_name, param in paramdict.items():
+
+            if isinstance(param.annotation, str):
+                typename = param.annotation  # Treat the string annotation as a regular string
+            else:
+                typename = param.annotation.__name__  # Access the __name__ attribute of the type object
+
+            oldtypename=typename
+            if typename in substitutions:
+                typename=substitutions[typename]
+            else:
+                continue
+            param_info = {
+                'type': typename,
+                'description': param_decorators.get(param_name, '')
+            }
+            if typename in to_ignore:
+                continue
+            if oldtypename== 'datetime':
+                param_info['format']='date-time'
+            if oldtypename == 'Literal':
+                literal_values = param.annotation.__args__
+                param_info['enum'] = literal_values
+            self.function_schema['parameters']['properties'][param_name] = param_info
+            if param.default == inspect.Parameter.empty or param_name in self.required:
+                self.function_schema['parameters']['required'].append(param_name)
+
+    def convert_args(self,function_args: Dict[str, Any]) -> Dict[str, Any]:
+        '''Preform any needed conversion of the function argument dictionary, such as
+        converting a string to a datetime object.
+
+        Args:
+            function_args (Dict[str, Any]): A dictionary containing the function arguments.
+
+        Returns:
+            Dict[str, Any]: The converted function argument dictionary.
+        '''
+        schema=self.function_schema
+        parameters=schema['parameters']
+        for i, v in parameters['properties'].items():
+            if i in function_args:
+                form=v.get('format',None)
+                if not form: continue
+                if form=='date-time':
+                    datetime_format = "%Y-%m-%dT%H:%M:%S%z"
+                    converted_datetime = datetime.strptime(
+                        function_args[i], datetime_format
+                        )
+                    function_args[i]=converted_datetime
+        return function_args
+
+    def check_force(self,query:str) -> bool:
+        '''
+        Checks if the given query contains any of the command's force words.
+
+        Args:
+           query (str): The query to be checked.
+
+        Returns:
+
+            bool: True if the query contains force words, False otherwise.
+        '''
+        if self.force_words:
+            pattern = r'\b(?:{})\b'.format('|'.join(map(re.escape,  self.force_words)))
+            regex = re.compile(pattern, re.IGNORECASE)
+            match = regex.search(query)
+            if match:
+                return True
+        return False
+
+
+
 class GPTFunctionLibrary:
     """
     A collection of methods to be used with OpenAI's chat completion endpoint.
     When subclassed, decorated methods, called LibCommands, will be added to an internal FunctionDict along with
     a special LibCommand object
     All methods will be converted to a function schema dictionary, which will be sent to OpenAI along with any user text.
     OpenAI will then format paramaters and return them within a JSON object, which will be used to trigger the method
@@ -46,15 +175,15 @@
     Bot Commands can be defined in any Cog, so long as add_in_commands is called at least once before
     the GPTFunctionLibrary is used with the API.
 
     Attributes:
         FunctionDict ( Dict[str, Union[Command,callable]]): A dictionary mapping command and method names to the corresponding Command or methods
     """
 
-    FunctionDict: Dict[str, Union[Command,callable]] = {}
+    FunctionDict: Dict[str, LibCommand] = {}
     do_expression: bool = False
     my_math_parser:callable=None
     def __new__(cls, *args: Any, **kwargs: Any) -> Any:
         """
         Override the __new__ method to update the FunctionDict when instantiating or subclassing.
 
         Returns:
@@ -69,64 +198,44 @@
         Update the FunctionDict with decorated methods from a descended class.
 
         This method iterates over the class's methods and adds the ones with function schema to the FunctionDict.
         """
         for name, method in self.__class__.__dict__.items():
             if hasattr(method, "libcommand"):
                 function_name = method.libcommand.function_name or method.__name__
-                self.FunctionDict[function_name] = method
-    def add_in_commands(self,bot:Bot) -> None:
-        """
-        Update the FunctionDict with decorated discord.py bot commands.
-        This has to be called somewhere before a call to the AI API if you
-        want to use the commands.
-        """
-        for command in bot.walk_commands():
-            print(command.qualified_name)
-            if "libcommand" in command.extras:
-                print(command.qualified_name, command.extras["libcommand"])
-                function_name = command.qualified_name
-                self.FunctionDict[function_name] = command
+                self.FunctionDict[function_name] = method.libcommand
+
     def force_word_check(self,query:str):
         '''
         Check if the query contains the force words of any command.
         force words will force OpenAI to invoke THAT particular command, as opposed to
         invoking a command automatically.
         '''
         functions_with_schema = []
         for name, method in self.FunctionDict.items():
             schema=None
-            comm=None
-            if isinstance(method,Command):
-                comm=method.extras['libcommand']
-            else:
-                comm=method.libcommand
+            comm=method
+
             if comm:
                 if comm.check_force(query):
                     schema=comm.function_schema
                     return [schema]
         return None
     def get_schema(self) -> List[Dict[str, Any]]:
         """
         Get the list of function schema dictionaries representing callable methods, coroutines, or bot Commands available to the library.
 
         Returns:
             A list of function schema dictionaries from each decorated method or Command
         """
         functions_with_schema = []
-        for name, method in self.FunctionDict.items():
+        for name, libmethod in self.FunctionDict.items():
             schema=None
-            if isinstance(method,Command):
-                comm=method.extras['libcommand']
-                if comm.enabled:
-                    schema=comm.function_schema
-            else:
-                comm=method.libcommand
-                if comm.enabled:
-                    schema=comm.function_schema
+            if libmethod.enabled:
+                schema=libmethod.function_schema
             if schema!=None:
                 if schema.get('parameters',None)!=None:
                     functions_with_schema.append(schema)
         return functions_with_schema
 
     def expression_match(self, function_args: str):
         '''because sometimes, the API returns an expression and not a single integer.'''
@@ -162,18 +271,16 @@
                     output=f"JSONDecodeError: {e.msg} at line {e.lineno} column {e.colno}: `{function_args_str[e.pos]}`"
                     raise json.JSONDecodeError(msg=f"{output}\n{function_args_str}", doc=function_args_str,pos=1)
             return function_name,function_args
         raise Exception(f"Function '{function_name}' not found.")
 
     def convert_args(self, function_name:str, function_args:Dict[str, Any]) -> Dict[str, Any]:
         '''Preform any needed conversion of the function arguments.'''
-        method=self.FunctionDict[function_name]
-        if isinstance(method,Command):
-            return method.extras['libcommand'].convert_args(function_args)
-        return method.libcommand.convert_args(function_args)
+        libmethod=self.FunctionDict[function_name]
+        return libmethod.convert_args(function_args)
 
 
     def call_by_dict(self, function_dict: Dict[str, Any]) -> Any:
         """
         Call a function based on the provided dictionary.
 
         Args:
@@ -186,270 +293,42 @@
             AttributeError: If the function name is not found or not callable.
         """
         try:
             function_name,function_args=self.parse_name_args(function_dict)
         except Exception as e:
             result=str(e)
             return result
-        method = self.FunctionDict.get(function_name)
-        if callable(method) and not isinstance(method,(Coroutine,Command)):
+        libmethod = self.FunctionDict.get(function_name)
+        if libmethod.comm_type=='callable':
             if len(function_args)>0:
-                for i, v in function_args.items():
-                    print("st",i,v)
-                return method(self, **function_args)
-            return method(self)
+                #for i, v in function_args.items():
+                #    print("st",i,v)
+                return libmethod.command(self, **function_args)
+            return libmethod.command(self)
         else:
             raise AttributeError(f"Method '{function_name}' not found or not callable.")
 
-    async def call_by_dict_ctx(self, ctx:Context, function_dict: Dict[str, Any]) -> Coroutine:
-        """
-        Call a Coroutine or Bot Command based on the provided dictionary.
-        Bot Commands must be decorated.
-
-        Args:
-            ctx (commands.Context): context object.
-            function_dict (Dict[str, Any]): The dictionary containing the function name and arguments.
-
-        Returns:
-            The result of the function call, or Done if there is no returned value.
-            This is so something can be added to the bot's message_chain.
-
-        Raises:
-            AttributeError: If the function name is not found or not callable.
-        """
-        try:
-            function_name,function_args=self.parse_name_args(function_dict)
-        except Exception as e:
-            result=str(e)
-            return result
-        print(function_name, function_args,len(function_args))
-        method = self.FunctionDict.get(function_name)
-        if isinstance(method,Command):
-            return await method.extras['libcommand'].invoke_command(ctx, function_args)
-
-        else:
-            comm=method.libcommand
-            if comm.comm_type=='coroutine':
-                if len(function_args)>0:
-                    return await method(self,**function_args)
-                return await method(self)
-            elif comm.comm_type=='callable':
-                if len(function_args)>0:
-                    return method(self,**function_args)
-                return method(self)
-            else:
-                raise AttributeError(f"Method '{function_name}' not found or not callable.")
 
 
-substitutions={
-    'str':'string',
-    'int':'integer',
-    'bool':'boolean',
-    'float':'number',
-    'datetime':'string',
-    'Literal':'string'
-}
-class LibCommand:
-    '''This class is a container for functions, coroutines, and discord.py Commands
-    that have been annotated with the LibParam and the AILibFunction decorators,
-    wrapping them up with attributes that help the GPTFunctionLibary invoke them.'''
-    def __init__(self, func: Union[Command,callable,Coroutine], name: str, description: str, required:List[str]=[],force_words:List[str]=[], enabled=True):
-        '''
-        Description: This class represents a library command. It encapsulates a Discord bot command, along with its associated metadata and functionality.
-
-        Args:
-            func (Command): The Discord.py bot command object. (commands.command())
-            name (str): The name of the command.
-            description (str): The description of the command.
-            required (List[str], optional): A list of required parameter names. Defaults to an empty list.
-            force_words (List[str], optional): A list of force words. Defaults to an empty list.
-            enabled (bool, optional): Indicates whether the command is enabled. Defaults to True.
-        '''
-        self.command=func
-        self.internal_name=self.function_name=name
-        self.comm_type='callable'
-
-        if isinstance(func, Command):
-            self.function_name=func.qualified_name
-            self.comm_type='command'
-        elif inspect.iscoroutinefunction(func):
-            self.comm_type='coroutine'
-        print(self.function_name,self.comm_type)
-        my_schema= {
-            'name': self.function_name,
-            'description': description,
-            'parameters':{'type': 'object','properties': {},'required': []}
-        }
-
-        self.function_schema=my_schema
-        self.required=required
-        #if 'parameter_decorators' in func.extras:
-        self.param_iterate()
-        self.enabled=enabled
-        self.force_words=force_words
-    def param_iterate(self):
-        '''
-        Iterates over the command's arguments and update the function_schema dictionary with parameter information.
-        Every parameter that isn't 'self' or ctx must be added!
-        '''
-        func=self.command
-        paramdict={}
-        param_decorators={}
-        if self.comm_type=='command':
-            if 'parameter_decorators' in func.extras:
-                paramdict=func.clean_params
-                param_decorators=func.extras['parameter_decorators']
-        else:
-            sig = inspect.signature(func)
-            if hasattr(func,'parameter_decorators'):
-                paramdict=sig.parameters
-                param_decorators=func.parameter_decorators
-        print("THE type is",self.comm_type)
-        self.function_schema.update(
-            { 'parameters': {'type': 'object','properties': {},'required': []}}
-        )
-        for param_name, param in paramdict.items():
-
-            if isinstance(param.annotation, str):
-                typename = param.annotation  # Treat the string annotation as a regular string
-            else:
-                typename = param.annotation.__name__  # Access the __name__ attribute of the type object
-
-            oldtypename=typename
-            if typename in substitutions:
-                typename=substitutions[typename]
-            else:
-                continue
-            param_info = {
-                'type': typename,
-                'description': param_decorators.get(param_name, '')
-            }
-            if self.comm_type!='command':
-                if typename == '_empty':
-                    continue
-                if typename == 'Context':
-                    continue
-            if oldtypename== 'datetime':
-                param_info['format']='date-time'
-            if oldtypename == 'Literal':
-                literal_values = param.annotation.__args__
-                param_info['enum'] = literal_values
-            self.function_schema['parameters']['properties'][param_name] = param_info
-            if param.default == inspect.Parameter.empty or param_name in self.required:
-                self.function_schema['parameters']['required'].append(param_name)
-
-    def convert_args(self,function_args: Dict[str, Any]) -> Dict[str, Any]:
-        '''Preform any needed conversion of the function argument dictionary, such as
-        converting a string to a datetime object.
-
-        Args:
-            function_args (Dict[str, Any]): A dictionary containing the function arguments.
-
-        Returns:
-            Dict[str, Any]: The converted function argument dictionary.
-        '''
-        schema=self.function_schema
-        parameters=schema['parameters']
-        for i, v in parameters['properties'].items():
-            if i in function_args:
-                form=v.get('format',None)
-                if not form: continue
-                if form=='date-time':
-                    datetime_format = "%Y-%m-%dT%H:%M:%S%z"
-                    converted_datetime = datetime.strptime(
-                        function_args[i], datetime_format
-                        )
-                    function_args[i]=converted_datetime
-        return function_args
-
-    def check_force(self,query:str) -> bool:
-        '''
-        Checks if the given query contains any of the command's force words.
-
-        Args:
-           query (str): The query to be checked.
-
-        Returns:
-
-            bool: True if the query contains force words, False otherwise.
-        '''
-        if self.force_words:
-            pattern = r'\b(?:{})\b'.format('|'.join(map(re.escape,  self.force_words)))
-            regex = re.compile(pattern, re.IGNORECASE)
-            match = regex.search(query)
-            if match:
-                return True
-        return False
-
-    async def invoke_command(self,ctx:Context,function_args:Dict[str,Any]) -> Any:
-        '''
-        Invokes the LibCommand's associated Discord bot command with the given function arguments.
-
-        Args:
-
-            ctx (Context): The Discord command context.
-            function_args (Dict[str, Any]): A dictionary containing the function arguments.
-
-        Returns:
-
-            Any: The outcome of the command execution.
-
-        '''
-        bot=ctx.bot
-        command=bot.get_command(self.function_name)
-        ctx.command=command
-        outcome="Done"
-        function_args=self.convert_args(function_args)
-        if len(function_args)>0:
-            for i, v in command.clean_params.items():
-                if not i in function_args:
-                    print(i,v)
-                    function_args[i]=v.default
-            ctx.kwargs=(function_args)
-        if ctx.command is not None:
-            bot.dispatch('command', ctx)
-            try:
-                if await bot.can_run(ctx, call_once=True):
-                    outcome2=await ctx.invoke(command,**function_args)
-                    if outcome2!=None:
-                        outcome=outcome2
-                else:
-                    raise CheckFailure('The global check once functions failed.')
-            except Exception as exc:
-                bot.dispatch('command_error', ctx, exc)
-            else:
-                bot.dispatch('command_completion', ctx)
-        elif ctx.invoked_with:
-            exc =  CommandNotFound(f'Command "{self.function_name}" is not found')
-            bot.dispatch('command_error', ctx, exc)
-        return outcome
 
 
 def LibParam(**kwargs: Any) -> Any:
     """
     Decorator to add descriptions to any valid parameter inside a GPTFunctionLibary method or discord.py bot command.
     AILibFunctions without this decorator will not be sent to the AI.
     Args:
         **kwargs: a function's parameters, and the description to be applied to each.
     Returns:
         The decorated function.
     """
-    def decorator(func: Union[Command,callable]) -> callable:
-        if isinstance(func,Command):
-            print(f"{func} is a command.")
-            if not 'parameter_decorators' in func.extras:
-                func.extras.setdefault('parameter_decorators',{})
-            func.extras['parameter_decorators'].update(kwargs)
-            print('new params:',func.extras['parameter_decorators'])
-            return func
-        else:
-            if not hasattr(func, "parameter_decorators"):
-                func.parameter_decorators = {}
-            func.parameter_decorators.update(kwargs)
-            return func
+    def decorator(func: callable) -> callable:
+        if not hasattr(func, "parameter_decorators"):
+            func.parameter_decorators = {}
+        func.parameter_decorators.update(kwargs)
+        return func
     return decorator
 
 def AILibFunction(name: str, description: str, required:List[str]=[],force_words:List[str]=[], enabled=True) -> Any:
     """
     Flags a callable method, Coroutine, or discord.py Command, creating a LibCommand object.
     In the case of a bot Command, the schema is added into the Command.extras attribute.
     Only Commands decorated with this can be called by the AI.
@@ -463,21 +342,15 @@
         description (str): The description of the function.
         required:List[str]: list of parameters you want the AI to always use reguardless of if they have defaults.
         force_words:List[str]: list of words that will be used to force this command to be triggered.
         enabled (bool): Whether or not this function is enabled by default.
     Returns:
         callable, Coroutine, or Command.
     """
-    def decorator(func: Union[Command,callable,Coroutine]):
-        if isinstance(func, Command):
-            #Added to the extras dictionary in the Command
-            mycommand=LibCommand(func,name,description,required,force_words,enabled)
-            func.extras['libcommand']=mycommand
-            return func
-        else:
-            print("ADDING CALLABLE",func,name)
-            mycommand=LibCommand(func,name,description,required,force_words,enabled)
-            func.libcommand=mycommand
+    def decorator(func: Union[callable,Coroutine]):
+        print("ADDING CALLABLE",func,name)
+        mycommand=LibCommand(func,name,description,required,force_words,enabled)
+        func.libcommand=mycommand
 
-            return func
+        return func
 
     return decorator
```

### Comparing `gptfunctionutil-0.1.6/src/gptfunctionutil.egg-info/PKG-INFO` & `gptfunctionutil-0.1.7/src/gptfunctionutil.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptfunctionutil
-Version: 0.1.6
+Version: 0.1.7
 Summary: A simple package for the purpose of providing a set of utilities that make it easier to invoke python methods and discord.py commands with the OpenAI Function Calling API
 Author-email: Crosswave Omega <xtream2pro@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 CrosswaveOmega
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -25,14 +25,15 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/CrosswaveOmega/GPT-Function-Calling-Utility
 Keywords: discord.py,OpenAI,Function Calling API
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Provides-Extra: discord
 Provides-Extra: spark
 Provides-Extra: test
 License-File: LICENSE
 
 # GPT Function Calling Utility
 
 The GPT Function Calling Utility is a Python package designed to streamline the process of calling Python functions using OpenAI's Function Calling API.
```

### Comparing `gptfunctionutil-0.1.6/tests/conftest.py` & `gptfunctionutil-0.1.7/tests/conftest.py`

 * *Files identical despite different names*

