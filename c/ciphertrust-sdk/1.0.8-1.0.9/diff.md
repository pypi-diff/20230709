# Comparing `tmp/ciphertrust-sdk-1.0.8.tar.gz` & `tmp/ciphertrust-sdk-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ciphertrust-sdk-1.0.8.tar", last modified: Thu Jul  6 17:02:36 2023, max compression
+gzip compressed data, was "ciphertrust-sdk-1.0.9.tar", last modified: Thu Jul  6 17:14:39 2023, max compression
```

## Comparing `ciphertrust-sdk-1.0.8.tar` & `ciphertrust-sdk-1.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-07-06 17:02:36.921940 ciphertrust-sdk-1.0.8/
--rw-rw-r--   0 adamt      (501) staff       (20)     1064 2023-07-06 16:49:06.000000 ciphertrust-sdk-1.0.8/LICENSE
--rw-r--r--   0 adamt      (501) staff       (20)    17591 2023-07-06 17:02:36.921300 ciphertrust-sdk-1.0.8/PKG-INFO
--rw-rw-r--   0 adamt      (501) staff       (20)    15908 2023-07-06 16:49:06.000000 ciphertrust-sdk-1.0.8/README.md
-drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-07-06 17:02:36.914054 ciphertrust-sdk-1.0.8/ciphertrust_sdk.egg-info/
--rw-r--r--   0 adamt      (501) staff       (20)    17591 2023-07-06 17:02:36.000000 ciphertrust-sdk-1.0.8/ciphertrust_sdk.egg-info/PKG-INFO
--rw-r--r--   0 adamt      (501) staff       (20)      509 2023-07-06 17:02:36.000000 ciphertrust-sdk-1.0.8/ciphertrust_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 adamt      (501) staff       (20)        1 2023-07-06 17:02:36.000000 ciphertrust-sdk-1.0.8/ciphertrust_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 adamt      (501) staff       (20)       94 2023-07-06 17:02:36.000000 ciphertrust-sdk-1.0.8/ciphertrust_sdk.egg-info/requires.txt
--rw-r--r--   0 adamt      (501) staff       (20)       12 2023-07-06 17:02:36.000000 ciphertrust-sdk-1.0.8/ciphertrust_sdk.egg-info/top_level.txt
--rw-rw-r--   0 adamt      (501) staff       (20)     1021 2023-07-06 16:49:06.000000 ciphertrust-sdk-1.0.8/pyproject.toml
--rw-rw-r--   0 adamt      (501) staff       (20)       93 2023-07-06 16:49:06.000000 ciphertrust-sdk-1.0.8/requirements.txt
--rw-r--r--   0 adamt      (501) staff       (20)       38 2023-07-06 17:02:36.922103 ciphertrust-sdk-1.0.8/setup.cfg
-drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-07-06 17:02:36.909491 ciphertrust-sdk-1.0.8/src/
-drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-07-06 17:02:36.920490 ciphertrust-sdk-1.0.8/src/ciphertrust/
--rw-rw-r--   0 adamt      (501) staff       (20)     1376 2023-07-06 16:49:06.000000 ciphertrust-sdk-1.0.8/src/ciphertrust/__init__.py
--rw-rw-r--   0 adamt      (501) staff       (20)       42 2023-07-06 16:49:06.000000 ciphertrust-sdk-1.0.8/src/ciphertrust/_version.py
--rw-rw-r--   0 adamt      (501) staff       (20)     7953 2023-07-06 16:49:06.000000 ciphertrust-sdk-1.0.8/src/ciphertrust/api.py
--rw-rw-r--   0 adamt      (501) staff       (20)    13595 2023-07-06 16:49:06.000000 ciphertrust-sdk-1.0.8/src/ciphertrust/auth.py
--rw-rw-r--   0 adamt      (501) staff       (20)     1472 2023-07-06 16:49:06.000000 ciphertrust-sdk-1.0.8/src/ciphertrust/config.py
--rw-rw-r--   0 adamt      (501) staff       (20)      471 2023-07-06 16:49:06.000000 ciphertrust-sdk-1.0.8/src/ciphertrust/exceptions.py
--rw-rw-r--   0 adamt      (501) staff       (20)     9482 2023-07-06 16:49:06.000000 ciphertrust-sdk-1.0.8/src/ciphertrust/models.py
--rw-rw-r--   0 adamt      (501) staff       (20)    15234 2023-07-06 16:49:06.000000 ciphertrust-sdk-1.0.8/src/ciphertrust/requestapi.py
--rw-rw-r--   0 adamt      (501) staff       (20)      729 2023-07-06 16:49:06.000000 ciphertrust-sdk-1.0.8/src/ciphertrust/static.py
--rw-rw-r--   0 adamt      (501) staff       (20)    10643 2023-07-06 16:49:06.000000 ciphertrust-sdk-1.0.8/src/ciphertrust/utils.py
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-07-06 17:14:39.716016 ciphertrust-sdk-1.0.9/
+-rw-rw-r--   0 adamt      (501) staff       (20)     1064 2023-07-06 17:12:42.000000 ciphertrust-sdk-1.0.9/LICENSE
+-rw-r--r--   0 adamt      (501) staff       (20)    17721 2023-07-06 17:14:39.714663 ciphertrust-sdk-1.0.9/PKG-INFO
+-rw-rw-r--   0 adamt      (501) staff       (20)    16038 2023-07-06 17:12:42.000000 ciphertrust-sdk-1.0.9/README.md
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-07-06 17:14:39.707740 ciphertrust-sdk-1.0.9/ciphertrust_sdk.egg-info/
+-rw-r--r--   0 adamt      (501) staff       (20)    17721 2023-07-06 17:14:39.000000 ciphertrust-sdk-1.0.9/ciphertrust_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 adamt      (501) staff       (20)      509 2023-07-06 17:14:39.000000 ciphertrust-sdk-1.0.9/ciphertrust_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 adamt      (501) staff       (20)        1 2023-07-06 17:14:39.000000 ciphertrust-sdk-1.0.9/ciphertrust_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 adamt      (501) staff       (20)      128 2023-07-06 17:14:39.000000 ciphertrust-sdk-1.0.9/ciphertrust_sdk.egg-info/requires.txt
+-rw-r--r--   0 adamt      (501) staff       (20)       12 2023-07-06 17:14:39.000000 ciphertrust-sdk-1.0.9/ciphertrust_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 adamt      (501) staff       (20)     1021 2023-07-06 17:12:42.000000 ciphertrust-sdk-1.0.9/pyproject.toml
+-rw-rw-r--   0 adamt      (501) staff       (20)      127 2023-07-06 17:12:42.000000 ciphertrust-sdk-1.0.9/requirements.txt
+-rw-r--r--   0 adamt      (501) staff       (20)       38 2023-07-06 17:14:39.716262 ciphertrust-sdk-1.0.9/setup.cfg
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-07-06 17:14:39.703393 ciphertrust-sdk-1.0.9/src/
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-07-06 17:14:39.713826 ciphertrust-sdk-1.0.9/src/ciphertrust/
+-rw-rw-r--   0 adamt      (501) staff       (20)     1376 2023-07-06 17:12:42.000000 ciphertrust-sdk-1.0.9/src/ciphertrust/__init__.py
+-rw-rw-r--   0 adamt      (501) staff       (20)       42 2023-07-06 17:12:42.000000 ciphertrust-sdk-1.0.9/src/ciphertrust/_version.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     7953 2023-07-06 17:12:42.000000 ciphertrust-sdk-1.0.9/src/ciphertrust/api.py
+-rw-rw-r--   0 adamt      (501) staff       (20)    13595 2023-07-06 17:12:42.000000 ciphertrust-sdk-1.0.9/src/ciphertrust/auth.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     1472 2023-07-06 17:12:42.000000 ciphertrust-sdk-1.0.9/src/ciphertrust/config.py
+-rw-rw-r--   0 adamt      (501) staff       (20)      471 2023-07-06 17:12:42.000000 ciphertrust-sdk-1.0.9/src/ciphertrust/exceptions.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     9482 2023-07-06 17:12:42.000000 ciphertrust-sdk-1.0.9/src/ciphertrust/models.py
+-rw-rw-r--   0 adamt      (501) staff       (20)    15234 2023-07-06 17:12:42.000000 ciphertrust-sdk-1.0.9/src/ciphertrust/requestapi.py
+-rw-rw-r--   0 adamt      (501) staff       (20)      729 2023-07-06 17:12:42.000000 ciphertrust-sdk-1.0.9/src/ciphertrust/static.py
+-rw-rw-r--   0 adamt      (501) staff       (20)    10643 2023-07-06 17:12:42.000000 ciphertrust-sdk-1.0.9/src/ciphertrust/utils.py
```

### Comparing `ciphertrust-sdk-1.0.8/LICENSE` & `ciphertrust-sdk-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ciphertrust-sdk-1.0.8/PKG-INFO` & `ciphertrust-sdk-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciphertrust-sdk
-Version: 1.0.8
+Version: 1.0.9
 Summary: Thales CipherTrust SDK RestAPI
 Author-email: atav928 <dev@tavnets.com>
 License: MIT License
         
         Copyright (c) 2023 atav928
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -524,14 +524,15 @@
 | __1.0.7__ | __hotfix__ | Fixes issues with not raising proper errors when params are being passed |
 | __1.0.7__ | __feature__ | Adjusted and tested remaining http calls; see notes for details |
 | __1.0.7__ | __feature__ | Adjusted responses for all types of API calls |
 | __1.0.8__ | __a1__ | Added Error Response handling to ensure metrics in responses and error reporting; reformated logging messages and added splunk style logs with color responses |
 | __1.0.8__ | __a2__ | Added a 30s buffer to expiration of Auth Token |
 | __1.0.8__ | __a3__ | Synced error and standard format json response under response_statistics and request_parmeters |
 | __1.0.8__ | __final__ | Formated responses to return statatics on calls as well as data from call being made |
+| __1.0.9__ | __final__ | Added dependencies to requirements to fix installation issues |
 
 ### Known Bugs/Futue Features
 
 __TODO:__
 
 * &#9745; Create a metrics fucntion to return
 * &#9745; Delete all private aand passwords being printed
@@ -541,14 +542,18 @@
   * &#9744; Logging metrics wrapper
 * &#9745; Create an average, mean, total time depending on calls being made for when you want to do a full list of keys
 * &#9745; Missing delete https action
 * &#9745; Create a download method to handle downlaoding files
 
 #### Release Notes
 
+#### v1.0.9
+
+* Fixed dependency issue.
+
 #### v1.0.8
 
 * Changed all timestamps to utc epoch float.
 * Updated formatting of logging.
 * Added easy_logger to help processs on screen and rotating log formats.
 * Added configuration for logger through a yaml configuration file.
 * Sets a default logger configuration if one isn't supplied in a config location area.
```

### Comparing `ciphertrust-sdk-1.0.8/README.md` & `ciphertrust-sdk-1.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -489,14 +489,15 @@
 | __1.0.7__ | __hotfix__ | Fixes issues with not raising proper errors when params are being passed |
 | __1.0.7__ | __feature__ | Adjusted and tested remaining http calls; see notes for details |
 | __1.0.7__ | __feature__ | Adjusted responses for all types of API calls |
 | __1.0.8__ | __a1__ | Added Error Response handling to ensure metrics in responses and error reporting; reformated logging messages and added splunk style logs with color responses |
 | __1.0.8__ | __a2__ | Added a 30s buffer to expiration of Auth Token |
 | __1.0.8__ | __a3__ | Synced error and standard format json response under response_statistics and request_parmeters |
 | __1.0.8__ | __final__ | Formated responses to return statatics on calls as well as data from call being made |
+| __1.0.9__ | __final__ | Added dependencies to requirements to fix installation issues |
 
 ### Known Bugs/Futue Features
 
 __TODO:__
 
 * &#9745; Create a metrics fucntion to return
 * &#9745; Delete all private aand passwords being printed
@@ -506,14 +507,18 @@
   * &#9744; Logging metrics wrapper
 * &#9745; Create an average, mean, total time depending on calls being made for when you want to do a full list of keys
 * &#9745; Missing delete https action
 * &#9745; Create a download method to handle downlaoding files
 
 #### Release Notes
 
+#### v1.0.9
+
+* Fixed dependency issue.
+
 #### v1.0.8
 
 * Changed all timestamps to utc epoch float.
 * Updated formatting of logging.
 * Added easy_logger to help processs on screen and rotating log formats.
 * Added configuration for logger through a yaml configuration file.
 * Sets a default logger configuration if one isn't supplied in a config location area.
```

### Comparing `ciphertrust-sdk-1.0.8/ciphertrust_sdk.egg-info/PKG-INFO` & `ciphertrust-sdk-1.0.9/ciphertrust_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciphertrust-sdk
-Version: 1.0.8
+Version: 1.0.9
 Summary: Thales CipherTrust SDK RestAPI
 Author-email: atav928 <dev@tavnets.com>
 License: MIT License
         
         Copyright (c) 2023 atav928
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -524,14 +524,15 @@
 | __1.0.7__ | __hotfix__ | Fixes issues with not raising proper errors when params are being passed |
 | __1.0.7__ | __feature__ | Adjusted and tested remaining http calls; see notes for details |
 | __1.0.7__ | __feature__ | Adjusted responses for all types of API calls |
 | __1.0.8__ | __a1__ | Added Error Response handling to ensure metrics in responses and error reporting; reformated logging messages and added splunk style logs with color responses |
 | __1.0.8__ | __a2__ | Added a 30s buffer to expiration of Auth Token |
 | __1.0.8__ | __a3__ | Synced error and standard format json response under response_statistics and request_parmeters |
 | __1.0.8__ | __final__ | Formated responses to return statatics on calls as well as data from call being made |
+| __1.0.9__ | __final__ | Added dependencies to requirements to fix installation issues |
 
 ### Known Bugs/Futue Features
 
 __TODO:__
 
 * &#9745; Create a metrics fucntion to return
 * &#9745; Delete all private aand passwords being printed
@@ -541,14 +542,18 @@
   * &#9744; Logging metrics wrapper
 * &#9745; Create an average, mean, total time depending on calls being made for when you want to do a full list of keys
 * &#9745; Missing delete https action
 * &#9745; Create a download method to handle downlaoding files
 
 #### Release Notes
 
+#### v1.0.9
+
+* Fixed dependency issue.
+
 #### v1.0.8
 
 * Changed all timestamps to utc epoch float.
 * Updated formatting of logging.
 * Added easy_logger to help processs on screen and rotating log formats.
 * Added configuration for logger through a yaml configuration file.
 * Sets a default logger configuration if one isn't supplied in a config location area.
```

### Comparing `ciphertrust-sdk-1.0.8/pyproject.toml` & `ciphertrust-sdk-1.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ciphertrust-sdk-1.0.8/src/ciphertrust/__init__.py` & `ciphertrust-sdk-1.0.9/src/ciphertrust/__init__.py`

 * *Files identical despite different names*

### Comparing `ciphertrust-sdk-1.0.8/src/ciphertrust/api.py` & `ciphertrust-sdk-1.0.9/src/ciphertrust/api.py`

 * *Files identical despite different names*

### Comparing `ciphertrust-sdk-1.0.8/src/ciphertrust/auth.py` & `ciphertrust-sdk-1.0.9/src/ciphertrust/auth.py`

 * *Files identical despite different names*

### Comparing `ciphertrust-sdk-1.0.8/src/ciphertrust/config.py` & `ciphertrust-sdk-1.0.9/src/ciphertrust/config.py`

 * *Files identical despite different names*

### Comparing `ciphertrust-sdk-1.0.8/src/ciphertrust/models.py` & `ciphertrust-sdk-1.0.9/src/ciphertrust/models.py`

 * *Files identical despite different names*

### Comparing `ciphertrust-sdk-1.0.8/src/ciphertrust/requestapi.py` & `ciphertrust-sdk-1.0.9/src/ciphertrust/requestapi.py`

 * *Files identical despite different names*

### Comparing `ciphertrust-sdk-1.0.8/src/ciphertrust/static.py` & `ciphertrust-sdk-1.0.9/src/ciphertrust/static.py`

 * *Files identical despite different names*

### Comparing `ciphertrust-sdk-1.0.8/src/ciphertrust/utils.py` & `ciphertrust-sdk-1.0.9/src/ciphertrust/utils.py`

 * *Files identical despite different names*

