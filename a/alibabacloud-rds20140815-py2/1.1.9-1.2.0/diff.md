# Comparing `tmp/alibabacloud_rds20140815_py2-1.1.9.tar.gz` & `tmp/alibabacloud_rds20140815_py2-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_rds20140815_py2-1.1.9.tar", last modified: Sat Jul  8 15:10:25 2023, max compression
+gzip compressed data, was "dist/alibabacloud_rds20140815_py2-1.2.0.tar", last modified: Sun Jul  9 15:08:01 2023, max compression
```

## Comparing `alibabacloud_rds20140815_py2-1.1.9.tar` & `alibabacloud_rds20140815_py2-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 15:10:25.000000 alibabacloud_rds20140815_py2-1.1.9/
--rw-r--r--   0 root         (0) root         (0)     1579 2023-07-08 15:10:25.000000 alibabacloud_rds20140815_py2-1.1.9/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-07-08 15:10:25.000000 alibabacloud_rds20140815_py2-1.1.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-07-08 15:10:25.000000 alibabacloud_rds20140815_py2-1.1.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2472 2023-07-08 15:10:25.000000 alibabacloud_rds20140815_py2-1.1.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1033 2023-07-08 15:10:25.000000 alibabacloud_rds20140815_py2-1.1.9/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2023-07-08 15:10:25.000000 alibabacloud_rds20140815_py2-1.1.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 15:10:25.000000 alibabacloud_rds20140815_py2-1.1.9/alibabacloud_rds20140815/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-08 15:10:25.000000 alibabacloud_rds20140815_py2-1.1.9/alibabacloud_rds20140815/__init__.py
--rw-r--r--   0 root         (0) root         (0)   753029 2023-07-08 15:10:25.000000 alibabacloud_rds20140815_py2-1.1.9/alibabacloud_rds20140815/client.py
--rw-r--r--   0 root         (0) root         (0)  2562574 2023-07-08 15:10:25.000000 alibabacloud_rds20140815_py2-1.1.9/alibabacloud_rds20140815/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 15:10:25.000000 alibabacloud_rds20140815_py2-1.1.9/alibabacloud_rds20140815_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2472 2023-07-08 15:10:25.000000 alibabacloud_rds20140815_py2-1.1.9/alibabacloud_rds20140815_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2023-07-08 15:10:25.000000 alibabacloud_rds20140815_py2-1.1.9/alibabacloud_rds20140815_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-08 15:10:25.000000 alibabacloud_rds20140815_py2-1.1.9/alibabacloud_rds20140815_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-07-08 15:10:25.000000 alibabacloud_rds20140815_py2-1.1.9/alibabacloud_rds20140815_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-07-08 15:10:25.000000 alibabacloud_rds20140815_py2-1.1.9/alibabacloud_rds20140815_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-08 15:10:25.000000 alibabacloud_rds20140815_py2-1.1.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2903 2023-07-08 15:10:25.000000 alibabacloud_rds20140815_py2-1.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:08:01.000000 alibabacloud_rds20140815_py2-1.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1648 2023-07-09 15:08:00.000000 alibabacloud_rds20140815_py2-1.2.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-07-09 15:08:00.000000 alibabacloud_rds20140815_py2-1.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-09 15:08:00.000000 alibabacloud_rds20140815_py2-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2472 2023-07-09 15:08:01.000000 alibabacloud_rds20140815_py2-1.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-07-09 15:08:00.000000 alibabacloud_rds20140815_py2-1.2.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2023-07-09 15:08:00.000000 alibabacloud_rds20140815_py2-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:08:01.000000 alibabacloud_rds20140815_py2-1.2.0/alibabacloud_rds20140815/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-09 15:08:00.000000 alibabacloud_rds20140815_py2-1.2.0/alibabacloud_rds20140815/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   753029 2023-07-09 15:08:00.000000 alibabacloud_rds20140815_py2-1.2.0/alibabacloud_rds20140815/client.py
+-rw-r--r--   0 root         (0) root         (0)  2562574 2023-07-09 15:08:00.000000 alibabacloud_rds20140815_py2-1.2.0/alibabacloud_rds20140815/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:08:01.000000 alibabacloud_rds20140815_py2-1.2.0/alibabacloud_rds20140815_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2472 2023-07-09 15:08:00.000000 alibabacloud_rds20140815_py2-1.2.0/alibabacloud_rds20140815_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2023-07-09 15:08:00.000000 alibabacloud_rds20140815_py2-1.2.0/alibabacloud_rds20140815_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 15:08:00.000000 alibabacloud_rds20140815_py2-1.2.0/alibabacloud_rds20140815_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-09 15:08:00.000000 alibabacloud_rds20140815_py2-1.2.0/alibabacloud_rds20140815_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-09 15:08:00.000000 alibabacloud_rds20140815_py2-1.2.0/alibabacloud_rds20140815_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-09 15:08:01.000000 alibabacloud_rds20140815_py2-1.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2903 2023-07-09 15:08:00.000000 alibabacloud_rds20140815_py2-1.2.0/setup.py
```

### Comparing `alibabacloud_rds20140815_py2-1.1.9/ChangeLog.md` & `alibabacloud_rds20140815_py2-1.2.0/ChangeLog.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2023-07-08 Version: 1.1.9
+- Add AutoUseCoupon field.
+- Api Offline.
+
 2023-07-07 Version: 1.1.8
 - Add AutoUseCoupon field.
 - Api Offline.
 
 2023-07-06 Version: 1.1.7
 - Add AutoUseCoupon field.
 - Api Offline.
```

### Comparing `alibabacloud_rds20140815_py2-1.1.9/LICENSE` & `alibabacloud_rds20140815_py2-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815_py2-1.1.9/PKG-INFO` & `alibabacloud_rds20140815_py2-1.2.0/alibabacloud_rds20140815_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_rds20140815_py2
-Version: 1.1.9
+Name: alibabacloud-rds20140815-py2
+Version: 1.2.0
 Summary: Alibaba Cloud rds (20140815) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_rds20140815_py2-1.1.9/README-CN.md` & `alibabacloud_rds20140815_py2-1.2.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815_py2-1.1.9/README.md` & `alibabacloud_rds20140815_py2-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815_py2-1.1.9/alibabacloud_rds20140815/client.py` & `alibabacloud_rds20140815_py2-1.2.0/alibabacloud_rds20140815/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815_py2-1.1.9/alibabacloud_rds20140815/models.py` & `alibabacloud_rds20140815_py2-1.2.0/alibabacloud_rds20140815/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815_py2-1.1.9/alibabacloud_rds20140815_py2.egg-info/PKG-INFO` & `alibabacloud_rds20140815_py2-1.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-rds20140815-py2
-Version: 1.1.9
+Name: alibabacloud_rds20140815_py2
+Version: 1.2.0
 Summary: Alibaba Cloud rds (20140815) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_rds20140815_py2-1.1.9/setup.py` & `alibabacloud_rds20140815_py2-1.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_rds20140815_py2.
 
-Created on 08/07/2023
+Created on 09/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_rds20140815"
 NAME = "alibabacloud_rds20140815_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud rds (20140815) SDK Library for Python2"
```

