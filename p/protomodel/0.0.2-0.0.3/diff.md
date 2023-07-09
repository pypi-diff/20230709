# Comparing `tmp/protomodel-0.0.2.tar.gz` & `tmp/protomodel-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protomodel-0.0.2.tar", max compression
+gzip compressed data, was "protomodel-0.0.3.tar", max compression
```

## Comparing `protomodel-0.0.2.tar` & `protomodel-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,14 @@
--rw-r--r--   0        0        0       84 2023-07-04 20:52:27.187402 protomodel-0.0.2/README.md
--rw-r--r--   0        0        0      108 2023-07-05 03:31:17.977392 protomodel-0.0.2/protomodel/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 04:40:34.047386 protomodel-0.0.2/protomodel/example/__init__.py
--rw-r--r--   0        0        0     1567 2023-07-05 04:43:58.577395 protomodel-0.0.2/protomodel/example/__pycache__/data.cpython-311.pyc
--rw-r--r--   0        0        0      330 2023-07-05 04:46:11.747388 protomodel-0.0.2/protomodel/example/data.proto
--rw-r--r--   0        0        0      330 2023-07-05 04:42:08.657389 protomodel-0.0.2/protomodel/example/data.py
--rw-r--r--   0        0        0      521 2023-07-05 04:44:24.847394 protomodel-0.0.2/protomodel/example/run.py
--rw-r--r--   0        0        0       22 2023-07-05 03:07:25.797387 protomodel-0.0.2/protomodel/grpc.py
--rw-r--r--   0        0        0     1068 2023-07-05 04:39:57.197387 protomodel-0.0.2/protomodel/message.py
--rw-r--r--   0        0        0        0 2023-07-05 03:31:11.937394 protomodel-0.0.2/protomodel/protomodel/__init__.py
--rw-r--r--   0        0        0      329 2023-07-04 21:40:33.857408 protomodel-0.0.2/protomodel/protomodel/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      377 2023-07-04 21:40:33.867408 protomodel-0.0.2/protomodel/protomodel/__pycache__/grpc.cpython-311.pyc
--rw-r--r--   0        0        0     2361 2023-07-05 03:00:39.517398 protomodel-0.0.2/protomodel/protomodel/__pycache__/message.cpython-311.pyc
--rw-r--r--   0        0        0      384 2023-07-04 21:40:33.867408 protomodel-0.0.2/protomodel/protomodel/__pycache__/service.cpython-311.pyc
--rw-r--r--   0        0        0       25 2023-07-05 03:07:52.257387 protomodel-0.0.2/protomodel/service.py
--rw-r--r--   0        0        0       45 2023-07-05 00:34:36.687412 protomodel-0.0.2/protomodel/types/__init__.py
--rw-r--r--   0        0        0      218 2023-07-05 00:34:59.067411 protomodel-0.0.2/protomodel/types/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      409 2023-07-05 01:01:08.637407 protomodel-0.0.2/protomodel/types/__pycache__/get_types.cpython-311.pyc
--rw-r--r--   0        0        0      169 2023-07-05 01:01:02.117407 protomodel-0.0.2/protomodel/types/get_types.py
--rw-r--r--   0        0        0        0 2023-07-05 00:59:28.647385 protomodel-0.0.2/protomodel/utils/__init__.py
--rw-r--r--   0        0        0      387 2023-07-05 04:47:02.627389 protomodel-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      452 1970-01-01 00:00:00.000000 protomodel-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       84 2023-07-04 20:52:27.187402 protomodel-0.0.3/README.md
+-rw-r--r--   0        0        0      107 2023-07-09 03:57:46.521399 protomodel-0.0.3/protomodel/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 04:40:34.047386 protomodel-0.0.3/protomodel/example/__init__.py
+-rw-r--r--   0        0        0      348 2023-07-05 18:47:04.977144 protomodel-0.0.3/protomodel/example/data.py
+-rw-r--r--   0        0        0      584 2023-07-09 03:00:20.241381 protomodel-0.0.3/protomodel/example/run.py
+-rw-r--r--   0        0        0     1306 2023-07-09 03:57:31.021375 protomodel-0.0.3/protomodel/message.py
+-rw-r--r--   0        0        0        0 2023-07-05 03:31:11.937394 protomodel-0.0.3/protomodel/protomodel/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-09 03:57:46.521399 protomodel-0.0.3/protomodel/rpc.py
+-rw-r--r--   0        0        0       25 2023-07-05 03:07:52.257387 protomodel-0.0.3/protomodel/service.py
+-rw-r--r--   0        0        0       45 2023-07-05 00:34:36.687412 protomodel-0.0.3/protomodel/types/__init__.py
+-rw-r--r--   0        0        0      247 2023-07-05 18:43:19.587132 protomodel-0.0.3/protomodel/types/get_types.py
+-rw-r--r--   0        0        0        0 2023-07-05 00:59:28.647385 protomodel-0.0.3/protomodel/utils/__init__.py
+-rw-r--r--   0        0        0      387 2023-07-09 03:58:23.321417 protomodel-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      452 1970-01-01 00:00:00.000000 protomodel-0.0.3/PKG-INFO
```

### Comparing `protomodel-0.0.2/protomodel/example/run.py` & `protomodel-0.0.3/protomodel/example/run.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import data
 from protomodel import message, service, rpc
+from typing import TextIO, List, Type, Any
 
 input_filename = "data.py"
 output_filename = "data.proto"
     
-proto_file = open(f"./{output_filename}", "w")
+proto_file: TextIO = open(f"./{output_filename}", "w")
 proto_file.write('syntax = "proto3";\n\npackage app.proto;\n\n')
 
 # global_symbols = globals()
 # messages = [cls for cls in global_symbols.values() if isinstance(cls, message)]
-messages = [cls for cls in data.__dict__.values() if isinstance(cls, message)]
+messages: List[message] = [cls for cls in data.__dict__.values() if isinstance(cls, message)]
 
 for msg in messages:
-    msg.add_messages(proto_file)
+    msg.add_field(proto_file)
 
 print('file created.')
 proto_file.close()
```

