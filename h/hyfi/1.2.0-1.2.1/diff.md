# Comparing `tmp/hyfi-1.2.0.tar.gz` & `tmp/hyfi-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-1.2.0.tar", max compression
+gzip compressed data, was "hyfi-1.2.1.tar", max compression
```

## Comparing `hyfi-1.2.0.tar` & `hyfi-1.2.1.tar`

### file list

```diff
@@ -1,110 +1,110 @@
--rw-r--r--   0        0        0     1071 2023-07-09 10:37:19.763455 hyfi-1.2.0/LICENSE
--rw-r--r--   0        0        0     1881 2023-07-09 10:37:19.763455 hyfi-1.2.0/README.md
--rw-r--r--   0        0        0     4863 2023-07-09 10:37:46.971159 hyfi-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     3312 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/__cli__.py
--rw-r--r--   0        0        0     2477 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/__click__.py
--rw-r--r--   0        0        0      792 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/__global__/__init__.py
--rw-r--r--   0        0        0    10587 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/__global__/config.py
--rw-r--r--   0        0        0      733 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/__init__.py
--rw-r--r--   0        0        0       22 2023-07-09 10:37:46.895160 hyfi-1.2.0/src/hyfi/_version.py
--rw-r--r--   0        0        0     2376 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/about/__init__.py
--rw-r--r--   0        0        0     7229 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/batch/__init__.py
--rw-r--r--   0        0        0     1206 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/cached_path/__init__.py
--rw-r--r--   0        0        0    14373 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/cached_path/_cached_path.py
--rw-r--r--   0        0        0     1619 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/cached_path/cache_file.py
--rw-r--r--   0        0        0     1100 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/cached_path/common.py
--rw-r--r--   0        0        0     1921 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/cached_path/file_lock.py
--rw-r--r--   0        0        0     3441 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/cached_path/meta.py
--rw-r--r--   0        0        0     3247 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/cached_path/progress.py
--rw-r--r--   0        0        0     1437 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/cached_path/schemes/__init__.py
--rw-r--r--   0        0        0     1815 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/cached_path/schemes/beaker.py
--rw-r--r--   0        0        0     2862 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/cached_path/schemes/hf.py
--rw-r--r--   0        0        0     2942 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/cached_path/schemes/http.py
--rw-r--r--   0        0        0     3645 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/cached_path/schemes/scheme_client.py
--rw-r--r--   0        0        0     1222 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/cached_path/testing.py
--rw-r--r--   0        0        0     4799 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/cached_path/util.py
--rw-r--r--   0        0        0      464 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/cached_path/version.py
--rw-r--r--   0        0        0    26040 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/composer/__init__.py
--rw-r--r--   0        0        0     1933 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/composer/pydantic.py
--rw-r--r--   0        0        0        0 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      233 2023-07-09 10:37:46.895160 hyfi-1.2.0/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      553 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0        0 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/conf/cmd/__init__.yaml
--rw-r--r--   0        0        0       49 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/conf/cmd/about.yaml
--rw-r--r--   0        0        0      155 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0       83 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0       91 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/conf/cmd/run_workflow.yaml
--rw-r--r--   0        0        0      328 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      569 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/conf/copier/conf.yaml
--rw-r--r--   0        0        0      709 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      322 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      137 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      198 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/conf/mode/__debug__.yaml
--rw-r--r--   0        0        0      901 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0       61 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/module/__init__.yaml
--rw-r--r--   0        0        0       73 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      880 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0      133 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/path/__task__.yaml
--rw-r--r--   0        0        0      291 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/path/dirnames/__init__.yaml
--rw-r--r--   0        0        0       76 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/pipe/__dataframe__.yaml
--rw-r--r--   0        0        0       77 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
--rw-r--r--   0        0        0       79 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
--rw-r--r--   0        0        0       70 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/pipe/__general_external_funcs__.yaml
--rw-r--r--   0        0        0       72 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/pipe/__general_instance_methods__.yaml
--rw-r--r--   0        0        0      128 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/pipe/__init__.yaml
--rw-r--r--   0        0        0      236 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/pipe/load_dataframes.yaml
--rw-r--r--   0        0        0      241 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/pipe/save_dataframes.yaml
--rw-r--r--   0        0        0       90 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/pipe/test_preprocessing.yaml
--rw-r--r--   0        0        0       69 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/pipeline/__init__.yaml
--rw-r--r--   0        0        0      388 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/pipeline/__test_dataframe__.yaml
--rw-r--r--   0        0        0      268 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/pipeline/__test_general__.yaml
--rw-r--r--   0        0        0      744 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0      170 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/project/__test__.yaml
--rw-r--r--   0        0        0       38 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/running/__init__.yaml
--rw-r--r--   0        0        0      161 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      305 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/task/__init__.yaml
--rw-r--r--   0        0        0      208 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/task/__test__.yaml
--rw-r--r--   0        0        0       99 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/workflow/__init__.yaml
--rw-r--r--   0        0        0       99 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/workflow/__test__.yaml
--rw-r--r--   0        0        0     6558 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/copier/__init__.py
--rw-r--r--   0        0        0     5915 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/dotenv/__init__.py
--rw-r--r--   0        0        0     3517 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/graphics/__init__.py
--rw-r--r--   0        0        0     8470 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/graphics/collage.py
--rw-r--r--   0        0        0     4538 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/graphics/motion.py
--rw-r--r--   0        0        0     7020 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/graphics/utils.py
--rw-r--r--   0        0        0     4228 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/joblib/__init__.py
--rw-r--r--   0        0        0      111 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/joblib/batch/__init__.py
--rw-r--r--   0        0        0     6312 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/joblib/batch/apply.py
--rw-r--r--   0        0        0     4779 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/joblib/batch/apply_batch.py
--rw-r--r--   0        0        0    13823 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/joblib/batch/batcher.py
--rw-r--r--   0        0        0    13620 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/main/__init__.py
--rw-r--r--   0        0        0      280 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/module/__init__.py
--rw-r--r--   0        0        0     4915 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/path/__init__.py
--rw-r--r--   0        0        0     4183 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/path/base.py
--rw-r--r--   0        0        0      782 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/path/batch.py
--rw-r--r--   0        0        0      599 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/path/dirnames.py
--rw-r--r--   0        0        0     1609 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/path/task.py
--rw-r--r--   0        0        0     5030 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/pipe/__init__.py
--rw-r--r--   0        0        0     1455 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/pipe/test.py
--rw-r--r--   0        0        0     8032 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/pipeline/__init__.py
--rw-r--r--   0        0        0     2874 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/pipeline/configs.py
--rw-r--r--   0        0        0     5618 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/project/__init__.py
--rw-r--r--   0        0        0        0 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/py.typed
--rw-r--r--   0        0        0     4268 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/task/__init__.py
--rw-r--r--   0        0        0     7041 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/task/batch.py
--rw-r--r--   0        0        0        0 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0    12742 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/utils/conf.py
--rw-r--r--   0        0        0     1314 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/utils/contexts.py
--rw-r--r--   0        0        0    30089 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/utils/datasets.py
--rw-r--r--   0        0        0     6568 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/utils/envs.py
--rw-r--r--   0        0        0    10857 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/utils/funcs.py
--rw-r--r--   0        0        0     4930 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/utils/gpumon.py
--rw-r--r--   0        0        0    20157 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/utils/iolibs.py
--rw-r--r--   0        0        0     2259 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0    12820 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/utils/notebooks.py
--rw-r--r--   0        0        0     6955 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/utils/packages.py
--rw-r--r--   0        0        0      382 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/utils/types.py
--rw-r--r--   0        0        0      753 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/workflow/__init__.py
--rw-r--r--   0        0        0     3393 1970-01-01 00:00:00.000000 hyfi-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-09 11:04:46.313678 hyfi-1.2.1/LICENSE
+-rw-r--r--   0        0        0     1881 2023-07-09 11:04:46.313678 hyfi-1.2.1/README.md
+-rw-r--r--   0        0        0     4863 2023-07-09 11:05:12.037407 hyfi-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3300 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0     2465 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/__click__.py
+-rw-r--r--   0        0        0      715 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-09 11:05:11.957407 hyfi-1.2.1/src/hyfi/_version.py
+-rw-r--r--   0        0        0     2376 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/about/__init__.py
+-rw-r--r--   0        0        0     7229 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/batch/__init__.py
+-rw-r--r--   0        0        0     1206 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/cached_path/__init__.py
+-rw-r--r--   0        0        0    14373 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/cached_path/_cached_path.py
+-rw-r--r--   0        0        0     1619 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/cached_path/cache_file.py
+-rw-r--r--   0        0        0     1100 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/cached_path/common.py
+-rw-r--r--   0        0        0     1921 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/cached_path/file_lock.py
+-rw-r--r--   0        0        0     3441 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/cached_path/meta.py
+-rw-r--r--   0        0        0     3247 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/cached_path/progress.py
+-rw-r--r--   0        0        0     1437 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/cached_path/schemes/__init__.py
+-rw-r--r--   0        0        0     1815 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/cached_path/schemes/beaker.py
+-rw-r--r--   0        0        0     2862 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/cached_path/schemes/hf.py
+-rw-r--r--   0        0        0     2942 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/cached_path/schemes/http.py
+-rw-r--r--   0        0        0     3645 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/cached_path/schemes/scheme_client.py
+-rw-r--r--   0        0        0     1222 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/cached_path/testing.py
+-rw-r--r--   0        0        0     4799 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/cached_path/util.py
+-rw-r--r--   0        0        0      464 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/cached_path/version.py
+-rw-r--r--   0        0        0    26034 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/composer/__init__.py
+-rw-r--r--   0        0        0     1933 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/composer/pydantic.py
+-rw-r--r--   0        0        0        0 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      233 2023-07-09 11:05:11.957407 hyfi-1.2.1/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      553 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0        0 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/cmd/__init__.yaml
+-rw-r--r--   0        0        0       49 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      155 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0       83 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0       91 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/cmd/run_workflow.yaml
+-rw-r--r--   0        0        0      328 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      569 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      709 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      322 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      137 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      198 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/mode/__debug__.yaml
+-rw-r--r--   0        0        0      901 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0       61 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       73 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      880 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      133 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/path/__task__.yaml
+-rw-r--r--   0        0        0      291 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/path/dirnames/__init__.yaml
+-rw-r--r--   0        0        0       76 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/pipe/__dataframe__.yaml
+-rw-r--r--   0        0        0       77 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
+-rw-r--r--   0        0        0       79 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
+-rw-r--r--   0        0        0       70 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/pipe/__general_external_funcs__.yaml
+-rw-r--r--   0        0        0       72 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/pipe/__general_instance_methods__.yaml
+-rw-r--r--   0        0        0      128 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/pipe/__init__.yaml
+-rw-r--r--   0        0        0      236 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/pipe/load_dataframes.yaml
+-rw-r--r--   0        0        0      241 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/pipe/save_dataframes.yaml
+-rw-r--r--   0        0        0       90 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/pipe/test_preprocessing.yaml
+-rw-r--r--   0        0        0       69 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/pipeline/__init__.yaml
+-rw-r--r--   0        0        0      388 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/pipeline/__test_dataframe__.yaml
+-rw-r--r--   0        0        0      268 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/pipeline/__test_general__.yaml
+-rw-r--r--   0        0        0      744 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0      170 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/project/__test__.yaml
+-rw-r--r--   0        0        0       38 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/running/__init__.yaml
+-rw-r--r--   0        0        0      161 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      305 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      208 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/task/__test__.yaml
+-rw-r--r--   0        0        0       99 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/workflow/__init__.yaml
+-rw-r--r--   0        0        0       99 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/conf/workflow/__test__.yaml
+-rw-r--r--   0        0        0     6558 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/copier/__init__.py
+-rw-r--r--   0        0        0      792 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/core/__init__.py
+-rw-r--r--   0        0        0    10581 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/core/config.py
+-rw-r--r--   0        0        0     5915 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/dotenv/__init__.py
+-rw-r--r--   0        0        0     3517 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/graphics/__init__.py
+-rw-r--r--   0        0        0     8470 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/graphics/collage.py
+-rw-r--r--   0        0        0     4538 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/graphics/motion.py
+-rw-r--r--   0        0        0     7020 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/graphics/utils.py
+-rw-r--r--   0        0        0     4192 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/joblib/__init__.py
+-rw-r--r--   0        0        0      111 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/joblib/batch/__init__.py
+-rw-r--r--   0        0        0     6312 2023-07-09 11:04:46.317678 hyfi-1.2.1/src/hyfi/joblib/batch/apply.py
+-rw-r--r--   0        0        0     4779 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/joblib/batch/apply_batch.py
+-rw-r--r--   0        0        0    13823 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/joblib/batch/batcher.py
+-rw-r--r--   0        0        0    13608 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/main/__init__.py
+-rw-r--r--   0        0        0      280 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/module/__init__.py
+-rw-r--r--   0        0        0     4909 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/path/__init__.py
+-rw-r--r--   0        0        0     4183 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/path/base.py
+-rw-r--r--   0        0        0      782 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/path/batch.py
+-rw-r--r--   0        0        0      599 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/path/dirnames.py
+-rw-r--r--   0        0        0     1609 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/path/task.py
+-rw-r--r--   0        0        0     5030 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/pipe/__init__.py
+-rw-r--r--   0        0        0     1455 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/pipe/test.py
+-rw-r--r--   0        0        0     8032 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/pipeline/__init__.py
+-rw-r--r--   0        0        0     2874 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/pipeline/configs.py
+-rw-r--r--   0        0        0     5612 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/py.typed
+-rw-r--r--   0        0        0     4268 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/task/__init__.py
+-rw-r--r--   0        0        0     7041 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/task/batch.py
+-rw-r--r--   0        0        0        0 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0    12742 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/utils/conf.py
+-rw-r--r--   0        0        0     1314 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/utils/contexts.py
+-rw-r--r--   0        0        0    30089 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/utils/datasets.py
+-rw-r--r--   0        0        0     6568 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/utils/envs.py
+-rw-r--r--   0        0        0    10857 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/utils/funcs.py
+-rw-r--r--   0        0        0     4930 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/utils/gpumon.py
+-rw-r--r--   0        0        0    20157 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/utils/iolibs.py
+-rw-r--r--   0        0        0     2259 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0    12820 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/utils/notebooks.py
+-rw-r--r--   0        0        0     6955 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/utils/packages.py
+-rw-r--r--   0        0        0      382 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/utils/types.py
+-rw-r--r--   0        0        0      753 2023-07-09 11:04:46.321679 hyfi-1.2.1/src/hyfi/workflow/__init__.py
+-rw-r--r--   0        0        0     3393 1970-01-01 00:00:00.000000 hyfi-1.2.1/PKG-INFO
```

### Comparing `hyfi-1.2.0/LICENSE` & `hyfi-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/README.md` & `hyfi-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/pyproject.toml` & `hyfi-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi"
-version = "1.2.0"
+version = "1.2.1"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
```

### Comparing `hyfi-1.2.0/src/hyfi/__cli__.py` & `hyfi-1.2.1/src/hyfi/__cli__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Command line interface for HyFI"""
 import os
 from typing import Optional
 
 import hydra
 from omegaconf import DictConfig
 
-from hyfi.__global__ import __about__, __hydra_version_base__
-from hyfi.__global__.config import HyfiConfig
+from hyfi.core import __about__, __hydra_version_base__
+from hyfi.core.config import HyfiConfig
 from hyfi.main import HyFI
 from hyfi.utils.logging import LOGGING
 
 logger = LOGGING.getLogger(__name__)
 
 
 __config_path__ = "conf"
```

### Comparing `hyfi-1.2.0/src/hyfi/__click__.py` & `hyfi-1.2.1/src/hyfi/__click__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Command line interface for HyFI"""
 
 import click
 
-from hyfi.__global__ import __hyfi_path__
-from hyfi.__global__.config import HyfiConfig
 from hyfi._version import __version__
 from hyfi.copier import Copier
+from hyfi.core import __hyfi_path__
+from hyfi.core.config import HyfiConfig
 from hyfi.utils.logging import LOGGING
 
 logger = LOGGING.getLogger(__name__)
 
 
 @click.group()
 @click.version_option(__version__)
```

### Comparing `hyfi-1.2.0/src/hyfi/__global__/__init__.py` & `hyfi-1.2.1/src/hyfi/core/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/__global__/config.py` & `hyfi-1.2.1/src/hyfi/core/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,17 @@
     ConfigDict,
     FieldValidationInfo,
     PrivateAttr,
     field_validator,
     model_validator,
 )
 
-from hyfi.__global__ import __about__, __hydra_config__
 from hyfi.about import AboutConfig, __app_name__, __version__
 from hyfi.copier import Copier
+from hyfi.core import __about__, __hydra_config__
 from hyfi.dotenv import DotEnvConfig
 from hyfi.pipeline import PipelineConfig, PIPELINEs
 from hyfi.project import ProjectConfig
 from hyfi.task import TaskConfig
 from hyfi.utils.conf import CONFs
 from hyfi.utils.envs import ENVs
 from hyfi.utils.logging import LOGGING
```

### Comparing `hyfi-1.2.0/src/hyfi/__init__.py` & `hyfi-1.2.1/src/hyfi/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,14 +4,14 @@
     All names of configuration folders and their counterparts folders for pydantic models
     are singular, e.g. `conf` instead of `configs`.
     All matching pydantic models are named `Config`, e.g. `BatchConfig` instead of `BatchConfigs`.
 
     Other module folders are plural, e.g. `utils` instead of `util`.
 """
 from hyfi.__cli__ import hydra_main
-from hyfi.__global__ import __about__ as about
-from hyfi.__global__ import __hydra_version_base__
-from hyfi.__global__.config import __global_config__ as global_config
+from hyfi.core import __about__ as about
+from hyfi.core import __hydra_version_base__
+from hyfi.core.config import __global_config__ as global_config
 from hyfi.main import HyFI
 from hyfi.main import HyFI as H
 from hyfi.main import HyFI as HI
 from hyfi.utils.logging import LOGGING
```

### Comparing `hyfi-1.2.0/src/hyfi/about/__init__.py` & `hyfi-1.2.1/src/hyfi/about/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/batch/__init__.py` & `hyfi-1.2.1/src/hyfi/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/cached_path/__init__.py` & `hyfi-1.2.1/src/hyfi/cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/cached_path/_cached_path.py` & `hyfi-1.2.1/src/hyfi/cached_path/_cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/cached_path/cache_file.py` & `hyfi-1.2.1/src/hyfi/cached_path/cache_file.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/cached_path/common.py` & `hyfi-1.2.1/src/hyfi/cached_path/common.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/cached_path/file_lock.py` & `hyfi-1.2.1/src/hyfi/cached_path/file_lock.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/cached_path/meta.py` & `hyfi-1.2.1/src/hyfi/cached_path/meta.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/cached_path/progress.py` & `hyfi-1.2.1/src/hyfi/cached_path/progress.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/cached_path/schemes/__init__.py` & `hyfi-1.2.1/src/hyfi/cached_path/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/cached_path/schemes/beaker.py` & `hyfi-1.2.1/src/hyfi/cached_path/schemes/beaker.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/cached_path/schemes/hf.py` & `hyfi-1.2.1/src/hyfi/cached_path/schemes/hf.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/cached_path/schemes/http.py` & `hyfi-1.2.1/src/hyfi/cached_path/schemes/http.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/cached_path/schemes/scheme_client.py` & `hyfi-1.2.1/src/hyfi/cached_path/schemes/scheme_client.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/cached_path/testing.py` & `hyfi-1.2.1/src/hyfi/cached_path/testing.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/cached_path/util.py` & `hyfi-1.2.1/src/hyfi/cached_path/util.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/composer/__init__.py` & `hyfi-1.2.1/src/hyfi/composer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Mapping, Optional, Set, Tuple, Union
 
 import hydra
 from omegaconf import DictConfig
 from pydantic import BaseModel, ConfigDict, PrivateAttr, model_validator
 
-from hyfi.__global__ import (
+from hyfi.core import (
     __about__,
     __hydra_config__,
     __hydra_default_config_group_value__,
     __hydra_version_base__,
 )
 from hyfi.utils.conf import CONFs
 from hyfi.utils.logging import LOGGING
```

### Comparing `hyfi-1.2.0/src/hyfi/composer/pydantic.py` & `hyfi-1.2.1/src/hyfi/composer/pydantic.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/conf/batch/__init__.yaml` & `hyfi-1.2.1/src/hyfi/conf/batch/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/conf/copier/conf.yaml` & `hyfi-1.2.1/src/hyfi/conf/copier/conf.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-1.2.1/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-1.2.1/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/conf/mode/__init__.yaml` & `hyfi-1.2.1/src/hyfi/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/conf/path/__init__.yaml` & `hyfi-1.2.1/src/hyfi/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/conf/project/__init__.yaml` & `hyfi-1.2.1/src/hyfi/conf/project/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/copier/__init__.py` & `hyfi-1.2.1/src/hyfi/copier/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/dotenv/__init__.py` & `hyfi-1.2.1/src/hyfi/dotenv/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/graphics/__init__.py` & `hyfi-1.2.1/src/hyfi/graphics/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/graphics/collage.py` & `hyfi-1.2.1/src/hyfi/graphics/collage.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/graphics/motion.py` & `hyfi-1.2.1/src/hyfi/graphics/motion.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/graphics/utils.py` & `hyfi-1.2.1/src/hyfi/graphics/utils.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/joblib/__init__.py` & `hyfi-1.2.1/src/hyfi/joblib/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Callable, Mapping, Optional, Sequence, Union
 
 import pandas as pd
 from pydantic import PrivateAttr
 from tqdm.auto import tqdm
 
-from hyfi import __global__
+from hyfi import core
 from hyfi.composer import BaseConfig
 from hyfi.joblib.batch import batcher
 from hyfi.joblib.batch.apply import decorator_apply
 from hyfi.joblib.batch.batcher import Batcher
 from hyfi.utils.logging import LOGGING
 
 logger = LOGGING.getLogger(__name__)
@@ -44,33 +44,33 @@
                 import ray  # type: ignore
 
                 ray_cfg = {"num_cpus": self.num_workers}
                 logger.debug(f"initializing ray with {ray_cfg}")
                 ray.init(**ray_cfg)
                 backend_handle = ray
 
-            __global__._batcher_instance_ = batcher.Batcher(
+            core._batcher_instance_ = batcher.Batcher(
                 backend_handle=backend_handle,
                 backend=self.backend,
                 procs=self.num_workers,
                 minibatch_size=self.minibatch_size,
                 task_num_cpus=self.num_workers,
                 task_num_gpus=self.task_num_gpus,
                 verbose=self.verbose,
             )
-            self._batcher_instance_ = __global__._batcher_instance_
-            logger.debug("initialized batcher with %s", __global__._batcher_instance_)
+            self._batcher_instance_ = core._batcher_instance_
+            logger.debug("initialized batcher with %s", core._batcher_instance_)
         self._initilized_ = True
 
     def stop_backend(self):
         """Stop the backend for joblib"""
         backend = self.backend
-        if __global__._batcher_instance_:
+        if core._batcher_instance_:
             logger.debug("stopping batcher")
-            del __global__._batcher_instance_
+            del core._batcher_instance_
 
         logger.debug("stopping distributed framework")
         if self.initialize_backend and backend == "ray":
             try:
                 import ray  # type: ignore
 
                 if ray.is_initialized():
```

### Comparing `hyfi-1.2.0/src/hyfi/joblib/batch/apply.py` & `hyfi-1.2.1/src/hyfi/joblib/batch/apply.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/joblib/batch/apply_batch.py` & `hyfi-1.2.1/src/hyfi/joblib/batch/apply_batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/joblib/batch/batcher.py` & `hyfi-1.2.1/src/hyfi/joblib/batch/batcher.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/main/__init__.py` & `hyfi-1.2.1/src/hyfi/main/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 import os
 import random
 from typing import Any, Callable, Dict, List, Optional, Union
 
 import hydra
 from omegaconf import DictConfig, OmegaConf
 
-from hyfi.__global__ import __home_path__, __hyfi_path__
-from hyfi.__global__.config import __global_config__, __search_package_path__
 from hyfi.about import __version__
 from hyfi.cached_path import cached_path
 from hyfi.composer import Composer, SpecialKeys
 from hyfi.copier import Copier
+from hyfi.core import __home_path__, __hyfi_path__
+from hyfi.core.config import __global_config__, __search_package_path__
 from hyfi.dotenv import DotEnvConfig
 from hyfi.graphics import GRAPHICs
 from hyfi.joblib import BATCHER, JobLibConfig
 from hyfi.pipeline import PIPELINEs
 from hyfi.pipeline.configs import PipeConfig
 from hyfi.project import ProjectConfig
 from hyfi.task import TaskConfig
```

### Comparing `hyfi-1.2.0/src/hyfi/path/__init__.py` & `hyfi-1.2.1/src/hyfi/path/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 
-from hyfi.__global__ import __about__
 from hyfi.composer import BaseConfig
+from hyfi.core import __about__
 from hyfi.path.base import BasePathConfig
 from hyfi.utils.logging import LOGGING
 
 logger = LOGGING.getLogger(__name__)
 
 
 class PathConfig(BaseConfig, BasePathConfig):
```

### Comparing `hyfi-1.2.0/src/hyfi/path/base.py` & `hyfi-1.2.1/src/hyfi/path/base.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/path/batch.py` & `hyfi-1.2.1/src/hyfi/path/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/path/dirnames.py` & `hyfi-1.2.1/src/hyfi/path/dirnames.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/path/task.py` & `hyfi-1.2.1/src/hyfi/path/task.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/pipe/__init__.py` & `hyfi-1.2.1/src/hyfi/pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/pipe/test.py` & `hyfi-1.2.1/src/hyfi/pipe/test.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/pipeline/__init__.py` & `hyfi-1.2.1/src/hyfi/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/pipeline/configs.py` & `hyfi-1.2.1/src/hyfi/pipeline/configs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/project/__init__.py` & `hyfi-1.2.1/src/hyfi/project/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from pathlib import Path
 from typing import Union
 
 from pydantic import field_validator
 
-from hyfi.__global__ import __about__
 from hyfi.composer import BaseConfig
+from hyfi.core import __about__
 from hyfi.dotenv import DotEnvConfig
 from hyfi.joblib import JobLibConfig
 from hyfi.path import PathConfig
 from hyfi.utils.logging import LOGGING
 from hyfi.utils.notebooks import NBs
 
 logger = LOGGING.getLogger(__name__)
```

### Comparing `hyfi-1.2.0/src/hyfi/task/__init__.py` & `hyfi-1.2.1/src/hyfi/task/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/task/batch.py` & `hyfi-1.2.1/src/hyfi/task/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/utils/conf.py` & `hyfi-1.2.1/src/hyfi/utils/conf.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/utils/contexts.py` & `hyfi-1.2.1/src/hyfi/utils/contexts.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/utils/datasets.py` & `hyfi-1.2.1/src/hyfi/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/utils/envs.py` & `hyfi-1.2.1/src/hyfi/utils/envs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/utils/funcs.py` & `hyfi-1.2.1/src/hyfi/utils/funcs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/utils/gpumon.py` & `hyfi-1.2.1/src/hyfi/utils/gpumon.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/utils/iolibs.py` & `hyfi-1.2.1/src/hyfi/utils/iolibs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/utils/logging.py` & `hyfi-1.2.1/src/hyfi/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/utils/notebooks.py` & `hyfi-1.2.1/src/hyfi/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/utils/packages.py` & `hyfi-1.2.1/src/hyfi/utils/packages.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/src/hyfi/workflow/__init__.py` & `hyfi-1.2.1/src/hyfi/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.0/PKG-INFO` & `hyfi-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 1.2.0
+Version: 1.2.1
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 Home-page: https://hyfi.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

