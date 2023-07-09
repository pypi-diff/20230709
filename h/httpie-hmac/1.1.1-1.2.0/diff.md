# Comparing `tmp/httpie-hmac-1.1.1.tar.gz` & `tmp/httpie-hmac-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpie-hmac-1.1.1.tar", last modified: Fri Apr  7 20:46:39 2023, max compression
+gzip compressed data, was "httpie-hmac-1.2.0.tar", last modified: Sun Jul  9 20:02:43 2023, max compression
```

## Comparing `httpie-hmac-1.1.1.tar` & `httpie-hmac-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:46:39.174649 httpie-hmac-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-07 20:46:30.000000 httpie-hmac-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-04-07 20:46:39.174649 httpie-hmac-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-04-07 20:46:30.000000 httpie-hmac-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:46:39.170649 httpie-hmac-1.1.1/httpie_hmac/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-07 20:46:30.000000 httpie-hmac-1.1.1/httpie_hmac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-04-07 20:46:30.000000 httpie-hmac-1.1.1/httpie_hmac/httpie_hmac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:46:39.174649 httpie-hmac-1.1.1/httpie_hmac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-04-07 20:46:39.000000 httpie-hmac-1.1.1/httpie_hmac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-07 20:46:39.000000 httpie-hmac-1.1.1/httpie_hmac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 20:46:39.000000 httpie-hmac-1.1.1/httpie_hmac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-07 20:46:39.000000 httpie-hmac-1.1.1/httpie_hmac.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-07 20:46:39.000000 httpie-hmac-1.1.1/httpie_hmac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-07 20:46:39.000000 httpie-hmac-1.1.1/httpie_hmac.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-07 20:46:30.000000 httpie-hmac-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 20:46:39.174649 httpie-hmac-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:02:43.860407 httpie-hmac-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-09 20:02:34.000000 httpie-hmac-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-09 20:02:43.860407 httpie-hmac-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-07-09 20:02:34.000000 httpie-hmac-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:02:43.856407 httpie-hmac-1.2.0/httpie_hmac/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-09 20:02:34.000000 httpie-hmac-1.2.0/httpie_hmac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-07-09 20:02:34.000000 httpie-hmac-1.2.0/httpie_hmac/httpie_hmac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:02:43.860407 httpie-hmac-1.2.0/httpie_hmac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-09 20:02:43.000000 httpie-hmac-1.2.0/httpie_hmac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-09 20:02:43.000000 httpie-hmac-1.2.0/httpie_hmac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 20:02:43.000000 httpie-hmac-1.2.0/httpie_hmac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-09 20:02:43.000000 httpie-hmac-1.2.0/httpie_hmac.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-09 20:02:43.000000 httpie-hmac-1.2.0/httpie_hmac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-09 20:02:43.000000 httpie-hmac-1.2.0/httpie_hmac.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-09 20:02:34.000000 httpie-hmac-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 20:02:43.860407 httpie-hmac-1.2.0/setup.cfg
```

### Comparing `httpie-hmac-1.1.1/LICENSE` & `httpie-hmac-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `httpie-hmac-1.1.1/PKG-INFO` & `httpie-hmac-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpie-hmac
-Version: 1.1.1
+Version: 1.2.0
 Summary: HMAC Auth Plugin for Httpie
 Author-email: Martyn Pittuck-Schols <martyn@rustfoo.com>
 License: MIT
 Project-URL: homepage, https://github.com/martynp/httpie-hmac/
 Project-URL: repository, https://github.com/martynp/httpie-hmac.git
 Keywords: httpie,auth,hmac,aws4
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `httpie-hmac-1.1.1/README.md` & `httpie-hmac-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `httpie-hmac-1.1.1/httpie_hmac/httpie_hmac.py` & `httpie-hmac-1.2.0/httpie_hmac/httpie_hmac.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 """
 import base64
 import datetime
 import hashlib
 import hmac
 import importlib.machinery
+import io
 import os
 import requests
 import types
 
 from aws_requests_auth.aws_auth import AWSRequestsAuth
 from dataclasses import dataclass
 from urllib.parse import urlparse
@@ -139,34 +140,48 @@
         # Method (GET, POST etc)
         method = r.method
 
         # Content type (e.g. application-json)
         content_type = r.headers.get('content-type')
         if not content_type:
             content_type = ''
+        else:
+            content_type = content_type.decode('utf-8')
 
         # If content-md5 is already given, use it, otherwise calculate
         # it ourselves and add it to the headers
         content_md5 = r.headers.get('content-md5')
         if not content_md5:
             if content_type and r.body:
                 m = hashlib.md5()
+                body = r.body
+                # If we have a buffer, convert it in to a string
+                if type(r.body) == io.BufferedReader:
+                    body = body.read()
+                    r.body = body
                 m.update(r.body)
-                content_md5 = base64.b64encode(m.digest()).rstrip()
+                content_md5 = base64 \
+                    .b64encode(m.digest()) \
+                    .rstrip() \
+                    .decode('utf-8')
                 r.headers['Content-MD5'] = content_md5
             else:
                 content_md5 = ''
+        else:
+            content_md5 = content_md5.decode('utf-8')
 
         # If date is given already, use it - otherwise generate it
         # ourselves and add it to the headers
         http_date = r.headers.get('date')
         if not http_date:
             now = datetime.datetime.utcnow()
             http_date = now.strftime('%a, %d %b %Y %H:%M:%S GMT')
             r.headers['Date'] = http_date
+        else:
+            http_date = http_date.decode('utf-8')
 
         # Get the path from the UL
         url = urlparse(r.url)
         path = url.path
 
         # Call the formatter to add the required headers and return r
         return self.formatter.generate(
```

### Comparing `httpie-hmac-1.1.1/httpie_hmac.egg-info/PKG-INFO` & `httpie-hmac-1.2.0/httpie_hmac.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpie-hmac
-Version: 1.1.1
+Version: 1.2.0
 Summary: HMAC Auth Plugin for Httpie
 Author-email: Martyn Pittuck-Schols <martyn@rustfoo.com>
 License: MIT
 Project-URL: homepage, https://github.com/martynp/httpie-hmac/
 Project-URL: repository, https://github.com/martynp/httpie-hmac.git
 Keywords: httpie,auth,hmac,aws4
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `httpie-hmac-1.1.1/pyproject.toml` & `httpie-hmac-1.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "httpie-hmac"
-version = "1.1.1"
+version = "1.2.0"
 authors = [
     {name = "Martyn Pittuck-Schols", email = "martyn@rustfoo.com"},
 ]
 description = "HMAC Auth Plugin for Httpie"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["httpie", "auth", "hmac", "aws4"]
```

