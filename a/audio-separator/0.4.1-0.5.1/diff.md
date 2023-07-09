# Comparing `tmp/audio_separator-0.4.1.tar.gz` & `tmp/audio_separator-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audio_separator-0.4.1.tar", max compression
+gzip compressed data, was "audio_separator-0.5.1.tar", max compression
```

## Comparing `audio_separator-0.4.1.tar` & `audio_separator-0.5.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-07-09 20:38:13.444192 audio_separator-0.4.1/LICENSE
--rw-r--r--   0        0        0     7479 2023-07-09 20:38:13.444192 audio_separator-0.4.1/README.md
--rw-r--r--   0        0        0       33 2023-07-09 20:38:13.444192 audio_separator-0.4.1/audio_separator/__init__.py
--rw-r--r--   0        0        0    12397 2023-07-09 20:38:13.444192 audio_separator-0.4.1/audio_separator/separator.py
--rw-r--r--   0        0        0        0 2023-07-09 20:38:13.444192 audio_separator-0.4.1/audio_separator/utils/__init__.py
--rwxr-xr-x   0        0        0     2520 2023-07-09 20:38:13.444192 audio_separator-0.4.1/audio_separator/utils/cli.py
--rw-r--r--   0        0        0    21906 2023-07-09 20:38:13.444192 audio_separator-0.4.1/audio_separator/utils/spec_utils.py
--rw-r--r--   0        0        0      991 2023-07-09 20:38:13.448192 audio_separator-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     8549 1970-01-01 00:00:00.000000 audio_separator-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-09 20:53:03.831268 audio_separator-0.5.1/LICENSE
+-rw-r--r--   0        0        0     7479 2023-07-09 20:53:03.831268 audio_separator-0.5.1/README.md
+-rw-r--r--   0        0        0       33 2023-07-09 20:53:03.831268 audio_separator-0.5.1/audio_separator/__init__.py
+-rw-r--r--   0        0        0    12879 2023-07-09 20:53:03.835268 audio_separator-0.5.1/audio_separator/separator.py
+-rw-r--r--   0        0        0        0 2023-07-09 20:53:03.835268 audio_separator-0.5.1/audio_separator/utils/__init__.py
+-rwxr-xr-x   0        0        0     2520 2023-07-09 20:53:03.835268 audio_separator-0.5.1/audio_separator/utils/cli.py
+-rw-r--r--   0        0        0    21906 2023-07-09 20:53:03.835268 audio_separator-0.5.1/audio_separator/utils/spec_utils.py
+-rw-r--r--   0        0        0      985 2023-07-09 20:53:03.835268 audio_separator-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     8539 1970-01-01 00:00:00.000000 audio_separator-0.5.1/PKG-INFO
```

### Comparing `audio_separator-0.4.1/LICENSE` & `audio_separator-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `audio_separator-0.4.1/README.md` & `audio_separator-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `audio_separator-0.4.1/audio_separator/separator.py` & `audio_separator-0.5.1/audio_separator/separator.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,17 +79,27 @@
         self.primary_source = None
         self.secondary_source = None
 
         warnings.filterwarnings("ignore")
         self.cpu = torch.device("cpu")
 
         if self.use_cuda:
-            self.logger.debug("Running in GPU mode")
-            self.device = torch.device("cuda")
-            self.run_type = ["CUDAExecutionProvider"]
+            self.logger.debug("CUDA requested, checking Torch version and CUDA status")
+            self.logger.debug(f"Torch version: {str(torch.__version__)}")
+
+            cuda_available = torch.cuda.is_available()
+            self.logger.debug(f"Is CUDA enabled? {str(cuda_available)}")
+
+            if cuda_available:
+                self.logger.debug("Running in GPU mode")
+                self.device = torch.device("cuda")
+                self.run_type = ["CUDAExecutionProvider"]
+            else:
+                raise Exception("CUDA requested but not available with current Torch installation. Do you have an Nvidia GPU?")
+
         else:
             self.logger.debug("Running in CPU mode")
             self.device = torch.device("cpu")
             self.run_type = ["CPUExecutionProvider"]
 
     def get_model_hash(self, model_path):
         try:
```

### Comparing `audio_separator-0.4.1/audio_separator/utils/cli.py` & `audio_separator-0.5.1/audio_separator/utils/cli.py`

 * *Files identical despite different names*

### Comparing `audio_separator-0.4.1/audio_separator/utils/spec_utils.py` & `audio_separator-0.5.1/audio_separator/utils/spec_utils.py`

 * *Files identical despite different names*

### Comparing `audio_separator-0.4.1/pyproject.toml` & `audio_separator-0.5.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "audio-separator"
-version = "0.4.1"
+version = "0.5.1"
 description = "Easy to use vocal separation on CLI or as a python package, using the amazing MDX-Net models from UVR trained by @Anjok07"
 authors = ["Andrew Beveridge <andrew@beveridge.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "audio_separator"}]
 homepage = "https://github.com/karaokenerds/python-audio-separator"
 repository = "https://github.com/karaokenerds/python-audio-separator"
 documentation = "https://github.com/karaokenerds/python-audio-separator/blob/main/README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
 onnx = "^1.14.0"
-onnxruntime = "^1.13"
+onnxruntime = "^1"
 numpy = "^1.23"
 soundfile = "^0.11"
 librosa = "^0.9"
-torch = "^1.13"
+torch = "^2"
 wget = "^3"
 six = "^1.16"
 
 [tool.poetry.scripts]
 audio-separator = 'audio_separator.utils.cli:main'
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `audio_separator-0.4.1/PKG-INFO` & `audio_separator-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: audio-separator
-Version: 0.4.1
+Version: 0.5.1
 Summary: Easy to use vocal separation on CLI or as a python package, using the amazing MDX-Net models from UVR trained by @Anjok07
 Home-page: https://github.com/karaokenerds/python-audio-separator
 License: MIT
 Author: Andrew Beveridge
 Author-email: andrew@beveridge.uk
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: librosa (>=0.9,<0.10)
 Requires-Dist: numpy (>=1.23,<2.0)
 Requires-Dist: onnx (>=1.14.0,<2.0.0)
-Requires-Dist: onnxruntime (>=1.13,<2.0)
+Requires-Dist: onnxruntime (>=1,<2)
 Requires-Dist: six (>=1.16,<2.0)
 Requires-Dist: soundfile (>=0.11,<0.12)
-Requires-Dist: torch (>=1.13,<2.0)
+Requires-Dist: torch (>=2,<3)
 Requires-Dist: wget (>=3,<4)
 Project-URL: Documentation, https://github.com/karaokenerds/python-audio-separator/blob/main/README.md
 Project-URL: Repository, https://github.com/karaokenerds/python-audio-separator
 Description-Content-Type: text/markdown
 
 # Audio Separator 🎶
```

