# Comparing `tmp/audio_separator-0.3.4.tar.gz` & `tmp/audio_separator-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audio_separator-0.3.4.tar", max compression
+gzip compressed data, was "audio_separator-0.4.1.tar", max compression
```

## Comparing `audio_separator-0.3.4.tar` & `audio_separator-0.4.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-07-07 23:30:53.386155 audio_separator-0.3.4/LICENSE
--rw-r--r--   0        0        0     7239 2023-07-07 23:30:53.386155 audio_separator-0.3.4/README.md
--rw-r--r--   0        0        0       33 2023-07-07 23:30:53.386155 audio_separator-0.3.4/audio_separator/__init__.py
--rw-r--r--   0        0        0    11986 2023-07-07 23:30:53.390156 audio_separator-0.3.4/audio_separator/separator.py
--rw-r--r--   0        0        0        0 2023-07-07 23:30:53.390156 audio_separator-0.3.4/audio_separator/utils/__init__.py
--rwxr-xr-x   0        0        0     2333 2023-07-07 23:30:53.390156 audio_separator-0.3.4/audio_separator/utils/cli.py
--rw-r--r--   0        0        0    21906 2023-07-07 23:30:53.390156 audio_separator-0.3.4/audio_separator/utils/spec_utils.py
--rw-r--r--   0        0        0      760 2023-07-07 23:30:53.390156 audio_separator-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     8060 1970-01-01 00:00:00.000000 audio_separator-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-09 20:38:13.444192 audio_separator-0.4.1/LICENSE
+-rw-r--r--   0        0        0     7479 2023-07-09 20:38:13.444192 audio_separator-0.4.1/README.md
+-rw-r--r--   0        0        0       33 2023-07-09 20:38:13.444192 audio_separator-0.4.1/audio_separator/__init__.py
+-rw-r--r--   0        0        0    12397 2023-07-09 20:38:13.444192 audio_separator-0.4.1/audio_separator/separator.py
+-rw-r--r--   0        0        0        0 2023-07-09 20:38:13.444192 audio_separator-0.4.1/audio_separator/utils/__init__.py
+-rwxr-xr-x   0        0        0     2520 2023-07-09 20:38:13.444192 audio_separator-0.4.1/audio_separator/utils/cli.py
+-rw-r--r--   0        0        0    21906 2023-07-09 20:38:13.444192 audio_separator-0.4.1/audio_separator/utils/spec_utils.py
+-rw-r--r--   0        0        0      991 2023-07-09 20:38:13.448192 audio_separator-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     8549 1970-01-01 00:00:00.000000 audio_separator-0.4.1/PKG-INFO
```

### Comparing `audio_separator-0.3.4/LICENSE` & `audio_separator-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `audio_separator-0.3.4/README.md` & `audio_separator-0.4.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -29,20 +29,21 @@
 
 You can use Audio Separator via the command line:
 
 ```sh
 audio-separator [audio_file] --model_name [model_name]
     
     audio_file: The path to the audio file to be separated. Supports all common formats (WAV, MP3, FLAC, M4A, etc.)
+    log_level: (Optional) Logging level, e.g. info, debug, warning. Default: INFO
+    log_formatter: (Optional) The log format. Default: '%(asctime)s - %(name)s - %(levelname)s - %(message)s'
     model_name: (Optional) The name of the model to use for separation. Default: UVR_MDXNET_KARA_2
     model_file_dir: (Optional) Directory to cache model files in. Default: /tmp/audio-separator-models/
     output_dir: (Optional) The directory where the separated files will be saved. If not specified, outputs to current dir.
     use_cuda: (Optional) Flag to use Nvidia GPU via CUDA for separation if available. Default: False
-    log_level: (Optional) Logging level, e.g. info, debug, warning. Default: INFO
-    log_formatter: (Optional) The log format. Default: '%(asctime)s - %(name)s - %(levelname)s - %(message)s'
+    output_format: (Optional) Format to encode output files, any common format (WAV, MP3, FLAC, M4A, etc.). Default: WAV
 ```
 
 Example:
 
 ```
 audio-separator /path/to/your/audio.wav --model_name UVR_MDXNET_KARA_2
 ```
@@ -65,20 +66,21 @@
 print(f'Primary stem saved at {primary_stem_path}')
 print(f'Secondary stem saved at {secondary_stem_path}')
 ```
 
 ## Parameters for the Separator class
 
 - audio_file: The path to the audio file to be separated. Supports all common formats (WAV, MP3, FLAC, M4A, etc.)
+- log_level: (Optional) Logging level, e.g. info, debug, warning. Default: INFO
+- log_formatter: (Optional) The log format. Default: '%(asctime)s - %(name)s - %(levelname)s - %(message)s'
 - model_name: (Optional) The name of the model to use for separation. Defaults to 'UVR_MDXNET_KARA_2', a very powerful model for Karaoke instrumental tracks.
 - model_file_dir: (Optional) Directory to cache model files in. Default: /tmp/audio-separator-models/
 - output_dir: (Optional) Directory where the separated files will be saved. If not specified, outputs to current dir.
 - use_cuda: (Optional) Flag to use Nvidia GPU via CUDA for separation if available. Default: False
-- log_level: (Optional) Logging level, e.g. info, debug, warning. Default: INFO
-- log_formatter: (Optional) The log format. Default: '%(asctime)s - %(name)s - %(levelname)s - %(message)s'
+- output_format: (Optional) Format to encode output files, any common format (WAV, MP3, FLAC, M4A, etc.). Default: WAV
 
 ## Requirements 📋
 
 Python <= 3.10 (one of the dependencies doesn't like 3.11 yet)
 
 Libraries: onnx, onnxruntime, numpy, soundfile, librosa, torch, wget, six
```

### Comparing `audio_separator-0.3.4/audio_separator/separator.py` & `audio_separator-0.4.1/audio_separator/separator.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,20 +13,22 @@
 from audio_separator.utils import spec_utils
 
 
 class Separator:
     def __init__(
         self,
         audio_file_path,
+        log_level=logging.DEBUG,
+        log_formatter=None,
         model_name="UVR_MDXNET_KARA_2",
         model_file_dir="/tmp/audio-separator-models/",
         output_dir=None,
         use_cuda=False,
-        log_level=logging.DEBUG,
-        log_formatter=None,
+        output_format="WAV",
+        output_subtype=None,
     ):
         self.logger = logging.getLogger(__name__)
         self.logger.setLevel(log_level)
         self.log_level = log_level
         self.log_formatter = log_formatter
 
         self.log_handler = logging.StreamHandler()
@@ -34,15 +36,15 @@
         if self.log_formatter is None:
             self.log_formatter = logging.Formatter("%(asctime)s - %(levelname)s - %(module)s - %(message)s")
 
         self.log_handler.setFormatter(self.log_formatter)
         self.logger.addHandler(self.log_handler)
 
         self.logger.debug(
-            f"Separator instantiating with input file: {audio_file_path}, model_name: {model_name}, output_dir: {output_dir}, use_cuda: {use_cuda}"
+            f"Separator instantiating with input file: {audio_file_path}, model_name: {model_name}, output_dir: {output_dir}, use_cuda: {use_cuda}, output_format: {output_format}"
         )
 
         self.model_name = model_name
         self.model_file_dir = model_file_dir
         self.output_dir = output_dir
         self.use_cuda = use_cuda
 
@@ -52,15 +54,23 @@
         self.audio_file_path = audio_file_path
         self.audio_file_base = os.path.splitext(os.path.basename(audio_file_path))[0]
 
         self.model_name = model_name
         self.model_url = f"https://github.com/TRvlvr/model_repo/releases/download/all_public_uvr_models/{self.model_name}.onnx"
         self.model_data_url = "https://raw.githubusercontent.com/TRvlvr/application_data/main/mdx_model_data/model_data.json"
 
-        self.wav_type_set = "PCM_16"
+        self.output_subtype = output_subtype
+        self.output_format = output_format
+
+        if self.output_format is None:
+            self.output_format = "WAV"
+
+        if self.output_subtype is None and output_format == "WAV":
+            self.output_subtype = "PCM_16"
+
         self.is_normalization = False
         self.is_denoise = False
 
         self.chunks = 0
         self.margin = 44100
         self.adjust = 1
         self.dim_c = 4
@@ -127,21 +137,21 @@
         self.logger.info("Running inference...")
         mdx_net_cut = True
         mix, raw_mix, samplerate = prepare_mix(self.audio_file_path, self.chunks, self.margin, mdx_net_cut=mdx_net_cut)
         self.logger.info("Demixing...")
         source = self.demix_base(mix)[0]
 
         self.logger.info(f"Saving {self.primary_stem} stem...")
-        primary_stem_path = os.path.join(f"{self.audio_file_base}_({self.primary_stem})_{self.model_name}.wav")
+        primary_stem_path = os.path.join(f"{self.audio_file_base}_({self.primary_stem})_{self.model_name}.{self.output_format.lower()}")
         if not isinstance(self.primary_source, np.ndarray):
             self.primary_source = spec_utils.normalize(self.logger, source, self.is_normalization).T
         self.write_audio(primary_stem_path, self.primary_source, samplerate)
 
         self.logger.info(f"Saving {self.secondary_stem} stem...")
-        secondary_stem_path = os.path.join(f"{self.audio_file_base}_({self.secondary_stem})_{self.model_name}.wav")
+        secondary_stem_path = os.path.join(f"{self.audio_file_base}_({self.secondary_stem})_{self.model_name}.{self.output_format.lower()}")
         if not isinstance(self.secondary_source, np.ndarray):
             raw_mix = self.demix_base(raw_mix, is_match_mix=True)[0] if mdx_net_cut else raw_mix
             self.secondary_source, raw_mix = spec_utils.normalize_two_stem(
                 self.logger, source * self.compensate, raw_mix, self.is_normalization
             )
             self.secondary_source = -self.secondary_source.T + raw_mix.T
         self.write_audio(secondary_stem_path, self.secondary_source, samplerate)
@@ -152,15 +162,15 @@
     def write_audio(self, stem_path, stem_source, samplerate):
         # If output_dir is specified, create it and join it with stem_path
         if self.output_dir:
             # Create the output directory if it does not exist
             os.makedirs(self.output_dir, exist_ok=True)
             stem_path = os.path.join(self.output_dir, stem_path)
 
-        sf.write(stem_path, stem_source, samplerate, subtype=self.wav_type_set)
+        sf.write(stem_path, stem_source, samplerate, subtype=self.output_subtype, format=self.output_format)
 
     def initialize_model_settings(self):
         self.n_bins = self.n_fft // 2 + 1
         self.trim = self.n_fft // 2
         self.chunk_size = self.hop * (self.dim_t - 1)
         self.window = torch.hann_window(window_length=self.n_fft, periodic=False).to(self.device)
         self.freq_pad = torch.zeros([1, self.dim_c, self.n_bins - self.dim_f, self.dim_t]).to(self.device)
```

### Comparing `audio_separator-0.3.4/audio_separator/utils/cli.py` & `audio_separator-0.4.1/audio_separator/utils/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,34 +23,36 @@
     parser.add_argument("-v", "--version", action="version", version=f"%(prog)s {package_version}")
     parser.add_argument("--log_level", default="INFO", help="Optional: Logging level, e.g. info, debug, warning. Default: INFO")
 
     parser.add_argument("--model_name", default="UVR_MDXNET_KARA_2", help="Optional: model name to be used for separation.")
     parser.add_argument("--model_file_dir", default="/tmp/audio-separator-models/", help="Optional: model files directory.")
     parser.add_argument("--output_dir", default=None, help="Optional: directory to write output files. Default: current dir.")
     parser.add_argument("--use_cuda", action="store_true", help="Optional: use Nvidia GPU with CUDA for separation.")
+    parser.add_argument("--output_format", default="FLAC", help="Optional: output format for separated files, any common format. Default: FLAC")
 
     args = parser.parse_args()
 
     log_level = getattr(logging, args.log_level.upper())
     logger.setLevel(log_level)
 
     if not hasattr(args, "audio_file"):
         parser.print_help()
         exit(1)
 
     logger.info(f"Separator beginning with input file: {args.audio_file}")
 
     separator = Separator(
         args.audio_file,
+        log_formatter=log_formatter,
+        log_level=log_level,
         model_name=args.model_name,
         model_file_dir=args.model_file_dir,
         output_dir=args.output_dir,
         use_cuda=args.use_cuda,
-        log_formatter=log_formatter,
-        log_level=log_level,
+        output_format=args.output_format,
     )
     primary_stem_path, secondary_stem_path = separator.separate()
 
     logger.info(f"Separation complete! Output files: {primary_stem_path} {secondary_stem_path}")
 
 
 if __name__ == "__main__":
```

### Comparing `audio_separator-0.3.4/audio_separator/utils/spec_utils.py` & `audio_separator-0.4.1/audio_separator/utils/spec_utils.py`

 * *Files identical despite different names*

### Comparing `audio_separator-0.3.4/pyproject.toml` & `audio_separator-0.4.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 [tool.poetry]
 name = "audio-separator"
-version = "0.3.4"
+version = "0.4.1"
 description = "Easy to use vocal separation on CLI or as a python package, using the amazing MDX-Net models from UVR trained by @Anjok07"
 authors = ["Andrew Beveridge <andrew@beveridge.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "audio_separator"}]
+homepage = "https://github.com/karaokenerds/python-audio-separator"
+repository = "https://github.com/karaokenerds/python-audio-separator"
+documentation = "https://github.com/karaokenerds/python-audio-separator/blob/main/README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
 onnx = "^1.14.0"
 onnxruntime = "^1.13"
 numpy = "^1.23"
 soundfile = "^0.11"
```

### Comparing `audio_separator-0.3.4/PKG-INFO` & `audio_separator-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: audio-separator
-Version: 0.3.4
+Version: 0.4.1
 Summary: Easy to use vocal separation on CLI or as a python package, using the amazing MDX-Net models from UVR trained by @Anjok07
+Home-page: https://github.com/karaokenerds/python-audio-separator
 License: MIT
 Author: Andrew Beveridge
 Author-email: andrew@beveridge.uk
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -14,14 +15,16 @@
 Requires-Dist: numpy (>=1.23,<2.0)
 Requires-Dist: onnx (>=1.14.0,<2.0.0)
 Requires-Dist: onnxruntime (>=1.13,<2.0)
 Requires-Dist: six (>=1.16,<2.0)
 Requires-Dist: soundfile (>=0.11,<0.12)
 Requires-Dist: torch (>=1.13,<2.0)
 Requires-Dist: wget (>=3,<4)
+Project-URL: Documentation, https://github.com/karaokenerds/python-audio-separator/blob/main/README.md
+Project-URL: Repository, https://github.com/karaokenerds/python-audio-separator
 Description-Content-Type: text/markdown
 
 # Audio Separator 🎶
 
 [![PyPI version](https://badge.fury.io/py/audio-separator.svg)](https://badge.fury.io/py/audio-separator)
 
 Summary: Easy to use vocal separation on CLI or as a python package, using the amazing MDX-Net models from UVR trained by @Anjok07
@@ -51,20 +54,21 @@
 
 You can use Audio Separator via the command line:
 
 ```sh
 audio-separator [audio_file] --model_name [model_name]
     
     audio_file: The path to the audio file to be separated. Supports all common formats (WAV, MP3, FLAC, M4A, etc.)
+    log_level: (Optional) Logging level, e.g. info, debug, warning. Default: INFO
+    log_formatter: (Optional) The log format. Default: '%(asctime)s - %(name)s - %(levelname)s - %(message)s'
     model_name: (Optional) The name of the model to use for separation. Default: UVR_MDXNET_KARA_2
     model_file_dir: (Optional) Directory to cache model files in. Default: /tmp/audio-separator-models/
     output_dir: (Optional) The directory where the separated files will be saved. If not specified, outputs to current dir.
     use_cuda: (Optional) Flag to use Nvidia GPU via CUDA for separation if available. Default: False
-    log_level: (Optional) Logging level, e.g. info, debug, warning. Default: INFO
-    log_formatter: (Optional) The log format. Default: '%(asctime)s - %(name)s - %(levelname)s - %(message)s'
+    output_format: (Optional) Format to encode output files, any common format (WAV, MP3, FLAC, M4A, etc.). Default: WAV
 ```
 
 Example:
 
 ```
 audio-separator /path/to/your/audio.wav --model_name UVR_MDXNET_KARA_2
 ```
@@ -87,20 +91,21 @@
 print(f'Primary stem saved at {primary_stem_path}')
 print(f'Secondary stem saved at {secondary_stem_path}')
 ```
 
 ## Parameters for the Separator class
 
 - audio_file: The path to the audio file to be separated. Supports all common formats (WAV, MP3, FLAC, M4A, etc.)
+- log_level: (Optional) Logging level, e.g. info, debug, warning. Default: INFO
+- log_formatter: (Optional) The log format. Default: '%(asctime)s - %(name)s - %(levelname)s - %(message)s'
 - model_name: (Optional) The name of the model to use for separation. Defaults to 'UVR_MDXNET_KARA_2', a very powerful model for Karaoke instrumental tracks.
 - model_file_dir: (Optional) Directory to cache model files in. Default: /tmp/audio-separator-models/
 - output_dir: (Optional) Directory where the separated files will be saved. If not specified, outputs to current dir.
 - use_cuda: (Optional) Flag to use Nvidia GPU via CUDA for separation if available. Default: False
-- log_level: (Optional) Logging level, e.g. info, debug, warning. Default: INFO
-- log_formatter: (Optional) The log format. Default: '%(asctime)s - %(name)s - %(levelname)s - %(message)s'
+- output_format: (Optional) Format to encode output files, any common format (WAV, MP3, FLAC, M4A, etc.). Default: WAV
 
 ## Requirements 📋
 
 Python <= 3.10 (one of the dependencies doesn't like 3.11 yet)
 
 Libraries: onnx, onnxruntime, numpy, soundfile, librosa, torch, wget, six
```

