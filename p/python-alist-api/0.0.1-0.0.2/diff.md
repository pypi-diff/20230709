# Comparing `tmp/python-alist-api-0.0.1.tar.gz` & `tmp/python-alist-api-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/devspace/python-alist-api/dist/.tmp-0xxmhdd7/python-alist-api-0.0.1.tar", last modified: Thu Jul  6 13:53:47 2023, max compression
+gzip compressed data, was "python-alist-api-0.0.2.tar", last modified: Sun Jul  9 09:06:05 2023, max compression
```

## Comparing `python-alist-api-0.0.1.tar` & `python-alist-api-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 pk        (1000) pk        (1000)        0 2023-07-06 13:53:47.866337 python-alist-api-0.0.1/
--rw-rw-r--   0 pk        (1000) pk        (1000)     1113 2023-07-06 13:44:59.000000 python-alist-api-0.0.1/LICENSE
--rw-rw-r--   0 pk        (1000) pk        (1000)     3414 2023-07-06 13:53:47.862337 python-alist-api-0.0.1/PKG-INFO
--rw-rw-r--   0 pk        (1000) pk        (1000)     1207 2023-07-06 13:12:38.000000 python-alist-api-0.0.1/README.md
-drwxrwxr-x   0 pk        (1000) pk        (1000)        0 2023-07-06 13:53:47.834337 python-alist-api-0.0.1/alist/
--rw-rw-r--   0 pk        (1000) pk        (1000)     5498 2023-07-03 12:58:57.000000 python-alist-api-0.0.1/alist/__init__.py
--rw-rw-r--   0 pk        (1000) pk        (1000)     4851 2023-07-03 15:12:02.000000 python-alist-api-0.0.1/alist/admin.py
--rw-rw-r--   0 pk        (1000) pk        (1000)     2093 2023-07-05 13:37:26.000000 python-alist-api-0.0.1/alist/public.py
--rw-rw-r--   0 pk        (1000) pk        (1000)    11129 2023-07-05 13:52:26.000000 python-alist-api-0.0.1/alist/setting.py
--rw-rw-r--   0 pk        (1000) pk        (1000)     6032 2023-07-06 13:49:39.000000 python-alist-api-0.0.1/pyproject.toml
-drwxrwxr-x   0 pk        (1000) pk        (1000)        0 2023-07-06 13:53:47.858337 python-alist-api-0.0.1/python_alist_api.egg-info/
--rw-rw-r--   0 pk        (1000) pk        (1000)     3414 2023-07-06 13:53:47.000000 python-alist-api-0.0.1/python_alist_api.egg-info/PKG-INFO
--rw-rw-r--   0 pk        (1000) pk        (1000)      297 2023-07-06 13:53:47.000000 python-alist-api-0.0.1/python_alist_api.egg-info/SOURCES.txt
--rw-rw-r--   0 pk        (1000) pk        (1000)        1 2023-07-06 13:53:47.000000 python-alist-api-0.0.1/python_alist_api.egg-info/dependency_links.txt
--rw-rw-r--   0 pk        (1000) pk        (1000)        9 2023-07-06 13:53:47.000000 python-alist-api-0.0.1/python_alist_api.egg-info/requires.txt
--rw-rw-r--   0 pk        (1000) pk        (1000)        6 2023-07-06 13:53:47.000000 python-alist-api-0.0.1/python_alist_api.egg-info/top_level.txt
--rw-rw-r--   0 pk        (1000) pk        (1000)       38 2023-07-06 13:53:47.866337 python-alist-api-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:06:05.300823 python-alist-api-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-09 09:05:55.000000 python-alist-api-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-07-09 09:06:05.300823 python-alist-api-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-09 09:05:55.000000 python-alist-api-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:06:05.300823 python-alist-api-0.0.2/alist/
+-rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-07-09 09:05:55.000000 python-alist-api-0.0.2/alist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-07-09 09:05:55.000000 python-alist-api-0.0.2/alist/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-09 09:05:55.000000 python-alist-api-0.0.2/alist/public.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11129 2023-07-09 09:05:55.000000 python-alist-api-0.0.2/alist/setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-07-09 09:05:55.000000 python-alist-api-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:06:05.300823 python-alist-api-0.0.2/python_alist_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-07-09 09:06:05.000000 python-alist-api-0.0.2/python_alist_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-09 09:06:05.000000 python-alist-api-0.0.2/python_alist_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 09:06:05.000000 python-alist-api-0.0.2/python_alist_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-09 09:06:05.000000 python-alist-api-0.0.2/python_alist_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-09 09:06:05.000000 python-alist-api-0.0.2/python_alist_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 09:06:05.300823 python-alist-api-0.0.2/setup.cfg
```

### Comparing `python-alist-api-0.0.1/LICENSE` & `python-alist-api-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-alist-api-0.0.1/PKG-INFO` & `python-alist-api-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-alist-api
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python wrapper for the Alist API
 Author-email: Kai Peng <pkemb@outlook.com>
 Maintainer-email: Kai Peng <pkemb@outlook.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Kai Peng, https://pkemb.com <pkemb@outlook.com>
```

### Comparing `python-alist-api-0.0.1/README.md` & `python-alist-api-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `python-alist-api-0.0.1/alist/__init__.py` & `python-alist-api-0.0.2/alist/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Kai Peng
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 
 from requests import Session
 from requests import HTTPError
 import json
 from urllib.parse import urlparse
 from alist.public import AlistPublic
 from alist.admin import AlistAdmin
@@ -18,20 +18,24 @@
     Python wrapper for the Alist API.
     """
     def __init__(
         self,
         base_url,
         password = None,
         authorization = None,
+        ssl_verify = True,
+        cert = None,
     ):
         self.base_url = base_url.rstrip('/')
         self.public = AlistPublic(self)
         self.admin  = None
         self.session = Session()
         self.password = ""
+        self.ssl_verify = ssl_verify
+        self.cert = cert
 
         self.url = urlparse(self.base_url)
 
         self.authorization = None
         self.login(password, authorization)
 
     def calc_authorization(self, password):
@@ -115,14 +119,17 @@
             # "Content-Type": "application/json;charset=UTF-8", # requests 自动填充
         }
         request_kwargs = kwargs
         if "headers" in request_kwargs:
             request_kwargs["headers"].update(headers)
         else:
             request_kwargs["headers"] = headers
+        request_kwargs['verify'] = self.ssl_verify
+        request_kwargs['cert']   = self.cert
+
         return request_kwargs
 
     def get_api_url(self, endpoint):
         """
         Return the api url including host and port for a given endpoint.
         :param endpoint: service endpoint as str
         :return: api url (including host and port) as str
```

### Comparing `python-alist-api-0.0.1/alist/admin.py` & `python-alist-api-0.0.2/alist/admin.py`

 * *Files identical despite different names*

### Comparing `python-alist-api-0.0.1/alist/public.py` & `python-alist-api-0.0.2/alist/public.py`

 * *Files identical despite different names*

### Comparing `python-alist-api-0.0.1/alist/setting.py` & `python-alist-api-0.0.2/alist/setting.py`

 * *Files identical despite different names*

### Comparing `python-alist-api-0.0.1/pyproject.toml` & `python-alist-api-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python-alist-api-0.0.1/python_alist_api.egg-info/PKG-INFO` & `python-alist-api-0.0.2/python_alist_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-alist-api
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python wrapper for the Alist API
 Author-email: Kai Peng <pkemb@outlook.com>
 Maintainer-email: Kai Peng <pkemb@outlook.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Kai Peng, https://pkemb.com <pkemb@outlook.com>
```

