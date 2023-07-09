# Comparing `tmp/Janex-0.0.2.tar.gz` & `tmp/Janex-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Janex-0.0.2.tar", last modified: Fri Jul  7 12:25:41 2023, max compression
+gzip compressed data, was "Janex-0.0.3.tar", last modified: Sun Jul  9 16:10:09 2023, max compression
```

## Comparing `Janex-0.0.2.tar` & `Janex-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,18 @@
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-07 12:25:41.741158 Janex-0.0.2/
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-07 12:25:41.740763 Janex-0.0.2/Janex.egg-info/
--rw-r--r--   0 cipher     (501) staff       (20)     3466 2023-07-07 12:25:41.000000 Janex-0.0.2/Janex.egg-info/PKG-INFO
--rw-r--r--   0 cipher     (501) staff       (20)      170 2023-07-07 12:25:41.000000 Janex-0.0.2/Janex.egg-info/SOURCES.txt
--rw-r--r--   0 cipher     (501) staff       (20)        1 2023-07-07 12:25:41.000000 Janex-0.0.2/Janex.egg-info/dependency_links.txt
--rw-r--r--   0 cipher     (501) staff       (20)       12 2023-07-07 12:25:41.000000 Janex-0.0.2/Janex.egg-info/requires.txt
--rw-r--r--   0 cipher     (501) staff       (20)        1 2023-07-07 12:25:41.000000 Janex-0.0.2/Janex.egg-info/top_level.txt
--rw-r--r--   0 cipher     (501) staff       (20)     2950 2023-06-30 12:37:43.000000 Janex-0.0.2/LICENSE
--rw-r--r--   0 cipher     (501) staff       (20)     3466 2023-07-07 12:25:41.741000 Janex-0.0.2/PKG-INFO
--rw-r--r--   0 cipher     (501) staff       (20)     3060 2023-07-07 12:02:54.000000 Janex-0.0.2/README.md
--rw-r--r--   0 cipher     (501) staff       (20)       38 2023-07-07 12:25:41.741196 Janex-0.0.2/setup.cfg
--rw-r--r--   0 cipher     (501) staff       (20)     1320 2023-07-07 12:25:38.000000 Janex-0.0.2/setup.py
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-09 16:10:09.149999 Janex-0.0.3/
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-09 16:10:09.143432 Janex-0.0.3/Janex/
+-rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:06:34.000000 Janex-0.0.3/Janex/Janex.py
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-09 16:10:09.149497 Janex-0.0.3/Janex/JanexSub/
+-rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:07:05.000000 Janex-0.0.3/Janex/JanexSub/JanexSub.py
+-rw-r--r--   0 cipher     (501) staff       (20)       15 2023-07-09 16:07:32.000000 Janex-0.0.3/Janex/JanexSub/__init__.py
+-rw-r--r--   0 cipher     (501) staff       (20)       15 2023-07-09 16:07:37.000000 Janex-0.0.3/Janex/__init__.py
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-09 16:10:09.148845 Janex-0.0.3/Janex.egg-info/
+-rw-r--r--   0 cipher     (501) staff       (20)     3470 2023-07-09 16:10:08.000000 Janex-0.0.3/Janex.egg-info/PKG-INFO
+-rw-r--r--   0 cipher     (501) staff       (20)      266 2023-07-09 16:10:08.000000 Janex-0.0.3/Janex.egg-info/SOURCES.txt
+-rw-r--r--   0 cipher     (501) staff       (20)        1 2023-07-09 16:10:08.000000 Janex-0.0.3/Janex.egg-info/dependency_links.txt
+-rw-r--r--   0 cipher     (501) staff       (20)       12 2023-07-09 16:10:08.000000 Janex-0.0.3/Janex.egg-info/requires.txt
+-rw-r--r--   0 cipher     (501) staff       (20)        6 2023-07-09 16:10:08.000000 Janex-0.0.3/Janex.egg-info/top_level.txt
+-rw-r--r--   0 cipher     (501) staff       (20)     2950 2023-07-07 12:33:15.000000 Janex-0.0.3/LICENSE
+-rw-r--r--   0 cipher     (501) staff       (20)     3470 2023-07-09 16:10:09.149797 Janex-0.0.3/PKG-INFO
+-rw-r--r--   0 cipher     (501) staff       (20)     3065 2023-07-07 20:09:35.000000 Janex-0.0.3/README.md
+-rw-r--r--   0 cipher     (501) staff       (20)     1319 2023-07-09 16:08:26.000000 Janex-0.0.3/Setup.py
+-rw-r--r--   0 cipher     (501) staff       (20)       38 2023-07-09 16:10:09.150054 Janex-0.0.3/setup.cfg
```

### Comparing `Janex-0.0.2/Janex.egg-info/PKG-INFO` & `Janex-0.0.3/Janex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: Janex
-Version: 0.0.2
+Version: 0.0.3
 Home-page: https://github.com/Cipher58
-Download-URL: https://github.com/Cipher58/Janex/archive/refs/tags/v0.0.2-gamma.tar.gz
+Download-URL: https://github.com/Cipher58/Janex/archive/refs/tags/v0.0.2-beta.tar.gz
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -43,15 +43,15 @@
 <h4>Using Janex in your code</h4>
 
 <h5>Create an instance</h5>
 
 Before anything else, you need to create an instance of the IntentMatcher class.
 
 ```
-intents_file_path = "intents.json"
+intents_file_path = "./intents.json"
 
 matcher = IntentMatcher(intents_file_path)
 ```
 
 <h5>Tokenizing:</h5>
 
 To utilise the tokenizer feature, here is an example of how it can be used.
@@ -67,25 +67,25 @@
 <h5>Intent classifying:</h5>
 
 To compare the input with the patterns from your intents.json storage file, you have to declare the intents file path.
 
 ```
 intents_file_path = "intents.json"
 
-intent_class = matcher.patterncompare(input_string, intents_file_path)
+intent_class = matcher.pattern_compare(input_string, intents_file_path)
 
 print(intent_class)
 ```
 
 <h5>Response similarity:</h5>
 
 Sometimes a list of responses in a class can become varied in terms of context, and so in order to get the best possible response, we can use the 'responsecompare' function to compare the input string with your list of responses.
 
 ```
-BestResponse = matcher.responsecompare(input_string, intents_file_path, intent_class)
+BestResponse = matcher.response_compare(input_string, intents_file_path, intent_class)
 
 print(BestResponse)
 ```
 
 <h5>Using Transformers:</h5>
 
 I am still currently learning about complex mathematical Machine Learning algorithms, so the numpy-based transformers included in this project are still in development, and may not always be useful or stable for a while. If you would like to use them for whatever, here's an example.
@@ -93,14 +93,14 @@
 ```
 output = matcher.Transform(input_string)
 print(output)
 ```
 
 <h3> Functionality </h3>
 
-<h4>Version 0.0.2-beta</h4>
+<h4>Version 0.0.2-Gamma</h4>
 
 - Word tokenizer ✓
 - Intent classifier ✓
 - Word Stemmer ✓
 - Support for Darwin, Unix-like and Windows ✓
 - Simple text transformer ✓
```

### Comparing `Janex-0.0.2/LICENSE` & `Janex-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Janex-0.0.2/PKG-INFO` & `Janex-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: Janex
-Version: 0.0.2
+Version: 0.0.3
 Home-page: https://github.com/Cipher58
-Download-URL: https://github.com/Cipher58/Janex/archive/refs/tags/v0.0.2-gamma.tar.gz
+Download-URL: https://github.com/Cipher58/Janex/archive/refs/tags/v0.0.2-beta.tar.gz
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -43,15 +43,15 @@
 <h4>Using Janex in your code</h4>
 
 <h5>Create an instance</h5>
 
 Before anything else, you need to create an instance of the IntentMatcher class.
 
 ```
-intents_file_path = "intents.json"
+intents_file_path = "./intents.json"
 
 matcher = IntentMatcher(intents_file_path)
 ```
 
 <h5>Tokenizing:</h5>
 
 To utilise the tokenizer feature, here is an example of how it can be used.
@@ -67,25 +67,25 @@
 <h5>Intent classifying:</h5>
 
 To compare the input with the patterns from your intents.json storage file, you have to declare the intents file path.
 
 ```
 intents_file_path = "intents.json"
 
-intent_class = matcher.patterncompare(input_string, intents_file_path)
+intent_class = matcher.pattern_compare(input_string, intents_file_path)
 
 print(intent_class)
 ```
 
 <h5>Response similarity:</h5>
 
 Sometimes a list of responses in a class can become varied in terms of context, and so in order to get the best possible response, we can use the 'responsecompare' function to compare the input string with your list of responses.
 
 ```
-BestResponse = matcher.responsecompare(input_string, intents_file_path, intent_class)
+BestResponse = matcher.response_compare(input_string, intents_file_path, intent_class)
 
 print(BestResponse)
 ```
 
 <h5>Using Transformers:</h5>
 
 I am still currently learning about complex mathematical Machine Learning algorithms, so the numpy-based transformers included in this project are still in development, and may not always be useful or stable for a while. If you would like to use them for whatever, here's an example.
@@ -93,14 +93,14 @@
 ```
 output = matcher.Transform(input_string)
 print(output)
 ```
 
 <h3> Functionality </h3>
 
-<h4>Version 0.0.2-beta</h4>
+<h4>Version 0.0.2-Gamma</h4>
 
 - Word tokenizer ✓
 - Intent classifier ✓
 - Word Stemmer ✓
 - Support for Darwin, Unix-like and Windows ✓
 - Simple text transformer ✓
```

### Comparing `Janex-0.0.2/README.md` & `Janex-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 <h4>Using Janex in your code</h4>
 
 <h5>Create an instance</h5>
 
 Before anything else, you need to create an instance of the IntentMatcher class.
 
 ```
-intents_file_path = "intents.json"
+intents_file_path = "./intents.json"
 
 matcher = IntentMatcher(intents_file_path)
 ```
 
 <h5>Tokenizing:</h5>
 
 To utilise the tokenizer feature, here is an example of how it can be used.
@@ -54,25 +54,25 @@
 <h5>Intent classifying:</h5>
 
 To compare the input with the patterns from your intents.json storage file, you have to declare the intents file path.
 
 ```
 intents_file_path = "intents.json"
 
-intent_class = matcher.patterncompare(input_string, intents_file_path)
+intent_class = matcher.pattern_compare(input_string, intents_file_path)
 
 print(intent_class)
 ```
 
 <h5>Response similarity:</h5>
 
 Sometimes a list of responses in a class can become varied in terms of context, and so in order to get the best possible response, we can use the 'responsecompare' function to compare the input string with your list of responses.
 
 ```
-BestResponse = matcher.responsecompare(input_string, intents_file_path, intent_class)
+BestResponse = matcher.response_compare(input_string, intents_file_path, intent_class)
 
 print(BestResponse)
 ```
 
 <h5>Using Transformers:</h5>
 
 I am still currently learning about complex mathematical Machine Learning algorithms, so the numpy-based transformers included in this project are still in development, and may not always be useful or stable for a while. If you would like to use them for whatever, here's an example.
@@ -80,14 +80,14 @@
 ```
 output = matcher.Transform(input_string)
 print(output)
 ```
 
 <h3> Functionality </h3>
 
-<h4>Version 0.0.2-beta</h4>
+<h4>Version 0.0.2-Gamma</h4>
 
 - Word tokenizer ✓
 - Intent classifier ✓
 - Word Stemmer ✓
 - Support for Darwin, Unix-like and Windows ✓
 - Simple text transformer ✓
```

### Comparing `Janex-0.0.2/setup.py` & `Janex-0.0.3/Setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
     long_description = fh.read()
 
 setuptools.setup(
     # Here is the module name.
     name="Janex",
 
     # version of the module
-    version="0.0.2",
+    version="0.0.3",
 
     # Name of Author
     author="Cipher58",
 
-    download_url = 'https://github.com/Cipher58/Janex/archive/refs/tags/v0.0.2-gamma.tar.gz',
+    download_url = 'https://github.com/Cipher58/Janex/archive/refs/tags/v0.0.2-beta.tar.gz',
 
     # your Email address
     author_email="cipher58public@gmail.com",
 
     # #Small Description about module
     # description="adding number",
```

