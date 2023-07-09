# Comparing `tmp/torchnmf-0.3.4.tar.gz` & `tmp/torchnmf-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchnmf-0.3.4.tar", last modified: Sun Mar 28 07:50:53 2021, max compression
+gzip compressed data, was "torchnmf-0.3.5.tar", last modified: Sun Jul  9 01:48:59 2023, max compression
```

## Comparing `torchnmf-0.3.4.tar` & `torchnmf-0.3.5.tar`

### file list

```diff
@@ -1,26 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 07:50:53.083520 torchnmf-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (121)     5257 2021-03-28 07:50:53.083520 torchnmf-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3884 2021-03-28 07:49:46.000000 torchnmf-0.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-03-28 07:50:53.083520 torchnmf-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      764 2021-03-28 07:49:46.000000 torchnmf-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 07:50:53.083520 torchnmf-0.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-28 07:49:46.000000 torchnmf-0.3.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      750 2021-03-28 07:49:46.000000 torchnmf-0.3.4/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     3864 2021-03-28 07:49:46.000000 torchnmf-0.3.4/tests/test_nmf.py
--rw-r--r--   0 runner    (1001) docker     (121)     4630 2021-03-28 07:49:46.000000 torchnmf-0.3.4/tests/test_nmf_sparse.py
--rw-r--r--   0 runner    (1001) docker     (121)     5722 2021-03-28 07:49:46.000000 torchnmf-0.3.4/tests/test_plca.py
--rw-r--r--   0 runner    (1001) docker     (121)     1832 2021-03-28 07:49:46.000000 torchnmf-0.3.4/tests/test_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 07:50:53.083520 torchnmf-0.3.4/torchnmf/
--rw-r--r--   0 runner    (1001) docker     (121)      166 2021-03-28 07:49:46.000000 torchnmf-0.3.4/torchnmf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       51 2021-03-28 07:49:46.000000 torchnmf-0.3.4/torchnmf/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     3713 2021-03-28 07:49:46.000000 torchnmf-0.3.4/torchnmf/metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)    34937 2021-03-28 07:49:46.000000 torchnmf-0.3.4/torchnmf/nmf.py
--rw-r--r--   0 runner    (1001) docker     (121)    23373 2021-03-28 07:49:46.000000 torchnmf-0.3.4/torchnmf/plca.py
--rw-r--r--   0 runner    (1001) docker     (121)     6895 2021-03-28 07:49:46.000000 torchnmf-0.3.4/torchnmf/trainer.py
--rw-r--r--   0 runner    (1001) docker     (121)      321 2021-03-28 07:49:46.000000 torchnmf-0.3.4/torchnmf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 07:50:53.083520 torchnmf-0.3.4/torchnmf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5257 2021-03-28 07:50:51.000000 torchnmf-0.3.4/torchnmf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      435 2021-03-28 07:50:52.000000 torchnmf-0.3.4/torchnmf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-28 07:50:51.000000 torchnmf-0.3.4/torchnmf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-28 07:50:51.000000 torchnmf-0.3.4/torchnmf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-03-28 07:50:51.000000 torchnmf-0.3.4/torchnmf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:48:59.989510 torchnmf-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-09 01:47:02.000000 torchnmf-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-07-09 01:48:59.989510 torchnmf-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-07-09 01:47:02.000000 torchnmf-0.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 01:48:59.989510 torchnmf-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-09 01:47:02.000000 torchnmf-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:48:59.989510 torchnmf-0.3.5/torchnmf/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-09 01:47:02.000000 torchnmf-0.3.5/torchnmf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-09 01:47:02.000000 torchnmf-0.3.5/torchnmf/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-07-09 01:47:02.000000 torchnmf-0.3.5/torchnmf/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35063 2023-07-09 01:47:02.000000 torchnmf-0.3.5/torchnmf/nmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23572 2023-07-09 01:47:02.000000 torchnmf-0.3.5/torchnmf/plca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-07-09 01:47:02.000000 torchnmf-0.3.5/torchnmf/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-09 01:47:02.000000 torchnmf-0.3.5/torchnmf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:48:59.989510 torchnmf-0.3.5/torchnmf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-07-09 01:48:59.000000 torchnmf-0.3.5/torchnmf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-09 01:48:59.000000 torchnmf-0.3.5/torchnmf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 01:48:59.000000 torchnmf-0.3.5/torchnmf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-09 01:48:59.000000 torchnmf-0.3.5/torchnmf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-09 01:48:59.000000 torchnmf-0.3.5/torchnmf.egg-info/top_level.txt
```

### Comparing `torchnmf-0.3.4/PKG-INFO` & `torchnmf-0.3.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,127 +1,127 @@
 Metadata-Version: 2.1
 Name: torchnmf
-Version: 0.3.4
+Version: 0.3.5
 Summary: A pytorch package for Non-negative Matrix Factorization
-Home-page: https://github.com/yoyololicon/pytorch-NMFs
+Home-page: https://github.com/yoyololicon/pytorch-NMF
 Author: Chin-Yun Yu
 Author-email: lolimaster.cs03@nctu.edu.tw
-License: UNKNOWN
-Description: # Non-negative Matrix Fatorization in PyTorch
-        
-        [![build](https://github.com/yoyololicon/pytorch-NMF/actions/workflows/python-package.yml/badge.svg)](https://github.com/yoyololicon/pytorch-NMF/actions/workflows/python-package.yml)
-        [![codecov](https://codecov.io/gh/yoyololicon/pytorch-NMF/branch/master/graph/badge.svg?token=9UXAZ6PG2N)](https://codecov.io/gh/yoyololicon/pytorch-NMF)
-        [![Documentation Status](https://readthedocs.org/projects/pytorch-nmf/badge/?version=latest)](https://pytorch-nmf.readthedocs.io/en/latest/?badge=latest)
-        [![PyPI version](https://badge.fury.io/py/torchnmf.svg)](https://badge.fury.io/py/torchnmf)
-        
-        PyTorch is not only a good deep learning framework, but also a fast tool when it comes to matrix operations and convolutions on large data.
-        A great example is [PyTorchWavelets](http://github.com/tomrunia/PyTorchWavelets).
-        
-        
-        In this package I implement NMF, PLCA and their deconvolutional variations in PyTorch based on `torch.nn.Module`, 
-        so the models can be moved freely among CPU/GPU devices and utilize parallel computation of cuda.
-        We also utilize the computational graph from `torch.autograd` to derive updated coefficients so the amount of codes is reduced and easy to maintain.
-        
-        # Modules
-        
-        ## NMF
-        
-        Basic NMF and NMFD module minimizing beta-divergence using multiplicative update rules.
-        
-        
-        The interface is similar to `sklearn.decomposition.NMF` with some extra options.
-        
-        * `NMF`: Original NMF algorithm.
-        * `NMFD`: 1-D deconvolutional NMF algorithm.
-        * `NMF2D`: 2-D deconvolutional NMF algorithm. 
-        * `NMF3D`: 3-D deconvolutional NMF algorithm. 
-        
-        ## PLCA
-        
-        Basic PLCA and SIPLCA module using EM algorithm to minimize
-        KL-divergence between the target distribution and the estimated
-        distribution.
-        
-        * `PLCA`: Original PLCA (Probabilistic Latent Component Analysis)
-          algorithm.
-        * `SIPLCA`: Shift-Invariant PLCA algorithm (similar to NMFD).
-        * `SIPLCA2`: 2-D deconvolutional SIPLCA algorithm.
-        * `SIPLCA3`: 3-D deconvolutional SIPLCA algorithm.
-        
-        
-        
-        ## Usage
-        
-        Here is a short example of decompose a spectrogram using deconvolutional NMF:
-        
-        ```python
-        import torch
-        import librosa
-        from torchnmf.nmf import NMFD
-        from torchnmf.metrics import kl_div
-        
-        y, sr = librosa.load(librosa.util.example_audio_file())
-        y = torch.from_numpy(y)
-        windowsize = 2048
-        S = torch.stft(y, windowsize, 
-                       window=torch.hann_window(windowsize),
-                       return_complex=True).abs().cuda()
-        S = S.unsqueeze(0)
-        
-        R = 8   # number of components
-        T = 400 # size of convolution window
-        
-        net = NMFD(S.shape, rank=R, T=T).cuda()
-        # run extremely fast on gpu
-        net.fit(S)      # fit to target matrix S
-        V = net()
-        print(kl_div(V, S))        # KL divergence to S
-        ```
-        A more detailed version can be found [here](examples/librosa_example.py). 
-        See our [documentation](https://pytorch-nmf.readthedocs.io/en/latest/) to find out more usage of this package.
-        
-        ![](examples/librosa_example.png)
-        
-        ## Compare to sklearn
-        
-        The barchart shows the time cost per iteration with different
-        beta-divergence. It shows that pytorch-based NMF has a much more constant process time across 
-        different beta values, which can take advantage when beta is not 0, 1, or 2.
-        This is because our implementation use the same computational graph regardless which beta-divergence are we minimizing.
-        It runs even faster when computation is done on GPU. The test is conducted on a
-        Acer E5 laptop with i5-7200U CPU and GTX 950M GPU.
-        
-        ![](examples/performance.png) 
-        
-        ## Installation
-        
-        ```
-        pip install torchnmf
-        ```
-        
-        ## Requirements
-        
-        * PyTorch
-        * tqdm
-        
-        ## Tips
-        
-        * If you notice significant slow down when operating on CPU, please flush denormal numbers by `
-        torch.set_flush_denormal(True)`.
-        
-        
-        ## TODO
-        
-        - [x] Support sparse matrix target (only on `NMF` module).
-        - [x] Regularization.
-        - [ ] NNDSVD initialization.
-        - [x] 2/3-D deconvolutional module.
-        - [x] PLCA.
-        - [x] Documentation.
-        - [ ] ipynb examples.
-        - [x] Refactor PLCA module.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Non-negative Matrix Fatorization in PyTorch
+
+[![build](https://github.com/yoyololicon/pytorch-NMF/actions/workflows/python-package.yml/badge.svg)](https://github.com/yoyololicon/pytorch-NMF/actions/workflows/python-package.yml)
+[![Upload Python Package](https://github.com/yoyololicon/pytorch-NMF/actions/workflows/python-publish.yml/badge.svg)](https://github.com/yoyololicon/pytorch-NMF/actions/workflows/python-publish.yml)
+[![codecov](https://codecov.io/gh/yoyololicon/pytorch-NMF/branch/master/graph/badge.svg?token=9UXAZ6PG2N)](https://codecov.io/gh/yoyololicon/pytorch-NMF)
+[![Documentation Status](https://readthedocs.org/projects/pytorch-nmf/badge/?version=latest)](https://pytorch-nmf.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/torchnmf.svg)](https://badge.fury.io/py/torchnmf)
+
+PyTorch is not only a good deep learning framework, but also a fast tool when it comes to matrix operations and convolutions on large data.
+A great example is [PyTorchWavelets](http://github.com/tomrunia/PyTorchWavelets).
+
+
+In this package I implement NMF, PLCA and their deconvolutional variations in PyTorch based on `torch.nn.Module`, 
+so the models can be moved freely among CPU/GPU devices and utilize parallel computation of cuda.
+We also utilize the computational graph from `torch.autograd` to derive updated coefficients so the amount of codes is reduced and easy to maintain.
+
+# Modules
+
+## NMF
+
+Basic NMF and NMFD module minimizing beta-divergence using multiplicative update rules.
+
+
+The interface is similar to `sklearn.decomposition.NMF` with some extra options.
+
+* `NMF`: Original NMF algorithm.
+* `NMFD`: 1-D deconvolutional NMF algorithm.
+* `NMF2D`: 2-D deconvolutional NMF algorithm. 
+* `NMF3D`: 3-D deconvolutional NMF algorithm. 
+
+## PLCA
+
+Basic PLCA and SIPLCA module using EM algorithm to minimize
+KL-divergence between the target distribution and the estimated
+distribution.
+
+* `PLCA`: Original PLCA (Probabilistic Latent Component Analysis)
+  algorithm.
+* `SIPLCA`: Shift-Invariant PLCA algorithm (similar to NMFD).
+* `SIPLCA2`: 2-D deconvolutional SIPLCA algorithm.
+* `SIPLCA3`: 3-D deconvolutional SIPLCA algorithm.
+
+
+
+## Usage
+
+Here is a short example of decompose a spectrogram using deconvolutional NMF:
+
+```python
+import torch
+import librosa
+from torchnmf.nmf import NMFD
+from torchnmf.metrics import kl_div
+
+y, sr = librosa.load(librosa.util.example_audio_file())
+y = torch.from_numpy(y)
+windowsize = 2048
+S = torch.stft(y, windowsize, 
+               window=torch.hann_window(windowsize),
+               return_complex=True).abs().cuda()
+S = S.unsqueeze(0)
+
+R = 8   # number of components
+T = 400 # size of convolution window
+
+net = NMFD(S.shape, rank=R, T=T).cuda()
+# run extremely fast on gpu
+net.fit(S)      # fit to target matrix S
+V = net()
+print(kl_div(V, S))        # KL divergence to S
+```
+A more detailed version can be found [here](examples/librosa_example.py). 
+See our [documentation](https://pytorch-nmf.readthedocs.io/en/latest/) to find out more usage of this package.
+
+![](examples/librosa_example.png)
+
+## Compare to sklearn
+
+The barchart shows the time cost per iteration with different
+beta-divergence. It shows that pytorch-based NMF has a much more constant process time across 
+different beta values, which can take advantage when beta is not 0, 1, or 2.
+This is because our implementation use the same computational graph regardless which beta-divergence are we minimizing.
+It runs even faster when computation is done on GPU. The test is conducted on a
+Acer E5 laptop with i5-7200U CPU and GTX 950M GPU.
+
+![](examples/performance.png) 
+
+## Installation
+
+```
+pip install torchnmf
+```
+
+## Requirements
+
+* PyTorch
+* tqdm
+
+## Tips
+
+* If you notice significant slow down when operating on CPU, please flush denormal numbers by `
+torch.set_flush_denormal(True)`.
+
+
+## TODO
+
+- [x] Support sparse matrix target (only on `NMF` module).
+- [x] Regularization.
+- [ ] NNDSVD initialization.
+- [x] 2/3-D deconvolutional module.
+- [x] PLCA.
+- [x] Documentation.
+- [ ] ipynb examples.
+- [x] Refactor PLCA module.
```

### Comparing `torchnmf-0.3.4/README.md` & `torchnmf-0.3.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Non-negative Matrix Fatorization in PyTorch
 
 [![build](https://github.com/yoyololicon/pytorch-NMF/actions/workflows/python-package.yml/badge.svg)](https://github.com/yoyololicon/pytorch-NMF/actions/workflows/python-package.yml)
+[![Upload Python Package](https://github.com/yoyololicon/pytorch-NMF/actions/workflows/python-publish.yml/badge.svg)](https://github.com/yoyololicon/pytorch-NMF/actions/workflows/python-publish.yml)
 [![codecov](https://codecov.io/gh/yoyololicon/pytorch-NMF/branch/master/graph/badge.svg?token=9UXAZ6PG2N)](https://codecov.io/gh/yoyololicon/pytorch-NMF)
 [![Documentation Status](https://readthedocs.org/projects/pytorch-nmf/badge/?version=latest)](https://pytorch-nmf.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/torchnmf.svg)](https://badge.fury.io/py/torchnmf)
 
 PyTorch is not only a good deep learning framework, but also a fast tool when it comes to matrix operations and convolutions on large data.
 A great example is [PyTorchWavelets](http://github.com/tomrunia/PyTorchWavelets).
```

### Comparing `torchnmf-0.3.4/setup.py` & `torchnmf-0.3.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,17 +8,16 @@
     name=name,
     version=__version__,
     author=__maintainer__,
     author_email=__email__,
     description="A pytorch package for Non-negative Matrix Factorization",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/yoyololicon/pytorch-NMFs",
-    packages=setuptools.find_packages(),
-    install_requires=['torch>=1.4',
-                      'tqdm'],
+    url="https://github.com/yoyololicon/pytorch-NMF",
+    packages=["torchnmf"],
+    install_requires=["torch>=1.4", "tqdm"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-)
+)
```

### Comparing `torchnmf-0.3.4/torchnmf/metrics.py` & `torchnmf-0.3.5/torchnmf/metrics.py`

 * *Files identical despite different names*

### Comparing `torchnmf-0.3.4/torchnmf/nmf.py` & `torchnmf-0.3.5/torchnmf/nmf.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,14 +239,17 @@
         if infer_rank is None:
             assert rank, "A rank should be given when W and H are not available!"
         else:
             if getattr(self, "H") is not None:
                 assert self.H.shape[1] == infer_rank, "Latent size of H does not match with others!"
             if getattr(self, "W") is not None:
                 assert self.W.shape[1] == infer_rank, "Latent size of W does not match with others!"
+                self.out_channels = self.W.shape[0]
+                if self.W.ndim > 2:
+                    self.kernel_size = self.W.shape[2:]
             rank = infer_rank
 
         self.rank = rank
 
     def extra_repr(self) -> str:
         s = ('{rank}')
         if self.W is not None:
@@ -596,15 +599,14 @@
         return n_iter + 1
 
 
 @torch.jit.script
 def _nmf_sparse_reconstruct(H: Tensor, W: Tensor, indices: Tensor):
     ii, jj = indices[0], indices[1]
     n_vals = indices.shape[1]
-    dot_vals = []
     rank = W.shape[1]
     batch_size = max(rank, n_vals // rank)
 
     dot_vals = torch.empty(n_vals, dtype=H.dtype, device=H.device)
     for start in range(0, n_vals, batch_size):
         batch = slice(start, start + batch_size)
         dot_vals[batch] = (W[jj[batch], :] * H[ii[batch], :]).sum(1)
```

### Comparing `torchnmf-0.3.4/torchnmf/plca.py` & `torchnmf-0.3.5/torchnmf/plca.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,14 +131,17 @@
         else:
             if getattr(self, "Z") is not None:
                 assert self.Z.shape[0] == infer_rank, "Latent size of Z does not match with others!"
             if getattr(self, "H") is not None:
                 assert self.H.shape[1] == infer_rank, "Latent size of H does not match with others!"
             if getattr(self, "W") is not None:
                 assert self.W.shape[1] == infer_rank, "Latent size of W does not match with others!"
+                self.out_channels = self.W.shape[0]
+                if self.W.ndim > 2:
+                    self.kernel_size = self.W.shape[2:]
             rank = infer_rank
 
         self.rank = rank
 
     def extra_repr(self) -> str:
         s = ('{rank}')
         if self.W is not None:
@@ -236,15 +239,16 @@
         Z = self.Z
 
         norm = V.sum()
         V = V.contiguous() / norm
 
         with torch.no_grad():
             WZH = self.reconstruct(H, W, Z)
-            loss_init = previous_loss = kl_div(WZH * norm, V * norm).mul(2).sqrt().item()
+            loss_init = previous_loss = kl_div(
+                WZH * norm, V * norm).mul(2).sqrt().item()
 
         with tqdm(total=max_iter, disable=not verbose) as pbar:
             for n_iter in range(max_iter):
                 self.zero_grad()
                 WZH = self.reconstruct(H, W, Z)
                 WZH.backward(V / WZH.add(eps))
 
@@ -283,15 +287,16 @@
                         H.data.add_(H_alpha - 1)
                         F.threshold(H.data, eps, eps, True)
                         H.data.div_(get_norm(H))
 
                 if n_iter % 10 == 9:
                     with torch.no_grad():
                         WZH = self.reconstruct(H, W, Z)
-                        loss = kl_div(WZH * norm, V * norm).mul(2).sqrt().item()
+                        loss = kl_div(WZH * norm, V *
+                                      norm).mul(2).sqrt().item()
                         log_pro = _log_probability(
                             V, WZH, W, Z, H, W_alpha, Z_alpha, H_alpha).item()
                     pbar.set_postfix(loss=loss, log_likelihood=log_pro)
                     pbar.update(10)
                     if (previous_loss - loss) / loss_init < tol:
                         break
                     previous_loss = loss
```

### Comparing `torchnmf-0.3.4/torchnmf/trainer.py` & `torchnmf-0.3.5/torchnmf/trainer.py`

 * *Files identical despite different names*

### Comparing `torchnmf-0.3.4/torchnmf.egg-info/PKG-INFO` & `torchnmf-0.3.5/torchnmf.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,127 +1,127 @@
 Metadata-Version: 2.1
 Name: torchnmf
-Version: 0.3.4
+Version: 0.3.5
 Summary: A pytorch package for Non-negative Matrix Factorization
-Home-page: https://github.com/yoyololicon/pytorch-NMFs
+Home-page: https://github.com/yoyololicon/pytorch-NMF
 Author: Chin-Yun Yu
 Author-email: lolimaster.cs03@nctu.edu.tw
-License: UNKNOWN
-Description: # Non-negative Matrix Fatorization in PyTorch
-        
-        [![build](https://github.com/yoyololicon/pytorch-NMF/actions/workflows/python-package.yml/badge.svg)](https://github.com/yoyololicon/pytorch-NMF/actions/workflows/python-package.yml)
-        [![codecov](https://codecov.io/gh/yoyololicon/pytorch-NMF/branch/master/graph/badge.svg?token=9UXAZ6PG2N)](https://codecov.io/gh/yoyololicon/pytorch-NMF)
-        [![Documentation Status](https://readthedocs.org/projects/pytorch-nmf/badge/?version=latest)](https://pytorch-nmf.readthedocs.io/en/latest/?badge=latest)
-        [![PyPI version](https://badge.fury.io/py/torchnmf.svg)](https://badge.fury.io/py/torchnmf)
-        
-        PyTorch is not only a good deep learning framework, but also a fast tool when it comes to matrix operations and convolutions on large data.
-        A great example is [PyTorchWavelets](http://github.com/tomrunia/PyTorchWavelets).
-        
-        
-        In this package I implement NMF, PLCA and their deconvolutional variations in PyTorch based on `torch.nn.Module`, 
-        so the models can be moved freely among CPU/GPU devices and utilize parallel computation of cuda.
-        We also utilize the computational graph from `torch.autograd` to derive updated coefficients so the amount of codes is reduced and easy to maintain.
-        
-        # Modules
-        
-        ## NMF
-        
-        Basic NMF and NMFD module minimizing beta-divergence using multiplicative update rules.
-        
-        
-        The interface is similar to `sklearn.decomposition.NMF` with some extra options.
-        
-        * `NMF`: Original NMF algorithm.
-        * `NMFD`: 1-D deconvolutional NMF algorithm.
-        * `NMF2D`: 2-D deconvolutional NMF algorithm. 
-        * `NMF3D`: 3-D deconvolutional NMF algorithm. 
-        
-        ## PLCA
-        
-        Basic PLCA and SIPLCA module using EM algorithm to minimize
-        KL-divergence between the target distribution and the estimated
-        distribution.
-        
-        * `PLCA`: Original PLCA (Probabilistic Latent Component Analysis)
-          algorithm.
-        * `SIPLCA`: Shift-Invariant PLCA algorithm (similar to NMFD).
-        * `SIPLCA2`: 2-D deconvolutional SIPLCA algorithm.
-        * `SIPLCA3`: 3-D deconvolutional SIPLCA algorithm.
-        
-        
-        
-        ## Usage
-        
-        Here is a short example of decompose a spectrogram using deconvolutional NMF:
-        
-        ```python
-        import torch
-        import librosa
-        from torchnmf.nmf import NMFD
-        from torchnmf.metrics import kl_div
-        
-        y, sr = librosa.load(librosa.util.example_audio_file())
-        y = torch.from_numpy(y)
-        windowsize = 2048
-        S = torch.stft(y, windowsize, 
-                       window=torch.hann_window(windowsize),
-                       return_complex=True).abs().cuda()
-        S = S.unsqueeze(0)
-        
-        R = 8   # number of components
-        T = 400 # size of convolution window
-        
-        net = NMFD(S.shape, rank=R, T=T).cuda()
-        # run extremely fast on gpu
-        net.fit(S)      # fit to target matrix S
-        V = net()
-        print(kl_div(V, S))        # KL divergence to S
-        ```
-        A more detailed version can be found [here](examples/librosa_example.py). 
-        See our [documentation](https://pytorch-nmf.readthedocs.io/en/latest/) to find out more usage of this package.
-        
-        ![](examples/librosa_example.png)
-        
-        ## Compare to sklearn
-        
-        The barchart shows the time cost per iteration with different
-        beta-divergence. It shows that pytorch-based NMF has a much more constant process time across 
-        different beta values, which can take advantage when beta is not 0, 1, or 2.
-        This is because our implementation use the same computational graph regardless which beta-divergence are we minimizing.
-        It runs even faster when computation is done on GPU. The test is conducted on a
-        Acer E5 laptop with i5-7200U CPU and GTX 950M GPU.
-        
-        ![](examples/performance.png) 
-        
-        ## Installation
-        
-        ```
-        pip install torchnmf
-        ```
-        
-        ## Requirements
-        
-        * PyTorch
-        * tqdm
-        
-        ## Tips
-        
-        * If you notice significant slow down when operating on CPU, please flush denormal numbers by `
-        torch.set_flush_denormal(True)`.
-        
-        
-        ## TODO
-        
-        - [x] Support sparse matrix target (only on `NMF` module).
-        - [x] Regularization.
-        - [ ] NNDSVD initialization.
-        - [x] 2/3-D deconvolutional module.
-        - [x] PLCA.
-        - [x] Documentation.
-        - [ ] ipynb examples.
-        - [x] Refactor PLCA module.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Non-negative Matrix Fatorization in PyTorch
+
+[![build](https://github.com/yoyololicon/pytorch-NMF/actions/workflows/python-package.yml/badge.svg)](https://github.com/yoyololicon/pytorch-NMF/actions/workflows/python-package.yml)
+[![Upload Python Package](https://github.com/yoyololicon/pytorch-NMF/actions/workflows/python-publish.yml/badge.svg)](https://github.com/yoyololicon/pytorch-NMF/actions/workflows/python-publish.yml)
+[![codecov](https://codecov.io/gh/yoyololicon/pytorch-NMF/branch/master/graph/badge.svg?token=9UXAZ6PG2N)](https://codecov.io/gh/yoyololicon/pytorch-NMF)
+[![Documentation Status](https://readthedocs.org/projects/pytorch-nmf/badge/?version=latest)](https://pytorch-nmf.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/torchnmf.svg)](https://badge.fury.io/py/torchnmf)
+
+PyTorch is not only a good deep learning framework, but also a fast tool when it comes to matrix operations and convolutions on large data.
+A great example is [PyTorchWavelets](http://github.com/tomrunia/PyTorchWavelets).
+
+
+In this package I implement NMF, PLCA and their deconvolutional variations in PyTorch based on `torch.nn.Module`, 
+so the models can be moved freely among CPU/GPU devices and utilize parallel computation of cuda.
+We also utilize the computational graph from `torch.autograd` to derive updated coefficients so the amount of codes is reduced and easy to maintain.
+
+# Modules
+
+## NMF
+
+Basic NMF and NMFD module minimizing beta-divergence using multiplicative update rules.
+
+
+The interface is similar to `sklearn.decomposition.NMF` with some extra options.
+
+* `NMF`: Original NMF algorithm.
+* `NMFD`: 1-D deconvolutional NMF algorithm.
+* `NMF2D`: 2-D deconvolutional NMF algorithm. 
+* `NMF3D`: 3-D deconvolutional NMF algorithm. 
+
+## PLCA
+
+Basic PLCA and SIPLCA module using EM algorithm to minimize
+KL-divergence between the target distribution and the estimated
+distribution.
+
+* `PLCA`: Original PLCA (Probabilistic Latent Component Analysis)
+  algorithm.
+* `SIPLCA`: Shift-Invariant PLCA algorithm (similar to NMFD).
+* `SIPLCA2`: 2-D deconvolutional SIPLCA algorithm.
+* `SIPLCA3`: 3-D deconvolutional SIPLCA algorithm.
+
+
+
+## Usage
+
+Here is a short example of decompose a spectrogram using deconvolutional NMF:
+
+```python
+import torch
+import librosa
+from torchnmf.nmf import NMFD
+from torchnmf.metrics import kl_div
+
+y, sr = librosa.load(librosa.util.example_audio_file())
+y = torch.from_numpy(y)
+windowsize = 2048
+S = torch.stft(y, windowsize, 
+               window=torch.hann_window(windowsize),
+               return_complex=True).abs().cuda()
+S = S.unsqueeze(0)
+
+R = 8   # number of components
+T = 400 # size of convolution window
+
+net = NMFD(S.shape, rank=R, T=T).cuda()
+# run extremely fast on gpu
+net.fit(S)      # fit to target matrix S
+V = net()
+print(kl_div(V, S))        # KL divergence to S
+```
+A more detailed version can be found [here](examples/librosa_example.py). 
+See our [documentation](https://pytorch-nmf.readthedocs.io/en/latest/) to find out more usage of this package.
+
+![](examples/librosa_example.png)
+
+## Compare to sklearn
+
+The barchart shows the time cost per iteration with different
+beta-divergence. It shows that pytorch-based NMF has a much more constant process time across 
+different beta values, which can take advantage when beta is not 0, 1, or 2.
+This is because our implementation use the same computational graph regardless which beta-divergence are we minimizing.
+It runs even faster when computation is done on GPU. The test is conducted on a
+Acer E5 laptop with i5-7200U CPU and GTX 950M GPU.
+
+![](examples/performance.png) 
+
+## Installation
+
+```
+pip install torchnmf
+```
+
+## Requirements
+
+* PyTorch
+* tqdm
+
+## Tips
+
+* If you notice significant slow down when operating on CPU, please flush denormal numbers by `
+torch.set_flush_denormal(True)`.
+
+
+## TODO
+
+- [x] Support sparse matrix target (only on `NMF` module).
+- [x] Regularization.
+- [ ] NNDSVD initialization.
+- [x] 2/3-D deconvolutional module.
+- [x] PLCA.
+- [x] Documentation.
+- [ ] ipynb examples.
+- [x] Refactor PLCA module.
```

