# Comparing `tmp/prefecto-0.0.3.tar.gz` & `tmp/prefecto-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefecto-0.0.3.tar", last modified: Wed Jun 21 22:25:24 2023, max compression
+gzip compressed data, was "prefecto-0.0.4.tar", last modified: Sun Jul  9 20:48:48 2023, max compression
```

## Comparing `prefecto-0.0.3.tar` & `prefecto-0.0.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:25:24.247321 prefecto-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-21 22:24:34.000000 prefecto-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-21 22:25:24.247321 prefecto-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-21 22:24:34.000000 prefecto-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-21 22:24:34.000000 prefecto-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-21 22:25:24.247321 prefecto-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-06-21 22:24:34.000000 prefecto-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:25:24.243321 prefecto-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:25:24.247321 prefecto-0.0.3/src/prefecto/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-21 22:24:34.000000 prefecto-0.0.3/src/prefecto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-21 22:25:24.247321 prefecto-0.0.3/src/prefecto/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-06-21 22:24:34.000000 prefecto-0.0.3/src/prefecto/concurrency.py
--rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-06-21 22:24:34.000000 prefecto-0.0.3/src/prefecto/filesystems.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-21 22:24:34.000000 prefecto-0.0.3/src/prefecto/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:25:24.247321 prefecto-0.0.3/src/prefecto/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-21 22:24:34.000000 prefecto-0.0.3/src/prefecto/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-06-21 22:24:34.000000 prefecto-0.0.3/src/prefecto/serializers/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-06-21 22:24:34.000000 prefecto-0.0.3/src/prefecto/serializers/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-06-21 22:24:34.000000 prefecto-0.0.3/src/prefecto/serializers/polars.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-21 22:24:34.000000 prefecto-0.0.3/src/prefecto/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:25:24.247321 prefecto-0.0.3/src/prefecto/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:24:34.000000 prefecto-0.0.3/src/prefecto/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-21 22:24:34.000000 prefecto-0.0.3/src/prefecto/testing/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:25:24.247321 prefecto-0.0.3/src/prefecto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-21 22:25:24.000000 prefecto-0.0.3/src/prefecto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-21 22:25:24.000000 prefecto-0.0.3/src/prefecto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 22:25:24.000000 prefecto-0.0.3/src/prefecto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-21 22:25:24.000000 prefecto-0.0.3/src/prefecto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-21 22:25:24.000000 prefecto-0.0.3/src/prefecto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 22:24:42.000000 prefecto-0.0.3/src/prefecto.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:25:24.247321 prefecto-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-21 22:24:34.000000 prefecto-0.0.3/tests/test_concurrency.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-21 22:24:34.000000 prefecto-0.0.3/tests/test_filesystems.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-21 22:24:34.000000 prefecto-0.0.3/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-06-21 22:24:34.000000 prefecto-0.0.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:48:48.616073 prefecto-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-09 20:48:08.000000 prefecto-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-09 20:48:48.616073 prefecto-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-09 20:48:08.000000 prefecto-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-09 20:48:08.000000 prefecto-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-09 20:48:48.616073 prefecto-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-09 20:48:08.000000 prefecto-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:48:48.612073 prefecto-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:48:48.612073 prefecto-0.0.4/src/prefecto/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-09 20:48:08.000000 prefecto-0.0.4/src/prefecto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-09 20:48:48.616073 prefecto-0.0.4/src/prefecto/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-07-09 20:48:08.000000 prefecto-0.0.4/src/prefecto/concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-07-09 20:48:08.000000 prefecto-0.0.4/src/prefecto/filesystems.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-09 20:48:08.000000 prefecto-0.0.4/src/prefecto/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:48:48.616073 prefecto-0.0.4/src/prefecto/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-09 20:48:08.000000 prefecto-0.0.4/src/prefecto/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-07-09 20:48:08.000000 prefecto-0.0.4/src/prefecto/serializers/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-07-09 20:48:08.000000 prefecto-0.0.4/src/prefecto/serializers/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-09 20:48:08.000000 prefecto-0.0.4/src/prefecto/serializers/polars.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-09 20:48:08.000000 prefecto-0.0.4/src/prefecto/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:48:48.616073 prefecto-0.0.4/src/prefecto/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 20:48:08.000000 prefecto-0.0.4/src/prefecto/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-07-09 20:48:08.000000 prefecto-0.0.4/src/prefecto/testing/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:48:48.616073 prefecto-0.0.4/src/prefecto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-09 20:48:48.000000 prefecto-0.0.4/src/prefecto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-09 20:48:48.000000 prefecto-0.0.4/src/prefecto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 20:48:48.000000 prefecto-0.0.4/src/prefecto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-09 20:48:48.000000 prefecto-0.0.4/src/prefecto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-09 20:48:48.000000 prefecto-0.0.4/src/prefecto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 20:48:14.000000 prefecto-0.0.4/src/prefecto.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:48:48.616073 prefecto-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-09 20:48:08.000000 prefecto-0.0.4/tests/test_concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-09 20:48:08.000000 prefecto-0.0.4/tests/test_filesystems.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-09 20:48:08.000000 prefecto-0.0.4/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-07-09 20:48:08.000000 prefecto-0.0.4/versioneer.py
```

### Comparing `prefecto-0.0.3/LICENSE` & `prefecto-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `prefecto-0.0.3/PKG-INFO` & `prefecto-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefecto
-Version: 0.0.3
+Version: 0.0.4
 Summary: Prefect development aid.
 Home-page: https://github.com/dominictarro/prefecto
 Author: Dominic Tarro
 Author-email: dtarro@oxfordeconomics.com
 Project-URL: Documentation, https://dominictarro.github.io/prefecto/
 Project-URL: Source, https://github.com/dominictarro/prefecto
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prefecto Version: 0.0.3 Summary: Prefect
+Metadata-Version: 2.1 Name: prefecto Version: 0.0.4 Summary: Prefect
 development aid. Home-page: https://github.com/dominictarro/prefecto Author:
 Dominic Tarro Author-email: dtarro@oxfordeconomics.com Project-URL:
 Documentation, https://dominictarro.github.io/prefecto/ Project-URL: Source,
 https://github.com/dominictarro/prefecto Classifier: Natural Language ::
 English Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: System Administrators Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 :: Only Classifier:
```

### Comparing `prefecto-0.0.3/README.md` & `prefecto-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `prefecto-0.0.3/pyproject.toml` & `prefecto-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `prefecto-0.0.3/setup.py` & `prefecto-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `prefecto-0.0.3/src/prefecto/concurrency.py` & `prefecto-0.0.4/src/prefecto/concurrency.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,25 +75,26 @@
                     raise ValueError(
                         f"Expected all iterables to be of length {length} like "
                         f"'{parameters[0]}'. '{k}' is length {len(params[k])}."
                     )
 
         batches = []
 
+        i = 0
         for i in range(length // self.size):
             batch = {p: [] for p in parameters}
             for p in parameters:
                 batch[p] = params[p][i * self.size : (i + 1) * self.size]
             batches.append(batch)
 
         # Add the remainder if there is one
         if length % self.size != 0:
             batch = {p: [] for p in parameters}
             for p in parameters:
-                batch[p] = params[p][(i + 1) * self.size :]
+                batch[p] = params[p][(length // self.size) * self.size :]
             batches.append(batch)
 
         return batches
 
     def map(self, *args, **kwds) -> list[PrefectFuture]:
         """Perform a `Task.map` operation in batches of the keyword arguments. The
         arguments must be iterables of equal length.
@@ -159,14 +160,16 @@
         Args:
             batches (list[dict[str, list[Any]]]): Batches of arguments to pass to
             `Task.map`.
 
         Returns:
             A list of futures for each batch.
         """
+        if len(batches) == 0:
+            return []
         logger = logging.get_prefect_or_default_logger()
         results: list[PrefectFuture] = []
         for i, batch in enumerate(batches[:-1]):
             logger.debug(f"Mapping {self.task.name} batch {i+1} of {len(batches)}.")
             # Map the batch
             futures = self.task.map(**batch)
             results.extend(futures)
```

### Comparing `prefecto-0.0.3/src/prefecto/filesystems.py` & `prefecto-0.0.4/src/prefecto/filesystems.py`

 * *Files identical despite different names*

### Comparing `prefecto-0.0.3/src/prefecto/logging.py` & `prefecto-0.0.4/src/prefecto/logging.py`

 * *Files identical despite different names*

### Comparing `prefecto-0.0.3/src/prefecto/serializers/core.py` & `prefecto-0.0.4/src/prefecto/serializers/core.py`

 * *Files identical despite different names*

### Comparing `prefecto-0.0.3/src/prefecto/serializers/pandas.py` & `prefecto-0.0.4/src/prefecto/serializers/pandas.py`

 * *Files identical despite different names*

### Comparing `prefecto-0.0.3/src/prefecto/serializers/polars.py` & `prefecto-0.0.4/src/prefecto/serializers/polars.py`

 * *Files 7% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
 @ExtendedSerializer.register
 class PolarsSerializer(ExtendedSerializer):
     """Serializer for `polars.DataFrame` objects.
 
     Args:
         method (str, optional): The method to use for reading and writing.
-            Must be a registered `Method`. Defaults to "polars.tsv".
+            Must be a registered `Method`. Defaults to "polars.parquet".
         read_kwargs (dict[str, Any], optional): Keyword arguments for the read
             method. Overrides default arguments for the method.
         write_kwargs (dict[str, Any], optional): Keyword arguments for the
             write method. Overrides default arguments for the method.
 
     Examples:
         Simple read and write.
```

### Comparing `prefecto-0.0.3/src/prefecto/states.py` & `prefecto-0.0.4/src/prefecto/states.py`

 * *Files identical despite different names*

### Comparing `prefecto-0.0.3/src/prefecto/testing/s3.py` & `prefecto-0.0.4/src/prefecto/testing/s3.py`

 * *Files identical despite different names*

### Comparing `prefecto-0.0.3/src/prefecto.egg-info/PKG-INFO` & `prefecto-0.0.4/src/prefecto.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefecto
-Version: 0.0.3
+Version: 0.0.4
 Summary: Prefect development aid.
 Home-page: https://github.com/dominictarro/prefecto
 Author: Dominic Tarro
 Author-email: dtarro@oxfordeconomics.com
 Project-URL: Documentation, https://dominictarro.github.io/prefecto/
 Project-URL: Source, https://github.com/dominictarro/prefecto
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prefecto Version: 0.0.3 Summary: Prefect
+Metadata-Version: 2.1 Name: prefecto Version: 0.0.4 Summary: Prefect
 development aid. Home-page: https://github.com/dominictarro/prefecto Author:
 Dominic Tarro Author-email: dtarro@oxfordeconomics.com Project-URL:
 Documentation, https://dominictarro.github.io/prefecto/ Project-URL: Source,
 https://github.com/dominictarro/prefecto Classifier: Natural Language ::
 English Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: System Administrators Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 :: Only Classifier:
```

### Comparing `prefecto-0.0.3/src/prefecto.egg-info/SOURCES.txt` & `prefecto-0.0.4/src/prefecto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prefecto-0.0.3/tests/test_concurrency.py` & `prefecto-0.0.4/tests/test_concurrency.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Unit tests for the `concurrency` module.
 
 """
 from __future__ import annotations
 
+import pytest
 from prefect import flow, task
 
 from prefecto.concurrency import BatchTask
 
 
 @task
 def add(a, b):
@@ -19,23 +20,31 @@
     """Unit tests for `BatchTask`."""
 
     def test_make_batches(self):
         """Test `_make_batches`."""
         batches = BatchTask(add, 3)._make_batches(a=[1, 2, 3, 4, 5], b=[2, 3, 4, 5, 6])
         assert batches == [{"a": [1, 2, 3], "b": [2, 3, 4]}, {"a": [4, 5], "b": [5, 6]}]
 
-    def test_map(self, harness):
+    @pytest.mark.parametrize(
+        "a,b,expectation",
+        [
+            ([1, 2, 3, 4, 5], [2, 3, 4, 5, 6], [3, 5, 7, 9, 11]),
+            ([1, 2], [2, 3], [3, 5]),
+            ([], [], []),
+        ],
+    )
+    def test_map(self, a: list[int], b: list[int], expectation: list[int], harness):
         """Test `BatchTask.map`."""
 
         @task
         def realize(futures: list[int]):
             """Converts futures to their values."""
             return futures
 
         @flow
         def test() -> list[int]:
             """Test flow."""
-            futures = BatchTask(add, 3).map([1, 2, 3, 4, 5], [2, 3, 4, 5, 6])
+            futures = BatchTask(add, 3).map(a, b)
             return realize(futures)
 
         result = test()
-        assert result == [3, 5, 7, 9, 11]
+        assert result == expectation
```

### Comparing `prefecto-0.0.3/tests/test_filesystems.py` & `prefecto-0.0.4/tests/test_filesystems.py`

 * *Files identical despite different names*

### Comparing `prefecto-0.0.3/versioneer.py` & `prefecto-0.0.4/versioneer.py`

 * *Files identical despite different names*

