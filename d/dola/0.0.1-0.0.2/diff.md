# Comparing `tmp/dola-0.0.1.tar.gz` & `tmp/dola-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dola-0.0.1.tar", last modified: Sun Jul  9 09:28:22 2023, max compression
+gzip compressed data, was "dola-0.0.2.tar", last modified: Sun Jul  9 15:29:50 2023, max compression
```

## Comparing `dola-0.0.1.tar` & `dola-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxr-xr-x   0 laizeqiang   (501) staff       (20)        0 2023-07-09 09:28:22.325662 dola-0.0.1/
--rw-r--r--   0 laizeqiang   (501) staff       (20)      105 2023-07-09 09:28:22.325520 dola-0.0.1/PKG-INFO
--rw-r--r--   0 laizeqiang   (501) staff       (20)      100 2023-07-09 09:20:57.000000 dola-0.0.1/README.md
-drwxr-xr-x   0 laizeqiang   (501) staff       (20)        0 2023-07-09 09:28:22.324762 dola-0.0.1/dola/
--rw-r--r--   0 laizeqiang   (501) staff       (20)        0 2023-07-09 09:06:08.000000 dola-0.0.1/dola/__init__.py
-drwxr-xr-x   0 laizeqiang   (501) staff       (20)        0 2023-07-09 09:28:22.325338 dola-0.0.1/dola.egg-info/
--rw-r--r--   0 laizeqiang   (501) staff       (20)      105 2023-07-09 09:28:22.000000 dola-0.0.1/dola.egg-info/PKG-INFO
--rw-r--r--   0 laizeqiang   (501) staff       (20)      147 2023-07-09 09:28:22.000000 dola-0.0.1/dola.egg-info/SOURCES.txt
--rw-r--r--   0 laizeqiang   (501) staff       (20)        1 2023-07-09 09:28:22.000000 dola-0.0.1/dola.egg-info/dependency_links.txt
--rw-r--r--   0 laizeqiang   (501) staff       (20)        5 2023-07-09 09:28:22.000000 dola-0.0.1/dola.egg-info/top_level.txt
--rw-r--r--   0 laizeqiang   (501) staff       (20)       38 2023-07-09 09:28:22.325712 dola-0.0.1/setup.cfg
--rw-r--r--   0 laizeqiang   (501) staff       (20)      222 2023-07-09 09:22:46.000000 dola-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:29:50.066240 dola-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-09 15:29:50.066240 dola-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-09 15:29:41.000000 dola-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:29:50.066240 dola-0.0.2/dola/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-09 15:29:41.000000 dola-0.0.2/dola/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-07-09 15:29:41.000000 dola-0.0.2/dola/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-09 15:29:41.000000 dola-0.0.2/dola/os.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-07-09 15:29:41.000000 dola-0.0.2/dola/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:29:50.066240 dola-0.0.2/dola.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-09 15:29:50.000000 dola-0.0.2/dola.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-09 15:29:50.000000 dola-0.0.2/dola.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 15:29:50.000000 dola-0.0.2/dola.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-09 15:29:50.000000 dola-0.0.2/dola.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 15:29:50.066240 dola-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-09 15:29:41.000000 dola-0.0.2/setup.py
```

