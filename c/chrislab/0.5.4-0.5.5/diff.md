# Comparing `tmp/chrislab-0.5.4.tar.gz` & `tmp/chrislab-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chrislab-0.5.4.tar", last modified: Thu Jun 29 14:12:47 2023, max compression
+gzip compressed data, was "chrislab-0.5.5.tar", last modified: Sun Jul  9 15:35:00 2023, max compression
```

## Comparing `chrislab-0.5.4.tar` & `chrislab-0.5.5.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-29 14:12:47.292331 chrislab-0.5.4/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1066 2023-06-29 13:39:49.000000 chrislab-0.5.4/LICENSE
--rw-rw-r--   0 chris     (1000) chris     (1000)      830 2023-06-29 14:12:47.292331 chrislab-0.5.4/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      291 2023-06-29 13:39:49.000000 chrislab-0.5.4/README.md
--rw-rw-r--   0 chris     (1000) chris     (1000)       81 2023-06-29 13:39:49.000000 chrislab-0.5.4/pyproject.toml
--rw-rw-r--   0 chris     (1000) chris     (1000)     1129 2023-06-29 14:12:47.296331 chrislab-0.5.4/setup.cfg
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-29 14:12:47.288331 chrislab-0.5.4/src/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-29 14:12:47.288331 chrislab-0.5.4/src/chrislab/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/chrislab/__init__.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-29 14:12:47.292331 chrislab-0.5.4/src/chrislab/common/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/chrislab/common/__init__.py
--rwxrwxr-x   0 chris     (1000) chris     (1000)     7852 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/chrislab/common/downloader.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    12638 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/chrislab/common/tokenizer_korbert.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    11372 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/chrislab/common/util.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-29 14:12:47.292331 chrislab-0.5.4/src/chrislab/language/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/chrislab/language/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1316 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/chrislab/language/cli.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    14142 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/chrislab/language/converter.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     9408 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/chrislab/language/evaluater.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    39567 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/chrislab/language/finetuner.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     6833 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/chrislab/language/modeling.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    14491 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/chrislab/language/predictor.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-29 14:12:47.288331 chrislab-0.5.4/src/chrislab.egg-info/
--rw-rw-r--   0 chris     (1000) chris     (1000)      830 2023-06-29 14:12:47.000000 chrislab-0.5.4/src/chrislab.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)     1518 2023-06-29 14:12:47.000000 chrislab-0.5.4/src/chrislab.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-06-29 14:12:47.000000 chrislab-0.5.4/src/chrislab.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)      132 2023-06-29 14:12:47.000000 chrislab-0.5.4/src/chrislab.egg-info/entry_points.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)      211 2023-06-29 14:12:47.000000 chrislab-0.5.4/src/chrislab.egg-info/requires.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       17 2023-06-29 14:12:47.000000 chrislab-0.5.4/src/chrislab.egg-info/top_level.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-06-29 14:12:47.000000 chrislab-0.5.4/src/chrislab.egg-info/zip-safe
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-29 14:12:47.292331 chrislab-0.5.4/src/nlpbook/
--rw-rw-r--   0 chris     (1000) chris     (1000)       95 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    10124 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/arguments.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-29 14:12:47.292331 chrislab-0.5.4/src/nlpbook/cls/
--rw-rw-r--   0 chris     (1000) chris     (1000)       59 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/cls/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     8870 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/cls/cli.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5209 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/cls/corpus.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2673 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/cls/task.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2246 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/data_utils.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-29 14:12:47.292331 chrislab-0.5.4/src/nlpbook/dp/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/dp/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    12333 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/dp/cli.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    19194 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/dp/corpus.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    11306 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/dp/model.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     3179 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/factory.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-29 14:12:47.292331 chrislab-0.5.4/src/nlpbook/generation/
--rw-rw-r--   0 chris     (1000) chris     (1000)      170 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/generation/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4280 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/generation/arguments.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5372 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/generation/corpus.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      882 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/generation/deploy.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1292 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/generation/task.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     9886 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/metrics.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-29 14:12:47.292331 chrislab-0.5.4/src/nlpbook/ner/
--rw-rw-r--   0 chris     (1000) chris     (1000)       48 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/ner/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    18392 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/ner/cli.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    13580 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/ner/corpus.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     9960 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/ner/task.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-29 14:12:47.292331 chrislab-0.5.4/src/nlpbook/paircls/
--rw-rw-r--   0 chris     (1000) chris     (1000)       62 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/paircls/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2657 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/paircls/corpus.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      641 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/paircls/deploy.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-29 14:12:47.292331 chrislab-0.5.4/src/nlpbook/qa/
--rw-rw-r--   0 chris     (1000) chris     (1000)      146 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/qa/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4984 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/qa/arguments.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    17105 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/qa/corpus.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      639 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/qa/deploy.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2071 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/qa/task.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    10847 2023-06-29 13:39:49.000000 chrislab-0.5.4/src/nlpbook/utils.py
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:35:00.777645 chrislab-0.5.5/
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     1066 2023-07-08 17:51:04.000000 chrislab-0.5.5/LICENSE
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)      830 2023-07-09 15:35:00.777645 chrislab-0.5.5/PKG-INFO
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)      291 2023-07-08 17:51:04.000000 chrislab-0.5.5/README.md
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)       81 2023-07-08 17:51:04.000000 chrislab-0.5.5/pyproject.toml
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     1129 2023-07-09 15:35:00.777645 chrislab-0.5.5/setup.cfg
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:35:00.773645 chrislab-0.5.5/src/
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:35:00.773645 chrislab-0.5.5/src/chrislab/
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)        0 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/chrislab/__init__.py
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:35:00.773645 chrislab-0.5.5/src/chrislab/common/
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)        0 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/chrislab/common/__init__.py
+-rwxr-xr-x   0 chrisjihee (1000016) users    (1000001)     7852 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/chrislab/common/downloader.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    12638 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/chrislab/common/tokenizer_korbert.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    11372 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/chrislab/common/util.py
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:35:00.773645 chrislab-0.5.5/src/chrislab/language/
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)        0 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/chrislab/language/__init__.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     1319 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/chrislab/language/cli.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    14142 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/chrislab/language/converter.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     9408 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/chrislab/language/evaluater.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    39568 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/chrislab/language/finetuner.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     6833 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/chrislab/language/modeling.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    14491 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/chrislab/language/predictor.py
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:35:00.773645 chrislab-0.5.5/src/chrislab.egg-info/
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)      830 2023-07-09 15:35:00.000000 chrislab-0.5.5/src/chrislab.egg-info/PKG-INFO
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     1541 2023-07-09 15:35:00.000000 chrislab-0.5.5/src/chrislab.egg-info/SOURCES.txt
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)        1 2023-07-09 15:35:00.000000 chrislab-0.5.5/src/chrislab.egg-info/dependency_links.txt
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)      132 2023-07-09 15:35:00.000000 chrislab-0.5.5/src/chrislab.egg-info/entry_points.txt
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)      211 2023-07-09 15:35:00.000000 chrislab-0.5.5/src/chrislab.egg-info/requires.txt
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)       17 2023-07-09 15:35:00.000000 chrislab-0.5.5/src/chrislab.egg-info/top_level.txt
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)        1 2023-07-09 15:35:00.000000 chrislab-0.5.5/src/chrislab.egg-info/zip-safe
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:35:00.773645 chrislab-0.5.5/src/nlpbook/
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)       95 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/__init__.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    12843 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/arguments.py
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:35:00.773645 chrislab-0.5.5/src/nlpbook/cls/
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)       59 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/cls/__init__.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     8835 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/cls/cli.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     5177 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/cls/corpus.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     2646 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/cls/task.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     2246 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/data_utils.py
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:35:00.777645 chrislab-0.5.5/src/nlpbook/dp/
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)      142 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/dp/__init__.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    12298 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/dp/cli.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    18570 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/dp/corpus.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    11240 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/dp/model.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     6968 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/dp/task.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     2057 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/factory.py
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:35:00.777645 chrislab-0.5.5/src/nlpbook/generation/
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)      170 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/generation/__init__.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     4280 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/generation/arguments.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     5354 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/generation/corpus.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)      882 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/generation/deploy.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     1293 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/generation/task.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     8968 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/metrics.py
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:35:00.777645 chrislab-0.5.5/src/nlpbook/ner/
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)       87 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/ner/__init__.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    18164 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/ner/cli.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    14181 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/ner/corpus.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    10013 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/ner/task.py
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:35:00.777645 chrislab-0.5.5/src/nlpbook/paircls/
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)       62 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/paircls/__init__.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     2654 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/paircls/corpus.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)      641 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/paircls/deploy.py
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:35:00.777645 chrislab-0.5.5/src/nlpbook/qa/
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)      146 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/qa/__init__.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     4984 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/qa/arguments.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    17080 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/qa/corpus.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)      639 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/qa/deploy.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     2072 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/qa/task.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     9761 2023-07-08 17:51:04.000000 chrislab-0.5.5/src/nlpbook/utils.py
```

### Comparing `chrislab-0.5.4/LICENSE` & `chrislab-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.4/PKG-INFO` & `chrislab-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chrislab
-Version: 0.5.4
+Version: 0.5.5
 Summary: An advanced tool for doing experimental study.
 Home-page: https://github.com/chrisjihee/chrislab
 Author: Jihee Ryu
 Author-email: chrisjihee@naver.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chrislab-0.5.4/setup.cfg` & `chrislab-0.5.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = chrislab
-version = 0.5.4
+version = 0.5.5
 author = Jihee Ryu
 author_email = chrisjihee@naver.com
 url = https://github.com/chrisjihee/chrislab
 description = An advanced tool for doing experimental study.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
```

### Comparing `chrislab-0.5.4/src/chrislab/common/downloader.py` & `chrislab-0.5.5/src/chrislab/common/downloader.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.4/src/chrislab/common/tokenizer_korbert.py` & `chrislab-0.5.5/src/chrislab/common/tokenizer_korbert.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.4/src/chrislab/common/util.py` & `chrislab-0.5.5/src/chrislab/common/util.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.4/src/chrislab/language/cli.py` & `chrislab-0.5.5/src/chrislab/language/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from .predictor import MyPredictor
 
 app = Typer()
 
 
 @app.command()
 def check(config: str, prefix: str = "", postfix: str = "", save_cache=True, reset_cache=False, show_state=False, draw_figure=False):
-    with JobTimer(verbose=True, mute_logger=["lightning.fabric.utilities.seed"]):
+    with JobTimer(verbose=True, mute_loggers=["lightning.fabric.utilities.seed"]):
         MyFinetuner(config=config, prefix=prefix, postfix=postfix, save_cache=save_cache, reset_cache=reset_cache).ready(show_state=show_state, draw_figure=draw_figure)
 
 
 @app.command()
 def train(config: str, prefix: str = "", postfix: str = "", save_cache=True, reset_cache=False, show_state=True):
     torch.set_float32_matmul_precision('high')
-    with JobTimer(verbose=True, mute_logger=["lightning.fabric.utilities.seed"]):
+    with JobTimer(verbose=True, mute_loggers=["lightning.fabric.utilities.seed"]):
         MyFinetuner(config=config, prefix=prefix, postfix=postfix, save_cache=save_cache, reset_cache=reset_cache).run(show_state=show_state)
 
 
 @app.command()
 def apply(config: str, prefix: str = "", postfix: str = "", save_cache=True, reset_cache=False, show_state=True):
-    with JobTimer(verbose=True, mute_logger=["lightning.fabric.utilities.seed"]):
+    with JobTimer(verbose=True, mute_loggers=["lightning.fabric.utilities.seed"]):
         MyPredictor(config=config, prefix=prefix, postfix=postfix, save_cache=save_cache, reset_cache=reset_cache).run(show_state=show_state)
```

### Comparing `chrislab-0.5.4/src/chrislab/language/converter.py` & `chrislab-0.5.5/src/chrislab/language/converter.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.4/src/chrislab/language/evaluater.py` & `chrislab-0.5.5/src/chrislab/language/evaluater.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.4/src/chrislab/language/finetuner.py` & `chrislab-0.5.5/src/chrislab/language/finetuner.py`

 * *Files 0% similar despite different names*

```diff
@@ -354,15 +354,15 @@
         score.update(self.score_metric.compute(references=ys, predictions=ps))
         return score
 
     def get_learning_rate(self):
         return self.optimizer.param_groups[0]['lr']
 
     def load_tokenizer(self, verbose=True) -> None:
-        with JobTimer(verbose=verbose, mute_logger="transformers.tokenization_utils_base"):
+        with JobTimer(verbose=verbose, mute_loggers="transformers.tokenization_utils_base"):
             if self.state.pretrained.type == 'morp':
                 self.tokenizer = KorbertTokenizer.from_pretrained(self.state.pretrained.path, max_len=self.state.max_sequence_length, use_fast=False, do_lower_case=False, tokenize_chinese_chars=False)
             elif self.state.pretrained.type == 'bbpe':
                 self.tokenizer = AutoTokenizer.from_pretrained(self.state.pretrained.path, max_len=self.state.max_sequence_length, use_fast=False, do_lower_case=False)
                 self.tok_coder = ByteLevelBPETokenizer(str(self.state.pretrained.path / "vocab.json"), str(self.state.pretrained.path / "merges.txt"))
             else:
                 self.tokenizer = AutoTokenizer.from_pretrained(self.state.pretrained.path, max_len=self.state.max_sequence_length)
```

### Comparing `chrislab-0.5.4/src/chrislab/language/modeling.py` & `chrislab-0.5.5/src/chrislab/language/modeling.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.4/src/chrislab/language/predictor.py` & `chrislab-0.5.5/src/chrislab/language/predictor.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.4/src/chrislab.egg-info/PKG-INFO` & `chrislab-0.5.5/src/chrislab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chrislab
-Version: 0.5.4
+Version: 0.5.5
 Summary: An advanced tool for doing experimental study.
 Home-page: https://github.com/chrisjihee/chrislab
 Author: Jihee Ryu
 Author-email: chrisjihee@naver.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chrislab-0.5.4/src/chrislab.egg-info/SOURCES.txt` & `chrislab-0.5.5/src/chrislab.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 src/nlpbook/cls/cli.py
 src/nlpbook/cls/corpus.py
 src/nlpbook/cls/task.py
 src/nlpbook/dp/__init__.py
 src/nlpbook/dp/cli.py
 src/nlpbook/dp/corpus.py
 src/nlpbook/dp/model.py
+src/nlpbook/dp/task.py
 src/nlpbook/generation/__init__.py
 src/nlpbook/generation/arguments.py
 src/nlpbook/generation/corpus.py
 src/nlpbook/generation/deploy.py
 src/nlpbook/generation/task.py
 src/nlpbook/ner/__init__.py
 src/nlpbook/ner/cli.py
```

### Comparing `chrislab-0.5.4/src/nlpbook/arguments.py` & `chrislab-0.5.5/src/nlpbook/arguments.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-import nlpbook
 import logging
 import math
 import os
+import sys
 from dataclasses import dataclass, field
 from datetime import datetime
 from pathlib import Path
-from typing import List, Tuple
+from typing import List
 
 import pandas as pd
+import pytorch_lightning
+import transformers
 from dataclasses_json import DataClassJsonMixin
-from lightning.fabric.accelerators import Accelerator
-from lightning.fabric.strategies import Strategy
-from lightning.pytorch.loggers import CSVLogger
+from pytorch_lightning.accelerators import Accelerator
+from pytorch_lightning.loggers import CSVLogger
+from pytorch_lightning.strategies import Strategy
 
-from chrisbase.io import ProjectEnv, make_dir
-from chrisbase.io import files, make_parent_dir, out_hr, out_table
+from chrisbase.io import files, make_parent_dir, hr, str_table, out_hr, out_table, get_hostname, get_hostaddr, running_file, first_or, cwd, configure_dual_logger, configure_unit_logger
 from chrisbase.time import now, str_delta
 from chrisbase.util import to_dataframe
 
+logger = logging.getLogger(__name__)
+
 
 @dataclass
 class TypedData(DataClassJsonMixin):
     data_type = None
 
     def __post_init__(self):
         self.data_type = self.__class__.__name__
@@ -57,30 +60,30 @@
 @dataclass
 class DataOption(OptionData):
     name: str | Path = field()
     home: str | Path | None = field(default=None)
     files: DataFiles | None = field(default=None)
     caching: bool = field(default=False)
     redownload: bool = field(default=False)
-    show_examples: int = field(default=3)
+    num_check: int = field(default=3)
 
     def __post_init__(self):
         if self.home:
             self.home = Path(self.home)
 
 
 @dataclass
 class ModelOption(OptionData):
     pretrained: str | Path = field()
-    finetuning_home: str | Path = field()
-    finetuning_name: str | Path | None = field(default=None)  # filename or filename format of downstream model
-    max_seq_length: int = field(default=128)  # maximum total input sequence length after tokenization
+    home: str | Path = field()
+    name: str | Path | None = field(default=None)  # filename or filename format of downstream model
+    seq_len: int = field(default=128)  # maximum total input sequence length after tokenization
 
     def __post_init__(self):
-        self.finetuning_home = Path(self.finetuning_home)
+        self.home = Path(self.home)
 
 
 @dataclass
 class HardwareOption(OptionData):
     # cpu_workers: int = field(default=0)
     cpu_workers: int = field(default=os.cpu_count())
     accelerator: str | Accelerator = field(default="auto")  # possbile value: "cpu", "gpu", "tpu", "ipu", "hpu", "mps", "auto"
@@ -95,29 +98,28 @@
                 self.strategy = "single_device"
             elif isinstance(self.devices, int) and self.devices > 1 or isinstance(self.devices, list) and len(self.devices) > 1:
                 self.strategy = "ddp"
 
 
 @dataclass
 class LearningOption(OptionData):
-    validating_fmt: str | None = field(default=None)
-    validating_on: int | float = field(default=1.0)
-    num_keeping: int = field(default=5)
-    keeping_by: str = field(default="min val_loss")
+    validate_fmt: str | None = field(default=None)
+    validate_on: int | float = field(default=1.0)
+    save_by: str = field(default="min val_loss")
+    num_save: int = field(default=5)
     epochs: int = field(default=1)
-    speed: float = field(default=5e-5)
+    lr: float = field(default=5e-5)
     seed: int | None = field(default=None)  # random seed
 
     def __post_init__(self):
-        self.validating_on = math.fabs(self.validating_on)
+        self.validate_on = math.fabs(self.validate_on)
 
 
 @dataclass
-class JobTimer(ResultData):
-    name: str = field()
+class TimeChecker(ResultData):
     t1 = datetime.now()
     t2 = datetime.now()
     started: str | None = field(default=None)
     settled: str | None = field(default=None)
     elapsed: str | None = field(default=None)
 
     def set_started(self):
@@ -131,146 +133,206 @@
         self.t2 = datetime.now()
         self.settled = now()
         self.elapsed = str_delta(self.t2 - self.t1)
         return self
 
 
 @dataclass
-class JobOutput(ResultData):
-    dir_path: Path | None = field(init=False, default=None)
-    csv_out: CSVLogger | None = field(init=False, default=None)
+class ProgressChecker(ResultData):
     result: dict = field(init=False, default_factory=dict)
     global_step: int = field(init=False, default=0)
     global_epoch: float = field(init=False, default=0.0)
     epoch_per_step: float = field(init=False, default=0.0)
 
 
 @dataclass
+class ProjectEnv(TypedData):
+    project: str = field()
+    job_name: str = field(default=None)
+    hostname: str = field(init=False)
+    hostaddr: str = field(init=False)
+    python_path: Path = field(init=False)
+    working_path: Path = field(init=False)
+    running_file: Path = field(init=False)
+    command_args: List[str] = field(init=False)
+    output_home: str | Path | None = field(default=None)
+    logging_file: str | Path = field(default="message.out")
+    argument_file: str | Path = field(default="arguments.json")
+    debugging: bool = field(default=False)
+    msg_level: int = field(default=logging.INFO)
+    msg_format: str = field(default=logging.BASIC_FORMAT)
+    date_format: str = field(default="[%m.%d %H:%M:%S]")
+    csv_logger: CSVLogger | None = field(init=False, default=None)
+
+    def set(self, name: str = None):
+        self.job_name = name
+        return self
+
+    def __post_init__(self):
+        assert self.project, "Project name must be provided"
+        self.hostname = get_hostname()
+        self.hostaddr = get_hostaddr()
+        self.python_path = Path(sys.executable)
+        self.running_file = running_file()
+        self.project_path = first_or([x for x in self.running_file.parents if x.name.startswith(self.project)])
+        assert self.project_path, f"Could not find project path for {self.project} in {', '.join([str(x) for x in self.running_file.parents])}"
+        self.working_path = cwd(self.project_path)
+        self.running_file = self.running_file.relative_to(self.working_path)
+        self.command_args = sys.argv[1:]
+        self.logging_file = Path(self.logging_file)
+        self.argument_file = Path(self.argument_file)
+        if self.output_home:
+            self.output_home = Path(self.output_home)
+            configure_dual_logger(level=self.msg_level, fmt=self.msg_format, datefmt=self.date_format,
+                                  filename=self.output_home / self.logging_file)
+        else:
+            configure_unit_logger(level=self.msg_level, fmt=self.msg_format, datefmt=self.date_format,
+                                  stream=sys.stdout)
+
+
+@dataclass
 class CommonArguments(ArgumentGroupData):
     tag = "common"
-    job: JobTimer = field()
     env: ProjectEnv = field()
+    time: TimeChecker = field(default=TimeChecker())
+    prog: ProgressChecker = field(default=ProgressChecker())
     data: DataOption | None = field(default=None)
     model: ModelOption | None = field(default=None)
-    output: JobOutput = field(default=JobOutput())
 
     def __post_init__(self):
         super().__post_init__()
         if not self.env.logging_file.stem.endswith(self.tag):
             self.env.logging_file = self.env.logging_file.with_stem(f"{self.env.logging_file.stem}-{self.tag}")
         if not self.env.argument_file.stem.endswith(self.tag):
             self.env.argument_file = self.env.argument_file.with_stem(f"{self.env.argument_file.stem}-{self.tag}")
+
+        self.env.output_home = self.env.output_home or Path("output")
         if self.data and self.model:
-            self.output.dir_path = self.model.finetuning_home / self.data.name
-        if self.model and self.tag in ("train",):
-            self.model.finetuning_home = make_dir(self.model.finetuning_home)
+            self.env.output_home = self.model.home / self.data.name
+        elif self.data:
+            self.env.output_home = self.env.output_home / self.data.home
+        configure_dual_logger(level=self.env.msg_level, fmt=self.env.msg_format, datefmt=self.env.date_format,
+                              filename=self.env.output_home / self.env.logging_file)
+
+    def reconfigure_output(self, version=None):
+        if not version:
+            version = now('%m%d.%H%M%S')
+        self.env.csv_logger = CSVLogger(self.model.home, name=self.data.name,
+                                        version=f'{self.tag}-{self.env.job_name}-{version}',
+                                        flush_logs_every_n_steps=1)
+        existing_file = self.env.output_home / self.env.logging_file
+        existing_content = existing_file.read_text() if existing_file.exists() else None
+        self.env.output_home = Path(self.env.csv_logger.log_dir)
+        configure_dual_logger(level=self.env.msg_level, fmt=self.env.msg_format, datefmt=self.env.date_format,
+                              filename=self.env.output_home / self.env.logging_file, existing_content=existing_content)
+        existing_file.unlink(missing_ok=True)
+        return self
+
+    def save_arguments(self, to: Path | str = None) -> Path | None:
+        if not self.env.output_home:
+            return None
+        args_file = to if to else self.env.output_home / self.env.argument_file
+        args_json = self.to_json(default=str, ensure_ascii=False, indent=2)
+        make_parent_dir(args_file).write_text(args_json, encoding="utf-8")
+        return args_file
+
+    def info_arguments(self):
+        table = str_table(self.dataframe(), tablefmt="presto")  # "plain", "presto"
+        for line in table.splitlines() + [hr(c='-')]:
+            logger.info(line)
+        return self
 
-    def dataframe(self, columns=None):
+    def dataframe(self, columns=None) -> pd.DataFrame:
         if not columns:
             columns = [self.data_type, "value"]
         return pd.concat([
-            to_dataframe(columns=columns, raw=self.job, data_prefix="job"),
             to_dataframe(columns=columns, raw=self.env, data_prefix="env"),
+            to_dataframe(columns=columns, raw=self.time, data_prefix="time"),
+            to_dataframe(columns=columns, raw=self.prog, data_prefix="prog"),
             to_dataframe(columns=columns, raw=self.data, data_prefix="data"),
             to_dataframe(columns=columns, raw=self.model, data_prefix="model"),
-            to_dataframe(columns=columns, raw=self.output, data_prefix="output"),
         ]).reset_index(drop=True)
 
-    def show(self):
+    def show(self):  # TODO: Remove someday
         out_hr(c='-')
         out_table(self.dataframe())
         out_hr(c='-')
         return self
 
-    def setup_csv_out(self, version=None):
-        if not version:
-            version = now('%m%d.%H%M%S')
-        self.output.csv_out = CSVLogger(self.model.finetuning_home, name=self.data.name,
-                                        version=f'{self.tag}-{self.job.name}-{version}',
-                                        flush_logs_every_n_steps=1)
-        self.output.dir_path = Path(self.output.csv_out.log_dir)
-        return self
-
-    def save(self, to: Path | str = None) -> Path | None:
-        if not self.output.dir_path:
-            return None
-        args_file = to if to else self.output.dir_path / self.env.argument_file
-        args_json = self.to_json(default=str, ensure_ascii=False, indent=2)
-        make_parent_dir(args_file).write_text(args_json, encoding="utf-8")
-        return args_file
-
 
 @dataclass
 class ServerArguments(CommonArguments):
     tag = "serve"
 
     def __post_init__(self):
         super().__post_init__()
         if self.tag in ("serve", "test"):
-            assert self.model.finetuning_home.exists() and self.model.finetuning_home.is_dir(), \
-                f"No finetuning home: {self.model.finetuning_home}"
-            if not self.model.finetuning_name:
-                ckpt_files: List[Path] = files(self.output.dir_path / "**/*.ckpt")
-                assert ckpt_files, f"No checkpoint file in {self.model.finetuning_home}"
+            assert self.model.home.exists() and self.model.home.is_dir(), \
+                f"No finetuning home: {self.model.home}"
+            if not self.model.name:
+                ckpt_files: List[Path] = files(self.env.output_home / "**/*.ckpt")
+                assert ckpt_files, f"No checkpoint file in {self.model.home}"
                 ckpt_files = sorted([x for x in ckpt_files if "temp" not in str(x) and "tmp" not in str(x)], key=str)
-                self.model.finetuning_name = ckpt_files[-1].relative_to(self.output.dir_path)
-            assert (self.output.dir_path / self.model.finetuning_name).exists() and (self.output.dir_path / self.model.finetuning_name).is_file(), \
-                f"No checkpoint file: {self.output.dir_path / self.model.finetuning_name}"
+                self.model.name = ckpt_files[-1].relative_to(self.env.output_home)
+            assert (self.env.output_home / self.model.name).exists() and (self.env.output_home / self.model.name).is_file(), \
+                f"No checkpoint file: {self.env.output_home / self.model.name}"
 
 
 @dataclass
 class TesterArguments(ServerArguments):
     tag = "test"
     hardware: HardwareOption = field(default=HardwareOption(), metadata={"help": "device information"})
 
-    def dataframe(self, columns=None):
+    def dataframe(self, columns=None) -> pd.DataFrame:
         if not columns:
             columns = [self.data_type, "value"]
         return pd.concat([
             super().dataframe(columns=columns),
             to_dataframe(columns=columns, raw=self.hardware, data_prefix="hardware"),
         ]).reset_index(drop=True)
 
 
 @dataclass
 class TrainerArguments(TesterArguments):
     tag = "train"
     learning: LearningOption = field(default=LearningOption())
 
-    def dataframe(self, columns=None):
+    def dataframe(self, columns=None) -> pd.DataFrame:
         if not columns:
             columns = [self.data_type, "value"]
         return pd.concat([
             super().dataframe(columns=columns),
-            to_dataframe(columns=columns, raw=self.learning, data_prefix="training"),
+            to_dataframe(columns=columns, raw=self.learning, data_prefix="learning"),
         ]).reset_index(drop=True)
 
+    def set_seed(self) -> None:
+        if self.learning.seed is not None:
+            transformers.set_seed(self.learning.seed)
+            pytorch_lightning.seed_everything(self.learning.seed)
+        else:
+            logger.warning("not fixed seed")
+
 
 class ArgumentsUsing:
-    def __init__(self, args: CommonArguments, logging_level: int = logging.INFO, delete_on_exit: bool = True):
+    def __init__(self, args: CommonArguments, delete_on_exit: bool = True):
         self.args: CommonArguments = args
-        self.logging_level = logging_level
         self.delete_on_exit: bool = delete_on_exit
 
-    def __enter__(self) -> Tuple[Path, logging.Logger]:
-        self.args_file: Path | None = self.args.save()
-        self.logger: logging.Logger = nlpbook.new_logger_file(name=f"main.{self.args.env.running_file.stem}",
-                                                              filepath=self.args.output.dir_path / self.args.env.logging_file,
-                                                              filemode="w",
-                                                              level=self.logging_level, )
-        return self.args_file, self.logger
+    def __enter__(self) -> Path:
+        self.args_file: Path | None = self.args.save_arguments()
+        return self.args_file
 
     def __exit__(self, *exc_info):
         if self.delete_on_exit and self.args_file:
             self.args_file.unlink(missing_ok=True)
 
 
 class RuntimeChecking:
     def __init__(self, args: CommonArguments):
         self.args: CommonArguments = args
 
     def __enter__(self):
-        self.args.job.set_started()
+        self.args.time.set_started()
 
     def __exit__(self, *exc_info):
-        self.args.job.set_settled()
-        self.args.save(self.args.output.dir_path / self.args.env.argument_file)
+        self.args.time.set_settled()
+        self.args.save_arguments(self.args.env.output_home / self.args.env.argument_file)
```

### Comparing `chrislab-0.5.4/src/nlpbook/cls/cli.py` & `chrislab-0.5.5/src/nlpbook/cls/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import logging
 from pathlib import Path
 
-import lightning.pytorch as pl
-import nlpbook
 import torch
 from Korpora import Korpora
-from chrisbase.io import JobTimer, err_hr
 from flask import Flask
-from nlpbook.arguments import TrainerArguments, ServerArguments, TesterArguments, RuntimeChecking
-from nlpbook.cls.corpus import NsmcCorpus, ClassificationDataset
-from nlpbook.cls.task import ClassificationTask
+from pytorch_lightning import Trainer
 from torch.utils.data import DataLoader, RandomSampler
 from torch.utils.data import SequentialSampler
 from transformers import BertConfig, BertForSequenceClassification, BertTokenizer
 from transformers.modeling_outputs import SequenceClassifierOutput
 from typer import Typer
 
+import nlpbook
+from chrisbase.io import JobTimer, err_hr
+from nlpbook.arguments import TrainerArguments, ServerArguments, TesterArguments, RuntimeChecking
+from nlpbook.cls.corpus import NsmcCorpus, ClassificationDataset
+from nlpbook.cls.task import ClassificationTask
+
 app = Typer()
-logger = logging.getLogger("chrislab")
+logger = logging.getLogger(__name__)
 
 
 @app.command()
 def train(args_file: Path | str):
     nlpbook.set_logger()
     args_file = Path(args_file)
     assert args_file.exists(), f"No args_file: {args_file}"
@@ -64,31 +65,31 @@
         )
         model = BertForSequenceClassification.from_pretrained(
             args.model.pretrained,
             config=pretrained_model_config,
         )
         err_hr(c='-')
 
-        with RuntimeChecking(nlpbook.setup_csv_out(args)):
+        with RuntimeChecking(args.reconfigure_output()):
             torch.set_float32_matmul_precision('high')
-            trainer: pl.Trainer = nlpbook.make_trainer(args)
+            trainer: Trainer = nlpbook.make_trainer(args)
             trainer.fit(ClassificationTask(model, args, trainer),
                         train_dataloaders=train_dataloader,
                         val_dataloaders=val_dataloader)
 
 
 @app.command()
 def test(args_file: Path | str):
     nlpbook.set_logger()
     args_file = Path(args_file)
     assert args_file.exists(), f"No args_file: {args_file}"
     args: TesterArguments = TesterArguments.from_json(args_file.read_text()).show()
 
     with JobTimer(f"chrialab.nlpbook.cls test {args_file}", mt=1, mb=1, rt=1, rb=1, rc='=', verbose=True, flush_sec=0.3):
-        checkpoint_path = args.output.dir_path / args.model.finetuning_name
+        checkpoint_path = args.env.output_home / args.model.name
         assert checkpoint_path.exists(), f"No checkpoint file: {checkpoint_path}"
         logger.info(f"Using finetuned checkpoint file at {checkpoint_path}")
         err_hr(c='-')
 
         if not (args.data.home / args.data.name).exists() or not (args.data.home / args.data.name).is_dir():
             Korpora.fetch(
                 corpus_name=args.data.name,
@@ -115,31 +116,31 @@
         )
         model = BertForSequenceClassification.from_pretrained(
             args.model.pretrained,
             config=pretrained_model_config,
         )
         err_hr(c='-')
 
-        with RuntimeChecking(nlpbook.setup_csv_out(args)):
+        with RuntimeChecking(args.reconfigure_output()):
             torch.set_float32_matmul_precision('high')
-            tester: pl.Trainer = nlpbook.make_tester(args)
+            tester: Trainer = nlpbook.make_tester(args)
             tester.test(ClassificationTask(model, args, tester),
                         dataloaders=test_dataloader,
                         ckpt_path=checkpoint_path)
 
 
 @app.command()
 def serve(args_file: Path | str):
     nlpbook.set_logger()
     args_file = Path(args_file)
     assert args_file.exists(), f"No args_file file: {args_file}"
     args: ServerArguments = ServerArguments.from_json(args_file.read_text()).show()
 
     with JobTimer(f"chrialab.nlpbook serve_cls {args_file}", mt=1, mb=1, rt=1, rb=1, rc='=', verbose=True, flush_sec=0.3):
-        checkpoint_path = args.output.dir_path / args.model.finetuning_name
+        checkpoint_path = args.env.output_home / args.model.name
         assert checkpoint_path.exists(), f"No downstream model file: {checkpoint_path}"
         checkpoint: dict = torch.load(checkpoint_path, map_location=torch.device("cpu"))
         logger.info(f"Using finetuned model file at {checkpoint_path}")
         err_hr(c='-')
 
         # tokenizer: PreTrainedTokenizerFast = AutoTokenizer.from_pretrained(args.model.pretrained, do_lower_case=False, use_fast=True)
         # assert isinstance(tokenizer, PreTrainedTokenizerFast), f"tokenizer is not PreTrainedTokenizerFast: {type(tokenizer)}"
@@ -153,15 +154,15 @@
         model.load_state_dict({k.replace("model.", ""): v for k, v in checkpoint['state_dict'].items()})
         model.eval()
         err_hr(c='-')
 
         def inference_fn(sentence):
             inputs = tokenizer(
                 [sentence],
-                max_length=args.model.max_seq_length,
+                max_length=args.model.seq_len,
                 padding="max_length",
                 truncation=True,
             )
             with torch.no_grad():
                 outputs: SequenceClassifierOutput = model(**{k: torch.tensor(v) for k, v in inputs.items()})
                 prob = outputs.logits.softmax(dim=1)
                 positive_prob = round(prob[0][1].item(), 4)
@@ -172,12 +173,12 @@
                 'prediction': pred,
                 'positive_data': f"긍정 {positive_prob:.4f}",
                 'negative_data': f"부정 {negative_prob:.4f}",
                 'positive_width': f"{positive_prob * 100}%",
                 'negative_width': f"{negative_prob * 100}%",
             }
 
-        with RuntimeChecking(nlpbook.setup_csv_out(args)):
+        with RuntimeChecking(args.reconfigure_output()):
             server: Flask = nlpbook.make_server(inference_fn,
                                                 template_file="serve_cls.html",
                                                 ngrok_home=args.env.working_path)
             server.run()
```

### Comparing `chrislab-0.5.4/src/nlpbook/cls/corpus.py` & `chrislab-0.5.5/src/nlpbook/cls/corpus.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import torch
 from filelock import FileLock
 from torch.utils.data.dataset import Dataset
 
 from nlpbook.arguments import TrainerArguments, TesterArguments
 from transformers import PreTrainedTokenizer
 
-logger = logging.getLogger("chrislab")
+logger = logging.getLogger(__name__)
 
 
 @dataclass
 class ClassificationExample:
     text_a: str
     text_b: Optional[str] = None
     label: Optional[str] = None
@@ -64,15 +64,15 @@
     label_map = {label: i for i, label in enumerate(label_list)}
     labels = [label_map[example.label] for example in examples]
 
     logger.info("tokenize sentences, it could take a lot of time...")
     start = time.time()
     batch_encoding = tokenizer(
         [(example.text_a, example.text_b) for example in examples],
-        max_length=args.model.max_seq_length,
+        max_length=args.model.seq_len,
         padding="max_length",
         truncation=True,
     )
     logger.info("tokenize sentences [took %.3f s]", time.time() - start)
 
     features = []
     for i in range(len(examples)):
@@ -110,26 +110,26 @@
         assert args.data.home, f"No data_home: {args.data.home}"
         assert args.data.name, f"No data_name: {args.data.name}"
         data_file_dict: dict = args.data.files.to_dict()
         assert split in data_file_dict, f"No '{split}' split in data_file: should be one of {list(data_file_dict.keys())}"
         assert data_file_dict[split], f"No data_file for '{split}' split: {args.data.files}"
         text_data_path: Path = Path(args.data.home) / args.data.name / data_file_dict[split]
         cache_data_path = text_data_path \
-            .with_stem(text_data_path.stem + f"-by-{tokenizer.__class__.__name__}-with-{args.model.max_seq_length}") \
+            .with_stem(text_data_path.stem + f"-by-{tokenizer.__class__.__name__}-with-{args.model.seq_len}") \
             .with_suffix(".cache")
         cache_lock_path = cache_data_path.with_suffix(".lock")
 
         with FileLock(cache_lock_path):
             if os.path.exists(cache_data_path) and args.data.caching:
                 start = time.time()
                 self.features = torch.load(cache_data_path)
                 logger.info(f"Loading features from cached file at {cache_data_path} [took {time.time() - start:.3f} s]")
             else:
                 assert text_data_path.exists() and text_data_path.is_file(), f"No data_text_path: {text_data_path}"
-                logger.info(f"Creating features from dataset file at {text_data_path}")
+                logger.info(f"Creating features from {text_data_path}")
                 examples = self.corpus.get_examples(text_data_path)
                 self.features = convert_examples_to_features_fn(examples, tokenizer, args, label_list=self.corpus.get_labels())
                 start = time.time()
                 logger.info("Saving features into cached file, it could take a lot of time...")
                 torch.save(self.features, cache_data_path)
                 logger.info(f"Saving features into cached file at {cache_data_path} [took {time.time() - start:.3f} s]")
```

### Comparing `chrislab-0.5.4/src/nlpbook/cls/task.py` & `chrislab-0.5.5/src/nlpbook/cls/task.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-import lightning.pytorch as pl
-from lightning.pytorch import LightningModule
-from nlpbook.arguments import TrainerArguments, TesterArguments
-from nlpbook.metrics import accuracy
+from pytorch_lightning import LightningModule, Trainer
 from torch.optim import AdamW
 from torch.optim.lr_scheduler import ExponentialLR
 from transformers import PreTrainedModel
 from transformers.modeling_outputs import SequenceClassifierOutput
 
+from nlpbook.arguments import TrainerArguments, TesterArguments
+from nlpbook.metrics import accuracy
+
 
 class ClassificationTask(LightningModule):
     def __init__(self, model: PreTrainedModel,
                  args: TrainerArguments | TesterArguments,
-                 trainer: pl.Trainer):
+                 trainer: Trainer):
         super().__init__()
         self.model = model
         self.args = args
         self.trainer = trainer
         self.train_acc = -1.0
         self.train_loss = -1.0
 
     def configure_optimizers(self):
-        optimizer = AdamW(self.parameters(), lr=self.args.learning.speed)
+        optimizer = AdamW(self.parameters(), lr=self.args.learning.lr)
         scheduler = ExponentialLR(optimizer, gamma=0.9)
         return {
             'optimizer': optimizer,
             'lr_scheduler': scheduler,
         }
 
     def training_step(self, inputs, batch_idx):
```

### Comparing `chrislab-0.5.4/src/nlpbook/data_utils.py` & `chrislab-0.5.5/src/nlpbook/data_utils.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.4/src/nlpbook/dp/cli.py` & `chrislab-0.5.5/src/nlpbook/dp/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,59 +8,58 @@
 import torch.nn.functional as F
 from torch.utils.data import DataLoader, RandomSampler, SequentialSampler
 from typer import Typer
 
 import lightning as L
 from chrisbase.io import JobTimer, pop_keys, err_hr
 from chrislab.common.util import time_tqdm_cls, mute_tqdm_cls
-from nlpbook import new_set_logger, save_checkpoint
+from nlpbook import save_checkpoint
 from nlpbook.arguments import TrainerArguments, RuntimeChecking
 from nlpbook.dp.corpus import DPCorpus, DPDataset
-from nlpbook.dp.model import DPTransformer
+from nlpbook.dp.model import ModelForDependencyParsing
 from nlpbook.metrics import DPResult
 from transformers import PreTrainedTokenizerFast, AutoTokenizer, AutoConfig, AutoModel, BertConfig, BertModel, RobertaConfig, RobertaModel, PreTrainedModel, PretrainedConfig
 
 app = Typer()
-logger = logging.getLogger("chrislab")
+logger = logging.getLogger(__name__)
 term_pattern = re.compile(re.escape("{") + "(.+?)(:.+?)?" + re.escape("}"))
 
 
 @app.command()
 def fabric_train(args_file: Path | str):
     args_file = Path(args_file)
     assert args_file.exists(), f"No args_file: {args_file}"
     args: TrainerArguments = TrainerArguments.from_json(args_file.read_text()).show()
-    new_set_logger()
     L.seed_everything(args.learning.seed)
 
     with JobTimer(f"chrialab.nlpbook.dp fabric_train {args_file}", mt=1, mb=1, rt=1, rb=1, rc='=', verbose=True, flush_sec=0.3):
         # Data
         tokenizer: PreTrainedTokenizerFast = AutoTokenizer.from_pretrained(args.model.pretrained, use_fast=True)
         assert isinstance(tokenizer, PreTrainedTokenizerFast), f"Our code support only PreTrainedTokenizerFast, but used {type(tokenizer)}"
         corpus = DPCorpus(args)
         train_dataset = DPDataset("train", args=args, corpus=corpus, tokenizer=tokenizer)
         train_dataloader = DataLoader(train_dataset,
                                       # sampler=SequentialSampler(train_dataset),  # TODO: temporary
                                       sampler=RandomSampler(train_dataset, replacement=False),
                                       num_workers=args.hardware.cpu_workers,
                                       batch_size=args.hardware.batch_size,
-                                      collate_fn=corpus.dp_encoded_examples_to_batch,
+                                      collate_fn=corpus.encoded_examples_to_batch,
                                       # drop_last=True,
                                       drop_last=False,  # TODO: temporary
                                       )
         logger.info(f"Created train_dataset providing {len(train_dataset)} examples")
         logger.info(f"Created train_dataloader loading {len(train_dataloader)} batches")
-        args.output.epoch_per_step = 1 / len(train_dataloader)
+        args.prog.epoch_per_step = 1 / len(train_dataloader)
         err_hr(c='-')
         valid_dataset = DPDataset("valid", args=args, corpus=corpus, tokenizer=tokenizer)
         valid_dataloader = DataLoader(valid_dataset,
                                       sampler=SequentialSampler(valid_dataset),
                                       num_workers=args.hardware.cpu_workers,
                                       batch_size=args.hardware.batch_size,
-                                      collate_fn=corpus.dp_encoded_examples_to_batch,
+                                      collate_fn=corpus.encoded_examples_to_batch,
                                       # drop_last=True,
                                       drop_last=False,  # TODO: temporary
                                       )
         logger.info(f"Created valid_dataset providing {len(valid_dataset)} examples")
         logger.info(f"Created valid_dataloader loading {len(valid_dataloader)} batches")
         err_hr(c='-')
 
@@ -69,59 +68,59 @@
             args.model.pretrained,
             num_labels=corpus.num_labels
         )
         pretrained_model: PreTrainedModel | BertModel | RobertaModel = AutoModel.from_pretrained(
             args.model.pretrained,
             config=pretrained_model_config
         )
-        model = DPTransformer(args, corpus, pretrained_model)
+        model = ModelForDependencyParsing(args, corpus, pretrained_model)
         err_hr(c='-')
 
         # Optimizer
-        optimizer = torch.optim.AdamW(model.parameters(), lr=args.learning.speed)
+        optimizer = torch.optim.AdamW(model.parameters(), lr=args.learning.lr)
         scheduler = torch.optim.lr_scheduler.ExponentialLR(optimizer, gamma=0.9)
 
         # Fabric
-        with RuntimeChecking(args.setup_csv_out()):
+        with RuntimeChecking(args.reconfigure_output()):
             torch.set_float32_matmul_precision('high')
             fabric = L.Fabric(
                 accelerator=args.hardware.accelerator,
                 precision=args.hardware.precision,
                 strategy=args.hardware.strategy,
                 devices=args.hardware.devices,
-                loggers=args.output.csv_out,
+                loggers=args.env.csv_logger,
             )
             fabric.setup(model, optimizer)
             train_dataloader, valid_dataloader = fabric.setup_dataloaders(train_dataloader, valid_dataloader)
             train_with_fabric(fabric, args, model, optimizer, scheduler, train_dataloader, valid_dataloader, valid_dataset)
 
 
-def train_with_fabric(fabric: L.Fabric, args: TrainerArguments, model: DPTransformer,
+def train_with_fabric(fabric: L.Fabric, args: TrainerArguments, model: ModelForDependencyParsing,
                       optimizer: torch.optim.Optimizer, scheduler: torch.optim.lr_scheduler.LRScheduler,
                       train_dataloader: DataLoader, valid_dataloader: DataLoader, valid_dataset: DPDataset):
     time_tqdm = time_tqdm_cls(bar_size=20, desc_size=8, file=sys.stdout)
     mute_tqdm = mute_tqdm_cls()
-    val_interval: float = args.learning.validating_on * len(train_dataloader) if args.learning.validating_on <= 1.0 else args.learning.validating_on
+    val_interval: float = args.learning.validate_on * len(train_dataloader) if args.learning.validate_on <= 1.0 else args.learning.validate_on
     sorted_checkpoints: List[Tuple[float, Path]] = []
-    sorting_reverse: bool = not args.learning.keeping_by.split()[0].lower().startswith("min")
-    sorting_metric: str = args.learning.keeping_by.split()[-1]
+    sorting_reverse: bool = not args.learning.save_by.split()[0].lower().startswith("min")
+    sorting_metric: str = args.learning.save_by.split()[-1]
     metric_values: Dict[str, Any] = {}
-    args.output.global_step = 0
-    args.output.global_epoch = 0.0
+    args.prog.global_step = 0
+    args.prog.global_epoch = 0.0
     for epoch in range(args.learning.epochs):
         epoch_info = f"(Epoch {epoch + 1:02d})"
-        metric_values["epoch"] = round(args.output.global_epoch, 4)
-        metric_values["trained_rate"] = round(args.output.global_epoch, 4) / args.learning.epochs
+        metric_values["epoch"] = round(args.prog.global_epoch, 4)
+        metric_values["trained_rate"] = round(args.prog.global_epoch, 4) / args.learning.epochs
         metric_values["lr"] = optimizer.param_groups[0]['lr']
         epoch_tqdm = time_tqdm if fabric.is_global_zero else mute_tqdm
         assert len(train_dataloader) > 0
         for batch_idx, batch in enumerate(epoch_tqdm(train_dataloader, position=fabric.global_rank, pre=epoch_info, desc="training", unit="batch")):
             model.train()
-            args.output.global_step += 1
-            args.output.global_epoch += args.output.epoch_per_step
+            args.prog.global_step += 1
+            args.prog.global_epoch += args.prog.epoch_per_step
             batch: Dict[str, torch.Tensor] = pop_keys(batch, "example_ids")
             inputs = {"input_ids": batch["input_ids"], "attention_mask": batch["attention_mask"]}
 
             batch_size = batch["head_ids"].size()[0]
             batch_index = torch.arange(0, int(batch_size)).long()
             max_word_length = batch["max_word_length"].item()
             head_index = (
@@ -156,34 +155,34 @@
 
             loss_arc = loss_arc[batch_index, head_index, batch["head_ids"].data.t()].transpose(0, 1)
             loss_type = loss_type[batch_index, head_index, batch["type_ids"].data.t()].transpose(0, 1)
             loss_arc = -loss_arc.sum() / num
             loss_type = -loss_type.sum() / num
             loss = loss_arc + loss_type
 
-            metric_values["epoch"] = round(args.output.global_epoch, 4)
-            metric_values["trained_rate"] = round(args.output.global_epoch, 4) / args.learning.epochs
+            metric_values["epoch"] = round(args.prog.global_epoch, 4)
+            metric_values["trained_rate"] = round(args.prog.global_epoch, 4) / args.learning.epochs
             metric_values["loss"] = loss.item()
 
             fabric.backward(loss)
             fabric.clip_gradients(model, optimizer, clip_val=0.25)
             optimizer.step()
             optimizer.zero_grad()
 
             model.eval()
             if batch_idx + 1 == len(train_dataloader) or (batch_idx + 1) % val_interval < 1:
                 validate(fabric, args, model, valid_dataloader, valid_dataset,
-                         metric_values=metric_values, print_result=args.learning.validating_fmt is not None)
+                         metric_values=metric_values, print_result=args.learning.validate_fmt is not None)
                 sorted_checkpoints = save_checkpoint(fabric, args, metric_values, model, optimizer,
                                                      sorted_checkpoints, sorting_reverse, sorting_metric)
-            fabric.log_dict(step=args.output.global_step, metrics=metric_values)
+            fabric.log_dict(step=args.prog.global_step, metrics=metric_values)
 
 
 @torch.no_grad()
-def validate(fabric: L.Fabric, args: TrainerArguments, model: DPTransformer,
+def validate(fabric: L.Fabric, args: TrainerArguments, model: ModelForDependencyParsing,
              valid_dataloader: DataLoader, valid_dataset: DPDataset,
              metric_values: Dict[str, Any], print_result: bool = True):
     metric_values["val_loss"] = torch.zeros(len(valid_dataloader))
     all_preds = []
     all_labels = []
     assert len(valid_dataloader) > 0
     for batch_idx, batch in enumerate(valid_dataloader):
@@ -243,10 +242,10 @@
     metric_values["val_loss"] = metric_values["val_loss"].mean().item()
     assert len(all_preds) > 0 and len(all_labels) and len(all_preds) == len(all_labels)
     for k, metric_tool in model.metric_tools.items():
         metric_tool(all_preds, all_labels)
         metric_values[f"val_{k}"] = metric_tool.compute()
 
     if print_result:
-        terms = [m.group(1) for m in term_pattern.finditer(args.learning.validating_fmt)]
+        terms = [m.group(1) for m in term_pattern.finditer(args.learning.validate_fmt)]
         terms = {term: metric_values[term] for term in terms}
-        fabric.print(' | ' + args.learning.validating_fmt.format(**terms))
+        fabric.print(' | ' + args.learning.validate_fmt.format(**terms))
```

### Comparing `chrislab-0.5.4/src/nlpbook/dp/corpus.py` & `chrislab-0.5.5/src/nlpbook/dp/corpus.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import logging
-import re
 from dataclasses import dataclass, field
 from pathlib import Path
-from typing import List, Optional, ClassVar, Dict
+from typing import List, Optional, Dict
 
 import torch
 from dataclasses_json import DataClassJsonMixin
 from torch.utils.data.dataset import Dataset
 
-from chrisbase.io import make_parent_dir, files, merge_dicts, out_hr, sys_stderr
-from nlpbook.arguments import TesterArguments
-from transformers import PreTrainedTokenizerFast, BatchEncoding, CharSpan
+from chrisbase.io import hr
+from nlpbook.arguments import TesterArguments, TrainerArguments
+from transformers import PreTrainedTokenizerFast, BatchEncoding
 from transformers.tokenization_utils_base import PaddingStrategy, TruncationStrategy
 
-logger = logging.getLogger("chrislab")
+logger = logging.getLogger(__name__)
 
 
 @dataclass
 class DPRawExample(DataClassJsonMixin):
     guid: str = field()
     text: str = field()
     sent_id: int = field()
@@ -37,105 +36,53 @@
     bpe_tail_mask: List[int]
     head_ids: List[int]
     dep_ids: List[int]
     pos_ids: List[int]
 
 
 class DPCorpus:
-    def __init__(self, args: TesterArguments):
+    def __init__(self, args: TesterArguments | TrainerArguments):
         self.args = args
-        self.dep_labels = [
-            "NP",
-            "NP_AJT",
-            "VP",
-            "NP_SBJ",
-            "VP_MOD",
-            "NP_OBJ",
-            "AP",
-            "NP_CNJ",
-            "NP_MOD",
-            "VNP",
-            "DP",
-            "VP_AJT",
-            "VNP_MOD",
-            "NP_CMP",
-            "VP_SBJ",
-            "VP_CMP",
-            "VP_OBJ",
-            "VNP_CMP",
-            "AP_MOD",
-            "X_AJT",
-            "VP_CNJ",
-            "VNP_AJT",
-            "IP",
-            "X",
-            "X_SBJ",
-            "VNP_OBJ",
-            "VNP_SBJ",
-            "X_OBJ",
-            "AP_AJT",
-            "L",
-            "X_MOD",
-            "X_CNJ",
-            "VNP_CNJ",
-            "X_CMP",
-            "AP_CMP",
-            "AP_SBJ",
-            "R",
-            "NP_SVJ",
-        ]
-        self.pos_labels = [
-            "NNG",
-            "NNP",
-            "NNB",
-            "NP",
-            "NR",
-            "VV",
-            "VA",
-            "VX",
-            "VCP",
-            "VCN",
-            "MMA",
-            "MMD",
-            "MMN",
-            "MAG",
-            "MAJ",
-            "JC",
-            "IC",
-            "JKS",
-            "JKC",
-            "JKG",
-            "JKO",
-            "JKB",
-            "JKV",
-            "JKQ",
-            "JX",
-            "EP",
-            "EF",
-            "EC",
-            "ETN",
-            "ETM",
-            "XPN",
-            "XSN",
-            "XSV",
-            "XSA",
-            "XR",
-            "SF",
-            "SP",
-            "SS",
-            "SE",
-            "SO",
-            "SL",
-            "SH",
-            "SW",
-            "SN",
-            "NA",
-        ]
 
-    def read_raw_examples(self, data_path: Path) -> List[DPRawExample]:
+    dep_labels = [
+        "NP", "NP_AJT", "VP", "NP_SBJ", "VP_MOD", "NP_OBJ", "AP", "NP_CNJ", "NP_MOD", "VNP",
+        "DP", "VP_AJT", "VNP_MOD", "NP_CMP", "VP_SBJ", "VP_CMP", "VP_OBJ", "VNP_CMP", "AP_MOD", "X_AJT",
+        "VP_CNJ", "VNP_AJT", "IP", "X", "X_SBJ", "VNP_OBJ", "VNP_SBJ", "X_OBJ", "AP_AJT", "L",
+        "X_MOD", "X_CNJ", "VNP_CNJ", "X_CMP", "AP_CMP", "AP_SBJ", "R", "NP_SVJ",
+    ]
+    pos_labels = [
+        "NNG", "NNP", "NNB", "NP", "NR", "VV", "VA", "VX", "VCP", "VCN",
+        "MMA", "MMD", "MMN", "MAG", "MAJ", "JC", "IC", "JKS", "JKC", "JKG",
+        "JKO", "JKB", "JKV", "JKQ", "JX", "EP", "EF", "EC", "ETN", "ETM",
+        "XPN", "XSN", "XSV", "XSA", "XR", "SF", "SP", "SS", "SE", "SO",
+        "SL", "SH", "SW", "SN", "NA",
+    ]
+
+    @property
+    def num_labels(self) -> int:
+        return len(self.get_dep_labels())
+
+    @classmethod
+    def get_dep_labels(cls) -> List[str]:
+        return cls.dep_labels
+
+    @classmethod
+    def get_pos_labels(cls) -> List[str]:
+        return cls.pos_labels
+
+    def read_raw_examples(self, split: str) -> List[DPRawExample]:
+        assert self.args.data.home, f"No data_home: {self.args.data.home}"
+        assert self.args.data.name, f"No data_name: {self.args.data.name}"
+        data_file_dict: dict = self.args.data.files.to_dict()
+        assert split in data_file_dict, f"No '{split}' split in data_file: should be one of {list(data_file_dict.keys())}"
+        assert data_file_dict[split], f"No data_file for '{split}' split: {self.args.data.files}"
+        data_path: Path = Path(self.args.data.home) / self.args.data.name / data_file_dict[split]
+        assert data_path.exists() and data_path.is_file(), f"No data_text_path: {data_path}"
+        logger.info(f"Creating features from {data_path}")
+
         sent_id = -1
         examples = []
         with data_path.open(encoding="utf-8") as inp:
             for line in inp:
                 line = line.strip()
                 if line == "" or line == "\n" or line == "\t":
                     continue
@@ -160,25 +107,192 @@
                             head=token_list[4],
                             dep=token_list[5],
                         )
                     )
         logger.info(f"Loaded {len(examples)} examples from {data_path}")
         return examples
 
-    def get_dep_labels(self) -> List[str]:
-        return self.dep_labels
+    def raw_examples_to_encoded_examples(
+            self,
+            raw_examples: List[DPRawExample],
+            tokenizer: PreTrainedTokenizerFast,
+            pos_label_list: List[str],
+            dep_label_list: List[str],
+    ) -> List[DPEncodedExample]:
+        pos_label_to_id = {label: i for i, label in enumerate(pos_label_list)}
+        dep_label_to_id = {label: i for i, label in enumerate(dep_label_list)}
+        id_to_pos_label = {i: label for i, label in enumerate(pos_label_list)}
+        id_to_dep_label = {i: label for i, label in enumerate(dep_label_list)}
+        logger.debug(f"pos_label_to_id = {pos_label_to_id}")
+        logger.debug(f"dep_label_to_id = {dep_label_to_id}")
+        logger.debug(f"id_to_pos_label = {id_to_pos_label}")
+        logger.debug(f"id_to_dep_label = {id_to_dep_label}")
+
+        SENT_ID = 0
+        token_list: List[str] = []
+        pos_list: List[str] = []
+        head_list: List[int] = []
+        dep_list: List[str] = []
+
+        encoded_examples: List[DPEncodedExample] = []
+        prev_raw_example: Optional[DPRawExample] = None
+        prev_SENT_ID: int = -1
+        for raw_example in raw_examples:
+            raw_example: DPRawExample = raw_example
+            if SENT_ID != raw_example.sent_id:
+                SENT_ID = raw_example.sent_id
+                encoded: BatchEncoding = tokenizer.encode_plus(" ".join(token_list),
+                                                               max_length=self.args.model.seq_len,
+                                                               truncation=TruncationStrategy.LONGEST_FIRST,
+                                                               padding=PaddingStrategy.MAX_LENGTH)
+                logger.debug(hr())
+                logger.debug(f"encoded.tokens()        = {encoded.tokens()}")
+                for key in encoded.keys():
+                    logger.debug(f"encoded[{key:14s}] = {encoded[key]}")
 
-    def get_pos_labels(self) -> List[str]:
-        return self.pos_labels
+                # TODO: 추후 encoded.word_to_tokens() 함수를 활용한 코드로 변경!
+                bpe_head_mask = [0]
+                bpe_tail_mask = [0]
+                head_ids = [-1]
+                dep_ids = [-1]
+                pos_ids = [-1]  # --> CLS token
+                for token, head, dep, pos in zip(token_list, head_list, dep_list, pos_list):
+                    bpe_len = len(tokenizer.tokenize(token))
+                    head_token_mask = [1] + [0] * (bpe_len - 1)
+                    tail_token_mask = [0] * (bpe_len - 1) + [1]
+                    head_mask = [head] + [-1] * (bpe_len - 1)
+                    dep_mask = [dep_label_to_id[dep]] + [-1] * (bpe_len - 1)
+                    pos_mask = [pos_label_to_id[pos]] + [-1] * (bpe_len - 1)
+                    bpe_head_mask.extend(head_token_mask)
+                    bpe_tail_mask.extend(tail_token_mask)
+                    head_ids.extend(head_mask)
+                    dep_ids.extend(dep_mask)
+                    pos_ids.extend(pos_mask)
+                bpe_head_mask.append(0)
+                bpe_tail_mask.append(0)
+                head_ids.append(-1)
+                dep_ids.append(-1)
+                pos_ids.append(-1)  # --> SEP token
+                if len(bpe_head_mask) > self.args.model.seq_len:
+                    bpe_head_mask = bpe_head_mask[:self.args.model.seq_len]
+                    bpe_tail_mask = bpe_tail_mask[:self.args.model.seq_len]
+                    head_ids = head_ids[:self.args.model.seq_len]
+                    dep_ids = dep_ids[:self.args.model.seq_len]
+                    pos_ids = pos_ids[:self.args.model.seq_len]
+                else:
+                    bpe_head_mask.extend([0] * (self.args.model.seq_len - len(bpe_head_mask)))
+                    bpe_tail_mask.extend([0] * (self.args.model.seq_len - len(bpe_tail_mask)))
+                    head_ids.extend([-1] * (self.args.model.seq_len - len(head_ids)))
+                    dep_ids.extend([-1] * (self.args.model.seq_len - len(dep_ids)))
+                    pos_ids.extend([-1] * (self.args.model.seq_len - len(pos_ids)))
+
+                encoded_example = DPEncodedExample(
+                    idx=prev_SENT_ID,
+                    raw=prev_raw_example,
+                    encoded=encoded,
+                    bpe_head_mask=bpe_head_mask,
+                    bpe_tail_mask=bpe_tail_mask,
+                    head_ids=head_ids,
+                    dep_ids=dep_ids,
+                    pos_ids=pos_ids,
+                )
+                encoded_examples.append(encoded_example)
+                logger.debug(hr())
+                logger.debug(f"bpe_head_mask           = {bpe_head_mask}")
+                logger.debug(f"bpe_tail_mask           = {bpe_tail_mask}")
+                logger.debug(f"head_ids                = {head_ids}")
+                logger.debug(f"dep_ids                 = {dep_ids}")
+                logger.debug(f"pos_ids                 = {pos_ids}")
+                logger.debug("")
+
+                token_list = []
+                head_list = []
+                dep_list = []
+                pos_list = []
+
+            token_list.append(raw_example.token)
+            pos_list.append(raw_example.pos.split("+")[-1])  # 맨 뒤 pos정보만 사용
+            head_list.append(int(raw_example.head))
+            dep_list.append(raw_example.dep)
+            prev_raw_example = raw_example
+            prev_SENT_ID = SENT_ID
+
+        encoded: BatchEncoding = tokenizer.encode_plus(" ".join(token_list),
+                                                       max_length=self.args.model.seq_len,
+                                                       truncation=TruncationStrategy.LONGEST_FIRST,
+                                                       padding=PaddingStrategy.MAX_LENGTH)
+        logger.debug(hr())
+        logger.debug(f"encoded.tokens()        = {encoded.tokens()}")
+        for key in encoded.keys():
+            logger.debug(f"encoded[{key:14s}] = {encoded[key]}")
 
-    @property
-    def num_labels(self):
-        return len(self.get_dep_labels())
+        # TODO: 추후 encoded.word_to_tokens() 함수를 활용한 코드로 변경!
+        bpe_head_mask = [0]
+        bpe_tail_mask = [0]
+        head_ids = [-1]
+        dep_ids = [-1]
+        pos_ids = [-1]  # --> CLS token
+        for token, head, dep, pos in zip(token_list, head_list, dep_list, pos_list):
+            bpe_len = len(tokenizer.tokenize(token))
+            head_token_mask = [1] + [0] * (bpe_len - 1)
+            tail_token_mask = [0] * (bpe_len - 1) + [1]
+            head_mask = [head] + [-1] * (bpe_len - 1)
+            dep_mask = [dep_label_to_id[dep]] + [-1] * (bpe_len - 1)
+            pos_mask = [pos_label_to_id[pos]] + [-1] * (bpe_len - 1)
+            bpe_head_mask.extend(head_token_mask)
+            bpe_tail_mask.extend(tail_token_mask)
+            head_ids.extend(head_mask)
+            dep_ids.extend(dep_mask)
+            pos_ids.extend(pos_mask)
+        bpe_head_mask.append(0)
+        bpe_tail_mask.append(0)
+        head_ids.append(-1)
+        dep_ids.append(-1)
+        pos_ids.append(-1)  # --> SEP token
+        bpe_head_mask.extend([0] * (self.args.model.seq_len - len(bpe_head_mask)))
+        bpe_tail_mask.extend([0] * (self.args.model.seq_len - len(bpe_tail_mask)))
+        head_ids.extend([-1] * (self.args.model.seq_len - len(head_ids)))
+        dep_ids.extend([-1] * (self.args.model.seq_len - len(dep_ids)))
+        pos_ids.extend([-1] * (self.args.model.seq_len - len(pos_ids)))
+
+        encoded_example = DPEncodedExample(
+            idx=prev_SENT_ID,
+            raw=prev_raw_example,
+            encoded=encoded,
+            bpe_head_mask=bpe_head_mask,
+            bpe_tail_mask=bpe_tail_mask,
+            head_ids=head_ids,
+            dep_ids=dep_ids,
+            pos_ids=pos_ids,
+        )
+        encoded_examples.append(encoded_example)
+        logger.debug(hr())
+        logger.debug(f"bpe_head_mask           = {bpe_head_mask}")
+        logger.debug(f"bpe_tail_mask           = {bpe_tail_mask}")
+        logger.debug(f"head_ids                = {head_ids}")
+        logger.debug(f"dep_ids                 = {dep_ids}")
+        logger.debug(f"pos_ids                 = {pos_ids}")
+        logger.debug("")
+
+        logger.info(hr())
+        for encoded_example in encoded_examples[:self.args.data.num_check]:
+            logger.info("  === [Example %s] ===" % encoded_example.idx)
+            logger.info("  = sentence      : %s" % encoded_example.raw.text)
+            logger.info("  = tokens        : %s" % " ".join(encoded_example.encoded.tokens()))
+            logger.info("  = bpe_head_mask : %s" % " ".join(str(x) for x in encoded_example.bpe_head_mask))
+            logger.info("  = bpe_tail_mask : %s" % " ".join(str(x) for x in encoded_example.bpe_tail_mask))
+            logger.info("  = head_ids      : %s" % " ".join(str(x) for x in encoded_example.head_ids))
+            logger.info("  = dep_labels    : %s" % " ".join(id_to_dep_label[x] if x in id_to_dep_label else str(x) for x in encoded_example.dep_ids))
+            logger.info("  = pos_labels    : %s" % " ".join(id_to_pos_label[x] if x in id_to_pos_label else str(x) for x in encoded_example.pos_ids))
+            logger.info("  === ")
+
+        logger.info(f"Converted {len(raw_examples)} raw examples to {len(encoded_examples)} encoded examples")
+        return encoded_examples
 
-    def dp_encoded_examples_to_batch(self, examples: List[DPEncodedExample]) -> Dict[str, torch.Tensor]:
+    def encoded_examples_to_batch(self, examples: List[DPEncodedExample]) -> Dict[str, torch.Tensor]:
         batch_size = len(examples)
         pos_padding_idx = len(self.get_pos_labels())
         first = examples[0]
         batch = {"example_ids": torch.tensor([ex.idx for ex in examples], dtype=torch.long)}
 
         # 2. build inputs : packing tensors
         # 나는 밥을 먹는다. => [CLS] 나 ##는 밥 ##을 먹 ##는 ##다 . [SEP]
@@ -224,221 +338,26 @@
             batch["mask_e"][batch_id] = torch.LongTensor([1] * (word_length + 1) + [0] * (max_word_length - word_length))
         batch["mask_d"] = batch["mask_e"][:, 1:]
 
         # 4. pack everything
         return batch
 
 
-def _convert_to_encoded_examples(
-        raw_examples: List[DPRawExample],
-        tokenizer: PreTrainedTokenizerFast,
-        args: TesterArguments,
-        pos_label_list: List[str],
-        dep_label_list: List[str],
-) -> List[DPEncodedExample]:
-    pos_label_to_id = {label: i for i, label in enumerate(pos_label_list)}
-    dep_label_to_id = {label: i for i, label in enumerate(dep_label_list)}
-    id_to_pos_label = {i: label for i, label in enumerate(pos_label_list)}
-    id_to_dep_label = {i: label for i, label in enumerate(dep_label_list)}
-    if args.env.off_debugging:
-        print(f"pos_label_to_id = {pos_label_to_id}")
-        print(f"dep_label_to_id = {dep_label_to_id}")
-        print(f"id_to_pos_label = {id_to_pos_label}")
-        print(f"id_to_dep_label = {id_to_dep_label}")
-
-    SENT_ID = 0
-    token_list: List[str] = []
-    pos_list: List[str] = []
-    head_list: List[int] = []
-    dep_list: List[str] = []
-
-    encoded_examples: List[DPEncodedExample] = []
-    prev_raw_example: Optional[DPRawExample] = None
-    prev_SENT_ID: int = -1
-    for raw_example in raw_examples:
-        raw_example: DPRawExample = raw_example
-        if SENT_ID != raw_example.sent_id:
-            SENT_ID = raw_example.sent_id
-            encoded: BatchEncoding = tokenizer.encode_plus(" ".join(token_list),
-                                                           max_length=args.model.max_seq_length,
-                                                           truncation=TruncationStrategy.LONGEST_FIRST,
-                                                           padding=PaddingStrategy.MAX_LENGTH)
-            if args.env.off_debugging:
-                out_hr()
-                print(f"encoded.tokens()        = {encoded.tokens()}")
-                for key in encoded.keys():
-                    print(f"encoded[{key:14s}] = {encoded[key]}")
-
-            # TODO: 추후 encoded.word_to_tokens() 함수를 활용한 코드로 변경!
-            bpe_head_mask = [0]
-            bpe_tail_mask = [0]
-            head_ids = [-1]
-            dep_ids = [-1]
-            pos_ids = [-1]  # --> CLS token
-            for token, head, dep, pos in zip(token_list, head_list, dep_list, pos_list):
-                bpe_len = len(tokenizer.tokenize(token))
-                head_token_mask = [1] + [0] * (bpe_len - 1)
-                tail_token_mask = [0] * (bpe_len - 1) + [1]
-                head_mask = [head] + [-1] * (bpe_len - 1)
-                dep_mask = [dep_label_to_id[dep]] + [-1] * (bpe_len - 1)
-                pos_mask = [pos_label_to_id[pos]] + [-1] * (bpe_len - 1)
-                bpe_head_mask.extend(head_token_mask)
-                bpe_tail_mask.extend(tail_token_mask)
-                head_ids.extend(head_mask)
-                dep_ids.extend(dep_mask)
-                pos_ids.extend(pos_mask)
-            bpe_head_mask.append(0)
-            bpe_tail_mask.append(0)
-            head_ids.append(-1)
-            dep_ids.append(-1)
-            pos_ids.append(-1)  # --> SEP token
-            if len(bpe_head_mask) > args.model.max_seq_length:
-                bpe_head_mask = bpe_head_mask[:args.model.max_seq_length]
-                bpe_tail_mask = bpe_tail_mask[:args.model.max_seq_length]
-                head_ids = head_ids[:args.model.max_seq_length]
-                dep_ids = dep_ids[:args.model.max_seq_length]
-                pos_ids = pos_ids[:args.model.max_seq_length]
-            else:
-                bpe_head_mask.extend([0] * (args.model.max_seq_length - len(bpe_head_mask)))
-                bpe_tail_mask.extend([0] * (args.model.max_seq_length - len(bpe_tail_mask)))
-                head_ids.extend([-1] * (args.model.max_seq_length - len(head_ids)))
-                dep_ids.extend([-1] * (args.model.max_seq_length - len(dep_ids)))
-                pos_ids.extend([-1] * (args.model.max_seq_length - len(pos_ids)))
-
-            encoded_example = DPEncodedExample(
-                idx=prev_SENT_ID,
-                raw=prev_raw_example,
-                encoded=encoded,
-                bpe_head_mask=bpe_head_mask,
-                bpe_tail_mask=bpe_tail_mask,
-                head_ids=head_ids,
-                dep_ids=dep_ids,
-                pos_ids=pos_ids,
-            )
-            encoded_examples.append(encoded_example)
-            if args.env.off_debugging:
-                out_hr()
-                print(f"bpe_head_mask           = {bpe_head_mask}")
-                print(f"bpe_tail_mask           = {bpe_tail_mask}")
-                print(f"head_ids                = {head_ids}")
-                print(f"dep_ids                 = {dep_ids}")
-                print(f"pos_ids                 = {pos_ids}")
-                print()
-
-            token_list = []
-            head_list = []
-            dep_list = []
-            pos_list = []
-
-        token_list.append(raw_example.token)
-        pos_list.append(raw_example.pos.split("+")[-1])  # 맨 뒤 pos정보만 사용
-        head_list.append(int(raw_example.head))
-        dep_list.append(raw_example.dep)
-        prev_raw_example = raw_example
-        prev_SENT_ID = SENT_ID
-
-    encoded: BatchEncoding = tokenizer.encode_plus(" ".join(token_list),
-                                                   max_length=args.model.max_seq_length,
-                                                   truncation=TruncationStrategy.LONGEST_FIRST,
-                                                   padding=PaddingStrategy.MAX_LENGTH)
-    if args.env.off_debugging:
-        out_hr()
-        print(f"encoded.tokens()        = {encoded.tokens()}")
-        for key in encoded.keys():
-            print(f"encoded[{key:14s}] = {encoded[key]}")
-
-    # TODO: 추후 encoded.word_to_tokens() 함수를 활용한 코드로 변경!
-    bpe_head_mask = [0]
-    bpe_tail_mask = [0]
-    head_ids = [-1]
-    dep_ids = [-1]
-    pos_ids = [-1]  # --> CLS token
-    for token, head, dep, pos in zip(token_list, head_list, dep_list, pos_list):
-        bpe_len = len(tokenizer.tokenize(token))
-        head_token_mask = [1] + [0] * (bpe_len - 1)
-        tail_token_mask = [0] * (bpe_len - 1) + [1]
-        head_mask = [head] + [-1] * (bpe_len - 1)
-        dep_mask = [dep_label_to_id[dep]] + [-1] * (bpe_len - 1)
-        pos_mask = [pos_label_to_id[pos]] + [-1] * (bpe_len - 1)
-        bpe_head_mask.extend(head_token_mask)
-        bpe_tail_mask.extend(tail_token_mask)
-        head_ids.extend(head_mask)
-        dep_ids.extend(dep_mask)
-        pos_ids.extend(pos_mask)
-    bpe_head_mask.append(0)
-    bpe_tail_mask.append(0)
-    head_ids.append(-1)
-    dep_ids.append(-1)
-    pos_ids.append(-1)  # --> SEP token
-    bpe_head_mask.extend([0] * (args.model.max_seq_length - len(bpe_head_mask)))
-    bpe_tail_mask.extend([0] * (args.model.max_seq_length - len(bpe_tail_mask)))
-    head_ids.extend([-1] * (args.model.max_seq_length - len(head_ids)))
-    dep_ids.extend([-1] * (args.model.max_seq_length - len(dep_ids)))
-    pos_ids.extend([-1] * (args.model.max_seq_length - len(pos_ids)))
-
-    encoded_example = DPEncodedExample(
-        idx=prev_SENT_ID,
-        raw=prev_raw_example,
-        encoded=encoded,
-        bpe_head_mask=bpe_head_mask,
-        bpe_tail_mask=bpe_tail_mask,
-        head_ids=head_ids,
-        dep_ids=dep_ids,
-        pos_ids=pos_ids,
-    )
-    encoded_examples.append(encoded_example)
-    if args.env.off_debugging:
-        out_hr()
-        print(f"bpe_head_mask           = {bpe_head_mask}")
-        print(f"bpe_tail_mask           = {bpe_tail_mask}")
-        print(f"head_ids                = {head_ids}")
-        print(f"dep_ids                 = {dep_ids}")
-        print(f"pos_ids                 = {pos_ids}")
-        print()
-
-    if args.env.off_debugging:
-        out_hr()
-    for encoded_example in encoded_examples[:args.data.show_examples]:
-        logger.info("  === [Example %s] ===" % encoded_example.idx)
-        logger.info("  = sentence      : %s" % encoded_example.raw.text)
-        logger.info("  = tokens        : %s" % " ".join(encoded_example.encoded.tokens()))
-        logger.info("  = bpe_head_mask : %s" % " ".join(str(x) for x in encoded_example.bpe_head_mask))
-        logger.info("  = bpe_tail_mask : %s" % " ".join(str(x) for x in encoded_example.bpe_tail_mask))
-        logger.info("  = head_ids      : %s" % " ".join(str(x) for x in encoded_example.head_ids))
-        logger.info("  = dep_labels    : %s" % " ".join(id_to_dep_label[x] if x in id_to_dep_label else str(x) for x in encoded_example.dep_ids))
-        logger.info("  = pos_labels    : %s" % " ".join(id_to_pos_label[x] if x in id_to_pos_label else str(x) for x in encoded_example.pos_ids))
-        logger.info("  === ")
-
-    logger.info(f"Converted {len(raw_examples)} raw examples to {len(encoded_examples)} encoded examples")
-    return encoded_examples
-
-
 class DPDataset(Dataset):
-    def __init__(self, split: str, args: TesterArguments, tokenizer: PreTrainedTokenizerFast, corpus: DPCorpus):
-        assert corpus, "corpus is not valid"
-        assert args.data.home, f"No data_home: {args.data.home}"
-        assert args.data.name, f"No data_name: {args.data.name}"
+    def __init__(self, split: str, tokenizer: PreTrainedTokenizerFast, corpus: DPCorpus):
         self.corpus: DPCorpus = corpus
-        data_file_dict: dict = args.data.files.to_dict()
-        assert split in data_file_dict, f"No '{split}' split in data_file: should be one of {list(data_file_dict.keys())}"
-        assert data_file_dict[split], f"No data_file for '{split}' split: {args.data.files}"
-        text_data_path: Path = Path(args.data.home) / args.data.name / data_file_dict[split]
-        assert text_data_path.exists() and text_data_path.is_file(), f"No data_text_path: {text_data_path}"
-        logger.info(f"Creating features from dataset file at {text_data_path}")
-        examples: List[DPRawExample] = self.corpus.read_raw_examples(text_data_path)
+        examples: List[DPRawExample] = self.corpus.read_raw_examples(split)
         self.dep_labels: List[str] = self.corpus.get_dep_labels()
         self.pos_labels: List[str] = self.corpus.get_pos_labels()
         self._dep_label_to_id: Dict[str, int] = {label: i for i, label in enumerate(self.dep_labels)}
         self._pos_label_to_id: Dict[str, int] = {label: i for i, label in enumerate(self.pos_labels)}
         self._id_to_dep_label: Dict[int, str] = {i: label for i, label in enumerate(self.dep_labels)}
         self._id_to_pos_label: Dict[int, str] = {i: label for i, label in enumerate(self.pos_labels)}
-        self.features: List[DPEncodedExample] = \
-            _convert_to_encoded_examples(examples, tokenizer, args,
-                                         pos_label_list=self.pos_labels,
-                                         dep_label_list=self.dep_labels)
+        self.features: List[DPEncodedExample] = self.corpus.raw_examples_to_encoded_examples(
+            examples, tokenizer, pos_label_list=self.pos_labels, dep_label_list=self.dep_labels)
 
     def __len__(self) -> int:
         return len(self.features)
 
     def __getitem__(self, i) -> DPEncodedExample:
         return self.features[i]
```

### Comparing `chrislab-0.5.4/src/nlpbook/dp/model.py` & `chrislab-0.5.5/src/nlpbook/dp/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,31 +3,29 @@
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.nn.parameter import Parameter
 from torch.nn.utils.rnn import pack_padded_sequence, pad_packed_sequence
 
-from nlpbook import TrainerArguments
 from nlpbook.dp.corpus import DPCorpus
 from nlpbook.metrics import DP_UASMacroF1, DP_UASMicroF1, DP_LASMacroF1, DP_LASMicroF1
 from transformers import PreTrainedModel
 from transformers.modeling_outputs import BaseModelOutputWithPoolingAndCrossAttentions
 
 metric_tools_for_DP = {
     "UASa": DP_UASMacroF1,
     "UASi": DP_UASMicroF1,
     "LASa": DP_LASMacroF1,
     "LASi": DP_LASMicroF1,
 }
 
 
-class DPTransformer(nn.Module):
+class ModelForDependencyParsing(nn.Module):
     def __init__(self,
-                 args: TrainerArguments,
                  corpus: DPCorpus,
                  pretrained_model: PreTrainedModel,
                  ):
         super().__init__()
         self.metric_tools = nn.ModuleDict(metric_tools_for_DP)
         self.encoder_layers = 1  # Number of layers of encoder
         self.decoder_layers = 1  # Number of layers of decoder
```

### Comparing `chrislab-0.5.4/src/nlpbook/generation/arguments.py` & `chrislab-0.5.5/src/nlpbook/generation/arguments.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.4/src/nlpbook/generation/corpus.py` & `chrislab-0.5.5/src/nlpbook/generation/corpus.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import torch
 from filelock import FileLock
 from torch.utils.data.dataset import Dataset
 
 from nlpbook.generation.arguments import GenerationTrainArguments
 from transformers import PreTrainedTokenizerFast
 
-logger = logging.getLogger("chrislab")
+logger = logging.getLogger(__name__)
 
 
 @dataclass
 class GenerationExample:
     text: str
 
 
@@ -129,15 +129,15 @@
                     f"Loading features from cached file {cached_features_file} [took %.3f s]", time.time() - start
                 )
             else:
                 corpus_path = os.path.join(
                     args.downstream_corpus_root_dir,
                     args.downstream_corpus_name,
                 )
-                logger.info(f"Creating features from dataset file at {corpus_path}")
+                logger.info(f"Creating features from {corpus_path}")
                 examples = self.corpus.get_examples(corpus_path, mode)
                 tokenizer.pad_token = tokenizer.eos_token
                 self.features = convert_examples_to_features_fn(
                     examples,
                     tokenizer,
                     args,
                 )
```

### Comparing `chrislab-0.5.4/src/nlpbook/generation/deploy.py` & `chrislab-0.5.5/src/nlpbook/generation/deploy.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.4/src/nlpbook/generation/task.py` & `chrislab-0.5.5/src/nlpbook/generation/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from lightning.pytorch import LightningModule
-from nlpbook.generation.arguments import GenerationTrainArguments
+from pytorch_lightning import LightningModule
 from torch.optim import AdamW
 from torch.optim.lr_scheduler import ExponentialLR
 from transformers import PreTrainedModel
 
+from nlpbook.generation.arguments import GenerationTrainArguments
+
 
 class GenerationTask(LightningModule):
 
     def __init__(self,
                  model: PreTrainedModel,
                  args: GenerationTrainArguments,
                  ):
```

### Comparing `chrislab-0.5.4/src/nlpbook/metrics.py` & `chrislab-0.5.5/src/nlpbook/metrics.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from typing import Any, Optional, List, Callable
 
 import numpy as np
 import torch
 from seqeval import metrics as se_metrics
 from seqeval import scheme as se_scheme
 from sklearn import metrics as sk_metrics
-from torchmetrics import Metric
 
 
 def accuracy(preds, labels, ignore_index=None):
     with torch.no_grad():
         assert preds.shape[0] == len(labels)
         correct = torch.sum(preds == labels)
         total = torch.sum(torch.ones_like(labels))
@@ -18,35 +17,30 @@
             # 모델이 맞춘 것 가운데 ignore index에 해당하는 것 제외
             correct -= torch.sum(torch.logical_and(preds == ignore_index, preds == labels))
             # accuracy의 분모 가운데 ignore index에 해당하는 것 제외
             total -= torch.sum(labels == ignore_index)
     return correct.to(dtype=torch.float) / total.to(dtype=torch.float)
 
 
-class BasicMetricTool(Metric):
+class BasicMetricTool(torch.nn.Module):
     """Base class for metrics."""
 
     def __init__(
             self,
             metric_fn: Callable,
-            compute_on_step: bool = True,
-            dist_sync_on_step: bool = False,
-            process_group: Optional[Any] = None,
-            dist_sync_fn: Optional[Callable] = None,
     ) -> None:
-        super().__init__(
-            compute_on_step=compute_on_step,
-            dist_sync_on_step=dist_sync_on_step,
-            process_group=process_group,
-            dist_sync_fn=dist_sync_fn,
-        )
-        self.add_state("preds", default=[], dist_reduce_fx=None)
-        self.add_state("targets", default=[], dist_reduce_fx=None)
+        super().__init__()
+        self.preds = []
+        self.targets = []
         self.metric_fn = metric_fn
 
+    def reset(self) -> None:
+        self.preds = []
+        self.targets = []
+
     def update(self, preds: torch.Tensor, targets: torch.Tensor) -> None:
         self.preds.append(preds)
         self.targets.append(targets)
 
     def compute(self) -> Any:
         preds = self.preds
         targets = self.targets
@@ -55,41 +49,29 @@
             preds = torch.cat(preds, dim=0)
             preds = preds.cpu().numpy()
         if type(targets[0]) == torch.Tensor:
             targets = torch.cat(targets, dim=0)
             targets = targets.cpu().numpy()
 
         score = self.metric_fn(preds, targets)
-        score = torch.tensor(score).to(self.device)
         return score
 
 
 class LabelMetricTool(BasicMetricTool):
     """Metrics requiring label information."""
 
     def __init__(
             self,
             metric_fn: Callable,
-            compute_on_step: bool = True,
-            dist_sync_on_step: bool = False,
-            process_group: Optional[Any] = None,
-            dist_sync_fn: Optional[Callable] = None,
     ) -> None:
-        super().__init__(
-            metric_fn=metric_fn,
-            compute_on_step=compute_on_step,
-            dist_sync_on_step=dist_sync_on_step,
-            process_group=process_group,
-            dist_sync_fn=dist_sync_fn,
-        )
+        super().__init__(metric_fn=metric_fn)
         self.label_info = None
 
     def update(self, preds: torch.Tensor, targets: torch.Tensor, label_info: Optional[Any] = None) -> None:
-        self.preds.append(preds)
-        self.targets.append(targets)
+        super().update(preds, targets)
         if self.label_info is None:
             self.label_info = label_info
 
     def compute(self) -> Any:
         preds = self.preds
         targets = self.targets
 
@@ -97,15 +79,14 @@
             preds = torch.cat(preds, dim=0)
             preds = preds.cpu().numpy()
         if type(targets[0]) == torch.Tensor:
             targets = torch.cat(targets, dim=0)
             targets = targets.cpu().numpy()
 
         score = self.metric_fn(preds, targets, self.label_info)
-        score = torch.tensor(score).to(self.device)
         return score
 
 
 @dataclass
 class DPResult:
     heads: torch.Tensor
     types: torch.Tensor
```

### Comparing `chrislab-0.5.4/src/nlpbook/ner/cli.py` & `chrislab-0.5.5/src/nlpbook/ner/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,70 +1,68 @@
 import logging
 import sys
 from pathlib import Path
 from typing import Any, Dict, List, Tuple
 
 import lightning as L
-import lightning.pytorch as pl
 import torch
 from flask import Flask
 from torch import Tensor
 from torch.utils.data import DataLoader, RandomSampler, SequentialSampler
 from transformers import PreTrainedTokenizerFast, AutoTokenizer, AutoConfig, AutoModelForTokenClassification, BertForTokenClassification, CharSpan
 from transformers.modeling_outputs import TokenClassifierOutput
 from typer import Typer
 
 import nlpbook
 from chrisbase.io import JobTimer, pop_keys, err_hr, out_hr
 from chrislab.common.util import time_tqdm_cls, mute_tqdm_cls
 from nlpbook import save_checkpoint, TERM_IN_NAME_FORMAT
 from nlpbook.arguments import TrainerArguments, ServerArguments, TesterArguments, RuntimeChecking
 from nlpbook.metrics import accuracy, NER_CharMacroF1, NER_EntityMacroF1, klue_ner_char_macro_f1, klue_ner_entity_macro_f1
-from nlpbook.ner.corpus import NERCorpus, NERDataset, ner_encoded_examples_to_batch, NEREncodedExample
+from nlpbook.ner.corpus import NERCorpus, NERDataset, NEREncodedExample
 from nlpbook.ner.task import NERTask
 
 app = Typer()
-logger = logging.getLogger("chrislab")
+logger = logging.getLogger(__name__)
 
 metric_tools_for_NER = {
     "F1c": NER_CharMacroF1,
     "F1e": NER_EntityMacroF1,
 }
 
 
 @app.command()
 def fabric_train(args_file: Path | str):
     args_file = Path(args_file)
     assert args_file.exists(), f"No args_file: {args_file}"
     args: TrainerArguments = TrainerArguments.from_json(args_file.read_text()).show()
-    new_set_logger()
     L.seed_everything(args.learning.seed)
 
     with JobTimer(f"chrialab.nlpbook.ner fabric_train {args_file}", mt=1, mb=1, rt=1, rb=1, rc='=', verbose=True, flush_sec=0.3):
         # Data
         tokenizer: PreTrainedTokenizerFast = AutoTokenizer.from_pretrained(args.model.pretrained, use_fast=True)
         assert isinstance(tokenizer, PreTrainedTokenizerFast), f"Our code support only PreTrainedTokenizerFast, but used {type(tokenizer)}"
-        corpus = NERCorpus(args)
-        train_dataset = NERDataset("train", args=args, corpus=corpus, tokenizer=tokenizer)
+        corpus = NERCorpus(args=args)
+        train_dataset = NERDataset("train", corpus=corpus, tokenizer=tokenizer)
         train_dataloader = DataLoader(train_dataset,
                                       sampler=RandomSampler(train_dataset, replacement=False),
                                       num_workers=args.hardware.cpu_workers,
                                       batch_size=args.hardware.batch_size,
-                                      collate_fn=ner_encoded_examples_to_batch,
+                                      collate_fn=corpus.encoded_examples_to_batch,
                                       drop_last=True)
         logger.info(f"Created train_dataset providing {len(train_dataset)} examples")
         logger.info(f"Created train_dataloader loading {len(train_dataloader)} batches")
-        args.output.epoch_per_step = 1 / len(train_dataloader)
+        args.prog.epoch_per_step = 1 / len(train_dataloader)
         err_hr(c='-')
-        valid_dataset = NERDataset("valid", args=args, corpus=corpus, tokenizer=tokenizer)
+        valid_dataset = NERDataset("valid", corpus=corpus, tokenizer=tokenizer)
         valid_dataloader = DataLoader(valid_dataset,
                                       sampler=SequentialSampler(valid_dataset),
                                       num_workers=args.hardware.cpu_workers,
                                       batch_size=args.hardware.batch_size,
-                                      collate_fn=ner_encoded_examples_to_batch,
+                                      collate_fn=corpus.encoded_examples_to_batch,
                                       drop_last=True)
         logger.info(f"Created valid_dataset providing {len(valid_dataset)} examples")
         logger.info(f"Created valid_dataloader loading {len(valid_dataloader)} batches")
         err_hr(c='-')
 
         # Model
         pretrained_model_config = AutoConfig.from_pretrained(
@@ -74,67 +72,67 @@
         model = AutoModelForTokenClassification.from_pretrained(
             args.model.pretrained,
             config=pretrained_model_config
         )
         err_hr(c='-')
 
         # Optimizer
-        optimizer = torch.optim.AdamW(model.parameters(), lr=args.learning.speed)
+        optimizer = torch.optim.AdamW(model.parameters(), lr=args.learning.lr)
         scheduler = torch.optim.lr_scheduler.ExponentialLR(optimizer, gamma=0.9)
 
         # Fabric
-        with RuntimeChecking(args.setup_csv_out()):
+        with RuntimeChecking(args.reconfigure_output()):
             torch.set_float32_matmul_precision('high')
-            fabric = L.Fabric(loggers=args.output.csv_out)
+            fabric = L.Fabric(loggers=args.env.csv_logger)
             fabric.setup(model, optimizer)
             train_dataloader, valid_dataloader = fabric.setup_dataloaders(train_dataloader, valid_dataloader)
             train_with_fabric(fabric, args, model, optimizer, scheduler, train_dataloader, valid_dataloader, valid_dataset)
 
 
 def train_with_fabric(fabric: L.Fabric, args: TrainerArguments, model: torch.nn.Module,
                       optimizer: torch.optim.Optimizer, scheduler: torch.optim.lr_scheduler._LRScheduler,
                       train_dataloader: DataLoader, valid_dataloader: DataLoader, valid_dataset: NERDataset):
     time_tqdm = time_tqdm_cls(bar_size=20, desc_size=8, file=sys.stdout)
     mute_tqdm = mute_tqdm_cls()
-    val_interval: float = args.learning.validating_on * len(train_dataloader) if args.learning.validating_on <= 1.0 else args.learning.validating_on
+    val_interval: float = args.learning.validate_on * len(train_dataloader) if args.learning.validate_on <= 1.0 else args.learning.validate_on
     sorted_checkpoints: List[Tuple[float, Path]] = []
-    sorting_reverse: bool = not args.learning.keeping_by.split()[0].lower().startswith("min")
-    sorting_metric: str = args.learning.keeping_by.split()[-1]
+    sorting_reverse: bool = not args.learning.save_by.split()[0].lower().startswith("min")
+    sorting_metric: str = args.learning.save_by.split()[-1]
     metrics: Dict[str, Any] = {}
-    args.output.global_step = 0
-    args.output.global_epoch = 0.0
+    args.prog.global_step = 0
+    args.prog.global_epoch = 0.0
     for epoch in range(args.learning.epochs):
         epoch_info = f"(Epoch {epoch + 1:02d})"
-        metrics["epoch"] = round(args.output.global_epoch, 4)
-        metrics["trained_rate"] = round(args.output.global_epoch, 4) / args.learning.epochs
+        metrics["epoch"] = round(args.prog.global_epoch, 4)
+        metrics["trained_rate"] = round(args.prog.global_epoch, 4) / args.learning.epochs
         metrics["lr"] = optimizer.param_groups[0]['lr']
         epoch_tqdm = time_tqdm if fabric.is_global_zero else mute_tqdm
         for batch_idx, batch in enumerate(epoch_tqdm(train_dataloader, position=fabric.global_rank, pre=epoch_info,
                                                      desc=f"training", unit=f"x{train_dataloader.batch_size}")):
-            args.output.global_step += 1
-            args.output.global_epoch += args.output.epoch_per_step
+            args.prog.global_step += 1
+            args.prog.global_epoch += args.prog.epoch_per_step
             batch: Dict[str, torch.Tensor] = pop_keys(batch, "example_ids")
             outputs: TokenClassifierOutput = model(**batch)
             labels: torch.Tensor = batch["labels"]
             preds: torch.Tensor = outputs.logits.argmax(dim=-1)
             acc: torch.Tensor = accuracy(preds, labels, ignore_index=0)
-            metrics["epoch"] = round(args.output.global_epoch, 4)
-            metrics["trained_rate"] = round(args.output.global_epoch, 4) / args.learning.epochs
+            metrics["epoch"] = round(args.prog.global_epoch, 4)
+            metrics["trained_rate"] = round(args.prog.global_epoch, 4) / args.learning.epochs
             metrics["loss"] = outputs.loss.item()
             metrics["acc"] = acc.item()
             fabric.backward(outputs.loss)
             fabric.clip_gradients(model, optimizer, clip_val=0.25)
             optimizer.step()
             optimizer.zero_grad()
             model.eval()
             if batch_idx + 1 == len(train_dataloader) or (batch_idx + 1) % val_interval < 1:
-                validate(fabric, args, model, valid_dataloader, valid_dataset, metrics=metrics, print_result=args.learning.validating_fmt is not None)
+                validate(fabric, args, model, valid_dataloader, valid_dataset, metrics=metrics, print_result=args.learning.validate_fmt is not None)
                 sorted_checkpoints = save_checkpoint(fabric, args, metrics, model, optimizer,
                                                      sorted_checkpoints, sorting_reverse, sorting_metric)
-            fabric.log_dict(step=args.output.global_step, metrics=metrics)
+            fabric.log_dict(step=args.prog.global_step, metrics=metrics)
             model.train()
         scheduler.step()
         metrics["lr"] = optimizer.param_groups[0]['lr']
         if epoch + 1 < args.learning.epochs:
             out_hr('-')
 
 
@@ -160,15 +158,15 @@
         preds: torch.Tensor = outputs.logits.argmax(dim=-1)
         # acc: torch.Tensor = accuracy(preds, labels, ignore_index=0)
         for example_id, pred_ids in zip(example_ids.tolist(), preds.tolist()):
             pred_labels = [valid_dataset.id_to_label(x) for x in pred_ids]
             encoded_example: NEREncodedExample = valid_dataset[example_id]
             offset_to_label: Dict[int, str] = encoded_example.raw.get_offset_label_dict()
             char_label_pairs: List[Tuple[str | None, str | None]] = [(None, None)] * len(encoded_example.raw.character_list)
-            for token_id in range(args.model.max_seq_length):
+            for token_id in range(args.model.seq_len):
                 token_span: CharSpan = encoded_example.encoded.token_to_chars(token_id)
                 if token_span:
                     char_pred_tags = label_to_char_labels(pred_labels[token_id], token_span.end - token_span.start)
                     for offset, char_pred_tag in zip(range(token_span.start, token_span.end), char_pred_tags):
                         char_label_pairs[offset] = (offset_to_label[offset], char_pred_tag)
             whole_char_label_pairs.extend([(valid_dataset.label_to_id(y), valid_dataset.label_to_id(p))
                                            for y, p in char_label_pairs if y and p])
@@ -177,17 +175,17 @@
     metrics["val_loss"] = metrics["val_loss"].mean().item()
     # metrics["val_acc"] = metrics["val_acc"].mean().item()
     char_preds, char_labels = ([p for (y, p) in whole_char_label_pairs],
                                [y for (y, p) in whole_char_label_pairs])
     metrics["val_F1c"] = klue_ner_char_macro_f1(preds=char_preds, labels=char_labels, label_list=valid_dataset.get_labels())
     metrics["val_F1e"] = klue_ner_entity_macro_f1(preds=char_preds, labels=char_labels, label_list=valid_dataset.get_labels())
     if print_result:
-        terms = [m.group(1) for m in TERM_IN_NAME_FORMAT.finditer(args.learning.validating_fmt)]
+        terms = [m.group(1) for m in TERM_IN_NAME_FORMAT.finditer(args.learning.validate_fmt)]
         terms = {term: metrics[term] for term in terms}
-        fabric.print(' | ' + args.learning.validating_fmt.format(**terms))
+        fabric.print(' | ' + args.learning.validate_fmt.format(**terms))
 
 
 @app.command()
 def train(args_file: Path | str):
     nlpbook.set_logger()
     args_file = Path(args_file)
     assert args_file.exists(), f"No args_file: {args_file}"
@@ -198,41 +196,41 @@
         if args.data.redownload:
             nlpbook.download_downstream_dataset(args)
             err_hr(c='-')
 
         corpus = NERCorpus(args)
         tokenizer: PreTrainedTokenizerFast = AutoTokenizer.from_pretrained(args.model.pretrained, use_fast=True)
         assert isinstance(tokenizer, PreTrainedTokenizerFast), f"Our code support only PreTrainedTokenizerFast, but used {type(tokenizer)}"
-        train_dataset = NERDataset("train", args=args, corpus=corpus, tokenizer=tokenizer)
+        train_dataset = NERDataset("train", corpus=corpus, tokenizer=tokenizer)
         train_dataloader = DataLoader(train_dataset, sampler=RandomSampler(train_dataset, replacement=False),
                                       num_workers=args.hardware.cpu_workers,
                                       batch_size=args.hardware.batch_size,
-                                      collate_fn=ner_encoded_examples_to_batch,
+                                      collate_fn=corpus.encoded_examples_to_batch,
                                       drop_last=False)
         err_hr(c='-')
 
-        val_dataset = NERDataset("valid", args=args, corpus=corpus, tokenizer=tokenizer)
+        val_dataset = NERDataset("valid", corpus=corpus, tokenizer=tokenizer)
         val_dataloader = DataLoader(val_dataset, sampler=SequentialSampler(val_dataset),
                                     num_workers=args.hardware.cpu_workers,
                                     batch_size=args.hardware.batch_size,
-                                    collate_fn=ner_encoded_examples_to_batch,
+                                    collate_fn=corpus.encoded_examples_to_batch,
                                     drop_last=False)
         err_hr(c='-')
 
         pretrained_model_config = AutoConfig.from_pretrained(
             args.model.pretrained,
             num_labels=corpus.num_labels
         )
         model = AutoModelForTokenClassification.from_pretrained(
             args.model.pretrained,
             config=pretrained_model_config
         )
         err_hr(c='-')
 
-        with RuntimeChecking(nlpbook.setup_csv_out(args)):
+        with RuntimeChecking(args.reconfigure_output()):
             torch.set_float32_matmul_precision('high')
             trainer: pl.Trainer = nlpbook.make_trainer(args)
             trainer.fit(NERTask(model=model, args=args, trainer=trainer, val_dataset=val_dataset,
                                 total_steps=len(train_dataloader) * args.learning.epochs),
                         train_dataloaders=train_dataloader,
                         val_dataloaders=val_dataloader)
 
@@ -241,26 +239,26 @@
 def test(args_file: Path | str):
     nlpbook.set_logger()
     args_file = Path(args_file)
     assert args_file.exists(), f"No args_file: {args_file}"
     args = TesterArguments.from_json(args_file.read_text()).show()
 
     with JobTimer(f"chrialab.nlpbook.ner test {args_file}", mt=1, mb=1, rt=1, rb=1, rc='=', verbose=True, flush_sec=0.3):
-        checkpoint_path = args.output.dir_path / args.model.finetuning_name
+        checkpoint_path = args.env.output_home / args.model.name
         assert checkpoint_path.exists(), f"No checkpoint file: {checkpoint_path}"
         logger.info(f"Using finetuned checkpoint file at {checkpoint_path}")
         err_hr(c='-')
 
         nlpbook.download_downstream_dataset(args)
         err_hr(c='-')
 
         corpus = NERCorpus(args)
         tokenizer: PreTrainedTokenizerFast = AutoTokenizer.from_pretrained(args.model.pretrained, use_fast=True)
         assert isinstance(tokenizer, PreTrainedTokenizerFast), f"Our code support only PreTrainedTokenizerFast, but used {type(tokenizer)}"
-        test_dataset = NERDataset("test", args=args, corpus=corpus, tokenizer=tokenizer)
+        test_dataset = NERDataset("test", corpus=corpus, tokenizer=tokenizer)
         test_dataloader = DataLoader(test_dataset,
                                      batch_size=args.hardware.batch_size,
                                      num_workers=args.hardware.cpu_workers,
                                      sampler=SequentialSampler(test_dataset),
                                      collate_fn=nlpbook.data_collator,
                                      drop_last=False)
         err_hr(c='-')
@@ -270,40 +268,39 @@
             num_labels=corpus.num_labels
         )
         model = AutoModelForTokenClassification.from_pretrained(
             args.model.pretrained,
             config=pretrained_model_config
         )
         err_hr(c='-')
-
-        with RuntimeChecking(nlpbook.setup_csv_out(args)):
-            torch.set_float32_matmul_precision('high')
-            tester: pl.Trainer = nlpbook.make_tester(args)
-            tester.test(NERTask(model, args, tester),
-                        dataloaders=test_dataloader,
-                        ckpt_path=checkpoint_path)
+    with RuntimeChecking(args.reconfigure_output()):
+        torch.set_float32_matmul_precision('high')
+        tester: pl.Trainer = nlpbook.make_tester(args)
+        tester.test(NERTask(model, args, tester),
+                    dataloaders=test_dataloader,
+                    ckpt_path=checkpoint_path)
 
 
 @app.command()
 def serve(args_file: Path | str):
     nlpbook.set_logger()
     args_file = Path(args_file)
     assert args_file.exists(), f"No args_file file: {args_file}"
     args: ServerArguments = ServerArguments.from_json(args_file.read_text()).show()
 
     with JobTimer(f"chrialab.nlpbook serve_ner {args_file}", mt=1, mb=1, rt=1, rb=1, rc='=', verbose=True, flush_sec=0.3):
-        checkpoint_path = args.output.dir_path / args.model.finetuning_name
+        checkpoint_path = args.env.output_home / args.model.name
         assert checkpoint_path.exists(), f"No checkpoint file: {checkpoint_path}"
         checkpoint: dict = torch.load(checkpoint_path, map_location=torch.device("cpu"))
         logger.info(f"Using finetuned checkpoint file at {checkpoint_path}")
         err_hr(c='-')
 
         tokenizer: PreTrainedTokenizerFast = AutoTokenizer.from_pretrained(args.model.pretrained, use_fast=True)
         assert isinstance(tokenizer, PreTrainedTokenizerFast), f"Our code support only PreTrainedTokenizerFast, but used {type(tokenizer)}"
-        label_map_path: Path = args.output.dir_path / "label_map.txt"
+        label_map_path: Path = args.env.output_home / "label_map.txt"
         assert label_map_path.exists(), f"No downstream label file: {label_map_path}"
         labels = label_map_path.read_text().splitlines(keepends=False)
         id_to_label = {idx: label for idx, label in enumerate(labels)}
 
         pretrained_model_config = AutoConfig.from_pretrained(
             args.model.pretrained,
             num_labels=checkpoint['state_dict']['model.classifier.bias'].shape.numel(),
@@ -312,15 +309,15 @@
         model.load_state_dict({k.replace("model.", ""): v for k, v in checkpoint['state_dict'].items()})
         model.eval()
         err_hr(c='-')
 
         def inference_fn(sentence):
             inputs = tokenizer(
                 [sentence],
-                max_length=args.model.max_seq_length,
+                max_length=args.model.seq_len,
                 padding="max_length",
                 truncation=True,
             )
             with torch.no_grad():
                 outputs: TokenClassifierOutput = model(**{k: torch.tensor(v) for k, v in inputs.items()})
                 all_probs: Tensor = outputs.logits[0].softmax(dim=1)
                 top_probs, top_preds = torch.topk(all_probs, dim=1, k=1)
@@ -336,12 +333,12 @@
                         "prob": f"{round(top_prob[0].item(), 4):.4f}",
                     })
             return {
                 'sentence': sentence,
                 'result': result,
             }
 
-        with RuntimeChecking(nlpbook.setup_csv_out(args)):
+        with RuntimeChecking(args.reconfigure_output()):
             server: Flask = nlpbook.make_server(inference_fn,
                                                 template_file="serve_ner.html",
                                                 ngrok_home=args.env.working_path)
             server.run()
```

### Comparing `chrislab-0.5.4/src/nlpbook/ner/corpus.py` & `chrislab-0.5.5/src/nlpbook/ner/corpus.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 from pathlib import Path
 from typing import List, Optional, ClassVar, Dict
 
 import torch
 from dataclasses_json import DataClassJsonMixin
 from torch.utils.data.dataset import Dataset
 
-from chrisbase.io import make_parent_dir, files, merge_dicts, out_hr
-from nlpbook.arguments import TesterArguments
+from chrisbase.io import make_parent_dir, files, merge_dicts, hr
+from nlpbook.arguments import TesterArguments, TrainerArguments
 from transformers import PreTrainedTokenizerFast, BatchEncoding, CharSpan
 from transformers.tokenization_utils_base import PaddingStrategy, TruncationStrategy
 
-logger = logging.getLogger("chrislab")
+logger = logging.getLogger(__name__)
 
 
 @dataclass
 class EntityInText(DataClassJsonMixin):
     pattern: ClassVar[re.Pattern] = re.compile('<([^<>]+?):([A-Z]{2,3})>')
     text: str
     label: str
@@ -53,43 +53,24 @@
 class NEREncodedExample:
     idx: int
     raw: NERRawExample
     encoded: BatchEncoding
     label_ids: Optional[List[int]] = None
 
 
-def ner_encoded_examples_to_batch(examples: List[NEREncodedExample]) -> Dict[str, torch.Tensor]:
-    first = examples[0]
-    batch = {}
-    for k, v in first.encoded.items():
-        if k not in ("label", "label_ids") and v is not None and not isinstance(v, str):
-            if isinstance(v, torch.Tensor):
-                batch[k] = torch.stack([ex.encoded[k] for ex in examples])
-            else:
-                batch[k] = torch.tensor([ex.encoded[k] for ex in examples], dtype=torch.long)
-    batch["labels"] = torch.tensor([ex.label_ids for ex in examples],
-                                   dtype=torch.long if type(first.label_ids[0]) is int else torch.float)
-    batch["example_ids"] = torch.tensor([ex.idx for ex in examples], dtype=torch.int)
-    return batch
-
-
 class NERCorpus:
-    def __init__(self, args: TesterArguments):
+    def __init__(self, args: TesterArguments | TrainerArguments):
         self.args = args
 
-    def read_raw_examples(self, data_path: Path) -> List[NERRawExample]:
-        examples = []
-        with data_path.open(encoding="utf-8") as inp:
-            for line in inp.readlines():
-                examples.append(NERRawExample.from_json(line))
-        logger.info(f"Loaded {len(examples)} examples from {data_path}")
-        return examples
+    @property
+    def num_labels(self) -> int:
+        return len(self.get_labels())
 
     def get_labels(self) -> List[str]:
-        label_map_path = make_parent_dir(self.args.output.dir_path / "label_map.txt")
+        label_map_path = make_parent_dir(self.args.env.output_home / "label_map.txt")
         if not label_map_path.exists():
             ner_tags = []
             train_data_path = self.args.data.home / self.args.data.name / self.args.data.files.train
             logger.info(f"Extracting labels from {train_data_path}")
             with train_data_path.open(encoding="utf-8") as inp:
                 for line in inp.readlines():
                     for x in NERRawExample.from_json(line).entity_list:
@@ -101,117 +82,127 @@
             logger.info(f"Saved {len(labels)} labels to {label_map_path}")
             with label_map_path.open("w", encoding="utf-8") as f:
                 f.writelines([x + "\n" for x in labels])
         else:
             labels = label_map_path.read_text(encoding="utf-8").splitlines()
         return labels
 
-    @property
-    def num_labels(self):
-        return len(self.get_labels())
+    def read_raw_examples(self, split: str) -> List[NERRawExample]:
+        assert self.args.data.home, f"No data_home: {self.args.data.home}"
+        assert self.args.data.name, f"No data_name: {self.args.data.name}"
+        data_file_dict: dict = self.args.data.files.to_dict()
+        assert split in data_file_dict, f"No '{split}' split in data_file: should be one of {list(data_file_dict.keys())}"
+        assert data_file_dict[split], f"No data_file for '{split}' split: {self.args.data.files}"
+        data_path: Path = Path(self.args.data.home) / self.args.data.name / data_file_dict[split]
+        assert data_path.exists() and data_path.is_file(), f"No data_text_path: {data_path}"
+        logger.info(f"Creating features from {data_path}")
 
+        examples = []
+        with data_path.open(encoding="utf-8") as inp:
+            for line in inp.readlines():
+                examples.append(NERRawExample.from_json(line))
+        logger.info(f"Loaded {len(examples)} examples from {data_path}")
+        return examples
 
-def _decide_span_label(span: CharSpan, offset_to_label: Dict[int, str]):
-    for x in [offset_to_label[i] for i in range(span.start, span.end)]:
-        if x.startswith("B-") or x.startswith("I-"):
-            return x
-    return "O"
-
-
-def _convert_to_encoded_examples(
-        raw_examples: List[NERRawExample],
-        tokenizer: PreTrainedTokenizerFast,
-        args: TesterArguments,
-        label_list: List[str],
-) -> List[NEREncodedExample]:
-    label_to_id: Dict[str, int] = {label: i for i, label in enumerate(label_list)}
-    id_to_label: Dict[int, str] = {i: label for i, label in enumerate(label_list)}
-    if args.env.off_debugging:
-        print(f"label_to_id = {label_to_id}")
-        print(f"id_to_label = {id_to_label}")
-
-    encoded_examples: List[NEREncodedExample] = []
-    for idx, raw_example in enumerate(raw_examples):
-        raw_example: NERRawExample = raw_example
-        offset_to_label: Dict[int, str] = raw_example.get_offset_label_dict()
-        if args.env.off_tracing:
-            out_hr()
-            print(f"offset_to_label = {offset_to_label}")
-        encoded: BatchEncoding = tokenizer.encode_plus(raw_example.origin,
-                                                       max_length=args.model.max_seq_length,
-                                                       truncation=TruncationStrategy.LONGEST_FIRST,
-                                                       padding=PaddingStrategy.MAX_LENGTH)
-        encoded_tokens: List[str] = encoded.tokens()
-        if args.env.off_debugging:
-            out_hr()
-            print(f"encoded.tokens()           = {encoded.tokens()}")
+    @staticmethod
+    def _decide_span_label(span: CharSpan, offset_to_label: Dict[int, str]):
+        for x in [offset_to_label[i] for i in range(span.start, span.end)]:
+            if x.startswith("B-") or x.startswith("I-"):
+                return x
+        return "O"
+
+    def raw_examples_to_encoded_examples(
+            self,
+            raw_examples: List[NERRawExample],
+            tokenizer: PreTrainedTokenizerFast,
+            label_list: List[str],
+    ) -> List[NEREncodedExample]:
+        label_to_id: Dict[str, int] = {label: i for i, label in enumerate(label_list)}
+        id_to_label: Dict[int, str] = {i: label for i, label in enumerate(label_list)}
+        logger.debug(f"label_to_id = {label_to_id}")
+        logger.debug(f"id_to_label = {id_to_label}")
+
+        encoded_examples: List[NEREncodedExample] = []
+        for idx, raw_example in enumerate(raw_examples):
+            raw_example: NERRawExample = raw_example
+            offset_to_label: Dict[int, str] = raw_example.get_offset_label_dict()
+            logger.debug(hr())
+            logger.debug(f"offset_to_label = {offset_to_label}")
+            encoded: BatchEncoding = tokenizer.encode_plus(raw_example.origin,
+                                                           max_length=self.args.model.seq_len,
+                                                           truncation=TruncationStrategy.LONGEST_FIRST,
+                                                           padding=PaddingStrategy.MAX_LENGTH)
+            encoded_tokens: List[str] = encoded.tokens()
+            logger.debug(hr())
+            logger.debug(f"encoded.tokens()           = {encoded.tokens()}")
             for key in encoded.keys():
-                print(f"encoded[{key:14s}]    = {encoded[key]}")
+                logger.debug(f"encoded[{key:14s}]    = {encoded[key]}")
 
-        if args.env.off_tracing:
-            out_hr()
-        label_list: List[str] = []
-        for token_id in range(args.model.max_seq_length):
-            token_repr: str = encoded_tokens[token_id]
-            token_span: CharSpan = encoded.token_to_chars(token_id)
-            if token_span:
-                token_label = _decide_span_label(token_span, offset_to_label)
-                label_list.append(token_label)
-                if args.env.off_tracing:
+            logger.debug(hr())
+            label_list: List[str] = []
+            for token_id in range(self.args.model.seq_len):
+                token_repr: str = encoded_tokens[token_id]
+                token_span: CharSpan = encoded.token_to_chars(token_id)
+                if token_span:
+                    token_label = self._decide_span_label(token_span, offset_to_label)
+                    label_list.append(token_label)
                     token_sstr = raw_example.origin[token_span.start:token_span.end]
-                    print('\t'.join(map(str, [token_id, token_repr, token_span, token_sstr, token_label])))
-            else:
-                label_list.append('O')
-                if args.env.off_tracing:
-                    print('\t'.join(map(str, [token_id, token_repr, token_span])))
-        label_ids: List[int] = [label_to_id[label] for label in label_list]
-        encoded_example = NEREncodedExample(idx=idx, raw=raw_example, encoded=encoded, label_ids=label_ids)
-        encoded_examples.append(encoded_example)
-        if args.env.off_debugging:
-            out_hr()
-            print(f"label_list                = {label_list}")
-            print(f"label_ids                 = {label_ids}")
-            out_hr()
-            print(f"encoded_example.idx       = {encoded_example.idx}")
-            print(f"encoded_example.raw       = {encoded_example.raw}")
-            print(f"encoded_example.encoded   = {encoded_example.encoded}")
-            print(f"encoded_example.label_ids = {encoded_example.label_ids}")
-
-    if args.env.off_debugging:
-        out_hr()
-    for encoded_example in encoded_examples[:args.data.show_examples]:
-        logger.info("  === [Example %d] ===" % encoded_example.idx)
-        logger.info("  = sentence   : %s" % encoded_example.raw.origin)
-        logger.info("  = characters : %s" % " | ".join(f"{x}/{y}" for x, y in encoded_example.raw.character_list))
-        logger.info("  = tokens     : %s" % " ".join(encoded_example.encoded.tokens()))
-        logger.info("  = labels     : %s" % " ".join([id_to_label[x] for x in encoded_example.label_ids]))
-        logger.info("  === ")
+                    logger.debug('\t'.join(map(str, [token_id, token_repr, token_span, token_sstr, token_label])))
+                else:
+                    label_list.append('O')
+                    logger.debug('\t'.join(map(str, [token_id, token_repr, token_span])))
+            label_ids: List[int] = [label_to_id[label] for label in label_list]
+            encoded_example = NEREncodedExample(idx=idx, raw=raw_example, encoded=encoded, label_ids=label_ids)
+            encoded_examples.append(encoded_example)
+            logger.debug(hr())
+            logger.debug(f"label_list                = {label_list}")
+            logger.debug(f"label_ids                 = {label_ids}")
+            logger.debug(hr())
+            logger.debug(f"encoded_example.idx       = {encoded_example.idx}")
+            logger.debug(f"encoded_example.raw       = {encoded_example.raw}")
+            logger.debug(f"encoded_example.encoded   = {encoded_example.encoded}")
+            logger.debug(f"encoded_example.label_ids = {encoded_example.label_ids}")
+
+        logger.info(hr())
+        for encoded_example in encoded_examples[:self.args.data.num_check]:
+            logger.info("  === [Example %d] ===" % encoded_example.idx)
+            logger.info("  = sentence   : %s" % encoded_example.raw.origin)
+            logger.info("  = characters : %s" % " | ".join(f"{x}/{y}" for x, y in encoded_example.raw.character_list))
+            logger.info("  = tokens     : %s" % " ".join(encoded_example.encoded.tokens()))
+            logger.info("  = labels     : %s" % " ".join([id_to_label[x] for x in encoded_example.label_ids]))
+            logger.info("  === ")
 
-    logger.info(f"Converted {len(raw_examples)} raw examples to {len(encoded_examples)} encoded examples")
-    return encoded_examples
+        logger.info(f"Converted {len(raw_examples)} raw examples to {len(encoded_examples)} encoded examples")
+        return encoded_examples
+
+    @staticmethod
+    def encoded_examples_to_batch(examples: List[NEREncodedExample]) -> Dict[str, torch.Tensor]:
+        first = examples[0]
+        batch = {}
+        for k, v in first.encoded.items():
+            if k not in ("label", "label_ids") and v is not None and not isinstance(v, str):
+                if isinstance(v, torch.Tensor):
+                    batch[k] = torch.stack([ex.encoded[k] for ex in examples])
+                else:
+                    batch[k] = torch.tensor([ex.encoded[k] for ex in examples], dtype=torch.long)
+        batch["labels"] = torch.tensor([ex.label_ids for ex in examples],
+                                       dtype=torch.long if type(first.label_ids[0]) is int else torch.float)
+        batch["example_ids"] = torch.tensor([ex.idx for ex in examples], dtype=torch.int)
+        return batch
 
 
 class NERDataset(Dataset):
-    def __init__(self, split: str, args: TesterArguments, tokenizer: PreTrainedTokenizerFast, corpus: NERCorpus):
-        assert corpus, "corpus is not valid"
-        assert args.data.home, f"No data_home: {args.data.home}"
-        assert args.data.name, f"No data_name: {args.data.name}"
+    def __init__(self, split: str, tokenizer: PreTrainedTokenizerFast, corpus: NERCorpus):
         self.corpus: NERCorpus = corpus
-        data_file_dict: dict = args.data.files.to_dict()
-        assert split in data_file_dict, f"No '{split}' split in data_file: should be one of {list(data_file_dict.keys())}"
-        assert data_file_dict[split], f"No data_file for '{split}' split: {args.data.files}"
-        text_data_path: Path = Path(args.data.home) / args.data.name / data_file_dict[split]
-        assert text_data_path.exists() and text_data_path.is_file(), f"No data_text_path: {text_data_path}"
-        logger.info(f"Creating features from dataset file at {text_data_path}")
-        examples: List[NERRawExample] = self.corpus.read_raw_examples(text_data_path)
+        examples: List[NERRawExample] = self.corpus.read_raw_examples(split)
         self.label_list: List[str] = self.corpus.get_labels()
         self._label_to_id: Dict[str, int] = {label: i for i, label in enumerate(self.label_list)}
         self._id_to_label: Dict[int, str] = {i: label for i, label in enumerate(self.label_list)}
-        self.features: List[NEREncodedExample] = \
-            _convert_to_encoded_examples(examples, tokenizer, args, label_list=self.label_list)
+        self.features: List[NEREncodedExample] = self.corpus.raw_examples_to_encoded_examples(
+            examples, tokenizer, label_list=self.label_list)
 
     def __len__(self) -> int:
         return len(self.features)
 
     def __getitem__(self, i) -> NEREncodedExample:
         return self.features[i]
 
@@ -221,85 +212,94 @@
     def label_to_id(self, label: str) -> int:
         return self._label_to_id[label]
 
     def id_to_label(self, label_id: int) -> str:
         return self._id_to_label[label_id]
 
 
-def parse_tagged(origin: str, tagged: str, debug: bool = False) -> Optional[NERRawExample]:
-    entity_list: List[EntityInText] = []
-    if debug:
-        print(f"* origin: {origin}")
-        print(f"  tagged: {tagged}")
-    restored = tagged[:]
-    no_problem = True
-    offset_labels = {i: "O" for i in range(len(origin))}
-    while True:
-        match: re.Match = EntityInText.pattern.search(restored)
-        if not match:
-            break
-        entity, restored = EntityInText.from_match(match, restored)
-        extracted = origin[entity.offset[0]:entity.offset[1]]
-        if entity.text == extracted:
-            entity_list.append(entity)
-            offset_labels = merge_dicts(offset_labels, entity.to_offset_lable_dict())
-        else:
-            no_problem = False
+class NERCorpusConverter:
+    @staticmethod
+    def parse_tagged(origin: str, tagged: str, debug: bool = False) -> Optional[NERRawExample]:
+        entity_list: List[EntityInText] = []
+        if debug:
+            print(f"* origin: {origin}")
+            print(f"  tagged: {tagged}")
+        restored = tagged[:]
+        no_problem = True
+        offset_labels = {i: "O" for i in range(len(origin))}
+        while True:
+            match: re.Match = EntityInText.pattern.search(restored)
+            if not match:
+                break
+            entity, restored = EntityInText.from_match(match, restored)
+            extracted = origin[entity.offset[0]:entity.offset[1]]
+            if entity.text == extracted:
+                entity_list.append(entity)
+                offset_labels = merge_dicts(offset_labels, entity.to_offset_lable_dict())
+            else:
+                no_problem = False
+            if debug:
+                print(f"  = {entity} -> {extracted}")
+                # print(f"    {offset_labels}")
         if debug:
-            print(f"  = {entity} -> {extracted}")
-            # print(f"    {offset_labels}")
-    if debug:
-        print(f"  --------------------")
-    character_list = [(origin[i], offset_labels[i]) for i in range(len(origin))]
-    if restored != origin:
-        no_problem = False
-    return NERRawExample(origin, entity_list, character_list) if no_problem else None
-
-
-def convert_kmou_format(infile: str | Path, outfile: str | Path, debug: bool = False):
-    with Path(infile).open(encoding="utf-8") as inp, Path(outfile).open("w", encoding="utf-8") as out:
-        for line in inp.readlines():
-            origin, tagged = line.strip().split("\u241E")
-            parsed: Optional[NERRawExample] = parse_tagged(origin, tagged, debug=debug)
-            if parsed:
-                out.write(parsed.to_json(ensure_ascii=False) + "\n")
-
-
-def convert_klue_format(infile: str | Path, outfile: str | Path, debug: bool = False):
-    with Path(infile) as inp, Path(outfile).open("w", encoding="utf-8") as out:
-        raw_text = inp.read_text(encoding="utf-8").strip()
-        raw_docs = re.split(r"\n\t?\n", raw_text)
-        for raw_doc in raw_docs:
-            raw_lines = raw_doc.splitlines()
-            num_header = 0
-            for line in raw_lines:
-                if not line.startswith("##"):
-                    break
-                num_header += 1
-            head_lines = raw_lines[:num_header]
-            body_lines = raw_lines[num_header:]
-
-            origin = ''.join(x.split("\t")[0] for x in body_lines)
-            tagged = head_lines[-1].split("\t")[1].strip()
-            parsed: Optional[NERRawExample] = parse_tagged(origin, tagged, debug=debug)
-            if parsed:
-                character_list_from_head = parsed.character_list
-                character_list_from_body = [tuple(x.split("\t")) for x in body_lines]
-                if character_list_from_head == character_list_from_body:
+            print(f"  --------------------")
+        character_list = [(origin[i], offset_labels[i]) for i in range(len(origin))]
+        if restored != origin:
+            no_problem = False
+        return NERRawExample(origin, entity_list, character_list) if no_problem else None
+
+    @classmethod
+    def convert_kmou_format(cls, infile: str | Path, outfile: str | Path, debug: bool = False):
+        with Path(infile).open(encoding="utf-8") as inp, Path(outfile).open("w", encoding="utf-8") as out:
+            for line in inp.readlines():
+                origin, tagged = line.strip().split("\u241E")
+                parsed: Optional[NERRawExample] = cls.parse_tagged(origin, tagged, debug=debug)
+                if parsed:
                     out.write(parsed.to_json(ensure_ascii=False) + "\n")
-                elif debug:
-                    print(f"* origin: {origin}")
-                    print(f"  tagged: {tagged}")
-                    for a, b in zip(character_list_from_head, character_list_from_body):
-                        if a != b:
-                            print(f"  = {a[0]}:{a[1]} <=> {b[0]}:{b[1]}")
-                    print(f"  ====================")
+
+    @classmethod
+    def convert_klue_format(cls, infile: str | Path, outfile: str | Path, debug: bool = False):
+        with Path(infile) as inp, Path(outfile).open("w", encoding="utf-8") as out:
+            raw_text = inp.read_text(encoding="utf-8").strip()
+            raw_docs = re.split(r"\n\t?\n", raw_text)
+            for raw_doc in raw_docs:
+                raw_lines = raw_doc.splitlines()
+                num_header = 0
+                for line in raw_lines:
+                    if not line.startswith("##"):
+                        break
+                    num_header += 1
+                head_lines = raw_lines[:num_header]
+                body_lines = raw_lines[num_header:]
+
+                origin = ''.join(x.split("\t")[0] for x in body_lines)
+                tagged = head_lines[-1].split("\t")[1].strip()
+                parsed: Optional[NERRawExample] = cls.parse_tagged(origin, tagged, debug=debug)
+                if parsed:
+                    character_list_from_head = parsed.character_list
+                    character_list_from_body = [tuple(x.split("\t")) for x in body_lines]
+                    if character_list_from_head == character_list_from_body:
+                        out.write(parsed.to_json(ensure_ascii=False) + "\n")
+                    elif debug:
+                        print(f"* origin: {origin}")
+                        print(f"  tagged: {tagged}")
+                        for a, b in zip(character_list_from_head, character_list_from_body):
+                            if a != b:
+                                print(f"  = {a[0]}:{a[1]} <=> {b[0]}:{b[1]}")
+                        print(f"  ====================")
 
 
 if __name__ == "__main__":
-    for path in files("data/kmou-ner-full/*.txt"):
-        print(f"[FILE]: {path}")
-        convert_kmou_format(path, path.with_suffix(".jsonl"), debug=True)
-
-    # for path in files("data/klue-ner/*.tsv"):
-    #     print(f"[FILE]: {path}")
-    #     convert_klue_format(path, path.with_suffix(".jsonl"), debug=True)
+    class RunOption:
+        run1: bool = True
+        run2: bool = False
+
+
+    if RunOption.run1:
+        for path in files("data/kmou-ner-full/*.txt"):
+            print(f"[FILE]: {path}")
+            NERCorpusConverter.convert_kmou_format(path, path.with_suffix(".jsonl"), debug=True)
+
+    if RunOption.run2:
+        for path in files("data/klue-ner/*.tsv"):
+            print(f"[FILE]: {path}")
+            NERCorpusConverter.convert_klue_format(path, path.with_suffix(".jsonl"), debug=True)
```

### Comparing `chrislab-0.5.4/src/nlpbook/ner/task.py` & `chrislab-0.5.5/src/nlpbook/ner/task.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,44 @@
+import logging
 from typing import List, Dict, Tuple
 
 import torch
+from pytorch_lightning import LightningModule, Trainer
 from torch.optim import AdamW
 from torch.optim.lr_scheduler import ExponentialLR
+from transformers import PreTrainedModel, CharSpan
+from transformers.modeling_outputs import TokenClassifierOutput
 
-import lightning.pytorch as pl
-from chrisbase.io import out_hr
-from lightning.pytorch import LightningModule
+from chrisbase.io import hr
 from nlpbook.arguments import TesterArguments, TrainerArguments
 from nlpbook.metrics import accuracy, klue_ner_char_macro_f1, klue_ner_entity_macro_f1
 from nlpbook.ner import NERDataset, NEREncodedExample
-from transformers import PreTrainedModel, CharSpan
-from transformers.modeling_outputs import TokenClassifierOutput
+
+logger = logging.getLogger(__name__)
 
 
 def label_to_char_labels(label, num_char):
     for i in range(num_char):
         if i > 0 and ("-" in label):
             yield "I-" + label.split("-", maxsplit=1)[-1]
         else:
             yield label
 
 
 class NERTask(LightningModule):
-    def __init__(self, model: PreTrainedModel,
+    def __init__(self,
                  args: TesterArguments | TrainerArguments,
-                 trainer: pl.Trainer,
+                 model: PreTrainedModel,
+                 trainer: Trainer,
                  val_dataset: NERDataset,
-                 total_steps: int,
-                 ):
+                 total_steps: int):
         super().__init__()
         self.model: PreTrainedModel = model
         self.args: TesterArguments | TrainerArguments = args
-        self.trainer: pl.Trainer = trainer
+        self.trainer: Trainer = trainer
 
         self.val_dataset: NERDataset = val_dataset
         self._validation_char_pred_ids = None
         self._validation_char_label_ids = None
 
         self._labels: List[str] = self.val_dataset.get_labels()
         self._label_to_id: Dict[str, int] = {label: i for i, label in enumerate(self._labels)}
@@ -58,15 +60,15 @@
     def _global_step(self):
         return self.trainer.lightning_module.global_step
 
     def _trained_rate(self):
         return self.trainer.lightning_module.global_step / self.total_steps
 
     def configure_optimizers(self):
-        optimizer = AdamW(self.parameters(), lr=self.args.learning.speed)
+        optimizer = AdamW(self.parameters(), lr=self.args.learning.lr)
         scheduler = ExponentialLR(optimizer, gamma=0.9)
         return {
             'optimizer': optimizer,
             'lr_scheduler': scheduler,
         }
 
     def training_step(self, batch: Dict[str, torch.Tensor], batch_idx: int) -> torch.Tensor:
@@ -76,101 +78,98 @@
         preds: torch.Tensor = outputs.logits.argmax(dim=-1)
         acc: torch.Tensor = accuracy(preds, labels, ignore_index=0)
         self.train_loss = outputs.loss
         self.train_acc = acc
         return outputs.loss
 
     def validation_step(self, batch: Dict[str, torch.Tensor], batch_idx: int) -> torch.Tensor:
-        if self.args.env.on_debugging:
-            print()
-            print(f"[validation_step] batch_idx: {batch_idx}, global_step: {self._global_step()}")
-            for key in batch.keys():
-                if isinstance(batch[key], torch.Tensor):
-                    print(f"  - batch[{key:14s}]     = {batch[key].shape} | {batch[key].tolist()}")
-                else:
-                    print(f"  - batch[{key:14s}]     = ({len(batch[key])}) | {batch[key]}")
+        logger.debug('')
+        logger.debug(f"[validation_step] batch_idx: {batch_idx}, global_step: {self._global_step()}")
+        for key in batch.keys():
+            if isinstance(batch[key], torch.Tensor):
+                logger.debug(f"  - batch[{key:14s}]     = {batch[key].shape} | {batch[key].tolist()}")
+            else:
+                logger.debug(f"  - batch[{key:14s}]     = ({len(batch[key])}) | {batch[key]}")
         example_ids: List[int] = batch.pop("example_ids").tolist()
         outputs: TokenClassifierOutput = self.model(**batch)
         labels: torch.Tensor = batch["labels"]
         preds: torch.Tensor = outputs.logits.argmax(dim=-1)
         acc: torch.Tensor = accuracy(preds, labels, ignore_index=0)
 
-        self.log(prog_bar=True, logger=False, on_epoch=True, name="global_step", value=self._global_step() * 1.0)
-        self.log(prog_bar=True, logger=False, on_epoch=True, name="trained_rate", value=self._trained_rate())
-        self.log(prog_bar=True, logger=False, on_epoch=True, name="train_loss", value=self.train_loss)
-        self.log(prog_bar=True, logger=False, on_epoch=True, name="train_acc", value=self.train_acc)
-        self.log(prog_bar=True, logger=False, on_epoch=True, name="val_loss", value=outputs.loss)
-        self.log(prog_bar=True, logger=False, on_epoch=True, name="val_acc", value=acc)
+        self.log(sync_dist=True, prog_bar=True, logger=False, on_epoch=True, name="global_step", value=self._global_step() * 1.0)
+        self.log(sync_dist=True, prog_bar=True, logger=False, on_epoch=True, name="trained_rate", value=self._trained_rate())
+        self.log(sync_dist=True, prog_bar=True, logger=False, on_epoch=True, name="train_loss", value=self.train_loss)
+        self.log(sync_dist=True, prog_bar=True, logger=False, on_epoch=True, name="train_acc", value=self.train_acc)
+        self.log(sync_dist=True, prog_bar=True, logger=False, on_epoch=True, name="val_loss", value=outputs.loss)
+        self.log(sync_dist=True, prog_bar=True, logger=False, on_epoch=True, name="val_acc", value=acc)
 
         dict_of_token_pred_ids: Dict[int, List[int]] = {}
         dict_of_char_label_ids: Dict[int, List[int]] = {}
         dict_of_char_pred_ids: Dict[int, List[int]] = {}
         for token_pred_ids, example_id in zip(preds.tolist(), example_ids):
             token_pred_tags: List[str] = [self.id_to_label(x) for x in token_pred_ids]
             encoded_example: NEREncodedExample = self.val_dataset[example_id]
             offset_to_label: Dict[int, str] = encoded_example.raw.get_offset_label_dict()
             all_char_pair_tags: List[Tuple[str | None, str | None]] = [(None, None)] * len(encoded_example.raw.character_list)
-            for token_id in range(self.args.model.max_seq_length):
+            for token_id in range(self.args.model.seq_len):
                 token_span: CharSpan = encoded_example.encoded.token_to_chars(token_id)
                 if token_span:
                     char_pred_tags = label_to_char_labels(token_pred_tags[token_id], token_span.end - token_span.start)
                     for offset, char_pred_tag in zip(range(token_span.start, token_span.end), char_pred_tags):
                         all_char_pair_tags[offset] = (offset_to_label[offset], char_pred_tag)
             valid_char_pair_tags = [(a, b) for a, b in all_char_pair_tags if a and b]
             valid_char_label_ids = [self.label_to_id(a) for a, b in valid_char_pair_tags]
             valid_char_pred_ids = [self.label_to_id(b) for a, b in valid_char_pair_tags]
             dict_of_token_pred_ids[example_id] = token_pred_ids
             dict_of_char_label_ids[example_id] = valid_char_label_ids
             dict_of_char_pred_ids[example_id] = valid_char_pred_ids
 
-        if self.args.env.on_tracing:
-            out_hr()
+        logger.debug(hr())
         flatlist_of_char_pred_ids: List[int] = []
         flatlist_of_char_label_ids: List[int] = []
         for encoded_example in [self.val_dataset[i] for i in example_ids]:
             token_pred_ids = dict_of_token_pred_ids[encoded_example.idx]
             char_label_ids = dict_of_char_label_ids[encoded_example.idx]
             char_pred_ids = dict_of_char_pred_ids[encoded_example.idx]
             flatlist_of_char_pred_ids.extend(char_pred_ids)
             flatlist_of_char_label_ids.extend(char_label_ids)
-            if self.args.env.on_tracing:
-                print(f"  - encoded_example.idx                = {encoded_example.idx}")
-                print(f"  - encoded_example.raw.entity_list    = ({len(encoded_example.raw.entity_list)}) {encoded_example.raw.entity_list}")
-                print(f"  - encoded_example.raw.origin         = ({len(encoded_example.raw.origin)}) {encoded_example.raw.origin}")
-                print(f"  - encoded_example.raw.character_list = ({len(encoded_example.raw.character_list)}) {' | '.join(f'{x}/{y}' for x, y in encoded_example.raw.character_list)}")
-                print(f"  - encoded_example.encoded.tokens()   = ({len(encoded_example.encoded.tokens())}) {' '.join(encoded_example.encoded.tokens())}")
-                current_repr = lambda x: f"{self.id_to_label(x):5s}"
-                print(f"  - encoded_example.label_ids          = ({len(encoded_example.label_ids)}) {' '.join(map(str, map(current_repr, encoded_example.label_ids)))}")
-                print(f"  - encoded_example.token_pred_ids     = ({len(token_pred_ids)}) {' '.join(map(str, map(current_repr, token_pred_ids)))}")
-                print(f"  - encoded_example.char_label_ids     = ({len(char_label_ids)}) {' '.join(map(str, map(current_repr, char_label_ids)))}")
-                print(f"  - encoded_example.char_pred_ids      = ({len(char_pred_ids)}) {' '.join(map(str, map(current_repr, char_pred_ids)))}")
-                out_hr('-')
-
-        if self.args.env.on_debugging:
-            current_repr = lambda x: f"{x:02d}"
-            print(f"  - flatlist_of_char_label_ids = ({len(flatlist_of_char_label_ids)}) {' '.join(map(str, map(current_repr, flatlist_of_char_label_ids)))}")
-            print(f"  - flatlist_of_char_pred_ids  = ({len(flatlist_of_char_pred_ids)}) {' '.join(map(str, map(current_repr, flatlist_of_char_pred_ids)))}")
+
+            logger.debug(f"  - encoded_example.idx                = {encoded_example.idx}")
+            logger.debug(f"  - encoded_example.raw.entity_list    = ({len(encoded_example.raw.entity_list)}) {encoded_example.raw.entity_list}")
+            logger.debug(f"  - encoded_example.raw.origin         = ({len(encoded_example.raw.origin)}) {encoded_example.raw.origin}")
+            logger.debug(f"  - encoded_example.raw.character_list = ({len(encoded_example.raw.character_list)}) {' | '.join(f'{x}/{y}' for x, y in encoded_example.raw.character_list)}")
+            logger.debug(f"  - encoded_example.encoded.tokens()   = ({len(encoded_example.encoded.tokens())}) {' '.join(encoded_example.encoded.tokens())}")
+            current_repr = lambda x: f"{self.id_to_label(x):5s}"
+            logger.debug(f"  - encoded_example.label_ids          = ({len(encoded_example.label_ids)}) {' '.join(map(str, map(current_repr, encoded_example.label_ids)))}")
+            logger.debug(f"  - encoded_example.token_pred_ids     = ({len(token_pred_ids)}) {' '.join(map(str, map(current_repr, token_pred_ids)))}")
+            logger.debug(f"  - encoded_example.char_label_ids     = ({len(char_label_ids)}) {' '.join(map(str, map(current_repr, char_label_ids)))}")
+            logger.debug(f"  - encoded_example.char_pred_ids      = ({len(char_pred_ids)}) {' '.join(map(str, map(current_repr, char_pred_ids)))}")
+            logger.debug(hr('-'))
+
+        current_repr = lambda x: f"{x:02d}"
+        logger.debug(f"  - flatlist_of_char_label_ids = ({len(flatlist_of_char_label_ids)}) {' '.join(map(str, map(current_repr, flatlist_of_char_label_ids)))}")
+        logger.debug(f"  - flatlist_of_char_pred_ids  = ({len(flatlist_of_char_pred_ids)}) {' '.join(map(str, map(current_repr, flatlist_of_char_pred_ids)))}")
         assert len(flatlist_of_char_label_ids) == len(flatlist_of_char_pred_ids)
         self._validation_char_pred_ids.extend(flatlist_of_char_pred_ids)
         self._validation_char_label_ids.extend(flatlist_of_char_label_ids)
         return outputs.loss
 
     def on_validation_start(self):
         self._validation_char_pred_ids: List[int] = []
         self._validation_char_label_ids: List[int] = []
 
     def on_validation_epoch_end(self):
         assert self._validation_char_pred_ids and self._validation_char_label_ids
         assert len(self._validation_char_pred_ids) == len(self._validation_char_label_ids)
         chr_f1 = klue_ner_char_macro_f1(preds=self._validation_char_pred_ids, labels=self._validation_char_label_ids, label_list=self._labels)
         ent_f1 = klue_ner_entity_macro_f1(preds=self._validation_char_pred_ids, labels=self._validation_char_label_ids, label_list=self._labels)
-        self.log(prog_bar=True, logger=True, on_epoch=True, name="val_F1c", value=chr_f1)
-        self.log(prog_bar=True, logger=True, on_epoch=True, name="val_F1e", value=ent_f1)
+        self.log(sync_dist=True, prog_bar=True, logger=True, on_epoch=True, name="val_F1c", value=chr_f1)
+        self.log(sync_dist=True, prog_bar=True, logger=True, on_epoch=True, name="val_F1e", value=ent_f1)
 
     def test_step(self, batch, batch_idx) -> torch.Tensor:
         outputs: TokenClassifierOutput = self.model(**batch)
         labels: torch.Tensor = batch["labels"]
         preds: torch.Tensor = outputs.logits.argmax(dim=-1)
         acc: torch.Tensor = accuracy(preds, labels, ignore_index=0)
-        self.log(prog_bar=False, logger=True, on_epoch=True, name="test_loss", value=outputs.loss)
-        self.log(prog_bar=False, logger=True, on_epoch=True, name="test_acc", value=acc)
+        self.log(sync_dist=True, prog_bar=False, logger=True, on_epoch=True, name="test_loss", value=outputs.loss)
+        self.log(sync_dist=True, prog_bar=False, logger=True, on_epoch=True, name="test_acc", value=acc)
         return outputs.loss
```

### Comparing `chrislab-0.5.4/src/nlpbook/paircls/corpus.py` & `chrislab-0.5.5/src/nlpbook/paircls/corpus.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import os
 import json
 import logging
-from nlpbook.cls.corpus import ClassificationExample
+import os
 
+from nlpbook.cls.corpus import ClassificationExample
 
-logger = logging.getLogger("chrislab")
+logger = logging.getLogger(__name__)
 
 
 class KlueNLICorpus:
 
     def __init__(self):
         pass
 
@@ -37,15 +37,14 @@
         return ["entailment", "contradiction", "neutral"]
 
     @property
     def num_labels(self):
         return len(self.get_labels())
 
 
-
 class KorNLICorpus:
 
     def __init__(self):
         pass
 
     def _create_examples(self, data_path):
         examples = []
```

### Comparing `chrislab-0.5.4/src/nlpbook/paircls/deploy.py` & `chrislab-0.5.5/src/nlpbook/paircls/deploy.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.4/src/nlpbook/qa/arguments.py` & `chrislab-0.5.5/src/nlpbook/qa/arguments.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.4/src/nlpbook/qa/corpus.py` & `chrislab-0.5.5/src/nlpbook/qa/corpus.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 from multiprocessing import Pool, cpu_count
 from typing import List, Optional
 
 import torch
 from filelock import FileLock
 from torch.utils.data.dataset import Dataset
 from tqdm import tqdm
+from transformers import PreTrainedTokenizer
 
 from nlpbook.qa import QATrainArguments
-from transformers import PreTrainedTokenizer
 
-logger = logging.getLogger("chrislab")
+logger = logging.getLogger(__name__)
 
 
 @dataclass
 class QAExample:
     # 질문 : 임종석이 여의도 농민 폭력 시위를 주도한 혐의로 지명수배 된 날은?
     question_text: str
     # (답 찾는 대상인)지문 : 1989년 2월 15일 여의도 농민 폭력 시위를 주도한 혐의 ... 서울지방경찰청 공안분실로 인계되었다.
@@ -373,15 +373,15 @@
                     f"Loading features from cached file {cached_features_file} [took %.3f s]", time.time() - start
                 )
             else:
                 corpus_fpath = os.path.join(
                     args.downstream_corpus_root_dir,
                     args.downstream_corpus_name.lower(),
                 )
-                logger.info(f"Creating features from {mode} dataset file at {corpus_fpath}")
+                logger.info(f"Creating features from {corpus_fpath}")
                 examples = self.corpus.get_examples(corpus_fpath, mode)
                 self.features = convert_examples_to_features_fn(examples, tokenizer, args)
                 start = time.time()
                 logger.info(
                     "Saving features into cached file, it could take a lot of time..."
                 )
                 torch.save(self.features, cached_features_file)
```

### Comparing `chrislab-0.5.4/src/nlpbook/qa/deploy.py` & `chrislab-0.5.5/src/nlpbook/qa/deploy.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.4/src/nlpbook/qa/task.py` & `chrislab-0.5.5/src/nlpbook/qa/task.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-from lightning.pytorch import LightningModule
-from nlpbook.metrics import accuracy
-from nlpbook.qa import QATrainArguments
+from pytorch_lightning import LightningModule
 from torch.optim import AdamW
 from torch.optim.lr_scheduler import ExponentialLR
 from transformers import PreTrainedModel
 
+from nlpbook.metrics import accuracy
+from nlpbook.qa import QATrainArguments
+
 
 class QATask(LightningModule):
 
     def __init__(self,
                  model: PreTrainedModel,
                  args: QATrainArguments,
                  ):
```

### Comparing `chrislab-0.5.4/src/nlpbook/utils.py` & `chrislab-0.5.5/src/nlpbook/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 from pathlib import Path
 from typing import List, Tuple
 
 import requests
 import tqdm
 from transformers import HfArgumentParser
 
-from chrisbase.io import sys_stdout
 from .arguments import TrainerArguments, TesterArguments
 
+logger = logging.getLogger(__name__)
+
 REMOTE_DATA_MAP = {
     "nsmc": {
         "train": {
             "web_url": "https://github.com/e9t/nsmc/raw/master/ratings_train.txt",
             "fname": "train.txt",
         },
         "val": {
@@ -72,15 +73,14 @@
         "config": {
             "googledrive_file_id": "1z6obNRWPHoVrMzT9THElblebdovuDLUZ",
             "fname": "config.json",
         },
     },
 }
 GOOGLE_DRIVE_URL = "https://docs.google.com/uc?export=download"
-logger = logging.getLogger("chrislab")
 TERM_IN_NAME_FORMAT = re.compile(re.escape("{") + "(.+?)(:.+?)?" + re.escape("}"))
 
 
 def save_response_content(response, save_path):
     with open(save_path, "wb") as f:
         content_length = response.headers.get("Content-Length")
         total = int(content_length) if content_length is not None else None
@@ -212,46 +212,22 @@
                         save_fname=value["fname"],
                         cache_dir=args.pretrained_model_cache_dir,
                     )
     else:
         raise ValueError(f"not valid model name({pretrained_model_name}), cannot download resources")
 
 
-def set_seed(args: TrainerArguments):
+def set_seed(args: TrainerArguments):  # TODO: Remove someday
     if args.learning.seed is not None:
         from transformers import set_seed
         set_seed(args.learning.seed)
-        from lightning.pytorch import seed_everything
+        from pytorch_lightning import seed_everything
         seed_everything(args.learning.seed)
     else:
-        print("not fixed seed", file=sys.stderr)
-
-
-def new_logger(name="chrislab", stream=sys_stdout, level=logging.INFO, fmt="%(levelname)s\t%(name)s\t%(message)s") -> logging.Logger:
-    stream_handler = logging.StreamHandler(stream=stream)
-    stream_handler.setFormatter(logging.Formatter(fmt=fmt))
-    new_logger = logging.getLogger(name)
-    new_logger.addHandler(stream_handler)
-    new_logger.setLevel(level)
-    return new_logger
-
-
-def new_logger_file(name="chrislab", filepath="running.log", filemode="a",
-                    stream=sys_stdout, level=logging.INFO, fmt="%(levelname)s\t%(name)s\t%(message)s") -> logging.Logger:
-    stream_handler = logging.StreamHandler(stream=stream)
-    file_handler = logging.FileHandler(filename=filepath, mode=filemode, encoding="utf-8")
-
-    stream_handler.setFormatter(logging.Formatter(fmt=fmt))
-    file_handler.setFormatter(logging.Formatter(fmt=fmt))
-
-    new_logger = logging.getLogger(name)
-    new_logger.addHandler(stream_handler)
-    new_logger.addHandler(file_handler)
-    new_logger.setLevel(level)
-    return new_logger
+        logger.warning("not fixed seed")
 
 
 def load_arguments(argument_class, json_file_path=None):
     parser = HfArgumentParser(argument_class)
     if json_file_path is not None:
         args, = parser.parse_json_file(json_file=json_file_path)
     elif len(sys.argv) == 2 and sys.argv[1].endswith(".json"):
@@ -261,22 +237,22 @@
     return args
 
 
 # https://lightning.ai/docs/fabric/stable/guide/checkpoint.html
 def save_checkpoint(fabric, args, metric_values, model, optimizer,
                     sorted_checkpoints: List[Tuple[float, Path]], sorting_reverse, sorting_metric):
     checkpoint_state = {"model": model, "optimizer": optimizer, "args": args}
-    terms = [m.group(1) for m in TERM_IN_NAME_FORMAT.finditer(args.model.finetuning_name)]
+    terms = [m.group(1) for m in TERM_IN_NAME_FORMAT.finditer(args.model.name)]
     terms = {term: metric_values[term] for term in terms}
-    checkpoint_stem = args.model.finetuning_name.format(**terms)
-    checkpoint_path: Path = (args.output.dir_path / "model.out").with_stem(checkpoint_stem).with_suffix(".ckpt")
+    checkpoint_stem = args.model.name.format(**terms)
+    checkpoint_path: Path = (args.env.output_home / "model.out").with_stem(checkpoint_stem).with_suffix(".ckpt")
 
     sorted_checkpoints.append((metric_values[sorting_metric], checkpoint_path))
     sorted_checkpoints.sort(key=lambda x: x[0], reverse=sorting_reverse)
-    for _, path in sorted_checkpoints[args.learning.num_keeping:]:
+    for _, path in sorted_checkpoints[args.learning.num_save:]:
         path.unlink(missing_ok=True)
-    sorted_checkpoints = [(value, path) for value, path in sorted_checkpoints[:args.learning.num_keeping] if path.exists()]
-    if len(sorted_checkpoints) < args.learning.num_keeping:
+    sorted_checkpoints = [(value, path) for value, path in sorted_checkpoints[:args.learning.num_save] if path.exists()]
+    if len(sorted_checkpoints) < args.learning.num_save:
         fabric.save(checkpoint_path, checkpoint_state)
         sorted_checkpoints.append((metric_values[sorting_metric], checkpoint_path))
         sorted_checkpoints.sort(key=lambda x: x[0], reverse=sorting_reverse)
     return sorted_checkpoints
```

