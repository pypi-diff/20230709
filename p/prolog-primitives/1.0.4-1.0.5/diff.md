# Comparing `tmp/prolog_primitives-1.0.4.tar.gz` & `tmp/prolog_primitives-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prolog_primitives-1.0.4.tar", last modified: Sun Jul  9 11:09:56 2023, max compression
+gzip compressed data, was "prolog_primitives-1.0.5.tar", last modified: Sun Jul  9 20:41:39 2023, max compression
```

## Comparing `prolog_primitives-1.0.4.tar` & `prolog_primitives-1.0.5.tar`

### file list

```diff
@@ -1,69 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 11:09:56.818715 prolog_primitives-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-09 11:09:56.818715 prolog_primitives-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-09 11:09:56.000000 prolog_primitives-1.0.4/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 11:09:56.782715 prolog_primitives-1.0.4/prolog_primitives/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-09 11:09:18.000000 prolog_primitives-1.0.4/prolog_primitives/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 11:09:56.794715 prolog_primitives-1.0.4/prolog_primitives/basic/
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/basic/DBManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/basic/DistributedElements.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/basic/PrimitiveWrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/basic/Session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/basic/SubRequestEvent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/basic/Utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/basic/filterKbPrimitive.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/basic/ntPrimitive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 11:09:56.798715 prolog_primitives-1.0.4/prolog_primitives/ml_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/ml_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/ml_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/ml_lib/collections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 11:09:56.802715 prolog_primitives-1.0.4/prolog_primitives/ml_lib/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/ml_lib/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/ml_lib/dataset/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/ml_lib/dataset/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/ml_lib/dataset/fold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/ml_lib/dataset/randomSplit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/ml_lib/dataset/row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/ml_lib/dataset/theoryToDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/ml_lib/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 11:09:56.806715 prolog_primitives-1.0.4/prolog_primitives/ml_lib/neuralNetwork/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/ml_lib/neuralNetwork/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 11:09:56.810715 prolog_primitives-1.0.4/prolog_primitives/ml_lib/predictors/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/ml_lib/predictors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/ml_lib/predictors/classify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/ml_lib/predictors/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/ml_lib/predictors/score.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/ml_lib/predictors/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 11:09:56.814715 prolog_primitives-1.0.4/prolog_primitives/ml_lib/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/ml_lib/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/ml_lib/schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/ml_lib/schema/schemaClass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/ml_lib/schema/theoryToSchema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 11:09:56.818715 prolog_primitives-1.0.4/prolog_primitives/ml_lib/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/ml_lib/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/ml_lib/transformations/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/ml_lib/transformations/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/ml_lib/transformations/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/ml_lib/transformations/one_hot_encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/ml_lib/transformations/schema_trasformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/ml_lib/transformations/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/prolog_primitives/ml_lib/transformations/transformationClass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 11:09:56.786715 prolog_primitives-1.0.4/prolog_primitives.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-09 11:09:56.000000 prolog_primitives-1.0.4/prolog_primitives.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-09 11:09:56.000000 prolog_primitives-1.0.4/prolog_primitives.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 11:09:56.000000 prolog_primitives-1.0.4/prolog_primitives.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 11:09:56.000000 prolog_primitives-1.0.4/prolog_primitives.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-09 11:09:56.000000 prolog_primitives-1.0.4/prolog_primitives.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-09 11:09:56.000000 prolog_primitives-1.0.4/prolog_primitives.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 11:09:56.818715 prolog_primitives-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-07-09 11:07:50.000000 prolog_primitives-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:39.379453 prolog_primitives-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-09 20:41:39.379453 prolog_primitives-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-09 20:41:39.000000 prolog_primitives-1.0.5/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:39.351453 prolog_primitives-1.0.5/prolog_primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-09 20:41:04.000000 prolog_primitives-1.0.5/prolog_primitives/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:39.355453 prolog_primitives-1.0.5/prolog_primitives/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/basic/DBManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/basic/DistributedElements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/basic/PrimitiveWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/basic/Session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/basic/SubRequestEvent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/basic/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/basic/filterKbPrimitive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/basic/nt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:39.363453 prolog_primitives-1.0.5/prolog_primitives/generatedProto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:04.000000 prolog_primitives-1.0.5/prolog_primitives/generatedProto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-07-09 20:41:04.000000 prolog_primitives-1.0.5/prolog_primitives/generatedProto/basicMessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-09 20:41:04.000000 prolog_primitives-1.0.5/prolog_primitives/generatedProto/basicMessages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-07-09 20:41:04.000000 prolog_primitives-1.0.5/prolog_primitives/generatedProto/errorsMessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-09 20:41:04.000000 prolog_primitives-1.0.5/prolog_primitives/generatedProto/errorsMessages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-07-09 20:41:04.000000 prolog_primitives-1.0.5/prolog_primitives/generatedProto/primitiveService_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-09 20:41:04.000000 prolog_primitives-1.0.5/prolog_primitives/generatedProto/primitiveService_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-07-09 20:41:04.000000 prolog_primitives-1.0.5/prolog_primitives/generatedProto/sideEffectsMessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-09 20:41:04.000000 prolog_primitives-1.0.5/prolog_primitives/generatedProto/sideEffectsMessages_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:39.363453 prolog_primitives-1.0.5/prolog_primitives/ml_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/collections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:39.367453 prolog_primitives-1.0.5/prolog_primitives/ml_lib/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/dataset/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/dataset/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/dataset/fold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/dataset/randomSplit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/dataset/row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/dataset/theoryToDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:39.371453 prolog_primitives-1.0.5/prolog_primitives/ml_lib/neuralNetwork/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/neuralNetwork/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:39.371453 prolog_primitives-1.0.5/prolog_primitives/ml_lib/predictors/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/predictors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/predictors/classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/predictors/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/predictors/score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/predictors/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:39.375453 prolog_primitives-1.0.5/prolog_primitives/ml_lib/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/schema/schemaClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/schema/theoryToSchema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:39.379453 prolog_primitives-1.0.5/prolog_primitives/ml_lib/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/transformations/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/transformations/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/transformations/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/transformations/one_hot_encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/transformations/schema_trasformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/transformations/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/prolog_primitives/ml_lib/transformations/transformationClass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:39.351453 prolog_primitives-1.0.5/prolog_primitives.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-09 20:41:39.000000 prolog_primitives-1.0.5/prolog_primitives.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-09 20:41:39.000000 prolog_primitives-1.0.5/prolog_primitives.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 20:41:39.000000 prolog_primitives-1.0.5/prolog_primitives.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 20:41:39.000000 prolog_primitives-1.0.5/prolog_primitives.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-09 20:41:39.000000 prolog_primitives-1.0.5/prolog_primitives.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-09 20:41:39.000000 prolog_primitives-1.0.5/prolog_primitives.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 20:41:39.379453 prolog_primitives-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-07-09 20:39:38.000000 prolog_primitives-1.0.5/setup.py
```

### Comparing `prolog_primitives-1.0.4/LICENSE` & `prolog_primitives-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.4/PKG-INFO` & `prolog_primitives-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prolog_primitives
-Version: 1.0.4
+Version: 1.0.5
 Summary: description here
 Home-page: https://github.com/lorenzo-osimani/prolog_primitives/
 Author: Lorenzo Osimani
 Author-email: lorenzo.osimani@studio.unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/lorenzo-osimani/prolog_primitives/issues
 Project-URL: Source, https://github.com/lorenzo-osimani/prolog_primitives/
```

### Comparing `prolog_primitives-1.0.4/prolog_primitives/basic/DBManager.py` & `prolog_primitives-1.0.5/prolog_primitives/basic/DBManager.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.4/prolog_primitives/basic/DistributedElements.py` & `prolog_primitives-1.0.5/prolog_primitives/basic/DistributedElements.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.4/prolog_primitives/basic/PrimitiveWrapper.py` & `prolog_primitives-1.0.5/prolog_primitives/basic/PrimitiveWrapper.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.4/prolog_primitives/basic/Session.py` & `prolog_primitives-1.0.5/prolog_primitives/basic/Session.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.4/prolog_primitives/basic/SubRequestEvent.py` & `prolog_primitives-1.0.5/prolog_primitives/basic/SubRequestEvent.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.4/prolog_primitives/basic/Utils.py` & `prolog_primitives-1.0.5/prolog_primitives/basic/Utils.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.4/prolog_primitives/basic/filterKbPrimitive.py` & `prolog_primitives-1.0.5/prolog_primitives/basic/filterKbPrimitive.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.4/prolog_primitives/basic/ntPrimitive.py` & `prolog_primitives-1.0.5/prolog_primitives/basic/nt.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from prolog_primitives.basic import DistributedElements, Utils
 from typing import Generator
 
 # this is the main module of your app
 # it is only required if your project must be runnable
 # this is the script to be executed whenever some users writes `python -m python-Primitives-Server` on the command line, eg.
-class NtPrimitive(DistributedElements.DistributedPrimitive):
+class __NtPrimitive(DistributedElements.DistributedPrimitive):
     
     def solve(self, request: DistributedElements.DistributedRequest) -> Generator[DistributedElements.DistributedResponse, None, None]:
         arg0 = request.arguments[0]
         if(arg0.HasField("var")):
             n = 0
             while(True):
                 substitutions = {}
                 substitutions[arg0.var] = Utils.buildConstantArgumentMsg(n)
                 yield request.replySuccess(substitutions = substitutions)
                 n += 1
         elif(arg0.HasField("numeric")):
             yield request.replySuccess(hasNext = False)
         else:
-            yield request.replyFail()
+            yield request.replyFail()
+            
+ntPrimitive = DistributedElements.DistributedPrimitiveWrapper("nt", 4, __NtPrimitive())
```

### Comparing `prolog_primitives-1.0.4/prolog_primitives/ml_lib/collections.py` & `prolog_primitives-1.0.5/prolog_primitives/ml_lib/collections.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.4/prolog_primitives/ml_lib/dataset/cell.py` & `prolog_primitives-1.0.5/prolog_primitives/ml_lib/dataset/cell.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.4/prolog_primitives/ml_lib/dataset/column.py` & `prolog_primitives-1.0.5/prolog_primitives/ml_lib/dataset/column.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.4/prolog_primitives/ml_lib/dataset/fold.py` & `prolog_primitives-1.0.5/prolog_primitives/ml_lib/dataset/fold.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.4/prolog_primitives/ml_lib/dataset/randomSplit.py` & `prolog_primitives-1.0.5/prolog_primitives/ml_lib/dataset/randomSplit.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.4/prolog_primitives/ml_lib/dataset/row.py` & `prolog_primitives-1.0.5/prolog_primitives/ml_lib/dataset/row.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.4/prolog_primitives/ml_lib/dataset/theoryToDataset.py` & `prolog_primitives-1.0.5/prolog_primitives/ml_lib/dataset/theoryToDataset.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.4/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py` & `prolog_primitives-1.0.5/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.4/prolog_primitives/ml_lib/launcher.py` & `prolog_primitives-1.0.5/prolog_primitives/ml_lib/launcher.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.4/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py` & `prolog_primitives-1.0.5/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.4/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py` & `prolog_primitives-1.0.5/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.4/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py` & `prolog_primitives-1.0.5/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.4/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py` & `prolog_primitives-1.0.5/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.4/prolog_primitives/ml_lib/predictors/classify.py` & `prolog_primitives-1.0.5/prolog_primitives/ml_lib/predictors/classify.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.4/prolog_primitives/ml_lib/predictors/predict.py` & `prolog_primitives-1.0.5/prolog_primitives/ml_lib/predictors/predict.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.4/prolog_primitives/ml_lib/predictors/score.py` & `prolog_primitives-1.0.5/prolog_primitives/ml_lib/predictors/score.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.4/prolog_primitives/ml_lib/predictors/train.py` & `prolog_primitives-1.0.5/prolog_primitives/ml_lib/predictors/train.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.4/prolog_primitives/ml_lib/schema/schema.py` & `prolog_primitives-1.0.5/prolog_primitives/ml_lib/schema/schema.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.4/prolog_primitives/ml_lib/schema/schemaClass.py` & `prolog_primitives-1.0.5/prolog_primitives/ml_lib/schema/schemaClass.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.4/prolog_primitives/ml_lib/schema/theoryToSchema.py` & `prolog_primitives-1.0.5/prolog_primitives/ml_lib/schema/theoryToSchema.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.4/prolog_primitives/ml_lib/transformations/drop.py` & `prolog_primitives-1.0.5/prolog_primitives/ml_lib/transformations/drop.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.4/prolog_primitives/ml_lib/transformations/fit.py` & `prolog_primitives-1.0.5/prolog_primitives/ml_lib/transformations/fit.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.4/prolog_primitives/ml_lib/transformations/normalization.py` & `prolog_primitives-1.0.5/prolog_primitives/ml_lib/transformations/normalization.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.4/prolog_primitives/ml_lib/transformations/one_hot_encode.py` & `prolog_primitives-1.0.5/prolog_primitives/ml_lib/transformations/one_hot_encode.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.4/prolog_primitives/ml_lib/transformations/schema_trasformation.py` & `prolog_primitives-1.0.5/prolog_primitives/ml_lib/transformations/schema_trasformation.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.4/prolog_primitives/ml_lib/transformations/transform.py` & `prolog_primitives-1.0.5/prolog_primitives/ml_lib/transformations/transform.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.4/prolog_primitives/ml_lib/transformations/transformationClass.py` & `prolog_primitives-1.0.5/prolog_primitives/ml_lib/transformations/transformationClass.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.0.4/prolog_primitives.egg-info/PKG-INFO` & `prolog_primitives-1.0.5/prolog_primitives.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prolog-primitives
-Version: 1.0.4
+Version: 1.0.5
 Summary: description here
 Home-page: https://github.com/lorenzo-osimani/prolog_primitives/
 Author: Lorenzo Osimani
 Author-email: lorenzo.osimani@studio.unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/lorenzo-osimani/prolog_primitives/issues
 Project-URL: Source, https://github.com/lorenzo-osimani/prolog_primitives/
```

### Comparing `prolog_primitives-1.0.4/prolog_primitives.egg-info/SOURCES.txt` & `prolog_primitives-1.0.5/prolog_primitives.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -16,15 +16,24 @@
 prolog_primitives/basic/DistributedElements.py
 prolog_primitives/basic/PrimitiveWrapper.py
 prolog_primitives/basic/Session.py
 prolog_primitives/basic/SubRequestEvent.py
 prolog_primitives/basic/Utils.py
 prolog_primitives/basic/__init__.py
 prolog_primitives/basic/filterKbPrimitive.py
-prolog_primitives/basic/ntPrimitive.py
+prolog_primitives/basic/nt.py
+prolog_primitives/generatedProto/__init__.py
+prolog_primitives/generatedProto/basicMessages_pb2.py
+prolog_primitives/generatedProto/basicMessages_pb2_grpc.py
+prolog_primitives/generatedProto/errorsMessages_pb2.py
+prolog_primitives/generatedProto/errorsMessages_pb2_grpc.py
+prolog_primitives/generatedProto/primitiveService_pb2.py
+prolog_primitives/generatedProto/primitiveService_pb2_grpc.py
+prolog_primitives/generatedProto/sideEffectsMessages_pb2.py
+prolog_primitives/generatedProto/sideEffectsMessages_pb2_grpc.py
 prolog_primitives/ml_lib/__init__.py
 prolog_primitives/ml_lib/__main__.py
 prolog_primitives/ml_lib/collections.py
 prolog_primitives/ml_lib/launcher.py
 prolog_primitives/ml_lib/dataset/__init__.py
 prolog_primitives/ml_lib/dataset/cell.py
 prolog_primitives/ml_lib/dataset/column.py
```

### Comparing `prolog_primitives-1.0.4/setup.py` & `prolog_primitives-1.0.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -54,44 +54,52 @@
 
     def run(self):
         print(version)
 
 
 class GenerateProtoCommand(distutils.cmd.Command):
     description = 'generate the files from .proto'
+    protoPath = "prolog_primitives/proto"
+    generatedPath = "prolog_primitives/generatedProto"
     user_options = []
 
     def initialize_options(self):
         pass
 
     def finalize_options(self):
         pass
     
     def run(self):
         import os
-        if not os.path.exists("prolog_primitives/generatedProto"):
-            os.mkdir("prolog_primitives/generatedProto")
+        if os.path.exists(self.generatedPath):
+            import shutil
+            shutil.rmtree(self.generatedPath)
+        os.mkdir(self.generatedPath)
+        
         subprocess.run(
-            "python -m grpc_tools.protoc -I prolog_primitives/proto " +
-                "--python_out=prolog_primitives/generatedProto " +
-                "--pyi_out=prolog_primitives/generatedProto " +
-                "--grpc_python_out=prolog_primitives/generatedProto prolog_primitives/proto/*.proto",
+            f"python -m grpc_tools.protoc -I {self.protoPath} " +
+                f"--python_out={self.generatedPath} " +
+                f"--pyi_out={self.generatedPath} " +
+                f"--grpc_python_out={self.generatedPath} {self.protoPath}/*.proto",
             text=True, check=True, shell=True)
         
         import glob
         import re
-        protoFiles = glob.glob('prolog_primitives\generatedProto\*.py',)
+        protoFiles = glob.glob(f'{self.generatedPath}/*.py',)
         for protoFile in protoFiles:
             with open(protoFile, 'r' ) as f:
+                print(protoFile)
                 content = f.read()
                 content_new = re.sub('(^import.*pb2)', r'from . \1', content, flags = re.M)
             with open(protoFile, 'w') as file:
                 file.write(content_new)
-        with open("prolog_primitives\generatedProto\__init__.py", "w") as f:
+        with open(f"{self.generatedPath}/__init__.py", "w") as f:
             f.close()
+        if os.path.exists(f"{self.generatedPath}/__init__.py"):
+            print("Files successfully generated from .proto")
             
 setup(
     name='prolog_primitives',  # Required
     version=version,
     description='description here',
     license='Apache 2.0 License',
     long_description=long_description,
```

