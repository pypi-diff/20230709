# Comparing `tmp/plugen-0.83.tar.gz` & `tmp/plugen-0.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plugen-0.83.tar", last modified: Sun Jul  9 18:35:23 2023, max compression
+gzip compressed data, was "plugen-0.84.tar", last modified: Sun Jul  9 18:35:47 2023, max compression
```

## Comparing `plugen-0.83.tar` & `plugen-0.84.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:35:23.120914 plugen-0.83/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      214 2023-07-09 18:35:23.120914 plugen-0.83/PKG-INFO
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     4400 2023-07-09 05:15:38.000000 plugen-0.83/README.md
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:35:23.120914 plugen-0.83/plugen/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-0.83/plugen/__init__.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:35:23.120914 plugen-0.83/plugen/lib/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       41 2023-07-09 05:59:38.000000 plugen-0.83/plugen/lib/__init__.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      942 2023-07-09 18:33:02.000000 plugen-0.83/plugen/lib/build.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     1968 2023-07-09 18:35:07.000000 plugen-0.83/plugen/lib/plugin.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     2526 2023-07-09 18:33:02.000000 plugen-0.83/plugen/lib/serve.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      522 2023-07-09 09:14:03.000000 plugen-0.83/plugen/lib/utils.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     1742 2023-07-09 18:34:51.000000 plugen-0.83/plugen/main.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:35:23.120914 plugen-0.83/plugen/plugins/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-0.83/plugen/plugins/__init__.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:35:23.120914 plugen-0.83/plugen/plugins/copydest/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-0.83/plugen/plugins/copydest/__init__.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      362 2023-07-09 09:15:39.000000 plugen-0.83/plugen/plugins/copydest/plugin.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:35:23.120914 plugen-0.83/plugen/plugins/hotreload/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-0.83/plugen/plugins/hotreload/__init__.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     1820 2023-07-09 09:36:13.000000 plugen-0.83/plugen/plugins/hotreload/plugin.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:35:23.120914 plugen-0.83/plugen/plugins/imagecompressor/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-0.83/plugen/plugins/imagecompressor/__init__.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      212 2023-07-09 06:47:18.000000 plugen-0.83/plugen/plugins/imagecompressor/plugin.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:35:23.120914 plugen-0.83/plugen/plugins/sass/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-0.83/plugen/plugins/sass/__init__.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      534 2023-07-09 10:19:25.000000 plugen-0.83/plugen/plugins/sass/plugin.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:35:23.120914 plugen-0.83/plugen/plugins/tailwind/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-0.83/plugen/plugins/tailwind/__init__.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      212 2023-07-09 06:47:22.000000 plugen-0.83/plugen/plugins/tailwind/plugin.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:35:23.120914 plugen-0.83/plugen.egg-info/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      214 2023-07-09 18:35:23.000000 plugen-0.83/plugen.egg-info/PKG-INFO
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      740 2023-07-09 18:35:23.000000 plugen-0.83/plugen.egg-info/SOURCES.txt
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        1 2023-07-09 18:35:23.000000 plugen-0.83/plugen.egg-info/dependency_links.txt
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       39 2023-07-09 18:35:23.000000 plugen-0.83/plugen.egg-info/entry_points.txt
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        7 2023-07-09 18:35:23.000000 plugen-0.83/plugen.egg-info/top_level.txt
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       38 2023-07-09 18:35:23.120914 plugen-0.83/setup.cfg
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      472 2023-07-09 18:35:16.000000 plugen-0.83/setup.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:35:47.929164 plugen-0.84/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      214 2023-07-09 18:35:47.929164 plugen-0.84/PKG-INFO
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     4400 2023-07-09 05:15:38.000000 plugen-0.84/README.md
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:35:47.925164 plugen-0.84/plugen/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-0.84/plugen/__init__.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:35:47.925164 plugen-0.84/plugen/lib/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       41 2023-07-09 05:59:38.000000 plugen-0.84/plugen/lib/__init__.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      942 2023-07-09 18:33:02.000000 plugen-0.84/plugen/lib/build.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     1968 2023-07-09 18:35:07.000000 plugen-0.84/plugen/lib/plugin.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     2526 2023-07-09 18:33:02.000000 plugen-0.84/plugen/lib/serve.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      522 2023-07-09 09:14:03.000000 plugen-0.84/plugen/lib/utils.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     1742 2023-07-09 18:34:51.000000 plugen-0.84/plugen/main.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:35:47.925164 plugen-0.84/plugen/plugins/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-0.84/plugen/plugins/__init__.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:35:47.925164 plugen-0.84/plugen/plugins/copydest/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-0.84/plugen/plugins/copydest/__init__.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      362 2023-07-09 09:15:39.000000 plugen-0.84/plugen/plugins/copydest/plugin.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:35:47.925164 plugen-0.84/plugen/plugins/hotreload/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-0.84/plugen/plugins/hotreload/__init__.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     1820 2023-07-09 09:36:13.000000 plugen-0.84/plugen/plugins/hotreload/plugin.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:35:47.925164 plugen-0.84/plugen/plugins/imagecompressor/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-0.84/plugen/plugins/imagecompressor/__init__.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      212 2023-07-09 06:47:18.000000 plugen-0.84/plugen/plugins/imagecompressor/plugin.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:35:47.929164 plugen-0.84/plugen/plugins/sass/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-0.84/plugen/plugins/sass/__init__.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      534 2023-07-09 10:19:25.000000 plugen-0.84/plugen/plugins/sass/plugin.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:35:47.929164 plugen-0.84/plugen/plugins/tailwind/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-0.84/plugen/plugins/tailwind/__init__.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      212 2023-07-09 06:47:22.000000 plugen-0.84/plugen/plugins/tailwind/plugin.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:35:47.925164 plugen-0.84/plugen.egg-info/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      214 2023-07-09 18:35:47.000000 plugen-0.84/plugen.egg-info/PKG-INFO
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      771 2023-07-09 18:35:47.000000 plugen-0.84/plugen.egg-info/SOURCES.txt
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        1 2023-07-09 18:35:47.000000 plugen-0.84/plugen.egg-info/dependency_links.txt
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       39 2023-07-09 18:35:47.000000 plugen-0.84/plugen.egg-info/entry_points.txt
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        5 2023-07-09 18:35:47.000000 plugen-0.84/plugen.egg-info/requires.txt
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        7 2023-07-09 18:35:47.000000 plugen-0.84/plugen.egg-info/top_level.txt
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       38 2023-07-09 18:35:47.929164 plugen-0.84/setup.cfg
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      478 2023-07-09 18:35:46.000000 plugen-0.84/setup.py
```

### Comparing `plugen-0.83/README.md` & `plugen-0.84/README.md`

 * *Files identical despite different names*

### Comparing `plugen-0.83/plugen/lib/build.py` & `plugen-0.84/plugen/lib/build.py`

 * *Files identical despite different names*

### Comparing `plugen-0.83/plugen/lib/plugin.py` & `plugen-0.84/plugen/lib/plugin.py`

 * *Files identical despite different names*

### Comparing `plugen-0.83/plugen/lib/serve.py` & `plugen-0.84/plugen/lib/serve.py`

 * *Files identical despite different names*

### Comparing `plugen-0.83/plugen/lib/utils.py` & `plugen-0.84/plugen/lib/utils.py`

 * *Files identical despite different names*

### Comparing `plugen-0.83/plugen/main.py` & `plugen-0.84/plugen/main.py`

 * *Files identical despite different names*

### Comparing `plugen-0.83/plugen/plugins/hotreload/plugin.py` & `plugen-0.84/plugen/plugins/hotreload/plugin.py`

 * *Files identical despite different names*

### Comparing `plugen-0.83/plugen/plugins/sass/plugin.py` & `plugen-0.84/plugen/plugins/sass/plugin.py`

 * *Files identical despite different names*

### Comparing `plugen-0.83/plugen.egg-info/SOURCES.txt` & `plugen-0.84/plugen.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 setup.py
 ./plugen/__init__.py
 ./plugen/main.py
 ./plugen.egg-info/PKG-INFO
 ./plugen.egg-info/SOURCES.txt
 ./plugen.egg-info/dependency_links.txt
 ./plugen.egg-info/entry_points.txt
+./plugen.egg-info/requires.txt
 ./plugen.egg-info/top_level.txt
 ./plugen/lib/__init__.py
 ./plugen/lib/build.py
 ./plugen/lib/plugin.py
 ./plugen/lib/serve.py
 ./plugen/lib/utils.py
 ./plugen/plugins/__init__.py
```

