# Comparing `tmp/threads-py-0.0.2.tar.gz` & `tmp/threads-py-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threads-py-0.0.2.tar", last modified: Sat Jul  8 19:25:53 2023, max compression
+gzip compressed data, was "threads-py-0.0.3.tar", last modified: Sat Jul  8 19:40:58 2023, max compression
```

## Comparing `threads-py-0.0.2.tar` & `threads-py-0.0.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-08 19:25:53.302879 threads-py-0.0.2/
--rw-r--r--   0 mineru     (501) staff       (20)     1066 2023-07-07 02:31:26.000000 threads-py-0.0.2/LICENSE
--rw-r--r--   0 mineru     (501) staff       (20)      340 2023-07-08 19:25:53.302703 threads-py-0.0.2/PKG-INFO
--rw-r--r--   0 mineru     (501) staff       (20)     2436 2023-07-08 19:21:10.000000 threads-py-0.0.2/README.md
--rw-r--r--   0 mineru     (501) staff       (20)       38 2023-07-08 19:25:53.302930 threads-py-0.0.2/setup.cfg
--rw-r--r--   0 mineru     (501) staff       (20)      941 2023-07-08 17:19:16.000000 threads-py-0.0.2/setup.py
-drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-08 19:25:53.297563 threads-py-0.0.2/threads_py.egg-info/
--rw-r--r--   0 mineru     (501) staff       (20)      340 2023-07-08 19:25:53.000000 threads-py-0.0.2/threads_py.egg-info/PKG-INFO
--rw-r--r--   0 mineru     (501) staff       (20)     1257 2023-07-08 19:25:53.000000 threads-py-0.0.2/threads_py.egg-info/SOURCES.txt
--rw-r--r--   0 mineru     (501) staff       (20)        1 2023-07-08 19:25:53.000000 threads-py-0.0.2/threads_py.egg-info/dependency_links.txt
--rw-r--r--   0 mineru     (501) staff       (20)       38 2023-07-08 19:25:53.000000 threads-py-0.0.2/threads_py.egg-info/requires.txt
--rw-r--r--   0 mineru     (501) staff       (20)       10 2023-07-08 19:25:53.000000 threads-py-0.0.2/threads_py.egg-info/top_level.txt
-drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-08 19:25:53.297816 threads-py-0.0.2/threadspy/
--rw-r--r--   0 mineru     (501) staff       (20)      111 2023-07-08 18:27:24.000000 threads-py-0.0.2/threadspy/__init__.py
--rw-r--r--   0 mineru     (501) staff       (20)    10788 2023-07-08 19:25:33.000000 threads-py-0.0.2/threadspy/_thread.py
-drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-08 19:25:53.302341 threads-py-0.0.2/threadspy/types/
--rw-r--r--   0 mineru     (501) staff       (20)     1250 2023-07-08 18:18:23.000000 threads-py-0.0.2/threadspy/types/__init__.py
--rw-r--r--   0 mineru     (501) staff       (20)      188 2023-07-07 08:49:18.000000 threads-py-0.0.2/threadspy/types/candidate.py
--rw-r--r--   0 mineru     (501) staff       (20)      134 2023-07-07 08:34:39.000000 threads-py-0.0.2/threadspy/types/caption.py
--rw-r--r--   0 mineru     (501) staff       (20)      622 2023-07-07 18:28:28.000000 threads-py-0.0.2/threadspy/types/common.py
--rw-r--r--   0 mineru     (501) staff       (20)      142 2023-07-07 08:49:13.000000 threads-py-0.0.2/threadspy/types/extensions.py
--rw-r--r--   0 mineru     (501) staff       (20)      302 2023-07-07 18:26:10.000000 threads-py-0.0.2/threadspy/types/get_thread_likers_response.py
--rw-r--r--   0 mineru     (501) staff       (20)      314 2023-07-07 17:56:07.000000 threads-py-0.0.2/threadspy/types/get_user_profile_replies_response.py
--rw-r--r--   0 mineru     (501) staff       (20)      302 2023-07-07 18:03:46.000000 threads-py-0.0.2/threadspy/types/get_user_profile_response.py
--rw-r--r--   0 mineru     (501) staff       (20)      315 2023-07-07 17:57:17.000000 threads-py-0.0.2/threadspy/types/get_user_profile_thread_response.py
--rw-r--r--   0 mineru     (501) staff       (20)      314 2023-07-07 17:57:25.000000 threads-py-0.0.2/threadspy/types/get_user_profile_threads_response.py
--rw-r--r--   0 mineru     (501) staff       (20)      233 2023-07-07 16:58:01.000000 threads-py-0.0.2/threadspy/types/image_versions2.py
--rw-r--r--   0 mineru     (501) staff       (20)      216 2023-07-07 16:58:01.000000 threads-py-0.0.2/threadspy/types/media_data.py
--rw-r--r--   0 mineru     (501) staff       (20)      772 2023-07-07 17:21:37.000000 threads-py-0.0.2/threadspy/types/post.py
--rw-r--r--   0 mineru     (501) staff       (20)      766 2023-07-07 17:21:46.000000 threads-py-0.0.2/threadspy/types/quoted_post.py
--rw-r--r--   0 mineru     (501) staff       (20)      189 2023-07-07 08:46:47.000000 threads-py-0.0.2/threadspy/types/reply_facepile_user.py
--rw-r--r--   0 mineru     (501) staff       (20)      812 2023-07-07 17:22:01.000000 threads-py-0.0.2/threadspy/types/reposted_post.py
--rw-r--r--   0 mineru     (501) staff       (20)      304 2023-07-07 16:58:01.000000 threads-py-0.0.2/threadspy/types/share_info.py
--rw-r--r--   0 mineru     (501) staff       (20)      313 2023-07-07 18:29:52.000000 threads-py-0.0.2/threadspy/types/text_post_app_info.py
--rw-r--r--   0 mineru     (501) staff       (20)      299 2023-07-07 16:58:01.000000 threads-py-0.0.2/threadspy/types/thread.py
--rw-r--r--   0 mineru     (501) staff       (20)      280 2023-07-08 18:20:59.000000 threads-py-0.0.2/threadspy/types/thread_data.py
--rw-r--r--   0 mineru     (501) staff       (20)      433 2023-07-07 16:58:01.000000 threads-py-0.0.2/threadspy/types/thread_item.py
--rw-r--r--   0 mineru     (501) staff       (20)      142 2023-07-07 17:23:07.000000 threads-py-0.0.2/threadspy/types/threads_bio_link.py
--rw-r--r--   0 mineru     (501) staff       (20)      185 2023-07-07 17:20:54.000000 threads-py-0.0.2/threadspy/types/threads_hd_profile_pic_version.py
--rw-r--r--   0 mineru     (501) staff       (20)      729 2023-07-08 18:23:31.000000 threads-py-0.0.2/threadspy/types/threads_user.py
--rw-r--r--   0 mineru     (501) staff       (20)      222 2023-07-07 17:20:21.000000 threads-py-0.0.2/threadspy/types/threads_user_summary.py
--rw-r--r--   0 mineru     (501) staff       (20)      198 2023-07-07 16:58:01.000000 threads-py-0.0.2/threadspy/types/user_data.py
--rw-r--r--   0 mineru     (501) staff       (20)      200 2023-07-07 16:58:00.000000 threads-py-0.0.2/threadspy/types/user_profile_data.py
--rw-r--r--   0 mineru     (501) staff       (20)      230 2023-07-07 18:11:06.000000 threads-py-0.0.2/threadspy/types/users.py
--rw-r--r--   0 mineru     (501) staff       (20)      174 2023-07-07 08:44:28.000000 threads-py-0.0.2/threadspy/types/video_version.py
+drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-08 19:40:58.910286 threads-py-0.0.3/
+-rw-r--r--   0 mineru     (501) staff       (20)     1066 2023-07-07 02:31:26.000000 threads-py-0.0.3/LICENSE
+-rw-r--r--   0 mineru     (501) staff       (20)      340 2023-07-08 19:40:58.910150 threads-py-0.0.3/PKG-INFO
+-rw-r--r--   0 mineru     (501) staff       (20)     2436 2023-07-08 19:21:10.000000 threads-py-0.0.3/README.md
+-rw-r--r--   0 mineru     (501) staff       (20)       38 2023-07-08 19:40:58.910327 threads-py-0.0.3/setup.cfg
+-rw-r--r--   0 mineru     (501) staff       (20)      941 2023-07-08 17:19:16.000000 threads-py-0.0.3/setup.py
+drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-08 19:40:58.906156 threads-py-0.0.3/threads_py.egg-info/
+-rw-r--r--   0 mineru     (501) staff       (20)      340 2023-07-08 19:40:58.000000 threads-py-0.0.3/threads_py.egg-info/PKG-INFO
+-rw-r--r--   0 mineru     (501) staff       (20)     1257 2023-07-08 19:40:58.000000 threads-py-0.0.3/threads_py.egg-info/SOURCES.txt
+-rw-r--r--   0 mineru     (501) staff       (20)        1 2023-07-08 19:40:58.000000 threads-py-0.0.3/threads_py.egg-info/dependency_links.txt
+-rw-r--r--   0 mineru     (501) staff       (20)       38 2023-07-08 19:40:58.000000 threads-py-0.0.3/threads_py.egg-info/requires.txt
+-rw-r--r--   0 mineru     (501) staff       (20)       10 2023-07-08 19:40:58.000000 threads-py-0.0.3/threads_py.egg-info/top_level.txt
+drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-08 19:40:58.906430 threads-py-0.0.3/threadspy/
+-rw-r--r--   0 mineru     (501) staff       (20)      111 2023-07-08 19:40:45.000000 threads-py-0.0.3/threadspy/__init__.py
+-rw-r--r--   0 mineru     (501) staff       (20)    10788 2023-07-08 19:26:32.000000 threads-py-0.0.3/threadspy/_thread.py
+drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-08 19:40:58.909962 threads-py-0.0.3/threadspy/types/
+-rw-r--r--   0 mineru     (501) staff       (20)     1250 2023-07-08 18:18:23.000000 threads-py-0.0.3/threadspy/types/__init__.py
+-rw-r--r--   0 mineru     (501) staff       (20)      188 2023-07-07 08:49:18.000000 threads-py-0.0.3/threadspy/types/candidate.py
+-rw-r--r--   0 mineru     (501) staff       (20)      134 2023-07-07 08:34:39.000000 threads-py-0.0.3/threadspy/types/caption.py
+-rw-r--r--   0 mineru     (501) staff       (20)      622 2023-07-07 18:28:28.000000 threads-py-0.0.3/threadspy/types/common.py
+-rw-r--r--   0 mineru     (501) staff       (20)      142 2023-07-07 08:49:13.000000 threads-py-0.0.3/threadspy/types/extensions.py
+-rw-r--r--   0 mineru     (501) staff       (20)      302 2023-07-07 18:26:10.000000 threads-py-0.0.3/threadspy/types/get_thread_likers_response.py
+-rw-r--r--   0 mineru     (501) staff       (20)      314 2023-07-07 17:56:07.000000 threads-py-0.0.3/threadspy/types/get_user_profile_replies_response.py
+-rw-r--r--   0 mineru     (501) staff       (20)      302 2023-07-07 18:03:46.000000 threads-py-0.0.3/threadspy/types/get_user_profile_response.py
+-rw-r--r--   0 mineru     (501) staff       (20)      315 2023-07-07 17:57:17.000000 threads-py-0.0.3/threadspy/types/get_user_profile_thread_response.py
+-rw-r--r--   0 mineru     (501) staff       (20)      314 2023-07-07 17:57:25.000000 threads-py-0.0.3/threadspy/types/get_user_profile_threads_response.py
+-rw-r--r--   0 mineru     (501) staff       (20)      233 2023-07-07 16:58:01.000000 threads-py-0.0.3/threadspy/types/image_versions2.py
+-rw-r--r--   0 mineru     (501) staff       (20)      216 2023-07-07 16:58:01.000000 threads-py-0.0.3/threadspy/types/media_data.py
+-rw-r--r--   0 mineru     (501) staff       (20)      772 2023-07-07 17:21:37.000000 threads-py-0.0.3/threadspy/types/post.py
+-rw-r--r--   0 mineru     (501) staff       (20)      766 2023-07-07 17:21:46.000000 threads-py-0.0.3/threadspy/types/quoted_post.py
+-rw-r--r--   0 mineru     (501) staff       (20)      189 2023-07-07 08:46:47.000000 threads-py-0.0.3/threadspy/types/reply_facepile_user.py
+-rw-r--r--   0 mineru     (501) staff       (20)      812 2023-07-07 17:22:01.000000 threads-py-0.0.3/threadspy/types/reposted_post.py
+-rw-r--r--   0 mineru     (501) staff       (20)      304 2023-07-07 16:58:01.000000 threads-py-0.0.3/threadspy/types/share_info.py
+-rw-r--r--   0 mineru     (501) staff       (20)      313 2023-07-07 18:29:52.000000 threads-py-0.0.3/threadspy/types/text_post_app_info.py
+-rw-r--r--   0 mineru     (501) staff       (20)      299 2023-07-07 16:58:01.000000 threads-py-0.0.3/threadspy/types/thread.py
+-rw-r--r--   0 mineru     (501) staff       (20)      280 2023-07-08 18:20:59.000000 threads-py-0.0.3/threadspy/types/thread_data.py
+-rw-r--r--   0 mineru     (501) staff       (20)      433 2023-07-07 16:58:01.000000 threads-py-0.0.3/threadspy/types/thread_item.py
+-rw-r--r--   0 mineru     (501) staff       (20)      142 2023-07-07 17:23:07.000000 threads-py-0.0.3/threadspy/types/threads_bio_link.py
+-rw-r--r--   0 mineru     (501) staff       (20)      185 2023-07-07 17:20:54.000000 threads-py-0.0.3/threadspy/types/threads_hd_profile_pic_version.py
+-rw-r--r--   0 mineru     (501) staff       (20)      729 2023-07-08 18:23:31.000000 threads-py-0.0.3/threadspy/types/threads_user.py
+-rw-r--r--   0 mineru     (501) staff       (20)      222 2023-07-07 17:20:21.000000 threads-py-0.0.3/threadspy/types/threads_user_summary.py
+-rw-r--r--   0 mineru     (501) staff       (20)      198 2023-07-07 16:58:01.000000 threads-py-0.0.3/threadspy/types/user_data.py
+-rw-r--r--   0 mineru     (501) staff       (20)      200 2023-07-07 16:58:00.000000 threads-py-0.0.3/threadspy/types/user_profile_data.py
+-rw-r--r--   0 mineru     (501) staff       (20)      230 2023-07-07 18:11:06.000000 threads-py-0.0.3/threadspy/types/users.py
+-rw-r--r--   0 mineru     (501) staff       (20)      174 2023-07-07 08:44:28.000000 threads-py-0.0.3/threadspy/types/video_version.py
```

### Comparing `threads-py-0.0.2/LICENSE` & `threads-py-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `threads-py-0.0.2/README.md` & `threads-py-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `threads-py-0.0.2/setup.py` & `threads-py-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `threads-py-0.0.2/threads_py.egg-info/SOURCES.txt` & `threads-py-0.0.3/threads_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `threads-py-0.0.2/threadspy/_thread.py` & `threads-py-0.0.3/threadspy/_thread.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,15 @@
             print("[fbLSDToken] USING", self.fbLSDToken)
         headers = self.__get_default_headers(username)
         headers["x-fb-friendly-name"] = "BarcelonaProfileRepliesTabQuery"
 
         params = {
             "lsd": f"{self.fbLSDToken}",
             "variables": f'{{"userID":"{user_id}"}}',
-            "doc_id": "6307072669391286",
+            "doc_id": "6684830921547925",
         }
 
         response = self.http_client.post(
             "https://www.threads.net/api/graphql", params=params, headers=headers
         )
 
         try:
```

### Comparing `threads-py-0.0.2/threadspy/types/__init__.py` & `threads-py-0.0.3/threadspy/types/__init__.py`

 * *Files identical despite different names*

### Comparing `threads-py-0.0.2/threadspy/types/common.py` & `threads-py-0.0.3/threadspy/types/common.py`

 * *Files identical despite different names*

### Comparing `threads-py-0.0.2/threadspy/types/post.py` & `threads-py-0.0.3/threadspy/types/post.py`

 * *Files identical despite different names*

### Comparing `threads-py-0.0.2/threadspy/types/quoted_post.py` & `threads-py-0.0.3/threadspy/types/quoted_post.py`

 * *Files identical despite different names*

### Comparing `threads-py-0.0.2/threadspy/types/reposted_post.py` & `threads-py-0.0.3/threadspy/types/reposted_post.py`

 * *Files identical despite different names*

### Comparing `threads-py-0.0.2/threadspy/types/threads_user.py` & `threads-py-0.0.3/threadspy/types/threads_user.py`

 * *Files identical despite different names*

