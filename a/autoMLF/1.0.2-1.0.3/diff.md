# Comparing `tmp/autoMLF-1.0.2.tar.gz` & `tmp/autoMLF-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoMLF-1.0.2.tar", last modified: Sun Jul  9 08:14:21 2023, max compression
+gzip compressed data, was "autoMLF-1.0.3.tar", last modified: Sun Jul  9 10:18:13 2023, max compression
```

## Comparing `autoMLF-1.0.2.tar` & `autoMLF-1.0.3.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:14:21.243019 autoMLF-1.0.2/
--rw-r--r--   0 macbook    (501) staff       (20)      529 2023-07-09 08:14:21.242843 autoMLF-1.0.2/PKG-INFO
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:14:21.232250 autoMLF-1.0.2/core/
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:14:21.232632 autoMLF-1.0.2/core/autoML/
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:14:21.232914 autoMLF-1.0.2/core/autoML/AutoDetect/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-07-01 12:14:57.000000 autoMLF-1.0.2/core/autoML/AutoDetect/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     8573 2023-07-09 07:53:00.000000 autoMLF-1.0.2/core/autoML/AutoDetect/auto_detect.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:14:21.233224 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2571 2023-07-09 07:53:00.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/nlp_onnx.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:14:21.233711 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:14:21.234385 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/loader/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/loader/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1735 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/loader/aug.py
--rw-r--r--   0 macbook    (501) staff       (20)     6278 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/loader/dataloader.py
--rw-r--r--   0 macbook    (501) staff       (20)     5021 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/loader/dataloader_v1.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:14:21.235201 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:14:21.235830 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/backbone/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/backbone/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      882 2023-07-09 07:53:00.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/backbone/cnn.py
--rw-r--r--   0 macbook    (501) staff       (20)     5311 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/backbone/resnet.py
--rw-r--r--   0 macbook    (501) staff       (20)     1655 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/backbone/vgg.py
--rw-r--r--   0 macbook    (501) staff       (20)     3777 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/beam.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:14:21.236466 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/seqmodel/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/seqmodel/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)    11634 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/seqmodel/convseq2seq.py
--rw-r--r--   0 macbook    (501) staff       (20)     5731 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/seqmodel/seq2seq.py
--rw-r--r--   0 macbook    (501) staff       (20)     4858 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/seqmodel/transformer.py
--rw-r--r--   0 macbook    (501) staff       (20)    13524 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/trainer.py
--rw-r--r--   0 macbook    (501) staff       (20)     1750 2023-07-09 07:53:00.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/transformerocr.py
--rw-r--r--   0 macbook    (501) staff       (20)      924 2023-05-10 09:12:33.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/vocab.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:14:21.237242 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/optim/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/optim/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1006 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/optim/labelsmoothingloss.py
--rw-r--r--   0 macbook    (501) staff       (20)     1798 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/optim/optim.py
--rw-r--r--   0 macbook    (501) staff       (20)      614 2023-07-09 05:25:34.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/predict.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:14:21.237682 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tests/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tests/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1039 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tests/utest.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:14:21.238943 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1226 2023-07-09 07:53:00.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/config.py
--rw-r--r--   0 macbook    (501) staff       (20)     2754 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/create_dataset.py
--rw-r--r--   0 macbook    (501) staff       (20)      325 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/logger.py
--rw-r--r--   0 macbook    (501) staff       (20)     1431 2023-07-09 05:25:34.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/predictor.py
--rw-r--r--   0 macbook    (501) staff       (20)     7306 2023-07-09 07:53:00.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/translate.py
--rw-r--r--   0 macbook    (501) staff       (20)     2688 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/utils.py
--rw-r--r--   0 macbook    (501) staff       (20)      559 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/train.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:14:21.239429 autoMLF-1.0.2/core/autoML/AutoTraining/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-07-01 12:15:07.000000 autoMLF-1.0.2/core/autoML/AutoTraining/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     7120 2023-07-09 05:27:54.000000 autoMLF-1.0.2/core/autoML/AutoTraining/auto_dir.py
--rw-r--r--   0 macbook    (501) staff       (20)     2096 2023-07-09 07:49:58.000000 autoMLF-1.0.2/core/autoML/AutoTraining/auto_trainer.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:14:21.239772 autoMLF-1.0.2/core/autoML/AutoTransform/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-07-03 03:16:43.000000 autoMLF-1.0.2/core/autoML/AutoTransform/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)    12177 2023-07-09 07:53:00.000000 autoMLF-1.0.2/core/autoML/AutoTransform/auto_four_point_transform.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:14:21.240501 autoMLF-1.0.2/core/autoML/AutoTransform/pyimagesearch/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-07-08 15:03:46.000000 autoMLF-1.0.2/core/autoML/AutoTransform/pyimagesearch/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1640 2023-06-07 08:38:05.000000 autoMLF-1.0.2/core/autoML/AutoTransform/pyimagesearch/imutils.py
--rw-r--r--   0 macbook    (501) staff       (20)     3444 2023-06-07 08:09:09.000000 autoMLF-1.0.2/core/autoML/AutoTransform/pyimagesearch/polygon_interacter.py
--rw-r--r--   0 macbook    (501) staff       (20)     2715 2023-07-09 07:53:00.000000 autoMLF-1.0.2/core/autoML/AutoTransform/pyimagesearch/transform.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:14:21.240831 autoMLF-1.0.2/core/autoML/CLI/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-07-08 15:02:30.000000 autoMLF-1.0.2/core/autoML/CLI/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     5143 2023-07-09 07:58:38.000000 autoMLF-1.0.2/core/autoML/CLI/automltoolkit.py
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-24 13:34:45.000000 autoMLF-1.0.2/core/autoML/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:14:21.241310 autoMLF-1.0.2/core/autoML/api_config/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-07-03 11:10:46.000000 autoMLF-1.0.2/core/autoML/api_config/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      633 2023-07-03 08:39:57.000000 autoMLF-1.0.2/core/autoML/api_config/pydantic_model.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:14:21.242580 autoMLF-1.0.2/core/autoMLF.egg-info/
--rw-r--r--   0 macbook    (501) staff       (20)      529 2023-07-09 08:14:21.000000 autoMLF-1.0.2/core/autoMLF.egg-info/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)     3079 2023-07-09 08:14:21.000000 autoMLF-1.0.2/core/autoMLF.egg-info/SOURCES.txt
--rw-r--r--   0 macbook    (501) staff       (20)        1 2023-07-09 08:14:21.000000 autoMLF-1.0.2/core/autoMLF.egg-info/dependency_links.txt
--rw-r--r--   0 macbook    (501) staff       (20)       74 2023-07-09 08:14:21.000000 autoMLF-1.0.2/core/autoMLF.egg-info/entry_points.txt
--rw-r--r--   0 macbook    (501) staff       (20)     1326 2023-07-09 08:14:21.000000 autoMLF-1.0.2/core/autoMLF.egg-info/requires.txt
--rw-r--r--   0 macbook    (501) staff       (20)        7 2023-07-09 08:14:21.000000 autoMLF-1.0.2/core/autoMLF.egg-info/top_level.txt
--rw-r--r--   0 macbook    (501) staff       (20)       38 2023-07-09 08:14:21.243083 autoMLF-1.0.2/setup.cfg
--rw-r--r--   0 macbook    (501) staff       (20)     1216 2023-07-09 08:14:12.000000 autoMLF-1.0.2/setup.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 10:18:13.862511 autoMLF-1.0.3/
+-rw-r--r--   0 macbook    (501) staff       (20)      529 2023-07-09 10:18:13.862361 autoMLF-1.0.3/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)     3075 2023-07-09 10:17:40.000000 autoMLF-1.0.3/README.md
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 10:18:13.853007 autoMLF-1.0.3/core/
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 10:18:13.853413 autoMLF-1.0.3/core/autoML/
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 10:18:13.853633 autoMLF-1.0.3/core/autoML/AutoDetect/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-07-01 12:14:57.000000 autoMLF-1.0.3/core/autoML/AutoDetect/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     8573 2023-07-09 07:53:00.000000 autoMLF-1.0.3/core/autoML/AutoDetect/auto_detect.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 10:18:13.853884 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2571 2023-07-09 07:53:00.000000 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/nlp_onnx.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 10:18:13.854295 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 10:18:13.854893 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/loader/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/loader/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1735 2023-04-12 07:19:46.000000 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/loader/aug.py
+-rw-r--r--   0 macbook    (501) staff       (20)     6278 2023-04-12 07:19:46.000000 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/loader/dataloader.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5021 2023-04-12 07:19:46.000000 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/loader/dataloader_v1.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 10:18:13.855836 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 10:18:13.856476 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/backbone/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/backbone/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      882 2023-07-09 07:53:00.000000 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/backbone/cnn.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5311 2023-04-12 07:19:46.000000 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/backbone/resnet.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1655 2023-04-12 07:19:46.000000 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/backbone/vgg.py
+-rw-r--r--   0 macbook    (501) staff       (20)     3777 2023-04-12 07:19:46.000000 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/beam.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 10:18:13.857498 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/seqmodel/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/seqmodel/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)    11634 2023-04-12 07:19:46.000000 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/seqmodel/convseq2seq.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5731 2023-04-12 07:19:46.000000 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/seqmodel/seq2seq.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4858 2023-04-12 07:19:46.000000 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/seqmodel/transformer.py
+-rw-r--r--   0 macbook    (501) staff       (20)    13524 2023-04-12 07:19:46.000000 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/trainer.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1750 2023-07-09 07:53:00.000000 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/transformerocr.py
+-rw-r--r--   0 macbook    (501) staff       (20)      924 2023-05-10 09:12:33.000000 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/vocab.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 10:18:13.857959 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/optim/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/optim/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1006 2023-04-12 07:19:46.000000 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/optim/labelsmoothingloss.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1798 2023-04-12 07:19:46.000000 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/optim/optim.py
+-rw-r--r--   0 macbook    (501) staff       (20)      614 2023-07-09 05:25:34.000000 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/predict.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 10:18:13.858275 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tests/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tests/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1039 2023-04-12 07:19:46.000000 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tests/utest.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 10:18:13.859413 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1226 2023-07-09 07:53:00.000000 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/config.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2754 2023-04-12 07:19:46.000000 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/create_dataset.py
+-rw-r--r--   0 macbook    (501) staff       (20)      325 2023-04-12 07:19:46.000000 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/logger.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1431 2023-07-09 05:25:34.000000 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/predictor.py
+-rw-r--r--   0 macbook    (501) staff       (20)     7306 2023-07-09 07:53:00.000000 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/translate.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2688 2023-04-12 07:19:46.000000 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/utils.py
+-rw-r--r--   0 macbook    (501) staff       (20)      559 2023-04-12 07:19:46.000000 autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/train.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 10:18:13.859870 autoMLF-1.0.3/core/autoML/AutoTraining/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-07-01 12:15:07.000000 autoMLF-1.0.3/core/autoML/AutoTraining/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     7120 2023-07-09 05:27:54.000000 autoMLF-1.0.3/core/autoML/AutoTraining/auto_dir.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2096 2023-07-09 07:49:58.000000 autoMLF-1.0.3/core/autoML/AutoTraining/auto_trainer.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 10:18:13.860153 autoMLF-1.0.3/core/autoML/AutoTransform/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-07-03 03:16:43.000000 autoMLF-1.0.3/core/autoML/AutoTransform/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)    12177 2023-07-09 07:53:00.000000 autoMLF-1.0.3/core/autoML/AutoTransform/auto_four_point_transform.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 10:18:13.860744 autoMLF-1.0.3/core/autoML/AutoTransform/pyimagesearch/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-07-08 15:03:46.000000 autoMLF-1.0.3/core/autoML/AutoTransform/pyimagesearch/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1640 2023-06-07 08:38:05.000000 autoMLF-1.0.3/core/autoML/AutoTransform/pyimagesearch/imutils.py
+-rw-r--r--   0 macbook    (501) staff       (20)     3444 2023-06-07 08:09:09.000000 autoMLF-1.0.3/core/autoML/AutoTransform/pyimagesearch/polygon_interacter.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2715 2023-07-09 07:53:00.000000 autoMLF-1.0.3/core/autoML/AutoTransform/pyimagesearch/transform.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 10:18:13.861022 autoMLF-1.0.3/core/autoML/CLI/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-07-08 15:02:30.000000 autoMLF-1.0.3/core/autoML/CLI/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5143 2023-07-09 07:58:38.000000 autoMLF-1.0.3/core/autoML/CLI/automltoolkit.py
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-24 13:34:45.000000 autoMLF-1.0.3/core/autoML/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 10:18:13.861284 autoMLF-1.0.3/core/autoML/api_config/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-07-03 11:10:46.000000 autoMLF-1.0.3/core/autoML/api_config/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      633 2023-07-03 08:39:57.000000 autoMLF-1.0.3/core/autoML/api_config/pydantic_model.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 10:18:13.862157 autoMLF-1.0.3/core/autoMLF.egg-info/
+-rw-r--r--   0 macbook    (501) staff       (20)      529 2023-07-09 10:18:13.000000 autoMLF-1.0.3/core/autoMLF.egg-info/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)     3089 2023-07-09 10:18:13.000000 autoMLF-1.0.3/core/autoMLF.egg-info/SOURCES.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        1 2023-07-09 10:18:13.000000 autoMLF-1.0.3/core/autoMLF.egg-info/dependency_links.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       74 2023-07-09 10:18:13.000000 autoMLF-1.0.3/core/autoMLF.egg-info/entry_points.txt
+-rw-r--r--   0 macbook    (501) staff       (20)     1326 2023-07-09 10:18:13.000000 autoMLF-1.0.3/core/autoMLF.egg-info/requires.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        7 2023-07-09 10:18:13.000000 autoMLF-1.0.3/core/autoMLF.egg-info/top_level.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       38 2023-07-09 10:18:13.862570 autoMLF-1.0.3/setup.cfg
+-rw-r--r--   0 macbook    (501) staff       (20)     1211 2023-07-09 10:18:12.000000 autoMLF-1.0.3/setup.py
```

### Comparing `autoMLF-1.0.2/PKG-INFO` & `autoMLF-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: autoMLF
-Version: 1.0.2
+Version: 1.0.3
 Summary: autoML for training and inference Deep Learning model
 Home-page: https://github.com/aihackervn
 Author: TinVo
 Author-email: tinprocoder0908@gmail.com
 License: MIT
 Keywords: AI HACKER VNESE,AI,autoML,Deep Learning,Computer Vision,Interface
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `autoMLF-1.0.2/core/autoML/AutoDetect/auto_detect.py` & `autoMLF-1.0.3/core/autoML/AutoDetect/auto_detect.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/nlp_onnx.py` & `autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/nlp_onnx.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/loader/aug.py` & `autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/loader/aug.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/loader/dataloader.py` & `autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/loader/dataloader.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/loader/dataloader_v1.py` & `autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/loader/dataloader_v1.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/backbone/cnn.py` & `autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/backbone/cnn.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/backbone/resnet.py` & `autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/backbone/resnet.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/backbone/vgg.py` & `autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/backbone/vgg.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/beam.py` & `autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/beam.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/seqmodel/convseq2seq.py` & `autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/seqmodel/convseq2seq.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/seqmodel/seq2seq.py` & `autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/seqmodel/seq2seq.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/seqmodel/transformer.py` & `autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/seqmodel/transformer.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/trainer.py` & `autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/trainer.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/transformerocr.py` & `autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/transformerocr.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/vocab.py` & `autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/vocab.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/optim/labelsmoothingloss.py` & `autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/optim/labelsmoothingloss.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/optim/optim.py` & `autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/optim/optim.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/predict.py` & `autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/predict.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tests/utest.py` & `autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tests/utest.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/config.py` & `autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/config.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/create_dataset.py` & `autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/create_dataset.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/predictor.py` & `autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/predictor.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/translate.py` & `autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/translate.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/utils.py` & `autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/utils.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/train.py` & `autoMLF-1.0.3/core/autoML/AutoDetect/vietnamese_nlp/vietocr/train.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.2/core/autoML/AutoTraining/auto_dir.py` & `autoMLF-1.0.3/core/autoML/AutoTraining/auto_dir.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.2/core/autoML/AutoTraining/auto_trainer.py` & `autoMLF-1.0.3/core/autoML/AutoTraining/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.2/core/autoML/AutoTransform/auto_four_point_transform.py` & `autoMLF-1.0.3/core/autoML/AutoTransform/auto_four_point_transform.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.2/core/autoML/AutoTransform/pyimagesearch/imutils.py` & `autoMLF-1.0.3/core/autoML/AutoTransform/pyimagesearch/imutils.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.2/core/autoML/AutoTransform/pyimagesearch/polygon_interacter.py` & `autoMLF-1.0.3/core/autoML/AutoTransform/pyimagesearch/polygon_interacter.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.2/core/autoML/AutoTransform/pyimagesearch/transform.py` & `autoMLF-1.0.3/core/autoML/AutoTransform/pyimagesearch/transform.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.2/core/autoML/CLI/automltoolkit.py` & `autoMLF-1.0.3/core/autoML/CLI/automltoolkit.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.2/core/autoML/api_config/pydantic_model.py` & `autoMLF-1.0.3/core/autoML/api_config/pydantic_model.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.2/core/autoMLF.egg-info/PKG-INFO` & `autoMLF-1.0.3/core/autoMLF.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: autoMLF
-Version: 1.0.2
+Version: 1.0.3
 Summary: autoML for training and inference Deep Learning model
 Home-page: https://github.com/aihackervn
 Author: TinVo
 Author-email: tinprocoder0908@gmail.com
 License: MIT
 Keywords: AI HACKER VNESE,AI,autoML,Deep Learning,Computer Vision,Interface
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `autoMLF-1.0.2/core/autoMLF.egg-info/SOURCES.txt` & `autoMLF-1.0.3/core/autoMLF.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+README.md
 setup.py
 core/autoML/__init__.py
 core/autoML/AutoDetect/__init__.py
 core/autoML/AutoDetect/auto_detect.py
 core/autoML/AutoDetect/vietnamese_nlp/__init__.py
 core/autoML/AutoDetect/vietnamese_nlp/nlp_onnx.py
 core/autoML/AutoDetect/vietnamese_nlp/vietocr/__init__.py
```

### Comparing `autoMLF-1.0.2/core/autoMLF.egg-info/requires.txt` & `autoMLF-1.0.3/core/autoMLF.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.2/setup.py` & `autoMLF-1.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import find_packages, setup
 
-# with open("app/JustScan/README.md", "r") as f:
-#     long_description = f.read()
+with open("core/autoML/README.md", "r") as f:
+    long_description = f.read()
 with open("requirements.txt", "r") as f:
     install_requires = [line.strip() for line in f if line.strip()]
 setup(
     name="autoMLF",
-    version="1.0.2",
+    version="1.0.3",
     description="autoML for training and inference Deep Learning model",
     package_dir={"": "core"},
     packages=find_packages(where="./core"),
     # long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aihackervn",
     author="TinVo",
@@ -29,9 +29,9 @@
         'console_scripts': [
             'auto_mls = autoML.CLI.automltoolkit:start_terminal_loop',
         ],
     },
     extras_require={
         "dev": ["pytest>=7.0", "twine>=4.0.2"],
     },
-    python_requires=">=3.8"
+    python_requires=">=3.9"
 )
```

