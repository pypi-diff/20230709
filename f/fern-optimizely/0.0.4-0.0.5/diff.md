# Comparing `tmp/fern_optimizely-0.0.4.tar.gz` & `tmp/fern_optimizely-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fern_optimizely-0.0.4.tar", max compression
+gzip compressed data, was "fern_optimizely-0.0.5.tar", max compression
```

## Comparing `fern_optimizely-0.0.4.tar` & `fern_optimizely-0.0.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     2858 2023-07-09 17:55:42.157995 fern_optimizely-0.0.4/README.md
--rw-r--r--   0        0        0      380 2023-07-09 17:55:42.157995 fern_optimizely-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      734 2023-07-09 17:55:42.157995 fern_optimizely-0.0.4/src/optimizely/__init__.py
--rw-r--r--   0        0        0     4751 2023-07-09 17:55:42.157995 fern_optimizely-0.0.4/src/optimizely/client.py
--rw-r--r--   0        0        0      348 2023-07-09 17:55:42.157995 fern_optimizely-0.0.4/src/optimizely/core/__init__.py
--rw-r--r--   0        0        0      426 2023-07-09 17:55:42.157995 fern_optimizely-0.0.4/src/optimizely/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-07-09 17:55:42.157995 fern_optimizely-0.0.4/src/optimizely/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-07-09 17:55:42.157995 fern_optimizely-0.0.4/src/optimizely/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-07-09 17:55:42.157995 fern_optimizely-0.0.4/src/optimizely/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      170 2023-07-09 17:55:42.157995 fern_optimizely-0.0.4/src/optimizely/errors/__init__.py
--rw-r--r--   0        0        0      313 2023-07-09 17:55:42.157995 fern_optimizely-0.0.4/src/optimizely/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2023-07-09 17:55:42.157995 fern_optimizely-0.0.4/src/optimizely/py.typed
--rw-r--r--   0        0        0      124 2023-07-09 17:55:42.157995 fern_optimizely-0.0.4/src/optimizely/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-09 17:55:42.157995 fern_optimizely-0.0.4/src/optimizely/resources/models/__init__.py
--rw-r--r--   0        0        0     3413 2023-07-09 17:55:42.157995 fern_optimizely-0.0.4/src/optimizely/resources/models/client.py
--rw-r--r--   0        0        0       65 2023-07-09 17:55:42.157995 fern_optimizely-0.0.4/src/optimizely/resources/proxy/__init__.py
--rw-r--r--   0        0        0     4234 2023-07-09 17:55:42.157995 fern_optimizely-0.0.4/src/optimizely/resources/proxy/client.py
--rw-r--r--   0        0        0      856 2023-07-09 17:55:42.157995 fern_optimizely-0.0.4/src/optimizely/types/__init__.py
--rw-r--r--   0        0        0      921 2023-07-09 17:55:42.157995 fern_optimizely-0.0.4/src/optimizely/types/chat_completions_response_dto.py
--rw-r--r--   0        0        0      815 2023-07-09 17:55:42.157995 fern_optimizely-0.0.4/src/optimizely/types/chat_completions_usage_dto.py
--rw-r--r--   0        0        0      765 2023-07-09 17:55:42.157995 fern_optimizely-0.0.4/src/optimizely/types/chat_message_dto.py
--rw-r--r--   0        0        0      836 2023-07-09 17:55:42.157995 fern_optimizely-0.0.4/src/optimizely/types/chat_request_dto.py
--rw-r--r--   0        0        0      843 2023-07-09 17:55:42.157995 fern_optimizely-0.0.4/src/optimizely/types/http_validation_error.py
--rw-r--r--   0        0        0      918 2023-07-09 17:55:42.157995 fern_optimizely-0.0.4/src/optimizely/types/model_dto.py
--rw-r--r--   0        0        0      803 2023-07-09 17:55:42.157995 fern_optimizely-0.0.4/src/optimizely/types/models_response_dto.py
--rw-r--r--   0        0        0      753 2023-07-09 17:55:42.157995 fern_optimizely-0.0.4/src/optimizely/types/tokens_response_dto.py
--rw-r--r--   0        0        0      869 2023-07-09 17:55:42.157995 fern_optimizely-0.0.4/src/optimizely/types/validation_error.py
--rw-r--r--   0        0        0      128 2023-07-09 17:55:42.157995 fern_optimizely-0.0.4/src/optimizely/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     3275 1970-01-01 00:00:00.000000 fern_optimizely-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     2858 2023-07-09 17:57:25.848065 fern_optimizely-0.0.5/README.md
+-rw-r--r--   0        0        0      380 2023-07-09 17:57:25.848065 fern_optimizely-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      734 2023-07-09 17:57:25.848065 fern_optimizely-0.0.5/src/optimizely/__init__.py
+-rw-r--r--   0        0        0     4751 2023-07-09 17:57:25.848065 fern_optimizely-0.0.5/src/optimizely/client.py
+-rw-r--r--   0        0        0      348 2023-07-09 17:57:25.848065 fern_optimizely-0.0.5/src/optimizely/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-09 17:57:25.848065 fern_optimizely-0.0.5/src/optimizely/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-07-09 17:57:25.848065 fern_optimizely-0.0.5/src/optimizely/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-07-09 17:57:25.848065 fern_optimizely-0.0.5/src/optimizely/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-07-09 17:57:25.848065 fern_optimizely-0.0.5/src/optimizely/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      170 2023-07-09 17:57:25.848065 fern_optimizely-0.0.5/src/optimizely/errors/__init__.py
+-rw-r--r--   0        0        0      313 2023-07-09 17:57:25.848065 fern_optimizely-0.0.5/src/optimizely/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2023-07-09 17:57:25.848065 fern_optimizely-0.0.5/src/optimizely/py.typed
+-rw-r--r--   0        0        0      124 2023-07-09 17:57:25.848065 fern_optimizely-0.0.5/src/optimizely/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-09 17:57:25.848065 fern_optimizely-0.0.5/src/optimizely/resources/models/__init__.py
+-rw-r--r--   0        0        0     3413 2023-07-09 17:57:25.848065 fern_optimizely-0.0.5/src/optimizely/resources/models/client.py
+-rw-r--r--   0        0        0       65 2023-07-09 17:57:25.848065 fern_optimizely-0.0.5/src/optimizely/resources/proxy/__init__.py
+-rw-r--r--   0        0        0     4234 2023-07-09 17:57:25.848065 fern_optimizely-0.0.5/src/optimizely/resources/proxy/client.py
+-rw-r--r--   0        0        0      856 2023-07-09 17:57:25.848065 fern_optimizely-0.0.5/src/optimizely/types/__init__.py
+-rw-r--r--   0        0        0      921 2023-07-09 17:57:25.848065 fern_optimizely-0.0.5/src/optimizely/types/chat_completions_response_dto.py
+-rw-r--r--   0        0        0      815 2023-07-09 17:57:25.848065 fern_optimizely-0.0.5/src/optimizely/types/chat_completions_usage_dto.py
+-rw-r--r--   0        0        0      765 2023-07-09 17:57:25.848065 fern_optimizely-0.0.5/src/optimizely/types/chat_message_dto.py
+-rw-r--r--   0        0        0      836 2023-07-09 17:57:25.848065 fern_optimizely-0.0.5/src/optimizely/types/chat_request_dto.py
+-rw-r--r--   0        0        0      843 2023-07-09 17:57:25.848065 fern_optimizely-0.0.5/src/optimizely/types/http_validation_error.py
+-rw-r--r--   0        0        0      918 2023-07-09 17:57:25.848065 fern_optimizely-0.0.5/src/optimizely/types/model_dto.py
+-rw-r--r--   0        0        0      803 2023-07-09 17:57:25.848065 fern_optimizely-0.0.5/src/optimizely/types/models_response_dto.py
+-rw-r--r--   0        0        0      753 2023-07-09 17:57:25.848065 fern_optimizely-0.0.5/src/optimizely/types/tokens_response_dto.py
+-rw-r--r--   0        0        0      869 2023-07-09 17:57:25.848065 fern_optimizely-0.0.5/src/optimizely/types/validation_error.py
+-rw-r--r--   0        0        0      128 2023-07-09 17:57:25.848065 fern_optimizely-0.0.5/src/optimizely/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     3275 1970-01-01 00:00:00.000000 fern_optimizely-0.0.5/PKG-INFO
```

### Comparing `fern_optimizely-0.0.4/README.md` & `fern_optimizely-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fern_optimizely-0.0.4/src/optimizely/__init__.py` & `fern_optimizely-0.0.5/src/optimizely/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_optimizely-0.0.4/src/optimizely/client.py` & `fern_optimizely-0.0.5/src/optimizely/client.py`

 * *Files identical despite different names*

### Comparing `fern_optimizely-0.0.4/src/optimizely/core/datetime_utils.py` & `fern_optimizely-0.0.5/src/optimizely/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `fern_optimizely-0.0.4/src/optimizely/core/jsonable_encoder.py` & `fern_optimizely-0.0.5/src/optimizely/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `fern_optimizely-0.0.4/src/optimizely/resources/models/client.py` & `fern_optimizely-0.0.5/src/optimizely/resources/models/client.py`

 * *Files identical despite different names*

### Comparing `fern_optimizely-0.0.4/src/optimizely/resources/proxy/client.py` & `fern_optimizely-0.0.5/src/optimizely/resources/proxy/client.py`

 * *Files identical despite different names*

### Comparing `fern_optimizely-0.0.4/src/optimizely/types/__init__.py` & `fern_optimizely-0.0.5/src/optimizely/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_optimizely-0.0.4/src/optimizely/types/chat_completions_response_dto.py` & `fern_optimizely-0.0.5/src/optimizely/types/chat_completions_response_dto.py`

 * *Files identical despite different names*

### Comparing `fern_optimizely-0.0.4/src/optimizely/types/chat_completions_usage_dto.py` & `fern_optimizely-0.0.5/src/optimizely/types/chat_completions_usage_dto.py`

 * *Files identical despite different names*

### Comparing `fern_optimizely-0.0.4/src/optimizely/types/chat_message_dto.py` & `fern_optimizely-0.0.5/src/optimizely/types/chat_message_dto.py`

 * *Files identical despite different names*

### Comparing `fern_optimizely-0.0.4/src/optimizely/types/chat_request_dto.py` & `fern_optimizely-0.0.5/src/optimizely/types/chat_request_dto.py`

 * *Files identical despite different names*

### Comparing `fern_optimizely-0.0.4/src/optimizely/types/http_validation_error.py` & `fern_optimizely-0.0.5/src/optimizely/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `fern_optimizely-0.0.4/src/optimizely/types/model_dto.py` & `fern_optimizely-0.0.5/src/optimizely/types/model_dto.py`

 * *Files identical despite different names*

### Comparing `fern_optimizely-0.0.4/src/optimizely/types/models_response_dto.py` & `fern_optimizely-0.0.5/src/optimizely/types/models_response_dto.py`

 * *Files identical despite different names*

### Comparing `fern_optimizely-0.0.4/src/optimizely/types/tokens_response_dto.py` & `fern_optimizely-0.0.5/src/optimizely/types/tokens_response_dto.py`

 * *Files identical despite different names*

### Comparing `fern_optimizely-0.0.4/src/optimizely/types/validation_error.py` & `fern_optimizely-0.0.5/src/optimizely/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `fern_optimizely-0.0.4/PKG-INFO` & `fern_optimizely-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fern-optimizely
-Version: 0.0.4
+Version: 0.0.5
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

