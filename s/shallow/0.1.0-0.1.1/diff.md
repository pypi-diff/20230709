# Comparing `tmp/shallow-0.1.0.tar.gz` & `tmp/shallow-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shallow-0.1.0.tar", last modified: Fri Jan 27 20:26:13 2023, max compression
+gzip compressed data, was "shallow-0.1.1.tar", last modified: Sat Jul  8 22:19:15 2023, max compression
```

## Comparing `shallow-0.1.0.tar` & `shallow-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 mdm988   (1344792526) domain users (1344200513)        0 2023-01-27 20:26:13.249601 shallow-0.1.0/
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)     1070 2022-08-02 16:27:49.000000 shallow-0.1.0/LICENSE
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      487 2023-01-27 20:26:13.249601 shallow-0.1.0/PKG-INFO
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      218 2023-01-27 20:24:52.000000 shallow-0.1.0/README.md
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)       38 2023-01-27 20:26:13.249601 shallow-0.1.0/setup.cfg
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      595 2023-01-27 20:25:55.000000 shallow-0.1.0/setup.py
-drwxr-xr-x   0 mdm988   (1344792526) domain users (1344200513)        0 2023-01-27 20:26:13.249601 shallow-0.1.0/shallow/
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)        0 2022-11-09 14:53:07.000000 shallow-0.1.0/shallow/__init__.py
-drwxr-xr-x   0 mdm988   (1344792526) domain users (1344200513)        0 2023-01-27 20:26:13.249601 shallow-0.1.0/shallow/pyro/
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)        0 2023-01-11 13:42:11.000000 shallow-0.1.0/shallow/pyro/__init__.py
-drwxr-xr-x   0 mdm988   (1344792526) domain users (1344200513)        0 2023-01-27 20:26:13.249601 shallow-0.1.0/shallow/tensorflow/
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)        0 2022-11-09 14:53:07.000000 shallow-0.1.0/shallow/tensorflow/__init__.py
-drwxr-xr-x   0 mdm988   (1344792526) domain users (1344200513)        0 2023-01-27 20:26:13.249601 shallow-0.1.0/shallow/torch/
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)    12867 2023-01-11 13:42:11.000000 shallow-0.1.0/shallow/torch/__init__.py
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)    20698 2023-01-27 20:04:05.000000 shallow-0.1.0/shallow/torch/flows.py
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)    10407 2023-01-27 20:05:43.000000 shallow-0.1.0/shallow/torch/nets.py
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      664 2023-01-26 18:19:00.000000 shallow-0.1.0/shallow/torch/train.py
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)     1387 2023-01-27 19:56:44.000000 shallow-0.1.0/shallow/torch/utils.py
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)     2067 2023-01-27 20:09:57.000000 shallow-0.1.0/shallow/utils.py
-drwxr-xr-x   0 mdm988   (1344792526) domain users (1344200513)        0 2023-01-27 20:26:13.249601 shallow-0.1.0/shallow.egg-info/
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      487 2023-01-27 20:26:13.000000 shallow-0.1.0/shallow.egg-info/PKG-INFO
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      390 2023-01-27 20:26:13.000000 shallow-0.1.0/shallow.egg-info/SOURCES.txt
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)        1 2023-01-27 20:26:13.000000 shallow-0.1.0/shallow.egg-info/dependency_links.txt
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)       17 2023-01-27 20:26:13.000000 shallow-0.1.0/shallow.egg-info/requires.txt
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)        8 2023-01-27 20:26:13.000000 shallow-0.1.0/shallow.egg-info/top_level.txt
+drwxr-xr-x   0 mdm988   (1344792526) domain users (1344200513)        0 2023-07-08 22:19:15.222496 shallow-0.1.1/
+-rwxrwxrwx   0 mdm988   (1344792526) domain users (1344200513)     1070 2023-05-10 14:38:12.000000 shallow-0.1.1/LICENSE
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      487 2023-07-08 22:19:15.222496 shallow-0.1.1/PKG-INFO
+-rwxrwxrwx   0 mdm988   (1344792526) domain users (1344200513)      218 2023-05-10 14:38:12.000000 shallow-0.1.1/README.md
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)       38 2023-07-08 22:19:15.222496 shallow-0.1.1/setup.cfg
+-rwxrwxrwx   0 mdm988   (1344792526) domain users (1344200513)      611 2023-07-08 22:18:53.000000 shallow-0.1.1/setup.py
+drwxr-xr-x   0 mdm988   (1344792526) domain users (1344200513)        0 2023-07-08 22:19:15.222496 shallow-0.1.1/shallow/
+-rwxrwxrwx   0 mdm988   (1344792526) domain users (1344200513)        0 2023-05-10 14:38:12.000000 shallow-0.1.1/shallow/__init__.py
+drwxr-xr-x   0 mdm988   (1344792526) domain users (1344200513)        0 2023-07-08 22:19:15.222496 shallow-0.1.1/shallow/pyro/
+-rwxrwxrwx   0 mdm988   (1344792526) domain users (1344200513)        0 2023-05-10 14:38:12.000000 shallow-0.1.1/shallow/pyro/__init__.py
+drwxr-xr-x   0 mdm988   (1344792526) domain users (1344200513)        0 2023-07-08 22:19:15.222496 shallow-0.1.1/shallow/tensorflow/
+-rwxrwxrwx   0 mdm988   (1344792526) domain users (1344200513)        0 2023-05-10 14:38:12.000000 shallow-0.1.1/shallow/tensorflow/__init__.py
+drwxr-xr-x   0 mdm988   (1344792526) domain users (1344200513)        0 2023-07-08 22:19:15.222496 shallow-0.1.1/shallow/torch/
+-rwxrwxrwx   0 mdm988   (1344792526) domain users (1344200513)    12867 2023-05-10 14:38:12.000000 shallow-0.1.1/shallow/torch/__init__.py
+-rwxrwxrwx   0 mdm988   (1344792526) domain users (1344200513)    21544 2023-05-10 14:38:12.000000 shallow-0.1.1/shallow/torch/flows.py
+-rwxrwxrwx   0 mdm988   (1344792526) domain users (1344200513)    13192 2023-05-10 14:38:12.000000 shallow-0.1.1/shallow/torch/nets.py
+-rwxrwxrwx   0 mdm988   (1344792526) domain users (1344200513)      720 2023-05-10 14:38:12.000000 shallow-0.1.1/shallow/torch/training.py
+-rwxrwxrwx   0 mdm988   (1344792526) domain users (1344200513)     2299 2023-05-10 14:38:12.000000 shallow-0.1.1/shallow/torch/utils.py
+-rwxrwxrwx   0 mdm988   (1344792526) domain users (1344200513)     2067 2023-05-10 14:38:12.000000 shallow-0.1.1/shallow/utils.py
+drwxr-xr-x   0 mdm988   (1344792526) domain users (1344200513)        0 2023-07-08 22:19:15.222496 shallow-0.1.1/shallow.egg-info/
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      487 2023-07-08 22:19:15.000000 shallow-0.1.1/shallow.egg-info/PKG-INFO
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      393 2023-07-08 22:19:15.000000 shallow-0.1.1/shallow.egg-info/SOURCES.txt
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)        1 2023-07-08 22:19:15.000000 shallow-0.1.1/shallow.egg-info/dependency_links.txt
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)       17 2023-07-08 22:19:15.000000 shallow-0.1.1/shallow.egg-info/requires.txt
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)        8 2023-07-08 22:19:15.000000 shallow-0.1.1/shallow.egg-info/top_level.txt
```

### Comparing `shallow-0.1.0/LICENSE` & `shallow-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shallow-0.1.0/setup.py` & `shallow-0.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 name = 'shallow'
-version = '0.1.0'
+version = '0.1.1' # current 0.1.1
 
 with open('README.md' ,'r') as f:
     long_description = f.read().strip()
 
 setup(
     name=name,
     version=version,
```

### Comparing `shallow-0.1.0/shallow/torch/__init__.py` & `shallow-0.1.1/shallow/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `shallow-0.1.0/shallow/torch/flows.py` & `shallow-0.1.1/shallow/torch/flows.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 import numpy as np
 from tqdm import tqdm
 from copy import deepcopy
 import torch
-from torch import nn
-from nflows.utils import(
-    create_alternating_binary_mask,
-    create_mid_split_binary_mask,
-    create_random_binary_mask,
-    )
-from nflows.nn.nets import ResidualNet
-from nflows.flows import Flow
+
 from nflows.distributions import StandardNormal
+from nflows.flows import Flow
 from nflows.transforms import(
     Transform,
     CompositeTransform,
     InverseTransform,
     IdentityTransform,
     PointwiseAffineTransform as AffineTransform,
     Exp,
@@ -24,55 +18,74 @@
     RandomPermutation,
     ReversePermutation,
     LULinear,
     MaskedAffineAutoregressiveTransform,
     PiecewiseRationalQuadraticCouplingTransform,
     MaskedPiecewiseRationalQuadraticAutoregressiveTransform,
     )
+from nflows.utils import(
+    create_alternating_binary_mask,
+    create_mid_split_binary_mask,
+    create_random_binary_mask,
+    )
 
 from .utils import cpu, device, get_activation, get_optimizer, shift_and_scale
-from .nets import AffineModule
-from .train import Trainer
+from .nets import NormModule, ForwardNetwork, ResidualNetwork
+from .training import Trainer ## TODO
+
+
+class NormTransform(AffineTransform):
+
+    def __init__(self, inputs):
+        
+        if type(inputs) is int:
+            shift = torch.zeros(inputs)
+            scale = torch.ones(inputs)
+            
+        else:
+            shift, scale = shift_and_scale(inputs)
+            
+        super().__init__(shift, scale)
 
 
 # Apply indpendent feature-wise (i.e., last axis) transforms
 # similar to:
-# https://www.tensorflow.org/probability/api_docs/python/tfp/bijectors/Blockwise
-# https://pytorch.org/docs/stable/_modules/torch/distributions/transforms.html#StackTransform
-# Details based on https://github.com/bayesiains/nflows/blob/master/nflows/transforms/base.py#L32
+# tnesorflow_probability.bijectors.Blockwise
+# torch.distributions.transforms.StackTransform
 class FeaturewiseTransform(Transform):
 
     def __init__(self, transforms):
     
         super().__init__()
-        self.transforms = torch.nn.ModuleList(transforms)
-        self.dim = -1
+        
+        self.forwards = [t.forward for t in transforms]
+        self.inverses = [t.inverse for t in transforms]
         
     def _map(self, transforms, inputs, context=None):
     
-        assert inputs.size(self.dim) == len(self.transforms)
+        assert inputs.size(-1) == len(transforms)
 
         outputs = torch.zeros_like(inputs)
-        logabsdet = torch.zeros_like(inputs)
+        logabsdet = torch.zeros(inputs.shape[0])
+        
         for i, transform in enumerate(transforms):
-            outputs[..., [i]], logabsdet[..., i] = transform(
-                inputs[..., [i]], context=context)
-        logabsdet = torch.sum(logabsdet, dim=self.dim)
+            outputs[..., [i]], logabsdet_ = transform(
+                inputs[..., [i]], context=context,
+                )
+            logabsdet += logabsdet_
 
         return outputs, logabsdet
         
     def forward(self, inputs, context=None):
 
-        return self._map(
-            (t.forward for t in self.transforms), inputs, context=context)
+        return self._map(self.forwards, inputs, context=context)
         
     def inverse(self, inputs, context=None):
         
-        return self._map(
-            (t.inverse for t in self.transforms), inputs, context=context)
+        return self._map(self.inverses, inputs, context=context)
 
 
 # Wrapper inspired by features from sbi and glasflow
 # https://github.com/mackelab/sbi/blob/main/sbi/neural_nets/flow.py
 # https://github.com/igr-ml/glasflow/blob/main/src/glasflow/flows/coupling.py
 # Features include:
 # - conditional densities
@@ -87,14 +100,15 @@
         self,
         inputs=1, # Number of parameter dimensions
         contexts=None, # Number of conditional dimensions
         bounds=None, # Parameter boundaries
         norm_inputs=False, # Standardize parameters, bool or array/tensor
         norm_contexts=False, # Standardize contexts, bool or array/tensor
         transforms=1, # Number of flow layers
+        residual=False, # MLP (False) or residual network (True)
         blocks=1, # Number of blocks/layers in the net
         hidden=1, # Number of hidden units in each block/layer of the net
         activation='relu', # Activation function
         dropout=0.0, # Dropout probability for hidden units, 0 <= dropout < 1
         batchnorm_within=False, # Batch normalization within the net
         batchnorm_between=False, # Batch normalization between flow layers
         permutation=None, # None, 'random', 'reverse', or list
@@ -102,241 +116,285 @@
         embedding=None, # Network to embed contexts
         distribution=None, # None (standard normal) or nflows Distribution
         **kwargs, # Keyword arguments passed to transform constructor
         ):
         
         self.inputs = inputs
         self.contexts = contexts
-        self.hidden = hidden
+        self.residual = residual
         self.blocks = blocks
-        self.activation = get_activation(activation, functional=True)
+        self.hidden = hidden
+        self.activation = activation
         self.dropout = dropout
         self.batchnorm_within = batchnorm_within
-        
-        # Fixed pre-transforms for bounded densities and standardization
-        pre_transform = []
-        
-        # Enforce boundaries
-        if bounds is not None:
-            assert len(bounds) == inputs
-            
-            # Add bijection required for each dimension
-            featurewise_transform = []
-            for bound in bounds:
-                
-                # Unbounded dimension
-                if (bound is None) or all(b is None for b in bound):
-                    featurewise_transform.append(IdentityTransform())
-                    
-                # One side unbounded
-                elif any(b is None for b in bound):
-                    # Left unbounded
-                    if bound[0] is None:
-                        shift = bound[1]
-                        scale = -1.0
-                    # Right unbounded
-                    elif bound[1] is None:
-                        shift = bound[0]
-                        scale = 1.0
-                    featurewise_transform.append(CompositeTransform([
-                        InverseTransform(AffineTransform(shift, scale)),
-                        InverseTransform(Exp()),
-                        ]))
-                
-                # Bounded
-                else:
-                    shift = min(bound)
-                    scale = max(bound) - min(bound)
-                    featurewise_transform.append(CompositeTransform([
-                        InverseTransform(AffineTransform(shift, scale)),
-                        InverseTransform(Sigmoid()),
-                        ]))
-                    
-            # Combine per-dimension bijections into one bijection
-            featurewise_transform = FeaturewiseTransform(featurewise_transform)
-            pre_transform.append(featurewise_transform)
-            
-        # Zero mean + unit variance per parameter dimension
-        if norm_inputs is not False:
-            # Place holder for loading state dict
-            if norm_inputs is True:
-                shift, scale = torch.zeros(inputs), torch.ones(inputs)
-            # Input tensor to compute mean and variance from
-            else:
-                norm_inputs = torch.as_tensor(norm_inputs)
-                assert norm_inputs.size(-1) == inputs
-                # Rescaling after boundary-enforcing bijection
-                if bounds is not None:
-                    norm_inputs = featurewise_transform.forward(norm_inputs)[0]
-                shift, scale = shift_and_scale(norm_inputs)
-            norm_transform = AffineTransform(shift, scale)
-            pre_transform.append(norm_transform)
             
+        # Zero mean + unit variance per context dimension
         if contexts is not None:
-            # Zero mean + unit variance per context dimension
-            if norm_contexts is not False:
-                # Place holder for loading state dict
-                if norm_contexts is True:
-                    shift, scale = torch.zeros(contexts), torch.ones(contexts)
-                # Input tensor to compute mean and variance from
-                else:
-                    norm_contexts = torch.as_tensor(norm_contexts)
-                    assert norm_contexts.size(-1) == contexts
-                    shift, scale = shift_and_scale(norm_contexts)
-                norm_embedding = AffineModule(shift, scale)
-                # Rescaling before context embedding network
-                if embedding is None:
-                    embedding = norm_embedding
-                else:
-                    embedding = nn.Sequential(norm_embedding, embedding)
-        else:
-            assert norm_contexts is False and embedding is None
+            embedding = self._get_embedding(norm_contexts, embedding)
+            
+        # Pre-transformations for boundaries and normalization
+        pre_transform = self._get_pre_transform(bounds, norm_inputs)
                 
         # Main transforms in the flow
-        main_transform = []
+        main_transform = self._get_main_transform(
+            transforms, permutation, linear, batchnorm_between, kwargs,
+            )
+
+        transform = CompositeTransform([pre_transform, main_transform])
         
-        for i in range(transforms):
-            
-            # Permute parameter order between flow layers
-            if permutation is not None:
-                if permutation == 'random':
-                    main_transform.append(RandomPermutation(inputs))
-                elif permutation == 'reverse':
-                    main_transform.append(ReversePermutation(inputs))
-                else:
-                    main_transform.append(Permutation(permutation))
-            
-            # Linear layer
-            if linear is not None:
-                if linear == 'lu':
-                    main_transform.append(LULinear(inputs, identity_init=True))
-                    
-            # Main bijection in this flow layers
-            main_transform.append(self._get_transform(**kwargs))
-            
-            # Batch normalization at the end of the flow layers
-            if batchnorm_between:
-                main_transform.append(BatchNorm(inputs))
-                
-        transform = CompositeTransform(pre_transform + main_transform)
         if distribution is None:
             distribution = StandardNormal((inputs,))
+            
         super().__init__(transform, distribution, embedding_net=embedding)
         
-        ## TODO: don't double register modules/parameters
-        self._pre_transform = CompositeTransform(pre_transform)
-        self._main_transform = CompositeTransform(main_transform)
-        
     def prob(self, inputs, context=None):
-        
+
         return torch.exp(self.log_prob(inputs, context=context))
-    
+
     # log_prob without scaling factors due to the fixed pre-transforms
-    # Based on https://github.com/bayesiains/nflows/blob/master/nflows/distributions/base.py#L16
+    # Based on nflows.distributions.base.Distribution.log_prob
+    # and nflows.flows.base.Flow._log_prob
     def _log_prob_without_pre(self, inputs, context=None):
         
         inputs = torch.as_tensor(inputs)
         if context is not None:
             context = torch.as_tensor(context)
             if inputs.shape[0] != context.shape[0]:
                 raise ValueError(
                     'Number of inputs must equal number of contexts.'
                     )
                 
         context = self._embedding_net(context)
-        inputs = self._pre_transform(inputs, context=context)[0]
-        noise, logabsdet = self._main_transform(inputs, context=context)
+        pre_transform, main_transform = self._transform._transforms
+        inputs = pre_transform(inputs, context=context)[0]
+        noise, logabsdet = main_transform(inputs, context=context)
         log_prob = self._distribution.log_prob(noise)
         
         return log_prob + logabsdet
     
+    def _get_embedding(self, norm_contexts, embedding):
+            
+        if norm_contexts is not False:
+            norm_embedding = NormModule(
+                self.contexts if norm_contexts is True else norm_contexts,
+                )
+
+            # Rescaling before context embedding network
+            if embedding is None:
+                embedding = norm_embedding
+            else:
+                embedding = torch.nn.Sequential(norm_embedding, embedding)
+                
+        else:
+            assert embedding is None
+                
+        return embedding
+
+    # Combine per-dimension bounds into one bijection
+    def _get_bounds_transform(self, bounds):
+        
+        assert len(bounds) == self.inputs
+
+        # Add bijection required for each dimension
+        featurewise_transforms = []
+        
+        for bound in bounds:
+
+            # Unbounded dimension
+            if (bound is None) or all(b is None for b in bound):
+                featurewise_transforms.append(IdentityTransform())
+
+            # One side unbounded
+            elif any(b is None for b in bound):
+                # Left unbounded
+                if bound[0] is None:
+                    shift = bound[1]
+                    scale = -1.0
+                # Right unbounded
+                elif bound[1] is None:
+                    shift = bound[0]
+                    scale = 1.0
+                featurewise_transforms.append(CompositeTransform([
+                    InverseTransform(AffineTransform(shift, scale)),
+                    InverseTransform(Exp()),
+                    ]))
+
+            # Bounded
+            else:
+                shift = min(bound)
+                scale = max(bound) - min(bound)
+                featurewise_transforms.append(CompositeTransform([
+                    InverseTransform(AffineTransform(shift, scale)),
+                    InverseTransform(Sigmoid()),
+                    ]))
+
+        return FeaturewiseTransform(featurewise_transforms)
+    
+    def _get_norm_transform(self, norm_inputs):
+        
+        return NormTransform(
+            self.inputs if norm_inputs is True else norm_inputs,
+            )
+
+    # Fixed pre-transforms for bounded densities and standardization
+    def _get_pre_transform(self, bounds, norm_inputs):
+        
+        pre_transform = IdentityTransform()
+
+        # Enforce boundaries
+        if bounds is not None:
+            pre_transform = self._get_bounds_transform(bounds)
+            
+        # Zero mean + unit variance per parameter dimension
+        if norm_inputs is not False:
+            if norm_inputs is not True:
+                norm_inputs = pre_transform(torch.as_tensor(norm_inputs))[0]
+            pre_transform = CompositeTransform(
+                [pre_transform, self._get_norm_transform(norm_inputs)],
+                )
+            
+        return pre_transform
+    
+    def _get_main_transform(
+        self, transforms, permutation, linear, batchnorm_between, kwargs,
+        ):
+        
+        main_transforms = []
+        
+        for i in range(transforms):
+            
+            # Permute parameter order between flow layers
+            if permutation is not None:
+                if permutation == 'random':
+                    main_transforms.append(RandomPermutation(self.inputs))
+                elif permutation == 'reverse':
+                    main_transforms.append(ReversePermutation(self.inputs))
+                else:
+                    assert len(permutation) == self.inputs
+                    main_transforms.append(Permutation(permutation))
+            
+            # Linear layer
+            if linear is not None:
+                if linear == 'lu':
+                    main_transforms.append(
+                        LULinear(self.inputs, identity_init=True),
+                        )
+                    
+            # Main bijection in this flow layers
+            main_transforms.append(self._get_transform(**kwargs))
+            
+            # Batch normalization at the end of the flow layers
+            if batchnorm_between:
+                main_transforms.append(BatchNorm(self.inputs))
+
+        return CompositeTransform(main_transforms)
+    
     def _get_transform(self, **kwargs):
         
         raise NotImplementedError
         
 
-# Masked affine autoregressivle flow
-# Use InverseTransform(AffineAutoregressiveFlow)
-# for inverse autoregressive flow
+# Masked affine autoregressive flow
+# InverseTransform(AffineAutoregressiveFlow) for inverse autoregressive flow
 class AffineAutoregressiveFlow(BaseFlow):
     
-    def _get_transform(self, residual=False, mask=False):
+    def _get_transform(self, mask=False):
         
         return MaskedAffineAutoregressiveTransform(
             self.inputs,
             self.hidden,
             context_features=self.contexts,
             num_blocks=self.blocks,
-            use_residual_blocks=residual,
+            use_residual_blocks=self.residual,
             random_mask=mask,
-            activation=self.activation,
+            activation=get_activation(self.activation, functional=True),
             dropout_probability=self.dropout,
             use_batch_norm=self.batchnorm_within,
             )
+
+
+class AutoregressiveNeuralSplineFlow(BaseFlow):
     
+    def _get_transform(
+        self, mask=False, bins=5, tails='linear', bound=5.0,
+        ):
+        
+        return MaskedPiecewiseRationalQuadraticAutoregressiveTransform(
+            self.inputs,
+            self.hidden,
+            context_features=self.contexts,
+            num_bins=bins,
+            tails=tails,
+            tail_bound=bound,
+            num_blocks=self.blocks,
+            use_residual_blocks=self.residual,
+            random_mask=mask,
+            activation=get_activation(self.activation, functional=True),
+            dropout_probability=self.dropout,
+            use_batch_norm=self.batchnorm_within,
+            )
+
 
-## TODO: allow non-residual blocks
 class CouplingNeuralSplineFlow(BaseFlow):
     
     def _get_transform(
-        self, residual=True, mask='mid', bins=5, tails='linear', bound=5.0,
+        self, mask='mid', bins=5, tails='linear', bound=5.0,
         ):
         
         if type(mask) is str:
             mask = dict(
                 alternating=create_alternating_binary_mask(self.inputs),
                 mid=create_mid_split_binary_mask(self.inputs),
                 random=create_random_binary_mask(self.inputs),
                 )[mask]
-            
-        if residual:
-            net = lambda inputs, outputs: ResidualNet(
-                inputs,
-                outputs,
-                hidden_features=self.hidden,
-                context_features=self.contexts,
-                num_blocks=self.blocks,
-                activation=self.activation,
-                dropout_probability=self.dropout,
-                use_batch_norm=self.batchnorm_within,
-                )
-        else:
-            net = lambda inputs, outputs: None
+
+        net = ResidualNetwork if self.residual else ForwardNetwork
+        fn = lambda inputs, outputs: net(
+            inputs=inputs,
+            outputs=outputs,
+            contexts=self.contexts,
+            blocks=self.blocks,
+            hidden=self.hidden,
+            activation=self.activation,
+            dropout=self.dropout,
+            batchnorm=self.batchnorm_within,
+            )
+
+        # if residual:
+        #     net = lambda inputs, outputs: ResidualNet(
+        #         inputs,
+        #         outputs,
+        #         context_features=self.contexts,
+        #         num_blocks=self.blocks,
+        #         hidden_features=self.hidden,
+        #         activation=get_activation(self.activation, functional=True),
+        #         dropout_probability=self.dropout,
+        #         use_batch_norm=self.batchnorm_within,
+        #         )
+        # else:
+        #     net = lambda inputs, outputs: ForwardNet(
+        #         inputs=inputs,
+        #         outputs=outputs,
+        #         contexts=self.contexts,
+        #         blocks=self.blocks,
+        #         hidden=self.hidden,
+        #         activation=self.activation,
+        #         dropout=self.dropout,
+        #         batchnorm=self.batchnorm_within,
+        #         )
         
         return PiecewiseRationalQuadraticCouplingTransform(
             mask=mask,
-            transform_net_create_fn=net,
+            transform_net_create_fn=fn,
             num_bins=bins,
             tails=tails,
             tail_bound=bound,
             )
 
 
-class AutoregressiveNeuralSplineFlow(BaseFlow):
-    
-    def _get_transform(
-        self, residual=False, mask=False, bins=5, tails='linear', bound=5.0,
-        ):
-        
-        return MaskedPiecewiseRationalQuadraticAutoregressiveTransform(
-            self.inputs,
-            self.hidden,
-            context_features=self.contexts,
-            num_bins=bins,
-            tails=tails,
-            tail_bound=bound,
-            num_blocks=self.blocks,
-            use_residual_blocks=residual,
-            random_mask=mask,
-            activation=self.activation,
-            dropout_probability=self.dropout,
-            use_batch_norm=self.batchnorm_within,
-            )
-    
-
 ## TODO: sub-class train.Trainer
 def trainer(
     model,
     inputs,
     contexts=None,
     inputs_valid=None,
     contexts_valid=None,
@@ -432,15 +490,15 @@
     
     optimizer = get_optimizer(optimizer)(
         model.parameters(), lr=learning_rate, weight_decay=weight_decay,
         )
     
     best_model = deepcopy(model.state_dict())
     best_epoch = 0
-    best_loss = np.inf
+    best_loss = float('inf')
     losses = {'train': []}
     if validate:
         losses['valid'] = []
     if reduce is not None:
            epoch_reduce = 0
         
     for epoch in range(1, epochs + 1):
```

### Comparing `shallow-0.1.0/shallow/torch/train.py` & `shallow-0.1.1/shallow/torch/training.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,17 +16,23 @@
 
 
 def kl_divergence(pred, true):
     return cross_entropy(pred, true) - cross_entropy(true, true)
 
 
 def binary_kl_divergence(pred, true):
-    return binary_cross_entropy(pred, true) - binary_cross_entropy(true, true)
+    return (
+        binary_cross_entropy(pred, true) -
+        binary_cross_entropy(true, true)
+        )
 
 
 ## TODO: base training class
 class Trainer:
     
-    def __init__(self):
+    def __init__(
+        self,
+        
+        ):
         
         pass
```

### Comparing `shallow-0.1.0/shallow/utils.py` & `shallow-0.1.1/shallow/utils.py`

 * *Files identical despite different names*

