# Comparing `tmp/autogluon.common-0.8.3b20230707.tar.gz` & `tmp/autogluon.common-0.8.3b20230708.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.common-0.8.3b20230707.tar", last modified: Fri Jul  7 09:03:56 2023, max compression
+gzip compressed data, was "autogluon.common-0.8.3b20230708.tar", last modified: Sat Jul  8 09:04:09 2023, max compression
```

## Comparing `autogluon.common-0.8.3b20230707.tar` & `autogluon.common-0.8.3b20230708.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:03:56.368562 autogluon.common-0.8.3b20230707/
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    12658 2023-07-07 09:03:56.368562 autogluon.common-0.8.3b20230707/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 09:03:56.368562 autogluon.common-0.8.3b20230707/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:03:56.352562 autogluon.common-0.8.3b20230707/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:03:56.352562 autogluon.common-0.8.3b20230707/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:03:56.356562 autogluon.common-0.8.3b20230707/src/autogluon/common/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:03:56.356562 autogluon.common-0.8.3b20230707/src/autogluon/common/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22823 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/features/feature_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/features/infer_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/features/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:03:56.360562 autogluon.common-0.8.3b20230707/src/autogluon/common/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9956 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/loaders/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/loaders/load_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8850 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/loaders/load_pd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/loaders/load_pkl.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/loaders/load_pointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/loaders/load_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/loaders/load_str.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/loaders/load_zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:03:56.360562 autogluon.common-0.8.3b20230707/src/autogluon/common/model_filter/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/model_filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/model_filter/_model_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:03:56.364562 autogluon.common-0.8.3b20230707/src/autogluon/common/savers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/savers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/savers/save_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/savers/save_pd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/savers/save_pkl.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/savers/save_pointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/savers/save_str.py
--rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:03:56.368562 autogluon.common-0.8.3b20230707/src/autogluon/common/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/utils/compression_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/utils/deprecated_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/utils/distribute_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/utils/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/utils/lite.py
--rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/utils/multiprocessing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/utils/nvutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/utils/pandas_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/utils/path_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/utils/resource_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15650 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/utils/s3_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/utils/try_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-07-07 09:03:45.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-07 09:03:55.000000 autogluon.common-0.8.3b20230707/src/autogluon/common/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:03:56.356562 autogluon.common-0.8.3b20230707/src/autogluon.common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12658 2023-07-07 09:03:56.000000 autogluon.common-0.8.3b20230707/src/autogluon.common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-07 09:03:56.000000 autogluon.common-0.8.3b20230707/src/autogluon.common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 09:03:56.000000 autogluon.common-0.8.3b20230707/src/autogluon.common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 09:03:56.000000 autogluon.common-0.8.3b20230707/src/autogluon.common.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-07 09:03:56.000000 autogluon.common-0.8.3b20230707/src/autogluon.common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 09:03:56.000000 autogluon.common-0.8.3b20230707/src/autogluon.common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 09:03:56.000000 autogluon.common-0.8.3b20230707/src/autogluon.common.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:04:09.161172 autogluon.common-0.8.3b20230708/
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    12658 2023-07-08 09:04:09.161172 autogluon.common-0.8.3b20230708/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 09:04:09.161172 autogluon.common-0.8.3b20230708/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:04:09.149172 autogluon.common-0.8.3b20230708/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:04:09.149172 autogluon.common-0.8.3b20230708/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:04:09.153172 autogluon.common-0.8.3b20230708/src/autogluon/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:04:09.153172 autogluon.common-0.8.3b20230708/src/autogluon/common/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22823 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/features/feature_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/features/infer_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/features/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:04:09.157172 autogluon.common-0.8.3b20230708/src/autogluon/common/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9956 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/loaders/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/loaders/load_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8850 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/loaders/load_pd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/loaders/load_pkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/loaders/load_pointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/loaders/load_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/loaders/load_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/loaders/load_zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:04:09.157172 autogluon.common-0.8.3b20230708/src/autogluon/common/model_filter/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/model_filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/model_filter/_model_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:04:09.157172 autogluon.common-0.8.3b20230708/src/autogluon/common/savers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/savers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/savers/save_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/savers/save_pd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/savers/save_pkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/savers/save_pointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/savers/save_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:04:09.161172 autogluon.common-0.8.3b20230708/src/autogluon/common/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/utils/compression_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/utils/deprecated_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/utils/distribute_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/utils/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/utils/lite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/utils/multiprocessing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/utils/nvutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/utils/pandas_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/utils/path_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/utils/resource_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15650 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/utils/s3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/utils/try_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-07-08 09:03:52.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-08 09:04:08.000000 autogluon.common-0.8.3b20230708/src/autogluon/common/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:04:09.153172 autogluon.common-0.8.3b20230708/src/autogluon.common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12658 2023-07-08 09:04:08.000000 autogluon.common-0.8.3b20230708/src/autogluon.common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-08 09:04:09.000000 autogluon.common-0.8.3b20230708/src/autogluon.common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 09:04:08.000000 autogluon.common-0.8.3b20230708/src/autogluon.common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-08 09:04:08.000000 autogluon.common-0.8.3b20230708/src/autogluon.common.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-08 09:04:08.000000 autogluon.common-0.8.3b20230708/src/autogluon.common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-08 09:04:08.000000 autogluon.common-0.8.3b20230708/src/autogluon.common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 09:04:08.000000 autogluon.common-0.8.3b20230708/src/autogluon.common.egg-info/zip-safe
```

### Comparing `autogluon.common-0.8.3b20230707/LICENSE` & `autogluon.common-0.8.3b20230708/LICENSE`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.3b20230707/PKG-INFO` & `autogluon.common-0.8.3b20230708/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.common
-Version: 0.8.3b20230707
+Version: 0.8.3b20230708
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.common-0.8.3b20230707/setup.py` & `autogluon.common-0.8.3b20230708/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.3b20230707/src/autogluon/common/features/feature_metadata.py` & `autogluon.common-0.8.3b20230708/src/autogluon/common/features/feature_metadata.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.3b20230707/src/autogluon/common/features/infer_types.py` & `autogluon.common-0.8.3b20230708/src/autogluon/common/features/infer_types.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.3b20230707/src/autogluon/common/features/types.py` & `autogluon.common-0.8.3b20230708/src/autogluon/common/features/types.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.3b20230707/src/autogluon/common/loaders/_utils.py` & `autogluon.common-0.8.3b20230708/src/autogluon/common/loaders/_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.3b20230707/src/autogluon/common/loaders/load_pd.py` & `autogluon.common-0.8.3b20230708/src/autogluon/common/loaders/load_pd.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.3b20230707/src/autogluon/common/loaders/load_pkl.py` & `autogluon.common-0.8.3b20230708/src/autogluon/common/loaders/load_pkl.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.3b20230707/src/autogluon/common/loaders/load_pointer.py` & `autogluon.common-0.8.3b20230708/src/autogluon/common/loaders/load_pointer.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.3b20230707/src/autogluon/common/loaders/load_s3.py` & `autogluon.common-0.8.3b20230708/src/autogluon/common/loaders/load_s3.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.3b20230707/src/autogluon/common/loaders/load_str.py` & `autogluon.common-0.8.3b20230708/src/autogluon/common/loaders/load_str.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.3b20230707/src/autogluon/common/model_filter/_model_filter.py` & `autogluon.common-0.8.3b20230708/src/autogluon/common/model_filter/_model_filter.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.3b20230707/src/autogluon/common/savers/save_json.py` & `autogluon.common-0.8.3b20230708/src/autogluon/common/savers/save_json.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.3b20230707/src/autogluon/common/savers/save_pd.py` & `autogluon.common-0.8.3b20230708/src/autogluon/common/savers/save_pd.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.3b20230707/src/autogluon/common/savers/save_pkl.py` & `autogluon.common-0.8.3b20230708/src/autogluon/common/savers/save_pkl.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.3b20230707/src/autogluon/common/savers/save_str.py` & `autogluon.common-0.8.3b20230708/src/autogluon/common/savers/save_str.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.3b20230707/src/autogluon/common/space.py` & `autogluon.common-0.8.3b20230708/src/autogluon/common/space.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.3b20230707/src/autogluon/common/utils/compression_utils.py` & `autogluon.common-0.8.3b20230708/src/autogluon/common/utils/compression_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.3b20230707/src/autogluon/common/utils/deprecated_utils.py` & `autogluon.common-0.8.3b20230708/src/autogluon/common/utils/deprecated_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.3b20230707/src/autogluon/common/utils/distribute_utils.py` & `autogluon.common-0.8.3b20230708/src/autogluon/common/utils/distribute_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.3b20230707/src/autogluon/common/utils/file_utils.py` & `autogluon.common-0.8.3b20230708/src/autogluon/common/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.3b20230707/src/autogluon/common/utils/log_utils.py` & `autogluon.common-0.8.3b20230708/src/autogluon/common/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.3b20230707/src/autogluon/common/utils/multiprocessing_utils.py` & `autogluon.common-0.8.3b20230708/src/autogluon/common/utils/multiprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.3b20230707/src/autogluon/common/utils/nvutil.py` & `autogluon.common-0.8.3b20230708/src/autogluon/common/utils/nvutil.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.3b20230707/src/autogluon/common/utils/pandas_utils.py` & `autogluon.common-0.8.3b20230708/src/autogluon/common/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.3b20230707/src/autogluon/common/utils/path_converter.py` & `autogluon.common-0.8.3b20230708/src/autogluon/common/utils/path_converter.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.3b20230707/src/autogluon/common/utils/resource_utils.py` & `autogluon.common-0.8.3b20230708/src/autogluon/common/utils/resource_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.3b20230707/src/autogluon/common/utils/s3_utils.py` & `autogluon.common-0.8.3b20230708/src/autogluon/common/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.3b20230707/src/autogluon/common/utils/try_import.py` & `autogluon.common-0.8.3b20230708/src/autogluon/common/utils/try_import.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,18 +216,18 @@
 def try_import_vowpalwabbit():
     try:
         import vowpalwabbit
         from pkg_resources import parse_version  # pylint: disable=import-outside-toplevel
 
         vowpalwabbit_version = parse_version(vowpalwabbit.__version__)
         assert vowpalwabbit_version >= parse_version("9.0.0") and vowpalwabbit_version < parse_version(
-            "9.5.0"
-        ), f"Currently, we only support vowpalwabbit version >=9.0 and <9.5. Found vowpalwabbit version: {vowpalwabbit_version}"
+            "9.9.0"
+        ), f"Currently, we only support vowpalwabbit version >=9.0 and <9.9. Found vowpalwabbit version: {vowpalwabbit_version}"
     except ImportError:
-        raise ImportError("`import vowpalwabbit` failed.\n" "A quick tip is to install via `pip install vowpalwabbit>=9,<9.5")
+        raise ImportError("`import vowpalwabbit` failed.\n" "A quick tip is to install via `pip install vowpalwabbit>=9,<9.9")
 
 
 def try_import_fasttext():
     try:
         import fasttext
 
         _ = fasttext.__file__
```

### Comparing `autogluon.common-0.8.3b20230707/src/autogluon/common/utils/utils.py` & `autogluon.common-0.8.3b20230708/src/autogluon/common/utils/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.3b20230707/src/autogluon.common.egg-info/PKG-INFO` & `autogluon.common-0.8.3b20230708/src/autogluon.common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.common
-Version: 0.8.3b20230707
+Version: 0.8.3b20230708
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.common-0.8.3b20230707/src/autogluon.common.egg-info/SOURCES.txt` & `autogluon.common-0.8.3b20230708/src/autogluon.common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

