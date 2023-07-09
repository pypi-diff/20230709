# Comparing `tmp/plugen-0.6.tar.gz` & `tmp/plugen-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plugen-0.6.tar", last modified: Sun Jul  9 18:20:57 2023, max compression
+gzip compressed data, was "plugen-0.7.tar", last modified: Sun Jul  9 18:27:07 2023, max compression
```

## Comparing `plugen-0.6.tar` & `plugen-0.7.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:20:57.482743 plugen-0.6/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      213 2023-07-09 18:20:57.482743 plugen-0.6/PKG-INFO
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     4400 2023-07-09 05:15:38.000000 plugen-0.6/README.md
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:20:57.482743 plugen-0.6/lib/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       41 2023-07-09 05:59:38.000000 plugen-0.6/lib/__init__.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      928 2023-07-09 14:11:26.000000 plugen-0.6/lib/build.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     2054 2023-07-09 14:43:08.000000 plugen-0.6/lib/plugin.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     2512 2023-07-09 14:11:26.000000 plugen-0.6/lib/serve.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      522 2023-07-09 09:14:03.000000 plugen-0.6/lib/utils.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:20:57.482743 plugen-0.6/plugen.egg-info/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      213 2023-07-09 18:20:57.000000 plugen-0.6/plugen.egg-info/PKG-INFO
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      225 2023-07-09 18:20:57.000000 plugen-0.6/plugen.egg-info/SOURCES.txt
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        1 2023-07-09 18:20:57.000000 plugen-0.6/plugen.egg-info/dependency_links.txt
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        4 2023-07-09 18:20:57.000000 plugen-0.6/plugen.egg-info/top_level.txt
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       38 2023-07-09 18:20:57.482743 plugen-0.6/setup.cfg
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      369 2023-07-09 18:16:58.000000 plugen-0.6/setup.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:27:07.944902 plugen-0.7/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      213 2023-07-09 18:27:07.944902 plugen-0.7/PKG-INFO
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     4400 2023-07-09 05:15:38.000000 plugen-0.7/README.md
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:27:07.944902 plugen-0.7/lib/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       41 2023-07-09 05:59:38.000000 plugen-0.7/lib/__init__.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      928 2023-07-09 14:11:26.000000 plugen-0.7/lib/build.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     2054 2023-07-09 14:43:08.000000 plugen-0.7/lib/plugin.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     2512 2023-07-09 14:11:26.000000 plugen-0.7/lib/serve.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      522 2023-07-09 09:14:03.000000 plugen-0.7/lib/utils.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:27:07.944902 plugen-0.7/plugen.egg-info/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      213 2023-07-09 18:27:07.000000 plugen-0.7/plugen.egg-info/PKG-INFO
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      260 2023-07-09 18:27:07.000000 plugen-0.7/plugen.egg-info/SOURCES.txt
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        1 2023-07-09 18:27:07.000000 plugen-0.7/plugen.egg-info/dependency_links.txt
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       37 2023-07-09 18:27:07.000000 plugen-0.7/plugen.egg-info/entry_points.txt
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        4 2023-07-09 18:27:07.000000 plugen-0.7/plugen.egg-info/top_level.txt
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       38 2023-07-09 18:27:07.944902 plugen-0.7/setup.cfg
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      469 2023-07-09 18:26:39.000000 plugen-0.7/setup.py
```

### Comparing `plugen-0.6/README.md` & `plugen-0.7/README.md`

 * *Files identical despite different names*

### Comparing `plugen-0.6/lib/build.py` & `plugen-0.7/lib/build.py`

 * *Files identical despite different names*

### Comparing `plugen-0.6/lib/plugin.py` & `plugen-0.7/lib/plugin.py`

 * *Files identical despite different names*

### Comparing `plugen-0.6/lib/serve.py` & `plugen-0.7/lib/serve.py`

 * *Files identical despite different names*

### Comparing `plugen-0.6/lib/utils.py` & `plugen-0.7/lib/utils.py`

 * *Files identical despite different names*

