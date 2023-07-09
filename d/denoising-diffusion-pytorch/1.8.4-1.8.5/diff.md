# Comparing `tmp/denoising-diffusion-pytorch-1.8.4.tar.gz` & `tmp/denoising-diffusion-pytorch-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denoising-diffusion-pytorch-1.8.4.tar", last modified: Wed Jul  5 18:31:54 2023, max compression
+gzip compressed data, was "denoising-diffusion-pytorch-1.8.5.tar", last modified: Sun Jul  9 15:20:09 2023, max compression
```

## Comparing `denoising-diffusion-pytorch-1.8.4.tar` & `denoising-diffusion-pytorch-1.8.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:31:54.017032 denoising-diffusion-pytorch-1.8.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-05 18:31:42.000000 denoising-diffusion-pytorch-1.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-05 18:31:54.017032 denoising-diffusion-pytorch-1.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-07-05 18:31:42.000000 denoising-diffusion-pytorch-1.8.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:31:54.017032 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-05 18:31:42.000000 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-05 18:31:42.000000 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    27823 2023-07-05 18:31:42.000000 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/classifier_free_guidance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-07-05 18:31:42.000000 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    36837 2023-07-05 18:31:42.000000 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    29929 2023-07-05 18:31:42.000000 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-07-05 18:31:42.000000 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/elucidated_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-07-05 18:31:42.000000 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/fid_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    35629 2023-07-05 18:31:42.000000 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/guided_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-07-05 18:31:42.000000 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    21236 2023-07-05 18:31:42.000000 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/simple_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-07-05 18:31:42.000000 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-05 18:31:42.000000 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-05 18:31:42.000000 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:31:54.017032 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-05 18:31:53.000000 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-05 18:31:53.000000 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 18:31:53.000000 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-05 18:31:53.000000 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 18:31:53.000000 denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 18:31:54.017032 denoising-diffusion-pytorch-1.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-05 18:31:42.000000 denoising-diffusion-pytorch-1.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:20:09.984936 denoising-diffusion-pytorch-1.8.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-09 15:20:01.000000 denoising-diffusion-pytorch-1.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-09 15:20:09.984936 denoising-diffusion-pytorch-1.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-07-09 15:20:01.000000 denoising-diffusion-pytorch-1.8.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:20:09.984936 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-09 15:20:01.000000 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-09 15:20:01.000000 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27823 2023-07-09 15:20:01.000000 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/classifier_free_guidance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-07-09 15:20:01.000000 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36837 2023-07-09 15:20:01.000000 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29929 2023-07-09 15:20:01.000000 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-07-09 15:20:01.000000 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/elucidated_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-09 15:20:01.000000 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/fid_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35629 2023-07-09 15:20:01.000000 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/guided_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-07-09 15:20:01.000000 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21236 2023-07-09 15:20:01.000000 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/simple_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-07-09 15:20:01.000000 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-09 15:20:01.000000 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-09 15:20:01.000000 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:20:09.984936 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-09 15:20:09.000000 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-09 15:20:09.000000 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 15:20:09.000000 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-09 15:20:09.000000 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-09 15:20:09.000000 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 15:20:09.984936 denoising-diffusion-pytorch-1.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-09 15:20:01.000000 denoising-diffusion-pytorch-1.8.5/setup.py
```

### Comparing `denoising-diffusion-pytorch-1.8.4/LICENSE` & `denoising-diffusion-pytorch-1.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.4/PKG-INFO` & `denoising-diffusion-pytorch-1.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.8.4
+Version: 1.8.5
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.8.4/README.md` & `denoising-diffusion-pytorch-1.8.5/README.md`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/__init__.py` & `denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/attend.py` & `denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/classifier_free_guidance.py` & `denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/classifier_free_guidance.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py` & `denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py` & `denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/elucidated_diffusion.py` & `denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/elucidated_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/fid_evaluation.py` & `denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/fid_evaluation.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,15 +44,18 @@
         block_idx = InceptionV3.BLOCK_INDEX_BY_DIM[inception_block_idx]
         self.inception_v3 = InceptionV3([block_idx]).to(device)
         self.dataset_stats_loaded = False
 
     def calculate_inception_features(self, samples):
         if self.channels == 1:
             samples = repeat(samples, "b 1 ... -> b c ...", c=3)
+
+        self.inception_v3.eval()
         features = self.inception_v3(samples)[0]
+
         if features.size(2) != 1 or features.size(3) != 1:
             features = adaptive_avg_pool2d(features, output_size=(1, 1))
         features = rearrange(features, "... 1 1 -> ...")
         return features
 
     def load_or_precalc_dataset_stats(self):
         path = os.path.join(self.stats_dir, "dataset_stats")
```

### Comparing `denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/guided_diffusion.py` & `denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/guided_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/learned_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/learned_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/simple_diffusion.py` & `denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/simple_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch.egg-info/PKG-INFO` & `denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.8.4
+Version: 1.8.5
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.8.4/denoising_diffusion_pytorch.egg-info/SOURCES.txt` & `denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.4/setup.py` & `denoising-diffusion-pytorch-1.8.5/setup.py`

 * *Files identical despite different names*

