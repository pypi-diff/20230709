# Comparing `tmp/threads-py-0.0.4.tar.gz` & `tmp/threads-py-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threads-py-0.0.4.tar", last modified: Sat Jul  8 22:17:22 2023, max compression
+gzip compressed data, was "threads-py-0.0.5.tar", last modified: Sun Jul  9 05:27:23 2023, max compression
```

## Comparing `threads-py-0.0.4.tar` & `threads-py-0.0.5.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-08 22:17:22.397738 threads-py-0.0.4/
--rw-r--r--   0 mineru     (501) staff       (20)     1066 2023-07-07 02:31:26.000000 threads-py-0.0.4/LICENSE
--rw-r--r--   0 mineru     (501) staff       (20)      340 2023-07-08 22:17:22.397585 threads-py-0.0.4/PKG-INFO
--rw-r--r--   0 mineru     (501) staff       (20)     2881 2023-07-08 22:12:05.000000 threads-py-0.0.4/README.md
--rw-r--r--   0 mineru     (501) staff       (20)       38 2023-07-08 22:17:22.397789 threads-py-0.0.4/setup.cfg
--rw-r--r--   0 mineru     (501) staff       (20)      941 2023-07-08 19:52:08.000000 threads-py-0.0.4/setup.py
-drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-08 22:17:22.393380 threads-py-0.0.4/threads_py.egg-info/
--rw-r--r--   0 mineru     (501) staff       (20)      340 2023-07-08 22:17:22.000000 threads-py-0.0.4/threads_py.egg-info/PKG-INFO
--rw-r--r--   0 mineru     (501) staff       (20)     1257 2023-07-08 22:17:22.000000 threads-py-0.0.4/threads_py.egg-info/SOURCES.txt
--rw-r--r--   0 mineru     (501) staff       (20)        1 2023-07-08 22:17:22.000000 threads-py-0.0.4/threads_py.egg-info/dependency_links.txt
--rw-r--r--   0 mineru     (501) staff       (20)       38 2023-07-08 22:17:22.000000 threads-py-0.0.4/threads_py.egg-info/requires.txt
--rw-r--r--   0 mineru     (501) staff       (20)       10 2023-07-08 22:17:22.000000 threads-py-0.0.4/threads_py.egg-info/top_level.txt
-drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-08 22:17:22.393625 threads-py-0.0.4/threadspy/
--rw-r--r--   0 mineru     (501) staff       (20)      111 2023-07-08 22:05:08.000000 threads-py-0.0.4/threadspy/__init__.py
--rw-r--r--   0 mineru     (501) staff       (20)    15139 2023-07-08 22:05:18.000000 threads-py-0.0.4/threadspy/_thread.py
-drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-08 22:17:22.397381 threads-py-0.0.4/threadspy/types/
--rw-r--r--   0 mineru     (501) staff       (20)     1250 2023-07-08 19:54:05.000000 threads-py-0.0.4/threadspy/types/__init__.py
--rw-r--r--   0 mineru     (501) staff       (20)      188 2023-07-07 08:49:18.000000 threads-py-0.0.4/threadspy/types/candidate.py
--rw-r--r--   0 mineru     (501) staff       (20)      134 2023-07-07 08:34:39.000000 threads-py-0.0.4/threadspy/types/caption.py
--rw-r--r--   0 mineru     (501) staff       (20)      622 2023-07-07 18:28:28.000000 threads-py-0.0.4/threadspy/types/common.py
--rw-r--r--   0 mineru     (501) staff       (20)      142 2023-07-07 08:49:13.000000 threads-py-0.0.4/threadspy/types/extensions.py
--rw-r--r--   0 mineru     (501) staff       (20)      302 2023-07-07 18:26:10.000000 threads-py-0.0.4/threadspy/types/get_thread_likers_response.py
--rw-r--r--   0 mineru     (501) staff       (20)      314 2023-07-07 17:56:07.000000 threads-py-0.0.4/threadspy/types/get_user_profile_replies_response.py
--rw-r--r--   0 mineru     (501) staff       (20)      302 2023-07-07 18:03:46.000000 threads-py-0.0.4/threadspy/types/get_user_profile_response.py
--rw-r--r--   0 mineru     (501) staff       (20)      315 2023-07-07 17:57:17.000000 threads-py-0.0.4/threadspy/types/get_user_profile_thread_response.py
--rw-r--r--   0 mineru     (501) staff       (20)      314 2023-07-07 17:57:25.000000 threads-py-0.0.4/threadspy/types/get_user_profile_threads_response.py
--rw-r--r--   0 mineru     (501) staff       (20)      233 2023-07-07 16:58:01.000000 threads-py-0.0.4/threadspy/types/image_versions2.py
--rw-r--r--   0 mineru     (501) staff       (20)      216 2023-07-07 16:58:01.000000 threads-py-0.0.4/threadspy/types/media_data.py
--rw-r--r--   0 mineru     (501) staff       (20)      772 2023-07-07 17:21:37.000000 threads-py-0.0.4/threadspy/types/post.py
--rw-r--r--   0 mineru     (501) staff       (20)      766 2023-07-07 17:21:46.000000 threads-py-0.0.4/threadspy/types/quoted_post.py
--rw-r--r--   0 mineru     (501) staff       (20)      189 2023-07-07 08:46:47.000000 threads-py-0.0.4/threadspy/types/reply_facepile_user.py
--rw-r--r--   0 mineru     (501) staff       (20)      812 2023-07-07 17:22:01.000000 threads-py-0.0.4/threadspy/types/reposted_post.py
--rw-r--r--   0 mineru     (501) staff       (20)      304 2023-07-07 16:58:01.000000 threads-py-0.0.4/threadspy/types/share_info.py
--rw-r--r--   0 mineru     (501) staff       (20)      313 2023-07-07 18:29:52.000000 threads-py-0.0.4/threadspy/types/text_post_app_info.py
--rw-r--r--   0 mineru     (501) staff       (20)      299 2023-07-07 16:58:01.000000 threads-py-0.0.4/threadspy/types/thread.py
--rw-r--r--   0 mineru     (501) staff       (20)      280 2023-07-08 19:54:05.000000 threads-py-0.0.4/threadspy/types/thread_data.py
--rw-r--r--   0 mineru     (501) staff       (20)      433 2023-07-07 16:58:01.000000 threads-py-0.0.4/threadspy/types/thread_item.py
--rw-r--r--   0 mineru     (501) staff       (20)      142 2023-07-07 17:23:07.000000 threads-py-0.0.4/threadspy/types/threads_bio_link.py
--rw-r--r--   0 mineru     (501) staff       (20)      185 2023-07-07 17:20:54.000000 threads-py-0.0.4/threadspy/types/threads_hd_profile_pic_version.py
--rw-r--r--   0 mineru     (501) staff       (20)      729 2023-07-08 18:23:31.000000 threads-py-0.0.4/threadspy/types/threads_user.py
--rw-r--r--   0 mineru     (501) staff       (20)      222 2023-07-07 17:20:21.000000 threads-py-0.0.4/threadspy/types/threads_user_summary.py
--rw-r--r--   0 mineru     (501) staff       (20)      198 2023-07-07 16:58:01.000000 threads-py-0.0.4/threadspy/types/user_data.py
--rw-r--r--   0 mineru     (501) staff       (20)      200 2023-07-07 16:58:00.000000 threads-py-0.0.4/threadspy/types/user_profile_data.py
--rw-r--r--   0 mineru     (501) staff       (20)      230 2023-07-07 18:11:06.000000 threads-py-0.0.4/threadspy/types/users.py
--rw-r--r--   0 mineru     (501) staff       (20)      174 2023-07-07 08:44:28.000000 threads-py-0.0.4/threadspy/types/video_version.py
+drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-09 05:27:23.586537 threads-py-0.0.5/
+-rw-r--r--   0 mineru     (501) staff       (20)     1066 2023-07-07 02:31:26.000000 threads-py-0.0.5/LICENSE
+-rw-r--r--   0 mineru     (501) staff       (20)      340 2023-07-09 05:27:23.586393 threads-py-0.0.5/PKG-INFO
+-rw-r--r--   0 mineru     (501) staff       (20)     2880 2023-07-09 03:41:22.000000 threads-py-0.0.5/README.md
+-rw-r--r--   0 mineru     (501) staff       (20)       38 2023-07-09 05:27:23.586584 threads-py-0.0.5/setup.cfg
+-rw-r--r--   0 mineru     (501) staff       (20)      953 2023-07-09 03:47:40.000000 threads-py-0.0.5/setup.py
+drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-09 05:27:23.581957 threads-py-0.0.5/threads_py.egg-info/
+-rw-r--r--   0 mineru     (501) staff       (20)      340 2023-07-09 05:27:23.000000 threads-py-0.0.5/threads_py.egg-info/PKG-INFO
+-rw-r--r--   0 mineru     (501) staff       (20)     1280 2023-07-09 05:27:23.000000 threads-py-0.0.5/threads_py.egg-info/SOURCES.txt
+-rw-r--r--   0 mineru     (501) staff       (20)        1 2023-07-09 05:27:23.000000 threads-py-0.0.5/threads_py.egg-info/dependency_links.txt
+-rw-r--r--   0 mineru     (501) staff       (20)       47 2023-07-09 05:27:23.000000 threads-py-0.0.5/threads_py.egg-info/requires.txt
+-rw-r--r--   0 mineru     (501) staff       (20)       10 2023-07-09 05:27:23.000000 threads-py-0.0.5/threads_py.egg-info/top_level.txt
+drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-09 05:27:23.582337 threads-py-0.0.5/threadspy/
+-rw-r--r--   0 mineru     (501) staff       (20)      111 2023-07-09 05:27:01.000000 threads-py-0.0.5/threadspy/__init__.py
+-rw-r--r--   0 mineru     (501) staff       (20)      676 2023-07-09 04:04:29.000000 threads-py-0.0.5/threadspy/_constant.py
+-rw-r--r--   0 mineru     (501) staff       (20)    22076 2023-07-09 05:25:26.000000 threads-py-0.0.5/threadspy/_thread.py
+drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-09 05:27:23.586188 threads-py-0.0.5/threadspy/types/
+-rw-r--r--   0 mineru     (501) staff       (20)     1250 2023-07-08 19:54:05.000000 threads-py-0.0.5/threadspy/types/__init__.py
+-rw-r--r--   0 mineru     (501) staff       (20)      188 2023-07-07 08:49:18.000000 threads-py-0.0.5/threadspy/types/candidate.py
+-rw-r--r--   0 mineru     (501) staff       (20)      134 2023-07-07 08:34:39.000000 threads-py-0.0.5/threadspy/types/caption.py
+-rw-r--r--   0 mineru     (501) staff       (20)      622 2023-07-07 18:28:28.000000 threads-py-0.0.5/threadspy/types/common.py
+-rw-r--r--   0 mineru     (501) staff       (20)      142 2023-07-07 08:49:13.000000 threads-py-0.0.5/threadspy/types/extensions.py
+-rw-r--r--   0 mineru     (501) staff       (20)      302 2023-07-07 18:26:10.000000 threads-py-0.0.5/threadspy/types/get_thread_likers_response.py
+-rw-r--r--   0 mineru     (501) staff       (20)      314 2023-07-07 17:56:07.000000 threads-py-0.0.5/threadspy/types/get_user_profile_replies_response.py
+-rw-r--r--   0 mineru     (501) staff       (20)      302 2023-07-07 18:03:46.000000 threads-py-0.0.5/threadspy/types/get_user_profile_response.py
+-rw-r--r--   0 mineru     (501) staff       (20)      315 2023-07-07 17:57:17.000000 threads-py-0.0.5/threadspy/types/get_user_profile_thread_response.py
+-rw-r--r--   0 mineru     (501) staff       (20)      314 2023-07-07 17:57:25.000000 threads-py-0.0.5/threadspy/types/get_user_profile_threads_response.py
+-rw-r--r--   0 mineru     (501) staff       (20)      233 2023-07-07 16:58:01.000000 threads-py-0.0.5/threadspy/types/image_versions2.py
+-rw-r--r--   0 mineru     (501) staff       (20)      216 2023-07-07 16:58:01.000000 threads-py-0.0.5/threadspy/types/media_data.py
+-rw-r--r--   0 mineru     (501) staff       (20)      772 2023-07-07 17:21:37.000000 threads-py-0.0.5/threadspy/types/post.py
+-rw-r--r--   0 mineru     (501) staff       (20)      766 2023-07-07 17:21:46.000000 threads-py-0.0.5/threadspy/types/quoted_post.py
+-rw-r--r--   0 mineru     (501) staff       (20)      189 2023-07-07 08:46:47.000000 threads-py-0.0.5/threadspy/types/reply_facepile_user.py
+-rw-r--r--   0 mineru     (501) staff       (20)      812 2023-07-07 17:22:01.000000 threads-py-0.0.5/threadspy/types/reposted_post.py
+-rw-r--r--   0 mineru     (501) staff       (20)      304 2023-07-07 16:58:01.000000 threads-py-0.0.5/threadspy/types/share_info.py
+-rw-r--r--   0 mineru     (501) staff       (20)      313 2023-07-07 18:29:52.000000 threads-py-0.0.5/threadspy/types/text_post_app_info.py
+-rw-r--r--   0 mineru     (501) staff       (20)      299 2023-07-07 16:58:01.000000 threads-py-0.0.5/threadspy/types/thread.py
+-rw-r--r--   0 mineru     (501) staff       (20)      280 2023-07-08 19:54:05.000000 threads-py-0.0.5/threadspy/types/thread_data.py
+-rw-r--r--   0 mineru     (501) staff       (20)      433 2023-07-07 16:58:01.000000 threads-py-0.0.5/threadspy/types/thread_item.py
+-rw-r--r--   0 mineru     (501) staff       (20)      142 2023-07-07 17:23:07.000000 threads-py-0.0.5/threadspy/types/threads_bio_link.py
+-rw-r--r--   0 mineru     (501) staff       (20)      185 2023-07-07 17:20:54.000000 threads-py-0.0.5/threadspy/types/threads_hd_profile_pic_version.py
+-rw-r--r--   0 mineru     (501) staff       (20)      729 2023-07-08 18:23:31.000000 threads-py-0.0.5/threadspy/types/threads_user.py
+-rw-r--r--   0 mineru     (501) staff       (20)      222 2023-07-07 17:20:21.000000 threads-py-0.0.5/threadspy/types/threads_user_summary.py
+-rw-r--r--   0 mineru     (501) staff       (20)      198 2023-07-07 16:58:01.000000 threads-py-0.0.5/threadspy/types/user_data.py
+-rw-r--r--   0 mineru     (501) staff       (20)      200 2023-07-07 16:58:00.000000 threads-py-0.0.5/threadspy/types/user_profile_data.py
+-rw-r--r--   0 mineru     (501) staff       (20)      230 2023-07-07 18:11:06.000000 threads-py-0.0.5/threadspy/types/users.py
+-rw-r--r--   0 mineru     (501) staff       (20)      174 2023-07-07 08:44:28.000000 threads-py-0.0.5/threadspy/types/video_version.py
```

### Comparing `threads-py-0.0.4/LICENSE` & `threads-py-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `threads-py-0.0.4/README.md` & `threads-py-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 - [ ] 🚧 LangChain Agent
   - [ ] 🚧 Link Threads & LLaMa
   - [ ] 🚧 Provide statistical analysis of posts in Threads
 - [ ] 🚧 Read private data
 - [x] ✅ Write data (i.e. write automated Threads)
   - [x] ✅ Create new Thread with text
     - [ ] 🚧 Make link previews to get shown
-  - [ ] 🚧 Create new Thread with media
+  - [x] ✅ Create new Thread with media
   - [ ] 🚧 Reply to existing Thread
 - [x] 🏴‍☠️ Restructure project as an monorepo
   - [ ] 🏴‍☠️ Cool CLI App to run Threads in the Terminal
 
 ## License
 
 <p align="center">
```

#### html2text {}

```diff
@@ -21,16 +21,16 @@
 â Read User Profile Info - [x] â Read list of User Threads - [x] â Read
 list of User Repiles - [x] â Fetch PostID(`3140957200974444958`) via PostURL
 (`https://www.threads.net/t/CuW6-7KyXme`) - [x] â Read Threads via PostID -
 [x] â Read Likers in Thread via PostID - [ ] ð§ Read User Followers - [ ]
 ð§ Read User Followings - [ ] ð§ LangChain Agent - [ ] ð§ Link Threads &
 LLaMa - [ ] ð§ Provide statistical analysis of posts in Threads - [ ] ð§
 Read private data - [x] â Write data (i.e. write automated Threads) - [x] â
-Create new Thread with text - [ ] ð§ Make link previews to get shown - [ ]
-ð§ Create new Thread with media - [ ] ð§ Reply to existing Thread - [x]
+Create new Thread with text - [ ] ð§ Make link previews to get shown - [x]
+â Create new Thread with media - [ ] ð§ Reply to existing Thread - [x]
 ð´ââ ï¸ Restructure project as an monorepo - [ ] ð´ââ ï¸ Cool CLI
 App to run Threads in the Terminal ## License
                            [./.github/labtocat.png]
                                MIT Â© Junho_Yeo
 If you find this project intriguing, **please consider starring it(â­)** or
 following me on [GitHub](https://github.com/junhoyeo) (I wouldn't say [Threads]
 (https://www.threads.net/@_junhoyeo)).
```

### Comparing `threads-py-0.0.4/setup.py` & `threads-py-0.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,10 +18,10 @@
     author_email="i@junho.io",
     url="https://github.com/junhoyeo/threads-py",
     license="MIT License",
     description="Unofficial, Reverse-Engineered Python client for Meta's Threads.",
     long_description_content_type="text/markdown",
     platforms=["any"],
     packages=find_packages(exclude=["tests", "assets"]),
-    install_requires=["requests", "dataclasses", "dataclasses-json"],
+    install_requires=["requests", "dataclasses", "dataclasses-json", "aiofiles"],
     python_requires=">=3.8",
 )
```

### Comparing `threads-py-0.0.4/threads_py.egg-info/SOURCES.txt` & `threads-py-0.0.5/threads_py.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 setup.py
 threads_py.egg-info/PKG-INFO
 threads_py.egg-info/SOURCES.txt
 threads_py.egg-info/dependency_links.txt
 threads_py.egg-info/requires.txt
 threads_py.egg-info/top_level.txt
 threadspy/__init__.py
+threadspy/_constant.py
 threadspy/_thread.py
 threadspy/types/__init__.py
 threadspy/types/candidate.py
 threadspy/types/caption.py
 threadspy/types/common.py
 threadspy/types/extensions.py
 threadspy/types/get_thread_likers_response.py
```

### Comparing `threads-py-0.0.4/threadspy/types/__init__.py` & `threads-py-0.0.5/threadspy/types/__init__.py`

 * *Files identical despite different names*

### Comparing `threads-py-0.0.4/threadspy/types/common.py` & `threads-py-0.0.5/threadspy/types/common.py`

 * *Files identical despite different names*

### Comparing `threads-py-0.0.4/threadspy/types/post.py` & `threads-py-0.0.5/threadspy/types/post.py`

 * *Files identical despite different names*

### Comparing `threads-py-0.0.4/threadspy/types/quoted_post.py` & `threads-py-0.0.5/threadspy/types/quoted_post.py`

 * *Files identical despite different names*

### Comparing `threads-py-0.0.4/threadspy/types/reposted_post.py` & `threads-py-0.0.5/threadspy/types/reposted_post.py`

 * *Files identical despite different names*

### Comparing `threads-py-0.0.4/threadspy/types/threads_user.py` & `threads-py-0.0.5/threadspy/types/threads_user.py`

 * *Files identical despite different names*

