# Comparing `tmp/dataclass_codec-0.5.1.tar.gz` & `tmp/dataclass_codec-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclass_codec-0.5.1.tar", max compression
+gzip compressed data, was "dataclass_codec-0.5.2.tar", max compression
```

## Comparing `dataclass_codec-0.5.1.tar` & `dataclass_codec-0.5.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     4985 2023-07-09 18:44:13.085711 dataclass_codec-0.5.1/README.md
--rw-r--r--   0        0        0      600 2023-07-09 18:45:05.535698 dataclass_codec-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      246 2023-06-21 01:44:15.139451 dataclass_codec-0.5.1/src/dataclass_codec/__init__.py
--rw-r--r--   0        0        0    15242 2023-07-09 03:57:07.697077 dataclass_codec-0.5.1/src/dataclass_codec/decode.py
--rw-r--r--   0        0        0     2929 2023-06-21 01:51:35.509431 dataclass_codec-0.5.1/src/dataclass_codec/encode.py
--rw-r--r--   0        0        0        0 2023-06-21 01:44:15.139451 dataclass_codec-0.5.1/src/dataclass_codec/py.typed
--rw-r--r--   0        0        0    21509 2023-07-09 04:07:07.587053 dataclass_codec-0.5.1/src/dataclass_codec/tests/test_dataclass_codec.py
--rw-r--r--   0        0        0      436 2023-07-09 03:52:02.877095 dataclass_codec-0.5.1/src/dataclass_codec/types_predicates.py
--rw-r--r--   0        0        0     5438 1970-01-01 00:00:00.000000 dataclass_codec-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     7158 2023-07-09 18:53:38.065575 dataclass_codec-0.5.2/README.md
+-rw-r--r--   0        0        0      600 2023-07-09 18:54:08.215568 dataclass_codec-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      246 2023-06-21 01:44:15.139451 dataclass_codec-0.5.2/src/dataclass_codec/__init__.py
+-rw-r--r--   0        0        0    15242 2023-07-09 03:57:07.697077 dataclass_codec-0.5.2/src/dataclass_codec/decode.py
+-rw-r--r--   0        0        0     2929 2023-06-21 01:51:35.509431 dataclass_codec-0.5.2/src/dataclass_codec/encode.py
+-rw-r--r--   0        0        0        0 2023-06-21 01:44:15.139451 dataclass_codec-0.5.2/src/dataclass_codec/py.typed
+-rw-r--r--   0        0        0    21509 2023-07-09 04:07:07.587053 dataclass_codec-0.5.2/src/dataclass_codec/tests/test_dataclass_codec.py
+-rw-r--r--   0        0        0      436 2023-07-09 03:52:02.877095 dataclass_codec-0.5.2/src/dataclass_codec/types_predicates.py
+-rw-r--r--   0        0        0     7611 1970-01-01 00:00:00.000000 dataclass_codec-0.5.2/PKG-INFO
```

### Comparing `dataclass_codec-0.5.1/pyproject.toml` & `dataclass_codec-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataclass-codec"
-version = "0.5.1"
+version = "0.5.2"
 description = ""
 authors = ["lucas.silva <lucas.silva@jeaholding.com.br>"]
 readme = "README.md"
 packages = [{include = "dataclass_codec", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `dataclass_codec-0.5.1/src/dataclass_codec/decode.py` & `dataclass_codec-0.5.2/src/dataclass_codec/decode.py`

 * *Files identical despite different names*

### Comparing `dataclass_codec-0.5.1/src/dataclass_codec/encode.py` & `dataclass_codec-0.5.2/src/dataclass_codec/encode.py`

 * *Files identical despite different names*

### Comparing `dataclass_codec-0.5.1/src/dataclass_codec/tests/test_dataclass_codec.py` & `dataclass_codec-0.5.2/src/dataclass_codec/tests/test_dataclass_codec.py`

 * *Files identical despite different names*

