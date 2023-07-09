# Comparing `tmp/imgk-1.0.0.tar.gz` & `tmp/imgk-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/imgk-1.0.0.tar", last modified: Sun Jul  9 03:55:33 2023, max compression
+gzip compressed data, was "dist/imgk-1.0.1.tar", last modified: Sun Jul  9 04:36:36 2023, max compression
```

## Comparing `imgk-1.0.0.tar` & `imgk-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 praveenrathore   (501) staff       (20)        0 2023-07-09 03:55:33.000000 imgk-1.0.0/
--rw-r--r--   0 praveenrathore   (501) staff       (20)      203 2023-07-09 03:55:33.000000 imgk-1.0.0/PKG-INFO
--rw-r--r--   0 praveenrathore   (501) staff       (20)     1609 2023-07-09 03:55:10.000000 imgk-1.0.0/README.md
--rw-r--r--   0 praveenrathore   (501) staff       (20)      244 2023-07-09 03:52:07.000000 imgk-1.0.0/setup.py
-drwxr-xr-x   0 praveenrathore   (501) staff       (20)        0 2023-07-09 03:55:33.000000 imgk-1.0.0/imgk/
--rw-r--r--   0 praveenrathore   (501) staff       (20)      566 2023-07-09 03:07:14.000000 imgk-1.0.0/imgk/__init__.py
--rw-r--r--   0 praveenrathore   (501) staff       (20)      145 2023-07-09 03:09:03.000000 imgk-1.0.0/imgk/utils.py
-drwxr-xr-x   0 praveenrathore   (501) staff       (20)        0 2023-07-09 03:55:33.000000 imgk-1.0.0/imgk/commands/
--rw-r--r--   0 praveenrathore   (501) staff       (20)      436 2023-07-09 03:08:43.000000 imgk-1.0.0/imgk/commands/metadata.py
--rw-r--r--   0 praveenrathore   (501) staff       (20)      632 2023-07-09 03:07:35.000000 imgk-1.0.0/imgk/commands/convert.py
--rw-r--r--   0 praveenrathore   (501) staff       (20)       32 2023-07-09 03:20:48.000000 imgk-1.0.0/imgk/commands/__init__.py
--rw-r--r--   0 praveenrathore   (501) staff       (20)      933 2023-07-09 03:08:23.000000 imgk-1.0.0/imgk/commands/crop.py
--rw-r--r--   0 praveenrathore   (501) staff       (20)      765 2023-07-09 03:08:51.000000 imgk-1.0.0/imgk/commands/resize.py
--rw-r--r--   0 praveenrathore   (501) staff       (20)      693 2023-07-09 03:08:35.000000 imgk-1.0.0/imgk/commands/filter.py
-drwxr-xr-x   0 praveenrathore   (501) staff       (20)        0 2023-07-09 03:55:33.000000 imgk-1.0.0/imgk.egg-info/
--rw-r--r--   0 praveenrathore   (501) staff       (20)      203 2023-07-09 03:55:33.000000 imgk-1.0.0/imgk.egg-info/PKG-INFO
--rw-r--r--   0 praveenrathore   (501) staff       (20)      335 2023-07-09 03:55:33.000000 imgk-1.0.0/imgk.egg-info/SOURCES.txt
--rw-r--r--   0 praveenrathore   (501) staff       (20)        7 2023-07-09 03:55:33.000000 imgk-1.0.0/imgk.egg-info/requires.txt
--rw-r--r--   0 praveenrathore   (501) staff       (20)        5 2023-07-09 03:55:33.000000 imgk-1.0.0/imgk.egg-info/top_level.txt
--rw-r--r--   0 praveenrathore   (501) staff       (20)        1 2023-07-09 03:55:33.000000 imgk-1.0.0/imgk.egg-info/dependency_links.txt
--rw-r--r--   0 praveenrathore   (501) staff       (20)       38 2023-07-09 03:55:33.000000 imgk-1.0.0/setup.cfg
+drwxr-xr-x   0 praveenrathore   (501) staff       (20)        0 2023-07-09 04:36:36.000000 imgk-1.0.1/
+-rw-r--r--   0 praveenrathore   (501) staff       (20)     2361 2023-07-09 04:36:36.000000 imgk-1.0.1/PKG-INFO
+-rw-r--r--   0 praveenrathore   (501) staff       (20)     1609 2023-07-09 03:55:10.000000 imgk-1.0.1/README.md
+-rw-r--r--   0 praveenrathore   (501) staff       (20)      641 2023-07-09 04:36:19.000000 imgk-1.0.1/setup.py
+drwxr-xr-x   0 praveenrathore   (501) staff       (20)        0 2023-07-09 04:36:36.000000 imgk-1.0.1/imgk/
+-rw-r--r--   0 praveenrathore   (501) staff       (20)      566 2023-07-09 03:07:14.000000 imgk-1.0.1/imgk/__init__.py
+-rw-r--r--   0 praveenrathore   (501) staff       (20)      145 2023-07-09 03:09:03.000000 imgk-1.0.1/imgk/utils.py
+drwxr-xr-x   0 praveenrathore   (501) staff       (20)        0 2023-07-09 04:36:36.000000 imgk-1.0.1/imgk/commands/
+-rw-r--r--   0 praveenrathore   (501) staff       (20)      436 2023-07-09 03:08:43.000000 imgk-1.0.1/imgk/commands/metadata.py
+-rw-r--r--   0 praveenrathore   (501) staff       (20)      632 2023-07-09 03:07:35.000000 imgk-1.0.1/imgk/commands/convert.py
+-rw-r--r--   0 praveenrathore   (501) staff       (20)       32 2023-07-09 03:20:48.000000 imgk-1.0.1/imgk/commands/__init__.py
+-rw-r--r--   0 praveenrathore   (501) staff       (20)      933 2023-07-09 03:08:23.000000 imgk-1.0.1/imgk/commands/crop.py
+-rw-r--r--   0 praveenrathore   (501) staff       (20)      765 2023-07-09 03:08:51.000000 imgk-1.0.1/imgk/commands/resize.py
+-rw-r--r--   0 praveenrathore   (501) staff       (20)      693 2023-07-09 03:08:35.000000 imgk-1.0.1/imgk/commands/filter.py
+drwxr-xr-x   0 praveenrathore   (501) staff       (20)        0 2023-07-09 04:36:36.000000 imgk-1.0.1/imgk.egg-info/
+-rw-r--r--   0 praveenrathore   (501) staff       (20)     2361 2023-07-09 04:36:36.000000 imgk-1.0.1/imgk.egg-info/PKG-INFO
+-rw-r--r--   0 praveenrathore   (501) staff       (20)      366 2023-07-09 04:36:36.000000 imgk-1.0.1/imgk.egg-info/SOURCES.txt
+-rw-r--r--   0 praveenrathore   (501) staff       (20)       40 2023-07-09 04:36:36.000000 imgk-1.0.1/imgk.egg-info/entry_points.txt
+-rw-r--r--   0 praveenrathore   (501) staff       (20)        7 2023-07-09 04:36:36.000000 imgk-1.0.1/imgk.egg-info/requires.txt
+-rw-r--r--   0 praveenrathore   (501) staff       (20)        5 2023-07-09 04:36:36.000000 imgk-1.0.1/imgk.egg-info/top_level.txt
+-rw-r--r--   0 praveenrathore   (501) staff       (20)        1 2023-07-09 04:36:36.000000 imgk-1.0.1/imgk.egg-info/dependency_links.txt
+-rw-r--r--   0 praveenrathore   (501) staff       (20)       38 2023-07-09 04:36:36.000000 imgk-1.0.1/setup.cfg
```

### Comparing `imgk-1.0.0/README.md` & `imgk-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `imgk-1.0.0/imgk/__init__.py` & `imgk-1.0.1/imgk/__init__.py`

 * *Files identical despite different names*

### Comparing `imgk-1.0.0/imgk/commands/convert.py` & `imgk-1.0.1/imgk/commands/convert.py`

 * *Files identical despite different names*

### Comparing `imgk-1.0.0/imgk/commands/crop.py` & `imgk-1.0.1/imgk/commands/crop.py`

 * *Files identical despite different names*

### Comparing `imgk-1.0.0/imgk/commands/resize.py` & `imgk-1.0.1/imgk/commands/resize.py`

 * *Files identical despite different names*

### Comparing `imgk-1.0.0/imgk/commands/filter.py` & `imgk-1.0.1/imgk/commands/filter.py`

 * *Files identical despite different names*

