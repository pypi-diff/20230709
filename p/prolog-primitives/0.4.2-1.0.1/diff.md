# Comparing `tmp/prolog_primitives-0.4.2.tar.gz` & `tmp/prolog_primitives-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prolog_primitives-0.4.2.tar", last modified: Sun Jul  2 16:00:33 2023, max compression
+gzip compressed data, was "prolog_primitives-1.0.1.tar", last modified: Sun Jul  9 09:54:15 2023, max compression
```

## Comparing `prolog_primitives-0.4.2.tar` & `prolog_primitives-1.0.1.tar`

### file list

```diff
@@ -1,78 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:00:33.364863 prolog_primitives-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-02 16:00:33.364863 prolog_primitives-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:00:33.356862 prolog_primitives-0.4.2/prolog_primitives/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-02 16:00:25.000000 prolog_primitives-0.4.2/prolog_primitives/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:00:33.360862 prolog_primitives-0.4.2/prolog_primitives/basic/
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/basic/DBManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/basic/DistributedElements.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/basic/PrimitiveWrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/basic/Session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/basic/SubRequestEvent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/basic/Utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/basic/filterKbPrimitive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/basic/ntPrimitive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:00:33.360862 prolog_primitives-0.4.2/prolog_primitives/generatedProto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 16:00:25.000000 prolog_primitives-0.4.2/prolog_primitives/generatedProto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7130 2023-07-02 16:00:25.000000 prolog_primitives-0.4.2/prolog_primitives/generatedProto/basicMessages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-02 16:00:25.000000 prolog_primitives-0.4.2/prolog_primitives/generatedProto/basicMessages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-07-02 16:00:25.000000 prolog_primitives-0.4.2/prolog_primitives/generatedProto/errorsMessages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-02 16:00:25.000000 prolog_primitives-0.4.2/prolog_primitives/generatedProto/errorsMessages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-07-02 16:00:25.000000 prolog_primitives-0.4.2/prolog_primitives/generatedProto/primitiveService_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-02 16:00:25.000000 prolog_primitives-0.4.2/prolog_primitives/generatedProto/primitiveService_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-07-02 16:00:25.000000 prolog_primitives-0.4.2/prolog_primitives/generatedProto/sideEffectsMessages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-02 16:00:25.000000 prolog_primitives-0.4.2/prolog_primitives/generatedProto/sideEffectsMessages_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:00:33.360862 prolog_primitives-0.4.2/prolog_primitives/ml_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/collections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:00:33.364863 prolog_primitives-0.4.2/prolog_primitives/ml_lib/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/dataset/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/dataset/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/dataset/fold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/dataset/randomSplit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/dataset/row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/dataset/theoryToDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:00:33.364863 prolog_primitives-0.4.2/prolog_primitives/ml_lib/neuralNetwork/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/neuralNetwork/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:00:33.364863 prolog_primitives-0.4.2/prolog_primitives/ml_lib/predictors/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/predictors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/predictors/classify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/predictors/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/predictors/score.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/predictors/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:00:33.364863 prolog_primitives-0.4.2/prolog_primitives/ml_lib/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/schema/schemaClass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/schema/theoryToSchema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:00:33.364863 prolog_primitives-0.4.2/prolog_primitives/ml_lib/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/transformations/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/transformations/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/transformations/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/transformations/one_hot_encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/transformations/schema_trasformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/transformations/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/transformations/transformationClass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:00:33.360862 prolog_primitives-0.4.2/prolog_primitives.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-02 16:00:33.000000 prolog_primitives-0.4.2/prolog_primitives.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-02 16:00:33.000000 prolog_primitives-0.4.2/prolog_primitives.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 16:00:33.000000 prolog_primitives-0.4.2/prolog_primitives.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 16:00:33.000000 prolog_primitives-0.4.2/prolog_primitives.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-02 16:00:33.000000 prolog_primitives-0.4.2/prolog_primitives.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-02 16:00:33.000000 prolog_primitives-0.4.2/prolog_primitives.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 16:00:33.364863 prolog_primitives-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:54:15.139854 prolog_primitives-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-09 09:54:15.139854 prolog_primitives-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-09 09:54:15.000000 prolog_primitives-1.0.1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:54:15.135854 prolog_primitives-1.0.1/prolog_primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-09 09:53:49.000000 prolog_primitives-1.0.1/prolog_primitives/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:54:15.135854 prolog_primitives-1.0.1/prolog_primitives/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/basic/DBManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/basic/DistributedElements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/basic/PrimitiveWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/basic/Session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/basic/SubRequestEvent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/basic/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/basic/filterKbPrimitive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/basic/ntPrimitive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:54:15.135854 prolog_primitives-1.0.1/prolog_primitives/ml_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/ml_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/ml_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/ml_lib/collections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:54:15.139854 prolog_primitives-1.0.1/prolog_primitives/ml_lib/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/ml_lib/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/ml_lib/dataset/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/ml_lib/dataset/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/ml_lib/dataset/fold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/ml_lib/dataset/randomSplit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/ml_lib/dataset/row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/ml_lib/dataset/theoryToDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/ml_lib/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:54:15.139854 prolog_primitives-1.0.1/prolog_primitives/ml_lib/neuralNetwork/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/ml_lib/neuralNetwork/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:54:15.139854 prolog_primitives-1.0.1/prolog_primitives/ml_lib/predictors/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/ml_lib/predictors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/ml_lib/predictors/classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/ml_lib/predictors/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/ml_lib/predictors/score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/ml_lib/predictors/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:54:15.139854 prolog_primitives-1.0.1/prolog_primitives/ml_lib/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/ml_lib/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/ml_lib/schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/ml_lib/schema/schemaClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/ml_lib/schema/theoryToSchema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:54:15.139854 prolog_primitives-1.0.1/prolog_primitives/ml_lib/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/ml_lib/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/ml_lib/transformations/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/ml_lib/transformations/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/ml_lib/transformations/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/ml_lib/transformations/one_hot_encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/ml_lib/transformations/schema_trasformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/ml_lib/transformations/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/prolog_primitives/ml_lib/transformations/transformationClass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:54:15.135854 prolog_primitives-1.0.1/prolog_primitives.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-09 09:54:15.000000 prolog_primitives-1.0.1/prolog_primitives.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-09 09:54:15.000000 prolog_primitives-1.0.1/prolog_primitives.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 09:54:15.000000 prolog_primitives-1.0.1/prolog_primitives.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 09:54:14.000000 prolog_primitives-1.0.1/prolog_primitives.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-09 09:54:15.000000 prolog_primitives-1.0.1/prolog_primitives.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-09 09:54:15.000000 prolog_primitives-1.0.1/prolog_primitives.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 09:54:15.139854 prolog_primitives-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-07-09 09:52:41.000000 prolog_primitives-1.0.1/setup.py
```

### Comparing `prolog_primitives-0.4.2/LICENSE` & `prolog_primitives-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.2/PKG-INFO` & `prolog_primitives-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prolog_primitives
-Version: 0.4.2
+Version: 1.0.1
 Summary: description here
 Home-page: https://github.com/lorenzo-osimani/prolog_primitives/
 Author: Lorenzo Osimani
 Author-email: lorenzo.osimani@studio.unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/lorenzo-osimani/prolog_primitives/issues
 Project-URL: Source, https://github.com/lorenzo-osimani/prolog_primitives/
```

### Comparing `prolog_primitives-0.4.2/prolog_primitives/basic/DBManager.py` & `prolog_primitives-1.0.1/prolog_primitives/basic/DBManager.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.2/prolog_primitives/basic/DistributedElements.py` & `prolog_primitives-1.0.1/prolog_primitives/basic/DistributedElements.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.2/prolog_primitives/basic/PrimitiveWrapper.py` & `prolog_primitives-1.0.1/prolog_primitives/basic/PrimitiveWrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     executor: futures.Executor
     
     def __init__(self, primitive: DistributedElements.DistributedPrimitive, functor: str, arity: int, executor):  
         self.primitive = primitive
         self.functor = functor
         self.arity = arity
         self.executor = executor
-        
 
     def getSignature(self, request, context):
         signature = (self.functor, self.arity)
         return basicMsg.SignatureMsg(name=signature[0], arity=signature[1])
 
     def callPrimitive(self, request_iterator, context: Context):
         queue = Queue[primitivesMsg.GeneratorMsg]()
@@ -35,25 +34,27 @@
                 if(session == None and msg.request.IsInitialized()):
                     session = Session.ServerSession(
                         primitive = self.primitive,
                         request = msg.request,
                         queue = queue)
                 else:
                     self.executor.submit(session.handleMessage, msg)
-        
         self.executor.submit(messageHandling)
         
         context.add_callback(lambda: queue.put(None))
+        
         while context.is_active():
             msg: primitivesMsg.GeneratorMsg = queue.get()
             if(msg != None):
-                yield msg              
+                yield msg
+            else:
+                context.cancel()
 
 def serve(primitive: DistributedElements.DistributedPrimitiveWrapper, port: int = 8080, libraryName: str = "", withDB: bool = False):
-    executor = futures.ThreadPoolExecutor(64)
+    executor = futures.ThreadPoolExecutor(32)
     service = GenericPrimitive(primitive.primitive, primitive.functor, primitive.arity, executor)
     server = grpc.server(executor)
     Server.add_GenericPrimitiveServiceServicer_to_server(service, server)
     server.add_insecure_port('[::]:' + str(port))
     server.start()
     if(withDB):
         DBManager.addPrimitive(service.functor, service.arity, libraryName, "localhost", port)
```

### Comparing `prolog_primitives-0.4.2/prolog_primitives/basic/Session.py` & `prolog_primitives-1.0.1/prolog_primitives/basic/Session.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.2/prolog_primitives/basic/SubRequestEvent.py` & `prolog_primitives-1.0.1/prolog_primitives/basic/SubRequestEvent.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.2/prolog_primitives/basic/Utils.py` & `prolog_primitives-1.0.1/prolog_primitives/basic/Utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 
 from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
+import numbers
 
 class Struct:
     functor: str
     arguments: list
     
     def __init__(self, functor: str, arguments: list):
         self.functor = functor
@@ -22,61 +23,74 @@
     if(msg.HasField("struct")):
         if(msg.struct.functor == "."):
             return parseArgumentMsgList(msg)
         else:   
             return parseStructMsg(msg.struct)
     elif(msg.HasField("var")):
         return msg.var
-    elif(msg.HasField("constant")):
-        return msg.constant
+    elif(msg.HasField("numeric")):
+        return msg.numeric
+    elif(msg.HasField("atom")):
+        return msg.atom
     
 def parseStructMsg(msg: basicMsg.StructMsg):
     if(len(msg.arguments) > 0):
         arguments = list()
         for arg in msg.arguments:
             arguments.append(parseArgumentMsg(arg))
         return Struct(msg.functor, arguments)
     else:   
         return msg.functor
-    
-    
+       
 def parseArgumentMsgList(msg: basicMsg.ArgumentMsg) -> list:
     returnValue = list()
     currentValue = msg.struct
     while(len(currentValue.arguments) != 0):
         returnValue.append(parseArgumentMsg(currentValue.arguments[0]))
         currentValue = currentValue.arguments[1].struct
     return returnValue 
 
 def fromListToArgumentMsg(elements: list) -> basicMsg.ArgumentMsg:
-    last_element = basicMsg.ArgumentMsg(
-        struct=basicMsg.StructMsg(
+    last_element = buildConstantArgumentMsg(
+        basicMsg.StructMsg(
                 functor = "[]"
             )
         )
     
     elements.reverse()
     for i in elements:
         current_element = basicMsg.StructMsg(
             functor="."
         )
         if(type(i) is basicMsg.StructMsg):
             current_element.arguments.append(
-                basicMsg.ArgumentMsg(struct=i)
+                buildConstantArgumentMsg(i)
             )
-        else:
+        elif(isinstance(i, numbers.Number)):
             current_element.arguments.append(
-                basicMsg.ArgumentMsg(constant=str(i))
+                buildConstantArgumentMsg(i)
+            )
+        elif(type(i) is str):
+            current_element.arguments.append(
+                buildConstantArgumentMsg(i)
             )
         current_element.arguments.append(
                 last_element
             )
-        last_element = basicMsg.ArgumentMsg(
-            struct = current_element
-        )
+        last_element = buildConstantArgumentMsg(current_element)
     return last_element
       
 def stringsConverter(x):
     if(type(x) is bytes):
-        return x.decode('utf-8')
+        return str(x.decode('utf-8'))
     else:
-        return str(x)
+        return float(x)
+
+def buildConstantArgumentMsg(value):
+    if(type(value) is str):
+        return basicMsg.ArgumentMsg(atom=value)
+    if(type(value) is basicMsg.StructMsg):
+        return basicMsg.ArgumentMsg(struct=value)
+    if(type(value) is bool):
+        return basicMsg.ArgumentMsg(flag=value)
+    if(isinstance(value, numbers.Number)):
+        return basicMsg.ArgumentMsg(numeric=value)
```

### Comparing `prolog_primitives-0.4.2/prolog_primitives/basic/filterKbPrimitive.py` & `prolog_primitives-1.0.1/prolog_primitives/basic/filterKbPrimitive.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from prolog_primitives.basic import DistributedElements
 from prolog_primitives.generatedProto import primitiveService_pb2 as primitiveMsg
-from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
 
 class __FilterKBPrimitive(DistributedElements.DistributedPrimitive):
     
     def solve(self, request: DistributedElements.DistributedRequest) -> Generator[DistributedElements.DistributedResponse, None, None]:
         arg0 = request.arguments[0]
@@ -14,15 +13,15 @@
                 primitiveMsg.InspectKbMsg.STATIC,
                 [(primitiveMsg.InspectKbMsg.STARTS_WITH, str(Utils.parseArgumentMsg(arg0)))]):
                 
                 if(i == None):
                     yield request.replyFail()
                 else:
                     substitutions = {}
-                    substitutions[arg1.var] = basicMsg.ArgumentMsg(struct=i)
+                    substitutions[arg1.var] = Utils.buildConstantArgumentMsg(i)
                     yield request.replySuccess(
                         substitutions=substitutions
                     )
         else:
             yield request.replyFail()
             
 filterKBPrimitive = DistributedElements.DistributedPrimitiveWrapper("filterKB", 2, __FilterKBPrimitive())
```

### Comparing `prolog_primitives-0.4.2/prolog_primitives/basic/ntPrimitive.py` & `prolog_primitives-1.0.1/prolog_primitives/basic/ntPrimitive.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-from prolog_primitives.basic import DistributedElements
-from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
+from prolog_primitives.basic import DistributedElements, Utils
 from typing import Generator
 
 # this is the main module of your app
 # it is only required if your project must be runnable
 # this is the script to be executed whenever some users writes `python -m python-Primitives-Server` on the command line, eg.
 class NtPrimitive(DistributedElements.DistributedPrimitive):
     
     def solve(self, request: DistributedElements.DistributedRequest) -> Generator[DistributedElements.DistributedResponse, None, None]:
         arg0 = request.arguments[0]
         if(arg0.HasField("var")):
             n = 0
             while(True):
                 substitutions = {}
-                substitutions[arg0.var] = basicMsg.ArgumentMsg(constant=str(n))
+                substitutions[arg0.var] = Utils.buildConstantArgumentMsg(n)
                 yield request.replySuccess(substitutions = substitutions)
                 n += 1
-        elif(arg0.HasField("constant") and arg0.constant.isdigit()):
+        elif(arg0.HasField("numeric")):
             yield request.replySuccess(hasNext = False)
         else:
             yield request.replyFail()
```

### Comparing `prolog_primitives-0.4.2/prolog_primitives/ml_lib/collections.py` & `prolog_primitives-1.0.1/prolog_primitives/ml_lib/collections.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.2/prolog_primitives/ml_lib/dataset/cell.py` & `prolog_primitives-1.0.1/prolog_primitives/ml_lib/dataset/cell.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from prolog_primitives.basic import DistributedElements
-from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
 from ..collections import SharedCollections
 import tensorflow as tf
 
 class __CellPrimitive(DistributedElements.DistributedPrimitive):
     
@@ -16,61 +15,61 @@
         if(not dataset_ref.HasField("var") and values.HasField("var")):
             dataset = SharedCollections().getDataset(str(Utils.parseArgumentMsg(dataset_ref)))
                 
             #Specific cell
             if(not row_index.HasField("var") and not column_index.HasField("var")): 
                 row_index = int(Utils.parseArgumentMsg(row_index))
                 column_index = Utils.parseArgumentMsg(column_index)
-                if(column_index.isdigit()):
+                if(type(column_index) is not str):
                     column_index = dataset.column_names[int(column_index)]
                 value = Utils.stringsConverter(tf.get_static_value(dataset[row_index][column_index]))
                 yield request.replySuccess({
-                    values.var: basicMsg.ArgumentMsg(constant=value)
+                    values.var: Utils.buildConstantArgumentMsg(value)
                 }, hasNext=False)
             
             #Cells in specific column    
             elif(not column_index.HasField("var")): 
                 column_index = Utils.parseArgumentMsg(column_index)
-                if(column_index.isdigit()):
+                if(type(column_index) is not str):
                     column_index = dataset.column_names[int(column_index)]
                 i = 0
                 while(i < dataset.shape[0]):  
                     value = Utils.stringsConverter(tf.get_static_value(dataset[i][column_index]))
                     i += 1
                     yield request.replySuccess({
-                        row_index.var: basicMsg.ArgumentMsg(constant=str(i)),
-                        values.var: basicMsg.ArgumentMsg(constant=value)
+                        row_index.var: Utils.buildConstantArgumentMsg(i),
+                        values.var: Utils.buildConstantArgumentMsg(value)
                     }, hasNext=i < dataset.shape[0])
                     
             #Cells in specific row        
             elif(not row_index.HasField("var")): 
                 row_index = int(Utils.parseArgumentMsg(row_index))
                 i = 0
                 while(i < dataset.shape[1]):  
                     name = dataset.column_names[i]
                     
                     value = Utils.stringsConverter(tf.get_static_value(dataset[row_index][name]))
                     i += 1
                     yield request.replySuccess({
-                        column_index.var: basicMsg.ArgumentMsg(constant=name),
-                        values.var: basicMsg.ArgumentMsg(constant=value)
+                        column_index.var: Utils.buildConstantArgumentMsg(name),
+                        values.var: Utils.buildConstantArgumentMsg(value)
                     }, hasNext=i < dataset.shape[1])
                     
             #All Cells      
             else:
                 col = 0
                 while(col < dataset.shape[1]):
                     name = dataset.column_names[col]
                     row = 0
                     while(row < dataset.shape[0]): 
                         value = Utils.stringsConverter(tf.get_static_value(dataset[row][name]))
                         yield request.replySuccess({
-                            row_index.var: basicMsg.ArgumentMsg(constant=str(row)),
-                            column_index.var: basicMsg.ArgumentMsg(constant=name),
-                            values.var: basicMsg.ArgumentMsg(constant=value)
+                            row_index.var: Utils.buildConstantArgumentMsg(row),
+                            column_index.var: Utils.buildConstantArgumentMsg(name),
+                            values.var: Utils.buildConstantArgumentMsg(value)
                         }, hasNext = (row+1, col+1) != dataset.shape)
                         row += 1   
                     col +=1                        
                 
         else:
             yield request.replyFail()
```

### Comparing `prolog_primitives-0.4.2/prolog_primitives/ml_lib/dataset/column.py` & `prolog_primitives-1.0.1/prolog_primitives/ml_lib/dataset/column.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from prolog_primitives.basic import DistributedElements
-from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
 from ..collections import SharedCollections
 import tensorflow as tf
 
 class __ColumnPrimitive(DistributedElements.DistributedPrimitive):
     
@@ -13,29 +12,29 @@
         values = request.arguments[2]
         
         if(not dataset_ref.HasField("var") and values.HasField("var")):
             dataset = SharedCollections().getDataset(str(Utils.parseArgumentMsg(dataset_ref)))
                 
             if(not column.HasField("var")): 
                 i = Utils.parseArgumentMsg(column)
-                if(i.isdigit()):
+                if(type(i) is not str):
                     i = dataset.column_names[int(i)]
                 column = list(map(Utils.stringsConverter, tf.get_static_value(dataset[i])))
                 yield request.replySuccess({
                     values.var: Utils.fromListToArgumentMsg(column)
                 }, hasNext=False)
             else:
                 i = 0
                 while(i < dataset.shape[1]):
                     name = dataset.column_names[i]
                     col = list(map(Utils.stringsConverter, tf.get_static_value(dataset[name])))
                     i += 1
                     yield request.replySuccess({
-                        column.var: basicMsg.ArgumentMsg(constant=name),
+                        column.var: Utils.buildConstantArgumentMsg(name),
                         values.var: Utils.fromListToArgumentMsg(col)
-                    }, hasNext= (i < dataset.shape[1]))
+                    }, hasNext = (i < dataset.shape[1]))
                 
         else:
             yield request.replyFail()
             
             
 columnPrimitive = DistributedElements.DistributedPrimitiveWrapper("column", 3, __ColumnPrimitive())
```

### Comparing `prolog_primitives-0.4.2/prolog_primitives/ml_lib/dataset/fold.py` & `prolog_primitives-1.0.1/prolog_primitives/ml_lib/dataset/randomSplit.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 from prolog_primitives.basic import DistributedElements
-from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
 from ..collections import SharedCollections
-from sklearn.model_selection import KFold
-import numpy as np
+from datasets import Dataset
 
-class __FoldPrimitive(DistributedElements.DistributedPrimitive):
+class __RandomSplitPrimitive(DistributedElements.DistributedPrimitive):
     
     def solve(self, request: DistributedElements.DistributedRequest) -> Generator[DistributedElements.DistributedResponse, None, None]:
         dataset_ref = request.arguments[0]
-        k = request.arguments[1]
+        ratio = request.arguments[1]
         train_ref = request.arguments[2]
         val_ref = request.arguments[3]
-        if(not dataset_ref.HasField("var") and not k.HasField("var") and 
+        if(not dataset_ref.HasField("var") and not ratio.HasField("var") and 
            train_ref.HasField("var") and val_ref.HasField("var")):
             datasetId = str(Utils.parseArgumentMsg(dataset_ref))
             schemaId = SharedCollections().getSchemaIdFromDataset(datasetId)
-            dataset = SharedCollections().getDataset(datasetId)
-            k = int(Utils.parseArgumentMsg(k))
-            for kfold, (train, test) in enumerate(KFold(n_splits=k, 
-                                shuffle=True).split(dataset)):
-                train_ds = dataset[train]   
-                val_ds = dataset[test]
-                
-                
-                train_id = SharedCollections().addDataset(train_ds, schemaId)
-                val_id = SharedCollections().addDataset(val_ds, schemaId)
+            dataset: Dataset = SharedCollections().getDataset(datasetId)
+            ratio = float(Utils.parseArgumentMsg(ratio))
+            train_size = int(ratio * len(list(dataset)))
+        
+            shuffled = dataset.shuffle()
+            train_ds = shuffled[:train_size]
+            val_ds = dataset[train_size:]
             
-                yield request.replySuccess(substitutions={
-                    train_ref.var: basicMsg.ArgumentMsg(constant=train_id),
-                    val_ref.var: basicMsg.ArgumentMsg(constant=val_id)
-                    }, hasNext= kfold + 1 < k)
+            train_id = SharedCollections().addDataset(train_ds, schemaId)
+            val_id = SharedCollections().addDataset(val_ds, schemaId)
+            
+            yield request.replySuccess(substitutions={
+                train_ref.var: Utils.buildConstantArgumentMsg(train_id),
+                val_ref.var: Utils.buildConstantArgumentMsg(val_id)
+                }, hasNext=False)
         else:
             yield request.replyFail()
             
-foldPrimitive = DistributedElements.DistributedPrimitiveWrapper("fold", 4, __FoldPrimitive())
+randomSplitPrimitive = DistributedElements.DistributedPrimitiveWrapper("random_split", 4, __RandomSplitPrimitive())
```

### Comparing `prolog_primitives-0.4.2/prolog_primitives/ml_lib/dataset/randomSplit.py` & `prolog_primitives-1.0.1/prolog_primitives/ml_lib/predictors/predict.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,60 @@
 from prolog_primitives.basic import DistributedElements
-from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
 from ..collections import SharedCollections
+import tensorflow as tf
 from datasets import Dataset
 
-class __RandomSplitPrimitive(DistributedElements.DistributedPrimitive):
+class __Predict(DistributedElements.DistributedPrimitive):
     
     def solve(self, request: DistributedElements.DistributedRequest) -> Generator[DistributedElements.DistributedResponse, None, None]:
-        dataset_ref = request.arguments[0]
-        ratio = request.arguments[1]
-        train_ref = request.arguments[2]
-        val_ref = request.arguments[3]
-        if(not dataset_ref.HasField("var") and not ratio.HasField("var") and 
-           train_ref.HasField("var") and val_ref.HasField("var")):
-            datasetId = str(Utils.parseArgumentMsg(dataset_ref))
-            schemaId = SharedCollections().getSchemaIdFromDataset(datasetId)
-            dataset: Dataset = SharedCollections().getDataset(datasetId)
-            ratio = float(Utils.parseArgumentMsg(ratio))
-            train_size = int(ratio * len(list(dataset)))
+        predictor_ref = request.arguments[0]
+        dataset_ref = request.arguments[1]
+        prediction_ref = request.arguments[2]
         
-            shuffled = dataset.shuffle()
-            train_ds = shuffled[:train_size]
-            val_ds = dataset[train_size:]
+        if(not predictor_ref.HasField('var') and not dataset_ref.HasField('var') and
+           prediction_ref.HasField('var')):
+            model: tf.keras.Model = SharedCollections().getModel(Utils.parseArgumentMsg(predictor_ref))
+            
+            data = None
+            
+            datasetId = Utils.parseArgumentMsg(dataset_ref)
+            dataset: Dataset = SharedCollections().getDataset(datasetId)
+            if(dataset != None):
+                schemaId = SharedCollections().getSchemaIdFromDataset(datasetId)
+                schema = SharedCollections().getSchema(schemaId)
+                for attr in dataset.column_names:
+                    if(not attr in schema.targets):
+                        if(data == None):
+                            data = tf.cast(dataset[attr], tf.float32)
+                        else:
+                            data = tf.stack([data, tf.cast(dataset[attr], tf.float32)], axis = 1)
+                            
+                
+                result = {}
+                for attr in schema.targets:
+                    result[attr] = []
+                
+                for row in model.predict(x=data):
+                    for attr, y in zip(schema.targets, row):
+                        result[attr].append(y)
+
+                dataset = Dataset.from_dict(result).with_format("tf")
+                datasetId = SharedCollections().addDataset(dataset, schemaId)
             
-            train_id = SharedCollections().addDataset(train_ds, schemaId)
-            val_id = SharedCollections().addDataset(val_ds, schemaId)
+                yield request.replySuccess(substitutions={
+                    prediction_ref.var: Utils.buildConstantArgumentMsg(datasetId)
+                    }, hasNext=False)
+            else:
+                row = [float(x) for x in Utils.parseArgumentMsg(dataset_ref).arguments]
+                data = tf.constant(value=[row], dtype=tf.float32)
             
-            yield request.replySuccess(substitutions={
-                train_ref.var: basicMsg.ArgumentMsg(constant=train_id),
-                val_ref.var: basicMsg.ArgumentMsg(constant=val_id)
-                }, hasNext=False)
+                result = model.predict(x=data)[0]
+                
+                yield request.replySuccess(substitutions={
+                    prediction_ref.var: Utils.fromListToArgumentMsg(result.tolist())
+                    }, hasNext=False)
         else:
             yield request.replyFail()
-            
-randomSplitPrimitive = DistributedElements.DistributedPrimitiveWrapper("random_split", 4, __RandomSplitPrimitive())
+             
+predictPrimitive = DistributedElements.DistributedPrimitiveWrapper("predict", 3, __Predict())
```

### Comparing `prolog_primitives-0.4.2/prolog_primitives/ml_lib/dataset/row.py` & `prolog_primitives-1.0.1/prolog_primitives/ml_lib/dataset/row.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from prolog_primitives.basic import DistributedElements
-from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
 from ..collections import SharedCollections
 import tensorflow as tf
 
 class __RowPrimitive(DistributedElements.DistributedPrimitive):
     
@@ -28,15 +27,15 @@
             else:
                 i = 0
                 while(i < dataset.shape[0]):
                     row = getRow(i)
                     i += 1
                     yield request.replySuccess(
                         substitutions={
-                            index.var: basicMsg.ArgumentMsg(constant=str(i)),
+                            index.var: Utils.buildConstantArgumentMsg(i),
                             values.var: Utils.fromListToArgumentMsg(row)
                             }, hasNext = (i < dataset.shape[0]))
         else:
             yield request.replyFail()
             
             
 rowPrimitive = DistributedElements.DistributedPrimitiveWrapper("row", 3, __RowPrimitive())
```

### Comparing `prolog_primitives-0.4.2/prolog_primitives/ml_lib/dataset/theoryToDataset.py` & `prolog_primitives-1.0.1/prolog_primitives/ml_lib/dataset/theoryToDataset.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,14 +37,14 @@
                             raise Exception("Wrong typecasting in attributes")
                         else:
                             data[j[0].name].append(value)
             
             dataset = Dataset.from_dict(data).with_format("tf")
             datasetId = SharedCollections().addDataset(dataset, schemaId)
             yield request.replySuccess(substitutions={
-                dataset_ref.var: basicMsg.ArgumentMsg(constant=datasetId)
+                dataset_ref.var: Utils.buildConstantArgumentMsg(datasetId)
                 }, hasNext=False)
         else:
             yield request.replyFail()
             
             
 theoryToDatasetPrimitive = DistributedElements.DistributedPrimitiveWrapper("theory_to_dataset", 2, __TheoryToDatasetPrimitive())
```

### Comparing `prolog_primitives-0.4.2/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py` & `prolog_primitives-1.0.1/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,69 +6,65 @@
 from ..collections import SharedCollections
 import tensorflow as tf
 
 def wrapInClause(struct: basicMsg.StructMsg):
     finalStruct = basicMsg.StructMsg(
         functor = ":-"
     )
-    finalStruct.arguments.append(basicMsg.ArgumentMsg(struct=struct))
-    finalStruct.arguments.append(basicMsg.ArgumentMsg(constant="true"))
+    finalStruct.arguments.append(Utils.buildConstantArgumentMsg(struct))
+    finalStruct.arguments.append(Utils.buildConstantArgumentMsg(True))
     return finalStruct
 
 class __TheoryFromDatasetPrimitive(DistributedElements.DistributedPrimitive):
     
     def solve(self, request: DistributedElements.DistributedRequest) -> Generator[DistributedElements.DistributedResponse, None, None]:
         schema_ref = request.arguments[0]
         dataset_ref = request.arguments[1]
         if(not schema_ref.HasField("var") and not dataset_ref.HasField("var")):  
             schema = SharedCollections().getSchema(Utils.parseArgumentMsg(schema_ref))
             dataset = SharedCollections().getDataset(Utils.parseArgumentMsg(dataset_ref))
             
             clauses = []
-            wrapInClause(
-                basicMsg.StructMsg(
-                    functor="schema_name",
-                    arguments=[basicMsg.ArgumentMsg(constant=schema.name)]
-            ))
             clauses.append(wrapInClause(
                 basicMsg.StructMsg(
                     functor="schema_name",
-                    arguments=[basicMsg.ArgumentMsg(constant=schema.name)]
+                    arguments=[Utils.buildConstantArgumentMsg(schema.name)]
             )))
             clauses.append(wrapInClause(
                 basicMsg.StructMsg(
                     functor="schema_target",
                     arguments=[Utils.fromListToArgumentMsg(schema.targets)]
             )))
             
             for i, attr in enumerate(schema.attributes):
                 clauses.append(wrapInClause(
                     basicMsg.StructMsg(
                         functor="attribute",
                         arguments=[
-                            basicMsg.ArgumentMsg(constant=str(i)),
-                            basicMsg.ArgumentMsg(constant=attr.name),
+                            Utils.buildConstantArgumentMsg(i),
+                            Utils.buildConstantArgumentMsg(attr.name),
                             attr.typeToArgumentMsg()]
                 )))
-                
+            
             for i in range(dataset.shape[0]):
                 values = list(map(
-                    lambda x: basicMsg.ArgumentMsg(constant = Utils.stringsConverter(x)),
+                    lambda x: Utils.buildConstantArgumentMsg(Utils.stringsConverter(x)),
                     [tf.get_static_value(x) for x in dataset[i].values()]))
                 clauses.append(wrapInClause(
                     basicMsg.StructMsg(
                         functor=schema.name,
                         arguments=values
                 )))
             
             yield request.replySuccess(
                 sideEffects = [SideEffectMsg(
                     clauses = SetClausesOfKBMsg(
                         kbType = SetClausesOfKBMsg.DYNAMIC,
                         operationType = SetClausesOfKBMsg.ADD, 
-                        clauses = clauses))],
+                        clauses = clauses
+                        ))],
                 hasNext=False)
         else:
             yield request.replyFail()
             
             
 theoryFromDatasetPrimitive = DistributedElements.DistributedPrimitiveWrapper("theory_from_dataset", 2, __TheoryFromDatasetPrimitive())
```

### Comparing `prolog_primitives-0.4.2/prolog_primitives/ml_lib/launcher.py` & `prolog_primitives-1.0.1/prolog_primitives/ml_lib/launcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,32 +27,36 @@
 def main():
     servers = []
     libraryName = "customLibrary"
 
     def launchPrimitive(primitive: DistributedElements.DistributedPrimitiveWrapper, port: int):
         server = PrimitiveWrapper.serve(primitive, port, libraryName)
         servers.append(server)
-        server.wait_for_termination()
+        #server.wait_for_termination()
         
     primitives = [schemaPrimitive, theoryToSchemaPrimitive,
                 theoryToDatasetPrimitive, randomSplitPrimitive,
                 rowPrimitive, columnPrimitive, cellPrimitive, foldPrimitive, 
                 theoryFromDatasetPrimitive, schemaTrasformation,
                 normalizePrimitive, one_hot_encodePrimitive, dropPrimitive,
                 fitPrimitive, transformPrimitive, inputLayerPrimitive,
                 denseLayerPrimitive, outputLayerPrimitive, neuralNetworkPrimitive,
                 trainPrimitive, predictPrimitive, classifyPrimitive, msePrimitive]
 
-    port = 8080
+    initialport = 8080
+    port = initialport
     executor = ThreadPoolExecutor(max_workers=len(primitives))
 
     for primitive in primitives:
-        future = executor.submit(launchPrimitive, primitive, port)
+        #future = executor.submit(launchPrimitive, primitive, port)
+        launchPrimitive(primitive, port)
         port += 1
 
+    print(f"Servers listening from {initialport} to {port-1}")
+
     try:
         for server in servers:
             server.wait_for_termination()
     except (Exception, KeyboardInterrupt, SystemExit) as inst:
         executor.shutdown(wait=False, cancel_futures=True)
         for server in servers:
             server.stop(0)
```

### Comparing `prolog_primitives-0.4.2/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py` & `prolog_primitives-1.0.1/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from prolog_primitives.basic import DistributedElements
-from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
 from ..collections import SharedCollections
 import tensorflow as tf
 
-class __DenseLayer(DistributedElements.DistributedPrimitive):
+class __OutputLayer(DistributedElements.DistributedPrimitive):
     
     def solve(self, request: DistributedElements.DistributedRequest) -> Generator[DistributedElements.DistributedResponse, None, None]:
         topology_in_ref = request.arguments[0]
         size = request.arguments[1]
         activation = request.arguments[2]
         topology_out_ref = request.arguments[3]
         
@@ -17,22 +16,21 @@
            not activation.HasField('var') and topology_out_ref.HasField('var')):
             topology: list = SharedCollections().getTopology(Utils.parseArgumentMsg(topology_in_ref))
             
             activation = str(Utils.parseArgumentMsg(activation))
             if(activation == "identity"):
                 activation = None
 
-            dense = tf.keras.layers.Dense(
+            output = tf.keras.layers.Dense(
                 units=int(Utils.parseArgumentMsg(size)),
                 activation=activation,
-                name="dense_"+str(len(topology)))
-            topology.append(dense)
-            
+                name="output")
+            topology.append(output)
             id = SharedCollections().addTopology(topology)
             yield request.replySuccess(substitutions={
-                topology_out_ref.var: basicMsg.ArgumentMsg(constant=id)
+                topology_out_ref.var: Utils.buildConstantArgumentMsg(id)
                 }, hasNext=False)
         else:
             yield request.replyFail()
             
             
-denseLayerPrimitive = DistributedElements.DistributedPrimitiveWrapper("dense_layer", 4, __DenseLayer())
+outputLayerPrimitive = DistributedElements.DistributedPrimitiveWrapper("output_layer", 4, __OutputLayer())
```

### Comparing `prolog_primitives-0.4.2/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py` & `prolog_primitives-1.0.1/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from prolog_primitives.basic import DistributedElements
-from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
 from ..collections import SharedCollections
 import tensorflow as tf
 from datasets import Dataset
 
 class __InputLayer(DistributedElements.DistributedPrimitive):
@@ -12,14 +11,14 @@
         size = request.arguments[0]
         topology_ref = request.arguments[1]
         
         if(not size.HasField('var') and topology_ref.HasField('var')):
             size = int(Utils.parseArgumentMsg(size))
             id = SharedCollections().addTopology([tf.keras.Input(shape=(size,), name="input")])
             yield request.replySuccess(substitutions={
-                topology_ref.var: basicMsg.ArgumentMsg(constant=id)
+                topology_ref.var: Utils.buildConstantArgumentMsg(id)
                 }, hasNext=False)
         else:
             yield request.replyFail()
             
             
 inputLayerPrimitive = DistributedElements.DistributedPrimitiveWrapper("input_layer", 2, __InputLayer())
```

### Comparing `prolog_primitives-0.4.2/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py` & `prolog_primitives-1.0.1/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from prolog_primitives.basic import DistributedElements
-from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
 from ..collections import SharedCollections
 import tensorflow as tf
 from datasets import Dataset
 
 class __NeuralNetwork(DistributedElements.DistributedPrimitive):
@@ -21,14 +20,14 @@
             
             model = tf.keras.Model(
                 inputs=[topology[0]], outputs = [output]
             )
             
             id = SharedCollections().addModel(model)
             yield request.replySuccess(substitutions={
-                predictor_ref.var: basicMsg.ArgumentMsg(constant=id)
+                predictor_ref.var: Utils.buildConstantArgumentMsg(id)
                 }, hasNext=False)
         else:
             yield request.replyFail()
             
             
 neuralNetworkPrimitive = DistributedElements.DistributedPrimitiveWrapper("neural_network", 2, __NeuralNetwork())
```

### Comparing `prolog_primitives-0.4.2/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py` & `prolog_primitives-1.0.1/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from prolog_primitives.basic import DistributedElements
-from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
 from ..collections import SharedCollections
 import tensorflow as tf
 
-class __OutputLayer(DistributedElements.DistributedPrimitive):
+class __DenseLayer(DistributedElements.DistributedPrimitive):
     
     def solve(self, request: DistributedElements.DistributedRequest) -> Generator[DistributedElements.DistributedResponse, None, None]:
         topology_in_ref = request.arguments[0]
         size = request.arguments[1]
         activation = request.arguments[2]
         topology_out_ref = request.arguments[3]
         
@@ -17,21 +16,22 @@
            not activation.HasField('var') and topology_out_ref.HasField('var')):
             topology: list = SharedCollections().getTopology(Utils.parseArgumentMsg(topology_in_ref))
             
             activation = str(Utils.parseArgumentMsg(activation))
             if(activation == "identity"):
                 activation = None
 
-            output = tf.keras.layers.Dense(
+            dense = tf.keras.layers.Dense(
                 units=int(Utils.parseArgumentMsg(size)),
                 activation=activation,
-                name="output")
-            topology.append(output)
+                name="dense_"+str(len(topology)))
+            topology.append(dense)
+            
             id = SharedCollections().addTopology(topology)
             yield request.replySuccess(substitutions={
-                topology_out_ref.var: basicMsg.ArgumentMsg(constant=id)
+                topology_out_ref.var: Utils.buildConstantArgumentMsg(id)
                 }, hasNext=False)
         else:
             yield request.replyFail()
             
             
-outputLayerPrimitive = DistributedElements.DistributedPrimitiveWrapper("output_layer", 4, __OutputLayer())
+denseLayerPrimitive = DistributedElements.DistributedPrimitiveWrapper("dense_layer", 4, __DenseLayer())
```

### Comparing `prolog_primitives-0.4.2/prolog_primitives/ml_lib/predictors/classify.py` & `prolog_primitives-1.0.1/prolog_primitives/ml_lib/predictors/classify.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from prolog_primitives.basic import DistributedElements
-from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
 from ..collections import SharedCollections
-import tensorflow as tf
 from datasets import Dataset
 
 
 
 class __Classify(DistributedElements.DistributedPrimitive):
     
     def solve(self, request: DistributedElements.DistributedRequest) -> Generator[DistributedElements.DistributedResponse, None, None]:
@@ -49,23 +47,23 @@
                     classification.append(classify(row.values()))
                     
                 
                     
                 dataset = Dataset.from_dict({"labels":classification}).with_format("tf")
                 datasetId = SharedCollections().addDataset(dataset, None)
                 yield request.replySuccess(substitutions={
-                    classification_ref.var: basicMsg.ArgumentMsg(constant=datasetId)
+                    classification_ref.var: Utils.buildConstantArgumentMsg(datasetId)
                     }, hasNext=False)
             else:
                 row = [float(x) for x in Utils.parseArgumentMsgList(prediction_ref)]
                 result = classify(row)
                 if(type(result) == list):
                     result = Utils.fromListToArgumentMsg(result)
                 else:
-                    result = basicMsg.ArgumentMsg(constant=result)
+                    result = Utils.buildConstantArgumentMsg(result)
                 
                 yield request.replySuccess(substitutions={
                     classification_ref.var: result
                     }, hasNext=False)
 
         else:
             yield request.replyFail()
```

### Comparing `prolog_primitives-0.4.2/prolog_primitives/ml_lib/predictors/predict.py` & `prolog_primitives-1.0.1/prolog_primitives/ml_lib/predictors/train.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,61 +1,77 @@
 from prolog_primitives.basic import DistributedElements
-from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
 from ..collections import SharedCollections
 import tensorflow as tf
 from datasets import Dataset
 
-class __Predict(DistributedElements.DistributedPrimitive):
+def parseParams(structs: list[Utils.Struct]):
+    params = {
+        "epoch": 1,
+        "loss": "mse",
+        "batch": None,
+        "learning_rate": 0.001
+    }
+    for struct in structs:
+        if(struct.functor == "max_epoch"):
+            params['epoch'] = int(struct.arguments[0])
+        elif(struct.functor == "batch_size"):
+            params['batch'] = int(struct.arguments[0])
+        elif(struct.functor == "learning_rate"):
+            params['learning_rate'] = float(struct.arguments[0])
+        elif(struct.functor == "loss"):
+            loss = struct.arguments[0]
+            if(loss == "mse"):
+                params['loss'] = "mse"
+            elif(loss == "mae"):
+                params['loss'] = "mae"
+            elif(loss == "cross_entropy"):
+                params['loss'] = tf.keras.losses.BinaryCrossentropy()
+    return params
+
+class __Train(DistributedElements.DistributedPrimitive):
     
     def solve(self, request: DistributedElements.DistributedRequest) -> Generator[DistributedElements.DistributedResponse, None, None]:
-        predictor_ref = request.arguments[0]
+        predictor_in_ref = request.arguments[0]
         dataset_ref = request.arguments[1]
-        prediction_ref = request.arguments[2]
+        params = request.arguments[2]
+        predictor_out_ref = request.arguments[3]
         
-        if(not predictor_ref.HasField('var') and not dataset_ref.HasField('var') and
-           prediction_ref.HasField('var')):
-            model: tf.keras.Model = SharedCollections().getModel(Utils.parseArgumentMsg(predictor_ref))
-            
-            data = None
-            
+        if(not predictor_in_ref.HasField('var') and not dataset_ref.HasField('var') and
+           not params.HasField('var') and predictor_out_ref.HasField('var')):
+            model: tf.keras.Model = SharedCollections().getModel(Utils.parseArgumentMsg(predictor_in_ref))
             datasetId = Utils.parseArgumentMsg(dataset_ref)
             dataset: Dataset = SharedCollections().getDataset(datasetId)
-            if(dataset != None):
-                schemaId = SharedCollections().getSchemaIdFromDataset(datasetId)
-                schema = SharedCollections().getSchema(schemaId)
-                for attr in dataset.column_names:
-                    if(not attr in schema.targets):
-                        if(data == None):
-                            data = tf.cast(dataset[attr], tf.float32)
-                        else:
-                            data = tf.stack([data, tf.cast(dataset[attr], tf.float32)], axis = 1)
-                            
-                
-                result = {}
-                for attr in schema.targets:
-                    result[attr] = []
-                
-                for row in model.predict(x=data):
-                    for attr, y in zip(schema.targets, row):
-                        result[attr].append(y)
-
-                dataset = Dataset.from_dict(result).with_format("tf")
-                datasetId = SharedCollections().addDataset(dataset, schemaId)
+            schema = SharedCollections().getSchema(SharedCollections().getSchemaIdFromDataset(datasetId))
+            params = parseParams(Utils.parseArgumentMsg(params))
+            
+            input = None
+            output = None
+            for attr in dataset.column_names:
+                if(attr in schema.targets):
+                    if(output == None):
+                        output = tf.cast(dataset[attr], tf.float32)
+                    else:
+                        output = tf.stack([output, tf.cast(dataset[attr], tf.float32)], axis = 1)
+                else:
+                    if(input == None):
+                        input = tf.cast(dataset[attr], tf.float32)
+                    else:
+                        input = tf.stack([input, tf.cast(dataset[attr], tf.float32)], axis = 1)
+            optimizer = tf.keras.optimizers.Adam(learning_rate=params["learning_rate"])
+            model.compile(
+                loss = params["loss"],
+                optimizer=optimizer,
+                metrics=[tf.keras.metrics.CategoricalAccuracy()],
+            )
             
-                yield request.replySuccess(substitutions={
-                    prediction_ref.var: basicMsg.ArgumentMsg(constant=datasetId)
-                    }, hasNext=False)
-            else:
-                row = [float(x) for x in Utils.parseArgumentMsg(dataset_ref).arguments]
-                data = tf.constant(value=[row], dtype=tf.float32)
+            model.fit(x=input,y=output, batch_size=params["batch"], epochs=params["epoch"])
             
-                result = model.predict(x=data)[0]
-                
-                yield request.replySuccess(substitutions={
-                    prediction_ref.var: Utils.fromListToArgumentMsg(result.tolist())
-                    }, hasNext=False)
+            id = SharedCollections().addModel(model)
+            yield request.replySuccess(substitutions={
+                predictor_out_ref.var: Utils.buildConstantArgumentMsg(id)
+                }, hasNext=False)
         else:
             yield request.replyFail()
              
-predictPrimitive = DistributedElements.DistributedPrimitiveWrapper("predict", 3, __Predict())
+trainPrimitive = DistributedElements.DistributedPrimitiveWrapper("train", 4, __Train())
```

### Comparing `prolog_primitives-0.4.2/prolog_primitives/ml_lib/predictors/score.py` & `prolog_primitives-1.0.1/prolog_primitives/ml_lib/predictors/score.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from prolog_primitives.basic import DistributedElements
-from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
 from ..collections import SharedCollections
 import tensorflow as tf
-from datasets import Dataset
 from abc import ABC, abstractmethod
 
 
 
 class __AssessTemplate(DistributedElements.DistributedPrimitive, ABC):
     
     @abstractmethod
@@ -49,15 +47,15 @@
             scores = []   
             for (attr, y1), y2 in zip(y_true.items(), y_pred):
                 scores.append(self.evaluator(y1, y2))
             
             totalscore = tf.get_static_value(sum(scores)/len(scores))
                             
             yield request.replySuccess(substitutions={
-                score.var: basicMsg.ArgumentMsg(constant=str(totalscore))
+                score.var:Utils.buildConstantArgumentMsg(totalscore)
             }, hasNext=False)
 
         else:
             yield request.replyFail()
             
 class __Mse(__AssessTemplate):
```

### Comparing `prolog_primitives-0.4.2/prolog_primitives/ml_lib/schema/schema.py` & `prolog_primitives-1.0.1/prolog_primitives/ml_lib/schema/schema.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,22 +13,22 @@
         attributes = request.arguments[2]
         targets = request.arguments[3]
 
         #First Case of only retrieving infos on existing schema
         if(not schema_ref.HasField("var") and schema_name.HasField("var") and attributes.HasField("var") and targets.HasField("var")):
             schema: Schema = SharedCollections().getSchema(str(Utils.parseArgumentMsg(schema_ref)))
             if(schema != None):
-                name_fact = basicMsg.ArgumentMsg(constant = schema.name)
+                name_fact = Utils.buildConstantArgumentMsg(schema.name)
                 attributes_facts = list[basicMsg.StructMsg]()
                 i: int = 0
                 
                 for attr in schema.attributes:
                     attribute = [
-                        basicMsg.ArgumentMsg(constant = str(i)),
-                        basicMsg.ArgumentMsg(constant = attr.name),
+                        Utils.buildConstantArgumentMsg(i),
+                        Utils.buildConstantArgumentMsg(attr.name),
                         attr.typeToArgumentMsg()
                     ]
                     attributes_facts.append(
                         basicMsg.StructMsg(
                             functor = "attribute",
                             arguments = attribute
                         )
@@ -49,13 +49,13 @@
                 attributesList.insert(int(attr.arguments[0]), parseAttributeFromStruct(attr))
             #Parsing targets
             targets =  Utils.parseArgumentMsgList(targets)
             targetsList = list(map(str, targets))
             id = SharedCollections().addSchema(
                 Schema(str(Utils.parseArgumentMsg(schema_name)), attributesList, targetsList))
             yield request.replySuccess(substitutions={
-                schema_ref.var:  basicMsg.ArgumentMsg(constant=id)
+                schema_ref.var:  Utils.buildConstantArgumentMsg(id)
             }, hasNext=False)
         else:
             yield request.replyFail()
             
 schemaPrimitive = DistributedElements.DistributedPrimitiveWrapper("schema", 4, __SchemaPrimitive())
```

### Comparing `prolog_primitives-0.4.2/prolog_primitives/ml_lib/schema/schemaClass.py` & `prolog_primitives-1.0.1/prolog_primitives/ml_lib/schema/schemaClass.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,52 +16,44 @@
         self.type = type
         self.vocab = vocab 
 
     def typeToArgumentMsg(self) -> basicMsg.ArgumentMsg:
         if(self.vocab != []):
             vocab_msg = Utils.fromListToArgumentMsg(self.vocab)
             if("int" in str(self.type)):    
-                return basicMsg.ArgumentMsg(
-                    struct = basicMsg.StructMsg(
+                return Utils.buildConstantArgumentMsg(
+                    basicMsg.StructMsg(
                         functor="ordinal",
                         arguments = [vocab_msg]
                     )
                 )
             else:
-                return basicMsg.ArgumentMsg(
-                    struct = basicMsg.StructMsg(
+                return Utils.buildConstantArgumentMsg(
+                    basicMsg.StructMsg(
                         functor="categorical",
                         arguments = [vocab_msg]
                     )
                 )
         if("int" in str(self.type)):
-            return basicMsg.ArgumentMsg(
-                constant="integer"
-            )
+            return Utils.buildConstantArgumentMsg("integer")
         elif("float" in str(self.type)):
-            return basicMsg.ArgumentMsg(
-                constant="real"
-            )
+            return Utils.buildConstantArgumentMsg("real")
         elif("str" in str(self.type)):
-            return basicMsg.ArgumentMsg(
-                constant="string"
-            )
+            return Utils.buildConstantArgumentMsg("string")
         elif("bool" in str(self.type)):
-            return basicMsg.ArgumentMsg(
-                constant="boolean"
-            )
+            return Utils.buildConstantArgumentMsg("boolean")
         
     def typeCastElement(self, element):
         if(self.vocab != []): 
             if(self.type == tf.string and element in self.vocab):
                 return element
             elif(self.type == tf.int64 and int(element) in self.vocab):
                 return int(element)
         elif(self.type == tf.int64):
-            return int(element)
+            return int(float(element))
         elif(self.type == tf.float64):
             return float(element)
         elif(self.type == tf.string):
             return element
         elif(self.type == tf.bool):
             return bool(element)
```

### Comparing `prolog_primitives-0.4.2/prolog_primitives/ml_lib/schema/theoryToSchema.py` & `prolog_primitives-1.0.1/prolog_primitives/ml_lib/schema/theoryToSchema.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from prolog_primitives.basic import DistributedElements
 from prolog_primitives.generatedProto import primitiveService_pb2 as primitiveMsg
-from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
 from .. import collections
 from .schemaClass import parseAttributeFromStruct
 
 class __TheoryToSchemaPrimitive(DistributedElements.DistributedPrimitive):
     
@@ -34,15 +33,15 @@
                 primitiveMsg.InspectKbMsg.STATIC,
                 [(primitiveMsg.InspectKbMsg.STARTS_WITH, "schema_target")]))
             if(targetFact == None):
                 yield request.replyFail()
             else:
                 targets = Utils.parseArgumentMsgList(targetFact.arguments[0].struct.arguments[0])
             substitutions = {
-                arg0.var: basicMsg.ArgumentMsg(constant=collections
+                arg0.var: Utils.buildConstantArgumentMsg(collections
                                                .SharedCollections()
                                                .addSchema(collections.Schema(schema_name, attributes, targets))) 
                 }
             yield request.replySuccess(substitutions, hasNext=False)
         else:
             request.replyFail()
```

### Comparing `prolog_primitives-0.4.2/prolog_primitives/ml_lib/transformations/drop.py` & `prolog_primitives-1.0.1/prolog_primitives/ml_lib/transformations/drop.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from prolog_primitives.basic import DistributedElements
-from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
 from ..collections import SharedCollections
 from .transformationClass import Dropper, Pipeline
 
 class __Drop(DistributedElements.DistributedPrimitive):
     
@@ -19,14 +18,14 @@
             if(listOfAttr != []):
                 attributes = listOfAttr
             else:
                 attributes = [Utils.parseArgumentMsg(attributes)]
                 
             id = SharedCollections().addPipeline(transf.append(dict.fromkeys(attributes, [Dropper()])))
             yield request.replySuccess(substitutions={
-                transf_out_ref.var: basicMsg.ArgumentMsg(constant=id)
+                transf_out_ref.var: Utils.buildConstantArgumentMsg(id)
                 }, hasNext=False)
         else:
             yield request.replyFail()
             
             
 dropPrimitive = DistributedElements.DistributedPrimitiveWrapper("drop", 3, __Drop())
```

### Comparing `prolog_primitives-0.4.2/prolog_primitives/ml_lib/transformations/fit.py` & `prolog_primitives-1.0.1/prolog_primitives/ml_lib/transformations/one_hot_encode.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 from prolog_primitives.basic import DistributedElements
-from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
 from ..collections import SharedCollections
-from .transformationClass import  Pipeline
-from datasets import Dataset
+from ..schema.schemaClass import Schema
+from .transformationClass import OneHotEncoder, Pipeline
 
-class __Fit(DistributedElements.DistributedPrimitive):
+class __One_Hot_Encode(DistributedElements.DistributedPrimitive):
     
     def solve(self, request: DistributedElements.DistributedRequest) -> Generator[DistributedElements.DistributedResponse, None, None]:
         transf_in_ref = request.arguments[0]
-        dataset_ref = request.arguments[1]
+        attributes = request.arguments[1]
         transf_out_ref = request.arguments[2]
         
-        if(not transf_in_ref.HasField('var') and not dataset_ref.HasField('var') and transf_out_ref.HasField('var')):
+        if(not transf_in_ref.HasField('var') and not attributes.HasField('var') and transf_out_ref.HasField('var')):
             transf: Pipeline = SharedCollections().getPipeline(Utils.parseArgumentMsg(transf_in_ref))
-            dataset: Dataset = SharedCollections().getDataset(Utils.parseArgumentMsg(dataset_ref))
+            schema: Schema = SharedCollections().getSchema(transf.originalSchemaId)
+            listOfAttr = Utils.parseArgumentMsgList(attributes)
+            if(listOfAttr != []):
+                attributes = listOfAttr
+            else:
+                attributes = [Utils.parseArgumentMsg(attributes)]
             
-            id = SharedCollections().addPipeline(transf.adapt(dataset))
+            layers = {}
+            for attr in attributes:
+                vocab = list(filter(lambda x: x.name == attr ,schema.attributes)).pop().vocab
+                layers[attr] = [OneHotEncoder(vocab)]
+            
+            id = SharedCollections().addPipeline(transf.append(layers))
             yield request.replySuccess(substitutions={
-                transf_out_ref.var: basicMsg.ArgumentMsg(constant=id)
+                transf_out_ref.var: Utils.buildConstantArgumentMsg(id)
                 }, hasNext=False)
         else:
             yield request.replyFail()
             
             
-fitPrimitive = DistributedElements.DistributedPrimitiveWrapper("fit", 3, __Fit())
+one_hot_encodePrimitive = DistributedElements.DistributedPrimitiveWrapper("one_hot_encode", 3, __One_Hot_Encode())
```

### Comparing `prolog_primitives-0.4.2/prolog_primitives/ml_lib/transformations/normalization.py` & `prolog_primitives-1.0.1/prolog_primitives/ml_lib/transformations/normalization.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from prolog_primitives.basic import DistributedElements
-from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
 from ..collections import SharedCollections
 from .transformationClass import Normalization, Pipeline
 
 class __Normalize(DistributedElements.DistributedPrimitive):
     
@@ -19,14 +18,14 @@
             if(listOfAttr != []):
                 attributes = listOfAttr
             else:
                 attributes = [Utils.parseArgumentMsg(attributes)]
             
             id = SharedCollections().addPipeline(transf.append(dict.fromkeys(attributes, [Normalization()])))
             yield request.replySuccess(substitutions={
-                transf_out_ref.var: basicMsg.ArgumentMsg(constant=id)
+                transf_out_ref.var: Utils.buildConstantArgumentMsg(id)
                 }, hasNext=False)
         else:
             yield request.replyFail()
             
             
 normalizePrimitive = DistributedElements.DistributedPrimitiveWrapper("normalize", 3, __Normalize())
```

### Comparing `prolog_primitives-0.4.2/prolog_primitives/ml_lib/transformations/schema_trasformation.py` & `prolog_primitives-1.0.1/prolog_primitives/ml_lib/transformations/schema_trasformation.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 from prolog_primitives.basic import DistributedElements
-from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
 from ..collections import SharedCollections
-import tensorflow as tf
 from .transformationClass import Pipeline
 
 class __SchemaTrasformation(DistributedElements.DistributedPrimitive):
     
     def solve(self, request: DistributedElements.DistributedRequest) -> Generator[DistributedElements.DistributedResponse, None, None]:
         schema_ref = request.arguments[0]
         transf_ref = request.arguments[1]
         
         if(not schema_ref.HasField('var') and transf_ref.HasField('var')):
             schema_id = Utils.parseArgumentMsg(schema_ref)
             
             id = SharedCollections().addPipeline(Pipeline(schema_id))
             yield request.replySuccess(substitutions={
-                transf_ref.var: basicMsg.ArgumentMsg(constant=id)
+                transf_ref.var: Utils.buildConstantArgumentMsg(id)
                 }, hasNext=False)
         elif(schema_ref.HasField('var') and not transf_ref.HasField('var')):
             transformation_id = Utils.parseArgumentMsg(transf_ref)
             transformation: Pipeline = SharedCollections().getPipeline(transformation_id)
             
             id = SharedCollections().addSchema(transformation.computeFinalSchema())
             yield request.replySuccess(substitutions = {
-                schema_ref.var: basicMsg.ArgumentMsg(constant=id)
+                schema_ref.var: Utils.buildConstantArgumentMsg(id)
             }, hasNext=False)            
         else:
             yield request.replyFail()
             
             
 schemaTrasformation = DistributedElements.DistributedPrimitiveWrapper("schema_trasformation", 2, __SchemaTrasformation())
```

### Comparing `prolog_primitives-0.4.2/prolog_primitives/ml_lib/transformations/transform.py` & `prolog_primitives-1.0.1/prolog_primitives/ml_lib/transformations/transform.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from prolog_primitives.basic import DistributedElements
-from prolog_primitives.generatedProto import basicMessages_pb2 as basicMsg
 from typing import Generator
 from prolog_primitives.basic import Utils
 from ..collections import SharedCollections
 from .transformationClass import Pipeline
 from datasets import Dataset
 
 class __Transform(DistributedElements.DistributedPrimitive):
@@ -19,22 +18,22 @@
             if(not dataset_in_ref.HasField("var") and dataset_out_ref.HasField("var")):
                 dataset_in: Dataset = SharedCollections().getDataset(Utils.parseArgumentMsg(dataset_in_ref))
                 schemaId = SharedCollections().addSchema(transf.computeFinalSchema())
                 dataset_out = transf.apply(dataset_in)
                 id = SharedCollections().addDataset(dataset_out, schemaId)
 
                 yield request.replySuccess(substitutions={
-                    dataset_out_ref.var: basicMsg.ArgumentMsg(constant=id)
+                    dataset_out_ref.var: Utils.buildConstantArgumentMsg(id)
                     }, hasNext=False)
             elif(dataset_in_ref.HasField("var") and not dataset_out_ref.HasField("var")):
                 dataset_out: Dataset = SharedCollections().getDataset(Utils.parseArgumentMsg(dataset_out_ref))
                 dataset_in: Dataset = transf.invert(dataset_out)
                 id = SharedCollections().addDataset(dataset_in, transf.originalSchema)
 
                 yield request.replySuccess(substitutions={
-                    dataset_in_ref.var: basicMsg.ArgumentMsg(constant=id)
+                    dataset_in_ref.var: Utils.buildConstantArgumentMsg(id)
                     }, hasNext=False)
         else:
             yield request.replyFail()
             
             
 transformPrimitive = DistributedElements.DistributedPrimitiveWrapper("transform", 3, __Transform())
```

### Comparing `prolog_primitives-0.4.2/prolog_primitives/ml_lib/transformations/transformationClass.py` & `prolog_primitives-1.0.1/prolog_primitives/ml_lib/transformations/transformationClass.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.2/prolog_primitives.egg-info/PKG-INFO` & `prolog_primitives-1.0.1/prolog_primitives.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prolog-primitives
-Version: 0.4.2
+Version: 1.0.1
 Summary: description here
 Home-page: https://github.com/lorenzo-osimani/prolog_primitives/
 Author: Lorenzo Osimani
 Author-email: lorenzo.osimani@studio.unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/lorenzo-osimani/prolog_primitives/issues
 Project-URL: Source, https://github.com/lorenzo-osimani/prolog_primitives/
```

### Comparing `prolog_primitives-0.4.2/prolog_primitives.egg-info/SOURCES.txt` & `prolog_primitives-1.0.1/prolog_primitives.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+VERSION
 pyproject.toml
 requirements.txt
 setup.py
 prolog_primitives/__init__.py
 prolog_primitives.egg-info/PKG-INFO
 prolog_primitives.egg-info/SOURCES.txt
 prolog_primitives.egg-info/dependency_links.txt
@@ -16,23 +17,14 @@
 prolog_primitives/basic/PrimitiveWrapper.py
 prolog_primitives/basic/Session.py
 prolog_primitives/basic/SubRequestEvent.py
 prolog_primitives/basic/Utils.py
 prolog_primitives/basic/__init__.py
 prolog_primitives/basic/filterKbPrimitive.py
 prolog_primitives/basic/ntPrimitive.py
-prolog_primitives/generatedProto/__init__.py
-prolog_primitives/generatedProto/basicMessages_pb2.py
-prolog_primitives/generatedProto/basicMessages_pb2_grpc.py
-prolog_primitives/generatedProto/errorsMessages_pb2.py
-prolog_primitives/generatedProto/errorsMessages_pb2_grpc.py
-prolog_primitives/generatedProto/primitiveService_pb2.py
-prolog_primitives/generatedProto/primitiveService_pb2_grpc.py
-prolog_primitives/generatedProto/sideEffectsMessages_pb2.py
-prolog_primitives/generatedProto/sideEffectsMessages_pb2_grpc.py
 prolog_primitives/ml_lib/__init__.py
 prolog_primitives/ml_lib/__main__.py
 prolog_primitives/ml_lib/collections.py
 prolog_primitives/ml_lib/launcher.py
 prolog_primitives/ml_lib/dataset/__init__.py
 prolog_primitives/ml_lib/dataset/cell.py
 prolog_primitives/ml_lib/dataset/column.py
```

