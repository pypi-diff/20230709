# Comparing `tmp/plugen-0.9.tar.gz` & `tmp/plugen-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plugen-0.9.tar", last modified: Sun Jul  9 18:37:41 2023, max compression
+gzip compressed data, was "plugen-1.0.0.tar", last modified: Sun Jul  9 18:54:13 2023, max compression
```

## Comparing `plugen-0.9.tar` & `plugen-1.0.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:37:41.682520 plugen-0.9/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      213 2023-07-09 18:37:41.682520 plugen-0.9/PKG-INFO
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     4400 2023-07-09 05:15:38.000000 plugen-0.9/README.md
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:37:41.678520 plugen-0.9/plugen/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-0.9/plugen/__init__.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:37:41.682520 plugen-0.9/plugen/lib/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       41 2023-07-09 05:59:38.000000 plugen-0.9/plugen/lib/__init__.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      942 2023-07-09 18:33:02.000000 plugen-0.9/plugen/lib/build.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     1984 2023-07-09 18:37:36.000000 plugen-0.9/plugen/lib/plugin.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     2526 2023-07-09 18:33:02.000000 plugen-0.9/plugen/lib/serve.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      522 2023-07-09 09:14:03.000000 plugen-0.9/plugen/lib/utils.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     1742 2023-07-09 18:34:51.000000 plugen-0.9/plugen/main.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:37:41.682520 plugen-0.9/plugen/plugins/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-0.9/plugen/plugins/__init__.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:37:41.682520 plugen-0.9/plugen/plugins/copydest/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-0.9/plugen/plugins/copydest/__init__.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      362 2023-07-09 09:15:39.000000 plugen-0.9/plugen/plugins/copydest/plugin.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:37:41.682520 plugen-0.9/plugen/plugins/hotreload/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-0.9/plugen/plugins/hotreload/__init__.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     1820 2023-07-09 09:36:13.000000 plugen-0.9/plugen/plugins/hotreload/plugin.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:37:41.682520 plugen-0.9/plugen/plugins/imagecompressor/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-0.9/plugen/plugins/imagecompressor/__init__.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      212 2023-07-09 06:47:18.000000 plugen-0.9/plugen/plugins/imagecompressor/plugin.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:37:41.682520 plugen-0.9/plugen/plugins/sass/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-0.9/plugen/plugins/sass/__init__.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      534 2023-07-09 10:19:25.000000 plugen-0.9/plugen/plugins/sass/plugin.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:37:41.682520 plugen-0.9/plugen/plugins/tailwind/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-0.9/plugen/plugins/tailwind/__init__.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      212 2023-07-09 06:47:22.000000 plugen-0.9/plugen/plugins/tailwind/plugin.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:37:41.682520 plugen-0.9/plugen.egg-info/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      213 2023-07-09 18:37:41.000000 plugen-0.9/plugen.egg-info/PKG-INFO
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      771 2023-07-09 18:37:41.000000 plugen-0.9/plugen.egg-info/SOURCES.txt
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        1 2023-07-09 18:37:41.000000 plugen-0.9/plugen.egg-info/dependency_links.txt
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       39 2023-07-09 18:37:41.000000 plugen-0.9/plugen.egg-info/entry_points.txt
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        5 2023-07-09 18:37:41.000000 plugen-0.9/plugen.egg-info/requires.txt
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        7 2023-07-09 18:37:41.000000 plugen-0.9/plugen.egg-info/top_level.txt
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       38 2023-07-09 18:37:41.682520 plugen-0.9/setup.cfg
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      477 2023-07-09 18:37:39.000000 plugen-0.9/setup.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:54:13.612508 plugen-1.0.0/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      215 2023-07-09 18:54:13.612508 plugen-1.0.0/PKG-INFO
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     4400 2023-07-09 05:15:38.000000 plugen-1.0.0/README.md
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:54:13.612508 plugen-1.0.0/plugen/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.0.0/plugen/__init__.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:54:13.612508 plugen-1.0.0/plugen/lib/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       41 2023-07-09 05:59:38.000000 plugen-1.0.0/plugen/lib/__init__.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      942 2023-07-09 18:33:02.000000 plugen-1.0.0/plugen/lib/build.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     1968 2023-07-09 18:38:01.000000 plugen-1.0.0/plugen/lib/plugin.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     2526 2023-07-09 18:33:02.000000 plugen-1.0.0/plugen/lib/serve.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      522 2023-07-09 09:14:03.000000 plugen-1.0.0/plugen/lib/utils.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     1742 2023-07-09 18:34:51.000000 plugen-1.0.0/plugen/main.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:54:13.612508 plugen-1.0.0/plugen/plugins/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.0.0/plugen/plugins/__init__.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:54:13.612508 plugen-1.0.0/plugen/plugins/copydest/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.0.0/plugen/plugins/copydest/__init__.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      362 2023-07-09 09:15:39.000000 plugen-1.0.0/plugen/plugins/copydest/plugin.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:54:13.612508 plugen-1.0.0/plugen/plugins/hotreload/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.0.0/plugen/plugins/hotreload/__init__.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     1820 2023-07-09 09:36:13.000000 plugen-1.0.0/plugen/plugins/hotreload/plugin.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:54:13.612508 plugen-1.0.0/plugen/plugins/imagecompressor/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.0.0/plugen/plugins/imagecompressor/__init__.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      212 2023-07-09 06:47:18.000000 plugen-1.0.0/plugen/plugins/imagecompressor/plugin.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:54:13.612508 plugen-1.0.0/plugen/plugins/sass/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.0.0/plugen/plugins/sass/__init__.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      534 2023-07-09 10:19:25.000000 plugen-1.0.0/plugen/plugins/sass/plugin.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:54:13.612508 plugen-1.0.0/plugen/plugins/tailwind/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.0.0/plugen/plugins/tailwind/__init__.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      212 2023-07-09 06:47:22.000000 plugen-1.0.0/plugen/plugins/tailwind/plugin.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:54:13.612508 plugen-1.0.0/plugen.egg-info/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      215 2023-07-09 18:54:13.000000 plugen-1.0.0/plugen.egg-info/PKG-INFO
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      771 2023-07-09 18:54:13.000000 plugen-1.0.0/plugen.egg-info/SOURCES.txt
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        1 2023-07-09 18:54:13.000000 plugen-1.0.0/plugen.egg-info/dependency_links.txt
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       39 2023-07-09 18:54:13.000000 plugen-1.0.0/plugen.egg-info/entry_points.txt
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        5 2023-07-09 18:54:13.000000 plugen-1.0.0/plugen.egg-info/requires.txt
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        7 2023-07-09 18:54:13.000000 plugen-1.0.0/plugen.egg-info/top_level.txt
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       38 2023-07-09 18:54:13.612508 plugen-1.0.0/setup.cfg
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      479 2023-07-09 18:54:11.000000 plugen-1.0.0/setup.py
```

### Comparing `plugen-0.9/README.md` & `plugen-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `plugen-0.9/plugen/lib/build.py` & `plugen-1.0.0/plugen/lib/build.py`

 * *Files identical despite different names*

### Comparing `plugen-0.9/plugen/lib/plugin.py` & `plugen-1.0.0/plugen/lib/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from pathlib import Path
 from pydoc import importfile
 from urllib import request
 
 
 def plugin_instances(config):
     instances = []
-    print('oo')
 
     print('Initializing plugins')
     for plugin_config in config['plugins']:
         print('  ' + plugin_config['name'])
         path = Path(__file__).resolve().parent.parent.joinpath(
             'plugins/{0}/plugin.py'.format(str(plugin_config['name']))
         )
```

### Comparing `plugen-0.9/plugen/lib/serve.py` & `plugen-1.0.0/plugen/lib/serve.py`

 * *Files identical despite different names*

### Comparing `plugen-0.9/plugen/lib/utils.py` & `plugen-1.0.0/plugen/lib/utils.py`

 * *Files identical despite different names*

### Comparing `plugen-0.9/plugen/main.py` & `plugen-1.0.0/plugen/main.py`

 * *Files identical despite different names*

### Comparing `plugen-0.9/plugen/plugins/hotreload/plugin.py` & `plugen-1.0.0/plugen/plugins/hotreload/plugin.py`

 * *Files identical despite different names*

### Comparing `plugen-0.9/plugen/plugins/sass/plugin.py` & `plugen-1.0.0/plugen/plugins/sass/plugin.py`

 * *Files identical despite different names*

### Comparing `plugen-0.9/plugen.egg-info/SOURCES.txt` & `plugen-1.0.0/plugen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

