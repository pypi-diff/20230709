# Comparing `tmp/threads-py-0.0.5.tar.gz` & `tmp/threads-py-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threads-py-0.0.5.tar", last modified: Sun Jul  9 05:27:23 2023, max compression
+gzip compressed data, was "threads-py-0.0.6.tar", last modified: Sun Jul  9 16:08:34 2023, max compression
```

## Comparing `threads-py-0.0.5.tar` & `threads-py-0.0.6.tar`

### file list

```diff
@@ -1,46 +1,52 @@
-drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-09 05:27:23.586537 threads-py-0.0.5/
--rw-r--r--   0 mineru     (501) staff       (20)     1066 2023-07-07 02:31:26.000000 threads-py-0.0.5/LICENSE
--rw-r--r--   0 mineru     (501) staff       (20)      340 2023-07-09 05:27:23.586393 threads-py-0.0.5/PKG-INFO
--rw-r--r--   0 mineru     (501) staff       (20)     2880 2023-07-09 03:41:22.000000 threads-py-0.0.5/README.md
--rw-r--r--   0 mineru     (501) staff       (20)       38 2023-07-09 05:27:23.586584 threads-py-0.0.5/setup.cfg
--rw-r--r--   0 mineru     (501) staff       (20)      953 2023-07-09 03:47:40.000000 threads-py-0.0.5/setup.py
-drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-09 05:27:23.581957 threads-py-0.0.5/threads_py.egg-info/
--rw-r--r--   0 mineru     (501) staff       (20)      340 2023-07-09 05:27:23.000000 threads-py-0.0.5/threads_py.egg-info/PKG-INFO
--rw-r--r--   0 mineru     (501) staff       (20)     1280 2023-07-09 05:27:23.000000 threads-py-0.0.5/threads_py.egg-info/SOURCES.txt
--rw-r--r--   0 mineru     (501) staff       (20)        1 2023-07-09 05:27:23.000000 threads-py-0.0.5/threads_py.egg-info/dependency_links.txt
--rw-r--r--   0 mineru     (501) staff       (20)       47 2023-07-09 05:27:23.000000 threads-py-0.0.5/threads_py.egg-info/requires.txt
--rw-r--r--   0 mineru     (501) staff       (20)       10 2023-07-09 05:27:23.000000 threads-py-0.0.5/threads_py.egg-info/top_level.txt
-drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-09 05:27:23.582337 threads-py-0.0.5/threadspy/
--rw-r--r--   0 mineru     (501) staff       (20)      111 2023-07-09 05:27:01.000000 threads-py-0.0.5/threadspy/__init__.py
--rw-r--r--   0 mineru     (501) staff       (20)      676 2023-07-09 04:04:29.000000 threads-py-0.0.5/threadspy/_constant.py
--rw-r--r--   0 mineru     (501) staff       (20)    22076 2023-07-09 05:25:26.000000 threads-py-0.0.5/threadspy/_thread.py
-drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-09 05:27:23.586188 threads-py-0.0.5/threadspy/types/
--rw-r--r--   0 mineru     (501) staff       (20)     1250 2023-07-08 19:54:05.000000 threads-py-0.0.5/threadspy/types/__init__.py
--rw-r--r--   0 mineru     (501) staff       (20)      188 2023-07-07 08:49:18.000000 threads-py-0.0.5/threadspy/types/candidate.py
--rw-r--r--   0 mineru     (501) staff       (20)      134 2023-07-07 08:34:39.000000 threads-py-0.0.5/threadspy/types/caption.py
--rw-r--r--   0 mineru     (501) staff       (20)      622 2023-07-07 18:28:28.000000 threads-py-0.0.5/threadspy/types/common.py
--rw-r--r--   0 mineru     (501) staff       (20)      142 2023-07-07 08:49:13.000000 threads-py-0.0.5/threadspy/types/extensions.py
--rw-r--r--   0 mineru     (501) staff       (20)      302 2023-07-07 18:26:10.000000 threads-py-0.0.5/threadspy/types/get_thread_likers_response.py
--rw-r--r--   0 mineru     (501) staff       (20)      314 2023-07-07 17:56:07.000000 threads-py-0.0.5/threadspy/types/get_user_profile_replies_response.py
--rw-r--r--   0 mineru     (501) staff       (20)      302 2023-07-07 18:03:46.000000 threads-py-0.0.5/threadspy/types/get_user_profile_response.py
--rw-r--r--   0 mineru     (501) staff       (20)      315 2023-07-07 17:57:17.000000 threads-py-0.0.5/threadspy/types/get_user_profile_thread_response.py
--rw-r--r--   0 mineru     (501) staff       (20)      314 2023-07-07 17:57:25.000000 threads-py-0.0.5/threadspy/types/get_user_profile_threads_response.py
--rw-r--r--   0 mineru     (501) staff       (20)      233 2023-07-07 16:58:01.000000 threads-py-0.0.5/threadspy/types/image_versions2.py
--rw-r--r--   0 mineru     (501) staff       (20)      216 2023-07-07 16:58:01.000000 threads-py-0.0.5/threadspy/types/media_data.py
--rw-r--r--   0 mineru     (501) staff       (20)      772 2023-07-07 17:21:37.000000 threads-py-0.0.5/threadspy/types/post.py
--rw-r--r--   0 mineru     (501) staff       (20)      766 2023-07-07 17:21:46.000000 threads-py-0.0.5/threadspy/types/quoted_post.py
--rw-r--r--   0 mineru     (501) staff       (20)      189 2023-07-07 08:46:47.000000 threads-py-0.0.5/threadspy/types/reply_facepile_user.py
--rw-r--r--   0 mineru     (501) staff       (20)      812 2023-07-07 17:22:01.000000 threads-py-0.0.5/threadspy/types/reposted_post.py
--rw-r--r--   0 mineru     (501) staff       (20)      304 2023-07-07 16:58:01.000000 threads-py-0.0.5/threadspy/types/share_info.py
--rw-r--r--   0 mineru     (501) staff       (20)      313 2023-07-07 18:29:52.000000 threads-py-0.0.5/threadspy/types/text_post_app_info.py
--rw-r--r--   0 mineru     (501) staff       (20)      299 2023-07-07 16:58:01.000000 threads-py-0.0.5/threadspy/types/thread.py
--rw-r--r--   0 mineru     (501) staff       (20)      280 2023-07-08 19:54:05.000000 threads-py-0.0.5/threadspy/types/thread_data.py
--rw-r--r--   0 mineru     (501) staff       (20)      433 2023-07-07 16:58:01.000000 threads-py-0.0.5/threadspy/types/thread_item.py
--rw-r--r--   0 mineru     (501) staff       (20)      142 2023-07-07 17:23:07.000000 threads-py-0.0.5/threadspy/types/threads_bio_link.py
--rw-r--r--   0 mineru     (501) staff       (20)      185 2023-07-07 17:20:54.000000 threads-py-0.0.5/threadspy/types/threads_hd_profile_pic_version.py
--rw-r--r--   0 mineru     (501) staff       (20)      729 2023-07-08 18:23:31.000000 threads-py-0.0.5/threadspy/types/threads_user.py
--rw-r--r--   0 mineru     (501) staff       (20)      222 2023-07-07 17:20:21.000000 threads-py-0.0.5/threadspy/types/threads_user_summary.py
--rw-r--r--   0 mineru     (501) staff       (20)      198 2023-07-07 16:58:01.000000 threads-py-0.0.5/threadspy/types/user_data.py
--rw-r--r--   0 mineru     (501) staff       (20)      200 2023-07-07 16:58:00.000000 threads-py-0.0.5/threadspy/types/user_profile_data.py
--rw-r--r--   0 mineru     (501) staff       (20)      230 2023-07-07 18:11:06.000000 threads-py-0.0.5/threadspy/types/users.py
--rw-r--r--   0 mineru     (501) staff       (20)      174 2023-07-07 08:44:28.000000 threads-py-0.0.5/threadspy/types/video_version.py
+drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-09 16:08:34.616391 threads-py-0.0.6/
+-rw-r--r--   0 mineru     (501) staff       (20)     1066 2023-07-07 02:31:26.000000 threads-py-0.0.6/LICENSE
+-rw-r--r--   0 mineru     (501) staff       (20)      340 2023-07-09 16:08:34.616238 threads-py-0.0.6/PKG-INFO
+-rw-r--r--   0 mineru     (501) staff       (20)     3730 2023-07-09 08:19:43.000000 threads-py-0.0.6/README.md
+drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-09 16:08:34.610067 threads-py-0.0.6/models/
+-rw-r--r--   0 mineru     (501) staff       (20)        0 2023-07-09 08:19:43.000000 threads-py-0.0.6/models/__init__.py
+-rw-r--r--   0 mineru     (501) staff       (20)       38 2023-07-09 16:08:34.616445 threads-py-0.0.6/setup.cfg
+-rw-r--r--   0 mineru     (501) staff       (20)      941 2023-07-09 05:30:57.000000 threads-py-0.0.6/setup.py
+drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-09 16:08:34.610780 threads-py-0.0.6/threads_py.egg-info/
+-rw-r--r--   0 mineru     (501) staff       (20)      340 2023-07-09 16:08:34.000000 threads-py-0.0.6/threads_py.egg-info/PKG-INFO
+-rw-r--r--   0 mineru     (501) staff       (20)     1378 2023-07-09 16:08:34.000000 threads-py-0.0.6/threads_py.egg-info/SOURCES.txt
+-rw-r--r--   0 mineru     (501) staff       (20)        1 2023-07-09 16:08:34.000000 threads-py-0.0.6/threads_py.egg-info/dependency_links.txt
+-rw-r--r--   0 mineru     (501) staff       (20)       38 2023-07-09 16:08:34.000000 threads-py-0.0.6/threads_py.egg-info/requires.txt
+-rw-r--r--   0 mineru     (501) staff       (20)       17 2023-07-09 16:08:34.000000 threads-py-0.0.6/threads_py.egg-info/top_level.txt
+drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-09 16:08:34.611271 threads-py-0.0.6/threadspy/
+-rw-r--r--   0 mineru     (501) staff       (20)      167 2023-07-09 16:08:18.000000 threads-py-0.0.6/threadspy/__init__.py
+-rw-r--r--   0 mineru     (501) staff       (20)     5500 2023-07-09 15:58:32.000000 threads-py-0.0.6/threadspy/_agent.py
+-rw-r--r--   0 mineru     (501) staff       (20)      676 2023-07-09 07:59:50.000000 threads-py-0.0.6/threadspy/_constant.py
+-rw-r--r--   0 mineru     (501) staff       (20)    21217 2023-07-09 15:58:58.000000 threads-py-0.0.6/threadspy/_thread.py
+drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-09 16:08:34.611536 threads-py-0.0.6/threadspy/templates/
+-rw-r--r--   0 mineru     (501) staff       (20)       29 2023-07-09 08:19:43.000000 threads-py-0.0.6/threadspy/templates/__init__.py
+-rw-r--r--   0 mineru     (501) staff       (20)      128 2023-07-09 08:19:43.000000 threads-py-0.0.6/threadspy/templates/qna.py
+drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-09 16:08:34.616027 threads-py-0.0.6/threadspy/types/
+-rw-r--r--   0 mineru     (501) staff       (20)     1250 2023-07-08 19:54:05.000000 threads-py-0.0.6/threadspy/types/__init__.py
+-rw-r--r--   0 mineru     (501) staff       (20)      188 2023-07-07 08:49:18.000000 threads-py-0.0.6/threadspy/types/candidate.py
+-rw-r--r--   0 mineru     (501) staff       (20)      134 2023-07-07 08:34:39.000000 threads-py-0.0.6/threadspy/types/caption.py
+-rw-r--r--   0 mineru     (501) staff       (20)      622 2023-07-07 18:28:28.000000 threads-py-0.0.6/threadspy/types/common.py
+-rw-r--r--   0 mineru     (501) staff       (20)      142 2023-07-07 08:49:13.000000 threads-py-0.0.6/threadspy/types/extensions.py
+-rw-r--r--   0 mineru     (501) staff       (20)      302 2023-07-07 18:26:10.000000 threads-py-0.0.6/threadspy/types/get_thread_likers_response.py
+-rw-r--r--   0 mineru     (501) staff       (20)      314 2023-07-07 17:56:07.000000 threads-py-0.0.6/threadspy/types/get_user_profile_replies_response.py
+-rw-r--r--   0 mineru     (501) staff       (20)      302 2023-07-07 18:03:46.000000 threads-py-0.0.6/threadspy/types/get_user_profile_response.py
+-rw-r--r--   0 mineru     (501) staff       (20)      315 2023-07-07 17:57:17.000000 threads-py-0.0.6/threadspy/types/get_user_profile_thread_response.py
+-rw-r--r--   0 mineru     (501) staff       (20)      314 2023-07-07 17:57:25.000000 threads-py-0.0.6/threadspy/types/get_user_profile_threads_response.py
+-rw-r--r--   0 mineru     (501) staff       (20)      233 2023-07-07 16:58:01.000000 threads-py-0.0.6/threadspy/types/image_versions2.py
+-rw-r--r--   0 mineru     (501) staff       (20)      216 2023-07-07 16:58:01.000000 threads-py-0.0.6/threadspy/types/media_data.py
+-rw-r--r--   0 mineru     (501) staff       (20)      772 2023-07-07 17:21:37.000000 threads-py-0.0.6/threadspy/types/post.py
+-rw-r--r--   0 mineru     (501) staff       (20)      766 2023-07-07 17:21:46.000000 threads-py-0.0.6/threadspy/types/quoted_post.py
+-rw-r--r--   0 mineru     (501) staff       (20)      189 2023-07-07 08:46:47.000000 threads-py-0.0.6/threadspy/types/reply_facepile_user.py
+-rw-r--r--   0 mineru     (501) staff       (20)      812 2023-07-07 17:22:01.000000 threads-py-0.0.6/threadspy/types/reposted_post.py
+-rw-r--r--   0 mineru     (501) staff       (20)      304 2023-07-07 16:58:01.000000 threads-py-0.0.6/threadspy/types/share_info.py
+-rw-r--r--   0 mineru     (501) staff       (20)      313 2023-07-07 18:29:52.000000 threads-py-0.0.6/threadspy/types/text_post_app_info.py
+-rw-r--r--   0 mineru     (501) staff       (20)      299 2023-07-07 16:58:01.000000 threads-py-0.0.6/threadspy/types/thread.py
+-rw-r--r--   0 mineru     (501) staff       (20)      280 2023-07-08 19:54:05.000000 threads-py-0.0.6/threadspy/types/thread_data.py
+-rw-r--r--   0 mineru     (501) staff       (20)      433 2023-07-07 16:58:01.000000 threads-py-0.0.6/threadspy/types/thread_item.py
+-rw-r--r--   0 mineru     (501) staff       (20)      142 2023-07-07 17:23:07.000000 threads-py-0.0.6/threadspy/types/threads_bio_link.py
+-rw-r--r--   0 mineru     (501) staff       (20)      185 2023-07-07 17:20:54.000000 threads-py-0.0.6/threadspy/types/threads_hd_profile_pic_version.py
+-rw-r--r--   0 mineru     (501) staff       (20)      729 2023-07-08 18:23:31.000000 threads-py-0.0.6/threadspy/types/threads_user.py
+-rw-r--r--   0 mineru     (501) staff       (20)      222 2023-07-07 17:20:21.000000 threads-py-0.0.6/threadspy/types/threads_user_summary.py
+-rw-r--r--   0 mineru     (501) staff       (20)      198 2023-07-07 16:58:01.000000 threads-py-0.0.6/threadspy/types/user_data.py
+-rw-r--r--   0 mineru     (501) staff       (20)      200 2023-07-07 16:58:00.000000 threads-py-0.0.6/threadspy/types/user_profile_data.py
+-rw-r--r--   0 mineru     (501) staff       (20)      230 2023-07-07 18:11:06.000000 threads-py-0.0.6/threadspy/types/users.py
+-rw-r--r--   0 mineru     (501) staff       (20)      174 2023-07-07 08:44:28.000000 threads-py-0.0.6/threadspy/types/video_version.py
```

### Comparing `threads-py-0.0.5/LICENSE` & `threads-py-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `threads-py-0.0.5/setup.py` & `threads-py-0.0.6/setup.py`

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
-    install_requires=["requests", "dataclasses", "dataclasses-json", "aiofiles"],
+    install_requires=["requests", "dataclasses", "dataclasses-json"],
     python_requires=">=3.8",
 )
```

### Comparing `threads-py-0.0.5/threads_py.egg-info/SOURCES.txt` & `threads-py-0.0.6/threads_py.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 LICENSE
 README.md
 setup.py
+models/__init__.py
 threads_py.egg-info/PKG-INFO
 threads_py.egg-info/SOURCES.txt
 threads_py.egg-info/dependency_links.txt
 threads_py.egg-info/requires.txt
 threads_py.egg-info/top_level.txt
 threadspy/__init__.py
+threadspy/_agent.py
 threadspy/_constant.py
 threadspy/_thread.py
+threadspy/templates/__init__.py
+threadspy/templates/qna.py
 threadspy/types/__init__.py
 threadspy/types/candidate.py
 threadspy/types/caption.py
 threadspy/types/common.py
 threadspy/types/extensions.py
 threadspy/types/get_thread_likers_response.py
 threadspy/types/get_user_profile_replies_response.py
```

### Comparing `threads-py-0.0.5/threadspy/_constant.py` & `threads-py-0.0.6/threadspy/_constant.py`

 * *Files identical despite different names*

### Comparing `threads-py-0.0.5/threadspy/_thread.py` & `threads-py-0.0.6/threadspy/_thread.py`

 * *Files 9% similar despite different names*

```diff
@@ -113,23 +113,23 @@
                 "pragma": "no-cache",
                 "referer": f"https://www.threads.net/@{username}",
                 "x-asbd-id": "129477",
                 "x-fb-lsd": self.fbLSDToken,
                 "x-ig-app-id": "238260118697367",
             }
 
-    def get_user_id_from_username(self, username) -> bool:
+    def get_user_id_from_username(self, username) -> str:
         """
         set user id by username.
 
         Args:
             username (str): username on threads.net
 
         Returns:
-            bool: validate user_id
+            string: user_id if not valid return None
         """
         headers = self.__get_default_headers(username)
         headers[
             "accept"
         ] = "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7"
         headers["accept-language"] = "ko,en;q=0.9,ko-KR;q=0.8,ja;q=0.7"
         headers["pragma"] = "no-cache"
@@ -154,17 +154,17 @@
 
         if not self.noUpdateLSD and self.fbLSDToken is not None:
             self.fbLSDToken = lsd_token
             if self.verbose:
                 print("[fbLSDToken] UPDATED", self.fbLSDToken)
         if user_id is not None:
             self.user_id = user_id
-            return True
+            return self.user_id
         else:
-            return False
+            return None
 
     def get_user_profile(self, username, user_id=None) -> ThreadsUser:
         """
         Returns profile info by username.
 
         Args:
             username (str): username on threads.net
@@ -378,23 +378,23 @@
             thread = GetThreadLikersResponse.from_dict(response.json())
             return thread.data.likers
         except Exception as e:
             if self.verbose:
                 print("[ERROR] ", e)
             return UsersData(users=[])
 
-    def get_token(self) -> bool:
+    def get_token(self) -> str:
         """
         set fb login token
 
         Returns:
-            bool: validate token
+            str: validate token string None if not valid
         """
         if self.username is None or self.password is None:
-            return False
+            return None
         try:
             blockVersion = "5f56efad68e1edec7801f630b5c122704ec5378adbee6609a448f105f34a9c73"
             headers = {
                 "User-Agent": "Barcelona 289.0.0.77.109 Android",
                 "Sec-Fetch-Site": "same-origin",
                 "Content-Type": "application/x-www-form-urlencoded; charset=UTF-8",
             }
@@ -411,49 +411,48 @@
                     },
                 }
             )
             bk_client_context = json.dumps(
                 {"bloks_version": blockVersion, "styles_id": "instagram"}
             )
             payload = f"params={urllib.parse.quote(params)}&bk_client_context={urllib.parse.quote(bk_client_context)}&bloks_versioning_id={blockVersion}"
-
             response = requests.post(LOGIN_URL, timeout=60 * 1000, headers=headers, data=payload)
             data = response.text
             if data == "Oops, an error occurred.":
                 return None
             pos = data.split("Bearer IGT:2:")
             if len(pos) > 1:
                 pos = pos[1]
                 pos = pos.split("==")[0]
                 token = f"{pos}=="
                 self.token = token
-                return True
-            return False
+                return self.token
+            return None
         except Exception as e:
             print("[ERROR] ", e)
-            return False
+            return None
 
     def publish(self, caption: str) -> bool:
         """
         Returns publish post
 
         Args:
             caption (str): post_id which is unique to each post.
 
         Returns:
             bool: verify that the post went publish
         """
         if self.username is None or self.password is None:
             return False
 
-        is_valid_user_id = self.get_user_id_from_username(self.username)
-        if not is_valid_user_id:
+        user_id = self.get_user_id_from_username(self.username)
+        if user_id is None:
             return False
-        is_valid_token = self.get_token()
-        if not is_valid_token:
+        token = self.get_token()
+        if token is None:
             return False
         params = json.dumps(
             {
                 "publish_mode": "text_post",
                 "text_post_app_info": '{"reply_control":0}',
                 "timezone_offset": "-25200",
                 "source_type": "4",
@@ -492,19 +491,19 @@
             image_path (str): image path
 
         Returns:
             bool: verify that the post with image went publish
         """
         if self.username is None or self.password is None:
             return False
-        is_valid_user_id = self.get_user_id_from_username(self.username)
-        if not is_valid_user_id:
+        user_id = self.get_user_id_from_username(self.username)
+        if user_id is None:
             return False
-        is_valid_token = self.get_token()
-        if not is_valid_token:
+        token = self.get_token()
+        if token is None:
             return False
         image_content = None
         if not (os.path.isfile(image_path) and os.path.exists(image_path)):
             if not self.__is_valid_url(image_path):
                 return False
             else:
                 image_content = self.__download(image_path)
@@ -582,14 +581,16 @@
                 "num_step_auto_retry": "0",
                 "num_reupload": "0",
                 "num_step_manual_retry": "0",
             },
             "IG-FB-Xpost-entry-point-v2": "feed",
         }
         contentLength = len(content)
+        if mime_type.startswith("image/"):
+            mime_type = mime_type.replace("image/", "")
         image_headers = {
             "X_FB_PHOTO_WATERFALL_ID": str(uuid.uuid4()),
             "X-Entity-Type": "image/" + mime_type,
             "Offset": "0",
             "X-Instagram-Rupload-Params": json.dumps(x_instagram_rupload_params),
             "X-Entity-Name": f"{name}",
             "X-Entity-Length": f"{contentLength}",
@@ -600,32 +601,7 @@
 
         headers.update(image_headers)
         response = self.http_client.post(url, headers=headers, data=content)
         if response.status_code == 200:
             return response.text
         else:
             return None
-
-    def update_media_with_pdq_hash_info(self, upload_id="87490918227685"):
-        headers = POST_HEADERS_DEFAULT.copy()
-        headers.update({"Authorization": f"Bearer IGT:2:{self.token}"})
-
-        pdq_hash_info = {
-            "pdq_hash": "17b1b91bb94b46e417b1319346b4ce6ce84eec4e46b413b117b1b91bb94b46e4:89",
-            "frame_time": 0,
-        }
-        body_data = {
-            "pdq_hash_info": json.dumps(pdq_hash_info),
-            "_uid": self.user_id,
-            "_uuid": "3d8ce049-3663-4cfe-9417-08d152df3874",
-            "upload_id": f"{upload_id}",
-        }
-
-        body = {"signed_body": f"SIGNATURE.{json.dumps(body_data)}"}
-        response = self.http_client.post(
-            "https://i.instagram.com/api/v1/media/update_media_with_pdq_hash_info/",
-            headers=headers,
-            data=body,
-        )
-        if response.status_code == 200:
-            post_result = response.json()
-            return post_result
```

### Comparing `threads-py-0.0.5/threadspy/types/__init__.py` & `threads-py-0.0.6/threadspy/types/__init__.py`

 * *Files identical despite different names*

### Comparing `threads-py-0.0.5/threadspy/types/common.py` & `threads-py-0.0.6/threadspy/types/common.py`

 * *Files identical despite different names*

### Comparing `threads-py-0.0.5/threadspy/types/post.py` & `threads-py-0.0.6/threadspy/types/post.py`

 * *Files identical despite different names*

### Comparing `threads-py-0.0.5/threadspy/types/quoted_post.py` & `threads-py-0.0.6/threadspy/types/quoted_post.py`

 * *Files identical despite different names*

### Comparing `threads-py-0.0.5/threadspy/types/reposted_post.py` & `threads-py-0.0.6/threadspy/types/reposted_post.py`

 * *Files identical despite different names*

### Comparing `threads-py-0.0.5/threadspy/types/threads_user.py` & `threads-py-0.0.6/threadspy/types/threads_user.py`

 * *Files identical despite different names*

