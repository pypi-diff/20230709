# Comparing `tmp/pypdfe-0.1.7.tar.gz` & `tmp/pypdfe-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypdfe-0.1.7.tar", last modified: Sun Jul  9 01:33:00 2023, max compression
+gzip compressed data, was "pypdfe-0.1.8.tar", last modified: Sun Jul  9 17:58:32 2023, max compression
```

## Comparing `pypdfe-0.1.7.tar` & `pypdfe-0.1.8.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-09 01:33:00.585834 pypdfe-0.1.7/
--rw-r--r--   0 nate       (501) staff       (20)    35148 2023-07-08 07:31:18.000000 pypdfe-0.1.7/LICENSE
--rw-r--r--   0 nate       (501) staff       (20)        9 2023-07-09 01:32:49.000000 pypdfe-0.1.7/MANIFEST.in
--rw-r--r--   0 nate       (501) staff       (20)      297 2023-07-09 01:33:00.585729 pypdfe-0.1.7/PKG-INFO
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-09 01:33:00.577352 pypdfe-0.1.7/pypdfe/
--rw-r--r--   0 nate       (501) staff       (20)     1025 2023-07-08 07:18:43.000000 pypdfe-0.1.7/pypdfe/__init__.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-09 01:33:00.578117 pypdfe-0.1.7/pypdfe.egg-info/
--rw-r--r--   0 nate       (501) staff       (20)      297 2023-07-09 01:33:00.000000 pypdfe-0.1.7/pypdfe.egg-info/PKG-INFO
--rw-r--r--   0 nate       (501) staff       (20)     2354 2023-07-09 01:33:00.000000 pypdfe-0.1.7/pypdfe.egg-info/SOURCES.txt
--rw-r--r--   0 nate       (501) staff       (20)        1 2023-07-09 01:33:00.000000 pypdfe-0.1.7/pypdfe.egg-info/dependency_links.txt
--rw-r--r--   0 nate       (501) staff       (20)        1 2023-07-09 01:33:00.000000 pypdfe-0.1.7/pypdfe.egg-info/not-zip-safe
--rw-r--r--   0 nate       (501) staff       (20)        6 2023-07-09 01:33:00.000000 pypdfe-0.1.7/pypdfe.egg-info/requires.txt
--rw-r--r--   0 nate       (501) staff       (20)        7 2023-07-09 01:33:00.000000 pypdfe-0.1.7/pypdfe.egg-info/top_level.txt
--rw-r--r--   0 nate       (501) staff       (20)      909 2023-07-09 01:32:49.000000 pypdfe-0.1.7/pyproject.toml
--rw-r--r--   0 nate       (501) staff       (20)       38 2023-07-09 01:33:00.585871 pypdfe-0.1.7/setup.cfg
--rw-r--r--   0 nate       (501) staff       (20)     1324 2023-07-09 01:32:49.000000 pypdfe-0.1.7/setup.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-09 01:33:00.578344 pypdfe-0.1.7/src/
--rw-r--r--   0 nate       (501) staff       (20)     8196 2023-07-09 01:32:13.000000 pypdfe-0.1.7/src/.DS_Store
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-09 01:33:00.582111 pypdfe-0.1.7/src/PDF-Estimator/
--rw-r--r--   0 nate       (501) staff       (20)     8196 2023-07-09 01:17:14.000000 pypdfe-0.1.7/src/PDF-Estimator/.DS_Store
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-09 01:33:00.582868 pypdfe-0.1.7/src/PDF-Estimator/.git/
--rw-r--r--   0 nate       (501) staff       (20)      103 2023-06-21 22:03:26.000000 pypdfe-0.1.7/src/PDF-Estimator/.git/FETCH_HEAD
--rw-r--r--   0 nate       (501) staff       (20)       21 2023-06-21 20:32:32.000000 pypdfe-0.1.7/src/PDF-Estimator/.git/HEAD
--rw-r--r--   0 nate       (501) staff       (20)      309 2023-06-21 20:32:32.000000 pypdfe-0.1.7/src/PDF-Estimator/.git/config
--rw-r--r--   0 nate       (501) staff       (20)       73 2023-06-21 20:32:31.000000 pypdfe-0.1.7/src/PDF-Estimator/.git/description
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-09 01:33:00.584570 pypdfe-0.1.7/src/PDF-Estimator/.git/hooks/
--rwxr-xr-x   0 nate       (501) staff       (20)      478 2023-06-21 20:32:31.000000 pypdfe-0.1.7/src/PDF-Estimator/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0 nate       (501) staff       (20)      896 2023-06-21 20:32:31.000000 pypdfe-0.1.7/src/PDF-Estimator/.git/hooks/commit-msg.sample
--rwxr-xr-x   0 nate       (501) staff       (20)     4726 2023-06-21 20:32:31.000000 pypdfe-0.1.7/src/PDF-Estimator/.git/hooks/fsmonitor-watchman.sample
--rwxr-xr-x   0 nate       (501) staff       (20)      189 2023-06-21 20:32:31.000000 pypdfe-0.1.7/src/PDF-Estimator/.git/hooks/post-update.sample
--rwxr-xr-x   0 nate       (501) staff       (20)      424 2023-06-21 20:32:31.000000 pypdfe-0.1.7/src/PDF-Estimator/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0 nate       (501) staff       (20)     1643 2023-06-21 20:32:31.000000 pypdfe-0.1.7/src/PDF-Estimator/.git/hooks/pre-commit.sample
--rwxr-xr-x   0 nate       (501) staff       (20)      416 2023-06-21 20:32:31.000000 pypdfe-0.1.7/src/PDF-Estimator/.git/hooks/pre-merge-commit.sample
--rwxr-xr-x   0 nate       (501) staff       (20)     1374 2023-06-21 20:32:31.000000 pypdfe-0.1.7/src/PDF-Estimator/.git/hooks/pre-push.sample
--rwxr-xr-x   0 nate       (501) staff       (20)     4898 2023-06-21 20:32:31.000000 pypdfe-0.1.7/src/PDF-Estimator/.git/hooks/pre-rebase.sample
--rwxr-xr-x   0 nate       (501) staff       (20)      544 2023-06-21 20:32:31.000000 pypdfe-0.1.7/src/PDF-Estimator/.git/hooks/pre-receive.sample
--rwxr-xr-x   0 nate       (501) staff       (20)     1492 2023-06-21 20:32:31.000000 pypdfe-0.1.7/src/PDF-Estimator/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0 nate       (501) staff       (20)     2783 2023-06-21 20:32:31.000000 pypdfe-0.1.7/src/PDF-Estimator/.git/hooks/push-to-checkout.sample
--rwxr-xr-x   0 nate       (501) staff       (20)     3650 2023-06-21 20:32:31.000000 pypdfe-0.1.7/src/PDF-Estimator/.git/hooks/update.sample
--rw-r--r--   0 nate       (501) staff       (20)     2102 2023-06-22 03:25:25.000000 pypdfe-0.1.7/src/PDF-Estimator/.git/index
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-09 01:33:00.584700 pypdfe-0.1.7/src/PDF-Estimator/.git/info/
--rw-r--r--   0 nate       (501) staff       (20)      240 2023-06-21 20:32:31.000000 pypdfe-0.1.7/src/PDF-Estimator/.git/info/exclude
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-09 01:33:00.584829 pypdfe-0.1.7/src/PDF-Estimator/.git/logs/
--rw-r--r--   0 nate       (501) staff       (20)      213 2023-06-21 20:32:32.000000 pypdfe-0.1.7/src/PDF-Estimator/.git/logs/HEAD
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-09 01:33:00.576179 pypdfe-0.1.7/src/PDF-Estimator/.git/logs/refs/
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-09 01:33:00.584946 pypdfe-0.1.7/src/PDF-Estimator/.git/logs/refs/heads/
--rw-r--r--   0 nate       (501) staff       (20)      213 2023-06-21 20:32:32.000000 pypdfe-0.1.7/src/PDF-Estimator/.git/logs/refs/heads/main
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-09 01:33:00.576232 pypdfe-0.1.7/src/PDF-Estimator/.git/logs/refs/remotes/
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-09 01:33:00.585053 pypdfe-0.1.7/src/PDF-Estimator/.git/logs/refs/remotes/origin/
--rw-r--r--   0 nate       (501) staff       (20)      213 2023-06-21 20:32:32.000000 pypdfe-0.1.7/src/PDF-Estimator/.git/logs/refs/remotes/origin/HEAD
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-09 01:33:00.576389 pypdfe-0.1.7/src/PDF-Estimator/.git/objects/
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-09 01:33:00.585297 pypdfe-0.1.7/src/PDF-Estimator/.git/objects/pack/
--r--r--r--   0 nate       (501) staff       (20)     1996 2023-06-21 20:32:32.000000 pypdfe-0.1.7/src/PDF-Estimator/.git/objects/pack/pack-68fcf6d5b1d91b28c20241431b9241a5762ddad3.idx
--r--r--r--   0 nate       (501) staff       (20)    47733 2023-06-21 20:32:32.000000 pypdfe-0.1.7/src/PDF-Estimator/.git/objects/pack/pack-68fcf6d5b1d91b28c20241431b9241a5762ddad3.pack
--rw-r--r--   0 nate       (501) staff       (20)      112 2023-06-21 20:32:32.000000 pypdfe-0.1.7/src/PDF-Estimator/.git/packed-refs
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-09 01:33:00.576629 pypdfe-0.1.7/src/PDF-Estimator/.git/refs/
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-09 01:33:00.585446 pypdfe-0.1.7/src/PDF-Estimator/.git/refs/heads/
--rw-r--r--   0 nate       (501) staff       (20)       41 2023-06-21 20:32:32.000000 pypdfe-0.1.7/src/PDF-Estimator/.git/refs/heads/main
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-09 01:33:00.576679 pypdfe-0.1.7/src/PDF-Estimator/.git/refs/remotes/
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-09 01:33:00.585553 pypdfe-0.1.7/src/PDF-Estimator/.git/refs/remotes/origin/
--rw-r--r--   0 nate       (501) staff       (20)       30 2023-06-21 20:32:32.000000 pypdfe-0.1.7/src/PDF-Estimator/.git/refs/remotes/origin/HEAD
--rw-r--r--   0 nate       (501) staff       (20)     2947 2023-06-21 20:32:32.000000 pypdfe-0.1.7/src/PDF-Estimator/ChebyShev.cpp
--rw-r--r--   0 nate       (501) staff       (20)     1542 2023-06-21 20:32:32.000000 pypdfe-0.1.7/src/PDF-Estimator/ChebyShev.h
--rw-r--r--   0 nate       (501) staff       (20)     9785 2023-06-21 20:32:32.000000 pypdfe-0.1.7/src/PDF-Estimator/InputData.cpp
--rw-r--r--   0 nate       (501) staff       (20)     2287 2023-07-08 23:26:42.000000 pypdfe-0.1.7/src/PDF-Estimator/InputData.h
--rw-r--r--   0 nate       (501) staff       (20)     2941 2023-07-09 01:31:58.000000 pypdfe-0.1.7/src/PDF-Estimator/InputParameters.cpp
--rw-r--r--   0 nate       (501) staff       (20)     2472 2023-07-09 01:32:10.000000 pypdfe-0.1.7/src/PDF-Estimator/InputParameters.h
--rw-r--r--   0 nate       (501) staff       (20)     4922 2023-06-21 20:32:32.000000 pypdfe-0.1.7/src/PDF-Estimator/JointProbability.cpp
--rw-r--r--   0 nate       (501) staff       (20)     1713 2023-07-08 23:11:17.000000 pypdfe-0.1.7/src/PDF-Estimator/JointProbability.h
--rw-r--r--   0 nate       (501) staff       (20)    35149 2023-06-21 20:32:32.000000 pypdfe-0.1.7/src/PDF-Estimator/LICENSE
--rw-r--r--   0 nate       (501) staff       (20)    17168 2023-06-21 20:32:32.000000 pypdfe-0.1.7/src/PDF-Estimator/MinimizeScore.cpp
--rw-r--r--   0 nate       (501) staff       (20)     2892 2023-07-08 23:24:11.000000 pypdfe-0.1.7/src/PDF-Estimator/MinimizeScore.h
--rw-r--r--   0 nate       (501) staff       (20)     1750 2023-07-09 00:53:58.000000 pypdfe-0.1.7/src/PDF-Estimator/OutputControl.cpp
--rw-r--r--   0 nate       (501) staff       (20)     1855 2023-07-09 00:55:20.000000 pypdfe-0.1.7/src/PDF-Estimator/OutputControl.h
--rw-r--r--   0 nate       (501) staff       (20)      773 2023-06-21 20:32:32.000000 pypdfe-0.1.7/src/PDF-Estimator/README.txt
--rw-r--r--   0 nate       (501) staff       (20)     1959 2023-06-21 20:32:32.000000 pypdfe-0.1.7/src/PDF-Estimator/Score.cpp
--rw-r--r--   0 nate       (501) staff       (20)     1857 2023-06-21 20:32:32.000000 pypdfe-0.1.7/src/PDF-Estimator/Score.h
--rw-r--r--   0 nate       (501) staff       (20)    16156 2023-06-21 20:32:32.000000 pypdfe-0.1.7/src/PDF-Estimator/ScoreQZ.cpp
--rw-r--r--   0 nate       (501) staff       (20)     1410 2023-07-08 23:21:32.000000 pypdfe-0.1.7/src/PDF-Estimator/ScoreQZ.h
--rw-r--r--   0 nate       (501) staff       (20)     5467 2023-06-21 20:32:32.000000 pypdfe-0.1.7/src/PDF-Estimator/Variable.cpp
--rw-r--r--   0 nate       (501) staff       (20)     2024 2023-07-08 23:42:47.000000 pypdfe-0.1.7/src/PDF-Estimator/Variable.h
--rw-r--r--   0 nate       (501) staff       (20)    11691 2023-06-21 20:32:32.000000 pypdfe-0.1.7/src/PDF-Estimator/WriteResults.cpp
--rw-r--r--   0 nate       (501) staff       (20)     2354 2023-07-08 23:16:34.000000 pypdfe-0.1.7/src/PDF-Estimator/WriteResults.h
--rw-r--r--   0 nate       (501) staff       (20)     2407 2023-06-21 20:32:32.000000 pypdfe-0.1.7/src/PDF-Estimator/callPDF.cpp
--rw-r--r--   0 nate       (501) staff       (20)     1007 2023-06-21 20:32:32.000000 pypdfe-0.1.7/src/PDF-Estimator/callPDF.h
--rw-r--r--   0 nate       (501) staff       (20)     1704 2023-07-08 23:54:12.000000 pypdfe-0.1.7/src/PDF-Estimator/mvPDFMain.cpp
--rw-r--r--   0 nate       (501) staff       (20)     1149 2023-07-09 01:32:49.000000 pypdfe-0.1.7/src/main.cpp
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-09 17:58:32.241111 pypdfe-0.1.8/
+-rw-r--r--   0 nate       (501) staff       (20)    35148 2023-07-08 07:31:18.000000 pypdfe-0.1.8/LICENSE
+-rw-r--r--   0 nate       (501) staff       (20)        9 2023-07-09 17:57:39.000000 pypdfe-0.1.8/MANIFEST.in
+-rw-r--r--   0 nate       (501) staff       (20)      297 2023-07-09 17:58:32.241018 pypdfe-0.1.8/PKG-INFO
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-09 17:58:32.233096 pypdfe-0.1.8/pypdfe/
+-rw-r--r--   0 nate       (501) staff       (20)     1025 2023-07-08 07:18:43.000000 pypdfe-0.1.8/pypdfe/__init__.py
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-09 17:58:32.233768 pypdfe-0.1.8/pypdfe.egg-info/
+-rw-r--r--   0 nate       (501) staff       (20)      297 2023-07-09 17:58:32.000000 pypdfe-0.1.8/pypdfe.egg-info/PKG-INFO
+-rw-r--r--   0 nate       (501) staff       (20)     2354 2023-07-09 17:58:32.000000 pypdfe-0.1.8/pypdfe.egg-info/SOURCES.txt
+-rw-r--r--   0 nate       (501) staff       (20)        1 2023-07-09 17:58:32.000000 pypdfe-0.1.8/pypdfe.egg-info/dependency_links.txt
+-rw-r--r--   0 nate       (501) staff       (20)        1 2023-07-09 17:58:32.000000 pypdfe-0.1.8/pypdfe.egg-info/not-zip-safe
+-rw-r--r--   0 nate       (501) staff       (20)        6 2023-07-09 17:58:32.000000 pypdfe-0.1.8/pypdfe.egg-info/requires.txt
+-rw-r--r--   0 nate       (501) staff       (20)        7 2023-07-09 17:58:32.000000 pypdfe-0.1.8/pypdfe.egg-info/top_level.txt
+-rw-r--r--   0 nate       (501) staff       (20)      909 2023-07-09 17:57:39.000000 pypdfe-0.1.8/pyproject.toml
+-rw-r--r--   0 nate       (501) staff       (20)       38 2023-07-09 17:58:32.241147 pypdfe-0.1.8/setup.cfg
+-rw-r--r--   0 nate       (501) staff       (20)     2401 2023-07-09 17:57:39.000000 pypdfe-0.1.8/setup.py
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-09 17:58:32.234037 pypdfe-0.1.8/src/
+-rw-r--r--   0 nate       (501) staff       (20)     8196 2023-07-09 01:38:32.000000 pypdfe-0.1.8/src/.DS_Store
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-09 17:58:32.237363 pypdfe-0.1.8/src/PDF-Estimator/
+-rw-r--r--   0 nate       (501) staff       (20)     8196 2023-07-09 01:17:14.000000 pypdfe-0.1.8/src/PDF-Estimator/.DS_Store
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-09 17:58:32.238020 pypdfe-0.1.8/src/PDF-Estimator/.git/
+-rw-r--r--   0 nate       (501) staff       (20)      103 2023-06-21 22:03:26.000000 pypdfe-0.1.8/src/PDF-Estimator/.git/FETCH_HEAD
+-rw-r--r--   0 nate       (501) staff       (20)       21 2023-06-21 20:32:32.000000 pypdfe-0.1.8/src/PDF-Estimator/.git/HEAD
+-rw-r--r--   0 nate       (501) staff       (20)      309 2023-06-21 20:32:32.000000 pypdfe-0.1.8/src/PDF-Estimator/.git/config
+-rw-r--r--   0 nate       (501) staff       (20)       73 2023-06-21 20:32:31.000000 pypdfe-0.1.8/src/PDF-Estimator/.git/description
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-09 17:58:32.239831 pypdfe-0.1.8/src/PDF-Estimator/.git/hooks/
+-rwxr-xr-x   0 nate       (501) staff       (20)      478 2023-06-21 20:32:31.000000 pypdfe-0.1.8/src/PDF-Estimator/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0 nate       (501) staff       (20)      896 2023-06-21 20:32:31.000000 pypdfe-0.1.8/src/PDF-Estimator/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0 nate       (501) staff       (20)     4726 2023-06-21 20:32:31.000000 pypdfe-0.1.8/src/PDF-Estimator/.git/hooks/fsmonitor-watchman.sample
+-rwxr-xr-x   0 nate       (501) staff       (20)      189 2023-06-21 20:32:31.000000 pypdfe-0.1.8/src/PDF-Estimator/.git/hooks/post-update.sample
+-rwxr-xr-x   0 nate       (501) staff       (20)      424 2023-06-21 20:32:31.000000 pypdfe-0.1.8/src/PDF-Estimator/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0 nate       (501) staff       (20)     1643 2023-06-21 20:32:31.000000 pypdfe-0.1.8/src/PDF-Estimator/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0 nate       (501) staff       (20)      416 2023-06-21 20:32:31.000000 pypdfe-0.1.8/src/PDF-Estimator/.git/hooks/pre-merge-commit.sample
+-rwxr-xr-x   0 nate       (501) staff       (20)     1374 2023-06-21 20:32:31.000000 pypdfe-0.1.8/src/PDF-Estimator/.git/hooks/pre-push.sample
+-rwxr-xr-x   0 nate       (501) staff       (20)     4898 2023-06-21 20:32:31.000000 pypdfe-0.1.8/src/PDF-Estimator/.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0 nate       (501) staff       (20)      544 2023-06-21 20:32:31.000000 pypdfe-0.1.8/src/PDF-Estimator/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0 nate       (501) staff       (20)     1492 2023-06-21 20:32:31.000000 pypdfe-0.1.8/src/PDF-Estimator/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0 nate       (501) staff       (20)     2783 2023-06-21 20:32:31.000000 pypdfe-0.1.8/src/PDF-Estimator/.git/hooks/push-to-checkout.sample
+-rwxr-xr-x   0 nate       (501) staff       (20)     3650 2023-06-21 20:32:31.000000 pypdfe-0.1.8/src/PDF-Estimator/.git/hooks/update.sample
+-rw-r--r--   0 nate       (501) staff       (20)     2102 2023-06-22 03:25:25.000000 pypdfe-0.1.8/src/PDF-Estimator/.git/index
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-09 17:58:32.239942 pypdfe-0.1.8/src/PDF-Estimator/.git/info/
+-rw-r--r--   0 nate       (501) staff       (20)      240 2023-06-21 20:32:31.000000 pypdfe-0.1.8/src/PDF-Estimator/.git/info/exclude
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-09 17:58:32.240055 pypdfe-0.1.8/src/PDF-Estimator/.git/logs/
+-rw-r--r--   0 nate       (501) staff       (20)      213 2023-06-21 20:32:32.000000 pypdfe-0.1.8/src/PDF-Estimator/.git/logs/HEAD
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-09 17:58:32.232131 pypdfe-0.1.8/src/PDF-Estimator/.git/logs/refs/
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-09 17:58:32.240171 pypdfe-0.1.8/src/PDF-Estimator/.git/logs/refs/heads/
+-rw-r--r--   0 nate       (501) staff       (20)      213 2023-06-21 20:32:32.000000 pypdfe-0.1.8/src/PDF-Estimator/.git/logs/refs/heads/main
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-09 17:58:32.232180 pypdfe-0.1.8/src/PDF-Estimator/.git/logs/refs/remotes/
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-09 17:58:32.240296 pypdfe-0.1.8/src/PDF-Estimator/.git/logs/refs/remotes/origin/
+-rw-r--r--   0 nate       (501) staff       (20)      213 2023-06-21 20:32:32.000000 pypdfe-0.1.8/src/PDF-Estimator/.git/logs/refs/remotes/origin/HEAD
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-09 17:58:32.232290 pypdfe-0.1.8/src/PDF-Estimator/.git/objects/
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-09 17:58:32.240563 pypdfe-0.1.8/src/PDF-Estimator/.git/objects/pack/
+-r--r--r--   0 nate       (501) staff       (20)     1996 2023-06-21 20:32:32.000000 pypdfe-0.1.8/src/PDF-Estimator/.git/objects/pack/pack-68fcf6d5b1d91b28c20241431b9241a5762ddad3.idx
+-r--r--r--   0 nate       (501) staff       (20)    47733 2023-06-21 20:32:32.000000 pypdfe-0.1.8/src/PDF-Estimator/.git/objects/pack/pack-68fcf6d5b1d91b28c20241431b9241a5762ddad3.pack
+-rw-r--r--   0 nate       (501) staff       (20)      112 2023-06-21 20:32:32.000000 pypdfe-0.1.8/src/PDF-Estimator/.git/packed-refs
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-09 17:58:32.232469 pypdfe-0.1.8/src/PDF-Estimator/.git/refs/
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-09 17:58:32.240729 pypdfe-0.1.8/src/PDF-Estimator/.git/refs/heads/
+-rw-r--r--   0 nate       (501) staff       (20)       41 2023-06-21 20:32:32.000000 pypdfe-0.1.8/src/PDF-Estimator/.git/refs/heads/main
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-09 17:58:32.232518 pypdfe-0.1.8/src/PDF-Estimator/.git/refs/remotes/
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-09 17:58:32.240863 pypdfe-0.1.8/src/PDF-Estimator/.git/refs/remotes/origin/
+-rw-r--r--   0 nate       (501) staff       (20)       30 2023-06-21 20:32:32.000000 pypdfe-0.1.8/src/PDF-Estimator/.git/refs/remotes/origin/HEAD
+-rw-r--r--   0 nate       (501) staff       (20)     2947 2023-06-21 20:32:32.000000 pypdfe-0.1.8/src/PDF-Estimator/ChebyShev.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     1542 2023-06-21 20:32:32.000000 pypdfe-0.1.8/src/PDF-Estimator/ChebyShev.h
+-rw-r--r--   0 nate       (501) staff       (20)     9785 2023-06-21 20:32:32.000000 pypdfe-0.1.8/src/PDF-Estimator/InputData.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     2287 2023-07-08 23:26:42.000000 pypdfe-0.1.8/src/PDF-Estimator/InputData.h
+-rw-r--r--   0 nate       (501) staff       (20)     2941 2023-07-09 01:31:58.000000 pypdfe-0.1.8/src/PDF-Estimator/InputParameters.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     2470 2023-07-09 01:38:31.000000 pypdfe-0.1.8/src/PDF-Estimator/InputParameters.h
+-rw-r--r--   0 nate       (501) staff       (20)     4922 2023-06-21 20:32:32.000000 pypdfe-0.1.8/src/PDF-Estimator/JointProbability.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     1713 2023-07-08 23:11:17.000000 pypdfe-0.1.8/src/PDF-Estimator/JointProbability.h
+-rw-r--r--   0 nate       (501) staff       (20)    35149 2023-06-21 20:32:32.000000 pypdfe-0.1.8/src/PDF-Estimator/LICENSE
+-rw-r--r--   0 nate       (501) staff       (20)    17168 2023-06-21 20:32:32.000000 pypdfe-0.1.8/src/PDF-Estimator/MinimizeScore.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     2892 2023-07-08 23:24:11.000000 pypdfe-0.1.8/src/PDF-Estimator/MinimizeScore.h
+-rw-r--r--   0 nate       (501) staff       (20)     1750 2023-07-09 00:53:58.000000 pypdfe-0.1.8/src/PDF-Estimator/OutputControl.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     1855 2023-07-09 00:55:20.000000 pypdfe-0.1.8/src/PDF-Estimator/OutputControl.h
+-rw-r--r--   0 nate       (501) staff       (20)      773 2023-06-21 20:32:32.000000 pypdfe-0.1.8/src/PDF-Estimator/README.txt
+-rw-r--r--   0 nate       (501) staff       (20)     1959 2023-06-21 20:32:32.000000 pypdfe-0.1.8/src/PDF-Estimator/Score.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     1857 2023-06-21 20:32:32.000000 pypdfe-0.1.8/src/PDF-Estimator/Score.h
+-rw-r--r--   0 nate       (501) staff       (20)    16156 2023-06-21 20:32:32.000000 pypdfe-0.1.8/src/PDF-Estimator/ScoreQZ.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     1410 2023-07-08 23:21:32.000000 pypdfe-0.1.8/src/PDF-Estimator/ScoreQZ.h
+-rw-r--r--   0 nate       (501) staff       (20)     5467 2023-06-21 20:32:32.000000 pypdfe-0.1.8/src/PDF-Estimator/Variable.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     2024 2023-07-08 23:42:47.000000 pypdfe-0.1.8/src/PDF-Estimator/Variable.h
+-rw-r--r--   0 nate       (501) staff       (20)    11691 2023-06-21 20:32:32.000000 pypdfe-0.1.8/src/PDF-Estimator/WriteResults.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     2354 2023-07-08 23:16:34.000000 pypdfe-0.1.8/src/PDF-Estimator/WriteResults.h
+-rw-r--r--   0 nate       (501) staff       (20)     2407 2023-06-21 20:32:32.000000 pypdfe-0.1.8/src/PDF-Estimator/callPDF.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     1007 2023-06-21 20:32:32.000000 pypdfe-0.1.8/src/PDF-Estimator/callPDF.h
+-rw-r--r--   0 nate       (501) staff       (20)     1704 2023-07-08 23:54:12.000000 pypdfe-0.1.8/src/PDF-Estimator/mvPDFMain.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     1149 2023-07-09 17:57:39.000000 pypdfe-0.1.8/src/main.cpp
```

### Comparing `pypdfe-0.1.7/LICENSE` & `pypdfe-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/pypdfe/__init__.py` & `pypdfe-0.1.8/pypdfe/__init__.py`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/pypdfe.egg-info/SOURCES.txt` & `pypdfe-0.1.8/pypdfe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/pyproject.toml` & `pypdfe-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/src/.DS_Store` & `pypdfe-0.1.8/src/.DS_Store`

 * *Files 4% similar despite different names*

```diff
@@ -305,18 +305,18 @@
 00001300: 0080 0097 00a3 00af 00c1 00ce 00e3 00f5  ................
 00001310: 0103 010d 0116 0122 012b 012c 0135 0137  .......".+.,.5.7
 00001320: 0140 0149 014a 015b 015c 0161 016a 0000  .@.I.J.[.\.a.j..
 00001330: 0000 0000 0201 0000 0000 0000 001d 0000  ................
 00001340: 0000 0000 0000 0000 0000 0000 0173 0000  .............s..
 00001350: 000d 0050 0044 0046 002d 0045 0073 0074  ...P.D.F.-.E.s.t
 00001360: 0069 006d 0061 0074 006f 0072 6c67 3153  .i.m.a.t.o.rlg1S
-00001370: 636f 6d70 0000 0000 0003 609c 0000 000d  comp......`.....
+00001370: 636f 6d70 0000 0000 0003 609a 0000 000d  comp......`.....
 00001380: 0050 0044 0046 002d 0045 0073 0074 0069  .P.D.F.-.E.s.t.i
 00001390: 006d 0061 0074 006f 0072 6d6f 4444 626c  .m.a.t.o.rmoDDbl
-000013a0: 6f62 0000 0008 a7ed 74cd 222d c541 0000  ob......t."-.A..
+000013a0: 6f62 0000 0008 750f c68b 232d c541 0000  ob....u...#-.A..
 000013b0: 000d 0050 0044 0046 002d 0045 0073 0074  ...P.D.F.-.E.s.t
 000013c0: 0069 006d 0061 0074 006f 0072 6d6f 6444  .i.m.a.t.o.rmodD
 000013d0: 626c 6f62 0000 0008 d970 74b2 222d c541  blob.....pt."-.A
 000013e0: 0000 000d 0050 0044 0046 002d 0045 0073  .....P.D.F.-.E.s
 000013f0: 0074 0069 006d 0061 0074 006f 0072 7068  .t.i.m.a.t.o.rph
 00001400: 3153 636f 6d70 0000 0000 0005 9000 0000  1Scomp..........
 00001410: 000d 0050 0044 0046 002d 0045 0073 0074  ...P.D.F.-.E.s.t
```

### Comparing `pypdfe-0.1.7/src/PDF-Estimator/.DS_Store` & `pypdfe-0.1.8/src/PDF-Estimator/.DS_Store`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/src/PDF-Estimator/.git/hooks/commit-msg.sample` & `pypdfe-0.1.8/src/PDF-Estimator/.git/hooks/commit-msg.sample`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/src/PDF-Estimator/.git/hooks/fsmonitor-watchman.sample` & `pypdfe-0.1.8/src/PDF-Estimator/.git/hooks/fsmonitor-watchman.sample`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/src/PDF-Estimator/.git/hooks/pre-commit.sample` & `pypdfe-0.1.8/src/PDF-Estimator/.git/hooks/pre-commit.sample`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/src/PDF-Estimator/.git/hooks/pre-push.sample` & `pypdfe-0.1.8/src/PDF-Estimator/.git/hooks/pre-push.sample`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/src/PDF-Estimator/.git/hooks/pre-rebase.sample` & `pypdfe-0.1.8/src/PDF-Estimator/.git/hooks/pre-rebase.sample`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/src/PDF-Estimator/.git/hooks/pre-receive.sample` & `pypdfe-0.1.8/src/PDF-Estimator/.git/hooks/pre-receive.sample`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/src/PDF-Estimator/.git/hooks/prepare-commit-msg.sample` & `pypdfe-0.1.8/src/PDF-Estimator/.git/hooks/prepare-commit-msg.sample`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/src/PDF-Estimator/.git/hooks/push-to-checkout.sample` & `pypdfe-0.1.8/src/PDF-Estimator/.git/hooks/push-to-checkout.sample`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/src/PDF-Estimator/.git/hooks/update.sample` & `pypdfe-0.1.8/src/PDF-Estimator/.git/hooks/update.sample`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/src/PDF-Estimator/.git/index` & `pypdfe-0.1.8/src/PDF-Estimator/.git/index`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/src/PDF-Estimator/.git/objects/pack/pack-68fcf6d5b1d91b28c20241431b9241a5762ddad3.idx` & `pypdfe-0.1.8/src/PDF-Estimator/.git/objects/pack/pack-68fcf6d5b1d91b28c20241431b9241a5762ddad3.idx`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/src/PDF-Estimator/.git/objects/pack/pack-68fcf6d5b1d91b28c20241431b9241a5762ddad3.pack` & `pypdfe-0.1.8/src/PDF-Estimator/.git/objects/pack/pack-68fcf6d5b1d91b28c20241431b9241a5762ddad3.pack`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/src/PDF-Estimator/ChebyShev.cpp` & `pypdfe-0.1.8/src/PDF-Estimator/ChebyShev.cpp`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/src/PDF-Estimator/ChebyShev.h` & `pypdfe-0.1.8/src/PDF-Estimator/ChebyShev.h`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/src/PDF-Estimator/InputData.cpp` & `pypdfe-0.1.8/src/PDF-Estimator/InputData.cpp`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/src/PDF-Estimator/InputData.h` & `pypdfe-0.1.8/src/PDF-Estimator/InputData.h`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/src/PDF-Estimator/InputParameters.cpp` & `pypdfe-0.1.8/src/PDF-Estimator/InputParameters.cpp`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/src/PDF-Estimator/InputParameters.h` & `pypdfe-0.1.8/src/PDF-Estimator/InputParameters.h`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     void setEstimationPoints(vector <double> x);    
     vector <double> estimatedPoints;
     bool estimatePoints;
         
     InputParameters();
 //    InputParameters(const InputParameters& orig);
     virtual ~InputParameters();
-    bool userInput(int argc, char** argv);    
+//    bool userInput(int argc, char** argv);
     
     OutputControl out;
     
 private:    
     void printUsage();
     
 };
```

### Comparing `pypdfe-0.1.7/src/PDF-Estimator/JointProbability.cpp` & `pypdfe-0.1.8/src/PDF-Estimator/JointProbability.cpp`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/src/PDF-Estimator/JointProbability.h` & `pypdfe-0.1.8/src/PDF-Estimator/JointProbability.h`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/src/PDF-Estimator/LICENSE` & `pypdfe-0.1.8/src/PDF-Estimator/LICENSE`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/src/PDF-Estimator/MinimizeScore.cpp` & `pypdfe-0.1.8/src/PDF-Estimator/MinimizeScore.cpp`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/src/PDF-Estimator/MinimizeScore.h` & `pypdfe-0.1.8/src/PDF-Estimator/MinimizeScore.h`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/src/PDF-Estimator/OutputControl.cpp` & `pypdfe-0.1.8/src/PDF-Estimator/OutputControl.cpp`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/src/PDF-Estimator/OutputControl.h` & `pypdfe-0.1.8/src/PDF-Estimator/OutputControl.h`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/src/PDF-Estimator/README.txt` & `pypdfe-0.1.8/src/PDF-Estimator/README.txt`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/src/PDF-Estimator/Score.cpp` & `pypdfe-0.1.8/src/PDF-Estimator/Score.cpp`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/src/PDF-Estimator/Score.h` & `pypdfe-0.1.8/src/PDF-Estimator/Score.h`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/src/PDF-Estimator/ScoreQZ.cpp` & `pypdfe-0.1.8/src/PDF-Estimator/ScoreQZ.cpp`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/src/PDF-Estimator/ScoreQZ.h` & `pypdfe-0.1.8/src/PDF-Estimator/ScoreQZ.h`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/src/PDF-Estimator/Variable.cpp` & `pypdfe-0.1.8/src/PDF-Estimator/Variable.cpp`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/src/PDF-Estimator/Variable.h` & `pypdfe-0.1.8/src/PDF-Estimator/Variable.h`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/src/PDF-Estimator/WriteResults.cpp` & `pypdfe-0.1.8/src/PDF-Estimator/WriteResults.cpp`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/src/PDF-Estimator/WriteResults.h` & `pypdfe-0.1.8/src/PDF-Estimator/WriteResults.h`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/src/PDF-Estimator/callPDF.cpp` & `pypdfe-0.1.8/src/PDF-Estimator/callPDF.cpp`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/src/PDF-Estimator/callPDF.h` & `pypdfe-0.1.8/src/PDF-Estimator/callPDF.h`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/src/PDF-Estimator/mvPDFMain.cpp` & `pypdfe-0.1.8/src/PDF-Estimator/mvPDFMain.cpp`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.7/src/main.cpp` & `pypdfe-0.1.8/src/main.cpp`

 * *Files identical despite different names*

