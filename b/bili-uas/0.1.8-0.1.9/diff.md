# Comparing `tmp/bili-uas-0.1.8.tar.gz` & `tmp/bili-uas-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bili-uas-0.1.8.tar", last modified: Sun Jul  9 01:57:57 2023, max compression
+gzip compressed data, was "bili-uas-0.1.9.tar", last modified: Sun Jul  9 02:00:31 2023, max compression
```

## Comparing `bili-uas-0.1.8.tar` & `bili-uas-0.1.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-09 01:57:57.746245 bili-uas-0.1.8/
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-09 01:57:57.741261 bili-uas-0.1.8/Bili_UAS/
--rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-30 10:47:09.000000 bili-uas-0.1.8/Bili_UAS/__init__.py
--rw-r--r--   0 jhzg       (501) staff       (20)     1903 2023-07-03 09:43:52.000000 bili-uas-0.1.8/Bili_UAS/bili_config.py
--rw-r--r--   0 jhzg       (501) staff       (20)     5275 2023-07-09 01:57:53.000000 bili-uas-0.1.8/Bili_UAS/bili_live.py
--rw-r--r--   0 jhzg       (501) staff       (20)     2831 2023-07-03 09:35:16.000000 bili-uas-0.1.8/Bili_UAS/bili_login.py
--rw-r--r--   0 jhzg       (501) staff       (20)     2826 2023-07-03 09:35:16.000000 bili-uas-0.1.8/Bili_UAS/bili_user.py
--rw-r--r--   0 jhzg       (501) staff       (20)     2510 2023-07-03 09:35:16.000000 bili-uas-0.1.8/Bili_UAS/bili_video.py
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-09 01:57:57.742728 bili-uas-0.1.8/Bili_UAS/scripts/
--rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-14 13:05:48.000000 bili-uas-0.1.8/Bili_UAS/scripts/__init__.py
--rw-r--r--   0 jhzg       (501) staff       (20)     2368 2023-06-30 11:28:07.000000 bili-uas-0.1.8/Bili_UAS/scripts/config.py
--rw-r--r--   0 jhzg       (501) staff       (20)     4270 2023-07-08 14:14:34.000000 bili-uas-0.1.8/Bili_UAS/scripts/live.py
--rw-r--r--   0 jhzg       (501) staff       (20)    10541 2023-06-30 11:05:14.000000 bili-uas-0.1.8/Bili_UAS/scripts/log_in.py
--rw-r--r--   0 jhzg       (501) staff       (20)     1366 2023-06-30 11:05:14.000000 bili-uas-0.1.8/Bili_UAS/scripts/user.py
--rw-r--r--   0 jhzg       (501) staff       (20)     5687 2023-06-30 11:44:32.000000 bili-uas-0.1.8/Bili_UAS/scripts/video.py
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-09 01:57:57.744745 bili-uas-0.1.8/Bili_UAS/utils/
--rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-13 07:49:27.000000 bili-uas-0.1.8/Bili_UAS/utils/__init__.py
--rw-r--r--   0 jhzg       (501) staff       (20)    50170 2023-07-06 12:45:25.000000 bili-uas-0.1.8/Bili_UAS/utils/live_utils.py
--rw-r--r--   0 jhzg       (501) staff       (20)     2186 2023-06-30 10:59:22.000000 bili-uas-0.1.8/Bili_UAS/utils/search_utils.py
--rw-r--r--   0 jhzg       (501) staff       (20)      359 2023-06-30 10:59:22.000000 bili-uas-0.1.8/Bili_UAS/utils/train_utils.py
--rw-r--r--   0 jhzg       (501) staff       (20)    15374 2023-06-30 10:59:22.000000 bili-uas-0.1.8/Bili_UAS/utils/user_utils.py
--rw-r--r--   0 jhzg       (501) staff       (20)    11258 2023-06-30 10:59:22.000000 bili-uas-0.1.8/Bili_UAS/utils/utils.py
--rw-r--r--   0 jhzg       (501) staff       (20)    18789 2023-06-30 10:59:22.000000 bili-uas-0.1.8/Bili_UAS/utils/video_utils.py
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-09 01:57:57.745264 bili-uas-0.1.8/Bili_UAS/writer/
--rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-05-16 02:00:41.000000 bili-uas-0.1.8/Bili_UAS/writer/__init__.py
--rw-r--r--   0 jhzg       (501) staff       (20)      488 2023-06-30 10:59:22.000000 bili-uas-0.1.8/Bili_UAS/writer/abnormal_monitor.py
--rw-r--r--   0 jhzg       (501) staff       (20)     3575 2023-07-03 09:41:05.000000 bili-uas-0.1.8/Bili_UAS/writer/log_writer.py
--rw-r--r--   0 jhzg       (501) staff       (20)    34523 2023-06-06 23:49:40.000000 bili-uas-0.1.8/LICENSE
--rw-r--r--   0 jhzg       (501) staff       (20)     4599 2023-07-09 01:57:57.746118 bili-uas-0.1.8/PKG-INFO
--rw-r--r--   0 jhzg       (501) staff       (20)     3874 2023-07-08 12:32:56.000000 bili-uas-0.1.8/README.md
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-09 01:57:57.745955 bili-uas-0.1.8/bili_uas.egg-info/
--rw-r--r--   0 jhzg       (501) staff       (20)     4599 2023-07-09 01:57:57.000000 bili-uas-0.1.8/bili_uas.egg-info/PKG-INFO
--rw-r--r--   0 jhzg       (501) staff       (20)      808 2023-07-09 01:57:57.000000 bili-uas-0.1.8/bili_uas.egg-info/SOURCES.txt
--rw-r--r--   0 jhzg       (501) staff       (20)        1 2023-07-09 01:57:57.000000 bili-uas-0.1.8/bili_uas.egg-info/dependency_links.txt
--rw-r--r--   0 jhzg       (501) staff       (20)      226 2023-07-09 01:57:57.000000 bili-uas-0.1.8/bili_uas.egg-info/entry_points.txt
--rw-r--r--   0 jhzg       (501) staff       (20)      245 2023-07-09 01:57:57.000000 bili-uas-0.1.8/bili_uas.egg-info/requires.txt
--rw-r--r--   0 jhzg       (501) staff       (20)        9 2023-07-09 01:57:57.000000 bili-uas-0.1.8/bili_uas.egg-info/top_level.txt
--rw-r--r--   0 jhzg       (501) staff       (20)       38 2023-07-09 01:57:57.746285 bili-uas-0.1.8/setup.cfg
--rw-r--r--   0 jhzg       (501) staff       (20)     2001 2023-07-09 01:57:53.000000 bili-uas-0.1.8/setup.py
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-09 02:00:31.523998 bili-uas-0.1.9/
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-09 02:00:31.518833 bili-uas-0.1.9/Bili_UAS/
+-rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-30 10:47:09.000000 bili-uas-0.1.9/Bili_UAS/__init__.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     1903 2023-07-03 09:43:52.000000 bili-uas-0.1.9/Bili_UAS/bili_config.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     5353 2023-07-09 02:00:21.000000 bili-uas-0.1.9/Bili_UAS/bili_live.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     2831 2023-07-03 09:35:16.000000 bili-uas-0.1.9/Bili_UAS/bili_login.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     2826 2023-07-03 09:35:16.000000 bili-uas-0.1.9/Bili_UAS/bili_user.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     2599 2023-07-09 02:00:21.000000 bili-uas-0.1.9/Bili_UAS/bili_video.py
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-09 02:00:31.520040 bili-uas-0.1.9/Bili_UAS/scripts/
+-rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-14 13:05:48.000000 bili-uas-0.1.9/Bili_UAS/scripts/__init__.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     2368 2023-06-30 11:28:07.000000 bili-uas-0.1.9/Bili_UAS/scripts/config.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     4270 2023-07-08 14:14:34.000000 bili-uas-0.1.9/Bili_UAS/scripts/live.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    10541 2023-06-30 11:05:14.000000 bili-uas-0.1.9/Bili_UAS/scripts/log_in.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     1366 2023-06-30 11:05:14.000000 bili-uas-0.1.9/Bili_UAS/scripts/user.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     5687 2023-06-30 11:44:32.000000 bili-uas-0.1.9/Bili_UAS/scripts/video.py
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-09 02:00:31.522131 bili-uas-0.1.9/Bili_UAS/utils/
+-rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-13 07:49:27.000000 bili-uas-0.1.9/Bili_UAS/utils/__init__.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    50170 2023-07-06 12:45:25.000000 bili-uas-0.1.9/Bili_UAS/utils/live_utils.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     2186 2023-06-30 10:59:22.000000 bili-uas-0.1.9/Bili_UAS/utils/search_utils.py
+-rw-r--r--   0 jhzg       (501) staff       (20)      359 2023-06-30 10:59:22.000000 bili-uas-0.1.9/Bili_UAS/utils/train_utils.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    15374 2023-06-30 10:59:22.000000 bili-uas-0.1.9/Bili_UAS/utils/user_utils.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    11258 2023-06-30 10:59:22.000000 bili-uas-0.1.9/Bili_UAS/utils/utils.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    18789 2023-06-30 10:59:22.000000 bili-uas-0.1.9/Bili_UAS/utils/video_utils.py
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-09 02:00:31.522739 bili-uas-0.1.9/Bili_UAS/writer/
+-rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-05-16 02:00:41.000000 bili-uas-0.1.9/Bili_UAS/writer/__init__.py
+-rw-r--r--   0 jhzg       (501) staff       (20)      488 2023-06-30 10:59:22.000000 bili-uas-0.1.9/Bili_UAS/writer/abnormal_monitor.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     3575 2023-07-03 09:41:05.000000 bili-uas-0.1.9/Bili_UAS/writer/log_writer.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    34523 2023-06-06 23:49:40.000000 bili-uas-0.1.9/LICENSE
+-rw-r--r--   0 jhzg       (501) staff       (20)     4599 2023-07-09 02:00:31.523769 bili-uas-0.1.9/PKG-INFO
+-rw-r--r--   0 jhzg       (501) staff       (20)     3874 2023-07-08 12:32:56.000000 bili-uas-0.1.9/README.md
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-09 02:00:31.523507 bili-uas-0.1.9/bili_uas.egg-info/
+-rw-r--r--   0 jhzg       (501) staff       (20)     4599 2023-07-09 02:00:31.000000 bili-uas-0.1.9/bili_uas.egg-info/PKG-INFO
+-rw-r--r--   0 jhzg       (501) staff       (20)      808 2023-07-09 02:00:31.000000 bili-uas-0.1.9/bili_uas.egg-info/SOURCES.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)        1 2023-07-09 02:00:31.000000 bili-uas-0.1.9/bili_uas.egg-info/dependency_links.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)      226 2023-07-09 02:00:31.000000 bili-uas-0.1.9/bili_uas.egg-info/entry_points.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)      245 2023-07-09 02:00:31.000000 bili-uas-0.1.9/bili_uas.egg-info/requires.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)        9 2023-07-09 02:00:31.000000 bili-uas-0.1.9/bili_uas.egg-info/top_level.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)       38 2023-07-09 02:00:31.524061 bili-uas-0.1.9/setup.cfg
+-rw-r--r--   0 jhzg       (501) staff       (20)     2001 2023-07-09 02:00:28.000000 bili-uas-0.1.9/setup.py
```

### Comparing `bili-uas-0.1.8/Bili_UAS/bili_config.py` & `bili-uas-0.1.9/Bili_UAS/bili_config.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.8/Bili_UAS/bili_live.py` & `bili-uas-0.1.9/Bili_UAS/bili_live.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,18 @@
 
     elif isinstance(config, sl.BiliLiveConfigProcess):
         log.warning("Set the mode to 'process', and in this mode, a data folder needs to be specified!")
 
         if config.data_dir is None:
             raise am.ParameterInputError("No data folder specified!")
 
-        mask: npt.NDArray = plt.imread(config.mask)
+        if config.mask is not None:
+            mask: npt.NDArray = plt.imread(config.mask)
+        else:
+            mask = None
         live_process = lu.BiliLiveProcess(log_file, config.data_dir)
         sync(live_process.analysis(config.revenue_interval, config.danmu_interval, config.robust,
                                    config.robust_interval, mask))
 
 
 def tyro_cli() -> None:
     """
```

### Comparing `bili-uas-0.1.8/Bili_UAS/bili_login.py` & `bili-uas-0.1.9/Bili_UAS/bili_login.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.8/Bili_UAS/bili_user.py` & `bili-uas-0.1.9/Bili_UAS/bili_user.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.8/Bili_UAS/bili_video.py` & `bili-uas-0.1.9/Bili_UAS/bili_video.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,18 @@
     if credential is not None:
         credential = sync(sli.refresh_credential(credential, log_file))
 
     if isinstance(config, sv.BiliVideoConfigWordCloud):
         if config.video_id is None:
             raise am.ParameterInputError("Video ID not entered!")
         wm = sv.WordCloudContent(config.mode)
-        word_cloud_mask: npt.NDArray = plt.imread(config.mask)
+        if config.mask is not None:
+            word_cloud_mask: npt.NDArray = plt.imread(config.mask)
+        else:
+            word_cloud_mask = None
         sync(sv.word_cloud(config.video_id, credential, wm, config.sec, word_cloud_mask, log_file, work_dir))
     else:
         if config.video_id is None:
             raise am.ParameterInputError("Video ID not entered!")
         dm = vu.VideoDownloadMode(config.mode)
         if isinstance(config.video_id, int):
             video = vu.BiliVideo(log=log_file, aid=config.video_id, credential=credential, work_dir=work_dir)
```

### Comparing `bili-uas-0.1.8/Bili_UAS/scripts/config.py` & `bili-uas-0.1.9/Bili_UAS/scripts/config.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.8/Bili_UAS/scripts/live.py` & `bili-uas-0.1.9/Bili_UAS/scripts/live.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.8/Bili_UAS/scripts/log_in.py` & `bili-uas-0.1.9/Bili_UAS/scripts/log_in.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.8/Bili_UAS/scripts/user.py` & `bili-uas-0.1.9/Bili_UAS/scripts/user.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.8/Bili_UAS/scripts/video.py` & `bili-uas-0.1.9/Bili_UAS/scripts/video.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.8/Bili_UAS/utils/live_utils.py` & `bili-uas-0.1.9/Bili_UAS/utils/live_utils.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.8/Bili_UAS/utils/search_utils.py` & `bili-uas-0.1.9/Bili_UAS/utils/search_utils.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.8/Bili_UAS/utils/user_utils.py` & `bili-uas-0.1.9/Bili_UAS/utils/user_utils.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.8/Bili_UAS/utils/utils.py` & `bili-uas-0.1.9/Bili_UAS/utils/utils.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.8/Bili_UAS/utils/video_utils.py` & `bili-uas-0.1.9/Bili_UAS/utils/video_utils.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.8/Bili_UAS/writer/log_writer.py` & `bili-uas-0.1.9/Bili_UAS/writer/log_writer.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.8/LICENSE` & `bili-uas-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.8/PKG-INFO` & `bili-uas-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bili-uas
-Version: 0.1.8
+Version: 0.1.9
 Summary: Assist up in personal, live, and video data analysis and prediction.
 Home-page: https://github.com/jhzgjhzg/BiliBili-UP-Auxiliary-System
 Author: jhzg
 Author-email: jhzg02200059@163.com
 License: GPLv3
 Keywords: BiliBili,auxiliary,analysis,live,video,word_cloud
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `bili-uas-0.1.8/README.md` & `bili-uas-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.8/bili_uas.egg-info/PKG-INFO` & `bili-uas-0.1.9/bili_uas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bili-uas
-Version: 0.1.8
+Version: 0.1.9
 Summary: Assist up in personal, live, and video data analysis and prediction.
 Home-page: https://github.com/jhzgjhzg/BiliBili-UP-Auxiliary-System
 Author: jhzg
 Author-email: jhzg02200059@163.com
 License: GPLv3
 Keywords: BiliBili,auxiliary,analysis,live,video,word_cloud
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `bili-uas-0.1.8/bili_uas.egg-info/SOURCES.txt` & `bili-uas-0.1.9/bili_uas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.8/setup.py` & `bili-uas-0.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     'apscheduler~=3.10.1',
     'requests~=2.31.0',
     'httpx~=0.24.1',
     'openpyxl~=3.1.2']
 
 setup(
     name='bili-uas',
-    version='0.1.8',
+    version='0.1.9',
     license='GPLv3',
     author='jhzg',
     author_email='jhzg02200059@163.com',
     url='https://github.com/jhzgjhzg/BiliBili-UP-Auxiliary-System',
     description='Assist up in personal, live, and video data analysis and prediction.',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

