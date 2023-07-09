# Comparing `tmp/mailpit-api-client-0.12.1.tar.gz` & `tmp/mailpit-api-client-0.12.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mailpit-api-client-0.12.1.tar", last modified: Sun Jul  9 12:49:58 2023, max compression
+gzip compressed data, was "mailpit-api-client-0.12.2.tar", last modified: Sun Jul  9 14:22:45 2023, max compression
```

## Comparing `mailpit-api-client-0.12.1.tar` & `mailpit-api-client-0.12.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:49:58.322992 mailpit-api-client-0.12.1/
--rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-07-09 12:49:31.000000 mailpit-api-client-0.12.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-07-09 12:49:58.322992 mailpit-api-client-0.12.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-07-09 12:49:31.000000 mailpit-api-client-0.12.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:49:58.318992 mailpit-api-client-0.12.1/mailpit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 12:49:31.000000 mailpit-api-client-0.12.1/mailpit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:49:58.318992 mailpit-api-client-0.12.1/mailpit/client/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-09 12:49:31.000000 mailpit-api-client-0.12.1/mailpit/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-07-09 12:49:31.000000 mailpit-api-client-0.12.1/mailpit/client/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12160 2023-07-09 12:49:31.000000 mailpit-api-client-0.12.1/mailpit/client/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-09 12:49:31.000000 mailpit-api-client-0.12.1/mailpit/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:49:58.318992 mailpit-api-client-0.12.1/mailpit/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 12:49:31.000000 mailpit-api-client-0.12.1/mailpit/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-09 12:49:31.000000 mailpit-api-client-0.12.1/mailpit/testing/pytest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-09 12:49:31.000000 mailpit-api-client-0.12.1/mailpit/testing/unittest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:49:58.322992 mailpit-api-client-0.12.1/mailpit_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-07-09 12:49:58.000000 mailpit-api-client-0.12.1/mailpit_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-09 12:49:58.000000 mailpit-api-client-0.12.1/mailpit_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 12:49:58.000000 mailpit-api-client-0.12.1/mailpit_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-09 12:49:58.000000 mailpit-api-client-0.12.1/mailpit_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-09 12:49:58.000000 mailpit-api-client-0.12.1/mailpit_api_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-07-09 12:49:31.000000 mailpit-api-client-0.12.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 12:49:58.322992 mailpit-api-client-0.12.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:22:45.496074 mailpit-api-client-0.12.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-07-09 14:22:25.000000 mailpit-api-client-0.12.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-07-09 14:22:45.496074 mailpit-api-client-0.12.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-07-09 14:22:25.000000 mailpit-api-client-0.12.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:22:45.496074 mailpit-api-client-0.12.2/mailpit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 14:22:25.000000 mailpit-api-client-0.12.2/mailpit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:22:45.496074 mailpit-api-client-0.12.2/mailpit/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-09 14:22:25.000000 mailpit-api-client-0.12.2/mailpit/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-07-09 14:22:25.000000 mailpit-api-client-0.12.2/mailpit/client/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12160 2023-07-09 14:22:25.000000 mailpit-api-client-0.12.2/mailpit/client/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-09 14:22:25.000000 mailpit-api-client-0.12.2/mailpit/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:22:45.496074 mailpit-api-client-0.12.2/mailpit/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 14:22:25.000000 mailpit-api-client-0.12.2/mailpit/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-09 14:22:25.000000 mailpit-api-client-0.12.2/mailpit/testing/pytest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-09 14:22:25.000000 mailpit-api-client-0.12.2/mailpit/testing/unittest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:22:45.496074 mailpit-api-client-0.12.2/mailpit_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-07-09 14:22:45.000000 mailpit-api-client-0.12.2/mailpit_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-09 14:22:45.000000 mailpit-api-client-0.12.2/mailpit_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 14:22:45.000000 mailpit-api-client-0.12.2/mailpit_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-09 14:22:45.000000 mailpit-api-client-0.12.2/mailpit_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-09 14:22:45.000000 mailpit-api-client-0.12.2/mailpit_api_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-07-09 14:22:25.000000 mailpit-api-client-0.12.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 14:22:45.496074 mailpit-api-client-0.12.2/setup.cfg
```

### Comparing `mailpit-api-client-0.12.1/LICENSE` & `mailpit-api-client-0.12.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mailpit-api-client-0.12.1/PKG-INFO` & `mailpit-api-client-0.12.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailpit-api-client
-Version: 0.12.1
+Version: 0.12.2
 Summary: A Mailpit API Client
 Author-email: Lars Liedtke <lars@familie-liedtke.net>
 License: GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -198,15 +198,15 @@
 -------------------------------------------------------------------
 API-client for https://github.com/axllent/mailpit written in Python
 -------------------------------------------------------------------
 
 :Authors:
     Lars Liedtke <corvan@gmx.de>
 :Version:
-    0.12.1
+    0.12.2
 
 Go to the `documentation <https://corvan.github.io/mailpit-api-client/>`_
 
 ----------
 Motivation
 ----------
 For work, I thought about introducing integration testing.
```

### Comparing `mailpit-api-client-0.12.1/README.rst` & `mailpit-api-client-0.12.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 -------------------------------------------------------------------
 API-client for https://github.com/axllent/mailpit written in Python
 -------------------------------------------------------------------
 
 :Authors:
     Lars Liedtke <corvan@gmx.de>
 :Version:
-    0.12.1
+    0.12.2
 
 Go to the `documentation <https://corvan.github.io/mailpit-api-client/>`_
 
 ----------
 Motivation
 ----------
 For work, I thought about introducing integration testing.
```

### Comparing `mailpit-api-client-0.12.1/mailpit/client/api.py` & `mailpit-api-client-0.12.2/mailpit/client/api.py`

 * *Files identical despite different names*

### Comparing `mailpit-api-client-0.12.1/mailpit/client/models.py` & `mailpit-api-client-0.12.2/mailpit/client/models.py`

 * *Files identical despite different names*

### Comparing `mailpit-api-client-0.12.1/mailpit/testing/pytest.py` & `mailpit-api-client-0.12.2/mailpit/testing/pytest.py`

 * *Files identical despite different names*

### Comparing `mailpit-api-client-0.12.1/mailpit/testing/unittest.py` & `mailpit-api-client-0.12.2/mailpit/testing/unittest.py`

 * *Files identical despite different names*

### Comparing `mailpit-api-client-0.12.1/mailpit_api_client.egg-info/PKG-INFO` & `mailpit-api-client-0.12.2/mailpit_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailpit-api-client
-Version: 0.12.1
+Version: 0.12.2
 Summary: A Mailpit API Client
 Author-email: Lars Liedtke <lars@familie-liedtke.net>
 License: GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -198,15 +198,15 @@
 -------------------------------------------------------------------
 API-client for https://github.com/axllent/mailpit written in Python
 -------------------------------------------------------------------
 
 :Authors:
     Lars Liedtke <corvan@gmx.de>
 :Version:
-    0.12.1
+    0.12.2
 
 Go to the `documentation <https://corvan.github.io/mailpit-api-client/>`_
 
 ----------
 Motivation
 ----------
 For work, I thought about introducing integration testing.
```

### Comparing `mailpit-api-client-0.12.1/pyproject.toml` & `mailpit-api-client-0.12.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mailpit-api-client"
-version = "0.12.1"
+version = "0.12.2"
 description = "A Mailpit API Client"
 authors = [{name = "Lars Liedtke", email = "lars@familie-liedtke.net"}]
 requires-python = ">=3.8"
 readme = "README.rst"
 license = {file = "LICENSE"}
 classifiers = [
     "Framework :: Pytest",
@@ -93,16 +93,16 @@
 python_versions = [
     "3.9",
     "3.10",
     "3.11",
     "3.12-rc"
 ]
 debian_codenames = [
-    "buster",
     "bullseye",
+    "bookworm"
 ]
 
 checkers = [
     "black",
     "lint",
     "mypy"
 ]
```

