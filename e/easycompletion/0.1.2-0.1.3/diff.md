# Comparing `tmp/easycompletion-0.1.2.tar.gz` & `tmp/easycompletion-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easycompletion-0.1.2.tar", last modified: Fri Jul  7 12:02:12 2023, max compression
+gzip compressed data, was "easycompletion-0.1.3.tar", last modified: Sun Jul  9 00:21:37 2023, max compression
```

## Comparing `easycompletion-0.1.2.tar` & `easycompletion-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-07 12:02:12.418508 easycompletion-0.1.2/
--rw-r--r--   0 shawwalters   (501) staff       (20)     1126 2023-07-07 00:23:10.000000 easycompletion-0.1.2/LICENSE
--rw-r--r--   0 shawwalters   (501) staff       (20)     3538 2023-07-07 12:02:12.418309 easycompletion-0.1.2/PKG-INFO
--rw-r--r--   0 shawwalters   (501) staff       (20)     2929 2023-07-07 11:54:52.000000 easycompletion-0.1.2/README.md
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-07 12:02:12.412197 easycompletion-0.1.2/easycompletion/
--rw-r--r--   0 shawwalters   (501) staff       (20)      368 2023-07-07 12:02:08.000000 easycompletion-0.1.2/easycompletion/__init__.py
--rw-r--r--   0 shawwalters   (501) staff       (20)      439 2023-07-07 11:44:12.000000 easycompletion-0.1.2/easycompletion/constants.py
--rw-r--r--   0 shawwalters   (501) staff       (20)    10224 2023-07-07 11:48:52.000000 easycompletion-0.1.2/easycompletion/language.py
--rw-r--r--   0 shawwalters   (501) staff       (20)     1250 2023-07-07 11:55:29.000000 easycompletion-0.1.2/easycompletion/language_test.py
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-07 12:02:12.418028 easycompletion-0.1.2/easycompletion.egg-info/
--rw-r--r--   0 shawwalters   (501) staff       (20)     3538 2023-07-07 12:02:12.000000 easycompletion-0.1.2/easycompletion.egg-info/PKG-INFO
--rw-r--r--   0 shawwalters   (501) staff       (20)      329 2023-07-07 12:02:12.000000 easycompletion-0.1.2/easycompletion.egg-info/SOURCES.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)        1 2023-07-07 12:02:12.000000 easycompletion-0.1.2/easycompletion.egg-info/dependency_links.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)        9 2023-07-07 12:02:12.000000 easycompletion-0.1.2/easycompletion.egg-info/requires.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       15 2023-07-07 12:02:12.000000 easycompletion-0.1.2/easycompletion.egg-info/top_level.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       38 2023-07-07 12:02:12.418564 easycompletion-0.1.2/setup.cfg
--rw-r--r--   0 shawwalters   (501) staff       (20)     1266 2023-07-07 12:02:08.000000 easycompletion-0.1.2/setup.py
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-09 00:21:37.225915 easycompletion-0.1.3/
+-rw-r--r--   0 shawwalters   (501) staff       (20)     1126 2023-07-07 00:23:10.000000 easycompletion-0.1.3/LICENSE
+-rw-r--r--   0 shawwalters   (501) staff       (20)     3534 2023-07-09 00:21:37.225648 easycompletion-0.1.3/PKG-INFO
+-rw-r--r--   0 shawwalters   (501) staff       (20)     2925 2023-07-07 13:55:30.000000 easycompletion-0.1.3/README.md
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-09 00:21:37.223996 easycompletion-0.1.3/easycompletion/
+-rw-r--r--   0 shawwalters   (501) staff       (20)      446 2023-07-09 00:21:33.000000 easycompletion-0.1.3/easycompletion/__init__.py
+-rw-r--r--   0 shawwalters   (501) staff       (20)      439 2023-07-09 00:18:12.000000 easycompletion-0.1.3/easycompletion/constants.py
+-rw-r--r--   0 shawwalters   (501) staff       (20)    11359 2023-07-09 00:18:17.000000 easycompletion-0.1.3/easycompletion/language.py
+-rw-r--r--   0 shawwalters   (501) staff       (20)     2163 2023-07-09 00:17:33.000000 easycompletion-0.1.3/easycompletion/language_test.py
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-09 00:21:37.224923 easycompletion-0.1.3/easycompletion.egg-info/
+-rw-r--r--   0 shawwalters   (501) staff       (20)     3534 2023-07-09 00:21:37.000000 easycompletion-0.1.3/easycompletion.egg-info/PKG-INFO
+-rw-r--r--   0 shawwalters   (501) staff       (20)      329 2023-07-09 00:21:37.000000 easycompletion-0.1.3/easycompletion.egg-info/SOURCES.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)        1 2023-07-09 00:21:37.000000 easycompletion-0.1.3/easycompletion.egg-info/dependency_links.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)        9 2023-07-09 00:21:37.000000 easycompletion-0.1.3/easycompletion.egg-info/requires.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)       15 2023-07-09 00:21:37.000000 easycompletion-0.1.3/easycompletion.egg-info/top_level.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)       38 2023-07-09 00:21:37.226006 easycompletion-0.1.3/setup.cfg
+-rw-r--r--   0 shawwalters   (501) staff       (20)     1266 2023-07-09 00:21:33.000000 easycompletion-0.1.3/setup.py
```

### Comparing `easycompletion-0.1.2/LICENSE` & `easycompletion-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `easycompletion-0.1.2/PKG-INFO` & `easycompletion-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easycompletion
-Version: 0.1.2
+Version: 0.1.3
 Summary: Easy-to-use agent memory, powered by chromadb
 Home-page: https://github.com/lalalune/easycompletion
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
@@ -103,8 +103,8 @@
 
 # Contributions Welcome
 
 If you like this library and want to contribute in any way, please feel free to submit a PR and I will review it. Please note that the goal here is simplicity and accesibility, using common language and few dependencies.
 
 # Questions, Comments, Concerns
 
-If you have any questions, please feel free to reach out to me on [Twitter](https://twitter.com/spatialweeb) or [Discord](@new.moon).
+If you have any questions, please feel free to reach out to me on [Twitter](https://twitter.com/spatialweeb) or Discord @new.moon
```

### Comparing `easycompletion-0.1.2/README.md` & `easycompletion-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -86,8 +86,8 @@
 
 # Contributions Welcome
 
 If you like this library and want to contribute in any way, please feel free to submit a PR and I will review it. Please note that the goal here is simplicity and accesibility, using common language and few dependencies.
 
 # Questions, Comments, Concerns
 
-If you have any questions, please feel free to reach out to me on [Twitter](https://twitter.com/spatialweeb) or [Discord](@new.moon).
+If you have any questions, please feel free to reach out to me on [Twitter](https://twitter.com/spatialweeb) or Discord @new.moon
```

### Comparing `easycompletion-0.1.2/easycompletion/language.py` & `easycompletion-0.1.3/easycompletion/language.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import openai
 import tiktoken
 import re
 import json
 import ast
 
-from constants import (
+from dotenv import load_dotenv
+
+load_dotenv()  # take environment variables from .env.
+
+from easycompletion.constants import (
     default_text_model,
     long_text_model,
     openai_api_key,
 )
 
 # Set OpenAI API key
 openai.api_key = openai_api_key
@@ -75,14 +79,42 @@
 
     # if the function argument keys are the same as the function call parameters, return true
     if set(function["parameters"]["properties"].keys()) == set(arguments.keys()):
         return True
 
     return False
 
+def compose_function(name, description, properties, required_property_names):
+    """
+    Composes a function.
+    properties is a dictionary of property objects, with the property name as the key
+    property object types are discussed here: https://openai.com/blog/function-calling-and-other-api-updates
+    required_property_names is a list of property names that are required for the model to return
+    example usage:
+    summarization_function = compose_function(
+        name="summarize_text",
+        description="Summarize the text. Include the topic, subtopics.",
+        properties={
+            "summary": {
+                "type": "string",
+                "description": "Detailed summary of the text.",
+            },
+        },
+        required_property_names=["summary"],
+    )
+    """
+    return {
+        "name": name,
+        "description": description,
+        "parameters": {
+            "type": "object",
+            "properties": properties,
+            "required": required_property_names,
+        },
+    }
 
 def compose_prompt(prompt_template, parameters):
     """
     Composes a prompt using a template and parameters.
     Parameter keys are enclosed in double curly brackets and replaced with parameter values.
     For example, {{actions}} will be replaced by the actions parameter.
     Parameter values can be a string, dictionary or list
```

### Comparing `easycompletion-0.1.2/easycompletion.egg-info/PKG-INFO` & `easycompletion-0.1.3/easycompletion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easycompletion
-Version: 0.1.2
+Version: 0.1.3
 Summary: Easy-to-use agent memory, powered by chromadb
 Home-page: https://github.com/lalalune/easycompletion
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
@@ -103,8 +103,8 @@
 
 # Contributions Welcome
 
 If you like this library and want to contribute in any way, please feel free to submit a PR and I will review it. Please note that the goal here is simplicity and accesibility, using common language and few dependencies.
 
 # Questions, Comments, Concerns
 
-If you have any questions, please feel free to reach out to me on [Twitter](https://twitter.com/spatialweeb) or [Discord](@new.moon).
+If you have any questions, please feel free to reach out to me on [Twitter](https://twitter.com/spatialweeb) or Discord @new.moon
```

### Comparing `easycompletion-0.1.2/setup.py` & `easycompletion-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = [line for line in long_description if not '<img' in line]
     # now join all the lines back together
     long_description = '\n'.join(long_description)
     
 
 setup(
     name='easycompletion',
-    version='0.1.2',
+    version='0.1.3',
     description='Easy-to-use agent memory, powered by chromadb',
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url='https://github.com/lalalune/easycompletion',
     author='Moon',
     author_email='shawmakesmagic@gmail.com',
     license='MIT',
```

