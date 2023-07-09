# Comparing `tmp/shubhlipi-0.0.0.17.tar.gz` & `tmp/shubhlipi-0.0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shubhlipi-0.0.0.17.tar", last modified: Mon Feb 27 14:07:26 2023, max compression
+gzip compressed data, was "shubhlipi-0.0.0.18.tar", last modified: Sun Jul  9 04:27:19 2023, max compression
```

## Comparing `shubhlipi-0.0.0.17.tar` & `shubhlipi-0.0.0.18.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 shubhattin  (1000) shubhattin  (1000)        0 2023-02-27 14:07:26.302685 shubhlipi-0.0.0.17/
--rw-r--r--   0 shubhattin  (1000) shubhattin  (1000)       79 2023-02-27 14:07:26.302685 shubhlipi-0.0.0.17/PKG-INFO
--rw-r--r--   0 shubhattin  (1000) shubhattin  (1000)       38 2023-02-27 14:07:26.302685 shubhlipi-0.0.0.17/setup.cfg
--rw-r--r--   0 shubhattin  (1000) shubhattin  (1000)      190 2023-02-27 14:07:24.000000 shubhlipi-0.0.0.17/setup.py
-drwxr-xr-x   0 shubhattin  (1000) shubhattin  (1000)        0 2023-02-27 14:07:26.302685 shubhlipi-0.0.0.17/shubhlipi/
--rw-r--r--   0 shubhattin  (1000) shubhattin  (1000)      241 2023-02-27 13:43:36.000000 shubhlipi-0.0.0.17/shubhlipi/__init__.py
--rw-r--r--   0 shubhattin  (1000) shubhattin  (1000)      923 2023-02-27 13:43:36.000000 shubhlipi-0.0.0.17/shubhlipi/crypted.py
--rw-r--r--   0 shubhattin  (1000) shubhattin  (1000)     4032 2023-02-27 13:43:36.000000 shubhlipi-0.0.0.17/shubhlipi/file.py
--rw-r--r--   0 shubhattin  (1000) shubhattin  (1000)     3176 2023-02-27 13:43:36.000000 shubhlipi-0.0.0.17/shubhlipi/git.py
--rw-r--r--   0 shubhattin  (1000) shubhattin  (1000)     5195 2023-02-27 13:43:36.000000 shubhlipi-0.0.0.17/shubhlipi/json.py
--rw-r--r--   0 shubhattin  (1000) shubhattin  (1000)     1091 2023-02-27 14:06:49.000000 shubhlipi-0.0.0.17/shubhlipi/kry.py
--rw-r--r--   0 shubhattin  (1000) shubhattin  (1000)     1723 2023-02-27 13:43:36.000000 shubhlipi-0.0.0.17/shubhlipi/lang_list.py
--rw-r--r--   0 shubhattin  (1000) shubhattin  (1000)     3122 2023-02-27 13:43:36.000000 shubhlipi-0.0.0.17/shubhlipi/min.py
--rw-r--r--   0 shubhattin  (1000) shubhattin  (1000)     1861 2023-02-27 13:43:36.000000 shubhlipi-0.0.0.17/shubhlipi/sign.py
--rw-r--r--   0 shubhattin  (1000) shubhattin  (1000)     1771 2023-02-27 13:43:36.000000 shubhlipi-0.0.0.17/shubhlipi/trans.py
-drwxr-xr-x   0 shubhattin  (1000) shubhattin  (1000)        0 2023-02-27 14:07:26.302685 shubhlipi-0.0.0.17/shubhlipi.egg-info/
--rw-r--r--   0 shubhattin  (1000) shubhattin  (1000)       79 2023-02-27 14:07:26.000000 shubhlipi-0.0.0.17/shubhlipi.egg-info/PKG-INFO
--rw-r--r--   0 shubhattin  (1000) shubhattin  (1000)      362 2023-02-27 14:07:26.000000 shubhlipi-0.0.0.17/shubhlipi.egg-info/SOURCES.txt
--rw-r--r--   0 shubhattin  (1000) shubhattin  (1000)        1 2023-02-27 14:07:26.000000 shubhlipi-0.0.0.17/shubhlipi.egg-info/dependency_links.txt
--rw-r--r--   0 shubhattin  (1000) shubhattin  (1000)       19 2023-02-27 14:07:26.000000 shubhlipi-0.0.0.17/shubhlipi.egg-info/requires.txt
--rw-r--r--   0 shubhattin  (1000) shubhattin  (1000)       10 2023-02-27 14:07:26.000000 shubhlipi-0.0.0.17/shubhlipi.egg-info/top_level.txt
+drwxr-xr-x   0 shubhattin  (1000) shubhattin  (1000)        0 2023-07-09 04:27:19.973369 shubhlipi-0.0.0.18/
+-rw-r--r--   0 shubhattin  (1000) shubhattin  (1000)       79 2023-07-09 04:27:19.973369 shubhlipi-0.0.0.18/PKG-INFO
+-rw-r--r--   0 shubhattin  (1000) shubhattin  (1000)       38 2023-07-09 04:27:19.973369 shubhlipi-0.0.0.18/setup.cfg
+-rw-r--r--   0 shubhattin  (1000) shubhattin  (1000)      190 2023-07-09 04:25:28.000000 shubhlipi-0.0.0.18/setup.py
+drwxr-xr-x   0 shubhattin  (1000) shubhattin  (1000)        0 2023-07-09 04:27:19.963369 shubhlipi-0.0.0.18/shubhlipi/
+-rw-r--r--   0 shubhattin  (1000) shubhattin  (1000)      241 2023-07-09 04:21:47.000000 shubhlipi-0.0.0.18/shubhlipi/__init__.py
+-rw-r--r--   0 shubhattin  (1000) shubhattin  (1000)      923 2023-07-09 04:21:47.000000 shubhlipi-0.0.0.18/shubhlipi/crypted.py
+-rw-r--r--   0 shubhattin  (1000) shubhattin  (1000)     4032 2023-07-09 04:21:47.000000 shubhlipi-0.0.0.18/shubhlipi/file.py
+-rw-r--r--   0 shubhattin  (1000) shubhattin  (1000)     3305 2023-07-09 04:24:21.000000 shubhlipi-0.0.0.18/shubhlipi/git.py
+-rw-r--r--   0 shubhattin  (1000) shubhattin  (1000)     5195 2023-07-09 04:21:47.000000 shubhlipi-0.0.0.18/shubhlipi/json.py
+-rw-r--r--   0 shubhattin  (1000) shubhattin  (1000)     1091 2023-07-09 04:21:47.000000 shubhlipi-0.0.0.18/shubhlipi/kry.py
+-rw-r--r--   0 shubhattin  (1000) shubhattin  (1000)     1723 2023-07-09 04:21:47.000000 shubhlipi-0.0.0.18/shubhlipi/lang_list.py
+-rw-r--r--   0 shubhattin  (1000) shubhattin  (1000)     3122 2023-07-09 04:21:47.000000 shubhlipi-0.0.0.18/shubhlipi/min.py
+-rw-r--r--   0 shubhattin  (1000) shubhattin  (1000)     1861 2023-07-09 04:21:47.000000 shubhlipi-0.0.0.18/shubhlipi/sign.py
+-rw-r--r--   0 shubhattin  (1000) shubhattin  (1000)     1771 2023-07-09 04:21:47.000000 shubhlipi-0.0.0.18/shubhlipi/trans.py
+drwxr-xr-x   0 shubhattin  (1000) shubhattin  (1000)        0 2023-07-09 04:27:19.973369 shubhlipi-0.0.0.18/shubhlipi.egg-info/
+-rw-r--r--   0 shubhattin  (1000) shubhattin  (1000)       79 2023-07-09 04:27:19.000000 shubhlipi-0.0.0.18/shubhlipi.egg-info/PKG-INFO
+-rw-r--r--   0 shubhattin  (1000) shubhattin  (1000)      362 2023-07-09 04:27:19.000000 shubhlipi-0.0.0.18/shubhlipi.egg-info/SOURCES.txt
+-rw-r--r--   0 shubhattin  (1000) shubhattin  (1000)        1 2023-07-09 04:27:19.000000 shubhlipi-0.0.0.18/shubhlipi.egg-info/dependency_links.txt
+-rw-r--r--   0 shubhattin  (1000) shubhattin  (1000)       19 2023-07-09 04:27:19.000000 shubhlipi-0.0.0.18/shubhlipi.egg-info/requires.txt
+-rw-r--r--   0 shubhattin  (1000) shubhattin  (1000)       10 2023-07-09 04:27:19.000000 shubhlipi-0.0.0.18/shubhlipi.egg-info/top_level.txt
```

### Comparing `shubhlipi-0.0.0.17/shubhlipi/crypted.py` & `shubhlipi-0.0.0.18/shubhlipi/crypted.py`

 * *Files identical despite different names*

### Comparing `shubhlipi-0.0.0.17/shubhlipi/file.py` & `shubhlipi-0.0.0.18/shubhlipi/file.py`

 * *Files identical despite different names*

### Comparing `shubhlipi-0.0.0.17/shubhlipi/git.py` & `shubhlipi-0.0.0.18/shubhlipi/git.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,20 @@
     upld=True,
     fl_type=None,
     fl_data=None,
     log=True,
 ):
     if log:
         print("Current File: ", file)
-    file_name = file.split("\\").split("/")[-1].replace(" ", ".")
+    if "/" in file:
+        file_name = file.split("/")[-1].replace(" ", ".")
+    elif "\\" in file:
+        file_name = file.split("\\")[-1].replace(" ", ".")
+    else:
+        file_name = file
     rq = get(
         "https://api.github.com/repos/" + repo + "/releases",
         headers={
             "Authorization": "token " + token,
         },
     )
     if log:
```

### Comparing `shubhlipi-0.0.0.17/shubhlipi/json.py` & `shubhlipi-0.0.0.18/shubhlipi/json.py`

 * *Files identical despite different names*

### Comparing `shubhlipi-0.0.0.17/shubhlipi/kry.py` & `shubhlipi-0.0.0.18/shubhlipi/kry.py`

 * *Files identical despite different names*

### Comparing `shubhlipi-0.0.0.17/shubhlipi/lang_list.py` & `shubhlipi-0.0.0.18/shubhlipi/lang_list.py`

 * *Files identical despite different names*

### Comparing `shubhlipi-0.0.0.17/shubhlipi/min.py` & `shubhlipi-0.0.0.18/shubhlipi/min.py`

 * *Files identical despite different names*

### Comparing `shubhlipi-0.0.0.17/shubhlipi/sign.py` & `shubhlipi-0.0.0.18/shubhlipi/sign.py`

 * *Files identical despite different names*

### Comparing `shubhlipi-0.0.0.17/shubhlipi/trans.py` & `shubhlipi-0.0.0.18/shubhlipi/trans.py`

 * *Files identical despite different names*

