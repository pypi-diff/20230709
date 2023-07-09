# Comparing `tmp/chrislab-0.5.5.tar.gz` & `tmp/chrislab-0.5.5.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chrislab-0.5.5.tar", last modified: Sun Jul  9 15:35:00 2023, max compression
+gzip compressed data, was "chrislab-0.5.5.post1.tar", last modified: Sun Jul  9 15:55:08 2023, max compression
```

## Comparing `chrislab-0.5.5.tar` & `chrislab-0.5.5.post1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:35:00.777645 chrislab-0.5.5/
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     1066 2023-07-08 17:51:04.000000 chrislab-0.5.5/LICENSE
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)      830 2023-07-09 15:35:00.777645 chrislab-0.5.5/PKG-INFO
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)      291 2023-07-08 17:51:04.000000 chrislab-0.5.5/README.md
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)       81 2023-07-08 17:51:04.000000 chrislab-0.5.5/pyproject.toml
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     1129 2023-07-09 15:35:00.777645 chrislab-0.5.5/setup.cfg
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:35:00.773645 chrislab-0.5.5/src/
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:35:00.773645 chrislab-0.5.5/src/chrislab/
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)        0 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/chrislab/__init__.py
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:35:00.773645 chrislab-0.5.5/src/chrislab/common/
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)        0 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/chrislab/common/__init__.py
--rwxr-xr-x   0 chrisjihee (1000016) users    (1000001)     7852 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/chrislab/common/downloader.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    12638 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/chrislab/common/tokenizer_korbert.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    11372 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/chrislab/common/util.py
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:35:00.773645 chrislab-0.5.5/src/chrislab/language/
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)        0 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/chrislab/language/__init__.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     1319 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/chrislab/language/cli.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    14142 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/chrislab/language/converter.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     9408 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/chrislab/language/evaluater.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    39568 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/chrislab/language/finetuner.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     6833 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/chrislab/language/modeling.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    14491 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/chrislab/language/predictor.py
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:35:00.773645 chrislab-0.5.5/src/chrislab.egg-info/
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)      830 2023-07-09 15:35:00.000000 chrislab-0.5.5/src/chrislab.egg-info/PKG-INFO
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     1541 2023-07-09 15:35:00.000000 chrislab-0.5.5/src/chrislab.egg-info/SOURCES.txt
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)        1 2023-07-09 15:35:00.000000 chrislab-0.5.5/src/chrislab.egg-info/dependency_links.txt
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)      132 2023-07-09 15:35:00.000000 chrislab-0.5.5/src/chrislab.egg-info/entry_points.txt
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)      211 2023-07-09 15:35:00.000000 chrislab-0.5.5/src/chrislab.egg-info/requires.txt
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)       17 2023-07-09 15:35:00.000000 chrislab-0.5.5/src/chrislab.egg-info/top_level.txt
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)        1 2023-07-09 15:35:00.000000 chrislab-0.5.5/src/chrislab.egg-info/zip-safe
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:35:00.773645 chrislab-0.5.5/src/nlpbook/
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)       95 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/__init__.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    12843 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/arguments.py
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:35:00.773645 chrislab-0.5.5/src/nlpbook/cls/
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)       59 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/cls/__init__.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     8835 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/cls/cli.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     5177 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/cls/corpus.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     2646 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/cls/task.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     2246 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/data_utils.py
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:35:00.777645 chrislab-0.5.5/src/nlpbook/dp/
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)      142 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/dp/__init__.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    12298 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/dp/cli.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    18570 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/dp/corpus.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    11240 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/dp/model.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     6968 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/dp/task.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     2057 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/factory.py
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:35:00.777645 chrislab-0.5.5/src/nlpbook/generation/
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)      170 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/generation/__init__.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     4280 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/generation/arguments.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     5354 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/generation/corpus.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)      882 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/generation/deploy.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     1293 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/generation/task.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     8968 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/metrics.py
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:35:00.777645 chrislab-0.5.5/src/nlpbook/ner/
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)       87 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/ner/__init__.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    18164 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/ner/cli.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    14181 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/ner/corpus.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    10013 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/ner/task.py
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:35:00.777645 chrislab-0.5.5/src/nlpbook/paircls/
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)       62 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/paircls/__init__.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     2654 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/paircls/corpus.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)      641 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/paircls/deploy.py
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:35:00.777645 chrislab-0.5.5/src/nlpbook/qa/
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)      146 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/qa/__init__.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     4984 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/qa/arguments.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    17080 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/qa/corpus.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)      639 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/qa/deploy.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     2072 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/qa/task.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     9761 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/utils.py
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:55:08.031606 chrislab-0.5.5.post1/
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     1066 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/LICENSE
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)      836 2023-07-09 15:55:08.031606 chrislab-0.5.5.post1/PKG-INFO
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)      291 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/README.md
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)       81 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/pyproject.toml
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     1207 2023-07-09 15:55:08.031606 chrislab-0.5.5.post1/setup.cfg
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:55:08.027606 chrislab-0.5.5.post1/src/
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:55:08.027606 chrislab-0.5.5.post1/src/chrislab/
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)        0 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/chrislab/__init__.py
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:55:08.027606 chrislab-0.5.5.post1/src/chrislab/common/
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)        0 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/chrislab/common/__init__.py
+-rwxr-xr-x   0 chrisjihee (1000016) users    (1000001)     7852 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/chrislab/common/downloader.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    12638 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/chrislab/common/tokenizer_korbert.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    11372 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/chrislab/common/util.py
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:55:08.027606 chrislab-0.5.5.post1/src/chrislab/language/
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)        0 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/chrislab/language/__init__.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     1319 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/chrislab/language/cli.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    14142 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/chrislab/language/converter.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     9408 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/chrislab/language/evaluater.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    39568 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/chrislab/language/finetuner.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     6833 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/chrislab/language/modeling.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    14491 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/chrislab/language/predictor.py
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:55:08.027606 chrislab-0.5.5.post1/src/chrislab.egg-info/
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)      836 2023-07-09 15:55:08.000000 chrislab-0.5.5.post1/src/chrislab.egg-info/PKG-INFO
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     1541 2023-07-09 15:55:08.000000 chrislab-0.5.5.post1/src/chrislab.egg-info/SOURCES.txt
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)       39 2023-07-09 15:55:08.000000 chrislab-0.5.5.post1/src/chrislab.egg-info/dependency_links.txt
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)      132 2023-07-09 15:55:08.000000 chrislab-0.5.5.post1/src/chrislab.egg-info/entry_points.txt
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)      223 2023-07-09 15:55:08.000000 chrislab-0.5.5.post1/src/chrislab.egg-info/requires.txt
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)       17 2023-07-09 15:55:08.000000 chrislab-0.5.5.post1/src/chrislab.egg-info/top_level.txt
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)        1 2023-07-09 15:55:07.000000 chrislab-0.5.5.post1/src/chrislab.egg-info/zip-safe
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:55:08.027606 chrislab-0.5.5.post1/src/nlpbook/
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)       95 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/nlpbook/__init__.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    12843 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/nlpbook/arguments.py
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:55:08.027606 chrislab-0.5.5.post1/src/nlpbook/cls/
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)       59 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/nlpbook/cls/__init__.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     8835 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/nlpbook/cls/cli.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     5177 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/nlpbook/cls/corpus.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     2646 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/nlpbook/cls/task.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     2246 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/nlpbook/data_utils.py
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:55:08.031606 chrislab-0.5.5.post1/src/nlpbook/dp/
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)      142 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/nlpbook/dp/__init__.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    12298 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/nlpbook/dp/cli.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    18570 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/nlpbook/dp/corpus.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    11240 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/nlpbook/dp/model.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     6968 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/nlpbook/dp/task.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     2057 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/nlpbook/factory.py
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:55:08.031606 chrislab-0.5.5.post1/src/nlpbook/generation/
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)      170 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/nlpbook/generation/__init__.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     4280 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/nlpbook/generation/arguments.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     5354 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/nlpbook/generation/corpus.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)      882 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/nlpbook/generation/deploy.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     1293 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/nlpbook/generation/task.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     8968 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/nlpbook/metrics.py
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:55:08.031606 chrislab-0.5.5.post1/src/nlpbook/ner/
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)       87 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/nlpbook/ner/__init__.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    18164 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/nlpbook/ner/cli.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    14181 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/nlpbook/ner/corpus.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    10013 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/nlpbook/ner/task.py
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:55:08.031606 chrislab-0.5.5.post1/src/nlpbook/paircls/
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)       62 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/nlpbook/paircls/__init__.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     2654 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/nlpbook/paircls/corpus.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)      641 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/nlpbook/paircls/deploy.py
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:55:08.031606 chrislab-0.5.5.post1/src/nlpbook/qa/
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)      146 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/nlpbook/qa/__init__.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     4984 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/nlpbook/qa/arguments.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    17080 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/nlpbook/qa/corpus.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)      639 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/nlpbook/qa/deploy.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     2072 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/nlpbook/qa/task.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     9761 2023-07-08 17:51:04.000000 chrislab-0.5.5.post1/src/nlpbook/utils.py
```

### Comparing `chrislab-0.5.5/LICENSE` & `chrislab-0.5.5.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5/PKG-INFO` & `chrislab-0.5.5.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chrislab
-Version: 0.5.5
+Version: 0.5.5.post1
 Summary: An advanced tool for doing experimental study.
 Home-page: https://github.com/chrisjihee/chrislab
 Author: Jihee Ryu
 Author-email: chrisjihee@naver.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chrislab-0.5.5/setup.cfg` & `chrislab-0.5.5.post1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = chrislab
-version = 0.5.5
+version = 0.5.5.post1
 author = Jihee Ryu
 author_email = chrisjihee@naver.com
 url = https://github.com/chrisjihee/chrislab
 description = An advanced tool for doing experimental study.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
@@ -19,16 +19,16 @@
 zip_safe = True
 packages = find:
 package_dir = 
 	=src
 include_package_data = True
 install_requires = 
 	chrisbase
-	torch>=1.7
-	lightning>=1.7
+	torch==2.0.1
+	pytorch-lightning==2.0.4
 	evaluate
 	datasets
 	tokenizers
 	transformers
 	Flask
 	Flask-Cors
 	Korpora
@@ -37,14 +37,16 @@
 	ipynbname
 	ipywidgets
 	jupyterlab
 	jupyter
 	tornado==6.1
 	tensorboard
 	tensorboardX>=2.2, <=2.5.1
+dependency_links = 
+	https://download.pytorch.org/whl/cu117
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 * = README.md
```

### Comparing `chrislab-0.5.5/src/chrislab/common/downloader.py` & `chrislab-0.5.5.post1/src/chrislab/common/downloader.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5/src/chrislab/common/tokenizer_korbert.py` & `chrislab-0.5.5.post1/src/chrislab/common/tokenizer_korbert.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5/src/chrislab/common/util.py` & `chrislab-0.5.5.post1/src/chrislab/common/util.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5/src/chrislab/language/cli.py` & `chrislab-0.5.5.post1/src/chrislab/language/cli.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5/src/chrislab/language/converter.py` & `chrislab-0.5.5.post1/src/chrislab/language/converter.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5/src/chrislab/language/evaluater.py` & `chrislab-0.5.5.post1/src/chrislab/language/evaluater.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5/src/chrislab/language/finetuner.py` & `chrislab-0.5.5.post1/src/chrislab/language/finetuner.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5/src/chrislab/language/modeling.py` & `chrislab-0.5.5.post1/src/chrislab/language/modeling.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5/src/chrislab/language/predictor.py` & `chrislab-0.5.5.post1/src/chrislab/language/predictor.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5/src/chrislab.egg-info/PKG-INFO` & `chrislab-0.5.5.post1/src/chrislab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chrislab
-Version: 0.5.5
+Version: 0.5.5.post1
 Summary: An advanced tool for doing experimental study.
 Home-page: https://github.com/chrisjihee/chrislab
 Author: Jihee Ryu
 Author-email: chrisjihee@naver.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chrislab-0.5.5/src/chrislab.egg-info/SOURCES.txt` & `chrislab-0.5.5.post1/src/chrislab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5/src/nlpbook/arguments.py` & `chrislab-0.5.5.post1/src/nlpbook/arguments.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5/src/nlpbook/cls/cli.py` & `chrislab-0.5.5.post1/src/nlpbook/cls/cli.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5/src/nlpbook/cls/corpus.py` & `chrislab-0.5.5.post1/src/nlpbook/cls/corpus.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5/src/nlpbook/cls/task.py` & `chrislab-0.5.5.post1/src/nlpbook/cls/task.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5/src/nlpbook/data_utils.py` & `chrislab-0.5.5.post1/src/nlpbook/data_utils.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5/src/nlpbook/dp/cli.py` & `chrislab-0.5.5.post1/src/nlpbook/dp/cli.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5/src/nlpbook/dp/corpus.py` & `chrislab-0.5.5.post1/src/nlpbook/dp/corpus.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5/src/nlpbook/dp/model.py` & `chrislab-0.5.5.post1/src/nlpbook/dp/model.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5/src/nlpbook/dp/task.py` & `chrislab-0.5.5.post1/src/nlpbook/dp/task.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5/src/nlpbook/factory.py` & `chrislab-0.5.5.post1/src/nlpbook/factory.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5/src/nlpbook/generation/arguments.py` & `chrislab-0.5.5.post1/src/nlpbook/generation/arguments.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5/src/nlpbook/generation/corpus.py` & `chrislab-0.5.5.post1/src/nlpbook/generation/corpus.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5/src/nlpbook/generation/deploy.py` & `chrislab-0.5.5.post1/src/nlpbook/generation/deploy.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5/src/nlpbook/generation/task.py` & `chrislab-0.5.5.post1/src/nlpbook/generation/task.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5/src/nlpbook/metrics.py` & `chrislab-0.5.5.post1/src/nlpbook/metrics.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5/src/nlpbook/ner/cli.py` & `chrislab-0.5.5.post1/src/nlpbook/ner/cli.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5/src/nlpbook/ner/corpus.py` & `chrislab-0.5.5.post1/src/nlpbook/ner/corpus.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5/src/nlpbook/ner/task.py` & `chrislab-0.5.5.post1/src/nlpbook/ner/task.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5/src/nlpbook/paircls/corpus.py` & `chrislab-0.5.5.post1/src/nlpbook/paircls/corpus.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5/src/nlpbook/paircls/deploy.py` & `chrislab-0.5.5.post1/src/nlpbook/paircls/deploy.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5/src/nlpbook/qa/arguments.py` & `chrislab-0.5.5.post1/src/nlpbook/qa/arguments.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5/src/nlpbook/qa/corpus.py` & `chrislab-0.5.5.post1/src/nlpbook/qa/corpus.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5/src/nlpbook/qa/deploy.py` & `chrislab-0.5.5.post1/src/nlpbook/qa/deploy.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5/src/nlpbook/qa/task.py` & `chrislab-0.5.5.post1/src/nlpbook/qa/task.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.5/src/nlpbook/utils.py` & `chrislab-0.5.5.post1/src/nlpbook/utils.py`

 * *Files identical despite different names*

