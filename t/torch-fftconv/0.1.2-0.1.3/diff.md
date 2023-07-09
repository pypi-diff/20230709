# Comparing `tmp/torch_fftconv-0.1.2.tar.gz` & `tmp/torch_fftconv-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_fftconv-0.1.2.tar", last modified: Sat Dec 18 06:13:53 2021, max compression
+gzip compressed data, was "torch_fftconv-0.1.3.tar", last modified: Sun Jul  9 01:56:52 2023, max compression
```

## Comparing `torch_fftconv-0.1.2.tar` & `torch_fftconv-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 06:13:53.077825 torch_fftconv-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)     2405 2021-12-18 06:13:53.077825 torch_fftconv-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1872 2021-12-18 06:13:40.000000 torch_fftconv-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-18 06:13:53.077825 torch_fftconv-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      857 2021-12-18 06:13:40.000000 torch_fftconv-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 06:13:53.077825 torch_fftconv-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 06:13:40.000000 torch_fftconv-0.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8582 2021-12-18 06:13:40.000000 torch_fftconv-0.1.2/tests/test_values.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 06:13:53.077825 torch_fftconv-0.1.2/torch_fftconv/
--rw-r--r--   0 runner    (1001) docker     (121)       50 2021-12-18 06:13:40.000000 torch_fftconv-0.1.2/torch_fftconv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11808 2021-12-18 06:13:40.000000 torch_fftconv-0.1.2/torch_fftconv/functional.py
--rw-r--r--   0 runner    (1001) docker     (121)     4118 2021-12-18 06:13:40.000000 torch_fftconv-0.1.2/torch_fftconv/modules.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 06:13:53.077825 torch_fftconv-0.1.2/torch_fftconv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2405 2021-12-18 06:13:53.000000 torch_fftconv-0.1.2/torch_fftconv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      320 2021-12-18 06:13:53.000000 torch_fftconv-0.1.2/torch_fftconv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-18 06:13:53.000000 torch_fftconv-0.1.2/torch_fftconv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-12-18 06:13:53.000000 torch_fftconv-0.1.2/torch_fftconv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-12-18 06:13:53.000000 torch_fftconv-0.1.2/torch_fftconv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:56:52.252031 torch_fftconv-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-09 01:56:52.252031 torch_fftconv-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-09 01:56:37.000000 torch_fftconv-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 01:56:52.252031 torch_fftconv-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-09 01:56:37.000000 torch_fftconv-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:56:52.252031 torch_fftconv-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-07-09 01:56:37.000000 torch_fftconv-0.1.3/tests/test_values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:56:52.252031 torch_fftconv-0.1.3/torch_fftconv/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-09 01:56:37.000000 torch_fftconv-0.1.3/torch_fftconv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11808 2023-07-09 01:56:37.000000 torch_fftconv-0.1.3/torch_fftconv/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-07-09 01:56:37.000000 torch_fftconv-0.1.3/torch_fftconv/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-09 01:56:37.000000 torch_fftconv-0.1.3/torch_fftconv/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:56:52.252031 torch_fftconv-0.1.3/torch_fftconv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-09 01:56:52.000000 torch_fftconv-0.1.3/torch_fftconv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-09 01:56:52.000000 torch_fftconv-0.1.3/torch_fftconv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 01:56:52.000000 torch_fftconv-0.1.3/torch_fftconv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-09 01:56:52.000000 torch_fftconv-0.1.3/torch_fftconv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-09 01:56:52.000000 torch_fftconv-0.1.3/torch_fftconv.egg-info/top_level.txt
```

### Comparing `torch_fftconv-0.1.2/PKG-INFO` & `torch_fftconv-0.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: torch_fftconv
-Version: 0.1.2
+Version: 0.1.3
 Summary: Implementation of 1D, 2D, and 3D FFT convolutions in PyTorch. Much faster than direct convolutions for large kernel sizes
 Home-page: https://github.com/yoyololicon/fft-conv-pytorch
 Author: Chin-Yun Yu
 Author-email: lolimaster.cs03@nctu.edu.tw
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # FFT Conv PyTorch
 
 [![Python package](https://github.com/yoyololicon/fft-conv-pytorch/actions/workflows/python-package.yml/badge.svg?branch=master)](https://github.com/yoyololicon/fft-conv-pytorch/actions/workflows/python-package.yml)
+[![Upload Python Package](https://github.com/yoyololicon/fft-conv-pytorch/actions/workflows/python-publish.yml/badge.svg)](https://github.com/yoyololicon/fft-conv-pytorch/actions/workflows/python-publish.yml)
+[![PyPI version](https://badge.fury.io/py/torch-fftconv.svg)](https://badge.fury.io/py/torch-fftconv)
 
 This is a fork of original [fft-conv-pytorch](https://github.com/fkodom/fft-conv-pytorch).
 I made some modifications to support dilated and strided convolution, so it can be a drop-in-replacement of original PyTorch `Conv*d` modules and `conv*d` functions, with the same function parameters and behavior.
 
 ### Install
 
 ```commandline
@@ -60,8 +60,7 @@
 For details and benchmarks on other parameters, check [this notebook](benchmark.ipynb).
 
 ## TODO
 
 - [ ] Jittability.
 - [x] Dilated Convolution.
 - [x] Transposed Convolution.
-
```

### Comparing `torch_fftconv-0.1.2/README.md` & `torch_fftconv-0.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # FFT Conv PyTorch
 
 [![Python package](https://github.com/yoyololicon/fft-conv-pytorch/actions/workflows/python-package.yml/badge.svg?branch=master)](https://github.com/yoyololicon/fft-conv-pytorch/actions/workflows/python-package.yml)
+[![Upload Python Package](https://github.com/yoyololicon/fft-conv-pytorch/actions/workflows/python-publish.yml/badge.svg)](https://github.com/yoyololicon/fft-conv-pytorch/actions/workflows/python-publish.yml)
+[![PyPI version](https://badge.fury.io/py/torch-fftconv.svg)](https://badge.fury.io/py/torch-fftconv)
 
 This is a fork of original [fft-conv-pytorch](https://github.com/fkodom/fft-conv-pytorch).
 I made some modifications to support dilated and strided convolution, so it can be a drop-in-replacement of original PyTorch `Conv*d` modules and `conv*d` functions, with the same function parameters and behavior.
 
 ### Install
 
 ```commandline
```

### Comparing `torch_fftconv-0.1.2/setup.py` & `torch_fftconv-0.1.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from os import name
 import setuptools
 
 NAME = "torch_fftconv"
-VERSION = '0.1.2'
+VERSION = '0.1.3'
 MAINTAINER = 'Chin-Yun Yu'
 EMAIL = 'lolimaster.cs03@nctu.edu.tw'
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
@@ -15,15 +15,15 @@
     version=VERSION,
     author=MAINTAINER,
     author_email=EMAIL,
     description="Implementation of 1D, 2D, and 3D FFT convolutions in PyTorch. Much faster than direct convolutions for large kernel sizes",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yoyololicon/fft-conv-pytorch",
-    packages=setuptools.find_packages(),
+    packages=["torch_fftconv"],
     install_requires=['torch>=1.7.0'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `torch_fftconv-0.1.2/tests/test_values.py` & `torch_fftconv-0.1.3/tests/test_values.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,99 @@
 import torch
 from torch.nn import Conv1d, Conv2d, Conv3d, ConvTranspose1d, ConvTranspose2d, ConvTranspose3d
 from torch_fftconv.modules import *
+from torch_fftconv.utils import convert_fft_conv
 
 import pytest
+from itertools import product
 
 device = 'cuda' if torch.cuda.is_available() else 'cpu'
 if torch.cuda.is_available():
     torch.backends.cuda.matmul.allow_tf32 = False
     torch.backends.cudnn.allow_tf32 = False
 
 
+@pytest.mark.parametrize('batch', [8])
+@pytest.mark.parametrize('in_channels', [32])
+@pytest.mark.parametrize('out_channels', [32])
+@pytest.mark.parametrize('length', [60])
+@pytest.mark.parametrize('kernel_size', [9, 11])
+@pytest.mark.parametrize('stride', [1, 2, 3, 5])
+@pytest.mark.parametrize('dilation', [1, 2, 3, 5])
+@pytest.mark.parametrize('padding', [0, 4, 5, 10])
+@pytest.mark.parametrize('bias', [True, False])
+def test_conv1d_circular(batch, length,
+                         in_channels, out_channels,
+                         kernel_size, stride, padding, dilation, bias):
+
+    x = torch.randn(batch, in_channels, length,
+                    requires_grad=True, device=device)
+    conv = Conv1d(in_channels, out_channels, kernel_size, stride,
+                  padding, dilation, 1, bias, 'circular').to(device)
+    fft_conv = convert_fft_conv(conv)
+
+    y1 = conv(x)
+    y2 = fft_conv(x)
+    assert torch.allclose(
+        y1, y2, atol=1e-5, rtol=1e-5), torch.abs(y1 - y2).max().item()
+    y2.sum().backward()
+
+
+@pytest.mark.parametrize('batch', [8])
+@pytest.mark.parametrize('in_channels', [16])
+@pytest.mark.parametrize('out_channels', [16])
+@pytest.mark.parametrize('length', [(72, 96)])
+@pytest.mark.parametrize('kernel_size', [17, 23])
+@pytest.mark.parametrize('stride', [1, 2, 3])
+@pytest.mark.parametrize('dilation', [1, 2, 3])
+@pytest.mark.parametrize('padding', [0, 8, 11, 22])
+@pytest.mark.parametrize('bias', [True, False])
+def test_conv2d_circular(batch, length,
+                         in_channels, out_channels,
+                         kernel_size, stride, padding, dilation, bias):
+
+    x = torch.randn(batch, in_channels, *length,
+                    requires_grad=True, device=device)
+    conv = Conv2d(in_channels, out_channels, kernel_size, stride,
+                  padding, dilation, 1, bias, 'circular').to(device)
+    fft_conv = convert_fft_conv(conv)
+
+    y1 = conv(x)
+    y2 = fft_conv(x)
+    assert torch.allclose(
+        y1, y2, atol=1e-5, rtol=1e-5), torch.abs(y1 - y2).max().item()
+    y2.sum().backward()
+
+
+@pytest.mark.parametrize('batch', [8])
+@pytest.mark.parametrize('in_channels', [8])
+@pytest.mark.parametrize('out_channels', [8])
+@pytest.mark.parametrize('length', [(48, 48, 48)])
+@pytest.mark.parametrize('kernel_size', [11])
+@pytest.mark.parametrize('stride', [1, 2, 3])
+@pytest.mark.parametrize('dilation', [1, 3])
+@pytest.mark.parametrize('padding', [0, 6, 8, 16])
+@pytest.mark.parametrize('bias', [True, False])
+def test_conv3d_circular(batch, length,
+                         in_channels, out_channels,
+                         kernel_size, stride, padding, dilation, bias):
+
+    x = torch.randn(batch, in_channels, *length,
+                    requires_grad=True, device=device)
+    conv = Conv3d(in_channels, out_channels, kernel_size, stride,
+                  padding, dilation, 1, bias, 'circular').to(device)
+    fft_conv = convert_fft_conv(conv)
+
+    y1 = conv(x)
+    y2 = fft_conv(x)
+    assert torch.allclose(
+        y1, y2, atol=1e-5, rtol=1e-5), torch.abs(y1 - y2).max().item()
+    y2.sum().backward()
+
+
 @pytest.mark.parametrize('batch', [1, 4])
 @pytest.mark.parametrize('in_channels', [16, 64])
 @pytest.mark.parametrize('out_channels', [8, 32])
 @pytest.mark.parametrize('length', [1733])
 @pytest.mark.parametrize('kernel_size', [128, 256])
 @pytest.mark.parametrize('stride', [1, 3, 4])
 @pytest.mark.parametrize('dilation', [1, 2, 4])
@@ -25,17 +105,16 @@
                 in_channels, out_channels,
                 kernel_size, stride, padding, dilation, groups, bias, padding_mode):
 
     x = torch.randn(batch, in_channels, length,
                     requires_grad=True, device=device)
     conv = Conv1d(in_channels, out_channels, kernel_size, stride,
                   padding, dilation, groups, bias, padding_mode).to(device)
-    fft_conv = FFTConv1d(in_channels, out_channels, kernel_size,
-                         stride, padding, dilation, groups, bias, padding_mode).to(device)
-    fft_conv.load_state_dict(conv.state_dict())
+    fft_conv = convert_fft_conv(conv)
+    assert isinstance(fft_conv, FFTConv1d)
 
     y1 = conv(x)
     y2 = fft_conv(x)
     assert torch.allclose(
         y1, y2, atol=1e-5, rtol=1e-5), torch.abs(y1 - y2).max().item()
     y2.sum().backward()
 
@@ -46,26 +125,25 @@
 @pytest.mark.parametrize('length', [(101, 101)])
 @pytest.mark.parametrize('kernel_size', [17, 23])
 @pytest.mark.parametrize('stride', [1, 2, 3])
 @pytest.mark.parametrize('dilation', [1, 2, 3])
 @pytest.mark.parametrize('padding', [0, 7])
 @pytest.mark.parametrize('bias', [True, False])
 @pytest.mark.parametrize('groups', [1, 2])
-@pytest.mark.parametrize('padding_mode', ['zeros', 'reflect'])
+@pytest.mark.parametrize('padding_mode', ['zeros', 'circular'])
 def test_conv2d(batch, length,
                 in_channels, out_channels,
                 kernel_size, stride, padding, dilation, groups, bias, padding_mode):
 
     x = torch.randn(batch, in_channels, *length,
                     requires_grad=True, device=device)
     conv = Conv2d(in_channels, out_channels, kernel_size, stride,
                   padding, dilation, groups, bias, padding_mode).to(device)
-    fft_conv = FFTConv2d(in_channels, out_channels, kernel_size,
-                         stride, padding, dilation, groups, bias, padding_mode).to(device)
-    fft_conv.load_state_dict(conv.state_dict())
+    fft_conv = convert_fft_conv(conv)
+    assert isinstance(fft_conv, FFTConv2d)
 
     y1 = conv(x)
     y2 = fft_conv(x)
     assert torch.allclose(
         y1, y2, atol=1e-5, rtol=1e-5), torch.abs(y1 - y2).max().item()
     y2.sum().backward()
 
@@ -85,109 +163,102 @@
                 in_channels, out_channels,
                 kernel_size, stride, padding, dilation, groups, bias, padding_mode):
 
     x = torch.randn(batch, in_channels, *length,
                     requires_grad=True, device=device)
     conv = Conv3d(in_channels, out_channels, kernel_size, stride,
                   padding, dilation, groups, bias, padding_mode).to(device)
-    fft_conv = FFTConv3d(in_channels, out_channels, kernel_size,
-                         stride, padding, dilation, groups, bias, padding_mode).to(device)
-    fft_conv.load_state_dict(conv.state_dict())
+    fft_conv = convert_fft_conv(conv)
+    assert isinstance(fft_conv, FFTConv3d)
 
     y1 = conv(x)
     y2 = fft_conv(x)
     assert torch.allclose(
         y1, y2, atol=1e-5, rtol=1e-5), torch.abs(y1 - y2).max().item()
     y2.sum().backward()
 
 
 @pytest.mark.parametrize('batch', [1, 4])
 @pytest.mark.parametrize('in_channels', [16, 64])
 @pytest.mark.parametrize('out_channels', [8, 32])
 @pytest.mark.parametrize('length', [409])
 @pytest.mark.parametrize('kernel_size', [128, 256])
-@pytest.mark.parametrize('stride', [1, 3, 4])
-@pytest.mark.parametrize('dilation', [1, 2, 4])
+@pytest.mark.parametrize('stride,dilation,output_padding',
+                         [x + (0,) for x in product([1, 3, 4], [1, 2, 4])] + [x + (1,) for x in product([3, 4], [2, 4])])
 @pytest.mark.parametrize('padding', [0, 3])
-@pytest.mark.parametrize('output_padding', [0])
 @pytest.mark.parametrize('bias', [True, False])
 @pytest.mark.parametrize('groups', [1, 4])
 @pytest.mark.parametrize('padding_mode', ['zeros'])
 def test_conv_transpose1d(batch, length,
                           in_channels, out_channels,
                           kernel_size, stride, padding, output_padding, dilation, groups, bias, padding_mode):
 
     x = torch.randn(batch, in_channels, length,
                     requires_grad=True, device=device)
     conv = ConvTranspose1d(in_channels, out_channels, kernel_size, stride,
                            padding, output_padding, groups, bias, dilation, padding_mode).to(device)
-    fft_conv = FFTConvTranspose1d(in_channels, out_channels, kernel_size,
-                                  stride, padding, output_padding, groups, bias, dilation, padding_mode).to(device)
-    fft_conv.load_state_dict(conv.state_dict())
+    fft_conv = convert_fft_conv(conv)
+    assert isinstance(fft_conv, FFTConvTranspose1d)
 
     y1 = conv(x)
     y2 = fft_conv(x)
     assert torch.allclose(
         y1, y2, atol=1e-5, rtol=1e-5), torch.abs(y1 - y2).max().item()
     y2.sum().backward()
 
 
 @pytest.mark.parametrize('batch', [2])
 @pytest.mark.parametrize('in_channels', [8, 32])
 @pytest.mark.parametrize('out_channels', [4, 16])
 @pytest.mark.parametrize('length', [(31, 31)])
 @pytest.mark.parametrize('kernel_size', [17, 23])
-@pytest.mark.parametrize('stride', [1, 2, 3])
-@pytest.mark.parametrize('dilation', [1, 2, 3])
 @pytest.mark.parametrize('padding', [0, 7])
-@pytest.mark.parametrize('output_padding', [0])
+@pytest.mark.parametrize('stride,dilation,output_padding',
+                         [x + (0,) for x in product([1, 2, 3], [1, 2, 3])] + [x + (1,) for x in product([2, 3], [2, 3])])
 @pytest.mark.parametrize('bias', [True, False])
 @pytest.mark.parametrize('groups', [1, 2])
 @pytest.mark.parametrize('padding_mode', ['zeros'])
 def test_conv_transpose2d(batch, length,
                           in_channels, out_channels,
                           kernel_size, stride, padding, output_padding, dilation, groups, bias, padding_mode):
 
     x = torch.randn(batch, in_channels, *length,
                     requires_grad=True, device=device)
     conv = ConvTranspose2d(in_channels, out_channels, kernel_size, stride,
                            padding, output_padding, groups, bias, dilation, padding_mode).to(device)
-    fft_conv = FFTConvTranspose2d(in_channels, out_channels, kernel_size,
-                                  stride, padding, output_padding, groups, bias, dilation, padding_mode).to(device)
-    fft_conv.load_state_dict(conv.state_dict())
+    fft_conv = convert_fft_conv(conv)
+    assert isinstance(fft_conv, FFTConvTranspose2d)
 
     y1 = conv(x)
     y2 = fft_conv(x)
     assert torch.allclose(
         y1, y2, atol=1e-5, rtol=1e-5), torch.abs(y1 - y2).max().item()
     y2.sum().backward()
 
 
 @pytest.mark.parametrize('batch', [2])
 @pytest.mark.parametrize('in_channels', [8])
 @pytest.mark.parametrize('out_channels', [8])
 @pytest.mark.parametrize('length', [(29, 23, 23)])
 @pytest.mark.parametrize('kernel_size', [9, 11])
-@pytest.mark.parametrize('stride', [1, 2, 3])
-@pytest.mark.parametrize('dilation', [1, 2, 3])
 @pytest.mark.parametrize('padding', [6])
-@pytest.mark.parametrize('output_padding', [0])
+@pytest.mark.parametrize('stride,dilation,output_padding',
+                         [x + (0,) for x in product([1, 2, 3], [1, 2, 3])] + [x + (1,) for x in product([2, 3], [2, 3])])
 @pytest.mark.parametrize('bias', [True, False])
 @pytest.mark.parametrize('groups', [1, 2])
 @pytest.mark.parametrize('padding_mode', ['zeros'])
 def test_conv_transpose3d(batch, length,
                           in_channels, out_channels,
                           kernel_size, stride, padding, output_padding, dilation, groups, bias, padding_mode):
 
     x = torch.randn(batch, in_channels, *length,
                     requires_grad=True, device=device)
     conv = ConvTranspose3d(in_channels, out_channels, kernel_size, stride,
                            padding, output_padding, groups, bias, dilation, padding_mode).to(device)
-    fft_conv = FFTConvTranspose3d(in_channels, out_channels, kernel_size,
-                                  stride, padding, output_padding, groups, bias, dilation, padding_mode).to(device)
-    fft_conv.load_state_dict(conv.state_dict())
+    fft_conv = convert_fft_conv(conv)
+    assert isinstance(fft_conv, FFTConvTranspose3d)
 
     y1 = conv(x)
     y2 = fft_conv(x)
     assert torch.allclose(
         y1, y2, atol=1e-5, rtol=1e-5), torch.abs(y1 - y2).max().item()
     y2.sum().backward()
```

### Comparing `torch_fftconv-0.1.2/torch_fftconv/functional.py` & `torch_fftconv-0.1.3/torch_fftconv/functional.py`

 * *Files identical despite different names*

### Comparing `torch_fftconv-0.1.2/torch_fftconv.egg-info/PKG-INFO` & `torch_fftconv-0.1.3/torch_fftconv.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: torch-fftconv
-Version: 0.1.2
+Version: 0.1.3
 Summary: Implementation of 1D, 2D, and 3D FFT convolutions in PyTorch. Much faster than direct convolutions for large kernel sizes
 Home-page: https://github.com/yoyololicon/fft-conv-pytorch
 Author: Chin-Yun Yu
 Author-email: lolimaster.cs03@nctu.edu.tw
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # FFT Conv PyTorch
 
 [![Python package](https://github.com/yoyololicon/fft-conv-pytorch/actions/workflows/python-package.yml/badge.svg?branch=master)](https://github.com/yoyololicon/fft-conv-pytorch/actions/workflows/python-package.yml)
+[![Upload Python Package](https://github.com/yoyololicon/fft-conv-pytorch/actions/workflows/python-publish.yml/badge.svg)](https://github.com/yoyololicon/fft-conv-pytorch/actions/workflows/python-publish.yml)
+[![PyPI version](https://badge.fury.io/py/torch-fftconv.svg)](https://badge.fury.io/py/torch-fftconv)
 
 This is a fork of original [fft-conv-pytorch](https://github.com/fkodom/fft-conv-pytorch).
 I made some modifications to support dilated and strided convolution, so it can be a drop-in-replacement of original PyTorch `Conv*d` modules and `conv*d` functions, with the same function parameters and behavior.
 
 ### Install
 
 ```commandline
@@ -60,8 +60,7 @@
 For details and benchmarks on other parameters, check [this notebook](benchmark.ipynb).
 
 ## TODO
 
 - [ ] Jittability.
 - [x] Dilated Convolution.
 - [x] Transposed Convolution.
-
```

