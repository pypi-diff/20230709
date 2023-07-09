# Comparing `tmp/autoMLF-1.0.1.tar.gz` & `tmp/autoMLF-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoMLF-1.0.1.tar", last modified: Sun Jul  9 08:13:04 2023, max compression
+gzip compressed data, was "autoMLF-1.0.2.tar", last modified: Sun Jul  9 08:14:21 2023, max compression
```

## Comparing `autoMLF-1.0.1.tar` & `autoMLF-1.0.2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:13:04.703196 autoMLF-1.0.1/
--rw-r--r--   0 macbook    (501) staff       (20)      529 2023-07-09 08:13:04.703001 autoMLF-1.0.1/PKG-INFO
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:13:04.692158 autoMLF-1.0.1/core/
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:13:04.692536 autoMLF-1.0.1/core/autoML/
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:13:04.692815 autoMLF-1.0.1/core/autoML/AutoDetect/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-07-01 12:14:57.000000 autoMLF-1.0.1/core/autoML/AutoDetect/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     8573 2023-07-09 07:53:00.000000 autoMLF-1.0.1/core/autoML/AutoDetect/auto_detect.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:13:04.693391 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     2571 2023-07-09 07:53:00.000000 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/nlp_onnx.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:13:04.694074 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:13:04.694832 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/loader/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/loader/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1735 2023-04-12 07:19:46.000000 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/loader/aug.py
--rw-r--r--   0 macbook    (501) staff       (20)     6278 2023-04-12 07:19:46.000000 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/loader/dataloader.py
--rw-r--r--   0 macbook    (501) staff       (20)     5021 2023-04-12 07:19:46.000000 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/loader/dataloader_v1.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:13:04.695688 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:13:04.696455 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/backbone/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/backbone/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      882 2023-07-09 07:53:00.000000 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/backbone/cnn.py
--rw-r--r--   0 macbook    (501) staff       (20)     5311 2023-04-12 07:19:46.000000 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/backbone/resnet.py
--rw-r--r--   0 macbook    (501) staff       (20)     1655 2023-04-12 07:19:46.000000 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/backbone/vgg.py
--rw-r--r--   0 macbook    (501) staff       (20)     3777 2023-04-12 07:19:46.000000 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/beam.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:13:04.697211 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/seqmodel/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/seqmodel/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)    11634 2023-04-12 07:19:46.000000 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/seqmodel/convseq2seq.py
--rw-r--r--   0 macbook    (501) staff       (20)     5731 2023-04-12 07:19:46.000000 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/seqmodel/seq2seq.py
--rw-r--r--   0 macbook    (501) staff       (20)     4858 2023-04-12 07:19:46.000000 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/seqmodel/transformer.py
--rw-r--r--   0 macbook    (501) staff       (20)    13524 2023-04-12 07:19:46.000000 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/trainer.py
--rw-r--r--   0 macbook    (501) staff       (20)     1750 2023-07-09 07:53:00.000000 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/transformerocr.py
--rw-r--r--   0 macbook    (501) staff       (20)      924 2023-05-10 09:12:33.000000 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/vocab.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:13:04.697747 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/optim/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/optim/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1006 2023-04-12 07:19:46.000000 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/optim/labelsmoothingloss.py
--rw-r--r--   0 macbook    (501) staff       (20)     1798 2023-04-12 07:19:46.000000 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/optim/optim.py
--rw-r--r--   0 macbook    (501) staff       (20)      614 2023-07-09 05:25:34.000000 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/predict.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:13:04.698083 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tests/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tests/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1039 2023-04-12 07:19:46.000000 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tests/utest.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:13:04.699215 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1226 2023-07-09 07:53:00.000000 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/config.py
--rw-r--r--   0 macbook    (501) staff       (20)     2754 2023-04-12 07:19:46.000000 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/create_dataset.py
--rw-r--r--   0 macbook    (501) staff       (20)      325 2023-04-12 07:19:46.000000 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/logger.py
--rw-r--r--   0 macbook    (501) staff       (20)     1431 2023-07-09 05:25:34.000000 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/predictor.py
--rw-r--r--   0 macbook    (501) staff       (20)     7306 2023-07-09 07:53:00.000000 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/translate.py
--rw-r--r--   0 macbook    (501) staff       (20)     2688 2023-04-12 07:19:46.000000 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/utils.py
--rw-r--r--   0 macbook    (501) staff       (20)      559 2023-04-12 07:19:46.000000 autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/train.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:13:04.699746 autoMLF-1.0.1/core/autoML/AutoTraining/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-07-01 12:15:07.000000 autoMLF-1.0.1/core/autoML/AutoTraining/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     7120 2023-07-09 05:27:54.000000 autoMLF-1.0.1/core/autoML/AutoTraining/auto_dir.py
--rw-r--r--   0 macbook    (501) staff       (20)     2096 2023-07-09 07:49:58.000000 autoMLF-1.0.1/core/autoML/AutoTraining/auto_trainer.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:13:04.700090 autoMLF-1.0.1/core/autoML/AutoTransform/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-07-03 03:16:43.000000 autoMLF-1.0.1/core/autoML/AutoTransform/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)    12177 2023-07-09 07:53:00.000000 autoMLF-1.0.1/core/autoML/AutoTransform/auto_four_point_transform.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:13:04.700837 autoMLF-1.0.1/core/autoML/AutoTransform/pyimagesearch/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-07-08 15:03:46.000000 autoMLF-1.0.1/core/autoML/AutoTransform/pyimagesearch/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1640 2023-06-07 08:38:05.000000 autoMLF-1.0.1/core/autoML/AutoTransform/pyimagesearch/imutils.py
--rw-r--r--   0 macbook    (501) staff       (20)     3444 2023-06-07 08:09:09.000000 autoMLF-1.0.1/core/autoML/AutoTransform/pyimagesearch/polygon_interacter.py
--rw-r--r--   0 macbook    (501) staff       (20)     2715 2023-07-09 07:53:00.000000 autoMLF-1.0.1/core/autoML/AutoTransform/pyimagesearch/transform.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:13:04.701209 autoMLF-1.0.1/core/autoML/CLI/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-07-08 15:02:30.000000 autoMLF-1.0.1/core/autoML/CLI/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     5143 2023-07-09 07:58:38.000000 autoMLF-1.0.1/core/autoML/CLI/automltoolkit.py
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-24 13:34:45.000000 autoMLF-1.0.1/core/autoML/__init__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:13:04.701573 autoMLF-1.0.1/core/autoML/api_config/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-07-03 11:10:46.000000 autoMLF-1.0.1/core/autoML/api_config/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      633 2023-07-03 08:39:57.000000 autoMLF-1.0.1/core/autoML/api_config/pydantic_model.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:13:04.702705 autoMLF-1.0.1/core/autoMLF.egg-info/
--rw-r--r--   0 macbook    (501) staff       (20)      529 2023-07-09 08:13:04.000000 autoMLF-1.0.1/core/autoMLF.egg-info/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)     3079 2023-07-09 08:13:04.000000 autoMLF-1.0.1/core/autoMLF.egg-info/SOURCES.txt
--rw-r--r--   0 macbook    (501) staff       (20)        1 2023-07-09 08:13:04.000000 autoMLF-1.0.1/core/autoMLF.egg-info/dependency_links.txt
--rw-r--r--   0 macbook    (501) staff       (20)       74 2023-07-09 08:13:04.000000 autoMLF-1.0.1/core/autoMLF.egg-info/entry_points.txt
--rw-r--r--   0 macbook    (501) staff       (20)     1325 2023-07-09 08:13:04.000000 autoMLF-1.0.1/core/autoMLF.egg-info/requires.txt
--rw-r--r--   0 macbook    (501) staff       (20)        7 2023-07-09 08:13:04.000000 autoMLF-1.0.1/core/autoMLF.egg-info/top_level.txt
--rw-r--r--   0 macbook    (501) staff       (20)       38 2023-07-09 08:13:04.703262 autoMLF-1.0.1/setup.cfg
--rw-r--r--   0 macbook    (501) staff       (20)     1216 2023-07-09 08:13:01.000000 autoMLF-1.0.1/setup.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:14:21.243019 autoMLF-1.0.2/
+-rw-r--r--   0 macbook    (501) staff       (20)      529 2023-07-09 08:14:21.242843 autoMLF-1.0.2/PKG-INFO
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:14:21.232250 autoMLF-1.0.2/core/
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:14:21.232632 autoMLF-1.0.2/core/autoML/
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:14:21.232914 autoMLF-1.0.2/core/autoML/AutoDetect/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-07-01 12:14:57.000000 autoMLF-1.0.2/core/autoML/AutoDetect/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     8573 2023-07-09 07:53:00.000000 autoMLF-1.0.2/core/autoML/AutoDetect/auto_detect.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:14:21.233224 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2571 2023-07-09 07:53:00.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/nlp_onnx.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:14:21.233711 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:14:21.234385 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/loader/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/loader/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1735 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/loader/aug.py
+-rw-r--r--   0 macbook    (501) staff       (20)     6278 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/loader/dataloader.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5021 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/loader/dataloader_v1.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:14:21.235201 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:14:21.235830 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/backbone/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/backbone/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      882 2023-07-09 07:53:00.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/backbone/cnn.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5311 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/backbone/resnet.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1655 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/backbone/vgg.py
+-rw-r--r--   0 macbook    (501) staff       (20)     3777 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/beam.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:14:21.236466 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/seqmodel/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/seqmodel/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)    11634 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/seqmodel/convseq2seq.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5731 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/seqmodel/seq2seq.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4858 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/seqmodel/transformer.py
+-rw-r--r--   0 macbook    (501) staff       (20)    13524 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/trainer.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1750 2023-07-09 07:53:00.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/transformerocr.py
+-rw-r--r--   0 macbook    (501) staff       (20)      924 2023-05-10 09:12:33.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/vocab.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:14:21.237242 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/optim/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/optim/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1006 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/optim/labelsmoothingloss.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1798 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/optim/optim.py
+-rw-r--r--   0 macbook    (501) staff       (20)      614 2023-07-09 05:25:34.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/predict.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:14:21.237682 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tests/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tests/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1039 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tests/utest.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:14:21.238943 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1226 2023-07-09 07:53:00.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/config.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2754 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/create_dataset.py
+-rw-r--r--   0 macbook    (501) staff       (20)      325 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/logger.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1431 2023-07-09 05:25:34.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/predictor.py
+-rw-r--r--   0 macbook    (501) staff       (20)     7306 2023-07-09 07:53:00.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/translate.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2688 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/utils.py
+-rw-r--r--   0 macbook    (501) staff       (20)      559 2023-04-12 07:19:46.000000 autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/train.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:14:21.239429 autoMLF-1.0.2/core/autoML/AutoTraining/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-07-01 12:15:07.000000 autoMLF-1.0.2/core/autoML/AutoTraining/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     7120 2023-07-09 05:27:54.000000 autoMLF-1.0.2/core/autoML/AutoTraining/auto_dir.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2096 2023-07-09 07:49:58.000000 autoMLF-1.0.2/core/autoML/AutoTraining/auto_trainer.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:14:21.239772 autoMLF-1.0.2/core/autoML/AutoTransform/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-07-03 03:16:43.000000 autoMLF-1.0.2/core/autoML/AutoTransform/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)    12177 2023-07-09 07:53:00.000000 autoMLF-1.0.2/core/autoML/AutoTransform/auto_four_point_transform.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:14:21.240501 autoMLF-1.0.2/core/autoML/AutoTransform/pyimagesearch/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-07-08 15:03:46.000000 autoMLF-1.0.2/core/autoML/AutoTransform/pyimagesearch/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1640 2023-06-07 08:38:05.000000 autoMLF-1.0.2/core/autoML/AutoTransform/pyimagesearch/imutils.py
+-rw-r--r--   0 macbook    (501) staff       (20)     3444 2023-06-07 08:09:09.000000 autoMLF-1.0.2/core/autoML/AutoTransform/pyimagesearch/polygon_interacter.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2715 2023-07-09 07:53:00.000000 autoMLF-1.0.2/core/autoML/AutoTransform/pyimagesearch/transform.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:14:21.240831 autoMLF-1.0.2/core/autoML/CLI/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-07-08 15:02:30.000000 autoMLF-1.0.2/core/autoML/CLI/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     5143 2023-07-09 07:58:38.000000 autoMLF-1.0.2/core/autoML/CLI/automltoolkit.py
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-06-24 13:34:45.000000 autoMLF-1.0.2/core/autoML/__init__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:14:21.241310 autoMLF-1.0.2/core/autoML/api_config/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-07-03 11:10:46.000000 autoMLF-1.0.2/core/autoML/api_config/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      633 2023-07-03 08:39:57.000000 autoMLF-1.0.2/core/autoML/api_config/pydantic_model.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-09 08:14:21.242580 autoMLF-1.0.2/core/autoMLF.egg-info/
+-rw-r--r--   0 macbook    (501) staff       (20)      529 2023-07-09 08:14:21.000000 autoMLF-1.0.2/core/autoMLF.egg-info/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)     3079 2023-07-09 08:14:21.000000 autoMLF-1.0.2/core/autoMLF.egg-info/SOURCES.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        1 2023-07-09 08:14:21.000000 autoMLF-1.0.2/core/autoMLF.egg-info/dependency_links.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       74 2023-07-09 08:14:21.000000 autoMLF-1.0.2/core/autoMLF.egg-info/entry_points.txt
+-rw-r--r--   0 macbook    (501) staff       (20)     1326 2023-07-09 08:14:21.000000 autoMLF-1.0.2/core/autoMLF.egg-info/requires.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        7 2023-07-09 08:14:21.000000 autoMLF-1.0.2/core/autoMLF.egg-info/top_level.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       38 2023-07-09 08:14:21.243083 autoMLF-1.0.2/setup.cfg
+-rw-r--r--   0 macbook    (501) staff       (20)     1216 2023-07-09 08:14:12.000000 autoMLF-1.0.2/setup.py
```

### Comparing `autoMLF-1.0.1/PKG-INFO` & `autoMLF-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoMLF
-Version: 1.0.1
+Version: 1.0.2
 Summary: autoML for training and inference Deep Learning model
 Home-page: https://github.com/aihackervn
 Author: TinVo
 Author-email: tinprocoder0908@gmail.com
 License: MIT
 Keywords: AI HACKER VNESE,AI,autoML,Deep Learning,Computer Vision,Interface
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autoMLF-1.0.1/core/autoML/AutoDetect/auto_detect.py` & `autoMLF-1.0.2/core/autoML/AutoDetect/auto_detect.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/nlp_onnx.py` & `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/nlp_onnx.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/loader/aug.py` & `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/loader/aug.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/loader/dataloader.py` & `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/loader/dataloader.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/loader/dataloader_v1.py` & `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/loader/dataloader_v1.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/backbone/cnn.py` & `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/backbone/cnn.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/backbone/resnet.py` & `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/backbone/resnet.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/backbone/vgg.py` & `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/backbone/vgg.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/beam.py` & `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/beam.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/seqmodel/convseq2seq.py` & `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/seqmodel/convseq2seq.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/seqmodel/seq2seq.py` & `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/seqmodel/seq2seq.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/seqmodel/transformer.py` & `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/seqmodel/transformer.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/trainer.py` & `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/trainer.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/transformerocr.py` & `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/transformerocr.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/vocab.py` & `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/model/vocab.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/optim/labelsmoothingloss.py` & `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/optim/labelsmoothingloss.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/optim/optim.py` & `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/optim/optim.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/predict.py` & `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/predict.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tests/utest.py` & `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tests/utest.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/config.py` & `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/config.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/create_dataset.py` & `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/create_dataset.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/predictor.py` & `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/predictor.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/translate.py` & `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/translate.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/utils.py` & `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/tool/utils.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.1/core/autoML/AutoDetect/vietnamese_nlp/vietocr/train.py` & `autoMLF-1.0.2/core/autoML/AutoDetect/vietnamese_nlp/vietocr/train.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.1/core/autoML/AutoTraining/auto_dir.py` & `autoMLF-1.0.2/core/autoML/AutoTraining/auto_dir.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.1/core/autoML/AutoTraining/auto_trainer.py` & `autoMLF-1.0.2/core/autoML/AutoTraining/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.1/core/autoML/AutoTransform/auto_four_point_transform.py` & `autoMLF-1.0.2/core/autoML/AutoTransform/auto_four_point_transform.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.1/core/autoML/AutoTransform/pyimagesearch/imutils.py` & `autoMLF-1.0.2/core/autoML/AutoTransform/pyimagesearch/imutils.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.1/core/autoML/AutoTransform/pyimagesearch/polygon_interacter.py` & `autoMLF-1.0.2/core/autoML/AutoTransform/pyimagesearch/polygon_interacter.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.1/core/autoML/AutoTransform/pyimagesearch/transform.py` & `autoMLF-1.0.2/core/autoML/AutoTransform/pyimagesearch/transform.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.1/core/autoML/CLI/automltoolkit.py` & `autoMLF-1.0.2/core/autoML/CLI/automltoolkit.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.1/core/autoML/api_config/pydantic_model.py` & `autoMLF-1.0.2/core/autoML/api_config/pydantic_model.py`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.1/core/autoMLF.egg-info/PKG-INFO` & `autoMLF-1.0.2/core/autoMLF.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoMLF
-Version: 1.0.1
+Version: 1.0.2
 Summary: autoML for training and inference Deep Learning model
 Home-page: https://github.com/aihackervn
 Author: TinVo
 Author-email: tinprocoder0908@gmail.com
 License: MIT
 Keywords: AI HACKER VNESE,AI,autoML,Deep Learning,Computer Vision,Interface
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autoMLF-1.0.1/core/autoMLF.egg-info/SOURCES.txt` & `autoMLF-1.0.2/core/autoMLF.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autoMLF-1.0.1/core/autoMLF.egg-info/requires.txt` & `autoMLF-1.0.2/core/autoMLF.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 six==1.16.0
 sniffio==1.3.0
 soupsieve==2.4.1
 starlette==0.27.0
 sympy==1.12
 threadpoolctl==3.1.0
 torch==1.9.0
-torchvision==0.9.0
+torchvision==0.10.0
 tqdm==4.65.0
 twine==4.0.2
 typing_extensions==4.7.1
 tzdata==2023.3
 ultralytics==8.0.131
 urllib3==2.0.3
 webencodings==0.5.1
```

### Comparing `autoMLF-1.0.1/setup.py` & `autoMLF-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # with open("app/JustScan/README.md", "r") as f:
 #     long_description = f.read()
 with open("requirements.txt", "r") as f:
     install_requires = [line.strip() for line in f if line.strip()]
 setup(
     name="autoMLF",
-    version="1.0.1",
+    version="1.0.2",
     description="autoML for training and inference Deep Learning model",
     package_dir={"": "core"},
     packages=find_packages(where="./core"),
     # long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aihackervn",
     author="TinVo",
```

