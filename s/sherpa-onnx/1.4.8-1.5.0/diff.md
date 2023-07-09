# Comparing `tmp/sherpa-onnx-1.4.8.tar.gz` & `tmp/sherpa-onnx-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sherpa-onnx-1.4.8.tar", last modified: Sun Jul  2 16:08:34 2023, max compression
+gzip compressed data, was "sherpa-onnx-1.5.0.tar", last modified: Sun Jul  9 07:03:52 2023, max compression
```

## Comparing `sherpa-onnx-1.4.8.tar` & `sherpa-onnx-1.5.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:08:34.421527 sherpa-onnx-1.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-02 15:57:43.000000 sherpa-onnx-1.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-02 16:08:34.421527 sherpa-onnx-1.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-02 15:57:43.000000 sherpa-onnx-1.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 16:08:34.421527 sherpa-onnx-1.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-02 15:57:43.000000 sherpa-onnx-1.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:08:34.421527 sherpa-onnx-1.4.8/sherpa-onnx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:08:34.421527 sherpa-onnx-1.4.8/sherpa-onnx/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:08:34.421527 sherpa-onnx-1.4.8/sherpa-onnx/python/sherpa_onnx/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-02 16:08:34.000000 sherpa-onnx-1.4.8/sherpa-onnx/python/sherpa_onnx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-07-02 15:57:43.000000 sherpa-onnx-1.4.8/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-07-02 15:57:43.000000 sherpa-onnx-1.4.8/sherpa-onnx/python/sherpa_onnx/online_recognizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-02 15:57:43.000000 sherpa-onnx-1.4.8/sherpa-onnx/python/sherpa_onnx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:08:34.421527 sherpa-onnx-1.4.8/sherpa_onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-02 16:08:34.000000 sherpa-onnx-1.4.8/sherpa_onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-02 16:08:34.000000 sherpa-onnx-1.4.8/sherpa_onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 16:08:34.000000 sherpa-onnx-1.4.8/sherpa_onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 16:08:34.000000 sherpa-onnx-1.4.8/sherpa_onnx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-02 16:08:34.000000 sherpa-onnx-1.4.8/sherpa_onnx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-02 16:08:34.000000 sherpa-onnx-1.4.8/sherpa_onnx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:03:52.945250 sherpa-onnx-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-09 06:50:35.000000 sherpa-onnx-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-09 07:03:52.945250 sherpa-onnx-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-09 06:50:35.000000 sherpa-onnx-1.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 07:03:52.945250 sherpa-onnx-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-09 06:50:35.000000 sherpa-onnx-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:03:52.941250 sherpa-onnx-1.5.0/sherpa-onnx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:03:52.941250 sherpa-onnx-1.5.0/sherpa-onnx/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:03:52.945250 sherpa-onnx-1.5.0/sherpa-onnx/python/sherpa_onnx/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-09 07:03:52.000000 sherpa-onnx-1.5.0/sherpa-onnx/python/sherpa_onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-07-09 06:50:35.000000 sherpa-onnx-1.5.0/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-07-09 06:50:35.000000 sherpa-onnx-1.5.0/sherpa-onnx/python/sherpa_onnx/online_recognizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-09 06:50:35.000000 sherpa-onnx-1.5.0/sherpa-onnx/python/sherpa_onnx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:03:52.945250 sherpa-onnx-1.5.0/sherpa_onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-09 07:03:52.000000 sherpa-onnx-1.5.0/sherpa_onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-09 07:03:52.000000 sherpa-onnx-1.5.0/sherpa_onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 07:03:52.000000 sherpa-onnx-1.5.0/sherpa_onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 07:03:52.000000 sherpa-onnx-1.5.0/sherpa_onnx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-09 07:03:52.000000 sherpa-onnx-1.5.0/sherpa_onnx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-09 07:03:52.000000 sherpa-onnx-1.5.0/sherpa_onnx.egg-info/top_level.txt
```

### Comparing `sherpa-onnx-1.4.8/LICENSE` & `sherpa-onnx-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.4.8/PKG-INFO` & `sherpa-onnx-1.5.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sherpa-onnx
-Version: 1.4.8
+Version: 1.5.0
 Summary: UNKNOWN
 Home-page: https://github.com/k2-fsa/sherpa-onnx
 Author: The sherpa-onnx development team
 Author-email: dpovey@gmail.com
 License: Apache licensed, as found in the LICENSE file
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
```

### Comparing `sherpa-onnx-1.4.8/setup.py` & `sherpa-onnx-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.4.8/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py` & `sherpa-onnx-1.5.0/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,14 +108,15 @@
         paraformer: str,
         tokens: str,
         num_threads: int,
         sample_rate: int = 16000,
         feature_dim: int = 80,
         decoding_method: str = "greedy_search",
         debug: bool = False,
+        provider: str = "cpu",
     ):
         """
         Please refer to
         `<https://k2-fsa.github.io/sherpa/onnx/pretrained_models/index.html>`_
         to download pre-trained models for different languages, e.g., Chinese,
         English, etc.
 
@@ -134,21 +135,24 @@
             Sample rate of the training data used to train the model.
           feature_dim:
             Dimension of the feature used to train the model.
           decoding_method:
             Valid values are greedy_search, modified_beam_search.
           debug:
             True to show debug messages.
+          provider:
+            onnxruntime execution providers. Valid values are: cpu, cuda, coreml.
         """
         self = cls.__new__(cls)
         model_config = OfflineModelConfig(
             paraformer=OfflineParaformerModelConfig(model=paraformer),
             tokens=tokens,
             num_threads=num_threads,
             debug=debug,
+            provider=provider,
         )
 
         feat_config = OfflineFeatureExtractorConfig(
             sampling_rate=sample_rate,
             feature_dim=feature_dim,
         )
 
@@ -166,14 +170,15 @@
         model: str,
         tokens: str,
         num_threads: int,
         sample_rate: int = 16000,
         feature_dim: int = 80,
         decoding_method: str = "greedy_search",
         debug: bool = False,
+        provider: str = "cpu",
     ):
         """
         Please refer to
         `<https://k2-fsa.github.io/sherpa/onnx/pretrained_models/index.html>`_
         to download pre-trained models for different languages, e.g., Chinese,
         English, etc.
 
@@ -192,21 +197,24 @@
             Sample rate of the training data used to train the model.
           feature_dim:
             Dimension of the feature used to train the model.
           decoding_method:
             Valid values are greedy_search, modified_beam_search.
           debug:
             True to show debug messages.
+          provider:
+            onnxruntime execution providers. Valid values are: cpu, cuda, coreml.
         """
         self = cls.__new__(cls)
         model_config = OfflineModelConfig(
             nemo_ctc=OfflineNemoEncDecCtcModelConfig(model=model),
             tokens=tokens,
             num_threads=num_threads,
             debug=debug,
+            provider=provider,
         )
 
         feat_config = OfflineFeatureExtractorConfig(
             sampling_rate=sample_rate,
             feature_dim=feature_dim,
         )
```

### Comparing `sherpa-onnx-1.4.8/sherpa-onnx/python/sherpa_onnx/online_recognizer.py` & `sherpa-onnx-1.5.0/sherpa-onnx/python/sherpa_onnx/online_recognizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
             max_active_paths=max_active_paths,
             context_score=context_score,
         )
 
         self.recognizer = _Recognizer(recognizer_config)
         self.config = recognizer_config
 
-    def create_stream(self, contexts_list : Optional[List[List[int]]] = None):
+    def create_stream(self, contexts_list: Optional[List[List[int]]] = None):
         if contexts_list is None:
             return self.recognizer.create_stream()
         else:
             return self.recognizer.create_stream(contexts_list)
 
     def decode_stream(self, s: OnlineStream):
         self.recognizer.decode_stream(s)
```

### Comparing `sherpa-onnx-1.4.8/sherpa-onnx/python/sherpa_onnx/utils.py` & `sherpa-onnx-1.5.0/sherpa-onnx/python/sherpa_onnx/utils.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.4.8/sherpa_onnx.egg-info/PKG-INFO` & `sherpa-onnx-1.5.0/sherpa_onnx.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sherpa-onnx
-Version: 1.4.8
+Version: 1.5.0
 Summary: UNKNOWN
 Home-page: https://github.com/k2-fsa/sherpa-onnx
 Author: The sherpa-onnx development team
 Author-email: dpovey@gmail.com
 License: Apache licensed, as found in the LICENSE file
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
```

