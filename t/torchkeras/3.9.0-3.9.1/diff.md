# Comparing `tmp/torchkeras-3.9.0.tar.gz` & `tmp/torchkeras-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/torchkeras-3.9.0.tar", last modified: Fri Jun 30 07:06:46 2023, max compression
+gzip compressed data, was "dist/torchkeras-3.9.1.tar", last modified: Sat Jul  8 13:05:37 2023, max compression
```

## Comparing `torchkeras-3.9.0.tar` & `torchkeras-3.9.1.tar`

### file list

```diff
@@ -1,38 +1,42 @@
-drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-06-30 07:06:46.888952 torchkeras-3.9.0/
--rw-r--r--   0 liangyun2   (502) staff       (20)    11325 2023-02-09 16:00:16.000000 torchkeras-3.9.0/LICENSE
--rw-r--r--   0 liangyun2   (502) staff       (20)      357 2023-02-09 16:55:42.000000 torchkeras-3.9.0/MANIFEST.in
--rw-r--r--   0 liangyun2   (502) staff       (20)     6252 2023-06-30 07:06:46.888637 torchkeras-3.9.0/PKG-INFO
--rw-r--r--   0 liangyun2   (502) staff       (20)    12396 2023-06-25 16:00:42.000000 torchkeras-3.9.0/README.md
--rw-r--r--   0 liangyun2   (502) staff       (20)       38 2023-06-30 07:06:46.889024 torchkeras-3.9.0/setup.cfg
--rw-r--r--   0 liangyun2   (502) staff       (20)     1273 2023-06-30 07:06:01.000000 torchkeras-3.9.0/setup.py
-drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-06-30 07:06:46.865748 torchkeras-3.9.0/torchkeras/
--rw-r--r--   0 liangyun2   (502) staff       (20)      246 2023-06-30 07:05:32.000000 torchkeras-3.9.0/torchkeras/__init__.py
-drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-06-30 07:06:46.883980 torchkeras-3.9.0/torchkeras/assets/
--rw-r--r--   0 liangyun2   (502) staff       (20) 10043912 2023-02-09 16:00:16.000000 torchkeras-3.9.0/torchkeras/assets/SimHei.ttf
--rw-r--r--   0 liangyun2   (502) staff       (20)  1012077 2023-02-09 16:00:16.000000 torchkeras-3.9.0/torchkeras/assets/park.jpg
--rw-r--r--   0 liangyun2   (502) staff       (20)   168949 2023-02-09 16:00:16.000000 torchkeras-3.9.0/torchkeras/assets/zidane.jpg
-drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-06-30 07:06:46.885511 torchkeras-3.9.0/torchkeras/chatgpt/
--rw-r--r--   0 liangyun2   (502) staff       (20)     4178 2023-05-14 01:50:00.000000 torchkeras-3.9.0/torchkeras/chatgpt/__init__.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     8621 2023-06-30 01:34:56.000000 torchkeras-3.9.0/torchkeras/data.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     5222 2023-04-13 09:25:41.000000 torchkeras-3.9.0/torchkeras/eda.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     1628 2023-04-13 07:46:39.000000 torchkeras-3.9.0/torchkeras/email.py
--rw-r--r--   0 liangyun2   (502) staff       (20)    11531 2023-06-25 03:42:54.000000 torchkeras-3.9.0/torchkeras/hugmodel.py
--rw-r--r--   0 liangyun2   (502) staff       (20)    10903 2023-06-29 23:05:25.000000 torchkeras-3.9.0/torchkeras/kerascallbacks.py
--rw-r--r--   0 liangyun2   (502) staff       (20)    13855 2023-06-30 07:03:22.000000 torchkeras-3.9.0/torchkeras/kerasmodel.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     7316 2023-02-22 02:34:47.000000 torchkeras-3.9.0/torchkeras/metrics.py
-drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-06-30 07:06:46.888235 torchkeras-3.9.0/torchkeras/models/
--rw-r--r--   0 liangyun2   (502) staff       (20)       75 2023-03-10 08:21:36.000000 torchkeras-3.9.0/torchkeras/models/__init__.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     4088 2023-02-24 04:01:48.000000 torchkeras-3.9.0/torchkeras/models/resnet.py
--rw-r--r--   0 liangyun2   (502) staff       (20)    31333 2023-05-20 15:18:08.000000 torchkeras-3.9.0/torchkeras/models/ssd.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     3374 2023-02-21 12:33:54.000000 torchkeras-3.9.0/torchkeras/models/unet.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     5444 2023-06-04 08:48:25.000000 torchkeras-3.9.0/torchkeras/pbar.py
--rw-r--r--   0 liangyun2   (502) staff       (20)    10676 2023-06-10 15:29:22.000000 torchkeras-3.9.0/torchkeras/plots.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     5737 2023-05-12 10:11:52.000000 torchkeras-3.9.0/torchkeras/soup.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     5256 2023-05-28 13:14:40.000000 torchkeras-3.9.0/torchkeras/summary.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     3843 2023-06-12 11:38:27.000000 torchkeras-3.9.0/torchkeras/utils.py
-drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-06-30 07:06:46.868796 torchkeras-3.9.0/torchkeras.egg-info/
--rw-r--r--   0 liangyun2   (502) staff       (20)     6252 2023-06-30 07:06:46.000000 torchkeras-3.9.0/torchkeras.egg-info/PKG-INFO
--rw-r--r--   0 liangyun2   (502) staff       (20)      711 2023-06-30 07:06:46.000000 torchkeras-3.9.0/torchkeras.egg-info/SOURCES.txt
--rw-r--r--   0 liangyun2   (502) staff       (20)        1 2023-06-30 07:06:46.000000 torchkeras-3.9.0/torchkeras.egg-info/dependency_links.txt
--rw-r--r--   0 liangyun2   (502) staff       (20)       16 2023-06-30 07:06:46.000000 torchkeras-3.9.0/torchkeras.egg-info/requires.txt
--rw-r--r--   0 liangyun2   (502) staff       (20)       26 2023-06-30 07:06:46.000000 torchkeras-3.9.0/torchkeras.egg-info/top_level.txt
+drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-07-08 13:05:37.117984 torchkeras-3.9.1/
+-rw-r--r--   0 liangyun2   (502) staff       (20)    11325 2023-02-09 16:00:16.000000 torchkeras-3.9.1/LICENSE
+-rw-r--r--   0 liangyun2   (502) staff       (20)      357 2023-02-09 16:55:42.000000 torchkeras-3.9.1/MANIFEST.in
+-rw-r--r--   0 liangyun2   (502) staff       (20)     6646 2023-07-08 13:05:37.117369 torchkeras-3.9.1/PKG-INFO
+-rw-r--r--   0 liangyun2   (502) staff       (20)    12671 2023-07-08 12:32:31.000000 torchkeras-3.9.1/README.md
+-rw-r--r--   0 liangyun2   (502) staff       (20)       38 2023-07-08 13:05:37.118093 torchkeras-3.9.1/setup.cfg
+-rw-r--r--   0 liangyun2   (502) staff       (20)     1273 2023-06-30 07:06:01.000000 torchkeras-3.9.1/setup.py
+drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-07-08 13:05:37.083495 torchkeras-3.9.1/torchkeras/
+-rw-r--r--   0 liangyun2   (502) staff       (20)      246 2023-07-06 21:29:51.000000 torchkeras-3.9.1/torchkeras/__init__.py
+drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-07-08 13:05:37.110683 torchkeras-3.9.1/torchkeras/assets/
+-rw-r--r--   0 liangyun2   (502) staff       (20) 10043912 2023-02-09 16:00:16.000000 torchkeras-3.9.1/torchkeras/assets/SimHei.ttf
+-rw-r--r--   0 liangyun2   (502) staff       (20)  1012077 2023-02-09 16:00:16.000000 torchkeras-3.9.1/torchkeras/assets/park.jpg
+-rw-r--r--   0 liangyun2   (502) staff       (20)   168949 2023-02-09 16:00:16.000000 torchkeras-3.9.1/torchkeras/assets/zidane.jpg
+drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-07-08 13:05:37.113214 torchkeras-3.9.1/torchkeras/chat/
+-rw-r--r--   0 liangyun2   (502) staff       (20)       57 2023-07-06 21:05:16.000000 torchkeras-3.9.1/torchkeras/chat/__init__.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     2089 2023-07-08 12:15:46.000000 torchkeras-3.9.1/torchkeras/chat/chatglm.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     4178 2023-05-14 01:50:00.000000 torchkeras-3.9.1/torchkeras/chat/chatgpt.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     8621 2023-06-30 01:34:56.000000 torchkeras-3.9.1/torchkeras/data.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     5222 2023-04-13 09:25:41.000000 torchkeras-3.9.1/torchkeras/eda.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     1628 2023-04-13 07:46:39.000000 torchkeras-3.9.1/torchkeras/email.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)    11531 2023-06-25 03:42:54.000000 torchkeras-3.9.1/torchkeras/hugmodel.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)    10939 2023-07-06 21:26:00.000000 torchkeras-3.9.1/torchkeras/kerascallbacks.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)    13883 2023-07-06 21:28:09.000000 torchkeras-3.9.1/torchkeras/kerasmodel.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     7316 2023-02-22 02:34:47.000000 torchkeras-3.9.1/torchkeras/metrics.py
+drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-07-08 13:05:37.116401 torchkeras-3.9.1/torchkeras/models/
+-rw-r--r--   0 liangyun2   (502) staff       (20)       75 2023-03-10 08:21:36.000000 torchkeras-3.9.1/torchkeras/models/__init__.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     4088 2023-02-24 04:01:48.000000 torchkeras-3.9.1/torchkeras/models/resnet.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)    31333 2023-05-20 15:18:08.000000 torchkeras-3.9.1/torchkeras/models/ssd.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     3374 2023-02-21 12:33:54.000000 torchkeras-3.9.1/torchkeras/models/unet.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     5444 2023-06-04 08:48:25.000000 torchkeras-3.9.1/torchkeras/pbar.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)    10676 2023-06-10 15:29:22.000000 torchkeras-3.9.1/torchkeras/plots.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     5737 2023-05-12 10:11:52.000000 torchkeras-3.9.1/torchkeras/soup.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     5256 2023-05-28 13:14:40.000000 torchkeras-3.9.1/torchkeras/summary.py
+drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-07-08 13:05:37.116968 torchkeras-3.9.1/torchkeras/tools/
+-rw-r--r--   0 liangyun2   (502) staff       (20)     3740 2023-07-06 21:11:38.000000 torchkeras-3.9.1/torchkeras/tools/catboost.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     3843 2023-06-12 11:38:27.000000 torchkeras-3.9.1/torchkeras/utils.py
+drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-07-08 13:05:37.090039 torchkeras-3.9.1/torchkeras.egg-info/
+-rw-r--r--   0 liangyun2   (502) staff       (20)     6646 2023-07-08 13:05:36.000000 torchkeras-3.9.1/torchkeras.egg-info/PKG-INFO
+-rw-r--r--   0 liangyun2   (502) staff       (20)      791 2023-07-08 13:05:37.000000 torchkeras-3.9.1/torchkeras.egg-info/SOURCES.txt
+-rw-r--r--   0 liangyun2   (502) staff       (20)        1 2023-07-08 13:05:36.000000 torchkeras-3.9.1/torchkeras.egg-info/dependency_links.txt
+-rw-r--r--   0 liangyun2   (502) staff       (20)       16 2023-07-08 13:05:36.000000 torchkeras-3.9.1/torchkeras.egg-info/requires.txt
+-rw-r--r--   0 liangyun2   (502) staff       (20)       32 2023-07-08 13:05:36.000000 torchkeras-3.9.1/torchkeras.egg-info/top_level.txt
```

### Comparing `torchkeras-3.9.0/LICENSE` & `torchkeras-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `torchkeras-3.9.0/PKG-INFO` & `torchkeras-3.9.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchkeras
-Version: 3.9.0
+Version: 3.9.1
 Summary: pytorch❤️keras
 Home-page: https://github.com/lyhue1991/torchkeras
 Author: PythonAiRoad, Laugh
 Author-email: lyhue1991@163.com
 Keywords: machine-learning,deep-learning,ML,DL,pytorch,torch,keras
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -129,14 +129,17 @@
 |ReinforcementLearning——DQN|- |[DQN](./examples/DQN.ipynb)|
 |ObjectDetection——FasterRCNN| torchvision  |  [FasterRCNN](./examples/FasterRCNN——vision.ipynb) | 
 |ImageSegmentation——DeepLabV3++ | segmentation_models_pytorch |  [Deeplabv3++](./examples/Deeplabv3plus——smp.ipynb) |
 |InstanceSegmentation——MaskRCNN | detectron2 |  [MaskRCNN](./examples/MaskRCNN——detectron2.ipynb) |
 |ObjectDetection——YOLOv8 🔥🔥| ultralytics |  [YOLOv8](./examples/YOLOv8——ultralytics.ipynb) |
 |TextClassification——BERT 🔥🔥| transformers |  [BERT](./examples/BERT——transformers.ipynb) |
 |TokenClassification——BERT | transformers |  [BERT_NER](./examples/BERT_NER——transformers.ipynb) |
+|FinetuneLLM——ChatGLM2 🔥🔥🔥| transformers |  [ChatGLM2](./examples/ChatGLM2——transformers.ipynb) |
+|FinetuneLLM——ChatGLM2_LoRA 🔥🔥🔥| transformers,peft |  [ChatGLM2_LoRA](./examples/ChatGLM2_LoRA——transformers.ipynb) |
+|FinetuneLLM——ChatGLM2_AdaLoRA 🔥🔥🔥| transformers,peft |  [ChatGLM2_AdaLoRA](./examples/ChatGLM2_AdaLoRA——transformers.ipynb) |
 |ImageClassification——SwinTransformer|timm| [Swin](./examples/SwinTransformer——timm.ipynb)|
 
 **If you want to understand or modify some details of this project, feel free to read and change the source code!!!**
 
 Any other questions, you can contact the author form the wechat official account below:
 
 **算法美食屋**
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchkeras Version: 3.9.0 Summary:
+Metadata-Version: 2.1 Name: torchkeras Version: 3.9.1 Summary:
 pytorchâ¤ï¸keras Home-page: https://github.com/lyhue1991/torchkeras Author:
 PythonAiRoad, Laugh Author-email: lyhue1991@163.com Keywords: machine-
 learning,deep-learning,ML,DL,pytorch,torch,keras Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.5
 Description-Content-Type: text/markdown License-File: LICENSE #
 Pytorchâ¤ï¸Keras English | [ç®ä½ä¸­æ](README.md) The torchkeras library
@@ -67,14 +67,19 @@
 segmentation_models_pytorch | [Deeplabv3++](./examples/
 Deeplabv3plusââsmp.ipynb) | |InstanceSegmentationââMaskRCNN |
 detectron2 | [MaskRCNN](./examples/MaskRCNNââdetectron2.ipynb) |
 |ObjectDetectionââYOLOv8 ð¥ð¥| ultralytics | [YOLOv8](./examples/
 YOLOv8ââultralytics.ipynb) | |TextClassificationââBERT ð¥ð¥|
 transformers | [BERT](./examples/BERTââtransformers.ipynb) |
 |TokenClassificationââBERT | transformers | [BERT_NER](./examples/
-BERT_NERââtransformers.ipynb) |
+BERT_NERââtransformers.ipynb) | |FinetuneLLMââChatGLM2 ð¥ð¥ð¥|
+transformers | [ChatGLM2](./examples/ChatGLM2ââtransformers.ipynb) |
+|FinetuneLLMââChatGLM2_LoRA ð¥ð¥ð¥| transformers,peft |
+[ChatGLM2_LoRA](./examples/ChatGLM2_LoRAââtransformers.ipynb) |
+|FinetuneLLMââChatGLM2_AdaLoRA ð¥ð¥ð¥| transformers,peft |
+[ChatGLM2_AdaLoRA](./examples/ChatGLM2_AdaLoRAââtransformers.ipynb) |
 |ImageClassificationââSwinTransformer|timm| [Swin](./examples/
 SwinTransformerââtimm.ipynb)| **If you want to understand or modify some
 details of this project, feel free to read and change the source code!!!** Any
 other questions, you can contact the author form the wechat official account
 below: **ç®æ³ç¾é£å±** ![](https://tva1.sinaimg.cn/large/
 e6c9d24egy1h41m2zugguj20k00b9q46.jpg)
```

### Comparing `torchkeras-3.9.0/README.md` & `torchkeras-3.9.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -281,14 +281,16 @@
 |强化学习——DQN|- |[DQN](./examples/DQN.ipynb)|
 |目标检测——FasterRCNN| torchvision  |  [FasterRCNN](./examples/FasterRCNN——vision.ipynb) | 
 |语义分割——DeepLabV3++ 🔥| segmentation_models_pytorch |  [Deeplabv3++](./examples/Deeplabv3plus——smp.ipynb) |
 |实例分割——MaskRCNN 🔥🔥| detectron2 |  [MaskRCNN](./examples/MaskRCNN——detectron2.ipynb) |
 |目标检测——YOLOv8 🔥🔥| ultralytics |  [YOLOv8](./examples/YOLOv8——ultralytics.ipynb) |
 |文本分类——BERT 🔥| transformers |  [BERT](./examples/BERT——transformers.ipynb) |
 |命名实体识别——BERT | transformers |  [BERT_NER](./examples/BERT_NER——transformers.ipynb) |
+|LLM微调——ChatGLM2_LoRA 🔥🔥🔥| transformers,peft |  [ChatGLM2_LoRA](./examples/ChatGLM2_LoRA——transformers.ipynb) |
+|LLM微调——ChatGLM2_AdaLoRA 🔥🔥🔥| transformers,peft |  [ChatGLM2_AdaLoRA](./examples/ChatGLM2_AdaLoRA——transformers.ipynb) |
 |图片分类——SwinTransformer|timm| [Swin](./examples/SwinTransformer——timm.ipynb)|
 
 
 ```python
 
 ```
```

### Comparing `torchkeras-3.9.0/setup.py` & `torchkeras-3.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.9.0/torchkeras/assets/SimHei.ttf` & `torchkeras-3.9.1/torchkeras/assets/SimHei.ttf`

 * *Files identical despite different names*

### Comparing `torchkeras-3.9.0/torchkeras/assets/park.jpg` & `torchkeras-3.9.1/torchkeras/assets/park.jpg`

 * *Files identical despite different names*

### Comparing `torchkeras-3.9.0/torchkeras/assets/zidane.jpg` & `torchkeras-3.9.1/torchkeras/assets/zidane.jpg`

 * *Files identical despite different names*

### Comparing `torchkeras-3.9.0/torchkeras/chatgpt/__init__.py` & `torchkeras-3.9.1/torchkeras/chat/chatgpt.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.9.0/torchkeras/data.py` & `torchkeras-3.9.1/torchkeras/data.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.9.0/torchkeras/eda.py` & `torchkeras-3.9.1/torchkeras/eda.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.9.0/torchkeras/email.py` & `torchkeras-3.9.1/torchkeras/email.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.9.0/torchkeras/hugmodel.py` & `torchkeras-3.9.1/torchkeras/hugmodel.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.9.0/torchkeras/kerascallbacks.py` & `torchkeras-3.9.1/torchkeras/kerascallbacks.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,14 +147,15 @@
         self.progress.update(dfhistory['epoch'].iloc[-1])
 
            
     def on_fit_end(self,  model:"KerasModel"):
         dfhistory = pd.DataFrame(model.history)
         if dfhistory['epoch'].max()<model.epochs:
             self.progress.on_interrupt(msg='earlystopping')
+        self.progress.display=False
             
 class VisMetric:
     def __init__(self,figsize = (6,4)):
         self.figsize = (6,4)
         
     def on_fit_start(self,model: 'KerasModel'):
         self.metric =  model.monitor.replace('val_','')
```

### Comparing `torchkeras-3.9.0/torchkeras/kerasmodel.py` & `torchkeras-3.9.1/torchkeras/kerasmodel.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,29 +74,30 @@
         
         for step, batch in loop: 
             with self.accelerator.accumulate(self.net):
                 step_losses,step_metrics = self.steprunner(batch)   
                 step_log = dict(step_losses,**step_metrics)
                 for k,v in step_losses.items():
                     epoch_losses[k] = epoch_losses.get(k,0.0)+v
-
+                    
                 if step<n:
                     loop.set_postfix(**step_log)
-            
+                    
                     if hasattr(self,'progress') and self.accelerator.is_local_main_process:
                         post_log = dict(**{'i':step,'n':n},**step_log)
                         self.progress.set_postfix(**post_log)
 
                 elif step==n:
                     epoch_metrics = step_metrics
                     epoch_metrics.update({self.stage+"_"+name:metric_fn.compute().item() 
                                      for name,metric_fn in self.steprunner.metrics_dict.items()})
                     epoch_losses = {k:v/step for k,v in epoch_losses.items()}
                     epoch_log = dict(epoch_losses,**epoch_metrics)
                     loop.set_postfix(**epoch_log)
+            
                     
                     if hasattr(self,'progress') and self.accelerator.is_local_main_process:
                         post_log = dict(**{'i':step,'n':n},**epoch_log)
                         self.progress.set_postfix(**post_log)
                     
                     for name,metric_fn in self.steprunner.metrics_dict.items():
                         metric_fn.reset()  
@@ -112,27 +113,27 @@
         super().__init__()
         self.net,self.loss_fn,self.metrics_dict = net, loss_fn, torch.nn.ModuleDict(metrics_dict) 
         self.optimizer = optimizer if optimizer is not None else torch.optim.Adam(
             self.net.parameters(), lr=3e-4)
         self.lr_scheduler = lr_scheduler
         self.from_scratch = True
         
-    def save_ckpt(self, ckpt_path='checkpoint.pt', accelerator= None):
+    def save_ckpt(self, ckpt_path='checkpoint', accelerator= None):
         accelerator = accelerator if accelerator is not None else self.accelerator
         net_dict = accelerator.get_state_dict(self.net)
         accelerator.save(net_dict,ckpt_path)
       
-    def load_ckpt(self, ckpt_path='checkpoint.pt'):
+    def load_ckpt(self, ckpt_path='checkpoint'):
         self.net.load_state_dict(torch.load(ckpt_path,map_location='cpu'))
         self.from_scratch = False
 
     def forward(self, x):
         return self.net.forward(x)
     
-    def fit(self, train_data, val_data=None, epochs=10, ckpt_path='checkpoint.pt',
+    def fit(self, train_data, val_data=None, epochs=10, ckpt_path='checkpoint',
             patience=5, monitor="val_loss", mode="min", callbacks=None, 
             plot=True,  wandb=False, quiet=None, 
             mixed_precision='no', cpu=False, gradient_accumulation_steps=1):
         from torchkeras.utils import colorful,is_jupyter
         
         self.__dict__.update(locals())
         self.accelerator = Accelerator(mixed_precision=mixed_precision,cpu=cpu,
@@ -269,15 +270,15 @@
         with torch.no_grad():
             val_metrics = val_epoch_runner(val_data)
         if accelerator.is_local_main_process:
             torch.save(val_metrics,'val_metrics.pt')
         return val_metrics
     
     def fit_ddp(self,num_processes,train_data,
-            val_data=None, epochs=10, ckpt_path='checkpoint.pt',
+            val_data=None, epochs=10, ckpt_path='checkpoint',
             patience=5, monitor="val_loss", mode="min", callbacks=None, 
             plot=True, wandb=False, quiet=None, 
             mixed_precision='no', cpu=False, gradient_accumulation_steps=1
            ):
         from accelerate import notebook_launcher
         train_size = train_data.size if hasattr(train_data,'size') else len(train_data)
         train_data.size = train_size//num_processes
@@ -299,8 +300,8 @@
         from accelerate import notebook_launcher
         val_size = val_data.size if hasattr(val_data,'size') else len(val_data)
         val_data.size = val_size//num_processes
         args = (val_data,quiet)
         notebook_launcher(self.evaluate, args, num_processes=num_processes)
         val_metrics = torch.load('val_metrics.pt')
         val_data.size = val_size
-        return val_metrics
+        return val_metrics
```

### Comparing `torchkeras-3.9.0/torchkeras/metrics.py` & `torchkeras-3.9.1/torchkeras/metrics.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.9.0/torchkeras/models/resnet.py` & `torchkeras-3.9.1/torchkeras/models/resnet.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.9.0/torchkeras/models/ssd.py` & `torchkeras-3.9.1/torchkeras/models/ssd.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.9.0/torchkeras/models/unet.py` & `torchkeras-3.9.1/torchkeras/models/unet.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.9.0/torchkeras/pbar.py` & `torchkeras-3.9.1/torchkeras/pbar.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.9.0/torchkeras/plots.py` & `torchkeras-3.9.1/torchkeras/plots.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.9.0/torchkeras/soup.py` & `torchkeras-3.9.1/torchkeras/soup.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.9.0/torchkeras/summary.py` & `torchkeras-3.9.1/torchkeras/summary.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.9.0/torchkeras/utils.py` & `torchkeras-3.9.1/torchkeras/utils.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.9.0/torchkeras.egg-info/PKG-INFO` & `torchkeras-3.9.1/torchkeras.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchkeras
-Version: 3.9.0
+Version: 3.9.1
 Summary: pytorch❤️keras
 Home-page: https://github.com/lyhue1991/torchkeras
 Author: PythonAiRoad, Laugh
 Author-email: lyhue1991@163.com
 Keywords: machine-learning,deep-learning,ML,DL,pytorch,torch,keras
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -129,14 +129,17 @@
 |ReinforcementLearning——DQN|- |[DQN](./examples/DQN.ipynb)|
 |ObjectDetection——FasterRCNN| torchvision  |  [FasterRCNN](./examples/FasterRCNN——vision.ipynb) | 
 |ImageSegmentation——DeepLabV3++ | segmentation_models_pytorch |  [Deeplabv3++](./examples/Deeplabv3plus——smp.ipynb) |
 |InstanceSegmentation——MaskRCNN | detectron2 |  [MaskRCNN](./examples/MaskRCNN——detectron2.ipynb) |
 |ObjectDetection——YOLOv8 🔥🔥| ultralytics |  [YOLOv8](./examples/YOLOv8——ultralytics.ipynb) |
 |TextClassification——BERT 🔥🔥| transformers |  [BERT](./examples/BERT——transformers.ipynb) |
 |TokenClassification——BERT | transformers |  [BERT_NER](./examples/BERT_NER——transformers.ipynb) |
+|FinetuneLLM——ChatGLM2 🔥🔥🔥| transformers |  [ChatGLM2](./examples/ChatGLM2——transformers.ipynb) |
+|FinetuneLLM——ChatGLM2_LoRA 🔥🔥🔥| transformers,peft |  [ChatGLM2_LoRA](./examples/ChatGLM2_LoRA——transformers.ipynb) |
+|FinetuneLLM——ChatGLM2_AdaLoRA 🔥🔥🔥| transformers,peft |  [ChatGLM2_AdaLoRA](./examples/ChatGLM2_AdaLoRA——transformers.ipynb) |
 |ImageClassification——SwinTransformer|timm| [Swin](./examples/SwinTransformer——timm.ipynb)|
 
 **If you want to understand or modify some details of this project, feel free to read and change the source code!!!**
 
 Any other questions, you can contact the author form the wechat official account below:
 
 **算法美食屋**
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchkeras Version: 3.9.0 Summary:
+Metadata-Version: 2.1 Name: torchkeras Version: 3.9.1 Summary:
 pytorchâ¤ï¸keras Home-page: https://github.com/lyhue1991/torchkeras Author:
 PythonAiRoad, Laugh Author-email: lyhue1991@163.com Keywords: machine-
 learning,deep-learning,ML,DL,pytorch,torch,keras Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.5
 Description-Content-Type: text/markdown License-File: LICENSE #
 Pytorchâ¤ï¸Keras English | [ç®ä½ä¸­æ](README.md) The torchkeras library
@@ -67,14 +67,19 @@
 segmentation_models_pytorch | [Deeplabv3++](./examples/
 Deeplabv3plusââsmp.ipynb) | |InstanceSegmentationââMaskRCNN |
 detectron2 | [MaskRCNN](./examples/MaskRCNNââdetectron2.ipynb) |
 |ObjectDetectionââYOLOv8 ð¥ð¥| ultralytics | [YOLOv8](./examples/
 YOLOv8ââultralytics.ipynb) | |TextClassificationââBERT ð¥ð¥|
 transformers | [BERT](./examples/BERTââtransformers.ipynb) |
 |TokenClassificationââBERT | transformers | [BERT_NER](./examples/
-BERT_NERââtransformers.ipynb) |
+BERT_NERââtransformers.ipynb) | |FinetuneLLMââChatGLM2 ð¥ð¥ð¥|
+transformers | [ChatGLM2](./examples/ChatGLM2ââtransformers.ipynb) |
+|FinetuneLLMââChatGLM2_LoRA ð¥ð¥ð¥| transformers,peft |
+[ChatGLM2_LoRA](./examples/ChatGLM2_LoRAââtransformers.ipynb) |
+|FinetuneLLMââChatGLM2_AdaLoRA ð¥ð¥ð¥| transformers,peft |
+[ChatGLM2_AdaLoRA](./examples/ChatGLM2_AdaLoRAââtransformers.ipynb) |
 |ImageClassificationââSwinTransformer|timm| [Swin](./examples/
 SwinTransformerââtimm.ipynb)| **If you want to understand or modify some
 details of this project, feel free to read and change the source code!!!** Any
 other questions, you can contact the author form the wechat official account
 below: **ç®æ³ç¾é£å±** ![](https://tva1.sinaimg.cn/large/
 e6c9d24egy1h41m2zugguj20k00b9q46.jpg)
```

### Comparing `torchkeras-3.9.0/torchkeras.egg-info/SOURCES.txt` & `torchkeras-3.9.1/torchkeras.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -19,12 +19,15 @@
 torchkeras.egg-info/SOURCES.txt
 torchkeras.egg-info/dependency_links.txt
 torchkeras.egg-info/requires.txt
 torchkeras.egg-info/top_level.txt
 torchkeras/assets/SimHei.ttf
 torchkeras/assets/park.jpg
 torchkeras/assets/zidane.jpg
-torchkeras/chatgpt/__init__.py
+torchkeras/chat/__init__.py
+torchkeras/chat/chatglm.py
+torchkeras/chat/chatgpt.py
 torchkeras/models/__init__.py
 torchkeras/models/resnet.py
 torchkeras/models/ssd.py
-torchkeras/models/unet.py
+torchkeras/models/unet.py
+torchkeras/tools/catboost.py
```

