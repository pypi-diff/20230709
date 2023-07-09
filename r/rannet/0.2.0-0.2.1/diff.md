# Comparing `tmp/rannet-0.2.0.tar.gz` & `tmp/rannet-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rannet-0.2.0.tar", last modified: Mon Jul  3 12:47:49 2023, max compression
+gzip compressed data, was "rannet-0.2.1.tar", last modified: Sun Jul  9 12:52:53 2023, max compression
```

## Comparing `rannet-0.2.0.tar` & `rannet-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2023-07-03 12:47:49.317198 rannet-0.2.0/
--rw-r--r--   0 seanlee    (501) staff       (20)     1060 2023-07-03 12:41:23.000000 rannet-0.2.0/LICENSE
--rw-r--r--   0 seanlee    (501) staff       (20)     5559 2023-07-03 12:47:49.317706 rannet-0.2.0/PKG-INFO
--rw-r--r--   0 seanlee    (501) staff       (20)     4851 2023-07-03 12:43:34.000000 rannet-0.2.0/README.md
-drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2023-07-03 12:47:49.310972 rannet-0.2.0/rannet/
--rw-r--r--   0 seanlee    (501) staff       (20)      323 2023-07-03 12:47:22.000000 rannet-0.2.0/rannet/__init__.py
--rw-r--r--   0 seanlee    (501) staff       (20)     9124 2023-07-03 12:41:23.000000 rannet-0.2.0/rannet/dataloader.py
--rw-r--r--   0 seanlee    (501) staff       (20)    24517 2023-07-03 12:41:23.000000 rannet-0.2.0/rannet/layers.py
--rw-r--r--   0 seanlee    (501) staff       (20)    17145 2023-07-03 12:41:23.000000 rannet-0.2.0/rannet/optimizer.py
--rw-r--r--   0 seanlee    (501) staff       (20)    14505 2023-07-03 12:41:23.000000 rannet-0.2.0/rannet/pretrain.py
--rw-r--r--   0 seanlee    (501) staff       (20)    29604 2023-07-03 12:41:23.000000 rannet-0.2.0/rannet/ran.py
--rw-r--r--   0 seanlee    (501) staff       (20)    25454 2023-07-03 12:44:13.000000 rannet-0.2.0/rannet/rannet.py
--rw-r--r--   0 seanlee    (501) staff       (20)     6394 2023-07-03 12:41:23.000000 rannet-0.2.0/rannet/tokenizer.py
--rw-r--r--   0 seanlee    (501) staff       (20)     1808 2023-07-03 12:41:23.000000 rannet-0.2.0/rannet/utils.py
-drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2023-07-03 12:47:49.316002 rannet-0.2.0/rannet.egg-info/
--rw-r--r--   0 seanlee    (501) staff       (20)     5559 2023-07-03 12:47:49.000000 rannet-0.2.0/rannet.egg-info/PKG-INFO
--rw-r--r--   0 seanlee    (501) staff       (20)      377 2023-07-03 12:47:49.000000 rannet-0.2.0/rannet.egg-info/SOURCES.txt
--rw-r--r--   0 seanlee    (501) staff       (20)        1 2023-07-03 12:47:49.000000 rannet-0.2.0/rannet.egg-info/dependency_links.txt
--rw-r--r--   0 seanlee    (501) staff       (20)        1 2023-07-03 12:47:49.000000 rannet-0.2.0/rannet.egg-info/not-zip-safe
--rw-r--r--   0 seanlee    (501) staff       (20)       31 2023-07-03 12:47:49.000000 rannet-0.2.0/rannet.egg-info/requires.txt
--rw-r--r--   0 seanlee    (501) staff       (20)        7 2023-07-03 12:47:49.000000 rannet-0.2.0/rannet.egg-info/top_level.txt
--rw-r--r--   0 seanlee    (501) staff       (20)      163 2023-07-03 12:47:49.319594 rannet-0.2.0/setup.cfg
--rw-r--r--   0 seanlee    (501) staff       (20)     1395 2023-07-03 12:47:22.000000 rannet-0.2.0/setup.py
+drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2023-07-09 12:52:53.699108 rannet-0.2.1/
+-rw-r--r--   0 seanlee    (501) staff       (20)     1060 2023-07-03 12:41:23.000000 rannet-0.2.1/LICENSE
+-rw-r--r--   0 seanlee    (501) staff       (20)     5581 2023-07-09 12:52:53.699308 rannet-0.2.1/PKG-INFO
+-rw-r--r--   0 seanlee    (501) staff       (20)     4873 2023-07-09 12:48:49.000000 rannet-0.2.1/README.md
+drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2023-07-09 12:52:53.690859 rannet-0.2.1/rannet/
+-rw-r--r--   0 seanlee    (501) staff       (20)      323 2023-07-09 12:52:22.000000 rannet-0.2.1/rannet/__init__.py
+-rw-r--r--   0 seanlee    (501) staff       (20)     9124 2023-07-03 12:41:23.000000 rannet-0.2.1/rannet/dataloader.py
+-rw-r--r--   0 seanlee    (501) staff       (20)    24517 2023-07-03 12:41:23.000000 rannet-0.2.1/rannet/layers.py
+-rw-r--r--   0 seanlee    (501) staff       (20)    17145 2023-07-03 12:41:23.000000 rannet-0.2.1/rannet/optimizer.py
+-rw-r--r--   0 seanlee    (501) staff       (20)    14505 2023-07-03 12:41:23.000000 rannet-0.2.1/rannet/pretrain.py
+-rw-r--r--   0 seanlee    (501) staff       (20)    29604 2023-07-09 09:11:20.000000 rannet-0.2.1/rannet/ran.py
+-rw-r--r--   0 seanlee    (501) staff       (20)    25469 2023-07-09 12:48:49.000000 rannet-0.2.1/rannet/rannet.py
+-rw-r--r--   0 seanlee    (501) staff       (20)     6394 2023-07-03 12:41:23.000000 rannet-0.2.1/rannet/tokenizer.py
+-rw-r--r--   0 seanlee    (501) staff       (20)     1808 2023-07-03 12:41:23.000000 rannet-0.2.1/rannet/utils.py
+drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2023-07-09 12:52:53.698403 rannet-0.2.1/rannet.egg-info/
+-rw-r--r--   0 seanlee    (501) staff       (20)     5581 2023-07-09 12:52:53.000000 rannet-0.2.1/rannet.egg-info/PKG-INFO
+-rw-r--r--   0 seanlee    (501) staff       (20)      377 2023-07-09 12:52:53.000000 rannet-0.2.1/rannet.egg-info/SOURCES.txt
+-rw-r--r--   0 seanlee    (501) staff       (20)        1 2023-07-09 12:52:53.000000 rannet-0.2.1/rannet.egg-info/dependency_links.txt
+-rw-r--r--   0 seanlee    (501) staff       (20)        1 2023-07-09 10:02:43.000000 rannet-0.2.1/rannet.egg-info/not-zip-safe
+-rw-r--r--   0 seanlee    (501) staff       (20)       31 2023-07-09 12:52:53.000000 rannet-0.2.1/rannet.egg-info/requires.txt
+-rw-r--r--   0 seanlee    (501) staff       (20)        7 2023-07-09 12:52:53.000000 rannet-0.2.1/rannet.egg-info/top_level.txt
+-rw-r--r--   0 seanlee    (501) staff       (20)      163 2023-07-09 12:52:53.700006 rannet-0.2.1/setup.cfg
+-rw-r--r--   0 seanlee    (501) staff       (20)     1395 2023-07-09 12:52:22.000000 rannet-0.2.1/setup.py
```

### Comparing `rannet-0.2.0/LICENSE` & `rannet-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rannet-0.2.0/PKG-INFO` & `rannet-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rannet
-Version: 0.2.0
+Version: 0.2.1
 Summary: Recurrent Attention Networks
 Author: sean lee
 Author-email: xmlee97@gmail.com
 Keywords: rannet
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -70,15 +70,15 @@
 
 # 🚀 Quick Tour
 
 ## 🈶 w/ pretrained models
 
 *Extract semantic feature*
 
-set `apply_cell_transform=False` to extract semantic feature.
+set `return_sequences=False` to extract semantic feature.
 
 ```python
 import numpy as np
 from rannet import RanNet, RanNetWordPieceTokenizer
 
 
 vocab_path = 'pretrained/vocab.txt'
@@ -86,15 +86,16 @@
 config_path = 'pretrained/config.json'
 tokenizer = RanNetWordPieceTokenizer(vocab_path, lowercase=True)
 
 rannet, rannet_model = RanNet.load_rannet(
     config_path=config_path,
     checkpoint_path=ckpt_path,
     return_sequences=False,
-    apply_cell_transform=False
+    apply_cell_transform=False,
+    cell_pooling='mean'
 )
 text = 'input text'
 tok = tokenizer.encode(text)
 vec = rannet_model.predict(np.array([tok.ids]))
 ```
 
 *For the classification task*
@@ -125,15 +126,15 @@
 
 vocab_path = 'pretrained/vocab.txt'
 ckpt_path = 'pretrained/model.ckpt'
 config_path = 'pretrained/config.json'
 tokenizer = RanNetWordPieceTokenizer(vocab_path, lowercase=True)
 
 rannet, rannet_model = RanNet.load_rannet(
-    config_path=config_path, checkpoint_path=ckpt_path, return_gpc=False)
+    config_path=config_path, checkpoint_path=ckpt_path, return_cell=False)
 output = rannet_model.output  # (B, L, D)
 rannet_model.summary()
 ```
 
 ## 🈚 w/o pretrained models
 
 Embed the `RAN` (a Keras layer) into your network.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rannet Version: 0.2.0 Summary: Recurrent Attention
+Metadata-Version: 2.1 Name: rannet Version: 0.2.1 Summary: Recurrent Attention
 Networks Author: sean lee Author-email: xmlee97@gmail.com Keywords: rannet
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
@@ -22,35 +22,35 @@
 view?usp=sharing) | [base](https://pan.baidu.com/s/18uhAkY46aIcy4ncwzXp5mA)\
 [code: djkj\] | | CN | [base](https://drive.google.com/file/d/1_gmrulSU-
 ln_jElc2hktPTTQDzaeG1wU/view?usp=sharing) \| [small](https://drive.google.com/
 file/d/1D-FCxY_UMwZCkvcwl6hkRcl6VnCzRGIj/view?usp=sharing) | [base](https://
 pan.baidu.com/s/1WIcePgmqb7Ox0w1qigWQ_w)\[code: e47w\] \| [small](https://
 pan.baidu.com/s/17DAboL9w0mArcBBuiy3tGg)\[code: mdmg\] | # ð Quick Tour ##
 ð¶ w/ pretrained models *Extract semantic feature* set
-`apply_cell_transform=False` to extract semantic feature. ```python import
-numpy as np from rannet import RanNet, RanNetWordPieceTokenizer vocab_path =
+`return_sequences=False` to extract semantic feature. ```python import numpy as
+np from rannet import RanNet, RanNetWordPieceTokenizer vocab_path =
 'pretrained/vocab.txt' ckpt_path = 'pretrained/model.ckpt' config_path =
 'pretrained/config.json' tokenizer = RanNetWordPieceTokenizer(vocab_path,
 lowercase=True) rannet, rannet_model = RanNet.load_rannet
 ( config_path=config_path, checkpoint_path=ckpt_path, return_sequences=False,
-apply_cell_transform=False ) text = 'input text' tok = tokenizer.encode(text)
-vec = rannet_model.predict(np.array([tok.ids])) ``` *For the classification
-task* ```python from rannet import RanNet, RanNetWordPieceTokenizer vocab_path
-= 'pretrained/vocab.txt' ckpt_path = 'pretrained/model.ckpt' config_path =
-'pretrained/config.json' tokenizer = RanNetWordPieceTokenizer(vocab_path,
-lowercase=True) rannet, rannet_model = RanNet.load_rannet
-( config_path=config_path, checkpoint_path=ckpt_path, return_sequences=False)
-output = rannet_model.output # (B, D) output = L.Dropout(0.1)(output) output =
-L.Dense(2, activation='softmax')(output) model = keras.models.Model
-(rannet_model.input, output) model.summary() ``` *For the sequence task*
-```python from rannet import RanNet, RanNetWordPieceTokenizer vocab_path =
-'pretrained/vocab.txt' ckpt_path = 'pretrained/model.ckpt' config_path =
-'pretrained/config.json' tokenizer = RanNetWordPieceTokenizer(vocab_path,
-lowercase=True) rannet, rannet_model = RanNet.load_rannet
-( config_path=config_path, checkpoint_path=ckpt_path, return_gpc=False) output
+apply_cell_transform=False, cell_pooling='mean' ) text = 'input text' tok =
+tokenizer.encode(text) vec = rannet_model.predict(np.array([tok.ids])) ``` *For
+the classification task* ```python from rannet import RanNet,
+RanNetWordPieceTokenizer vocab_path = 'pretrained/vocab.txt' ckpt_path =
+'pretrained/model.ckpt' config_path = 'pretrained/config.json' tokenizer =
+RanNetWordPieceTokenizer(vocab_path, lowercase=True) rannet, rannet_model =
+RanNet.load_rannet( config_path=config_path, checkpoint_path=ckpt_path,
+return_sequences=False) output = rannet_model.output # (B, D) output =
+L.Dropout(0.1)(output) output = L.Dense(2, activation='softmax')(output) model
+= keras.models.Model(rannet_model.input, output) model.summary() ``` *For the
+sequence task* ```python from rannet import RanNet, RanNetWordPieceTokenizer
+vocab_path = 'pretrained/vocab.txt' ckpt_path = 'pretrained/model.ckpt'
+config_path = 'pretrained/config.json' tokenizer = RanNetWordPieceTokenizer
+(vocab_path, lowercase=True) rannet, rannet_model = RanNet.load_rannet
+( config_path=config_path, checkpoint_path=ckpt_path, return_cell=False) output
 = rannet_model.output # (B, L, D) rannet_model.summary() ``` ## ð w/
 o pretrained models Embed the `RAN` (a Keras layer) into your network.
 ```python from rannet import RAN ran = RAN(head_num=8, head_size=256,
 window_size=256, min_window_size=16, activation='swish',
 kernel_initializer='glorot_normal', apply_lm_mask=False,
 apply_seq2seq_mask=False, apply_memory_review=True, dropout_rate=0.0,
 cell_initializer_type='zero') output, cell = ran(X) ``` # ð Citation If you
```

### Comparing `rannet-0.2.0/README.md` & `rannet-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 # 🚀 Quick Tour
 
 ## 🈶 w/ pretrained models
 
 *Extract semantic feature*
 
-set `apply_cell_transform=False` to extract semantic feature.
+set `return_sequences=False` to extract semantic feature.
 
 ```python
 import numpy as np
 from rannet import RanNet, RanNetWordPieceTokenizer
 
 
 vocab_path = 'pretrained/vocab.txt'
@@ -66,15 +66,16 @@
 config_path = 'pretrained/config.json'
 tokenizer = RanNetWordPieceTokenizer(vocab_path, lowercase=True)
 
 rannet, rannet_model = RanNet.load_rannet(
     config_path=config_path,
     checkpoint_path=ckpt_path,
     return_sequences=False,
-    apply_cell_transform=False
+    apply_cell_transform=False,
+    cell_pooling='mean'
 )
 text = 'input text'
 tok = tokenizer.encode(text)
 vec = rannet_model.predict(np.array([tok.ids]))
 ```
 
 *For the classification task*
@@ -105,15 +106,15 @@
 
 vocab_path = 'pretrained/vocab.txt'
 ckpt_path = 'pretrained/model.ckpt'
 config_path = 'pretrained/config.json'
 tokenizer = RanNetWordPieceTokenizer(vocab_path, lowercase=True)
 
 rannet, rannet_model = RanNet.load_rannet(
-    config_path=config_path, checkpoint_path=ckpt_path, return_gpc=False)
+    config_path=config_path, checkpoint_path=ckpt_path, return_cell=False)
 output = rannet_model.output  # (B, L, D)
 rannet_model.summary()
 ```
 
 ## 🈚 w/o pretrained models
 
 Embed the `RAN` (a Keras layer) into your network.
```

#### html2text {}

```diff
@@ -12,35 +12,35 @@
 view?usp=sharing) | [base](https://pan.baidu.com/s/18uhAkY46aIcy4ncwzXp5mA)\
 [code: djkj\] | | CN | [base](https://drive.google.com/file/d/1_gmrulSU-
 ln_jElc2hktPTTQDzaeG1wU/view?usp=sharing) \| [small](https://drive.google.com/
 file/d/1D-FCxY_UMwZCkvcwl6hkRcl6VnCzRGIj/view?usp=sharing) | [base](https://
 pan.baidu.com/s/1WIcePgmqb7Ox0w1qigWQ_w)\[code: e47w\] \| [small](https://
 pan.baidu.com/s/17DAboL9w0mArcBBuiy3tGg)\[code: mdmg\] | # ð Quick Tour ##
 ð¶ w/ pretrained models *Extract semantic feature* set
-`apply_cell_transform=False` to extract semantic feature. ```python import
-numpy as np from rannet import RanNet, RanNetWordPieceTokenizer vocab_path =
+`return_sequences=False` to extract semantic feature. ```python import numpy as
+np from rannet import RanNet, RanNetWordPieceTokenizer vocab_path =
 'pretrained/vocab.txt' ckpt_path = 'pretrained/model.ckpt' config_path =
 'pretrained/config.json' tokenizer = RanNetWordPieceTokenizer(vocab_path,
 lowercase=True) rannet, rannet_model = RanNet.load_rannet
 ( config_path=config_path, checkpoint_path=ckpt_path, return_sequences=False,
-apply_cell_transform=False ) text = 'input text' tok = tokenizer.encode(text)
-vec = rannet_model.predict(np.array([tok.ids])) ``` *For the classification
-task* ```python from rannet import RanNet, RanNetWordPieceTokenizer vocab_path
-= 'pretrained/vocab.txt' ckpt_path = 'pretrained/model.ckpt' config_path =
-'pretrained/config.json' tokenizer = RanNetWordPieceTokenizer(vocab_path,
-lowercase=True) rannet, rannet_model = RanNet.load_rannet
-( config_path=config_path, checkpoint_path=ckpt_path, return_sequences=False)
-output = rannet_model.output # (B, D) output = L.Dropout(0.1)(output) output =
-L.Dense(2, activation='softmax')(output) model = keras.models.Model
-(rannet_model.input, output) model.summary() ``` *For the sequence task*
-```python from rannet import RanNet, RanNetWordPieceTokenizer vocab_path =
-'pretrained/vocab.txt' ckpt_path = 'pretrained/model.ckpt' config_path =
-'pretrained/config.json' tokenizer = RanNetWordPieceTokenizer(vocab_path,
-lowercase=True) rannet, rannet_model = RanNet.load_rannet
-( config_path=config_path, checkpoint_path=ckpt_path, return_gpc=False) output
+apply_cell_transform=False, cell_pooling='mean' ) text = 'input text' tok =
+tokenizer.encode(text) vec = rannet_model.predict(np.array([tok.ids])) ``` *For
+the classification task* ```python from rannet import RanNet,
+RanNetWordPieceTokenizer vocab_path = 'pretrained/vocab.txt' ckpt_path =
+'pretrained/model.ckpt' config_path = 'pretrained/config.json' tokenizer =
+RanNetWordPieceTokenizer(vocab_path, lowercase=True) rannet, rannet_model =
+RanNet.load_rannet( config_path=config_path, checkpoint_path=ckpt_path,
+return_sequences=False) output = rannet_model.output # (B, D) output =
+L.Dropout(0.1)(output) output = L.Dense(2, activation='softmax')(output) model
+= keras.models.Model(rannet_model.input, output) model.summary() ``` *For the
+sequence task* ```python from rannet import RanNet, RanNetWordPieceTokenizer
+vocab_path = 'pretrained/vocab.txt' ckpt_path = 'pretrained/model.ckpt'
+config_path = 'pretrained/config.json' tokenizer = RanNetWordPieceTokenizer
+(vocab_path, lowercase=True) rannet, rannet_model = RanNet.load_rannet
+( config_path=config_path, checkpoint_path=ckpt_path, return_cell=False) output
 = rannet_model.output # (B, L, D) rannet_model.summary() ``` ## ð w/
 o pretrained models Embed the `RAN` (a Keras layer) into your network.
 ```python from rannet import RAN ran = RAN(head_num=8, head_size=256,
 window_size=256, min_window_size=16, activation='swish',
 kernel_initializer='glorot_normal', apply_lm_mask=False,
 apply_seq2seq_mask=False, apply_memory_review=True, dropout_rate=0.0,
 cell_initializer_type='zero') output, cell = ran(X) ``` # ð Citation If you
```

### Comparing `rannet-0.2.0/rannet/dataloader.py` & `rannet-0.2.1/rannet/dataloader.py`

 * *Files identical despite different names*

### Comparing `rannet-0.2.0/rannet/layers.py` & `rannet-0.2.1/rannet/layers.py`

 * *Files identical despite different names*

### Comparing `rannet-0.2.0/rannet/optimizer.py` & `rannet-0.2.1/rannet/optimizer.py`

 * *Files identical despite different names*

### Comparing `rannet-0.2.0/rannet/pretrain.py` & `rannet-0.2.1/rannet/pretrain.py`

 * *Files identical despite different names*

### Comparing `rannet-0.2.0/rannet/ran.py` & `rannet-0.2.1/rannet/ran.py`

 * *Files identical despite different names*

### Comparing `rannet-0.2.0/rannet/rannet.py` & `rannet-0.2.1/rannet/rannet.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,29 +50,29 @@
         return ','.join([f'{k}={v}' for k, v in self.__dict__.items()])
 
 
 class RanNet:
     def __init__(self,
                  params: RanNetParams,
                  return_sequences: bool = True,
-                 return_gpc: bool = True,
+                 return_cell: bool = True,
                  return_history: bool = True,
                  mlm_softmax: bool = False,
                  apply_cell_transform: bool = True,
                  apply_lm_mask: bool = False,
                  apply_seq2seq_mask: bool = False,
                  apply_memory_review: bool = True,
                  cell_initializer_type: str = 'zero',
                  cell_pooling: str = 'last',
                  min_window_size: Optional[int] = None,
                  window_size: Optional[int] = None,
                  prefix: str = ''):
         self.params = params
         self.return_sequences = return_sequences
-        self.return_gpc = return_gpc
+        self.return_cell = return_cell
         self.return_history = return_history
         self.apply_cell_transform = apply_cell_transform
         self.cell_initializer_type = cell_initializer_type
         self.cell_pooling = cell_pooling
         self.min_window_size = min_window_size
         self.window_size = window_size
         self.prefix = prefix
@@ -143,15 +143,15 @@
         return name
 
     def get_inputs(self, with_cell: bool = False, with_segment: bool = False):
         x_in = L.Input(name=self.get_weight_name('Input-Token'), shape=(None, ))
         x = x_in
         self.inputs = [x_in]
         if with_cell:
-            cell_in = L.Input(name=self.get_weight_name('Input-GPC'), shape=(self.params.embedding_size, ))
+            cell_in = L.Input(name=self.get_weight_name('Input-Cell'), shape=(self.params.embedding_size, ))
             self.inputs.append(cell_in)
             cell = cell_in
         else:
             cell = None
         if with_segment:
             segment_in = L.Input(name=self.get_weight_name('Input-Segment'), shape=(None, ))
             self.inputs.append(segment_in)
@@ -168,15 +168,15 @@
         x = self.embedding_layernorm(x)
         x = self.embedding_dropout(x)
 
         outputs = x
         for kernel in self.rans:
             outputs, cell = kernel([outputs, x_mask], cell=cell, segments=segments)
 
-        if self.return_gpc and self.apply_cell_transform:
+        if self.return_cell and self.apply_cell_transform:
             cell = L.Lambda(lambda x: K.expand_dims(x, axis=1))(cell)
             cell = L.Dense(self.params.embedding_size,
                            kernel_initializer=self.initializer,
                            activation='swish',
                            name='Output-Cell-Dense')(cell)
             cell = L.Dropout(self.params.dropout_rate)(cell)
             cell = GatedLinearUnit(
@@ -187,15 +187,15 @@
             max_pooling = L.Dense(self.params.embedding_size,
                                   kernel_initializer=self.initializer,
                                   name='Output-Pooling-Dense')(max_pooling)
             # ct = p + g(c), use maxpooling to enhance semantic feature
             cell = L.Lambda(lambda x: x[0] + x[1], name='Output-Cell-Fuse')([cell, max_pooling])
             cell = L.Lambda(lambda x: K.squeeze(x, axis=1), name='Output-Cell-Squeeze')(cell)
         if self.return_sequences:
-            if self.return_gpc:
+            if self.return_cell:
                 return [outputs, cell]
             return outputs
         return cell
 
     def __call__(self,
                  with_cell: bool = False,
                  with_mlm: bool = False,
@@ -227,15 +227,15 @@
         outputs = self.encode(x, x_mask, cell, segments=segments)
 
         if not with_mlm:
             if return_model:
                 return keras.Model(self.inputs, outputs)
             return outputs
 
-        output = outputs[0] if self.return_gpc else outputs
+        output = outputs[0] if self.return_cell else outputs
         mlm = self.mlm_hidden(output)
         mlm = self.mlm_matching([mlm, embedding_weights])
 
         if return_model:
             return keras.Model(self.inputs, mlm)
         return mlm
 
@@ -438,19 +438,19 @@
             **kwargs
         )
 
 
 class RanNetForLM(RanNet):
     def __init__(self,
                  params: RanNetParams,
-                 return_gpc: bool = False,
+                 return_cell: bool = False,
                  prefix: str = ''):
         super().__init__(params,
                          return_sequences=True,
-                         return_gpc=return_gpc,
+                         return_cell=return_cell,
                          apply_cell_transform=False,
                          mlm_softmax=True,
                          apply_lm_mask=True,
                          apply_seq2seq_mask=False,
                          prefix=prefix)
 
     def __call__(self, with_cell: bool = False, return_model: bool = True) -> Union[Models, Tensors]:
@@ -459,19 +459,19 @@
 
 class RanNetForAdaptiveLM(RanNet):
     def __init__(self,
                  params: RanNetParams,
                  cutoffs: List[int],
                  div_val: int = 1,
                  output_dropout_rate: float = 0.0,
-                 return_gpc: bool = False,
+                 return_cell: bool = False,
                  prefix: str = ''):
         super().__init__(params,
                          return_sequences=True,
-                         return_gpc=return_gpc,
+                         return_cell=return_cell,
                          mlm_softmax=False,
                          apply_cell_transform=False,
                          apply_lm_mask=True,
                          apply_seq2seq_mask=False,
                          prefix=prefix)
         dropout_rate = output_dropout_rate or self.params.dropout_rate
         self.output_dropout = L.Dropout(dropout_rate, name='Output-Dropout')
@@ -524,29 +524,29 @@
 
 class RanNetForSeq2Seq(RanNet):
     def __init__(self,
                  params: RanNetParams,
                  prefix: str = ''):
         super().__init__(params,
                          return_sequences=True,
-                         return_gpc=False,
+                         return_cell=False,
                          mlm_softmax=True,
                          apply_cell_transform=False,
                          apply_lm_mask=False,
                          apply_seq2seq_mask=True,
                          prefix=prefix)
 
     def __call__(self, with_cell: bool = False, return_model: bool = True) -> Union[Models, Tensors]:
         return super().__call__(with_cell=with_cell, with_mlm=True, return_model=return_model, seq2seq=True)
 
 
 class RanNetForMLMPretrain(RanNet):
     def __init__(self, params: RanNetParams, **kwargs):
         super().__init__(params,
-                         return_gpc=False,
+                         return_cell=False,
                          return_sequences=True,
                          apply_cell_transform=False,
                          **kwargs)
 
     def __call__(self) -> Tuple[Models, Models, Dict]:
         mlm_output = super().__call__(with_mlm=True, return_model=False)
         token_ids_in = L.Input(name=self.get_weight_name('token_ids'),
```

### Comparing `rannet-0.2.0/rannet/tokenizer.py` & `rannet-0.2.1/rannet/tokenizer.py`

 * *Files identical despite different names*

### Comparing `rannet-0.2.0/rannet/utils.py` & `rannet-0.2.1/rannet/utils.py`

 * *Files identical despite different names*

### Comparing `rannet-0.2.0/rannet.egg-info/PKG-INFO` & `rannet-0.2.1/rannet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rannet
-Version: 0.2.0
+Version: 0.2.1
 Summary: Recurrent Attention Networks
 Author: sean lee
 Author-email: xmlee97@gmail.com
 Keywords: rannet
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -70,15 +70,15 @@
 
 # 🚀 Quick Tour
 
 ## 🈶 w/ pretrained models
 
 *Extract semantic feature*
 
-set `apply_cell_transform=False` to extract semantic feature.
+set `return_sequences=False` to extract semantic feature.
 
 ```python
 import numpy as np
 from rannet import RanNet, RanNetWordPieceTokenizer
 
 
 vocab_path = 'pretrained/vocab.txt'
@@ -86,15 +86,16 @@
 config_path = 'pretrained/config.json'
 tokenizer = RanNetWordPieceTokenizer(vocab_path, lowercase=True)
 
 rannet, rannet_model = RanNet.load_rannet(
     config_path=config_path,
     checkpoint_path=ckpt_path,
     return_sequences=False,
-    apply_cell_transform=False
+    apply_cell_transform=False,
+    cell_pooling='mean'
 )
 text = 'input text'
 tok = tokenizer.encode(text)
 vec = rannet_model.predict(np.array([tok.ids]))
 ```
 
 *For the classification task*
@@ -125,15 +126,15 @@
 
 vocab_path = 'pretrained/vocab.txt'
 ckpt_path = 'pretrained/model.ckpt'
 config_path = 'pretrained/config.json'
 tokenizer = RanNetWordPieceTokenizer(vocab_path, lowercase=True)
 
 rannet, rannet_model = RanNet.load_rannet(
-    config_path=config_path, checkpoint_path=ckpt_path, return_gpc=False)
+    config_path=config_path, checkpoint_path=ckpt_path, return_cell=False)
 output = rannet_model.output  # (B, L, D)
 rannet_model.summary()
 ```
 
 ## 🈚 w/o pretrained models
 
 Embed the `RAN` (a Keras layer) into your network.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rannet Version: 0.2.0 Summary: Recurrent Attention
+Metadata-Version: 2.1 Name: rannet Version: 0.2.1 Summary: Recurrent Attention
 Networks Author: sean lee Author-email: xmlee97@gmail.com Keywords: rannet
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
@@ -22,35 +22,35 @@
 view?usp=sharing) | [base](https://pan.baidu.com/s/18uhAkY46aIcy4ncwzXp5mA)\
 [code: djkj\] | | CN | [base](https://drive.google.com/file/d/1_gmrulSU-
 ln_jElc2hktPTTQDzaeG1wU/view?usp=sharing) \| [small](https://drive.google.com/
 file/d/1D-FCxY_UMwZCkvcwl6hkRcl6VnCzRGIj/view?usp=sharing) | [base](https://
 pan.baidu.com/s/1WIcePgmqb7Ox0w1qigWQ_w)\[code: e47w\] \| [small](https://
 pan.baidu.com/s/17DAboL9w0mArcBBuiy3tGg)\[code: mdmg\] | # ð Quick Tour ##
 ð¶ w/ pretrained models *Extract semantic feature* set
-`apply_cell_transform=False` to extract semantic feature. ```python import
-numpy as np from rannet import RanNet, RanNetWordPieceTokenizer vocab_path =
+`return_sequences=False` to extract semantic feature. ```python import numpy as
+np from rannet import RanNet, RanNetWordPieceTokenizer vocab_path =
 'pretrained/vocab.txt' ckpt_path = 'pretrained/model.ckpt' config_path =
 'pretrained/config.json' tokenizer = RanNetWordPieceTokenizer(vocab_path,
 lowercase=True) rannet, rannet_model = RanNet.load_rannet
 ( config_path=config_path, checkpoint_path=ckpt_path, return_sequences=False,
-apply_cell_transform=False ) text = 'input text' tok = tokenizer.encode(text)
-vec = rannet_model.predict(np.array([tok.ids])) ``` *For the classification
-task* ```python from rannet import RanNet, RanNetWordPieceTokenizer vocab_path
-= 'pretrained/vocab.txt' ckpt_path = 'pretrained/model.ckpt' config_path =
-'pretrained/config.json' tokenizer = RanNetWordPieceTokenizer(vocab_path,
-lowercase=True) rannet, rannet_model = RanNet.load_rannet
-( config_path=config_path, checkpoint_path=ckpt_path, return_sequences=False)
-output = rannet_model.output # (B, D) output = L.Dropout(0.1)(output) output =
-L.Dense(2, activation='softmax')(output) model = keras.models.Model
-(rannet_model.input, output) model.summary() ``` *For the sequence task*
-```python from rannet import RanNet, RanNetWordPieceTokenizer vocab_path =
-'pretrained/vocab.txt' ckpt_path = 'pretrained/model.ckpt' config_path =
-'pretrained/config.json' tokenizer = RanNetWordPieceTokenizer(vocab_path,
-lowercase=True) rannet, rannet_model = RanNet.load_rannet
-( config_path=config_path, checkpoint_path=ckpt_path, return_gpc=False) output
+apply_cell_transform=False, cell_pooling='mean' ) text = 'input text' tok =
+tokenizer.encode(text) vec = rannet_model.predict(np.array([tok.ids])) ``` *For
+the classification task* ```python from rannet import RanNet,
+RanNetWordPieceTokenizer vocab_path = 'pretrained/vocab.txt' ckpt_path =
+'pretrained/model.ckpt' config_path = 'pretrained/config.json' tokenizer =
+RanNetWordPieceTokenizer(vocab_path, lowercase=True) rannet, rannet_model =
+RanNet.load_rannet( config_path=config_path, checkpoint_path=ckpt_path,
+return_sequences=False) output = rannet_model.output # (B, D) output =
+L.Dropout(0.1)(output) output = L.Dense(2, activation='softmax')(output) model
+= keras.models.Model(rannet_model.input, output) model.summary() ``` *For the
+sequence task* ```python from rannet import RanNet, RanNetWordPieceTokenizer
+vocab_path = 'pretrained/vocab.txt' ckpt_path = 'pretrained/model.ckpt'
+config_path = 'pretrained/config.json' tokenizer = RanNetWordPieceTokenizer
+(vocab_path, lowercase=True) rannet, rannet_model = RanNet.load_rannet
+( config_path=config_path, checkpoint_path=ckpt_path, return_cell=False) output
 = rannet_model.output # (B, L, D) rannet_model.summary() ``` ## ð w/
 o pretrained models Embed the `RAN` (a Keras layer) into your network.
 ```python from rannet import RAN ran = RAN(head_num=8, head_size=256,
 window_size=256, min_window_size=16, activation='swish',
 kernel_initializer='glorot_normal', apply_lm_mask=False,
 apply_seq2seq_mask=False, apply_memory_review=True, dropout_rate=0.0,
 cell_initializer_type='zero') output, cell = ran(X) ``` # ð Citation If you
```

### Comparing `rannet-0.2.0/setup.py` & `rannet-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     requirements = [l for l in f.read().splitlines() if l]
 
 with open('dev-requirements.txt', encoding='utf-8') as f:
     test_requirements = [l for l in f.read().splitlines() if l][1:]
 
 setup(
     name='rannet',
-    version='0.2.0',
+    version='0.2.1',
     description='Recurrent Attention Networks',
     long_description=readme,
     long_description_content_type="text/markdown",
     author='sean lee',
     author_email='xmlee97@gmail.com',
     packages=find_packages(exclude=("tests", "tests.*", "examples", "examples.*")),
     install_requires=requirements,
```

