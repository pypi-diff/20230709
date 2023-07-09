# Comparing `tmp/dataclass_codec-0.5.2.tar.gz` & `tmp/dataclass_codec-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclass_codec-0.5.2.tar", max compression
+gzip compressed data, was "dataclass_codec-0.5.3.tar", max compression
```

## Comparing `dataclass_codec-0.5.2.tar` & `dataclass_codec-0.5.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     7158 2023-07-09 18:53:38.065575 dataclass_codec-0.5.2/README.md
--rw-r--r--   0        0        0      600 2023-07-09 18:54:08.215568 dataclass_codec-0.5.2/pyproject.toml
--rw-r--r--   0        0        0      246 2023-06-21 01:44:15.139451 dataclass_codec-0.5.2/src/dataclass_codec/__init__.py
--rw-r--r--   0        0        0    15242 2023-07-09 03:57:07.697077 dataclass_codec-0.5.2/src/dataclass_codec/decode.py
--rw-r--r--   0        0        0     2929 2023-06-21 01:51:35.509431 dataclass_codec-0.5.2/src/dataclass_codec/encode.py
--rw-r--r--   0        0        0        0 2023-06-21 01:44:15.139451 dataclass_codec-0.5.2/src/dataclass_codec/py.typed
--rw-r--r--   0        0        0    21509 2023-07-09 04:07:07.587053 dataclass_codec-0.5.2/src/dataclass_codec/tests/test_dataclass_codec.py
--rw-r--r--   0        0        0      436 2023-07-09 03:52:02.877095 dataclass_codec-0.5.2/src/dataclass_codec/types_predicates.py
--rw-r--r--   0        0        0     7611 1970-01-01 00:00:00.000000 dataclass_codec-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0    10143 2023-07-09 19:00:29.355476 dataclass_codec-0.5.3/README.md
+-rw-r--r--   0        0        0      600 2023-07-09 19:00:42.995473 dataclass_codec-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0      246 2023-06-21 01:44:15.139451 dataclass_codec-0.5.3/src/dataclass_codec/__init__.py
+-rw-r--r--   0        0        0    15242 2023-07-09 03:57:07.697077 dataclass_codec-0.5.3/src/dataclass_codec/decode.py
+-rw-r--r--   0        0        0     2929 2023-06-21 01:51:35.509431 dataclass_codec-0.5.3/src/dataclass_codec/encode.py
+-rw-r--r--   0        0        0        0 2023-06-21 01:44:15.139451 dataclass_codec-0.5.3/src/dataclass_codec/py.typed
+-rw-r--r--   0        0        0    21509 2023-07-09 04:07:07.587053 dataclass_codec-0.5.3/src/dataclass_codec/tests/test_dataclass_codec.py
+-rw-r--r--   0        0        0      436 2023-07-09 03:52:02.877095 dataclass_codec-0.5.3/src/dataclass_codec/types_predicates.py
+-rw-r--r--   0        0        0    10596 1970-01-01 00:00:00.000000 dataclass_codec-0.5.3/PKG-INFO
```

### Comparing `dataclass_codec-0.5.2/README.md` & `dataclass_codec-0.5.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -168,10 +168,71 @@
     # The specified decoding context will be in effect
 ```
 
 By using the `decode_context_scope` context manager, you can easily control the decoding behavior within a specific scope, allowing you to customize options such as strict decoding, casting values, handling unset fields, and collecting errors.
 
 Feel free to include this section in your readme to explain the usage of `DecodeContext` and `decode_context_scope` for managing the decoding behavior within different contexts.
 
+Certainly! Here's an updated version of the section that includes a dataclass with a bytes property:
+
+## Bytes Encoding and Decoding (ID: `bytes-encoding-decoding`)
+
+The `dataclass_codec` library provides built-in support for encoding and decoding byte data, including working with bytes properties within dataclasses. You can easily encode byte data into a string representation and decode it back into its original byte form. This is useful when working with binary data or when serializing and deserializing byte data in your applications.
+
+### Encoding Bytes
+
+To encode byte data, you can use the `encode` function provided by the `dataclass_codec` library. The `encode` function takes a byte object as input and returns its string representation.
+
+Example:
+
+```python
+import base64
+from dataclasses import dataclass
+from dataclass_codec import encode
+
+@dataclass
+class MyData:
+    binary_data: bytes
+
+# Create an instance of the dataclass
+my_data = MyData(binary_data=b"Hello, world!")
+
+# Encode the byte data
+encoded_data = encode(my_data)
+
+# Print the encoded data
+print(encoded_data)  # Output: '{"binary_data": "SGVsbG8sIHdvcmxkIQ=="}'
+```
+
+In this example, we define a dataclass `MyData` with a `binary_data` property of type `bytes`. We create an instance of the dataclass and set the `binary_data` property to `b"Hello, world!"`. We then use the `encode` function to encode the dataclass instance, including the byte data. The resulting encoded data is `{"binary_data": "SGVsbG8sIHdvcmxkIQ=="}`. The byte data is encoded using Base64 encoding within the JSON representation of the dataclass instance.
+
+### Decoding Bytes
+
+To decode byte data back into its original form, you can use the `decode` function provided by the `dataclass_codec` library. The `decode` function takes the encoded data as a string and the target dataclass type and returns the decoded dataclass instance.
+
+Example:
+
+```python
+import base64
+from dataclasses import dataclass
+from dataclass_codec import decode
+
+@dataclass
+class MyData:
+    binary_data: bytes
+
+# Decode the encoded data
+decoded_data = decode({"binary_data": "SGVsbG8sIHdvcmxkIQ=="}, MyData)
+
+# Access the byte data
+print(decoded_data.binary_data)  # Output: b"Hello, world!"
+```
+
+In this example, we define the same `MyData` dataclass with a `binary_data` property of type `bytes`. We use the `decode` function to decode the encoded data `{"binary_data": "SGVsbG8sIHdvcmxkIQ=="}` back into its original dataclass form. The resulting decoded dataclass instance contains the byte data `b"Hello, world!"`.
+
+By leveraging the encoding and decoding capabilities provided by the `dataclass_codec` library, you can seamlessly work with byte data within dataclasses, ensuring efficient serialization and deserialization of binary data.
+
+Feel free to include this section in your readme to explain the process of encoding and decoding byte data, including working with bytes properties within dataclasses using the `dataclass_codec` library.
+
 ## Conclusion
 
 dataclass_codec is a powerful library for decoding dictionaries into dataclasses in Python. It provides an easy and efficient way to convert data between Python objects and JSON-compatible formats. Whether you need to deserialize data for processing or manipulation purposes, dataclass_codec can simplify the process and save you time. Give it a try and see how it can enhance your data manipulation workflow.
```

### Comparing `dataclass_codec-0.5.2/pyproject.toml` & `dataclass_codec-0.5.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataclass-codec"
-version = "0.5.2"
+version = "0.5.3"
 description = ""
 authors = ["lucas.silva <lucas.silva@jeaholding.com.br>"]
 readme = "README.md"
 packages = [{include = "dataclass_codec", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `dataclass_codec-0.5.2/src/dataclass_codec/decode.py` & `dataclass_codec-0.5.3/src/dataclass_codec/decode.py`

 * *Files identical despite different names*

### Comparing `dataclass_codec-0.5.2/src/dataclass_codec/encode.py` & `dataclass_codec-0.5.3/src/dataclass_codec/encode.py`

 * *Files identical despite different names*

### Comparing `dataclass_codec-0.5.2/src/dataclass_codec/tests/test_dataclass_codec.py` & `dataclass_codec-0.5.3/src/dataclass_codec/tests/test_dataclass_codec.py`

 * *Files identical despite different names*

### Comparing `dataclass_codec-0.5.2/PKG-INFO` & `dataclass_codec-0.5.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataclass-codec
-Version: 0.5.2
+Version: 0.5.3
 Summary: 
 Author: lucas.silva
 Author-email: lucas.silva@jeaholding.com.br
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -182,11 +182,72 @@
     # The specified decoding context will be in effect
 ```
 
 By using the `decode_context_scope` context manager, you can easily control the decoding behavior within a specific scope, allowing you to customize options such as strict decoding, casting values, handling unset fields, and collecting errors.
 
 Feel free to include this section in your readme to explain the usage of `DecodeContext` and `decode_context_scope` for managing the decoding behavior within different contexts.
 
+Certainly! Here's an updated version of the section that includes a dataclass with a bytes property:
+
+## Bytes Encoding and Decoding (ID: `bytes-encoding-decoding`)
+
+The `dataclass_codec` library provides built-in support for encoding and decoding byte data, including working with bytes properties within dataclasses. You can easily encode byte data into a string representation and decode it back into its original byte form. This is useful when working with binary data or when serializing and deserializing byte data in your applications.
+
+### Encoding Bytes
+
+To encode byte data, you can use the `encode` function provided by the `dataclass_codec` library. The `encode` function takes a byte object as input and returns its string representation.
+
+Example:
+
+```python
+import base64
+from dataclasses import dataclass
+from dataclass_codec import encode
+
+@dataclass
+class MyData:
+    binary_data: bytes
+
+# Create an instance of the dataclass
+my_data = MyData(binary_data=b"Hello, world!")
+
+# Encode the byte data
+encoded_data = encode(my_data)
+
+# Print the encoded data
+print(encoded_data)  # Output: '{"binary_data": "SGVsbG8sIHdvcmxkIQ=="}'
+```
+
+In this example, we define a dataclass `MyData` with a `binary_data` property of type `bytes`. We create an instance of the dataclass and set the `binary_data` property to `b"Hello, world!"`. We then use the `encode` function to encode the dataclass instance, including the byte data. The resulting encoded data is `{"binary_data": "SGVsbG8sIHdvcmxkIQ=="}`. The byte data is encoded using Base64 encoding within the JSON representation of the dataclass instance.
+
+### Decoding Bytes
+
+To decode byte data back into its original form, you can use the `decode` function provided by the `dataclass_codec` library. The `decode` function takes the encoded data as a string and the target dataclass type and returns the decoded dataclass instance.
+
+Example:
+
+```python
+import base64
+from dataclasses import dataclass
+from dataclass_codec import decode
+
+@dataclass
+class MyData:
+    binary_data: bytes
+
+# Decode the encoded data
+decoded_data = decode({"binary_data": "SGVsbG8sIHdvcmxkIQ=="}, MyData)
+
+# Access the byte data
+print(decoded_data.binary_data)  # Output: b"Hello, world!"
+```
+
+In this example, we define the same `MyData` dataclass with a `binary_data` property of type `bytes`. We use the `decode` function to decode the encoded data `{"binary_data": "SGVsbG8sIHdvcmxkIQ=="}` back into its original dataclass form. The resulting decoded dataclass instance contains the byte data `b"Hello, world!"`.
+
+By leveraging the encoding and decoding capabilities provided by the `dataclass_codec` library, you can seamlessly work with byte data within dataclasses, ensuring efficient serialization and deserialization of binary data.
+
+Feel free to include this section in your readme to explain the process of encoding and decoding byte data, including working with bytes properties within dataclasses using the `dataclass_codec` library.
+
 ## Conclusion
 
 dataclass_codec is a powerful library for decoding dictionaries into dataclasses in Python. It provides an easy and efficient way to convert data between Python objects and JSON-compatible formats. Whether you need to deserialize data for processing or manipulation purposes, dataclass_codec can simplify the process and save you time. Give it a try and see how it can enhance your data manipulation workflow.
```

