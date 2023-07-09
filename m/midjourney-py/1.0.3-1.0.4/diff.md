# Comparing `tmp/midjourney-py-1.0.3.tar.gz` & `tmp/midjourney-py-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midjourney-py-1.0.3.tar", last modified: Thu Jul  6 08:27:35 2023, max compression
+gzip compressed data, was "midjourney-py-1.0.4.tar", last modified: Sun Jul  9 06:32:27 2023, max compression
```

## Comparing `midjourney-py-1.0.3.tar` & `midjourney-py-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:27:35.555539 midjourney-py-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     9674 2023-07-06 08:27:35.555539 midjourney-py-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-07-06 08:27:08.000000 midjourney-py-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:27:35.555539 midjourney-py-1.0.3/midjourney/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-06 08:27:08.000000 midjourney-py-1.0.3/midjourney/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-06 08:27:08.000000 midjourney-py-1.0.3/midjourney/decrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-06 08:27:08.000000 midjourney-py-1.0.3/midjourney/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-06 08:27:08.000000 midjourney-py-1.0.3/midjourney/irequest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:27:35.555539 midjourney-py-1.0.3/midjourney_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9674 2023-07-06 08:27:34.000000 midjourney-py-1.0.3/midjourney_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-06 08:27:35.000000 midjourney-py-1.0.3/midjourney_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 08:27:34.000000 midjourney-py-1.0.3/midjourney_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 08:27:34.000000 midjourney-py-1.0.3/midjourney_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 08:27:34.000000 midjourney-py-1.0.3/midjourney_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 08:27:35.555539 midjourney-py-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-06 08:27:08.000000 midjourney-py-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:32:27.335518 midjourney-py-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     9837 2023-07-09 06:32:27.335518 midjourney-py-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-07-09 06:32:17.000000 midjourney-py-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:32:27.335518 midjourney-py-1.0.4/midjourney/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-09 06:32:17.000000 midjourney-py-1.0.4/midjourney/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-09 06:32:17.000000 midjourney-py-1.0.4/midjourney/decrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-09 06:32:17.000000 midjourney-py-1.0.4/midjourney/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-09 06:32:17.000000 midjourney-py-1.0.4/midjourney/irequest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:32:27.335518 midjourney-py-1.0.4/midjourney_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9837 2023-07-09 06:32:27.000000 midjourney-py-1.0.4/midjourney_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-09 06:32:27.000000 midjourney-py-1.0.4/midjourney_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 06:32:27.000000 midjourney-py-1.0.4/midjourney_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-09 06:32:27.000000 midjourney-py-1.0.4/midjourney_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-09 06:32:27.000000 midjourney-py-1.0.4/midjourney_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 06:32:27.335518 midjourney-py-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-09 06:32:17.000000 midjourney-py-1.0.4/setup.py
```

### Comparing `midjourney-py-1.0.3/PKG-INFO` & `midjourney-py-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: midjourney-py
-Version: 1.0.3
+Version: 1.0.4
 Summary: MidjourneyPy allows developers to easily use midjourney api without complications.
 Home-page: UNKNOWN
 Author: Ajaga Abdulbasit (Code  Ninja)
 Author-email: basitng2004@gmail.com
 License: UNKNOWN
 Description: 
         # Installation
         
         ```installation
-        pip install midjourney-py==1.0.0
+        pip install midjourney-py
         ```
         
-        # midjourney
+        # Midjourney
         
-        midjourney library provides a simplified and convenient way for developers to interact with the Midjourney API. With this library, developers can easily integrate Midjourney's powerful image processing capabilities into their applications without dealing with the complexities of manual API calls.
+        The Midjourney library provides a simplified and convenient way for developers to interact with the Midjourney API. With this library, developers can easily integrate Midjourney's powerful image processing capabilities into their applications without dealing with the complexities of manual API calls.
         
         ## Key Features
         
         1. _Simplified Interface_: The APIRequest class abstracts away the complexities of API
-        2. _Authentication Handling_: he library handles the authentication process, ensuring that API requests are properly authenticated with the provided API key.
+        2. _Authentication Handling_: The library handles the authentication process, ensuring that API requests are properly authenticated with the provided API key.
         3. _Endpoint Methods_: The library provides intuitive methods for each API endpoint, making it easy to perform actions such as describing images, retrieving results, upscaling images, generating images based on prompts, and generating seeds for image generation.
         4. _Response Handling_: The library processes API responses and provides them in a structured format, simplifying the integration of API results into the application workflow.
         
         ### Using the Imagine API
         
         ```python
         
@@ -182,14 +182,18 @@
         
         #### Seed response
         
         ```json
         { "taskId": "https://..........png" }
         ```
         
+        ### If you prefer learning with visual you will love this video tutorial by Code Ninja
+        
+        [Watch video](https://youtu.be/3EW5pP1t1PA)
+        
         # Get a midjourney api to interact with midjourney-py
         
         [Get API key](https://slashimagine.pro)
         
         The midjourney is created to make interacting with midjourney-py easy and more structured.
         
         # Wonderful Piece of art generated by the midjourney-py project
```

### Comparing `midjourney-py-1.0.3/README.md` & `midjourney-py-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # Installation
 
 ```installation
-pip install midjourney-py==1.0.0
+pip install midjourney-py
 ```
 
-# midjourney
+# Midjourney
 
-midjourney library provides a simplified and convenient way for developers to interact with the Midjourney API. With this library, developers can easily integrate Midjourney's powerful image processing capabilities into their applications without dealing with the complexities of manual API calls.
+The Midjourney library provides a simplified and convenient way for developers to interact with the Midjourney API. With this library, developers can easily integrate Midjourney's powerful image processing capabilities into their applications without dealing with the complexities of manual API calls.
 
 ## Key Features
 
 1. _Simplified Interface_: The APIRequest class abstracts away the complexities of API
-2. _Authentication Handling_: he library handles the authentication process, ensuring that API requests are properly authenticated with the provided API key.
+2. _Authentication Handling_: The library handles the authentication process, ensuring that API requests are properly authenticated with the provided API key.
 3. _Endpoint Methods_: The library provides intuitive methods for each API endpoint, making it easy to perform actions such as describing images, retrieving results, upscaling images, generating images based on prompts, and generating seeds for image generation.
 4. _Response Handling_: The library processes API responses and provides them in a structured format, simplifying the integration of API results into the application workflow.
 
 ### Using the Imagine API
 
 ```python
 
@@ -173,14 +173,18 @@
 
 #### Seed response
 
 ```json
 { "taskId": "https://..........png" }
 ```
 
+### If you prefer learning with visual you will love this video tutorial by Code Ninja
+
+[Watch video](https://youtu.be/3EW5pP1t1PA)
+
 # Get a midjourney api to interact with midjourney-py
 
 [Get API key](https://slashimagine.pro)
 
 The midjourney is created to make interacting with midjourney-py easy and more structured.
 
 # Wonderful Piece of art generated by the midjourney-py project
```

### Comparing `midjourney-py-1.0.3/midjourney/index.py` & `midjourney-py-1.0.4/midjourney/index.py`

 * *Files identical despite different names*

### Comparing `midjourney-py-1.0.3/midjourney/irequest.py` & `midjourney-py-1.0.4/midjourney/irequest.py`

 * *Files identical despite different names*

### Comparing `midjourney-py-1.0.3/midjourney_py.egg-info/PKG-INFO` & `midjourney-py-1.0.4/midjourney_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: midjourney-py
-Version: 1.0.3
+Version: 1.0.4
 Summary: MidjourneyPy allows developers to easily use midjourney api without complications.
 Home-page: UNKNOWN
 Author: Ajaga Abdulbasit (Code  Ninja)
 Author-email: basitng2004@gmail.com
 License: UNKNOWN
 Description: 
         # Installation
         
         ```installation
-        pip install midjourney-py==1.0.0
+        pip install midjourney-py
         ```
         
-        # midjourney
+        # Midjourney
         
-        midjourney library provides a simplified and convenient way for developers to interact with the Midjourney API. With this library, developers can easily integrate Midjourney's powerful image processing capabilities into their applications without dealing with the complexities of manual API calls.
+        The Midjourney library provides a simplified and convenient way for developers to interact with the Midjourney API. With this library, developers can easily integrate Midjourney's powerful image processing capabilities into their applications without dealing with the complexities of manual API calls.
         
         ## Key Features
         
         1. _Simplified Interface_: The APIRequest class abstracts away the complexities of API
-        2. _Authentication Handling_: he library handles the authentication process, ensuring that API requests are properly authenticated with the provided API key.
+        2. _Authentication Handling_: The library handles the authentication process, ensuring that API requests are properly authenticated with the provided API key.
         3. _Endpoint Methods_: The library provides intuitive methods for each API endpoint, making it easy to perform actions such as describing images, retrieving results, upscaling images, generating images based on prompts, and generating seeds for image generation.
         4. _Response Handling_: The library processes API responses and provides them in a structured format, simplifying the integration of API results into the application workflow.
         
         ### Using the Imagine API
         
         ```python
         
@@ -182,14 +182,18 @@
         
         #### Seed response
         
         ```json
         { "taskId": "https://..........png" }
         ```
         
+        ### If you prefer learning with visual you will love this video tutorial by Code Ninja
+        
+        [Watch video](https://youtu.be/3EW5pP1t1PA)
+        
         # Get a midjourney api to interact with midjourney-py
         
         [Get API key](https://slashimagine.pro)
         
         The midjourney is created to make interacting with midjourney-py easy and more structured.
         
         # Wonderful Piece of art generated by the midjourney-py project
```

### Comparing `midjourney-py-1.0.3/setup.py` & `midjourney-py-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.3'
+VERSION = '1.0.4'
 DESCRIPTION = 'MidjourneyPy allows developers to easily use midjourney api without complications.'
 LONG_DESCRIPTION = '''The MidjourneyPy APIRequest library provides a simplified and convenient way for developers to interact with the Midjourney API. With this library, developers can easily integrate Midjourney's powerful image processing capabilities into their applications without dealing with the complexities of manual API calls.'''
 
 # Setting up
 setup(
     name="midjourney-py",
     version=VERSION,
```

