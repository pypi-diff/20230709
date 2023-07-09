# Comparing `tmp/seunggabi_core_python-0.7.0.tar.gz` & `tmp/seunggabi_core_python-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seunggabi_core_python-0.7.0.tar", last modified: Sun Jul  9 04:59:23 2023, max compression
+gzip compressed data, was "seunggabi_core_python-0.8.0.tar", last modified: Sun Jul  9 13:54:39 2023, max compression
```

## Comparing `seunggabi_core_python-0.7.0.tar` & `seunggabi_core_python-0.8.0.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-07-09 04:59:23.169787 seunggabi_core_python-0.7.0/
--rw-r--r--   0 seunggabi   (501) staff       (20)     1070 2023-05-13 14:31:33.000000 seunggabi_core_python-0.7.0/LICENSE
--rw-r--r--   0 seunggabi   (501) staff       (20)      573 2023-07-09 04:59:23.169671 seunggabi_core_python-0.7.0/PKG-INFO
--rw-r--r--   0 seunggabi   (501) staff       (20)      366 2023-07-08 06:47:51.000000 seunggabi_core_python-0.7.0/README.md
--rw-r--r--   0 seunggabi   (501) staff       (20)       38 2023-07-09 04:59:23.169818 seunggabi_core_python-0.7.0/setup.cfg
--rw-r--r--   0 seunggabi   (501) staff       (20)      821 2023-07-08 08:02:23.000000 seunggabi_core_python-0.7.0/setup.py
-drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-07-09 04:59:23.165898 seunggabi_core_python-0.7.0/seunggabi_core_python/
--rw-r--r--   0 seunggabi   (501) staff       (20)       22 2023-07-09 04:59:20.000000 seunggabi_core_python-0.7.0/seunggabi_core_python/__init__.py
--rw-r--r--   0 seunggabi   (501) staff       (20)       48 2023-05-15 13:10:17.000000 seunggabi_core_python-0.7.0/seunggabi_core_python/const.py
-drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-07-09 04:59:23.167091 seunggabi_core_python-0.7.0/seunggabi_core_python/exception/
--rw-r--r--   0 seunggabi   (501) staff       (20)        0 2023-05-15 12:46:34.000000 seunggabi_core_python-0.7.0/seunggabi_core_python/exception/__init__.py
--rw-r--r--   0 seunggabi   (501) staff       (20)      143 2023-06-11 18:12:39.000000 seunggabi_core_python-0.7.0/seunggabi_core_python/exception/bad_request.py
--rw-r--r--   0 seunggabi   (501) staff       (20)      139 2023-06-11 18:12:39.000000 seunggabi_core_python-0.7.0/seunggabi_core_python/exception/not_found.py
-drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-07-09 04:59:23.169515 seunggabi_core_python-0.7.0/seunggabi_core_python/util/
--rw-r--r--   0 seunggabi   (501) staff       (20)        0 2023-05-13 15:22:13.000000 seunggabi_core_python-0.7.0/seunggabi_core_python/util/__init__.py
--rw-r--r--   0 seunggabi   (501) staff       (20)     1001 2023-05-18 14:08:20.000000 seunggabi_core_python-0.7.0/seunggabi_core_python/util/arg_util.py
--rw-r--r--   0 seunggabi   (501) staff       (20)      458 2023-07-08 06:46:01.000000 seunggabi_core_python-0.7.0/seunggabi_core_python/util/bs_util.py
--rw-r--r--   0 seunggabi   (501) staff       (20)      915 2023-06-11 18:11:25.000000 seunggabi_core_python-0.7.0/seunggabi_core_python/util/config_util.py
--rw-r--r--   0 seunggabi   (501) staff       (20)      157 2023-07-08 08:05:53.000000 seunggabi_core_python-0.7.0/seunggabi_core_python/util/dependency_util.py
--rw-r--r--   0 seunggabi   (501) staff       (20)      210 2023-07-08 14:10:08.000000 seunggabi_core_python-0.7.0/seunggabi_core_python/util/json_util.py
--rw-r--r--   0 seunggabi   (501) staff       (20)      802 2023-07-08 16:18:14.000000 seunggabi_core_python-0.7.0/seunggabi_core_python/util/mysql_util.py
--rw-r--r--   0 seunggabi   (501) staff       (20)      219 2023-07-08 06:24:47.000000 seunggabi_core_python-0.7.0/seunggabi_core_python/util/obj_util.py
--rw-r--r--   0 seunggabi   (501) staff       (20)      271 2023-07-08 06:46:01.000000 seunggabi_core_python-0.7.0/seunggabi_core_python/util/request_util.py
--rw-r--r--   0 seunggabi   (501) staff       (20)       54 2023-07-09 04:58:59.000000 seunggabi_core_python-0.7.0/seunggabi_core_python/util/str_util.py
-drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-07-09 04:59:23.166576 seunggabi_core_python-0.7.0/seunggabi_core_python.egg-info/
--rw-r--r--   0 seunggabi   (501) staff       (20)      573 2023-07-09 04:59:23.000000 seunggabi_core_python-0.7.0/seunggabi_core_python.egg-info/PKG-INFO
--rw-r--r--   0 seunggabi   (501) staff       (20)      857 2023-07-09 04:59:23.000000 seunggabi_core_python-0.7.0/seunggabi_core_python.egg-info/SOURCES.txt
--rw-r--r--   0 seunggabi   (501) staff       (20)        1 2023-07-09 04:59:23.000000 seunggabi_core_python-0.7.0/seunggabi_core_python.egg-info/dependency_links.txt
--rw-r--r--   0 seunggabi   (501) staff       (20)       44 2023-07-09 04:59:23.000000 seunggabi_core_python-0.7.0/seunggabi_core_python.egg-info/requires.txt
--rw-r--r--   0 seunggabi   (501) staff       (20)       22 2023-07-09 04:59:23.000000 seunggabi_core_python-0.7.0/seunggabi_core_python.egg-info/top_level.txt
+drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-07-09 13:54:39.528636 seunggabi_core_python-0.8.0/
+-rw-r--r--   0 seunggabi   (501) staff       (20)     1070 2023-05-13 14:31:33.000000 seunggabi_core_python-0.8.0/LICENSE
+-rw-r--r--   0 seunggabi   (501) staff       (20)      573 2023-07-09 13:54:39.528422 seunggabi_core_python-0.8.0/PKG-INFO
+-rw-r--r--   0 seunggabi   (501) staff       (20)      366 2023-07-08 06:47:51.000000 seunggabi_core_python-0.8.0/README.md
+-rw-r--r--   0 seunggabi   (501) staff       (20)       38 2023-07-09 13:54:39.528690 seunggabi_core_python-0.8.0/setup.cfg
+-rw-r--r--   0 seunggabi   (501) staff       (20)      821 2023-07-08 08:02:23.000000 seunggabi_core_python-0.8.0/setup.py
+drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-07-09 13:54:39.523908 seunggabi_core_python-0.8.0/seunggabi_core_python/
+-rw-r--r--   0 seunggabi   (501) staff       (20)       22 2023-07-09 13:54:36.000000 seunggabi_core_python-0.8.0/seunggabi_core_python/__init__.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)       48 2023-05-15 13:10:17.000000 seunggabi_core_python-0.8.0/seunggabi_core_python/const.py
+drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-07-09 13:54:39.525096 seunggabi_core_python-0.8.0/seunggabi_core_python/exception/
+-rw-r--r--   0 seunggabi   (501) staff       (20)        0 2023-05-15 12:46:34.000000 seunggabi_core_python-0.8.0/seunggabi_core_python/exception/__init__.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)      143 2023-06-11 18:12:39.000000 seunggabi_core_python-0.8.0/seunggabi_core_python/exception/bad_request.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)      139 2023-06-11 18:12:39.000000 seunggabi_core_python-0.8.0/seunggabi_core_python/exception/not_found.py
+drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-07-09 13:54:39.527890 seunggabi_core_python-0.8.0/seunggabi_core_python/util/
+-rw-r--r--   0 seunggabi   (501) staff       (20)        0 2023-05-13 15:22:13.000000 seunggabi_core_python-0.8.0/seunggabi_core_python/util/__init__.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)     1001 2023-05-18 14:08:20.000000 seunggabi_core_python-0.8.0/seunggabi_core_python/util/arg_util.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)      458 2023-07-08 06:46:01.000000 seunggabi_core_python-0.8.0/seunggabi_core_python/util/bs_util.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)      915 2023-06-11 18:11:25.000000 seunggabi_core_python-0.8.0/seunggabi_core_python/util/config_util.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)      111 2023-07-09 13:41:53.000000 seunggabi_core_python-0.8.0/seunggabi_core_python/util/date_util.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)      157 2023-07-08 08:05:53.000000 seunggabi_core_python-0.8.0/seunggabi_core_python/util/dependency_util.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)      294 2023-07-09 13:54:04.000000 seunggabi_core_python-0.8.0/seunggabi_core_python/util/file_util.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)      210 2023-07-08 14:10:08.000000 seunggabi_core_python-0.8.0/seunggabi_core_python/util/json_util.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)      802 2023-07-08 16:18:14.000000 seunggabi_core_python-0.8.0/seunggabi_core_python/util/mysql_util.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)      219 2023-07-08 06:24:47.000000 seunggabi_core_python-0.8.0/seunggabi_core_python/util/obj_util.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)      271 2023-07-08 06:46:01.000000 seunggabi_core_python-0.8.0/seunggabi_core_python/util/request_util.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)       54 2023-07-09 04:58:59.000000 seunggabi_core_python-0.8.0/seunggabi_core_python/util/str_util.py
+drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-07-09 13:54:39.524601 seunggabi_core_python-0.8.0/seunggabi_core_python.egg-info/
+-rw-r--r--   0 seunggabi   (501) staff       (20)      573 2023-07-09 13:54:39.000000 seunggabi_core_python-0.8.0/seunggabi_core_python.egg-info/PKG-INFO
+-rw-r--r--   0 seunggabi   (501) staff       (20)      937 2023-07-09 13:54:39.000000 seunggabi_core_python-0.8.0/seunggabi_core_python.egg-info/SOURCES.txt
+-rw-r--r--   0 seunggabi   (501) staff       (20)        1 2023-07-09 13:54:39.000000 seunggabi_core_python-0.8.0/seunggabi_core_python.egg-info/dependency_links.txt
+-rw-r--r--   0 seunggabi   (501) staff       (20)       44 2023-07-09 13:54:39.000000 seunggabi_core_python-0.8.0/seunggabi_core_python.egg-info/requires.txt
+-rw-r--r--   0 seunggabi   (501) staff       (20)       22 2023-07-09 13:54:39.000000 seunggabi_core_python-0.8.0/seunggabi_core_python.egg-info/top_level.txt
```

### Comparing `seunggabi_core_python-0.7.0/LICENSE` & `seunggabi_core_python-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seunggabi_core_python-0.7.0/PKG-INFO` & `seunggabi_core_python-0.8.0/seunggabi_core_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: seunggabi_core_python
-Version: 0.7.0
+Name: seunggabi-core-python
+Version: 0.8.0
 Summary: A collection of core Python modules
 Home-page: https://github.com/seunggabi/core_python
 Author: seunggabi
 Author-email: seunggabi@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `seunggabi_core_python-0.7.0/setup.py` & `seunggabi_core_python-0.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `seunggabi_core_python-0.7.0/seunggabi_core_python/util/arg_util.py` & `seunggabi_core_python-0.8.0/seunggabi_core_python/util/arg_util.py`

 * *Files identical despite different names*

### Comparing `seunggabi_core_python-0.7.0/seunggabi_core_python/util/config_util.py` & `seunggabi_core_python-0.8.0/seunggabi_core_python/util/config_util.py`

 * *Files identical despite different names*

### Comparing `seunggabi_core_python-0.7.0/seunggabi_core_python/util/mysql_util.py` & `seunggabi_core_python-0.8.0/seunggabi_core_python/util/mysql_util.py`

 * *Files identical despite different names*

### Comparing `seunggabi_core_python-0.7.0/seunggabi_core_python.egg-info/PKG-INFO` & `seunggabi_core_python-0.8.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: seunggabi-core-python
-Version: 0.7.0
+Name: seunggabi_core_python
+Version: 0.8.0
 Summary: A collection of core Python modules
 Home-page: https://github.com/seunggabi/core_python
 Author: seunggabi
 Author-email: seunggabi@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `seunggabi_core_python-0.7.0/seunggabi_core_python.egg-info/SOURCES.txt` & `seunggabi_core_python-0.8.0/seunggabi_core_python.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -11,13 +11,15 @@
 seunggabi_core_python/exception/__init__.py
 seunggabi_core_python/exception/bad_request.py
 seunggabi_core_python/exception/not_found.py
 seunggabi_core_python/util/__init__.py
 seunggabi_core_python/util/arg_util.py
 seunggabi_core_python/util/bs_util.py
 seunggabi_core_python/util/config_util.py
+seunggabi_core_python/util/date_util.py
 seunggabi_core_python/util/dependency_util.py
+seunggabi_core_python/util/file_util.py
 seunggabi_core_python/util/json_util.py
 seunggabi_core_python/util/mysql_util.py
 seunggabi_core_python/util/obj_util.py
 seunggabi_core_python/util/request_util.py
 seunggabi_core_python/util/str_util.py
```

