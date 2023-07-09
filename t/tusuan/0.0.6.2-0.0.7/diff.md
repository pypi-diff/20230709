# Comparing `tmp/tusuan-0.0.6.2.tar.gz` & `tmp/tusuan-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tusuan-0.0.6.2.tar", last modified: Thu May 18 16:04:22 2023, max compression
+gzip compressed data, was "tusuan-0.0.7.tar", last modified: Sun Jul  9 14:56:14 2023, max compression
```

## Comparing `tusuan-0.0.6.2.tar` & `tusuan-0.0.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-05-18 16:04:22.363945 tusuan-0.0.6.2/
--rw-r--r--   0 xiangyang   (501) staff       (20)      172 2022-12-29 07:25:59.000000 tusuan-0.0.6.2/MANIFEST.in
--rw-r--r--   0 xiangyang   (501) staff       (20)      565 2023-05-18 16:04:22.363806 tusuan-0.0.6.2/PKG-INFO
--rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-03-29 03:34:53.000000 tusuan-0.0.6.2/README.md
--rw-r--r--   0 xiangyang   (501) staff       (20)       90 2023-05-18 10:11:09.000000 tusuan-0.0.6.2/requirements.txt
--rw-r--r--   0 xiangyang   (501) staff       (20)       38 2023-05-18 16:04:22.363995 tusuan-0.0.6.2/setup.cfg
--rw-r--r--   0 xiangyang   (501) staff       (20)     1648 2023-05-18 16:03:36.000000 tusuan-0.0.6.2/setup.py
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-05-18 16:04:22.360928 tusuan-0.0.6.2/tusuan/
--rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-03-29 03:37:06.000000 tusuan-0.0.6.2/tusuan/__init__.py
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-05-18 16:04:22.361884 tusuan-0.0.6.2/tusuan/datasets/
--rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-05-18 04:55:21.000000 tusuan-0.0.6.2/tusuan/datasets/__init__.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     4332 2023-05-18 16:03:26.000000 tusuan-0.0.6.2/tusuan/datasets/imagenet.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     1099 2023-03-15 10:31:32.000000 tusuan-0.0.6.2/tusuan/file_function.py
--rw-r--r--   0 xiangyang   (501) staff       (20)       40 2023-03-29 03:39:48.000000 tusuan-0.0.6.2/tusuan/hello.py
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-05-18 16:04:22.363413 tusuan-0.0.6.2/tusuan/image_video_utils/
--rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-03-29 17:21:56.000000 tusuan-0.0.6.2/tusuan/image_video_utils/__init__.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     2137 2023-05-08 05:08:27.000000 tusuan-0.0.6.2/tusuan/image_video_utils/croppers.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     1163 2023-05-07 17:43:48.000000 tusuan-0.0.6.2/tusuan/image_video_utils/display.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     1329 2023-04-07 04:48:17.000000 tusuan-0.0.6.2/tusuan/image_video_utils/image_visual_selector.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     4013 2023-05-08 05:14:00.000000 tusuan-0.0.6.2/tusuan/image_video_utils/readers.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     2583 2023-05-08 18:11:39.000000 tusuan-0.0.6.2/tusuan/image_video_utils/writers.py
--rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-04-21 16:44:19.000000 tusuan-0.0.6.2/tusuan/path_utils.py
--rw-r--r--   0 xiangyang   (501) staff       (20)       97 2023-05-14 11:47:37.000000 tusuan-0.0.6.2/tusuan/time_utils.py
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-05-18 16:04:22.361633 tusuan-0.0.6.2/tusuan.egg-info/
--rw-r--r--   0 xiangyang   (501) staff       (20)      565 2023-05-18 16:04:22.000000 tusuan-0.0.6.2/tusuan.egg-info/PKG-INFO
--rw-r--r--   0 xiangyang   (501) staff       (20)      585 2023-05-18 16:04:22.000000 tusuan-0.0.6.2/tusuan.egg-info/SOURCES.txt
--rw-r--r--   0 xiangyang   (501) staff       (20)        1 2023-05-18 16:04:22.000000 tusuan-0.0.6.2/tusuan.egg-info/dependency_links.txt
--rw-r--r--   0 xiangyang   (501) staff       (20)       90 2023-05-18 16:04:22.000000 tusuan-0.0.6.2/tusuan.egg-info/requires.txt
--rw-r--r--   0 xiangyang   (501) staff       (20)        7 2023-05-18 16:04:22.000000 tusuan-0.0.6.2/tusuan.egg-info/top_level.txt
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-07-09 14:56:14.719703 tusuan-0.0.7/
+-rw-r--r--   0 xiangyang   (501) staff       (20)      172 2022-12-29 07:25:59.000000 tusuan-0.0.7/MANIFEST.in
+-rw-r--r--   0 xiangyang   (501) staff       (20)      563 2023-07-09 14:56:14.719578 tusuan-0.0.7/PKG-INFO
+-rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-03-29 03:34:53.000000 tusuan-0.0.7/README.md
+-rw-r--r--   0 xiangyang   (501) staff       (20)       90 2023-05-18 10:11:09.000000 tusuan-0.0.7/requirements.txt
+-rw-r--r--   0 xiangyang   (501) staff       (20)       38 2023-07-09 14:56:14.719741 tusuan-0.0.7/setup.cfg
+-rw-r--r--   0 xiangyang   (501) staff       (20)     1646 2023-07-09 14:55:58.000000 tusuan-0.0.7/setup.py
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-07-09 14:56:14.718187 tusuan-0.0.7/tusuan/
+-rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-03-29 03:37:06.000000 tusuan-0.0.7/tusuan/__init__.py
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-07-09 14:56:14.718842 tusuan-0.0.7/tusuan/datasets/
+-rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-05-18 04:55:21.000000 tusuan-0.0.7/tusuan/datasets/__init__.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     4332 2023-05-18 16:03:26.000000 tusuan-0.0.7/tusuan/datasets/imagenet.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     1099 2023-03-15 10:31:32.000000 tusuan-0.0.7/tusuan/file_function.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)       40 2023-03-29 03:39:48.000000 tusuan-0.0.7/tusuan/hello.py
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-07-09 14:56:14.719427 tusuan-0.0.7/tusuan/image_video_utils/
+-rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-03-29 17:21:56.000000 tusuan-0.0.7/tusuan/image_video_utils/__init__.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     2137 2023-05-08 05:08:27.000000 tusuan-0.0.7/tusuan/image_video_utils/croppers.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     1163 2023-05-07 17:43:48.000000 tusuan-0.0.7/tusuan/image_video_utils/display.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     1329 2023-04-07 04:48:17.000000 tusuan-0.0.7/tusuan/image_video_utils/image_visual_selector.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     4013 2023-05-08 05:14:00.000000 tusuan-0.0.7/tusuan/image_video_utils/readers.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     2583 2023-05-08 18:11:39.000000 tusuan-0.0.7/tusuan/image_video_utils/writers.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     1018 2023-07-09 14:55:10.000000 tusuan-0.0.7/tusuan/path_utils.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)       98 2023-07-09 14:55:48.000000 tusuan-0.0.7/tusuan/time_utils.py
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-07-09 14:56:14.718666 tusuan-0.0.7/tusuan.egg-info/
+-rw-r--r--   0 xiangyang   (501) staff       (20)      563 2023-07-09 14:56:14.000000 tusuan-0.0.7/tusuan.egg-info/PKG-INFO
+-rw-r--r--   0 xiangyang   (501) staff       (20)      585 2023-07-09 14:56:14.000000 tusuan-0.0.7/tusuan.egg-info/SOURCES.txt
+-rw-r--r--   0 xiangyang   (501) staff       (20)        1 2023-07-09 14:56:14.000000 tusuan-0.0.7/tusuan.egg-info/dependency_links.txt
+-rw-r--r--   0 xiangyang   (501) staff       (20)       90 2023-07-09 14:56:14.000000 tusuan-0.0.7/tusuan.egg-info/requires.txt
+-rw-r--r--   0 xiangyang   (501) staff       (20)        7 2023-07-09 14:56:14.000000 tusuan-0.0.7/tusuan.egg-info/top_level.txt
```

### Comparing `tusuan-0.0.6.2/PKG-INFO` & `tusuan-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tusuan
-Version: 0.0.6.2
+Version: 0.0.7
 Summary: useful functions.
 Home-page: https://github.com/tusuan
 Author: tusuan
 Author-email: btk@qq.com
 License: MIT
 Keywords: tusuan
 Platform: UNKNOWN
```

### Comparing `tusuan-0.0.6.2/setup.py` & `tusuan-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from read import read
 from setuptools import setup, find_packages
 
 setup(name='tusuan',  # 包名
       python_requires='>=3.8.0',  # python环境
-      version='0.0.6.2',  # 包的版本
+      version='0.0.7',  # 包的版本
       description="useful functions.",  # 包简介，显示在PyPI上
 
       long_description=read('README.md'),  # 读取的Readme文档内容，一整块字符串
       long_description_content_type="text/markdown",  # 指定包文档格式为markdown
 
       author="tusuan",  # 作者相关信息
       author_email='btk@qq.com',
```

### Comparing `tusuan-0.0.6.2/tusuan/datasets/imagenet.py` & `tusuan-0.0.7/tusuan/datasets/imagenet.py`

 * *Files identical despite different names*

### Comparing `tusuan-0.0.6.2/tusuan/file_function.py` & `tusuan-0.0.7/tusuan/file_function.py`

 * *Files identical despite different names*

### Comparing `tusuan-0.0.6.2/tusuan/image_video_utils/croppers.py` & `tusuan-0.0.7/tusuan/image_video_utils/croppers.py`

 * *Files identical despite different names*

### Comparing `tusuan-0.0.6.2/tusuan/image_video_utils/display.py` & `tusuan-0.0.7/tusuan/image_video_utils/display.py`

 * *Files identical despite different names*

### Comparing `tusuan-0.0.6.2/tusuan/image_video_utils/image_visual_selector.py` & `tusuan-0.0.7/tusuan/image_video_utils/image_visual_selector.py`

 * *Files identical despite different names*

### Comparing `tusuan-0.0.6.2/tusuan/image_video_utils/readers.py` & `tusuan-0.0.7/tusuan/image_video_utils/readers.py`

 * *Files identical despite different names*

### Comparing `tusuan-0.0.6.2/tusuan/image_video_utils/writers.py` & `tusuan-0.0.7/tusuan/image_video_utils/writers.py`

 * *Files identical despite different names*

### Comparing `tusuan-0.0.6.2/tusuan.egg-info/PKG-INFO` & `tusuan-0.0.7/tusuan.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tusuan
-Version: 0.0.6.2
+Version: 0.0.7
 Summary: useful functions.
 Home-page: https://github.com/tusuan
 Author: tusuan
 Author-email: btk@qq.com
 License: MIT
 Keywords: tusuan
 Platform: UNKNOWN
```

### Comparing `tusuan-0.0.6.2/tusuan.egg-info/SOURCES.txt` & `tusuan-0.0.7/tusuan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

