# Comparing `tmp/npdtools-0.1a5.tar.gz` & `tmp/npdtools-1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npdtools-0.1a5.tar", last modified: Thu Sep  9 11:10:54 2021, max compression
+gzip compressed data, was "npdtools-1.0a1.tar", last modified: Sun Jul  9 13:50:10 2023, max compression
```

## Comparing `npdtools-0.1a5.tar` & `npdtools-1.0a1.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxr-xr-x   0 white     (1000) white     (1000)        0 2021-09-09 11:10:54.984191 npdtools-0.1a5/
--rw-r--r--   0 white     (1000) white     (1000)    16725 2021-06-06 10:07:23.000000 npdtools-0.1a5/LICENSE
--rw-r--r--   0 white     (1000) white     (1000)     5725 2021-09-09 11:10:54.984191 npdtools-0.1a5/PKG-INFO
--rw-r--r--   0 white     (1000) white     (1000)     5066 2021-06-06 10:03:55.000000 npdtools-0.1a5/README.md
-drwxr-xr-x   0 white     (1000) white     (1000)        0 2021-09-09 11:10:54.977525 npdtools-0.1a5/npdtools/
--rw-r--r--   0 white     (1000) white     (1000)       37 2021-05-04 21:08:54.000000 npdtools-0.1a5/npdtools/__init__.py
--rw-r--r--   0 white     (1000) white     (1000)    10464 2021-09-09 10:25:50.000000 npdtools-0.1a5/npdtools/client.py
-drwxr-xr-x   0 white     (1000) white     (1000)        0 2021-09-09 11:10:54.980858 npdtools-0.1a5/npdtools/errors/
--rw-r--r--   0 white     (1000) white     (1000)      436 2021-05-15 04:28:17.000000 npdtools-0.1a5/npdtools/errors/FNSError.py
--rw-r--r--   0 white     (1000) white     (1000)       46 2021-05-15 04:12:30.000000 npdtools-0.1a5/npdtools/errors/__init__.py
-drwxr-xr-x   0 white     (1000) white     (1000)        0 2021-09-09 11:10:54.980858 npdtools-0.1a5/npdtools/types/
--rw-r--r--   0 white     (1000) white     (1000)      172 2021-05-05 01:29:59.000000 npdtools-0.1a5/npdtools/types/__init__.py
--rw-r--r--   0 white     (1000) white     (1000)      960 2021-09-09 11:10:04.000000 npdtools-0.1a5/npdtools/types/client.py
--rw-r--r--   0 white     (1000) white     (1000)     3720 2021-05-06 04:29:02.000000 npdtools-0.1a5/npdtools/types/income.py
--rw-r--r--   0 white     (1000) white     (1000)     2884 2021-06-06 09:02:21.000000 npdtools-0.1a5/npdtools/types/services.py
-drwxr-xr-x   0 white     (1000) white     (1000)        0 2021-09-09 11:10:54.980858 npdtools-0.1a5/npdtools.egg-info/
--rw-r--r--   0 white     (1000) white     (1000)     5725 2021-09-09 11:10:54.000000 npdtools-0.1a5/npdtools.egg-info/PKG-INFO
--rw-r--r--   0 white     (1000) white     (1000)      385 2021-09-09 11:10:54.000000 npdtools-0.1a5/npdtools.egg-info/SOURCES.txt
--rw-r--r--   0 white     (1000) white     (1000)        1 2021-09-09 11:10:54.000000 npdtools-0.1a5/npdtools.egg-info/dependency_links.txt
--rw-r--r--   0 white     (1000) white     (1000)       13 2021-09-09 11:10:54.000000 npdtools-0.1a5/npdtools.egg-info/requires.txt
--rw-r--r--   0 white     (1000) white     (1000)        9 2021-09-09 11:10:54.000000 npdtools-0.1a5/npdtools.egg-info/top_level.txt
--rw-r--r--   0 white     (1000) white     (1000)       38 2021-09-09 11:10:54.984191 npdtools-0.1a5/setup.cfg
--rw-r--r--   0 white     (1000) white     (1000)      906 2021-09-09 11:10:49.000000 npdtools-0.1a5/setup.py
+drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2023-07-09 13:50:10.045077 npdtools-1.0a1/
+-rw-r--r--   0 white     (1000) wjite     (1001)    16725 2021-06-06 10:07:23.000000 npdtools-1.0a1/LICENSE
+-rw-r--r--   0 white     (1000) wjite     (1001)    11342 2023-07-09 13:50:10.045077 npdtools-1.0a1/PKG-INFO
+-rw-r--r--   0 white     (1000) wjite     (1001)    10788 2023-07-09 13:45:12.000000 npdtools-1.0a1/README.md
+drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2023-07-09 13:50:10.041743 npdtools-1.0a1/npdtools/
+-rw-r--r--   0 white     (1000) wjite     (1001)       51 2023-07-09 12:34:14.000000 npdtools-1.0a1/npdtools/__init__.py
+drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2023-07-09 13:50:10.045077 npdtools-1.0a1/npdtools/errors/
+-rw-r--r--   0 white     (1000) wjite     (1001)      494 2023-07-09 12:34:14.000000 npdtools-1.0a1/npdtools/errors/FNSError.py
+-rw-r--r--   0 white     (1000) wjite     (1001)       46 2021-05-15 04:12:30.000000 npdtools-1.0a1/npdtools/errors/__init__.py
+-rw-r--r--   0 white     (1000) wjite     (1001)      149 2023-07-09 12:44:17.000000 npdtools-1.0a1/npdtools/helpers.py
+-rw-r--r--   0 white     (1000) wjite     (1001)      114 2023-07-09 08:05:30.000000 npdtools-1.0a1/npdtools/settings.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     3627 2023-07-09 08:49:31.000000 npdtools-1.0a1/npdtools/token_manager.py
+drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2023-07-09 13:50:10.045077 npdtools-1.0a1/npdtools/types/
+-rw-r--r--   0 white     (1000) wjite     (1001)      392 2023-07-09 12:34:39.000000 npdtools-1.0a1/npdtools/types/__init__.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     1738 2023-07-09 12:33:56.000000 npdtools-1.0a1/npdtools/types/entity.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     4622 2023-07-09 12:34:39.000000 npdtools-1.0a1/npdtools/types/income.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     5346 2023-07-09 13:29:22.000000 npdtools-1.0a1/npdtools/types/invoice.py
+-rw-r--r--   0 white     (1000) wjite     (1001)      560 2023-07-09 12:44:58.000000 npdtools-1.0a1/npdtools/types/service.py
+drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2023-07-09 13:50:10.045077 npdtools-1.0a1/npdtools.egg-info/
+-rw-r--r--   0 white     (1000) wjite     (1001)    11342 2023-07-09 13:50:10.000000 npdtools-1.0a1/npdtools.egg-info/PKG-INFO
+-rw-r--r--   0 white     (1000) wjite     (1001)      458 2023-07-09 13:50:10.000000 npdtools-1.0a1/npdtools.egg-info/SOURCES.txt
+-rw-r--r--   0 white     (1000) wjite     (1001)        1 2023-07-09 13:50:10.000000 npdtools-1.0a1/npdtools.egg-info/dependency_links.txt
+-rw-r--r--   0 white     (1000) wjite     (1001)       45 2023-07-09 13:50:10.000000 npdtools-1.0a1/npdtools.egg-info/requires.txt
+-rw-r--r--   0 white     (1000) wjite     (1001)        9 2023-07-09 13:50:10.000000 npdtools-1.0a1/npdtools.egg-info/top_level.txt
+-rw-r--r--   0 white     (1000) wjite     (1001)       38 2023-07-09 13:50:10.045077 npdtools-1.0a1/setup.cfg
+-rw-r--r--   0 white     (1000) wjite     (1001)      917 2023-07-09 13:48:43.000000 npdtools-1.0a1/setup.py
```

### Comparing `npdtools-0.1a5/LICENSE` & `npdtools-1.0a1/LICENSE`

 * *Files identical despite different names*

