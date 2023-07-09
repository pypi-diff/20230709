# Comparing `tmp/hyfi-1.1.0.tar.gz` & `tmp/hyfi-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-1.1.0.tar", max compression
+gzip compressed data, was "hyfi-1.2.0.tar", max compression
```

## Comparing `hyfi-1.1.0.tar` & `hyfi-1.2.0.tar`

### file list

```diff
@@ -1,110 +1,110 @@
--rw-r--r--   0        0        0     1071 2023-07-08 12:48:12.957773 hyfi-1.1.0/LICENSE
--rw-r--r--   0        0        0     1881 2023-07-08 12:48:12.957773 hyfi-1.1.0/README.md
--rw-r--r--   0        0        0     4863 2023-07-08 12:48:40.322071 hyfi-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4206 2023-07-08 12:48:12.957773 hyfi-1.1.0/src/hyfi/__cli__.py
--rw-r--r--   0        0        0     2550 2023-07-08 12:48:12.957773 hyfi-1.1.0/src/hyfi/__click__.py
--rw-r--r--   0        0        0      788 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/__global__/__init__.py
--rw-r--r--   0        0        0     9332 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/__global__/config.py
--rw-r--r--   0        0        0      733 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/__init__.py
--rw-r--r--   0        0        0       22 2023-07-08 12:48:40.246070 hyfi-1.1.0/src/hyfi/_version.py
--rw-r--r--   0        0        0     2376 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/about/__init__.py
--rw-r--r--   0        0        0     7229 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/batch/__init__.py
--rw-r--r--   0        0        0     1206 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/cached_path/__init__.py
--rw-r--r--   0        0        0    14373 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/cached_path/_cached_path.py
--rw-r--r--   0        0        0     1619 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/cached_path/cache_file.py
--rw-r--r--   0        0        0     1100 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/cached_path/common.py
--rw-r--r--   0        0        0     1921 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/cached_path/file_lock.py
--rw-r--r--   0        0        0     3441 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/cached_path/meta.py
--rw-r--r--   0        0        0     3247 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/cached_path/progress.py
--rw-r--r--   0        0        0     1437 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/cached_path/schemes/__init__.py
--rw-r--r--   0        0        0     1815 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/cached_path/schemes/beaker.py
--rw-r--r--   0        0        0     2862 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/cached_path/schemes/hf.py
--rw-r--r--   0        0        0     2942 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/cached_path/schemes/http.py
--rw-r--r--   0        0        0     3645 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/cached_path/schemes/scheme_client.py
--rw-r--r--   0        0        0     1222 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/cached_path/testing.py
--rw-r--r--   0        0        0     4799 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/cached_path/util.py
--rw-r--r--   0        0        0      464 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/cached_path/version.py
--rw-r--r--   0        0        0    32964 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/composer/__init__.py
--rw-r--r--   0        0        0     7426 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/composer/extended.py
--rw-r--r--   0        0        0     1933 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/composer/pydantic.py
--rw-r--r--   0        0        0        0 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      233 2023-07-08 12:48:40.246070 hyfi-1.1.0/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      553 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0        0 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/cmd/__init__.yaml
--rw-r--r--   0        0        0       49 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/cmd/about.yaml
--rw-r--r--   0        0        0      155 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0       83 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0       91 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/cmd/run_workflow.yaml
--rw-r--r--   0        0        0      320 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      569 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/copier/conf.yaml
--rw-r--r--   0        0        0      709 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      319 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      137 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      217 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/mode/__debug__.yaml
--rw-r--r--   0        0        0      921 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0       61 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/module/__init__.yaml
--rw-r--r--   0        0        0       73 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      880 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0      133 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/path/__task__.yaml
--rw-r--r--   0        0        0      291 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/path/dirnames/__init__.yaml
--rw-r--r--   0        0        0       76 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/pipe/__dataframe__.yaml
--rw-r--r--   0        0        0       77 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
--rw-r--r--   0        0        0       79 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
--rw-r--r--   0        0        0       70 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/pipe/__general_external_funcs__.yaml
--rw-r--r--   0        0        0       72 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/pipe/__general_instance_methods__.yaml
--rw-r--r--   0        0        0      128 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/pipe/__init__.yaml
--rw-r--r--   0        0        0      236 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/pipe/load_dataframes.yaml
--rw-r--r--   0        0        0      241 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/pipe/save_dataframes.yaml
--rw-r--r--   0        0        0       90 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/pipe/test_preprocessing.yaml
--rw-r--r--   0        0        0       69 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/pipeline/__init__.yaml
--rw-r--r--   0        0        0      388 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/pipeline/__test_dataframe__.yaml
--rw-r--r--   0        0        0      268 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/pipeline/__test_general__.yaml
--rw-r--r--   0        0        0      744 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0      170 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/project/__test__.yaml
--rw-r--r--   0        0        0       38 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/running/__init__.yaml
--rw-r--r--   0        0        0      161 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      359 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/task/__init__.yaml
--rw-r--r--   0        0        0      378 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/task/__test__.yaml
--rw-r--r--   0        0        0       99 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/workflow/__init__.yaml
--rw-r--r--   0        0        0       99 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/conf/workflow/__test__.yaml
--rw-r--r--   0        0        0     6548 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/copier/__init__.py
--rw-r--r--   0        0        0     5915 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/dotenv/__init__.py
--rw-r--r--   0        0        0        0 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/graphics/__init__.py
--rw-r--r--   0        0        0     8470 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/graphics/collage.py
--rw-r--r--   0        0        0     4538 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/graphics/motion.py
--rw-r--r--   0        0        0     7020 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/graphics/utils.py
--rw-r--r--   0        0        0     4228 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/joblib/__init__.py
--rw-r--r--   0        0        0      111 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/joblib/batch/__init__.py
--rw-r--r--   0        0        0     6312 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/joblib/batch/apply.py
--rw-r--r--   0        0        0     4779 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/joblib/batch/apply_batch.py
--rw-r--r--   0        0        0    13823 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/joblib/batch/batcher.py
--rw-r--r--   0        0        0    50273 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/main/__init__.py
--rw-r--r--   0        0        0      280 2023-07-08 12:48:12.961773 hyfi-1.1.0/src/hyfi/module/__init__.py
--rw-r--r--   0        0        0     4915 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/path/__init__.py
--rw-r--r--   0        0        0     4183 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/path/base.py
--rw-r--r--   0        0        0      782 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/path/batch.py
--rw-r--r--   0        0        0      599 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/path/dirnames.py
--rw-r--r--   0        0        0     1609 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/path/task.py
--rw-r--r--   0        0        0     5030 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/pipe/__init__.py
--rw-r--r--   0        0        0     1455 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/pipe/test.py
--rw-r--r--   0        0        0     8085 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/pipeline/__init__.py
--rw-r--r--   0        0        0     2900 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/pipeline/configs.py
--rw-r--r--   0        0        0     5618 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/project/__init__.py
--rw-r--r--   0        0        0        0 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/py.typed
--rw-r--r--   0        0        0     4268 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/task/__init__.py
--rw-r--r--   0        0        0     7014 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/task/batch.py
--rw-r--r--   0        0        0        0 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0     1314 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/utils/contexts.py
--rw-r--r--   0        0        0    30058 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/utils/datasets.py
--rw-r--r--   0        0        0     6568 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/utils/envs.py
--rw-r--r--   0        0        0    10857 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/utils/funcs.py
--rw-r--r--   0        0        0     3769 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/utils/gpumon.py
--rw-r--r--   0        0        0    20157 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/utils/iolibs.py
--rw-r--r--   0        0        0     2259 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0    12820 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/utils/notebooks.py
--rw-r--r--   0        0        0     6955 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/utils/packages.py
--rw-r--r--   0        0        0      382 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/utils/types.py
--rw-r--r--   0        0        0      753 2023-07-08 12:48:12.965773 hyfi-1.1.0/src/hyfi/workflow/__init__.py
--rw-r--r--   0        0        0     3393 1970-01-01 00:00:00.000000 hyfi-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-09 10:37:19.763455 hyfi-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1881 2023-07-09 10:37:19.763455 hyfi-1.2.0/README.md
+-rw-r--r--   0        0        0     4863 2023-07-09 10:37:46.971159 hyfi-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3312 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0     2477 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/__click__.py
+-rw-r--r--   0        0        0      792 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/__global__/__init__.py
+-rw-r--r--   0        0        0    10587 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/__global__/config.py
+-rw-r--r--   0        0        0      733 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-09 10:37:46.895160 hyfi-1.2.0/src/hyfi/_version.py
+-rw-r--r--   0        0        0     2376 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/about/__init__.py
+-rw-r--r--   0        0        0     7229 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/batch/__init__.py
+-rw-r--r--   0        0        0     1206 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/cached_path/__init__.py
+-rw-r--r--   0        0        0    14373 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/cached_path/_cached_path.py
+-rw-r--r--   0        0        0     1619 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/cached_path/cache_file.py
+-rw-r--r--   0        0        0     1100 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/cached_path/common.py
+-rw-r--r--   0        0        0     1921 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/cached_path/file_lock.py
+-rw-r--r--   0        0        0     3441 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/cached_path/meta.py
+-rw-r--r--   0        0        0     3247 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/cached_path/progress.py
+-rw-r--r--   0        0        0     1437 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/cached_path/schemes/__init__.py
+-rw-r--r--   0        0        0     1815 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/cached_path/schemes/beaker.py
+-rw-r--r--   0        0        0     2862 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/cached_path/schemes/hf.py
+-rw-r--r--   0        0        0     2942 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/cached_path/schemes/http.py
+-rw-r--r--   0        0        0     3645 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/cached_path/schemes/scheme_client.py
+-rw-r--r--   0        0        0     1222 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/cached_path/testing.py
+-rw-r--r--   0        0        0     4799 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/cached_path/util.py
+-rw-r--r--   0        0        0      464 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/cached_path/version.py
+-rw-r--r--   0        0        0    26040 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/composer/__init__.py
+-rw-r--r--   0        0        0     1933 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/composer/pydantic.py
+-rw-r--r--   0        0        0        0 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      233 2023-07-09 10:37:46.895160 hyfi-1.2.0/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      553 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0        0 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/conf/cmd/__init__.yaml
+-rw-r--r--   0        0        0       49 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      155 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0       83 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0       91 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/conf/cmd/run_workflow.yaml
+-rw-r--r--   0        0        0      328 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      569 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      709 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      322 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      137 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      198 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/conf/mode/__debug__.yaml
+-rw-r--r--   0        0        0      901 2023-07-09 10:37:19.767455 hyfi-1.2.0/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0       61 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       73 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      880 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      133 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/path/__task__.yaml
+-rw-r--r--   0        0        0      291 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/path/dirnames/__init__.yaml
+-rw-r--r--   0        0        0       76 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/pipe/__dataframe__.yaml
+-rw-r--r--   0        0        0       77 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
+-rw-r--r--   0        0        0       79 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
+-rw-r--r--   0        0        0       70 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/pipe/__general_external_funcs__.yaml
+-rw-r--r--   0        0        0       72 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/pipe/__general_instance_methods__.yaml
+-rw-r--r--   0        0        0      128 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/pipe/__init__.yaml
+-rw-r--r--   0        0        0      236 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/pipe/load_dataframes.yaml
+-rw-r--r--   0        0        0      241 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/pipe/save_dataframes.yaml
+-rw-r--r--   0        0        0       90 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/pipe/test_preprocessing.yaml
+-rw-r--r--   0        0        0       69 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/pipeline/__init__.yaml
+-rw-r--r--   0        0        0      388 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/pipeline/__test_dataframe__.yaml
+-rw-r--r--   0        0        0      268 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/pipeline/__test_general__.yaml
+-rw-r--r--   0        0        0      744 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0      170 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/project/__test__.yaml
+-rw-r--r--   0        0        0       38 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/running/__init__.yaml
+-rw-r--r--   0        0        0      161 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      305 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      208 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/task/__test__.yaml
+-rw-r--r--   0        0        0       99 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/workflow/__init__.yaml
+-rw-r--r--   0        0        0       99 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/conf/workflow/__test__.yaml
+-rw-r--r--   0        0        0     6558 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/copier/__init__.py
+-rw-r--r--   0        0        0     5915 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/dotenv/__init__.py
+-rw-r--r--   0        0        0     3517 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/graphics/__init__.py
+-rw-r--r--   0        0        0     8470 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/graphics/collage.py
+-rw-r--r--   0        0        0     4538 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/graphics/motion.py
+-rw-r--r--   0        0        0     7020 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/graphics/utils.py
+-rw-r--r--   0        0        0     4228 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/joblib/__init__.py
+-rw-r--r--   0        0        0      111 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/joblib/batch/__init__.py
+-rw-r--r--   0        0        0     6312 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/joblib/batch/apply.py
+-rw-r--r--   0        0        0     4779 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/joblib/batch/apply_batch.py
+-rw-r--r--   0        0        0    13823 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/joblib/batch/batcher.py
+-rw-r--r--   0        0        0    13620 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/main/__init__.py
+-rw-r--r--   0        0        0      280 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/module/__init__.py
+-rw-r--r--   0        0        0     4915 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/path/__init__.py
+-rw-r--r--   0        0        0     4183 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/path/base.py
+-rw-r--r--   0        0        0      782 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/path/batch.py
+-rw-r--r--   0        0        0      599 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/path/dirnames.py
+-rw-r--r--   0        0        0     1609 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/path/task.py
+-rw-r--r--   0        0        0     5030 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/pipe/__init__.py
+-rw-r--r--   0        0        0     1455 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/pipe/test.py
+-rw-r--r--   0        0        0     8032 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/pipeline/__init__.py
+-rw-r--r--   0        0        0     2874 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/pipeline/configs.py
+-rw-r--r--   0        0        0     5618 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/py.typed
+-rw-r--r--   0        0        0     4268 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/task/__init__.py
+-rw-r--r--   0        0        0     7041 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/task/batch.py
+-rw-r--r--   0        0        0        0 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0    12742 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/utils/conf.py
+-rw-r--r--   0        0        0     1314 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/utils/contexts.py
+-rw-r--r--   0        0        0    30089 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/utils/datasets.py
+-rw-r--r--   0        0        0     6568 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/utils/envs.py
+-rw-r--r--   0        0        0    10857 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/utils/funcs.py
+-rw-r--r--   0        0        0     4930 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/utils/gpumon.py
+-rw-r--r--   0        0        0    20157 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/utils/iolibs.py
+-rw-r--r--   0        0        0     2259 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0    12820 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/utils/notebooks.py
+-rw-r--r--   0        0        0     6955 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/utils/packages.py
+-rw-r--r--   0        0        0      382 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/utils/types.py
+-rw-r--r--   0        0        0      753 2023-07-09 10:37:19.771455 hyfi-1.2.0/src/hyfi/workflow/__init__.py
+-rw-r--r--   0        0        0     3393 1970-01-01 00:00:00.000000 hyfi-1.2.0/PKG-INFO
```

### Comparing `hyfi-1.1.0/LICENSE` & `hyfi-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/README.md` & `hyfi-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/pyproject.toml` & `hyfi-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi"
-version = "1.1.0"
+version = "1.2.0"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
```

### Comparing `hyfi-1.1.0/src/hyfi/__cli__.py` & `hyfi-1.2.0/src/hyfi/__cli__.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,68 +3,52 @@
 from typing import Optional
 
 import hydra
 from omegaconf import DictConfig
 
 from hyfi.__global__ import __about__, __hydra_version_base__
 from hyfi.__global__.config import HyfiConfig
-from hyfi.copier import Copier
-from hyfi.main import HyFI, _about
+from hyfi.main import HyFI
 from hyfi.utils.logging import LOGGING
 
 logger = LOGGING.getLogger(__name__)
 
 
 __config_path__ = "conf"
 __config_name__ = "config"
 
 
 def about(**args):
     """
     Print the about information for Hyfi.
     This is a wrapper around _about which takes a HyfiConfig as an argument
     """
-    cfg = HyfiConfig(**args)
-    _about(cfg)
+    HyFI.run(args)
 
 
 def run_copy(**args):
     """
     Copy all config files to the current working directory.
     This is a wrapper around HyfiConfig to allow us to pass arguments to it.
     """
-    if "copier" not in args:
-        raise ValueError("No copier configuration found")
-    cfg = HyFI.to_dict(args["copier"])
-    print(type(cfg), cfg)
-    with Copier(**cfg) as worker:
-        worker.run_copy()
+    HyFI.run(args, "copier")
 
 
 def run_task(**args):
     """
     Run a task. This is a wrapper around HyFI
     """
-    # Check if task is not in args
-    if "task" not in args:
-        raise ValueError("No task configuration found")
-    project = HyFI.init_project(**args["project"]) if "project" in args else None
-    task = HyFI.task_config(**args["task"])
-    HyFI.run_task(task, project=project)
+    HyFI.run(args, "task")
 
 
 def run_workflow(**args):
     """
     Run a workflow. This is a wrapper around HyFI. run_workflow
     """
-    # Raised if no workflow configuration is specified.
-    if "workflow" not in args:
-        raise ValueError("No workflow configuration found")
-    workflow = HyFI.workflow_config(**args["workflow"])
-    HyFI.run_workflow(workflow)
+    HyFI.run(args, "workflow")
 
 
 def cli_main(cfg: DictConfig) -> None:
     """
     Main function for the command line interface.
     Initializes Hydra and instantiates the class.
     Prints the configuration to standard out if verbose is set to True
@@ -73,41 +57,35 @@
         cfg: Configuration dictionary to be used for instantiation
 
     Returns:
         None if everything went fine otherwise an error is raised
         to indicate the reason for the failure
     """
     hyfi = HyfiConfig(**cfg)  # type: ignore
-    hyfi.initialize()
     verbose = hyfi.verbose
-    app_name = hyfi.app_name
-    print_config = hyfi.print_config
-    resolve = hyfi.resolve
-
     # Print out the command line interface for the application.
     if verbose:
+        app_name = hyfi.app_name
         print(f"## Command Line Interface for {app_name} ##")
-    HyFI.initialize()
 
-    # Print the configuration to the console.
-    if print_config:
         # Prints the configuration to the console.
-        if resolve:
+        if hyfi.resolve:
             logger.info("## hydra configuration resolved ##")
-            HyFI.pprint(cfg)
+            HyFI.print(cfg)
         else:
             logger.info("## hydra configuration ##")
             print(HyFI.to_yaml(cfg))
 
-    # Prints out the working directory and original working directory.
-    if verbose:
         logger.info("Hydra working directory : %s", {os.getcwd()})
         logger.info("Orig working directory  : %s", {hydra.utils.get_original_cwd()})
 
-    HyFI.instantiate(cfg)
+    if HyFI.is_instantiatable(cfg):
+        HyFI.instantiate(cfg)
+    else:
+        hyfi.run()
 
     HyFI.terminate()
 
 
 def hydra_main(
     config_path: Optional[str] = __config_path__,
     config_name: Optional[str] = __config_name__,
@@ -121,14 +99,14 @@
                         Relative paths are interpreted relative to the declaring python
                         file. Alternatively, you can use the prefix `pkg://` to specify
                         a python package to add to the searchpath.
                         If config_path is None no directory is added to the Config search path.
         config_name: The name of the config (usually the file name without the .yaml extension)
     """
     # Returns the path to the config file.
-    # if config_path is None:
-    config_path = __about__.config_path
+    if config_path is None:
+        config_path = __about__.config_path
     hydra.main(
         config_path=config_path,
         config_name=config_name,
         version_base=__hydra_version_base__,
     )(cli_main)()
```

### Comparing `hyfi-1.1.0/src/hyfi/__click__.py` & `hyfi-1.2.0/src/hyfi/__click__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import click
 
 from hyfi.__global__ import __hyfi_path__
 from hyfi.__global__.config import HyfiConfig
 from hyfi._version import __version__
 from hyfi.copier import Copier
-from hyfi.main import _about
 from hyfi.utils.logging import LOGGING
 
 logger = LOGGING.getLogger(__name__)
 
 
 @click.group()
 @click.version_option(__version__)
@@ -68,17 +67,15 @@
 
 
 @cli.command()
 def about():
     """
     Print the about information for Hyfi.
     """
-    cfg = HyfiConfig()
-    cfg.about.version = __version__
-    _about(cfg)
+    HyfiConfig().print_about()
 
 
 @cli.command()
 @click.option(
     "--uninstall",
     "-u",
     is_flag=True,
```

### Comparing `hyfi-1.1.0/src/hyfi/__global__/__init__.py` & `hyfi-1.2.0/src/hyfi/__global__/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 class HydraConfig(BaseModel):
     """Global configuration for Hydra"""
 
     hyfi_config_path: str = __about__.config_path
     hyfi_config_module: str = __about__.config_module
-    hyfi_user_config_path: str = ""
+    hyfi_user_config_path: str = "conf"
 
 
 __hydra_config__ = HydraConfig()
 
 
 def __hyfi_path__():
     """Returns the path to the HyFI root folder"""
```

### Comparing `hyfi-1.1.0/src/hyfi/__global__/config.py` & `hyfi-1.2.0/src/hyfi/__global__/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,43 +12,48 @@
     PrivateAttr,
     field_validator,
     model_validator,
 )
 
 from hyfi.__global__ import __about__, __hydra_config__
 from hyfi.about import AboutConfig, __app_name__, __version__
+from hyfi.copier import Copier
 from hyfi.dotenv import DotEnvConfig
+from hyfi.pipeline import PipelineConfig, PIPELINEs
 from hyfi.project import ProjectConfig
 from hyfi.task import TaskConfig
+from hyfi.utils.conf import CONFs
 from hyfi.utils.envs import ENVs
 from hyfi.utils.logging import LOGGING
 from hyfi.utils.notebooks import NBs
+from hyfi.workflow import WorkflowConfig
 
 logger = LOGGING.getLogger(__name__)
 
 
 class HyfiConfig(BaseModel):
     """HyFI root config class.  This class is used to store the configuration"""
 
     hyfi_config_path: str = __about__.config_path
     hyfi_config_module: str = __about__.config_module
-    hyfi_user_config_path: str = ""
+    hyfi_user_config_path: str = "conf"
 
     debug_mode: bool = False
-    print_config: bool = False
     resolve: bool = False
     verbose: bool = False
     logging_level: str = "WARNING"
 
     hydra: Optional[DictConfig] = None
 
     about: Optional[AboutConfig] = None
     copier: Optional[DictConfig] = None
     project: Optional[ProjectConfig] = None
+    pipeline: Optional[PipelineConfig] = None
     task: Optional[TaskConfig] = None
+    workflow: Optional[WorkflowConfig] = None
 
     _version_: str = PrivateAttr(__version__())
     _initilized_: bool = PrivateAttr(False)
 
     model_config = ConfigDict(
         arbitrary_types_allowed=True,
         validate_assignment=True,
@@ -270,14 +275,39 @@
     def dotenv(self):
         return DotEnvConfig()  # type: ignore
 
     @property
     def osenv(self):
         return os.environ
 
+    def print_about(self):
+        about = AboutConfig() if self.about is None else self.about
+        pkg_name = about.__package_name__
+        name = about.name
+        print()
+        for k, v in about.model_dump().items():
+            if k.startswith("_"):
+                continue
+            print(f"{k:11} : {v}")
+        if pkg_name:
+            print(f"\nExecute `{pkg_name} --help` to see what you can do with {name}")
+
+    def run(self, target: Optional[str] = None):
+        """Run the config"""
+        if self.workflow is not None and (target is None or target == "workflow"):
+            PIPELINEs.run_workflow(self.workflow)
+        elif self.task is not None and (target is None or target == "task"):
+            PIPELINEs.run_task(self.task, project=self.project)
+        elif self.copier is not None and (target is None or target == "copier"):
+            args = CONFs.to_dict(self.copier)
+            with Copier(**args) as worker:
+                worker.run_copy()
+        else:
+            self.print_about()
+
 
 __global_config__ = HyfiConfig()
 if __global_config__.about:
     __global_config__.about.version = __version__()
 
 
 def __search_package_path__():
```

### Comparing `hyfi-1.1.0/src/hyfi/__init__.py` & `hyfi-1.2.0/src/hyfi/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/about/__init__.py` & `hyfi-1.2.0/src/hyfi/about/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/batch/__init__.py` & `hyfi-1.2.0/src/hyfi/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/cached_path/__init__.py` & `hyfi-1.2.0/src/hyfi/cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/cached_path/_cached_path.py` & `hyfi-1.2.0/src/hyfi/cached_path/_cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/cached_path/cache_file.py` & `hyfi-1.2.0/src/hyfi/cached_path/cache_file.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/cached_path/common.py` & `hyfi-1.2.0/src/hyfi/cached_path/common.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/cached_path/file_lock.py` & `hyfi-1.2.0/src/hyfi/cached_path/file_lock.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/cached_path/meta.py` & `hyfi-1.2.0/src/hyfi/cached_path/meta.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/cached_path/progress.py` & `hyfi-1.2.0/src/hyfi/cached_path/progress.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/cached_path/schemes/__init__.py` & `hyfi-1.2.0/src/hyfi/cached_path/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/cached_path/schemes/beaker.py` & `hyfi-1.2.0/src/hyfi/cached_path/schemes/beaker.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/cached_path/schemes/hf.py` & `hyfi-1.2.0/src/hyfi/cached_path/schemes/hf.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/cached_path/schemes/http.py` & `hyfi-1.2.0/src/hyfi/cached_path/schemes/http.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/cached_path/schemes/scheme_client.py` & `hyfi-1.2.0/src/hyfi/cached_path/schemes/scheme_client.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/cached_path/testing.py` & `hyfi-1.2.0/src/hyfi/cached_path/testing.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/cached_path/util.py` & `hyfi-1.2.0/src/hyfi/cached_path/util.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/composer/__init__.py` & `hyfi-1.2.0/src/hyfi/composer/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 """
     Hydra configuration management
 """
 import collections.abc
-import json
 import os
 import re
 from enum import Enum
 from pathlib import Path
-from typing import IO, Any, Dict, List, Mapping, Optional, Set, Tuple, Union
+from typing import Any, Callable, Dict, List, Mapping, Optional, Set, Tuple, Union
 
 import hydra
-from omegaconf import DictConfig, ListConfig, OmegaConf, SCMode
+from omegaconf import DictConfig
 from pydantic import BaseModel, ConfigDict, PrivateAttr, model_validator
 
 from hyfi.__global__ import (
     __about__,
     __hydra_config__,
     __hydra_default_config_group_value__,
     __hydra_version_base__,
 )
+from hyfi.utils.conf import CONFs
 from hyfi.utils.logging import LOGGING
+from hyfi.utils.packages import PKGs
 
 if level := os.environ.get("HYFI_LOG_LEVEL"):
     LOGGING.setLogger(level)
 logger = LOGGING.getLogger(__name__)
 
-DictKeyType = Union[str, int, Enum, float, bool]
-
 
 class SpecialKeys(str, Enum):
     """Special keys in configs used by HyFI."""
 
     CALL = "_call_"
     CONFIG = "_config_"
     CONFIG_GROUP = "_config_group_"
@@ -44,15 +43,15 @@
     RECURSIVE = "_recursive_"
     RUN = "_run_"
     TARGET = "_target_"
     TYPE = "_type_"
     WITH = "_with_"
 
 
-class Composer(BaseModel):
+class Composer(BaseModel, CONFs):
     """
     Compose a configuration by applying overrides
     """
 
     config_group: Union[str, None] = None
     overrides: Union[List[str], None] = None
     config_data: Union[Dict[str, Any], DictConfig, None] = None
@@ -189,83 +188,14 @@
     def __hash__(self):
         return hash(self._cfg_)
 
     def __getstate__(self):
         return self._cfg_
 
     @staticmethod
-    def select(
-        cfg: Any,
-        key: str,
-        default: Any = None,
-        throw_on_resolution_failure: bool = True,
-        throw_on_missing: bool = False,
-    ):
-        """
-        Wrapper for OmegaConf. select value from a config object using a key.
-
-        Args:
-            cfg: Config node to select from
-            key: Key to select
-            default: Default value to return if key is not found
-            throw_on_resolution_failure: Raise an exception if an interpolation
-                resolution error occurs, otherwise return None
-            throw_on_missing: Raise an exception if an attempt to select a missing key (with the value '???')
-                is made, otherwise return None
-
-        Returns:
-            selected value or None if not found.
-        """
-        key = key.replace("/", ".")
-        return OmegaConf.select(
-            cfg,
-            key=key,
-            default=default,
-            throw_on_resolution_failure=throw_on_resolution_failure,
-            throw_on_missing=throw_on_missing,
-        )
-
-    @staticmethod
-    def to_dict(cfg: Any) -> Any:
-        """
-        Convert a config to a dict
-
-        Args:
-            cfg: The config to convert.
-
-        Returns:
-            The dict representation of the config.
-        """
-        # Convert a config object to a config object.
-        if isinstance(cfg, dict):
-            cfg = Composer.to_config(cfg)
-        # Returns a container for the given config.
-        if isinstance(cfg, (DictConfig, ListConfig)):
-            return OmegaConf.to_container(
-                cfg,
-                resolve=True,
-                throw_on_missing=False,
-                structured_config_mode=SCMode.DICT,
-            )
-        return cfg
-
-    @staticmethod
-    def to_config(cfg: Any) -> Union[DictConfig, ListConfig]:
-        """
-        Convert a config object to OmegaConf
-
-        Args:
-            cfg: The config to convert.
-
-        Returns:
-            A Config object that corresponds to the given config.
-        """
-        return OmegaConf.create(cfg)
-
-    @staticmethod
     def hydra_compose(
         root_config_name: Union[str, None] = None,
         config_module: Union[str, None] = None,
         overrides: Union[List[str], None] = None,
     ):
         is_initialized = hydra.core.global_hydra.GlobalHydra.instance().is_initialized()  # type: ignore
         config_module = config_module or __hydra_config__.hyfi_config_module
@@ -415,194 +345,27 @@
                 throw_on_missing=throw_on_missing,
                 throw_on_resolution_failure=throw_on_resolution_failure,
             )
         # logger.debug("Composed config: %s", OmegaConf.to_yaml(_to_dict(cfg)))
         return cfg
 
     @staticmethod
-    def print(cfg: Any, resolve: bool = True, **kwargs):
-        """
-        Prints the configuration object in a human-readable format.
-
-        Args:
-            cfg (Any): The configuration object to print.
-            resolve (bool, optional): Whether to resolve the configuration object before printing. Defaults to True.
-            **kwargs: Additional keyword arguments to pass to the pprint.pprint function.
-
-        Returns:
-            None
-        """
-        import pprint
-
-        if Composer.is_config(cfg):
-            if resolve:
-                pprint.pprint(Composer.to_dict(cfg), **kwargs)
-            else:
-                pprint.pprint(cfg, **kwargs)
-        else:
-            print(cfg)
-
-    @staticmethod
-    def is_config(cfg: Any):
-        """
-        Determines whether the input object is a valid configuration object.
-
-        Args:
-            cfg (Any): The object to check.
-
-        Returns:
-            bool: True if the object is a valid configuration object, False otherwise.
-        """
-        return isinstance(cfg, (DictConfig, dict))
-
-    @staticmethod
-    def is_list(cfg: Any):
-        """
-        Determines whether the input object is a valid list configuration object.
-
-        Args:
-            cfg (Any): The object to check.
-
-        Returns:
-            bool: True if the object is a valid list configuration object, False otherwise.
-        """
-        return isinstance(cfg, (ListConfig, list))
-
-    @staticmethod
     def is_instantiatable(cfg: Any):
         """
         Determines whether the input configuration object is instantiatable.
 
         Args:
             cfg (Any): The configuration object to check.
 
         Returns:
             bool: True if the configuration object is instantiatable, False otherwise.
         """
         return Composer.is_config(cfg) and SpecialKeys.TARGET in cfg
 
     @staticmethod
-    def load(file_: Union[str, Path, IO[Any]]) -> Union[DictConfig, ListConfig]:
-        """
-        Load a configuration file and return a configuration object.
-
-        Args:
-            file_ (Union[str, Path, IO[Any]]): The path to the configuration file or a file-like object.
-
-        Returns:
-            Union[DictConfig, ListConfig]: The configuration object.
-        """
-        return OmegaConf.load(file_)
-
-    @staticmethod
-    def save(config: Any, f: Union[str, Path, IO[Any]], resolve: bool = False) -> None:
-        """
-        Save a configuration object to a file.
-
-        Args:
-            config (Any): The configuration object to save.
-            f (Union[str, Path, IO[Any]]): The path to the file or a file-like object.
-            resolve (bool, optional): Whether to resolve the configuration object before saving. Defaults to False.
-        """
-        os.makedirs(os.path.dirname(str(f)), exist_ok=True)
-        OmegaConf.save(config, f, resolve=resolve)
-
-    @staticmethod
-    def save_json(
-        json_dict: dict,
-        f: Union[str, Path, IO[Any]],
-        indent=4,
-        ensure_ascii=False,
-        default=None,
-        encoding="utf-8",
-        **kwargs,
-    ):
-        """
-        Save a dictionary to a JSON file.
-
-        Args:
-            json_dict (dict): The dictionary to save.
-            f (Union[str, Path, IO[Any]]): The path to the file or a file-like object.
-            indent (int, optional): The number of spaces to use for indentation. Defaults to 4.
-            ensure_ascii (bool, optional): Whether to escape non-ASCII characters. Defaults to False.
-            default (Any, optional): A function to convert non-serializable objects. Defaults to None.
-            encoding (str, optional): The encoding to use. Defaults to "utf-8".
-            **kwargs: Additional arguments to pass to json.dump().
-        """
-        f = str(f)
-        os.makedirs(os.path.dirname(f), exist_ok=True)
-        with open(f, "w", encoding=encoding) as f:
-            json.dump(
-                json_dict,
-                f,
-                indent=indent,
-                ensure_ascii=ensure_ascii,
-                default=default,
-                **kwargs,
-            )
-
-    @staticmethod
-    def load_json(f: Union[str, Path, IO[Any]], encoding="utf-8", **kwargs) -> dict:
-        """
-        Load a JSON file into a dictionary.
-
-        Args:
-            f (Union[str, Path, IO[Any]]): The path to the file or a file-like object.
-            encoding (str, optional): The encoding to use. Defaults to "utf-8".
-            **kwargs: Additional arguments to pass to json.load().
-
-        Returns:
-            dict: The dictionary loaded from the JSON file.
-        """
-        f = str(f)
-        with open(f, "r", encoding=encoding) as f:
-            return json.load(f, **kwargs)
-
-    @staticmethod
-    def update(_dict: Mapping[str, Any], _overrides: Mapping[str, Any]) -> Mapping:
-        """
-        Update a dictionary with overrides.
-
-        Args:
-            _dict (Mapping[str, Any]): The dictionary to update.
-            _overrides (Mapping[str, Any]): The dictionary with overrides.
-
-        Returns:
-            Mapping: The updated dictionary.
-        """
-        for k, v in _overrides.items():
-            if isinstance(v, collections.abc.Mapping):
-                _dict[k] = Composer.update((_dict.get(k) or {}), v)  # type: ignore
-            else:
-                _dict[k] = v  # type: ignore
-        return _dict
-
-    @staticmethod
-    def replace_keys(_dict: Mapping[str, Any], old_key: str, new_key: str) -> Mapping:
-        """
-        Replace a key in a dictionary.
-
-        Args:
-            _dict (Mapping[str, Any]): The dictionary to update.
-            old_key (str): The old key to replace.
-            new_key (str): The new key to use.
-
-        Returns:
-            Mapping: The updated dictionary.
-        """
-        _new_dict = {}
-        for k, v in _dict.items():
-            key = new_key if k == old_key else k
-            if isinstance(v, collections.abc.Mapping):
-                _new_dict[key] = Composer.replace_keys(v, old_key, new_key)
-            else:
-                _new_dict[key] = v
-        return _new_dict
-
-    @staticmethod
     def replace_special_keys(_dict: Mapping[str, Any]) -> Mapping:
         """
         Replace special keys in a dictionary.
 
         Args:
             _dict (Mapping[str, Any]): The dictionary to update.
 
@@ -615,164 +378,153 @@
             if isinstance(v, collections.abc.Mapping):
                 _new_dict[key] = Composer.replace_special_keys(v)
             else:
                 _new_dict[key] = v
         return _new_dict
 
     @staticmethod
-    def merge(
-        *configs: Union[
-            DictConfig,
-            ListConfig,
-            Dict[DictKeyType, Any],
-            List[Any],
-            Tuple[Any, ...],
-            Any,
-        ],
-    ) -> Union[ListConfig, DictConfig]:
-        """
-        Merge a list of previously created configs into a single one.
-
-        Args:
-            *configs: Input configs.
-
-        Returns:
-            Union[ListConfig, DictConfig]: The merged config object.
-        """
-        return OmegaConf.merge(*configs)
-
-    @staticmethod
-    def merge_as_dict(
-        *configs: Union[
-            DictConfig,
-            ListConfig,
-            Dict[DictKeyType, Any],
-            List[Any],
-            Tuple[Any, ...],
-            Any,
-        ],
-    ) -> Union[ListConfig, DictConfig]:
+    def generate_alias_for_special_keys(key: str) -> str:
         """
-        Merge a list of previously created configs into a single dictionary.
+        Generate an alias for special keys.
+        _with_ -> run_with
+        _pipe_ -> run_pipe
+        _run_ -> run
 
         Args:
-            *configs: Input configs.
+            key (str): The special key to generate an alias for.
 
         Returns:
-            Union[ListConfig, DictConfig]: The merged config object as a dictionary.
+            str: The alias for the special key.
         """
-        return Composer.to_dict(OmegaConf.merge(*configs))
+        # replace the exact `with`, `pipe` with `run_with`, `run_pipe`
+        key_ = re.sub(r"^with$", "run_with", key)
+        # replace the prefix `_` with `run_`
+        key_ = re.sub(r"^_with_$", "run_with", key_)
+        key_ = re.sub(r"^_pipe_$", "pipe_target", key_)
+        key_ = re.sub(r"^_run_$", "run", key_)
+        return key_
 
     @staticmethod
-    def to_yaml(cfg: Any, resolve: bool = False, sort_keys: bool = False) -> str:
-        """
-        Convert the input config object to a YAML string.
-
-        Args:
-            cfg (Any): The input config object.
-            resolve (bool, optional): Whether to resolve the config object before converting it to YAML. Defaults to False.
-            sort_keys (bool, optional): Whether to sort the keys in the resulting YAML string. Defaults to False.
-
+    def partial(
+        config: Union[str, Dict],
+        *args: Any,
+        **kwargs: Any,
+    ) -> Callable:
+        """
+        Returns a callable object that is a partial version of the function or class specified in the config object.
+
+        Args:
+            config: An config object describing what to call and what params to use.
+                    In addition to the parameters, the config must contain:
+                    _target_ : target class or callable name (str)
+                    And may contain:
+                    _partial_: If True, return functools.partial wrapped method or object
+                                False by default. Configure per target.
+            args: Optional positional parameters pass-through
+            kwargs: Optional named parameters to override
+                    parameters in the config object. Parameters not present
+                    in the config objects are being passed as is to the target.
+                    IMPORTANT: dataclasses instances in kwargs are interpreted as config
+                                and cannot be used as passthrough
         Returns:
-            str: The YAML string representation of the input config object.
+            A callable object that is a partial version of the function or class specified in the config object.
         """
-        if resolve:
-            cfg = Composer.to_dict(cfg)
-        return OmegaConf.to_yaml(cfg, resolve=resolve, sort_keys=sort_keys)
+        if isinstance(config, str):
+            config = {SpecialKeys.TARGET.value: config}
+        else:
+            config = Composer.to_dict(config)
+        if not isinstance(config, dict):
+            raise ValueError("config must be a dict or a str")
+        config[SpecialKeys.PARTIAL.value] = True
+        rc_kwargs_ = config.pop(SpecialKeys.KWARGS, {})
+        if rc_kwargs_ and kwargs:
+            kwargs.update(rc_kwargs_)
+        return Composer.instantiate(config, *args, **kwargs)
 
     @staticmethod
-    def to_container(
-        cfg: Any,
-        resolve: bool = False,
-        throw_on_missing: bool = False,
-        enum_to_str: bool = False,
-        structured_config_mode: SCMode = SCMode.DICT,
-    ):
+    def instantiate(config: Any, *args: Any, **kwargs: Any) -> Any:
         """
-        Convert the input config object to a nested container (e.g. dictionary).
+        Instantiates an object using the provided config object.
 
         Args:
-            cfg (Any): The input config object.
-            resolve (bool, optional): Whether to resolve the config object before converting it to a container. Defaults to False.
-            throw_on_missing (bool, optional): Whether to throw an exception if a missing key is encountered. Defaults to False.
-            enum_to_str (bool, optional): Whether to convert enum values to strings. Defaults to False.
-            structured_config_mode (SCMode, optional): The structured config mode to use. Defaults to SCMode.DICT.
+            config: An config object describing what to call and what params to use.
+                    In addition to the parameters, the config must contain:
+                    _target_ : target class or callable name (str)
+                    And may contain:
+                    _args_: List-like of positional arguments to pass to the target
+                    _recursive_: Construct nested objects as well (bool).
+                                    False by default.
+                                    may be overridden via a _recursive_ key in
+                                    the kwargs
+                    _convert_: Conversion strategy
+                            none    : Passed objects are DictConfig and ListConfig, default
+                            partial : Passed objects are converted to dict and list, with
+                                    the exception of Structured Configs (and their fields).
+                            all     : Passed objects are dicts, lists and primitives without
+                                    a trace of OmegaConf containers
+                    _partial_: If True, return functools.partial wrapped method or object
+                                False by default. Configure per target.
+                    _args_: List-like of positional arguments
+            args: Optional positional parameters pass-through
+            kwargs: Optional named parameters to override
+                    parameters in the config object. Parameters not present
+                    in the config objects are being passed as is to the target.
+                    IMPORTANT: dataclasses instances in kwargs are interpreted as config
+                                and cannot be used as passthrough
 
         Returns:
-            The nested container (e.g. dictionary) representation of the input config object.
+            if _target_ is a class name: the instantiated object
+            if _target_ is a callable: the return value of the call
         """
-        return OmegaConf.to_container(
-            cfg,
-            resolve=resolve,
-            throw_on_missing=throw_on_missing,
-            enum_to_str=enum_to_str,
-            structured_config_mode=structured_config_mode,
-        )
+        verbose = config.get("verbose", False)
+        if not Composer.is_instantiatable(config):
+            if verbose:
+                logger.info("Config is not instantiatable, returning config")
+            return config
+        _recursive_ = config.get(SpecialKeys.RECURSIVE, False)
+        if SpecialKeys.RECURSIVE not in kwargs:
+            kwargs[SpecialKeys.RECURSIVE.value] = _recursive_
+        if verbose:
+            logger.info("instantiating %s ...", config.get(SpecialKeys.TARGET))
+        return hydra.utils.instantiate(config, *args, **kwargs)
 
     @staticmethod
-    def ensure_list(value):
+    def getsource(obj: Any) -> str:
         """
-        Ensure that the given value is a list. If the value is None or an empty string, an empty list is returned.
-        If the value is already a list, it is returned as is. If the value is a string, it is returned as a list
-        containing only that string. Otherwise, the value is converted to a dictionary using the Composer.to_dict method
-        and the resulting dictionary is returned as a list.
+        Return the source code of the object.
 
         Args:
-            value (Any): The value to ensure as a list.
+            obj: The object to get the source code of.
 
         Returns:
-            List: The value as a list.
-        """
-        if not value:
-            return []
-        elif isinstance(value, str):
-            return [value]
-        return Composer.to_dict(value)
+            The source code of the object as a string.
 
-    @staticmethod
-    def ensure_kwargs(_kwargs, _fn):
-        """
-        Ensure that the given keyword arguments are valid for the given function.
-
-        Args:
-            _kwargs (dict): The keyword arguments to validate.
-            _fn (callable): The function to validate the keyword arguments against.
-
-        Returns:
-            dict: The valid keyword arguments for the given function.
         """
-        from inspect import getfullargspec as getargspec
-
-        if callable(_fn):
-            args = getargspec(_fn).args
-            logger.info(f"args of {_fn}: {args}")
-            return {k: v for k, v in _kwargs.items() if k in args}
-        return _kwargs
+        try:
+            target_string = ""
+            if Composer.is_config(obj):
+                if SpecialKeys.TARGET in obj:
+                    target_string = obj[SpecialKeys.TARGET]
+            elif isinstance(obj, str):
+                target_string = obj
+            return PKGs.getsource(target_string) if target_string else ""
+        except Exception as e:
+            logger.error(f"Error getting source: {e}")
+            return ""
 
     @staticmethod
-    def generate_alias_for_special_keys(key: str) -> str:
+    def viewsource(obj: Any):
         """
-        Generate an alias for special keys.
-        _with_ -> run_with
-        _pipe_ -> run_pipe
-        _run_ -> run
+        Print the source code of the object.
 
         Args:
-            key (str): The special key to generate an alias for.
+            obj: The object to print the source code of.
 
-        Returns:
-            str: The alias for the special key.
         """
-        # replace the exact `with`, `pipe` with `run_with`, `run_pipe`
-        key_ = re.sub(r"^with$", "run_with", key)
-        # replace the prefix `_` with `run_`
-        key_ = re.sub(r"^_with_$", "run_with", key_)
-        key_ = re.sub(r"^_pipe_$", "pipe_target", key_)
-        key_ = re.sub(r"^_run_$", "run", key_)
-        return key_
+        print(Composer.getsource(obj))
 
 
 class BaseConfig(BaseModel):
     """
     Base class for all config classes.
     """
```

### Comparing `hyfi-1.1.0/src/hyfi/composer/pydantic.py` & `hyfi-1.2.0/src/hyfi/composer/pydantic.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/conf/batch/__init__.yaml` & `hyfi-1.2.0/src/hyfi/conf/batch/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/conf/copier/conf.yaml` & `hyfi-1.2.0/src/hyfi/conf/copier/conf.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-1.2.0/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-1.2.0/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/conf/mode/__init__.yaml` & `hyfi-1.2.0/src/hyfi/conf/mode/__init__.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # @package _global_
 debug_mode: false
-print_config: false
 resolve: true
 verbose: false
 ignore_warnings: true
 logging_level: ${oc.env:HYFI_LOG_LEVEL,WARNING}
 hydra_log_dir: ${oc.select:project.path.project_logs, ${oc.select:task.path.task_logs, ${alt:${oc.env:HYFI_GLOBAL_ROOT,null},${__home_path__:}/.hyfi}/logs}}/hydra
 
 hydra:
```

### Comparing `hyfi-1.1.0/src/hyfi/conf/path/__init__.yaml` & `hyfi-1.2.0/src/hyfi/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/conf/project/__init__.yaml` & `hyfi-1.2.0/src/hyfi/conf/project/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/copier/__init__.py` & `hyfi-1.2.0/src/hyfi/copier/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,16 +73,16 @@
 
         verbose:
             When `True`, show all output.
     """
 
     src_path: Path = field(default=Path("conf"))
     dst_path: Path = field(default=Path("."))
-    filetypes: Optional[Union[List, str]] = field(default=None)
-    exclude: Optional[Union[List, str]] = field(default=None)
+    filetypes: Optional[Union[List[str], str]] = field(default=None)
+    exclude: Optional[Union[List[str], str]] = field(default=None)
     skip_if_exists: bool = False
     cleanup_on_error: bool = True
     overwrite: bool = False
     dry_run: bool = False
     verbose: bool = True
 
     def __post_init__(self):
```

### Comparing `hyfi-1.1.0/src/hyfi/dotenv/__init__.py` & `hyfi-1.2.0/src/hyfi/dotenv/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/graphics/collage.py` & `hyfi-1.2.0/src/hyfi/graphics/collage.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/graphics/motion.py` & `hyfi-1.2.0/src/hyfi/graphics/motion.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/graphics/utils.py` & `hyfi-1.2.0/src/hyfi/graphics/utils.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/joblib/__init__.py` & `hyfi-1.2.0/src/hyfi/joblib/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/joblib/batch/apply.py` & `hyfi-1.2.0/src/hyfi/joblib/batch/apply.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/joblib/batch/apply_batch.py` & `hyfi-1.2.0/src/hyfi/joblib/batch/apply_batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/joblib/batch/batcher.py` & `hyfi-1.2.0/src/hyfi/joblib/batch/batcher.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/path/__init__.py` & `hyfi-1.2.0/src/hyfi/path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/path/base.py` & `hyfi-1.2.0/src/hyfi/path/base.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/path/batch.py` & `hyfi-1.2.0/src/hyfi/path/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/path/dirnames.py` & `hyfi-1.2.0/src/hyfi/path/dirnames.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/path/task.py` & `hyfi-1.2.0/src/hyfi/path/task.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/pipe/__init__.py` & `hyfi-1.2.0/src/hyfi/pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/pipe/test.py` & `hyfi-1.2.0/src/hyfi/pipe/test.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/pipeline/__init__.py` & `hyfi-1.2.0/src/hyfi/pipeline/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 A class to run a pipeline.
 """
 from functools import reduce
 from typing import Any, Dict, List, Optional, Union
 
 from pydantic import field_validator
 
-from hyfi.__global__.config import __global_config__
 from hyfi.composer import Composer
 from hyfi.pipeline.configs import BaseRunConfig, PipeConfig, Pipes, RunningConfig
 from hyfi.project import ProjectConfig
 from hyfi.task import TaskConfig
 from hyfi.utils.contexts import change_directory
 from hyfi.utils.logging import LOGGING
 from hyfi.workflow import WorkflowConfig
```

### Comparing `hyfi-1.1.0/src/hyfi/pipeline/configs.py` & `hyfi-1.2.0/src/hyfi/pipeline/configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
     Configuration for HyFi Pipelines
 """
 from typing import Any, Callable, Dict, List, Optional, Union
 
 from pydantic import BaseModel, ConfigDict, model_validator
 
 from hyfi.composer import Composer
-from hyfi.composer.extended import XC
 from hyfi.task import TaskConfig
 from hyfi.utils.envs import ENVs
 from hyfi.utils.logging import LOGGING
 
 logger = LOGGING.getLogger(__name__)
 
 
@@ -66,26 +65,26 @@
         if self.env:
             ENVs.check_and_set_osenv_vars(self.env)
 
     def get_pipe_func(self) -> Optional[Callable]:
         if self.pipe_target.startswith("lambda"):
             return eval(self.pipe_target)
         elif self.pipe_target:
-            return XC.partial(self.pipe_target)
+            return Composer.partial(self.pipe_target)
         else:
             return None
 
     def get_run_func(self) -> Optional[Callable]:
         if self.run.startswith("lambda"):
             return eval(self.run)
         elif self.run:
             kwargs = self.run_with or {}
             if self.pipe_obj_arg_name:
                 kwargs.pop(self.pipe_obj_arg_name)
-            return XC.partial(self.run, **kwargs)
+            return Composer.partial(self.run, **kwargs)
         else:
             return None
 
 
 class DataframePipeConfig(PipeConfig):
     columns_to_apply: Optional[Union[str, List[str]]] = []
     use_batcher: bool = True
```

### Comparing `hyfi-1.1.0/src/hyfi/project/__init__.py` & `hyfi-1.2.0/src/hyfi/project/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/task/__init__.py` & `hyfi-1.2.0/src/hyfi/task/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/task/batch.py` & `hyfi-1.2.0/src/hyfi/task/batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Configuration class for batch tasks. Inherits from TaskConfig.
 """
 from pathlib import Path
 from typing import Dict, List, Optional, Set, Union
 
 from hyfi.batch import BatchConfig
-from hyfi.composer.extended import XC
+from hyfi.composer import Composer
 from hyfi.task import TaskConfig
 from hyfi.utils.logging import LOGGING
 
 logger = LOGGING.getLogger(__name__)
 
 
 class BatchTaskConfig(TaskConfig):
@@ -184,28 +184,28 @@
                 batch_name,
                 batch_num,
             )
         cfg = self.export_config()
         if filepath:
             if filepath.is_file():
                 logger.info("Loading config from %s", filepath)
-                batch_cfg = XC.load(filepath)
+                batch_cfg = Composer.load(filepath)
                 logger.info("Merging config with the loaded config")
-                cfg = XC.merge(cfg, batch_cfg)
+                cfg = Composer.merge(cfg, batch_cfg)
             else:
                 logger.info("No config file found at %s", filepath)
         if self.verbose:
             logger.info("Updating config with config_kwargs: %s", config_kwargs)
-        cfg = XC.update(XC.to_dict(cfg), config_kwargs)
+        cfg = Composer.update(Composer.to_dict(cfg), config_kwargs)
 
         # initialize self with the config
         self.__init__(**cfg)
 
         return self.model_dump()
 
     def print_config(
         self,
         batch_name: Optional[str] = None,
         batch_num: Optional[int] = None,
     ):
         self.load_config(batch_name, batch_num)
-        XC.print(self.model_dump())
+        Composer.print(self.model_dump())
```

### Comparing `hyfi-1.1.0/src/hyfi/utils/contexts.py` & `hyfi-1.2.0/src/hyfi/utils/contexts.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/utils/datasets.py` & `hyfi-1.2.0/src/hyfi/utils/datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 logger = LOGGING.getLogger(__name__)
 
 DatasetType = Union[Dataset, IterableDataset]
 DatasetLikeType = Union[Dataset, IterableDataset, DatasetDict, IterableDatasetDict]
 
 
-class Datasets:
+class DATASETs:
     @staticmethod
     def is_dataframe(data: Any) -> bool:
         """Check if data is a pandas dataframe"""
         return isinstance(data, pd.DataFrame)
 
     @staticmethod
     def concatenate_data(
@@ -42,22 +42,22 @@
         axis: int = 0,
         split: Optional[str] = None,
         verbose: bool = False,
         **kwargs,
     ) -> Union[pd.DataFrame, DatasetType]:
         # if data is a list of datasets, concatenate them
         if isinstance(data, list) and isinstance(data[0], Dataset):
-            return Datasets.concatenate_datasets(
+            return DATASETs.concatenate_datasets(
                 data,
                 axis=axis,
                 split=split,
                 **kwargs,
             )
         else:
-            return Datasets.concatenate_dataframes(
+            return DATASETs.concatenate_dataframes(
                 data,
                 columns=columns,
                 add_split_key_column=add_split_key_column,
                 added_column_name=added_column_name,
                 ignore_index=ignore_index,
                 axis=axis,
                 verbose=verbose,
@@ -102,50 +102,51 @@
 
     @staticmethod
     def load_data(
         path: Optional[str] = "pandas",
         name: Optional[str] = None,
         data_dir: Optional[str] = "",
         data_files: Optional[Union[str, Sequence[str]]] = None,
-        split: Optional[str] = None,
+        split: Optional[str] = "train",
         filetype: Optional[str] = "",
         concatenate: Optional[bool] = False,
         use_cached: bool = False,
         verbose: Optional[bool] = False,
         **kwargs,
     ) -> Union[Dict[str, pd.DataFrame], Dict[str, DatasetType]]:
         """Load data from a file or a list of files"""
         if path in ["dataframe", "df", "pandas"]:
-            if data := Datasets.load_dataframes(
+            data = DATASETs.load_dataframes(
                 data_files,
                 data_dir=data_dir,
                 filetype=filetype,
                 split=split,
                 concatenate=concatenate,
                 use_cached=use_cached,
                 verbose=verbose,
                 **kwargs,
-            ):
+            )
+            if data is not None:
                 return data if isinstance(data, dict) else {split: data}
             else:
                 return {}
         else:
-            dset = Datasets.load_dataset(
+            dset = DATASETs.load_dataset(
                 path,
                 name=name,
                 data_dir=data_dir,
                 data_files=data_files,
                 split=split,
                 **kwargs,
             )
             split = split or "train"
             if isinstance(dset, (Dataset, IterableDataset)):
                 return {split: dset}
             if concatenate:
-                return {split: Datasets.concatenate_datasets(dset.values())}
+                return {split: DATASETs.concatenate_datasets(dset.values())}
             else:
                 return {k: v for k, v in dset.items() if v is not None}
 
     @staticmethod
     def get_data_files(
         data_files: Optional[
             Union[str, Sequence[str], Mapping[str, Union[str, Sequence[str]]]]
@@ -192,41 +193,41 @@
         **kwargs,
     ) -> Union[Dict[str, pd.DataFrame], pd.DataFrame]:
         """Load data from a file or a list of files"""
         if not data_files:
             logger.warning("No data_files provided")
             return {}
 
-        filepaths = Datasets.get_data_files(
+        filepaths = DATASETs.get_data_files(
             data_files,
             data_dir,
             split=split,
             use_cached=use_cached,
             verbose=verbose,
             **kwargs,
         )
 
         if isinstance(filepaths, dict):
             data = {
                 name: pd.concat(
                     [
-                        Datasets.load_dataframe(
+                        DATASETs.load_dataframe(
                             f, verbose=verbose, filetype=filetype, **kwargs
                         )
                         for f in files
                     ],
                     ignore_index=ignore_index,
                 )
                 for name, files in filepaths.items()
             }
             data = {k: v for k, v in data.items() if v is not None}
             return data
         else:
             data = {
-                os.path.basename(f): Datasets.load_dataframe(
+                os.path.basename(f): DATASETs.load_dataframe(
                     f, verbose=verbose, filetype=filetype, **kwargs
                 )
                 for f in filepaths
             }
             data = {k: v for k, v in data.items() if v is not None}
             if len(data) == 1:
                 data = list(data.values())[0]
@@ -321,26 +322,26 @@
         filepath = os.path.join(data_dir, data_file) if data_dir else data_file
         data_dir = os.path.dirname(filepath)
         data_file = os.path.basename(filepath)
         os.makedirs(data_dir, exist_ok=True)
 
         if isinstance(data, dict):
             for k, v in data.items():
-                Datasets.save_dataframes(
+                DATASETs.save_dataframes(
                     v,
                     data_file,
                     data_dir=data_dir,
                     columns=columns,
                     index=index,
                     filetype=filetype,
                     suffix=k,
                     verbose=verbose,
                     **kwargs,
                 )
-        elif Datasets.is_dataframe(data):
+        elif DATASETs.is_dataframe(data):
             logger.info("Saving dataframe to %s", filepath)
             if isinstance(columns, list):
                 columns = [c for c in columns if c in data.columns]
                 data = data[columns]
             with elapsed_timer(format_time=True) as elapsed:
                 if "csv" in filetype or "tsv" in filetype:
                     data.to_csv(filepath, index=index)
```

### Comparing `hyfi-1.1.0/src/hyfi/utils/envs.py` & `hyfi-1.2.0/src/hyfi/utils/envs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/utils/funcs.py` & `hyfi-1.2.0/src/hyfi/utils/funcs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/utils/gpumon.py` & `hyfi-1.2.0/src/hyfi/utils/gpumon.py`

 * *Files 22% similar despite different names*

```diff
@@ -68,17 +68,21 @@
         order="first",
         maxLoad=0.5,
         maxMemory=0.5,
         attempts=1,
         interval=900,
         verbose=False,
         includeNan=False,
-        excludeID=[],
-        excludeUUID=[],
+        excludeID=None,
+        excludeUUID=None,
     ):
+        if excludeID is None:
+            excludeID = []
+        if excludeUUID is None:
+            excludeUUID = []
         return GPUtil.getFirstAvailable(
             order=order,
             maxLoad=maxLoad,
             maxMemory=maxMemory,
             attempts=attempts,
             interval=interval,
             verbose=verbose,
@@ -136,7 +140,41 @@
         logger.info(f"Setting cuda device to {_names}")
         device = ", ".join(ids)
         os.environ["CUDA_DEVICE_ORDER"] = "PCI_BUS_ID"
         os.environ["CUDA_VISIBLE_DEVICES"] = device
     except ImportError as e:
         os.environ["CUDA_VISIBLE_DEVICES"] = ""
         raise CudaDeviceNotFoundError("Cuda device not found") from e
+
+
+class GPUs:
+    ###############################
+    # GPU Utility functions
+    ###############################
+    @staticmethod
+    def nvidia_smi():
+        return nvidia_smi()
+
+    @staticmethod
+    def set_cuda(device=0):
+        return set_cuda(device)
+
+    @staticmethod
+    def gpu_usage(all=False, attrList=None, useOldCode=False):
+        """
+        Show GPU utilization in human readable format. This is a wrapper around the GPUtil library.
+
+        Args:
+                all: If True show all available GPUs ( default : False )
+                attrList: List of attributes to show ( default : None )
+                useOldCode: If True use old code instead of new code ( default : False )
+
+        Returns:
+                A string with the
+        """
+        try:
+            from GPUtil import showUtilization  # type: ignore
+        except ImportError:
+            logger.error("GPUtil is not installed. To install, run: pip install GPUtil")
+            return
+
+        return showUtilization(all, attrList, useOldCode)
```

### Comparing `hyfi-1.1.0/src/hyfi/utils/iolibs.py` & `hyfi-1.2.0/src/hyfi/utils/iolibs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/utils/logging.py` & `hyfi-1.2.0/src/hyfi/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/utils/notebooks.py` & `hyfi-1.2.0/src/hyfi/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/utils/packages.py` & `hyfi-1.2.0/src/hyfi/utils/packages.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/src/hyfi/workflow/__init__.py` & `hyfi-1.2.0/src/hyfi/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.1.0/PKG-INFO` & `hyfi-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 1.1.0
+Version: 1.2.0
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 Home-page: https://hyfi.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

