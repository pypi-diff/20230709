# Comparing `tmp/pypdfe-0.1.5.tar.gz` & `tmp/pypdfe-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypdfe-0.1.5.tar", last modified: Sat Jul  8 19:24:15 2023, max compression
+gzip compressed data, was "pypdfe-0.1.6.tar", last modified: Sat Jul  8 21:53:56 2023, max compression
```

## Comparing `pypdfe-0.1.5.tar` & `pypdfe-0.1.6.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:24:15.511738 pypdfe-0.1.5/
--rw-r--r--   0 nate       (501) staff       (20)    35148 2023-07-08 07:31:18.000000 pypdfe-0.1.5/LICENSE
--rw-r--r--   0 nate       (501) staff       (20)        9 2023-07-08 19:23:32.000000 pypdfe-0.1.5/MANIFEST.in
--rw-r--r--   0 nate       (501) staff       (20)      297 2023-07-08 19:24:15.511637 pypdfe-0.1.5/PKG-INFO
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:24:15.503744 pypdfe-0.1.5/pypdfe/
--rw-r--r--   0 nate       (501) staff       (20)     1025 2023-07-08 07:18:43.000000 pypdfe-0.1.5/pypdfe/__init__.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:24:15.504485 pypdfe-0.1.5/pypdfe.egg-info/
--rw-r--r--   0 nate       (501) staff       (20)      297 2023-07-08 19:24:15.000000 pypdfe-0.1.5/pypdfe.egg-info/PKG-INFO
--rw-r--r--   0 nate       (501) staff       (20)     3658 2023-07-08 19:24:15.000000 pypdfe-0.1.5/pypdfe.egg-info/SOURCES.txt
--rw-r--r--   0 nate       (501) staff       (20)        1 2023-07-08 19:24:15.000000 pypdfe-0.1.5/pypdfe.egg-info/dependency_links.txt
--rw-r--r--   0 nate       (501) staff       (20)        1 2023-07-08 19:24:15.000000 pypdfe-0.1.5/pypdfe.egg-info/not-zip-safe
--rw-r--r--   0 nate       (501) staff       (20)        6 2023-07-08 19:24:15.000000 pypdfe-0.1.5/pypdfe.egg-info/requires.txt
--rw-r--r--   0 nate       (501) staff       (20)        7 2023-07-08 19:24:15.000000 pypdfe-0.1.5/pypdfe.egg-info/top_level.txt
--rw-r--r--   0 nate       (501) staff       (20)      131 2023-07-08 19:23:32.000000 pypdfe-0.1.5/pyproject.toml
--rw-r--r--   0 nate       (501) staff       (20)       38 2023-07-08 19:24:15.511783 pypdfe-0.1.5/setup.cfg
--rw-r--r--   0 nate       (501) staff       (20)     1698 2023-07-08 19:23:32.000000 pypdfe-0.1.5/setup.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:24:15.504733 pypdfe-0.1.5/src/
--rw-r--r--   0 nate       (501) staff       (20)     8196 2023-07-08 03:12:16.000000 pypdfe-0.1.5/src/.DS_Store
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:24:15.508040 pypdfe-0.1.5/src/PDF-Estimator/
--rw-r--r--   0 nate       (501) staff       (20)     8196 2023-06-21 21:23:08.000000 pypdfe-0.1.5/src/PDF-Estimator/.DS_Store
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:24:15.508772 pypdfe-0.1.5/src/PDF-Estimator/.git/
--rw-r--r--   0 nate       (501) staff       (20)      103 2023-06-21 22:03:26.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/FETCH_HEAD
--rw-r--r--   0 nate       (501) staff       (20)       21 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/HEAD
--rw-r--r--   0 nate       (501) staff       (20)      309 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/config
--rw-r--r--   0 nate       (501) staff       (20)       73 2023-06-21 20:32:31.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/description
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:24:15.510331 pypdfe-0.1.5/src/PDF-Estimator/.git/hooks/
--rwxr-xr-x   0 nate       (501) staff       (20)      478 2023-06-21 20:32:31.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0 nate       (501) staff       (20)      896 2023-06-21 20:32:31.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/hooks/commit-msg.sample
--rwxr-xr-x   0 nate       (501) staff       (20)     4726 2023-06-21 20:32:31.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/hooks/fsmonitor-watchman.sample
--rwxr-xr-x   0 nate       (501) staff       (20)      189 2023-06-21 20:32:31.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/hooks/post-update.sample
--rwxr-xr-x   0 nate       (501) staff       (20)      424 2023-06-21 20:32:31.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0 nate       (501) staff       (20)     1643 2023-06-21 20:32:31.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/hooks/pre-commit.sample
--rwxr-xr-x   0 nate       (501) staff       (20)      416 2023-06-21 20:32:31.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/hooks/pre-merge-commit.sample
--rwxr-xr-x   0 nate       (501) staff       (20)     1374 2023-06-21 20:32:31.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/hooks/pre-push.sample
--rwxr-xr-x   0 nate       (501) staff       (20)     4898 2023-06-21 20:32:31.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/hooks/pre-rebase.sample
--rwxr-xr-x   0 nate       (501) staff       (20)      544 2023-06-21 20:32:31.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/hooks/pre-receive.sample
--rwxr-xr-x   0 nate       (501) staff       (20)     1492 2023-06-21 20:32:31.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0 nate       (501) staff       (20)     2783 2023-06-21 20:32:31.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/hooks/push-to-checkout.sample
--rwxr-xr-x   0 nate       (501) staff       (20)     3650 2023-06-21 20:32:31.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/hooks/update.sample
--rw-r--r--   0 nate       (501) staff       (20)     2102 2023-06-22 03:25:25.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/index
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:24:15.510459 pypdfe-0.1.5/src/PDF-Estimator/.git/info/
--rw-r--r--   0 nate       (501) staff       (20)      240 2023-06-21 20:32:31.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/info/exclude
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:24:15.510578 pypdfe-0.1.5/src/PDF-Estimator/.git/logs/
--rw-r--r--   0 nate       (501) staff       (20)      213 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/logs/HEAD
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:24:15.502333 pypdfe-0.1.5/src/PDF-Estimator/.git/logs/refs/
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:24:15.510717 pypdfe-0.1.5/src/PDF-Estimator/.git/logs/refs/heads/
--rw-r--r--   0 nate       (501) staff       (20)      213 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/logs/refs/heads/main
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:24:15.502377 pypdfe-0.1.5/src/PDF-Estimator/.git/logs/refs/remotes/
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:24:15.510853 pypdfe-0.1.5/src/PDF-Estimator/.git/logs/refs/remotes/origin/
--rw-r--r--   0 nate       (501) staff       (20)      213 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/logs/refs/remotes/origin/HEAD
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:24:15.502503 pypdfe-0.1.5/src/PDF-Estimator/.git/objects/
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:24:15.511157 pypdfe-0.1.5/src/PDF-Estimator/.git/objects/pack/
--r--r--r--   0 nate       (501) staff       (20)     1996 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/objects/pack/pack-68fcf6d5b1d91b28c20241431b9241a5762ddad3.idx
--r--r--r--   0 nate       (501) staff       (20)    47733 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/objects/pack/pack-68fcf6d5b1d91b28c20241431b9241a5762ddad3.pack
--rw-r--r--   0 nate       (501) staff       (20)      112 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/packed-refs
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:24:15.502701 pypdfe-0.1.5/src/PDF-Estimator/.git/refs/
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:24:15.511318 pypdfe-0.1.5/src/PDF-Estimator/.git/refs/heads/
--rw-r--r--   0 nate       (501) staff       (20)       41 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/refs/heads/main
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:24:15.502740 pypdfe-0.1.5/src/PDF-Estimator/.git/refs/remotes/
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 19:24:15.511450 pypdfe-0.1.5/src/PDF-Estimator/.git/refs/remotes/origin/
--rw-r--r--   0 nate       (501) staff       (20)       30 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/.git/refs/remotes/origin/HEAD
--rw-r--r--   0 nate       (501) staff       (20)     2947 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/ChebyShev.cpp
--rw-r--r--   0 nate       (501) staff       (20)     1542 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/ChebyShev.h
--rw-r--r--   0 nate       (501) staff       (20)     9785 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/InputData.cpp
--rw-r--r--   0 nate       (501) staff       (20)     2214 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/InputData.h
--rw-r--r--   0 nate       (501) staff       (20)     8394 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/InputParameters.cpp
--rw-r--r--   0 nate       (501) staff       (20)     2470 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/InputParameters.h
--rw-r--r--   0 nate       (501) staff       (20)     4922 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/JointProbability.cpp
--rw-r--r--   0 nate       (501) staff       (20)     1711 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/JointProbability.h
--rw-r--r--   0 nate       (501) staff       (20)    35149 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/LICENSE
--rw-r--r--   0 nate       (501) staff       (20)    17168 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/MinimizeScore.cpp
--rw-r--r--   0 nate       (501) staff       (20)     2839 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/MinimizeScore.h
--rw-r--r--   0 nate       (501) staff       (20)     4372 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/OutputControl.cpp
--rw-r--r--   0 nate       (501) staff       (20)     2028 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/OutputControl.h
--rw-r--r--   0 nate       (501) staff       (20)      773 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/README.txt
--rw-r--r--   0 nate       (501) staff       (20)     1959 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/Score.cpp
--rw-r--r--   0 nate       (501) staff       (20)     1857 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/Score.h
--rw-r--r--   0 nate       (501) staff       (20)    16156 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/ScoreQZ.cpp
--rw-r--r--   0 nate       (501) staff       (20)     1410 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/ScoreQZ.h
--rw-r--r--   0 nate       (501) staff       (20)     5467 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/Variable.cpp
--rw-r--r--   0 nate       (501) staff       (20)     1995 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/Variable.h
--rw-r--r--   0 nate       (501) staff       (20)    11691 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/WriteResults.cpp
--rw-r--r--   0 nate       (501) staff       (20)     2352 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/WriteResults.h
--rw-r--r--   0 nate       (501) staff       (20)     2407 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/callPDF.cpp
--rw-r--r--   0 nate       (501) staff       (20)     1007 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/callPDF.h
--rw-r--r--   0 nate       (501) staff       (20)     1669 2023-06-21 20:32:32.000000 pypdfe-0.1.5/src/PDF-Estimator/mvPDFMain.cpp
--rw-r--r--   0 nate       (501) staff       (20)     1149 2023-07-08 19:23:32.000000 pypdfe-0.1.5/src/main.cpp
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 21:53:56.883204 pypdfe-0.1.6/
+-rw-r--r--   0 nate       (501) staff       (20)    35148 2023-07-08 07:31:18.000000 pypdfe-0.1.6/LICENSE
+-rw-r--r--   0 nate       (501) staff       (20)        9 2023-07-08 21:53:25.000000 pypdfe-0.1.6/MANIFEST.in
+-rw-r--r--   0 nate       (501) staff       (20)      297 2023-07-08 21:53:56.883099 pypdfe-0.1.6/PKG-INFO
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 21:53:56.875016 pypdfe-0.1.6/pypdfe/
+-rw-r--r--   0 nate       (501) staff       (20)     1025 2023-07-08 07:18:43.000000 pypdfe-0.1.6/pypdfe/__init__.py
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 21:53:56.875740 pypdfe-0.1.6/pypdfe.egg-info/
+-rw-r--r--   0 nate       (501) staff       (20)      297 2023-07-08 21:53:56.000000 pypdfe-0.1.6/pypdfe.egg-info/PKG-INFO
+-rw-r--r--   0 nate       (501) staff       (20)     2354 2023-07-08 21:53:56.000000 pypdfe-0.1.6/pypdfe.egg-info/SOURCES.txt
+-rw-r--r--   0 nate       (501) staff       (20)        1 2023-07-08 21:53:56.000000 pypdfe-0.1.6/pypdfe.egg-info/dependency_links.txt
+-rw-r--r--   0 nate       (501) staff       (20)        1 2023-07-08 21:53:56.000000 pypdfe-0.1.6/pypdfe.egg-info/not-zip-safe
+-rw-r--r--   0 nate       (501) staff       (20)        6 2023-07-08 21:53:56.000000 pypdfe-0.1.6/pypdfe.egg-info/requires.txt
+-rw-r--r--   0 nate       (501) staff       (20)        7 2023-07-08 21:53:56.000000 pypdfe-0.1.6/pypdfe.egg-info/top_level.txt
+-rw-r--r--   0 nate       (501) staff       (20)      909 2023-07-08 21:53:25.000000 pypdfe-0.1.6/pyproject.toml
+-rw-r--r--   0 nate       (501) staff       (20)       38 2023-07-08 21:53:56.883242 pypdfe-0.1.6/setup.cfg
+-rw-r--r--   0 nate       (501) staff       (20)     1324 2023-07-08 21:53:25.000000 pypdfe-0.1.6/setup.py
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 21:53:56.875963 pypdfe-0.1.6/src/
+-rw-r--r--   0 nate       (501) staff       (20)     8196 2023-07-08 03:12:16.000000 pypdfe-0.1.6/src/.DS_Store
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 21:53:56.879306 pypdfe-0.1.6/src/PDF-Estimator/
+-rw-r--r--   0 nate       (501) staff       (20)     8196 2023-06-21 21:23:08.000000 pypdfe-0.1.6/src/PDF-Estimator/.DS_Store
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 21:53:56.880010 pypdfe-0.1.6/src/PDF-Estimator/.git/
+-rw-r--r--   0 nate       (501) staff       (20)      103 2023-06-21 22:03:26.000000 pypdfe-0.1.6/src/PDF-Estimator/.git/FETCH_HEAD
+-rw-r--r--   0 nate       (501) staff       (20)       21 2023-06-21 20:32:32.000000 pypdfe-0.1.6/src/PDF-Estimator/.git/HEAD
+-rw-r--r--   0 nate       (501) staff       (20)      309 2023-06-21 20:32:32.000000 pypdfe-0.1.6/src/PDF-Estimator/.git/config
+-rw-r--r--   0 nate       (501) staff       (20)       73 2023-06-21 20:32:31.000000 pypdfe-0.1.6/src/PDF-Estimator/.git/description
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 21:53:56.881913 pypdfe-0.1.6/src/PDF-Estimator/.git/hooks/
+-rwxr-xr-x   0 nate       (501) staff       (20)      478 2023-06-21 20:32:31.000000 pypdfe-0.1.6/src/PDF-Estimator/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0 nate       (501) staff       (20)      896 2023-06-21 20:32:31.000000 pypdfe-0.1.6/src/PDF-Estimator/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0 nate       (501) staff       (20)     4726 2023-06-21 20:32:31.000000 pypdfe-0.1.6/src/PDF-Estimator/.git/hooks/fsmonitor-watchman.sample
+-rwxr-xr-x   0 nate       (501) staff       (20)      189 2023-06-21 20:32:31.000000 pypdfe-0.1.6/src/PDF-Estimator/.git/hooks/post-update.sample
+-rwxr-xr-x   0 nate       (501) staff       (20)      424 2023-06-21 20:32:31.000000 pypdfe-0.1.6/src/PDF-Estimator/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0 nate       (501) staff       (20)     1643 2023-06-21 20:32:31.000000 pypdfe-0.1.6/src/PDF-Estimator/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0 nate       (501) staff       (20)      416 2023-06-21 20:32:31.000000 pypdfe-0.1.6/src/PDF-Estimator/.git/hooks/pre-merge-commit.sample
+-rwxr-xr-x   0 nate       (501) staff       (20)     1374 2023-06-21 20:32:31.000000 pypdfe-0.1.6/src/PDF-Estimator/.git/hooks/pre-push.sample
+-rwxr-xr-x   0 nate       (501) staff       (20)     4898 2023-06-21 20:32:31.000000 pypdfe-0.1.6/src/PDF-Estimator/.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0 nate       (501) staff       (20)      544 2023-06-21 20:32:31.000000 pypdfe-0.1.6/src/PDF-Estimator/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0 nate       (501) staff       (20)     1492 2023-06-21 20:32:31.000000 pypdfe-0.1.6/src/PDF-Estimator/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0 nate       (501) staff       (20)     2783 2023-06-21 20:32:31.000000 pypdfe-0.1.6/src/PDF-Estimator/.git/hooks/push-to-checkout.sample
+-rwxr-xr-x   0 nate       (501) staff       (20)     3650 2023-06-21 20:32:31.000000 pypdfe-0.1.6/src/PDF-Estimator/.git/hooks/update.sample
+-rw-r--r--   0 nate       (501) staff       (20)     2102 2023-06-22 03:25:25.000000 pypdfe-0.1.6/src/PDF-Estimator/.git/index
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 21:53:56.882032 pypdfe-0.1.6/src/PDF-Estimator/.git/info/
+-rw-r--r--   0 nate       (501) staff       (20)      240 2023-06-21 20:32:31.000000 pypdfe-0.1.6/src/PDF-Estimator/.git/info/exclude
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 21:53:56.882141 pypdfe-0.1.6/src/PDF-Estimator/.git/logs/
+-rw-r--r--   0 nate       (501) staff       (20)      213 2023-06-21 20:32:32.000000 pypdfe-0.1.6/src/PDF-Estimator/.git/logs/HEAD
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 21:53:56.874039 pypdfe-0.1.6/src/PDF-Estimator/.git/logs/refs/
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 21:53:56.882258 pypdfe-0.1.6/src/PDF-Estimator/.git/logs/refs/heads/
+-rw-r--r--   0 nate       (501) staff       (20)      213 2023-06-21 20:32:32.000000 pypdfe-0.1.6/src/PDF-Estimator/.git/logs/refs/heads/main
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 21:53:56.874091 pypdfe-0.1.6/src/PDF-Estimator/.git/logs/refs/remotes/
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 21:53:56.882384 pypdfe-0.1.6/src/PDF-Estimator/.git/logs/refs/remotes/origin/
+-rw-r--r--   0 nate       (501) staff       (20)      213 2023-06-21 20:32:32.000000 pypdfe-0.1.6/src/PDF-Estimator/.git/logs/refs/remotes/origin/HEAD
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 21:53:56.874205 pypdfe-0.1.6/src/PDF-Estimator/.git/objects/
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 21:53:56.882632 pypdfe-0.1.6/src/PDF-Estimator/.git/objects/pack/
+-r--r--r--   0 nate       (501) staff       (20)     1996 2023-06-21 20:32:32.000000 pypdfe-0.1.6/src/PDF-Estimator/.git/objects/pack/pack-68fcf6d5b1d91b28c20241431b9241a5762ddad3.idx
+-r--r--r--   0 nate       (501) staff       (20)    47733 2023-06-21 20:32:32.000000 pypdfe-0.1.6/src/PDF-Estimator/.git/objects/pack/pack-68fcf6d5b1d91b28c20241431b9241a5762ddad3.pack
+-rw-r--r--   0 nate       (501) staff       (20)      112 2023-06-21 20:32:32.000000 pypdfe-0.1.6/src/PDF-Estimator/.git/packed-refs
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 21:53:56.874387 pypdfe-0.1.6/src/PDF-Estimator/.git/refs/
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 21:53:56.882799 pypdfe-0.1.6/src/PDF-Estimator/.git/refs/heads/
+-rw-r--r--   0 nate       (501) staff       (20)       41 2023-06-21 20:32:32.000000 pypdfe-0.1.6/src/PDF-Estimator/.git/refs/heads/main
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 21:53:56.874436 pypdfe-0.1.6/src/PDF-Estimator/.git/refs/remotes/
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-07-08 21:53:56.882926 pypdfe-0.1.6/src/PDF-Estimator/.git/refs/remotes/origin/
+-rw-r--r--   0 nate       (501) staff       (20)       30 2023-06-21 20:32:32.000000 pypdfe-0.1.6/src/PDF-Estimator/.git/refs/remotes/origin/HEAD
+-rw-r--r--   0 nate       (501) staff       (20)     2947 2023-06-21 20:32:32.000000 pypdfe-0.1.6/src/PDF-Estimator/ChebyShev.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     1542 2023-06-21 20:32:32.000000 pypdfe-0.1.6/src/PDF-Estimator/ChebyShev.h
+-rw-r--r--   0 nate       (501) staff       (20)     9785 2023-06-21 20:32:32.000000 pypdfe-0.1.6/src/PDF-Estimator/InputData.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     2214 2023-06-21 20:32:32.000000 pypdfe-0.1.6/src/PDF-Estimator/InputData.h
+-rw-r--r--   0 nate       (501) staff       (20)     8394 2023-06-21 20:32:32.000000 pypdfe-0.1.6/src/PDF-Estimator/InputParameters.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     2470 2023-06-21 20:32:32.000000 pypdfe-0.1.6/src/PDF-Estimator/InputParameters.h
+-rw-r--r--   0 nate       (501) staff       (20)     4922 2023-06-21 20:32:32.000000 pypdfe-0.1.6/src/PDF-Estimator/JointProbability.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     1711 2023-06-21 20:32:32.000000 pypdfe-0.1.6/src/PDF-Estimator/JointProbability.h
+-rw-r--r--   0 nate       (501) staff       (20)    35149 2023-06-21 20:32:32.000000 pypdfe-0.1.6/src/PDF-Estimator/LICENSE
+-rw-r--r--   0 nate       (501) staff       (20)    17168 2023-06-21 20:32:32.000000 pypdfe-0.1.6/src/PDF-Estimator/MinimizeScore.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     2839 2023-06-21 20:32:32.000000 pypdfe-0.1.6/src/PDF-Estimator/MinimizeScore.h
+-rw-r--r--   0 nate       (501) staff       (20)     4372 2023-06-21 20:32:32.000000 pypdfe-0.1.6/src/PDF-Estimator/OutputControl.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     2028 2023-06-21 20:32:32.000000 pypdfe-0.1.6/src/PDF-Estimator/OutputControl.h
+-rw-r--r--   0 nate       (501) staff       (20)      773 2023-06-21 20:32:32.000000 pypdfe-0.1.6/src/PDF-Estimator/README.txt
+-rw-r--r--   0 nate       (501) staff       (20)     1959 2023-06-21 20:32:32.000000 pypdfe-0.1.6/src/PDF-Estimator/Score.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     1857 2023-06-21 20:32:32.000000 pypdfe-0.1.6/src/PDF-Estimator/Score.h
+-rw-r--r--   0 nate       (501) staff       (20)    16156 2023-06-21 20:32:32.000000 pypdfe-0.1.6/src/PDF-Estimator/ScoreQZ.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     1410 2023-06-21 20:32:32.000000 pypdfe-0.1.6/src/PDF-Estimator/ScoreQZ.h
+-rw-r--r--   0 nate       (501) staff       (20)     5467 2023-06-21 20:32:32.000000 pypdfe-0.1.6/src/PDF-Estimator/Variable.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     1995 2023-06-21 20:32:32.000000 pypdfe-0.1.6/src/PDF-Estimator/Variable.h
+-rw-r--r--   0 nate       (501) staff       (20)    11691 2023-06-21 20:32:32.000000 pypdfe-0.1.6/src/PDF-Estimator/WriteResults.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     2352 2023-06-21 20:32:32.000000 pypdfe-0.1.6/src/PDF-Estimator/WriteResults.h
+-rw-r--r--   0 nate       (501) staff       (20)     2407 2023-06-21 20:32:32.000000 pypdfe-0.1.6/src/PDF-Estimator/callPDF.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     1007 2023-06-21 20:32:32.000000 pypdfe-0.1.6/src/PDF-Estimator/callPDF.h
+-rw-r--r--   0 nate       (501) staff       (20)     1669 2023-06-21 20:32:32.000000 pypdfe-0.1.6/src/PDF-Estimator/mvPDFMain.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     1149 2023-07-08 21:53:25.000000 pypdfe-0.1.6/src/main.cpp
```

### Comparing `pypdfe-0.1.5/LICENSE` & `pypdfe-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/pypdfe/__init__.py` & `pypdfe-0.1.6/pypdfe/__init__.py`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/.DS_Store` & `pypdfe-0.1.6/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/PDF-Estimator/.DS_Store` & `pypdfe-0.1.6/src/PDF-Estimator/.DS_Store`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/PDF-Estimator/.git/hooks/commit-msg.sample` & `pypdfe-0.1.6/src/PDF-Estimator/.git/hooks/commit-msg.sample`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/PDF-Estimator/.git/hooks/fsmonitor-watchman.sample` & `pypdfe-0.1.6/src/PDF-Estimator/.git/hooks/fsmonitor-watchman.sample`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/PDF-Estimator/.git/hooks/pre-commit.sample` & `pypdfe-0.1.6/src/PDF-Estimator/.git/hooks/pre-commit.sample`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/PDF-Estimator/.git/hooks/pre-push.sample` & `pypdfe-0.1.6/src/PDF-Estimator/.git/hooks/pre-push.sample`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/PDF-Estimator/.git/hooks/pre-rebase.sample` & `pypdfe-0.1.6/src/PDF-Estimator/.git/hooks/pre-rebase.sample`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/PDF-Estimator/.git/hooks/pre-receive.sample` & `pypdfe-0.1.6/src/PDF-Estimator/.git/hooks/pre-receive.sample`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/PDF-Estimator/.git/hooks/prepare-commit-msg.sample` & `pypdfe-0.1.6/src/PDF-Estimator/.git/hooks/prepare-commit-msg.sample`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/PDF-Estimator/.git/hooks/push-to-checkout.sample` & `pypdfe-0.1.6/src/PDF-Estimator/.git/hooks/push-to-checkout.sample`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/PDF-Estimator/.git/hooks/update.sample` & `pypdfe-0.1.6/src/PDF-Estimator/.git/hooks/update.sample`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/PDF-Estimator/.git/index` & `pypdfe-0.1.6/src/PDF-Estimator/.git/index`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/PDF-Estimator/.git/objects/pack/pack-68fcf6d5b1d91b28c20241431b9241a5762ddad3.idx` & `pypdfe-0.1.6/src/PDF-Estimator/.git/objects/pack/pack-68fcf6d5b1d91b28c20241431b9241a5762ddad3.idx`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/PDF-Estimator/.git/objects/pack/pack-68fcf6d5b1d91b28c20241431b9241a5762ddad3.pack` & `pypdfe-0.1.6/src/PDF-Estimator/.git/objects/pack/pack-68fcf6d5b1d91b28c20241431b9241a5762ddad3.pack`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/PDF-Estimator/ChebyShev.cpp` & `pypdfe-0.1.6/src/PDF-Estimator/ChebyShev.cpp`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/PDF-Estimator/ChebyShev.h` & `pypdfe-0.1.6/src/PDF-Estimator/ChebyShev.h`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/PDF-Estimator/InputData.cpp` & `pypdfe-0.1.6/src/PDF-Estimator/InputData.cpp`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/PDF-Estimator/InputData.h` & `pypdfe-0.1.6/src/PDF-Estimator/InputData.h`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/PDF-Estimator/InputParameters.cpp` & `pypdfe-0.1.6/src/PDF-Estimator/InputParameters.cpp`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/PDF-Estimator/InputParameters.h` & `pypdfe-0.1.6/src/PDF-Estimator/InputParameters.h`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/PDF-Estimator/JointProbability.cpp` & `pypdfe-0.1.6/src/PDF-Estimator/JointProbability.cpp`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/PDF-Estimator/JointProbability.h` & `pypdfe-0.1.6/src/PDF-Estimator/JointProbability.h`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/PDF-Estimator/LICENSE` & `pypdfe-0.1.6/src/PDF-Estimator/LICENSE`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/PDF-Estimator/MinimizeScore.cpp` & `pypdfe-0.1.6/src/PDF-Estimator/MinimizeScore.cpp`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/PDF-Estimator/MinimizeScore.h` & `pypdfe-0.1.6/src/PDF-Estimator/MinimizeScore.h`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/PDF-Estimator/OutputControl.cpp` & `pypdfe-0.1.6/src/PDF-Estimator/OutputControl.cpp`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/PDF-Estimator/OutputControl.h` & `pypdfe-0.1.6/src/PDF-Estimator/OutputControl.h`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/PDF-Estimator/README.txt` & `pypdfe-0.1.6/src/PDF-Estimator/README.txt`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/PDF-Estimator/Score.cpp` & `pypdfe-0.1.6/src/PDF-Estimator/Score.cpp`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/PDF-Estimator/Score.h` & `pypdfe-0.1.6/src/PDF-Estimator/Score.h`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/PDF-Estimator/ScoreQZ.cpp` & `pypdfe-0.1.6/src/PDF-Estimator/ScoreQZ.cpp`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/PDF-Estimator/ScoreQZ.h` & `pypdfe-0.1.6/src/PDF-Estimator/ScoreQZ.h`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/PDF-Estimator/Variable.cpp` & `pypdfe-0.1.6/src/PDF-Estimator/Variable.cpp`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/PDF-Estimator/Variable.h` & `pypdfe-0.1.6/src/PDF-Estimator/Variable.h`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/PDF-Estimator/WriteResults.cpp` & `pypdfe-0.1.6/src/PDF-Estimator/WriteResults.cpp`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/PDF-Estimator/WriteResults.h` & `pypdfe-0.1.6/src/PDF-Estimator/WriteResults.h`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/PDF-Estimator/callPDF.cpp` & `pypdfe-0.1.6/src/PDF-Estimator/callPDF.cpp`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/PDF-Estimator/callPDF.h` & `pypdfe-0.1.6/src/PDF-Estimator/callPDF.h`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/PDF-Estimator/mvPDFMain.cpp` & `pypdfe-0.1.6/src/PDF-Estimator/mvPDFMain.cpp`

 * *Files identical despite different names*

### Comparing `pypdfe-0.1.5/src/main.cpp` & `pypdfe-0.1.6/src/main.cpp`

 * *Files identical despite different names*

