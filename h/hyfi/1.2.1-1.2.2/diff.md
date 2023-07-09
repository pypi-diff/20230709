# Comparing `tmp/hyfi-1.2.1.tar.gz` & `tmp/hyfi-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-1.2.1.tar", max compression
+gzip compressed data, was "hyfi-1.2.2.tar", max compression
```

## Comparing `hyfi-1.2.1.tar` & `hyfi-1.2.2.tar`

### file list

```diff
@@ -1,110 +1,110 @@
--rw-r--r--   0        0        0     1071 2023-07-09 11:04:46.313678 hyfi-1.2.1/LICENSE
--rw-r--r--   0        0        0     1881 2023-07-09 11:04:46.313678 hyfi-1.2.1/README.md
--rw-r--r--   0        0        0     4863 2023-07-09 11:05:12.037407 hyfi-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     3300 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/__cli__.py
--rw-r--r--   0        0        0     2465 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/__click__.py
--rw-r--r--   0        0        0      715 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/__init__.py
--rw-r--r--   0        0        0       22 2023-07-09 11:05:11.957407 hyfi-1.2.1/src/hyfi/_version.py
--rw-r--r--   0        0        0     2376 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/about/__init__.py
--rw-r--r--   0        0        0     7229 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/batch/__init__.py
--rw-r--r--   0        0        0     1206 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/cached_path/__init__.py
--rw-r--r--   0        0        0    14373 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/cached_path/_cached_path.py
--rw-r--r--   0        0        0     1619 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/cached_path/cache_file.py
--rw-r--r--   0        0        0     1100 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/cached_path/common.py
--rw-r--r--   0        0        0     1921 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/cached_path/file_lock.py
--rw-r--r--   0        0        0     3441 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/cached_path/meta.py
--rw-r--r--   0        0        0     3247 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/cached_path/progress.py
--rw-r--r--   0        0        0     1437 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/cached_path/schemes/__init__.py
--rw-r--r--   0        0        0     1815 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/cached_path/schemes/beaker.py
--rw-r--r--   0        0        0     2862 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/cached_path/schemes/hf.py
--rw-r--r--   0        0        0     2942 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/cached_path/schemes/http.py
--rw-r--r--   0        0        0     3645 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/cached_path/schemes/scheme_client.py
--rw-r--r--   0        0        0     1222 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/cached_path/testing.py
--rw-r--r--   0        0        0     4799 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/cached_path/util.py
--rw-r--r--   0        0        0      464 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/cached_path/version.py
--rw-r--r--   0        0        0    26034 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/composer/__init__.py
--rw-r--r--   0        0        0     1933 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/composer/pydantic.py
--rw-r--r--   0        0        0        0 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      233 2023-07-09 11:05:11.957407 hyfi-1.2.1/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      553 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0        0 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/cmd/__init__.yaml
--rw-r--r--   0        0        0       49 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/cmd/about.yaml
--rw-r--r--   0        0        0      155 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0       83 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0       91 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/cmd/run_workflow.yaml
--rw-r--r--   0        0        0      328 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      569 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/copier/conf.yaml
--rw-r--r--   0        0        0      709 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      322 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      137 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      198 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/mode/__debug__.yaml
--rw-r--r--   0        0        0      901 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0       61 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/module/__init__.yaml
--rw-r--r--   0        0        0       73 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      880 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0      133 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/path/__task__.yaml
--rw-r--r--   0        0        0      291 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/path/dirnames/__init__.yaml
--rw-r--r--   0        0        0       76 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/pipe/__dataframe__.yaml
--rw-r--r--   0        0        0       77 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
--rw-r--r--   0        0        0       79 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
--rw-r--r--   0        0        0       70 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/pipe/__general_external_funcs__.yaml
--rw-r--r--   0        0        0       72 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/pipe/__general_instance_methods__.yaml
--rw-r--r--   0        0        0      128 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/pipe/__init__.yaml
--rw-r--r--   0        0        0      236 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/pipe/load_dataframes.yaml
--rw-r--r--   0        0        0      241 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/pipe/save_dataframes.yaml
--rw-r--r--   0        0        0       90 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/pipe/test_preprocessing.yaml
--rw-r--r--   0        0        0       69 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/pipeline/__init__.yaml
--rw-r--r--   0        0        0      388 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/pipeline/__test_dataframe__.yaml
--rw-r--r--   0        0        0      268 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/pipeline/__test_general__.yaml
--rw-r--r--   0        0        0      744 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0      170 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/project/__test__.yaml
--rw-r--r--   0        0        0       38 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/running/__init__.yaml
--rw-r--r--   0        0        0      161 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      305 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/task/__init__.yaml
--rw-r--r--   0        0        0      208 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/task/__test__.yaml
--rw-r--r--   0        0        0       99 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/workflow/__init__.yaml
--rw-r--r--   0        0        0       99 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/workflow/__test__.yaml
--rw-r--r--   0        0        0     6558 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/copier/__init__.py
--rw-r--r--   0        0        0      792 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/core/__init__.py
--rw-r--r--   0        0        0    10581 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/core/config.py
--rw-r--r--   0        0        0     5915 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/dotenv/__init__.py
--rw-r--r--   0        0        0     3517 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/graphics/__init__.py
--rw-r--r--   0        0        0     8470 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/graphics/collage.py
--rw-r--r--   0        0        0     4538 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/graphics/motion.py
--rw-r--r--   0        0        0     7020 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/graphics/utils.py
--rw-r--r--   0        0        0     4192 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/joblib/__init__.py
--rw-r--r--   0        0        0      111 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/joblib/batch/__init__.py
--rw-r--r--   0        0        0     6312 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/joblib/batch/apply.py
--rw-r--r--   0        0        0     4779 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/joblib/batch/apply_batch.py
--rw-r--r--   0        0        0    13823 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/joblib/batch/batcher.py
--rw-r--r--   0        0        0    13608 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/main/__init__.py
--rw-r--r--   0        0        0      280 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/module/__init__.py
--rw-r--r--   0        0        0     4909 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/path/__init__.py
--rw-r--r--   0        0        0     4183 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/path/base.py
--rw-r--r--   0        0        0      782 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/path/batch.py
--rw-r--r--   0        0        0      599 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/path/dirnames.py
--rw-r--r--   0        0        0     1609 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/path/task.py
--rw-r--r--   0        0        0     5030 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/pipe/__init__.py
--rw-r--r--   0        0        0     1455 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/pipe/test.py
--rw-r--r--   0        0        0     8032 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/pipeline/__init__.py
--rw-r--r--   0        0        0     2874 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/pipeline/configs.py
--rw-r--r--   0        0        0     5612 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/project/__init__.py
--rw-r--r--   0        0        0        0 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/py.typed
--rw-r--r--   0        0        0     4268 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/task/__init__.py
--rw-r--r--   0        0        0     7041 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/task/batch.py
--rw-r--r--   0        0        0        0 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0    12742 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/utils/conf.py
--rw-r--r--   0        0        0     1314 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/utils/contexts.py
--rw-r--r--   0        0        0    30089 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/utils/datasets.py
--rw-r--r--   0        0        0     6568 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/utils/envs.py
--rw-r--r--   0        0        0    10857 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/utils/funcs.py
--rw-r--r--   0        0        0     4930 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/utils/gpumon.py
--rw-r--r--   0        0        0    20157 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/utils/iolibs.py
--rw-r--r--   0        0        0     2259 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0    12820 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/utils/notebooks.py
--rw-r--r--   0        0        0     6955 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/utils/packages.py
--rw-r--r--   0        0        0      382 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/utils/types.py
--rw-r--r--   0        0        0      753 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/workflow/__init__.py
--rw-r--r--   0        0        0     3393 1970-01-01 00:00:00.000000 hyfi-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-09 19:55:10.639835 hyfi-1.2.2/LICENSE
+-rw-r--r--   0        0        0     1881 2023-07-09 19:55:10.639835 hyfi-1.2.2/README.md
+-rw-r--r--   0        0        0     4863 2023-07-09 19:55:45.447852 hyfi-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3281 2023-07-09 19:55:10.643835 hyfi-1.2.2/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0     2465 2023-07-09 19:55:10.643835 hyfi-1.2.2/src/hyfi/__click__.py
+-rw-r--r--   0        0        0      715 2023-07-09 19:55:10.643835 hyfi-1.2.2/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-09 19:55:45.343852 hyfi-1.2.2/src/hyfi/_version.py
+-rw-r--r--   0        0        0     2376 2023-07-09 19:55:10.643835 hyfi-1.2.2/src/hyfi/about/__init__.py
+-rw-r--r--   0        0        0     7229 2023-07-09 19:55:10.643835 hyfi-1.2.2/src/hyfi/batch/__init__.py
+-rw-r--r--   0        0        0     1206 2023-07-09 19:55:10.643835 hyfi-1.2.2/src/hyfi/cached_path/__init__.py
+-rw-r--r--   0        0        0    14373 2023-07-09 19:55:10.643835 hyfi-1.2.2/src/hyfi/cached_path/_cached_path.py
+-rw-r--r--   0        0        0     1619 2023-07-09 19:55:10.643835 hyfi-1.2.2/src/hyfi/cached_path/cache_file.py
+-rw-r--r--   0        0        0     1100 2023-07-09 19:55:10.643835 hyfi-1.2.2/src/hyfi/cached_path/common.py
+-rw-r--r--   0        0        0     1921 2023-07-09 19:55:10.643835 hyfi-1.2.2/src/hyfi/cached_path/file_lock.py
+-rw-r--r--   0        0        0     3441 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/cached_path/meta.py
+-rw-r--r--   0        0        0     3247 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/cached_path/progress.py
+-rw-r--r--   0        0        0     1437 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/cached_path/schemes/__init__.py
+-rw-r--r--   0        0        0     1815 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/cached_path/schemes/beaker.py
+-rw-r--r--   0        0        0     2862 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/cached_path/schemes/hf.py
+-rw-r--r--   0        0        0     2942 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/cached_path/schemes/http.py
+-rw-r--r--   0        0        0     3645 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/cached_path/schemes/scheme_client.py
+-rw-r--r--   0        0        0     1222 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/cached_path/testing.py
+-rw-r--r--   0        0        0     4799 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/cached_path/util.py
+-rw-r--r--   0        0        0      464 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/cached_path/version.py
+-rw-r--r--   0        0        0    26044 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/composer/__init__.py
+-rw-r--r--   0        0        0     1933 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/composer/pydantic.py
+-rw-r--r--   0        0        0        0 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      233 2023-07-09 19:55:45.343852 hyfi-1.2.2/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      553 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0        0 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/cmd/__init__.yaml
+-rw-r--r--   0        0        0       49 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      155 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0       83 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0       91 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/cmd/run_workflow.yaml
+-rw-r--r--   0        0        0      328 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      569 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      709 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      322 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      137 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      198 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/mode/__debug__.yaml
+-rw-r--r--   0        0        0      901 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0       61 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       73 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      880 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      133 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/path/__task__.yaml
+-rw-r--r--   0        0        0      291 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/path/dirnames/__init__.yaml
+-rw-r--r--   0        0        0       76 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/pipe/__dataframe__.yaml
+-rw-r--r--   0        0        0       77 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
+-rw-r--r--   0        0        0       79 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
+-rw-r--r--   0        0        0       70 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/pipe/__general_external_funcs__.yaml
+-rw-r--r--   0        0        0       72 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/pipe/__general_instance_methods__.yaml
+-rw-r--r--   0        0        0      128 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/pipe/__init__.yaml
+-rw-r--r--   0        0        0      236 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/pipe/load_dataframes.yaml
+-rw-r--r--   0        0        0      241 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/pipe/save_dataframes.yaml
+-rw-r--r--   0        0        0       90 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/pipe/test_preprocessing.yaml
+-rw-r--r--   0        0        0       69 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/pipeline/__init__.yaml
+-rw-r--r--   0        0        0      388 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/pipeline/__test_dataframe__.yaml
+-rw-r--r--   0        0        0      268 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/pipeline/__test_general__.yaml
+-rw-r--r--   0        0        0      744 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0      185 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/project/__test__.yaml
+-rw-r--r--   0        0        0       38 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/running/__init__.yaml
+-rw-r--r--   0        0        0      161 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      305 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      208 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/task/__test__.yaml
+-rw-r--r--   0        0        0      114 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/workflow/__init__.yaml
+-rw-r--r--   0        0        0      113 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/conf/workflow/__test__.yaml
+-rw-r--r--   0        0        0     6558 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/copier/__init__.py
+-rw-r--r--   0        0        0      844 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/core/__init__.py
+-rw-r--r--   0        0        0    10581 2023-07-09 19:55:10.647835 hyfi-1.2.2/src/hyfi/core/config.py
+-rw-r--r--   0        0        0     5915 2023-07-09 19:55:10.651835 hyfi-1.2.2/src/hyfi/dotenv/__init__.py
+-rw-r--r--   0        0        0     3517 2023-07-09 19:55:10.651835 hyfi-1.2.2/src/hyfi/graphics/__init__.py
+-rw-r--r--   0        0        0     8470 2023-07-09 19:55:10.651835 hyfi-1.2.2/src/hyfi/graphics/collage.py
+-rw-r--r--   0        0        0     4538 2023-07-09 19:55:10.651835 hyfi-1.2.2/src/hyfi/graphics/motion.py
+-rw-r--r--   0        0        0     7020 2023-07-09 19:55:10.651835 hyfi-1.2.2/src/hyfi/graphics/utils.py
+-rw-r--r--   0        0        0     4214 2023-07-09 19:55:10.651835 hyfi-1.2.2/src/hyfi/joblib/__init__.py
+-rw-r--r--   0        0        0      111 2023-07-09 19:55:10.651835 hyfi-1.2.2/src/hyfi/joblib/batch/__init__.py
+-rw-r--r--   0        0        0     6312 2023-07-09 19:55:10.651835 hyfi-1.2.2/src/hyfi/joblib/batch/apply.py
+-rw-r--r--   0        0        0     4779 2023-07-09 19:55:10.651835 hyfi-1.2.2/src/hyfi/joblib/batch/apply_batch.py
+-rw-r--r--   0        0        0    13823 2023-07-09 19:55:10.651835 hyfi-1.2.2/src/hyfi/joblib/batch/batcher.py
+-rw-r--r--   0        0        0    13627 2023-07-09 19:55:10.651835 hyfi-1.2.2/src/hyfi/main/__init__.py
+-rw-r--r--   0        0        0      280 2023-07-09 19:55:10.651835 hyfi-1.2.2/src/hyfi/module/__init__.py
+-rw-r--r--   0        0        0     4909 2023-07-09 19:55:10.651835 hyfi-1.2.2/src/hyfi/path/__init__.py
+-rw-r--r--   0        0        0     4183 2023-07-09 19:55:10.651835 hyfi-1.2.2/src/hyfi/path/base.py
+-rw-r--r--   0        0        0      782 2023-07-09 19:55:10.651835 hyfi-1.2.2/src/hyfi/path/batch.py
+-rw-r--r--   0        0        0      599 2023-07-09 19:55:10.651835 hyfi-1.2.2/src/hyfi/path/dirnames.py
+-rw-r--r--   0        0        0     1609 2023-07-09 19:55:10.651835 hyfi-1.2.2/src/hyfi/path/task.py
+-rw-r--r--   0        0        0     5030 2023-07-09 19:55:10.651835 hyfi-1.2.2/src/hyfi/pipe/__init__.py
+-rw-r--r--   0        0        0     1455 2023-07-09 19:55:10.651835 hyfi-1.2.2/src/hyfi/pipe/test.py
+-rw-r--r--   0        0        0     8169 2023-07-09 19:55:10.651835 hyfi-1.2.2/src/hyfi/pipeline/__init__.py
+-rw-r--r--   0        0        0     2874 2023-07-09 19:55:10.651835 hyfi-1.2.2/src/hyfi/pipeline/configs.py
+-rw-r--r--   0        0        0     5825 2023-07-09 19:55:10.651835 hyfi-1.2.2/src/hyfi/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 19:55:10.651835 hyfi-1.2.2/src/hyfi/py.typed
+-rw-r--r--   0        0        0     4268 2023-07-09 19:55:10.651835 hyfi-1.2.2/src/hyfi/task/__init__.py
+-rw-r--r--   0        0        0     7041 2023-07-09 19:55:10.651835 hyfi-1.2.2/src/hyfi/task/batch.py
+-rw-r--r--   0        0        0        0 2023-07-09 19:55:10.651835 hyfi-1.2.2/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0    12742 2023-07-09 19:55:10.651835 hyfi-1.2.2/src/hyfi/utils/conf.py
+-rw-r--r--   0        0        0     1314 2023-07-09 19:55:10.651835 hyfi-1.2.2/src/hyfi/utils/contexts.py
+-rw-r--r--   0        0        0    30089 2023-07-09 19:55:10.651835 hyfi-1.2.2/src/hyfi/utils/datasets.py
+-rw-r--r--   0        0        0     6568 2023-07-09 19:55:10.651835 hyfi-1.2.2/src/hyfi/utils/envs.py
+-rw-r--r--   0        0        0    10857 2023-07-09 19:55:10.651835 hyfi-1.2.2/src/hyfi/utils/funcs.py
+-rw-r--r--   0        0        0     4930 2023-07-09 19:55:10.651835 hyfi-1.2.2/src/hyfi/utils/gpumon.py
+-rw-r--r--   0        0        0    20157 2023-07-09 19:55:10.651835 hyfi-1.2.2/src/hyfi/utils/iolibs.py
+-rw-r--r--   0        0        0     2259 2023-07-09 19:55:10.651835 hyfi-1.2.2/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0    12820 2023-07-09 19:55:10.651835 hyfi-1.2.2/src/hyfi/utils/notebooks.py
+-rw-r--r--   0        0        0     6955 2023-07-09 19:55:10.651835 hyfi-1.2.2/src/hyfi/utils/packages.py
+-rw-r--r--   0        0        0      382 2023-07-09 19:55:10.651835 hyfi-1.2.2/src/hyfi/utils/types.py
+-rw-r--r--   0        0        0      753 2023-07-09 19:55:10.651835 hyfi-1.2.2/src/hyfi/workflow/__init__.py
+-rw-r--r--   0        0        0     3393 1970-01-01 00:00:00.000000 hyfi-1.2.2/PKG-INFO
```

### Comparing `hyfi-1.2.1/LICENSE` & `hyfi-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/README.md` & `hyfi-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/pyproject.toml` & `hyfi-1.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi"
-version = "1.2.1"
+version = "1.2.2"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
```

### Comparing `hyfi-1.2.1/src/hyfi/__cli__.py` & `hyfi-1.2.2/src/hyfi/__cli__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """Command line interface for HyFI"""
 import os
 from typing import Optional
 
 import hydra
 from omegaconf import DictConfig
 
-from hyfi.core import __about__, __hydra_version_base__
+from hyfi.core import (
+    __about__,
+    __config_name__,
+    __config_path__,
+    __hydra_version_base__,
+)
 from hyfi.core.config import HyfiConfig
 from hyfi.main import HyFI
-from hyfi.utils.logging import LOGGING
 
-logger = LOGGING.getLogger(__name__)
-
-
-__config_path__ = "conf"
-__config_name__ = "config"
+logger = HyFI.getLogger(__name__)
 
 
 def about(**args):
     """
     Print the about information for Hyfi.
     This is a wrapper around _about which takes a HyfiConfig as an argument
     """
@@ -56,14 +56,15 @@
     Args:
         cfg: Configuration dictionary to be used for instantiation
 
     Returns:
         None if everything went fine otherwise an error is raised
         to indicate the reason for the failure
     """
+    HyFI.initialize()
     hyfi = HyfiConfig(**cfg)  # type: ignore
     verbose = hyfi.verbose
     # Print out the command line interface for the application.
     if verbose:
         app_name = hyfi.app_name
         print(f"## Command Line Interface for {app_name} ##")
```

### Comparing `hyfi-1.2.1/src/hyfi/__click__.py` & `hyfi-1.2.2/src/hyfi/__click__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/__init__.py` & `hyfi-1.2.2/src/hyfi/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/about/__init__.py` & `hyfi-1.2.2/src/hyfi/about/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/batch/__init__.py` & `hyfi-1.2.2/src/hyfi/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/cached_path/__init__.py` & `hyfi-1.2.2/src/hyfi/cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/cached_path/_cached_path.py` & `hyfi-1.2.2/src/hyfi/cached_path/_cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/cached_path/cache_file.py` & `hyfi-1.2.2/src/hyfi/cached_path/cache_file.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/cached_path/common.py` & `hyfi-1.2.2/src/hyfi/cached_path/common.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/cached_path/file_lock.py` & `hyfi-1.2.2/src/hyfi/cached_path/file_lock.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/cached_path/meta.py` & `hyfi-1.2.2/src/hyfi/cached_path/meta.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/cached_path/progress.py` & `hyfi-1.2.2/src/hyfi/cached_path/progress.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/cached_path/schemes/__init__.py` & `hyfi-1.2.2/src/hyfi/cached_path/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/cached_path/schemes/beaker.py` & `hyfi-1.2.2/src/hyfi/cached_path/schemes/beaker.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/cached_path/schemes/hf.py` & `hyfi-1.2.2/src/hyfi/cached_path/schemes/hf.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/cached_path/schemes/http.py` & `hyfi-1.2.2/src/hyfi/cached_path/schemes/http.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/cached_path/schemes/scheme_client.py` & `hyfi-1.2.2/src/hyfi/cached_path/schemes/scheme_client.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/cached_path/testing.py` & `hyfi-1.2.2/src/hyfi/cached_path/testing.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/cached_path/util.py` & `hyfi-1.2.2/src/hyfi/cached_path/util.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/composer/__init__.py` & `hyfi-1.2.2/src/hyfi/composer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -540,15 +540,15 @@
     model_config = ConfigDict(
         arbitrary_types_allowed=True,
         extra="allow",
         validate_assignment=False,
     )  # type: ignore
 
     def __init__(self, **config_kwargs):
-        logger.debug("init %s with %s", self.__class__.__name__, config_kwargs)
+        logger.debug("init %s with %s args", self.__class__.__name__, len(config_kwargs))
         super().__init__(**config_kwargs)
         self.initialize_subconfigs(config_kwargs)
 
     def __setattr__(self, key, val):
         """
         Overrides the default __setattr__ method to allow for custom property set methods.
```

### Comparing `hyfi-1.2.1/src/hyfi/composer/pydantic.py` & `hyfi-1.2.2/src/hyfi/composer/pydantic.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/conf/batch/__init__.yaml` & `hyfi-1.2.2/src/hyfi/conf/batch/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/conf/copier/conf.yaml` & `hyfi-1.2.2/src/hyfi/conf/copier/conf.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-1.2.2/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-1.2.2/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/conf/mode/__init__.yaml` & `hyfi-1.2.2/src/hyfi/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/conf/path/__init__.yaml` & `hyfi-1.2.2/src/hyfi/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/conf/project/__init__.yaml` & `hyfi-1.2.2/src/hyfi/conf/project/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/copier/__init__.py` & `hyfi-1.2.2/src/hyfi/copier/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/core/__init__.py` & `hyfi-1.2.2/src/hyfi/core/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from hyfi.about import AboutConfig
 from hyfi.utils.logging import LOGGING
 
 logger = LOGGING.getLogger(__name__)
 
 __hydra_version_base__ = "1.2"
 __hydra_default_config_group_value__ = "default"
+__config_path__ = "conf"
+__config_name__ = "config"
 
 __about__ = AboutConfig()
 _batcher_instance_ = None
 
 
 class HydraConfig(BaseModel):
     """Global configuration for Hydra"""
```

### Comparing `hyfi-1.2.1/src/hyfi/core/config.py` & `hyfi-1.2.2/src/hyfi/core/config.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/dotenv/__init__.py` & `hyfi-1.2.2/src/hyfi/dotenv/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/graphics/__init__.py` & `hyfi-1.2.2/src/hyfi/graphics/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/graphics/collage.py` & `hyfi-1.2.2/src/hyfi/graphics/collage.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/graphics/motion.py` & `hyfi-1.2.2/src/hyfi/graphics/motion.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/graphics/utils.py` & `hyfi-1.2.2/src/hyfi/graphics/utils.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/joblib/__init__.py` & `hyfi-1.2.2/src/hyfi/joblib/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     def initialize(self):
         self.init_backend()
 
     def init_backend(
         self,
     ):
         """Initialize the backend for joblib"""
-        if self.initialize_backend:
+        if self.initialize_backend and not self._initilized_:
             backend_handle = None
             backend = self.backend
 
             if backend == "ray":
                 import ray  # type: ignore
 
                 ray_cfg = {"num_cpus": self.num_workers}
@@ -54,15 +54,15 @@
                 procs=self.num_workers,
                 minibatch_size=self.minibatch_size,
                 task_num_cpus=self.num_workers,
                 task_num_gpus=self.task_num_gpus,
                 verbose=self.verbose,
             )
             self._batcher_instance_ = core._batcher_instance_
-            logger.debug("initialized batcher with %s", core._batcher_instance_)
+            logger.info("initialized batcher with %s", core._batcher_instance_)
         self._initilized_ = True
 
     def stop_backend(self):
         """Stop the backend for joblib"""
         backend = self.backend
         if core._batcher_instance_:
             logger.debug("stopping batcher")
@@ -115,10 +115,10 @@
                     description=description,  # type: ignore
                 )(series)
                 if batcher_instance is not None:
                     batcher_instance.minibatch_size = batcher_minibatch_size
                 return results
 
         if batcher_instance is None:
-            logger.info("Warning: batcher not initialized")
+            logger.warning("batcher is not initialized")
         tqdm.pandas(desc=description)
         return series.progress_apply(func)  # type: ignore
```

### Comparing `hyfi-1.2.1/src/hyfi/joblib/batch/apply.py` & `hyfi-1.2.2/src/hyfi/joblib/batch/apply.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/joblib/batch/apply_batch.py` & `hyfi-1.2.2/src/hyfi/joblib/batch/apply_batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/joblib/batch/batcher.py` & `hyfi-1.2.2/src/hyfi/joblib/batch/batcher.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/main/__init__.py` & `hyfi-1.2.2/src/hyfi/main/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,26 @@
 OmegaConf.register_new_resolver(
     "lower_case_with_underscores", FUNCs.lower_case_with_underscores
 )
 OmegaConf.register_new_resolver("dotenv_values", ENVs.dotenv_values)
 
 
 class HyFI(
-    BATCHER, CONFs, DATASETs, ENVs, FUNCs, GPUs, GRAPHICs, IOLIBs, NBs, PIPELINEs, PKGs
+    BATCHER,
+    CONFs,
+    DATASETs,
+    ENVs,
+    FUNCs,
+    GPUs,
+    GRAPHICs,
+    IOLIBs,
+    LOGGING,
+    NBs,
+    PIPELINEs,
+    PKGs,
 ):
     """Primary class for the hyfi config package"""
 
     config = __global_config__
     SpeicialKeys = SpecialKeys
     __version__ = __global_config__._version_
     __hyfi_path__ = __hyfi_path__()
@@ -187,41 +198,41 @@
 
         Returns:
             dict: A dictionary containing the os environment variables.
         """
         return os.environ
 
     @staticmethod
-    def pipe_config(**kwargs) -> PipeConfig:
+    def pipe(**kwargs) -> PipeConfig:
         """
         Return the PipeConfig.
 
         Args:
             **kwargs: Additional keyword arguments to pass to the PipeConfig constructor.
 
         Returns:
             PipeConfig: An instance of the PipeConfig class.
         """
         return PipeConfig(**kwargs)
 
     @staticmethod
-    def task_config(**kwargs) -> TaskConfig:
+    def task(**kwargs) -> TaskConfig:
         """
         Return the TaskConfig.
 
         Args:
             **kwargs: Additional keyword arguments to pass to the TaskConfig constructor.
 
         Returns:
             TaskConfig: An instance of the TaskConfig class.
         """
         return TaskConfig(**kwargs)
 
     @staticmethod
-    def workflow_config(**kwargs) -> WorkflowConfig:
+    def workflow(**kwargs) -> WorkflowConfig:
         """
         Return the WorkflowConfig.
 
         Args:
             **kwargs: Additional keyword arguments to pass to the WorkflowConfig constructor.
 
         Returns:
@@ -341,19 +352,19 @@
     ###############################
     @staticmethod
     def run(cfg: Union[Dict, DictConfig], target: Optional[str] = None):
         """Run the config"""
         if target and target not in cfg:
             raise ValueError(f"No {target} configuration found")
         if "workflow" in cfg and (target is None or target == "workflow"):
-            workflow = HyFI.workflow_config(**cfg["workflow"])
+            workflow = HyFI.workflow(**cfg["workflow"])
             HyFI.run_workflow(workflow)
         elif "task" in cfg and (target is None or target == "task"):
             project = HyFI.init_project(**cfg["project"]) if "project" in cfg else None
-            task = HyFI.task_config(**cfg["task"])
+            task = HyFI.task(**cfg["task"])
             HyFI.run_task(task, project=project)
         elif "copier" in cfg and (target is None or target == "copier"):
             cfg = HyFI.to_dict(cfg["copier"])
             with Copier(**cfg) as worker:
                 worker.run_copy()
         else:
             HyFI.about()
```

### Comparing `hyfi-1.2.1/src/hyfi/path/__init__.py` & `hyfi-1.2.2/src/hyfi/path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/path/base.py` & `hyfi-1.2.2/src/hyfi/path/base.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/path/batch.py` & `hyfi-1.2.2/src/hyfi/path/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/path/dirnames.py` & `hyfi-1.2.2/src/hyfi/path/dirnames.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/path/task.py` & `hyfi-1.2.2/src/hyfi/path/task.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/pipe/__init__.py` & `hyfi-1.2.2/src/hyfi/pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/pipe/test.py` & `hyfi-1.2.2/src/hyfi/pipe/test.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/pipeline/__init__.py` & `hyfi-1.2.2/src/hyfi/pipeline/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,31 +222,34 @@
 
         Args:
             task: TaskConfig to run pipelines for
             project: ProjectConfig to run pipelines
         """
         # Set project to the project.
         if project:
+            project.initialize()
             task.project = project
         # Run all pipelines in the pipeline.
         if task.verbose:
-            logger.info("Running %s pipelines", len(task.pipelines or []))
+            logger.info("Running %s pipeline(s)", len(task.pipelines or []))
         for pipeline in PIPELINEs.get_pipelines(task):
             if task.verbose:
                 logger.info("Running pipeline: %s", pipeline.model_dump())
             initial_object = task if pipeline.use_task_as_initial_object else None
             PIPELINEs.run_pipeline(pipeline, initial_object, task)
 
     @staticmethod
     def run_workflow(workflow: WorkflowConfig):
         """
         Run the tasks specified in the workflow
 
         Args:
             workflow: WorkflowConfig object to run
         """
+        if workflow.verbose:
+            logger.info("Running %s task(s)", len(workflow.tasks or []))
         # Run all tasks in the workflow.
         for task in workflow.get_tasks():
             # Run the task if verbose is true.
             if workflow.verbose:
                 logger.info("Running task: %s", task.task_name)
             PIPELINEs.run_task(task, project=workflow.project)
```

### Comparing `hyfi-1.2.1/src/hyfi/pipeline/configs.py` & `hyfi-1.2.2/src/hyfi/pipeline/configs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/project/__init__.py` & `hyfi-1.2.2/src/hyfi/project/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -67,25 +67,32 @@
         return v
 
     def __init__(self, **config_kwargs):
         super().__init__(**config_kwargs)
         self.initialize()
 
     def initialize(self):
+        logger.debug("Initializing Project Config: %s", self.project_name)
         self.dotenv = DotEnvConfig()
 
         self.dotenv.HYFI_PROJECT_NAME = self.project_name
         self.dotenv.HYFI_PROJECT_DESC = self.project_description
         self.dotenv.HYFI_PROJECT_ROOT = self.project_root
         self.dotenv.HYFI_PROJECT_WORKSPACE_NAME = self.project_workspace_name
         self.dotenv.HYFI_GLOBAL_ROOT = self.global_hyfi_root
         self.dotenv.HYFI_GLOBAL_WORKSPACE_NAME = self.global_workspace_name
         self.dotenv.HYFI_NUM_WORKERS = self.num_workers
         self.dotenv.HYFI_VERBOSE = self.verbose
         self.dotenv.CACHED_PATH_CACHE_ROOT = str(self.path.cache_dir / "cached_path")
+
+        if self.joblib:
+            self.joblib.init_backend()
+        else:
+            logger.warning("JoblibConfig not initialized")
+
         self.init_wandb()
         if self.use_huggingface_hub:
             self.init_huggingface_hub()
 
     def init_wandb(self):
         if self.path is None:
             raise ValueError("Path object not initialized")
```

### Comparing `hyfi-1.2.1/src/hyfi/task/__init__.py` & `hyfi-1.2.2/src/hyfi/task/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/task/batch.py` & `hyfi-1.2.2/src/hyfi/task/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/utils/conf.py` & `hyfi-1.2.2/src/hyfi/utils/conf.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/utils/contexts.py` & `hyfi-1.2.2/src/hyfi/utils/contexts.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/utils/datasets.py` & `hyfi-1.2.2/src/hyfi/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/utils/envs.py` & `hyfi-1.2.2/src/hyfi/utils/envs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/utils/funcs.py` & `hyfi-1.2.2/src/hyfi/utils/funcs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/utils/gpumon.py` & `hyfi-1.2.2/src/hyfi/utils/gpumon.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/utils/iolibs.py` & `hyfi-1.2.2/src/hyfi/utils/iolibs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/utils/logging.py` & `hyfi-1.2.2/src/hyfi/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/utils/notebooks.py` & `hyfi-1.2.2/src/hyfi/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/utils/packages.py` & `hyfi-1.2.2/src/hyfi/utils/packages.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/src/hyfi/workflow/__init__.py` & `hyfi-1.2.2/src/hyfi/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.1/PKG-INFO` & `hyfi-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 1.2.1
+Version: 1.2.2
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 Home-page: https://hyfi.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

