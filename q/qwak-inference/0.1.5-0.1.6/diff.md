# Comparing `tmp/qwak_inference-0.1.5.tar.gz` & `tmp/qwak_inference-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_inference-0.1.5.tar", max compression
+gzip compressed data, was "qwak_inference-0.1.6.tar", max compression
```

## Comparing `qwak_inference-0.1.5.tar` & `qwak_inference-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    10480 2023-06-08 11:22:31.002831 qwak_inference-0.1.5/LICENSE
--rw-r--r--   0        0        0      267 2023-06-08 11:22:31.002831 qwak_inference-0.1.5/README.md
--rw-r--r--   0        0        0     1893 2023-06-08 11:23:26.943152 qwak_inference-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      804 2023-06-08 11:23:26.943152 qwak_inference-0.1.5/qwak_inference/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 11:22:31.002831 qwak_inference-0.1.5/qwak_inference/batch_client/__init__.py
--rw-r--r--   0        0        0    20136 2023-06-08 11:22:31.002831 qwak_inference-0.1.5/qwak_inference/batch_client/batch_client.py
--rw-r--r--   0        0        0     2172 2023-06-08 11:22:31.006831 qwak_inference-0.1.5/qwak_inference/batch_client/file_serialization.py
--rw-r--r--   0        0        0     1497 2023-06-08 11:22:31.006831 qwak_inference-0.1.5/qwak_inference/batch_client/instance_validation.py
--rw-r--r--   0        0        0      739 2023-06-08 11:22:31.006831 qwak_inference-0.1.5/qwak_inference/batch_client/s3.py
--rw-r--r--   0        0        0       95 2023-06-08 11:22:31.006831 qwak_inference-0.1.5/qwak_inference/configuration/__init__.py
--rw-r--r--   0        0        0     3127 2023-06-08 11:22:31.006831 qwak_inference-0.1.5/qwak_inference/configuration/account.py
--rw-r--r--   0        0        0     2676 2023-06-08 11:22:31.006831 qwak_inference-0.1.5/qwak_inference/configuration/auth.py
--rw-r--r--   0        0        0      929 2023-06-08 11:22:31.006831 qwak_inference-0.1.5/qwak_inference/configuration/session.py
--rw-r--r--   0        0        0      688 2023-06-08 11:22:31.006831 qwak_inference-0.1.5/qwak_inference/constants.py
--rw-r--r--   0        0        0     1592 2023-06-08 11:22:31.006831 qwak_inference-0.1.5/qwak_inference/exceptions.py
--rw-r--r--   0        0        0     1999 2023-06-08 11:22:31.006831 qwak_inference-0.1.5/qwak_inference/feedback_client.py
--rw-r--r--   0        0        0       65 2023-06-08 11:22:31.006831 qwak_inference-0.1.5/qwak_inference/realtime_client/__init__.py
--rw-r--r--   0        0        0     4811 2023-06-08 11:22:31.006831 qwak_inference-0.1.5/qwak_inference/realtime_client/client.py
--rw-r--r--   0        0        0     2345 2023-06-08 11:22:31.006831 qwak_inference-0.1.5/qwak_inference/realtime_client/rest_helpers.py
--rw-r--r--   0        0        0     2050 1970-01-01 00:00:00.000000 qwak_inference-0.1.5/setup.py
--rw-r--r--   0        0        0     1809 1970-01-01 00:00:00.000000 qwak_inference-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    10480 2023-07-09 06:43:09.509103 qwak_inference-0.1.6/LICENSE
+-rw-r--r--   0        0        0      267 2023-07-09 06:43:09.509103 qwak_inference-0.1.6/README.md
+-rw-r--r--   0        0        0     1893 2023-07-09 06:44:01.485719 qwak_inference-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      804 2023-07-09 06:44:01.485719 qwak_inference-0.1.6/qwak_inference/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 06:43:09.513104 qwak_inference-0.1.6/qwak_inference/batch_client/__init__.py
+-rw-r--r--   0        0        0    20136 2023-07-09 06:43:09.513104 qwak_inference-0.1.6/qwak_inference/batch_client/batch_client.py
+-rw-r--r--   0        0        0     2172 2023-07-09 06:43:09.513104 qwak_inference-0.1.6/qwak_inference/batch_client/file_serialization.py
+-rw-r--r--   0        0        0     1497 2023-07-09 06:43:09.513104 qwak_inference-0.1.6/qwak_inference/batch_client/instance_validation.py
+-rw-r--r--   0        0        0      739 2023-07-09 06:43:09.513104 qwak_inference-0.1.6/qwak_inference/batch_client/s3.py
+-rw-r--r--   0        0        0       95 2023-07-09 06:43:09.513104 qwak_inference-0.1.6/qwak_inference/configuration/__init__.py
+-rw-r--r--   0        0        0     3127 2023-07-09 06:43:09.513104 qwak_inference-0.1.6/qwak_inference/configuration/account.py
+-rw-r--r--   0        0        0     2676 2023-07-09 06:43:09.513104 qwak_inference-0.1.6/qwak_inference/configuration/auth.py
+-rw-r--r--   0        0        0      929 2023-07-09 06:43:09.513104 qwak_inference-0.1.6/qwak_inference/configuration/session.py
+-rw-r--r--   0        0        0      688 2023-07-09 06:43:09.513104 qwak_inference-0.1.6/qwak_inference/constants.py
+-rw-r--r--   0        0        0     1592 2023-07-09 06:43:09.513104 qwak_inference-0.1.6/qwak_inference/exceptions.py
+-rw-r--r--   0        0        0     1999 2023-07-09 06:43:09.513104 qwak_inference-0.1.6/qwak_inference/feedback_client.py
+-rw-r--r--   0        0        0       65 2023-07-09 06:43:09.513104 qwak_inference-0.1.6/qwak_inference/realtime_client/__init__.py
+-rw-r--r--   0        0        0     4811 2023-07-09 06:43:09.513104 qwak_inference-0.1.6/qwak_inference/realtime_client/client.py
+-rw-r--r--   0        0        0     2346 2023-07-09 06:43:09.513104 qwak_inference-0.1.6/qwak_inference/realtime_client/rest_helpers.py
+-rw-r--r--   0        0        0     2050 1970-01-01 00:00:00.000000 qwak_inference-0.1.6/setup.py
+-rw-r--r--   0        0        0     1809 1970-01-01 00:00:00.000000 qwak_inference-0.1.6/PKG-INFO
```

### Comparing `qwak_inference-0.1.5/LICENSE` & `qwak_inference-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.5/pyproject.toml` & `qwak_inference-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-inference"
-version = "0.1.5"
+version = "0.1.6"
 description = "Qwak Inference is a Python library for running predictions again Qwak Models."
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.7",
```

### Comparing `qwak_inference-0.1.5/qwak_inference/__init__.py` & `qwak_inference-0.1.6/qwak_inference/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,8 +16,8 @@
     print(
         "Notice that BatchInferenceClient and FeedbackClient are not available in the skinny package. "
         'In order to use them, please install them as extras: pip install "qwak-inference[batch,feedback]".'
     )
 
 __all__ = clients
 
-__version__ = "0.1.5"
+__version__ = "0.1.6"
```

### Comparing `qwak_inference-0.1.5/qwak_inference/batch_client/batch_client.py` & `qwak_inference-0.1.6/qwak_inference/batch_client/batch_client.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.5/qwak_inference/batch_client/file_serialization.py` & `qwak_inference-0.1.6/qwak_inference/batch_client/file_serialization.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.5/qwak_inference/batch_client/instance_validation.py` & `qwak_inference-0.1.6/qwak_inference/batch_client/instance_validation.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.5/qwak_inference/batch_client/s3.py` & `qwak_inference-0.1.6/qwak_inference/batch_client/s3.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.5/qwak_inference/configuration/account.py` & `qwak_inference-0.1.6/qwak_inference/configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.5/qwak_inference/configuration/auth.py` & `qwak_inference-0.1.6/qwak_inference/configuration/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.5/qwak_inference/configuration/session.py` & `qwak_inference-0.1.6/qwak_inference/configuration/session.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.5/qwak_inference/constants.py` & `qwak_inference-0.1.6/qwak_inference/constants.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.5/qwak_inference/exceptions.py` & `qwak_inference-0.1.6/qwak_inference/exceptions.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.5/qwak_inference/feedback_client.py` & `qwak_inference-0.1.6/qwak_inference/feedback_client.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.5/qwak_inference/realtime_client/client.py` & `qwak_inference-0.1.6/qwak_inference/realtime_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.5/qwak_inference/realtime_client/rest_helpers.py` & `qwak_inference-0.1.6/qwak_inference/realtime_client/rest_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,17 +36,17 @@
 
 class RestSession(requests.Session):
     def __init__(self):
         super().__init__()
         self.headers.update({"Content-Type": "application/json"})
         socket_options = [
             ("SOL_SOCKET", "SO_KEEPALIVE", 1),
-            ("SOL_TCP", "TCP_KEEPIDLE", 45),
-            ("SOL_TCP", "TCP_KEEPINTVL", 10),
-            ("SOL_TCP", "TCP_KEEPCNT", 6),
+            ("SOL_TCP", "TCP_KEEPIDLE", 120),
+            ("SOL_TCP", "TCP_KEEPINTVL", 75),
+            ("SOL_TCP", "TCP_KEEPCNT", 9),
         ]
         socket_options = validate_socket_config(socket_options)
         adapter = HTTPAdapterWithSocketOptions(socket_options=socket_options)
         self.mount("https://", adapter)
         self.mount("http://", adapter)
 
     def prepare_request(self, request):
```

### Comparing `qwak_inference-0.1.5/setup.py` & `qwak_inference-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
  'feedback:python_full_version >= "3.7.1" and python_version < "3.8"': ['pandas<1.4',
                                                                         'pandas<1.4'],
  'feedback:python_version >= "3.8" and python_version < "3.10"': ['pandas>=1.4.3,<2.0.0',
                                                                   'pandas>=1.4.3,<2.0.0']}
 
 setup_kwargs = {
     'name': 'qwak-inference',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': 'Qwak Inference is a Python library for running predictions again Qwak Models.',
     'long_description': '# Qwak Inference\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Inference contains tools that allow predicting against the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_inference-0.1.5/PKG-INFO` & `qwak_inference-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-inference
-Version: 0.1.5
+Version: 0.1.6
 Summary: Qwak Inference is a Python library for running predictions again Qwak Models.
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

