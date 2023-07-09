# Comparing `tmp/py115-0.0.1.tar.gz` & `tmp/py115-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py115-0.0.1.tar", last modified: Thu May 25 13:02:54 2023, max compression
+gzip compressed data, was "py115-0.0.2.tar", last modified: Sun Jul  9 10:34:09 2023, max compression
```

## Comparing `py115-0.0.1.tar` & `py115-0.0.2.tar`

### file list

```diff
@@ -1,42 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:02:54.907670 py115-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-25 13:02:41.000000 py115-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-05-25 13:02:54.907670 py115-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-25 13:02:41.000000 py115-0.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:02:54.899670 py115-0.0.1/py115/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-25 13:02:41.000000 py115-0.0.1/py115/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:02:54.903670 py115-0.0.1/py115/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 13:02:41.000000 py115-0.0.1/py115/_internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:02:54.903670 py115-0.0.1/py115/_internal/api/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 13:02:41.000000 py115-0.0.1/py115/_internal/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-25 13:02:41.000000 py115-0.0.1/py115/_internal/api/dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-25 13:02:41.000000 py115-0.0.1/py115/_internal/api/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-25 13:02:41.000000 py115-0.0.1/py115/_internal/api/offline.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-25 13:02:41.000000 py115-0.0.1/py115/_internal/api/space.py
--rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-05-25 13:02:41.000000 py115-0.0.1/py115/_internal/api/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-25 13:02:41.000000 py115-0.0.1/py115/_internal/api/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-25 13:02:41.000000 py115-0.0.1/py115/_internal/api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:02:54.903670 py115-0.0.1/py115/_internal/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 13:02:41.000000 py115-0.0.1/py115/_internal/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-25 13:02:41.000000 py115-0.0.1/py115/_internal/crypto/_rsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-25 13:02:41.000000 py115-0.0.1/py115/_internal/crypto/_xor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-05-25 13:02:41.000000 py115-0.0.1/py115/_internal/crypto/ec115.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-25 13:02:41.000000 py115-0.0.1/py115/_internal/crypto/m115.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-25 13:02:41.000000 py115-0.0.1/py115/_internal/oss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:02:54.907670 py115-0.0.1/py115/_internal/protocol/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 13:02:41.000000 py115-0.0.1/py115/_internal/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-25 13:02:41.000000 py115-0.0.1/py115/_internal/protocol/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-05-25 13:02:41.000000 py115-0.0.1/py115/_internal/protocol/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-25 13:02:41.000000 py115-0.0.1/py115/_internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-05-25 13:02:41.000000 py115-0.0.1/py115/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-05-25 13:02:41.000000 py115-0.0.1/py115/services.py
--rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-05-25 13:02:41.000000 py115-0.0.1/py115/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:02:54.899670 py115-0.0.1/py115.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-05-25 13:02:54.000000 py115-0.0.1/py115.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-25 13:02:54.000000 py115-0.0.1/py115.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 13:02:54.000000 py115-0.0.1/py115.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-25 13:02:54.000000 py115-0.0.1/py115.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-25 13:02:54.000000 py115-0.0.1/py115.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-25 13:02:41.000000 py115-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-25 13:02:41.000000 py115-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 13:02:54.907670 py115-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-25 13:02:41.000000 py115-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:34:09.537325 py115-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-09 10:33:59.000000 py115-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-09 10:34:09.537325 py115-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-09 10:33:59.000000 py115-0.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:34:09.533325 py115-0.0.2/py115/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-09 10:33:59.000000 py115-0.0.2/py115/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:34:09.537325 py115-0.0.2/py115/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:34:09.537325 py115-0.0.2/py115/_internal/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/api/dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/api/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/api/m115.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/api/offline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/api/qrcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/api/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/api/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:34:09.537325 py115-0.0.2/py115/_internal/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/crypto/_rsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/crypto/_xor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/crypto/ec115.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/crypto/m115.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/oss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:34:09.537325 py115-0.0.2/py115/_internal/protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/protocol/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/protocol/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-09 10:33:59.000000 py115-0.0.2/py115/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-09 10:33:59.000000 py115-0.0.2/py115/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9769 2023-07-09 10:33:59.000000 py115-0.0.2/py115/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-09 10:33:59.000000 py115-0.0.2/py115/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:34:09.533325 py115-0.0.2/py115.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-09 10:34:09.000000 py115-0.0.2/py115.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-09 10:34:09.000000 py115-0.0.2/py115.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 10:34:09.000000 py115-0.0.2/py115.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-09 10:34:09.000000 py115-0.0.2/py115.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-09 10:34:09.000000 py115-0.0.2/py115.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-09 10:33:59.000000 py115-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-09 10:33:59.000000 py115-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 10:34:09.537325 py115-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-09 10:33:59.000000 py115-0.0.2/setup.py
```

### Comparing `py115-0.0.1/LICENSE` & `py115-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py115-0.0.1/PKG-INFO` & `py115-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py115
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python SDK for 115 cloud storage service.
 Author-email: deadblue <public@dead.blue>
 License: MIT License
         
         Copyright 2023 deadblue
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of 
@@ -43,18 +43,23 @@
 An API client of 115 cloud storage service.
 
 Install
 =======
 
 .. code:: shell
 
+    # Install from PyPI
+    pip install py115
+
+    # Or install from source
     pip install git+https://github.com/deadblue/py115.git
 
-Example
-=======
+
+Usage
+=====
 
 .. code:: python
 
     import py115
     from py115.types import Credentail
 
     # Connect to cloud
@@ -77,7 +82,19 @@
         print('Task: %r' % task)
     # Add task by download URLs
     offline.add_url(
         'magnet:?xt=urn:btih:000123456789abcdef1151150123456789abcdef',
         'ed2k://|file|ED2k-file|115115115|1234567890abcdef1234567890abcdef|/',
         'https://dl.some-server.com/some/file.ext'
     )
+
+
+Document
+========
+
+https://py115.readthedocs.io/en/stable/
+
+
+License
+=======
+
+MIT
```

### Comparing `py115-0.0.1/README.rst` & `py115-0.0.2/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -5,18 +5,23 @@
 An API client of 115 cloud storage service.
 
 Install
 =======
 
 .. code:: shell
 
+    # Install from PyPI
+    pip install py115
+
+    # Or install from source
     pip install git+https://github.com/deadblue/py115.git
 
-Example
-=======
+
+Usage
+=====
 
 .. code:: python
 
     import py115
     from py115.types import Credentail
 
     # Connect to cloud
@@ -39,7 +44,19 @@
         print('Task: %r' % task)
     # Add task by download URLs
     offline.add_url(
         'magnet:?xt=urn:btih:000123456789abcdef1151150123456789abcdef',
         'ed2k://|file|ED2k-file|115115115|1234567890abcdef1234567890abcdef|/',
         'https://dl.some-server.com/some/file.ext'
     )
+
+
+Document
+========
+
+https://py115.readthedocs.io/en/stable/
+
+
+License
+=======
+
+MIT
```

### Comparing `py115-0.0.1/py115/__init__.py` & `py115-0.0.2/py115/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 storage = cloud.storage()
 
 for file in storage.list():
     print(f'File: {file.name}')
 
 """
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 
 import py115.cloud
 import py115.types
 
 def connect(
         credential: py115.types.Credential = None,
         protocol_kwargs: dict=  None
```

### Comparing `py115-0.0.1/py115/_internal/api/dir.py` & `py115-0.0.2/py115/_internal/api/dir.py`

 * *Files identical despite different names*

### Comparing `py115-0.0.1/py115/_internal/api/file.py` & `py115-0.0.2/py115/_internal/api/file.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 __author__ = 'deadblue'
 
 import time
 import typing
 
+from py115._internal.api import m115
 from py115._internal.protocol import api
 
 
 class ListApi(api.ApiSpec):
 
     def __init__(self, dir_id: str) -> None:
         super().__init__(None)
@@ -27,15 +28,15 @@
     def url(self) -> str:
         order = self._qs.get('o')
         if order == 'file_name':
             return 'https://aps.115.com/natsort/files.php'
         else:
             return 'https://webapi.115.com/files'
 
-    def parse_result(self, result: dict):
+    def parse_result(self, result: dict) -> dict:
         if result.get('state', False):
             return {
                 'count': result.get('count'),
                 'offset': result.get('offset'),
                 'files': result.get('data')
             }
         else:
@@ -51,14 +52,43 @@
 
     def set_offset(self, offset: int):
         self.update_qs({
             'offset': str(offset)
         })
 
 
+class SearchApi(api.ApiSpec):
+
+    def __init__(self, keyword: str, dir_id: str) -> None:
+        super().__init__('https://webapi.115.com/files/search')
+        self.update_qs({
+            'aid': '1',
+            'cid': dir_id,
+            'offset': '0',
+            'limit': '115',
+            'format': 'json',
+            'search_value': keyword
+        })
+    
+    def parse_result(self, result: dict) -> dict:
+        if result.get('state', False):
+            return {
+                'count': result.get('count'),
+                'offset': result.get('offset'),
+                'files': result.get('data')
+            }
+        else:
+            raise api.ApiException(api.find_error_code(result))
+
+    def set_offset(self, offset: int):
+        self.update_qs({
+            'offset': str(offset)
+        })
+
+
 class DeleteApi(api.ApiSpec):
 
     def __init__(self, file_ids: typing.Iterable[str]) -> None:
         super().__init__('https://webapi.115.com/rb/delete')
         self.update_from({
             'fid': file_ids,
             'ignore_warn': '1'
@@ -81,15 +111,15 @@
         super().__init__('https://webapi.115.com/files/batch_rename')
         key = 'files_new_name[%s]' % file_id
         self.update_from({
             key: new_name
         })
 
 
-class DownloadApi(api.M115ApiSpec):
+class DownloadApi(m115.M115ApiSpec):
 
     def __init__(self, pickcode: str) -> None:
         super().__init__('https://proapi.115.com/app/chrome/downurl', True)
         self.update_qs({
             't': int(time.time())
         })
         self.update_from({
@@ -97,14 +127,29 @@
         })
 
     def parse_result(self, result: dict):
         result = super().parse_result(result)
         if len(result) == 0:
             return None
         file_id, down_info = result.popitem()
-        result = {
-            'file_id': file_id,
-            'file_name': down_info['file_name'],
-            'fize_size': int(down_info['file_size']),
-            'url': down_info['url']['url'].replace('http://', 'https://')
-        }
-        return result
+        if 'url' in down_info and isinstance(down_info['url'], dict):
+            return {
+                'file_id': file_id,
+                'file_name': down_info['file_name'],
+                'fize_size': int(down_info['file_size']),
+                'url': down_info['url']['url'].replace('http://', 'https://')
+            }
+        else:
+            return None
+
+
+class VideoApi(api.ApiSpec):
+
+    def __init__(self, pickcode: str) -> None:
+        super().__init__('https://webapi.115.com/files/video', False)
+        self.update_qs({'pickcode': pickcode})
+    
+    def parse_result(self, result: dict) -> str:
+        err_code = api.find_error_code(result)
+        if err_code != 0:
+            raise api.ApiException(code=err_code)
+        return result.get('video_url')
```

### Comparing `py115-0.0.1/py115/_internal/api/offline.py` & `py115-0.0.2/py115/_internal/api/offline.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 __author__ = 'deadblue'
 
 import typing
 
+from py115._internal.api import m115
 from py115._internal.protocol import api
 
 
 class ListApi(api.ApiSpec):
     
     def __init__(self, page: int = 1) -> None:
         super().__init__('https://lixian.115.com/lixian/', True)
@@ -56,15 +57,15 @@
             'ac': 'task_clear'
         })
         self.update_from({
             'flag': flag
         })
 
 
-class AddUrlsApi(api.M115ApiSpec):
+class AddUrlsApi(m115.M115ApiSpec):
     
     def __init__(self, app_ver: str, user_id: int, urls: typing.Iterable[str], **kwargs) -> None:
         super().__init__('https://lixian.115.com/lixianssp/', True)
         self.update_qs({
             'ac': 'add_task_urls'
         })
         params = {
```

### Comparing `py115-0.0.1/py115/_internal/api/upload.py` & `py115-0.0.2/py115/_internal/api/upload.py`

 * *Files identical despite different names*

### Comparing `py115-0.0.1/py115/_internal/crypto/_rsa.py` & `py115-0.0.2/py115/_internal/crypto/_rsa.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             plaintext = plaintext[slice_size:]
             remain_size -= slice_size
         return bytes(ciphertext)
 
 
     def _decrypt_slice(self, segment: bytes) -> bytes:
         msg = int.from_bytes(segment, 'big')
-        ret = pow(msg, self._e, self._n).to_bytes(self._key_len)
+        ret = pow(msg, self._e, self._n).to_bytes(self._key_len, 'big')
         for i, b in enumerate(ret):
             if i != 0 and b == 0:
                 ret = ret[i+1:]
                 break
         return ret
```

### Comparing `py115-0.0.1/py115/_internal/crypto/_xor.py` & `py115-0.0.2/py115/_internal/crypto/_xor.py`

 * *Files identical despite different names*

### Comparing `py115-0.0.1/py115/_internal/crypto/ec115.py` & `py115-0.0.2/py115/_internal/crypto/ec115.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         # Generate client key
         client_key = ECC.generate(curve=_curve_name)
         # Export client public key
         self._pub_key = b'\x1d' + client_key.public_key().export_key(
             format='SEC1', compress=True
         )
         # ECDH key exchange
-        shared_secret = (server_key.pointQ * client_key.d).x.to_bytes(28)
+        shared_secret = (server_key.pointQ * client_key.d).x.to_bytes(28, 'big')
         self._aes_key = shared_secret[:16]
         self._aes_iv = shared_secret[-16:]
     
     def encode_token(self, timestamp: int) -> str:
         token = bytearray(struct.pack(
             '<15sBII15sBI',
             self._pub_key[:15], 0, 115, timestamp,
```

### Comparing `py115-0.0.1/py115/_internal/crypto/m115.py` & `py115-0.0.2/py115/_internal/crypto/m115.py`

 * *Files identical despite different names*

### Comparing `py115-0.0.1/py115/_internal/protocol/api.py` & `py115-0.0.2/py115/_internal/protocol/api.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 __author__ = 'deadblue'
 
-import json
 import random
 import typing
 import urllib.parse
 
-from py115._internal.crypto import m115
-
 
 class ApiException(Exception):
 
     def __init__(self, code: int, *args: object) -> None:
         super().__init__(*args)
         self._code = code
     
@@ -103,25 +100,7 @@
         if error_code == 0:
             return None
         else:
             raise ApiException(error_code)
 
     def get_delay(self) -> float:
         return random.randint(100, 500) / 1000.0
-
-class M115ApiSpec(ApiSpec):
-
-    def __init__(self, url: str, use_ec: bool = False) -> None:
-        super().__init__(url, use_ec)
-        self._m_key = m115.generate_key()
-
-    @property
-    def payload(self) -> bytes:
-        data = m115.encode(self._m_key, json.dumps(self._form))
-        return urllib.parse.urlencode({
-            'data': data
-        }).encode()
-
-    def parse_result(self, result: dict):
-        data = super().parse_result(result)
-        # M115 decode
-        return json.loads(m115.decode(self._m_key, data))
```

### Comparing `py115-0.0.1/py115/_internal/protocol/client.py` & `py115-0.0.2/py115/_internal/protocol/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,7 +117,11 @@
             self._next_request_time = time.time() + spec.get_delay()
         if spec.use_ec:
             result = json.loads(self._ecc.decode(resp.content))
         else:
             result = resp.json()
         _logger.debug('API result: %r', result)
         return spec.parse_result(result)
+
+    def fetch(self, url: str) -> bytes:
+        resp = self._session.get(url)
+        return resp.content
```

### Comparing `py115-0.0.1/py115/_internal/utils.py` & `py115-0.0.2/py115/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `py115-0.0.1/py115/cloud.py` & `py115-0.0.2/py115/cloud.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 __author__ = 'deadblue'
 
 import typing
 
 from py115._internal.protocol.client import Client
-from py115._internal.api import upload, version
+from py115._internal.api import qrcode, upload, version
 
-from py115 import services
-from py115.types import Credential
+from py115 import login, services
+from py115.types import Credential, LoginPlatform
 
 
-class Cloud:
+class Cloud(login._Handler):
     """115 cloud service.
 
     Args:
         credential (py115.types.Credential): Credential object.
         protocol_kwargs (dict): Settings for underlying protocol client.
     """
 
@@ -44,35 +44,56 @@
         Args:
             credential (py115.types.Credential): Credential object to identity user.
 
         Return:
             bool: Is credential valid.
         """
         self._client.import_cookies(credential.to_dict())
-        try:
-        # Initialize upload helper
-            user_id, user_key = self._client.execute_api(upload.InfoApi())
-            self._upload_helper = upload.Helper(
-                self._app_ver, user_id, user_key
-            )
-            return True
-        except:
-            return False
+        return self._on_login()
 
     def export_credentail(self) -> typing.Union[Credential, None]:
         """Export current credentail from cloud instance.
 
         Return:
             py115.types.Credential: Credential object, or None when credential is invalid.
         """
         # TODO: Check credential before return.
         return Credential.from_dict(
             self._client.export_cookies()
         )
 
+    def qrcode_login(self, platform: LoginPlatform) -> login.QrcodeSession:
+        """Start QRcode login session.
+
+        Args:
+            platform (py115.types.LoginPlatform): Platform to login.
+
+        Returns:
+            py115.login.QrcodeSession: QRcode login session.
+        """
+        token = self._client.execute_api(qrcode.TokenApi(platform.value))
+        return login.QrcodeSession._create(
+            client=self._client,
+            handler=self,
+            platform=platform.value,
+            uid=token.get('uid'), 
+            time=token.get('time'),
+            sign=token.get('sign')
+        )
+
+    def _on_login(self) -> bool:
+        try:
+            user_id, user_key = self._client.execute_api(upload.InfoApi())
+            self._upload_helper = upload.Helper(
+                self._app_ver, user_id, user_key
+            )
+            return True
+        except:
+            return False
+
     def offline(self) -> services.OfflineService:
         """Get offline service.
 
         Return:
             py115.services.OfflineService: Offline service instance.
         """
         return services.OfflineService._create(
```

### Comparing `py115-0.0.1/py115/services.py` & `py115-0.0.2/py115/services.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 import os
 import os.path
 import typing
 
 from py115._internal.api import offline, file, dir, space, upload
 from py115._internal.protocol.client import Client
 
-from py115.types import TaskStatus, Task, File, DownloadTicket, UploadTicket
+from py115 import types
 
 
 _CLEAR_FLAG_MAPPING = {
-    TaskStatus.Complete: 1,
-    TaskStatus.Failed: 2,
-    TaskStatus.Running: 3
+    types.TaskStatus.Complete: 1,
+    types.TaskStatus.Failed: 2,
+    types.TaskStatus.Running: 3
 }
 
 
 class OfflineService:
     """Offline task manager."""
 
     _client: Client = None
@@ -28,58 +28,58 @@
     def _create(cls, client: Client, app_ver: str, user_id: str):
         s = cls()
         s._client = client
         s._app_ver = app_ver
         s._user_id = user_id
         return s
 
-    def list(self) -> typing.Generator[Task, None, None]:
+    def list(self) -> typing.Generator[types.Task, None, None]:
         """Get all tasks.
 
         Yields:
             py115.types.Task: Task object
         """
         spec = offline.ListApi()
         while True:
             result = self._client.execute_api(spec)
             for t in result['tasks']:
-                yield Task._create(t)
+                yield types.Task._create(t)
             page, page_count = result['page'], result['page_count']
             if page < page_count:
                 spec.set_page(page + 1)
             else:
                 break
 
-    def add_url(self, *urls: str) -> typing.Iterable[Task]:
+    def add_url(self, *urls: str) -> typing.Iterable[types.Task]:
         """Create task(s) from download URL.
 
         Args:
             *urls (str): Download URL, can be a http/ftp/ed2k/magnet link.
 
         Return:
             Iterable[py115.types.Task]: Task list for the download URLs.
         """
         if len(urls) == 0:
             return []
         add_results = self._client.execute_api(offline.AddUrlsApi(
             self._app_ver, self._user_id, urls
         ))
-        return [Task._create(r) for r in add_results]
+        return [types.Task._create(r) for r in add_results]
 
     def delete(self, *task_ids: str):
         """Delete task(s).
 
         Args:
             *task_ids (str): The ID of tasks you wants to delete.
         """
         if len(task_ids) == 0:
             return
         self._client.execute_api(offline.DeleteApi(task_ids))
 
-    def clear(self, status: TaskStatus = TaskStatus.Complete):
+    def clear(self, status: types.TaskStatus = types.TaskStatus.Complete):
         """Clear tasks.
 
         Args:
             status (py115.types.TaskStatus): 
                 Tasks in given status will be cleared. Set status to None to 
                 clear all tasks.
         """
@@ -117,28 +117,49 @@
         if result is not None:
             total = int(result['all_total']['size'])
             used = int(result['all_use']['size'])
             return (total, used)
         else:
             return (0, 0)
 
-    def list(self, dir_id: str = '0') -> typing.Generator[File, None, None]:
+    def list(self, dir_id: str = '0') -> typing.Generator[types.File, None, None]:
         """Get files under a directory.
 
         Args:
             dir_id (str): Directory ID to list, default is "0" which means root directory.
 
         Yields:
             py115.types.File: File object under the directory.
         """
         spec = file.ListApi(dir_id)
         while True:
             result = self._client.execute_api(spec)
             for f in result['files']:
-                yield File._create(f)
+                yield types.File._create(f)
+            next_offset = result['offset'] + len(result['files'])
+            if next_offset >= result['count']:
+                break
+            else:
+                spec.set_offset(next_offset)
+
+    def search(self, keyword: str, dir_id: str = '0'):
+        """Recursively search files under a directory.
+
+        Args:
+            keyword (str): Keyword to search files.
+            dir_id (str): Directory ID to search.
+
+        Yields:
+            py115.types.File: File object whose name contains the keyword.
+        """
+        spec = file.SearchApi(keyword=keyword, dir_id=dir_id)
+        while True:
+            result = self._client.execute_api(spec)
+            for f in result['files']:
+                yield types.File._create(f)
             next_offset = result['offset'] + len(result['files'])
             if next_offset >= result['count']:
                 break
             else:
                 spec.set_offset(next_offset)
 
     def move(self, target_dir_id: str, *file_ids: str):
@@ -167,52 +188,78 @@
         Args:
             *file_ids (str): ID of files to be deleted.
         """
         if len(file_ids) == 0:
             return
         self._client.execute_api(file.DeleteApi(file_ids))
 
-    def make_dir(self, parent_id: str, name: str) -> File:
+    def make_dir(self, parent_id: str, name: str) -> types.File:
         """Make new directory under a directory.
         
         Args:
             parent_id (str): ID of parent directory where to make new directory.
             name (str): Name for the new directory.
         
         Return:
             py115.types.File: File object of the created directory.
         """
         result = self._client.execute_api(dir.AddApi(parent_id, name))
         result['pid'] = parent_id
-        return File._create(result)
+        return types.File._create(result)
 
-    def request_download(self, pickcode: str) -> DownloadTicket:
+    def request_download(self, pickcode: str) -> types.DownloadTicket:
         """Download file from cloud storage.
 
         Args:
             pickcode (str): Pick code of file.
 
         Returns:
             py115.types.DownloadTicket: A ticket contains all required fields to 
             download file from cloud.
         """
         result = self._client.execute_api(file.DownloadApi(pickcode))
         if result is None or 'url' not in result:
             return None
+        ticket = types.DownloadTicket()
+        ticket.url = result['url']
+        ticket.file_name = result.get('file_name')
+        ticket.file_size = result.get('file_size')
         # Required headers for downloading
         cookies = self._client.export_cookies(url=result['url'])
-        headers = {
+        ticket.headers = {
+            'User-Agent': self._client.user_agent,
+            'Cookie': '; '.join([
+                f'{k}={v}' for k, v in cookies.items()
+            ])
+        }
+        return ticket
+
+    def request_play(self, pickcode: str) -> types.PlayTicket:
+        """Play a video file on cloud, returns required parameters as a ticket.
+
+        Args:
+            pickcode (str): Pick code of file.
+        
+        Returns:
+            py115.types.PlayTicket: A ticket contains all required fields to 
+            play the media file on cloud.
+        """
+        ticket = types.PlayTicket()
+        ticket.url = self._client.execute_api(file.VideoApi(pickcode=pickcode))
+        # Prepare headers for playing
+        cookies = self._client.export_cookies(url=ticket.url)
+        ticket.headers = {
             'User-Agent': self._client.user_agent,
             'Cookie': '; '.join([
                 f'{k}={v}' for k, v in cookies.items()
             ])
         }
-        return DownloadTicket._create(result, headers)
+        return ticket
 
-    def request_upload(self, dir_id: str, file_path: str) -> UploadTicket:
+    def request_upload(self, dir_id: str, file_path: str) -> types.UploadTicket:
         """Upload local file to cloud storage.
 
         Args:
             dir_id (str): ID of directory where to store the file.
             file_path (str): Path of the local file.
         
         Return:
@@ -226,15 +273,15 @@
             return self.request_upload_data(dir_id, file_name, file_io)
 
     def request_upload_data(
             self, 
             dir_id: str, 
             save_name: str, 
             data_io: typing.BinaryIO, 
-        ) -> UploadTicket:
+        ) -> types.UploadTicket:
         """Upload data as a file to cloud storage.
 
         Args:
             dir_id (str): ID of directory where to store the file.
             save_name (str): File name to be saved.
             data_io (BinaryIO): IO stream of data.
 
@@ -249,8 +296,8 @@
             file_name=save_name,
             file_io=data_io,
             helper=self._upload_helper
         ))
         token_result = None
         if not init_result['done']:
             token_result = self._client.execute_api(upload.TokenApi())
-        return UploadTicket._create(init_result, token_result)
+        return types.UploadTicket._create(init_result, token_result)
```

### Comparing `py115-0.0.1/py115/types.py` & `py115-0.0.2/py115/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,30 @@
 __author__ = 'deadblue'
 
 from datetime import datetime
-from enum import IntEnum
+from enum import IntEnum, StrEnum
 
 from py115._internal import oss, utils
 
 
+class LoginPlatform(StrEnum):
+
+    Web = "web"
+    """Web."""
+
+    Mac = "mac"
+    """MAC App."""
+
+    Linux = "linux"
+    """Linux App."""
+
+    Windows = "windows"
+    """Windows App."""
+
+
 class _Base:
     """Base clase for all types."""
 
     def __repr__(self) -> str:
         cls_name = type(self).__name__
         attrs = ', '.join([
             f'{k}={v}' for k, v in self.__dict__.items()
@@ -61,17 +76,14 @@
         """
         return {
             'UID': self._uid,
             'CID': self._cid,
             'SEID': self._seid,
         }
 
-    # def __repr__(self) -> str:
-    #     return f'Credential(UID={self._uid}, CID={self._cid}, SEID={self._seid})'
-
 
 class File(_Base):
     """File represents a cloud file or directory."""
 
     file_id: str
     """Unique ID of the file on cloud."""
 
@@ -101,15 +113,18 @@
         category_id = raw.get('cid')
         file_id = raw.get('fid')
         parent_id = raw.get('pid')
 
         r = cls()
         r.is_dir = file_id is None
         r.name = raw.get('n')
-        r.modified_time = utils.parse_datetime_str(raw.get('t'))
+        if 'te' in raw:
+            r.modified_time = utils.parse_datetime_str(raw.get('te'))
+        else:
+            r.modified_time = utils.parse_datetime_str(raw.get('t'))
         if r.is_dir:
             r.file_id = category_id
             r.parent_id = parent_id
             r.size, r.sha1, r.pickcode = 0, None, None
         else:
             r.file_id = file_id
             r.parent_id = category_id
@@ -141,22 +156,22 @@
 
     url: str
     """Download URL."""
 
     headers: dict
     """Required headers that should be used with download URL."""
 
-    @classmethod
-    def _create(cls, raw: dict, header: dict):
-        r = cls()
-        r.file_name = raw.get('file_name')
-        r.file_size = raw.get('file_size')
-        r.url = raw.get('url')
-        r.headers = header.copy()
-        return r
+
+class PlayTicket(_Base):
+
+    url: str
+    """Download URL."""
+
+    headers: dict
+    """Required headers that should be used with download URL."""
 
 
 class UploadTicket(_Base):
     """
     UploadTicket contains required parameters to upload a file to 
     cloud storage.
```

### Comparing `py115-0.0.1/py115.egg-info/PKG-INFO` & `py115-0.0.2/py115.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py115
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python SDK for 115 cloud storage service.
 Author-email: deadblue <public@dead.blue>
 License: MIT License
         
         Copyright 2023 deadblue
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of 
@@ -43,18 +43,23 @@
 An API client of 115 cloud storage service.
 
 Install
 =======
 
 .. code:: shell
 
+    # Install from PyPI
+    pip install py115
+
+    # Or install from source
     pip install git+https://github.com/deadblue/py115.git
 
-Example
-=======
+
+Usage
+=====
 
 .. code:: python
 
     import py115
     from py115.types import Credentail
 
     # Connect to cloud
@@ -77,7 +82,19 @@
         print('Task: %r' % task)
     # Add task by download URLs
     offline.add_url(
         'magnet:?xt=urn:btih:000123456789abcdef1151150123456789abcdef',
         'ed2k://|file|ED2k-file|115115115|1234567890abcdef1234567890abcdef|/',
         'https://dl.some-server.com/some/file.ext'
     )
+
+
+Document
+========
+
+https://py115.readthedocs.io/en/stable/
+
+
+License
+=======
+
+MIT
```

### Comparing `py115-0.0.1/py115.egg-info/SOURCES.txt` & `py115-0.0.2/py115.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 LICENSE
 README.rst
 pyproject.toml
 requirements.txt
 setup.py
 py115/__init__.py
 py115/cloud.py
+py115/login.py
 py115/services.py
 py115/types.py
 py115.egg-info/PKG-INFO
 py115.egg-info/SOURCES.txt
 py115.egg-info/dependency_links.txt
 py115.egg-info/requires.txt
 py115.egg-info/top_level.txt
 py115/_internal/__init__.py
 py115/_internal/oss.py
 py115/_internal/utils.py
 py115/_internal/api/__init__.py
 py115/_internal/api/dir.py
 py115/_internal/api/file.py
+py115/_internal/api/m115.py
 py115/_internal/api/offline.py
+py115/_internal/api/qrcode.py
 py115/_internal/api/space.py
 py115/_internal/api/upload.py
 py115/_internal/api/user.py
 py115/_internal/api/version.py
 py115/_internal/crypto/__init__.py
 py115/_internal/crypto/_rsa.py
 py115/_internal/crypto/_xor.py
```

### Comparing `py115-0.0.1/pyproject.toml` & `py115-0.0.2/pyproject.toml`

 * *Files identical despite different names*

