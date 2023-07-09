# Comparing `tmp/pymino-1.2.3.1.tar.gz` & `tmp/pymino-1.2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymino-1.2.3.1.tar", last modified: Thu Jul  6 22:46:04 2023, max compression
+gzip compressed data, was "C:\Users\12095\Desktop\rr\pymino\dist\.tmp-l7srb8sc\pymino-1.2.3.2.tar", last modified: Sun Jul  9 18:22:13 2023, max compression
```

## Comparing `pymino-1.2.3.1.tar` & `pymino-1.2.3.2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 22:46:04.633788 pymino-1.2.3.1/
--rw-rw-rw-   0        0        0     1085 2023-07-06 22:24:35.000000 pymino-1.2.3.1/LICENSE
--rw-rw-rw-   0        0        0     7424 2023-07-06 22:46:04.635789 pymino-1.2.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     6706 2023-07-06 22:44:02.000000 pymino-1.2.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 22:46:04.525555 pymino-1.2.3.1/pymino/
--rw-rw-rw-   0        0        0      775 2023-07-06 22:40:10.000000 pymino-1.2.3.1/pymino/__init__.py
--rw-rw-rw-   0        0        0    11744 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/async_bot.py
--rw-rw-rw-   0        0        0    37317 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/async_client.py
--rw-rw-rw-   0        0        0    31005 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/bot.py
--rw-rw-rw-   0        0        0    36840 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/client.py
-drwxrwxrwx   0        0        0        0 2023-07-06 22:46:04.579925 pymino-1.2.3.1/pymino/ext/
--rw-rw-rw-   0        0        0      651 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/__init__.py
--rw-rw-rw-   0        0        0      192 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/_global.py
--rw-rw-rw-   0        0        0    11196 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/account.py
--rw-rw-rw-   0        0        0    11496 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/async_account.py
--rw-rw-rw-   0        0        0   345260 2023-07-06 22:39:40.000000 pymino-1.2.3.1/pymino/ext/async_community.py
--rw-rw-rw-   0        0        0    21402 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/async_context.py
--rw-rw-rw-   0        0        0    25878 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/async_event_handler.py
--rw-rw-rw-   0        0        0    67975 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/async_global_client.py
--rw-rw-rw-   0        0        0     7233 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/async_socket.py
--rw-rw-rw-   0        0        0   344192 2023-07-06 22:40:58.000000 pymino-1.2.3.1/pymino/ext/community.py
--rw-rw-rw-   0        0        0     3040 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/console.py
--rw-rw-rw-   0        0        0    45520 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/context.py
--rw-rw-rw-   0        0        0     1856 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-07-06 22:46:04.613834 pymino-1.2.3.1/pymino/ext/entities/
--rw-rw-rw-   0        0        0      428 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/entities/__init__.py
--rw-rw-rw-   0        0        0     8044 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/entities/acm.py
--rw-rw-rw-   0        0        0     9014 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/entities/admin_log.py
--rw-rw-rw-   0        0        0     1670 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/entities/api_response.py
--rw-rw-rw-   0        0        0    17769 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/entities/bubble.py
--rw-rw-rw-   0        0        0    20322 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/entities/chat_threads.py
--rw-rw-rw-   0        0        0    13223 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/entities/comments.py
--rw-rw-rw-   0        0        0      765 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/entities/enums.py
--rw-rw-rw-   0        0        0    16021 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/entities/exceptions.py
--rw-rw-rw-   0        0        0    43596 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/entities/general.py
--rw-rw-rw-   0        0        0     4802 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/entities/handlers.py
--rw-rw-rw-   0        0        0     5127 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/entities/link_info.py
--rw-rw-rw-   0        0        0     3831 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/entities/member.py
--rw-rw-rw-   0        0        0    42520 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/entities/messages.py
--rw-rw-rw-   0        0        0     1839 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/entities/notification.py
--rw-rw-rw-   0        0        0    31711 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/entities/sticker.py
--rw-rw-rw-   0        0        0     6185 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/entities/threads.py
--rw-rw-rw-   0        0        0    31609 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/entities/userprofile.py
--rw-rw-rw-   0        0        0     2451 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/entities/wsevents.py
--rw-rw-rw-   0        0        0    70299 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/global_client.py
--rw-rw-rw-   0        0        0      543 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/handle_queue.py
--rw-rw-rw-   0        0        0     6657 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/socket.py
-drwxrwxrwx   0        0        0        0 2023-07-06 22:46:04.631793 pymino-1.2.3.1/pymino/ext/utilities/
--rw-rw-rw-   0        0        0      234 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/utilities/__init__.py
--rw-rw-rw-   0        0        0    11544 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/utilities/async_request_handler.py
--rw-rw-rw-   0        0        0    11309 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/utilities/chat_console.py
--rw-rw-rw-   0        0        0     6280 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/utilities/commands.py
--rw-rw-rw-   0        0        0     2078 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/utilities/community_console.py
--rw-rw-rw-   0        0        0     1110 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/utilities/generate.py
--rw-rw-rw-   0        0        0     2911 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/utilities/menu.py
--rw-rw-rw-   0        0        0     2106 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/utilities/profile_console.py
--rw-rw-rw-   0        0        0    10404 2023-07-06 22:24:35.000000 pymino-1.2.3.1/pymino/ext/utilities/request_handler.py
-drwxrwxrwx   0        0        0        0 2023-07-06 22:46:04.547018 pymino-1.2.3.1/pymino.egg-info/
--rw-rw-rw-   0        0        0     7424 2023-07-06 22:46:04.000000 pymino-1.2.3.1/pymino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1640 2023-07-06 22:46:04.000000 pymino-1.2.3.1/pymino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 22:46:04.000000 pymino-1.2.3.1/pymino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      117 2023-07-06 22:46:04.000000 pymino-1.2.3.1/pymino.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-06 22:46:04.000000 pymino-1.2.3.1/pymino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      873 2023-07-06 22:46:04.645268 pymino-1.2.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1394 2023-07-06 22:24:35.000000 pymino-1.2.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:22:13.291209 pymino-1.2.3.2/
+-rw-rw-rw-   0        0        0     1085 2023-07-09 18:10:54.000000 pymino-1.2.3.2/LICENSE
+-rw-rw-rw-   0        0        0     7373 2023-07-09 18:22:13.291705 pymino-1.2.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6706 2023-07-09 18:21:53.000000 pymino-1.2.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 18:22:13.215325 pymino-1.2.3.2/pymino/
+-rw-rw-rw-   0        0        0      775 2023-07-09 18:20:43.000000 pymino-1.2.3.2/pymino/__init__.py
+-rw-rw-rw-   0        0        0    11744 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/async_bot.py
+-rw-rw-rw-   0        0        0    37317 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/async_client.py
+-rw-rw-rw-   0        0        0    31005 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/bot.py
+-rw-rw-rw-   0        0        0    36840 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/client.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:22:13.253018 pymino-1.2.3.2/pymino/ext/
+-rw-rw-rw-   0        0        0      651 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/__init__.py
+-rw-rw-rw-   0        0        0      192 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/_global.py
+-rw-rw-rw-   0        0        0    11196 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/account.py
+-rw-rw-rw-   0        0        0    11496 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/async_account.py
+-rw-rw-rw-   0        0        0   345197 2023-07-09 18:16:52.000000 pymino-1.2.3.2/pymino/ext/async_community.py
+-rw-rw-rw-   0        0        0    21402 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/async_context.py
+-rw-rw-rw-   0        0        0    25878 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/async_event_handler.py
+-rw-rw-rw-   0        0        0    67975 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/async_global_client.py
+-rw-rw-rw-   0        0        0     7233 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/async_socket.py
+-rw-rw-rw-   0        0        0   344129 2023-07-09 18:16:44.000000 pymino-1.2.3.2/pymino/ext/community.py
+-rw-rw-rw-   0        0        0     3040 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/console.py
+-rw-rw-rw-   0        0        0    45520 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/context.py
+-rw-rw-rw-   0        0        0     1856 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:22:13.277818 pymino-1.2.3.2/pymino/ext/entities/
+-rw-rw-rw-   0        0        0      428 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/entities/__init__.py
+-rw-rw-rw-   0        0        0     8044 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/entities/acm.py
+-rw-rw-rw-   0        0        0     9014 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/entities/admin_log.py
+-rw-rw-rw-   0        0        0     1670 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/entities/api_response.py
+-rw-rw-rw-   0        0        0    17769 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/entities/bubble.py
+-rw-rw-rw-   0        0        0    20322 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/entities/chat_threads.py
+-rw-rw-rw-   0        0        0    13223 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/entities/comments.py
+-rw-rw-rw-   0        0        0      765 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/entities/enums.py
+-rw-rw-rw-   0        0        0    16021 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/entities/exceptions.py
+-rw-rw-rw-   0        0        0    43596 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/entities/general.py
+-rw-rw-rw-   0        0        0     4802 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/entities/handlers.py
+-rw-rw-rw-   0        0        0     5127 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/entities/link_info.py
+-rw-rw-rw-   0        0        0     3831 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/entities/member.py
+-rw-rw-rw-   0        0        0    42520 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/entities/messages.py
+-rw-rw-rw-   0        0        0     1839 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/entities/notification.py
+-rw-rw-rw-   0        0        0    31711 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/entities/sticker.py
+-rw-rw-rw-   0        0        0     6185 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/entities/threads.py
+-rw-rw-rw-   0        0        0    31609 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/entities/userprofile.py
+-rw-rw-rw-   0        0        0     2451 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/entities/wsevents.py
+-rw-rw-rw-   0        0        0    70299 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/global_client.py
+-rw-rw-rw-   0        0        0      543 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/handle_queue.py
+-rw-rw-rw-   0        0        0     6657 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/socket.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:22:13.290218 pymino-1.2.3.2/pymino/ext/utilities/
+-rw-rw-rw-   0        0        0      234 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/utilities/__init__.py
+-rw-rw-rw-   0        0        0    11544 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/utilities/async_request_handler.py
+-rw-rw-rw-   0        0        0    11309 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/utilities/chat_console.py
+-rw-rw-rw-   0        0        0     6280 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/utilities/commands.py
+-rw-rw-rw-   0        0        0     2078 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/utilities/community_console.py
+-rw-rw-rw-   0        0        0     1110 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/utilities/generate.py
+-rw-rw-rw-   0        0        0     2911 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/utilities/menu.py
+-rw-rw-rw-   0        0        0     2106 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/utilities/profile_console.py
+-rw-rw-rw-   0        0        0    10404 2023-07-09 18:10:54.000000 pymino-1.2.3.2/pymino/ext/utilities/request_handler.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:22:13.231690 pymino-1.2.3.2/pymino.egg-info/
+-rw-rw-rw-   0        0        0     7373 2023-07-09 18:22:13.000000 pymino-1.2.3.2/pymino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1640 2023-07-09 18:22:13.000000 pymino-1.2.3.2/pymino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 18:22:13.000000 pymino-1.2.3.2/pymino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      117 2023-07-09 18:22:13.000000 pymino-1.2.3.2/pymino.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-09 18:22:13.000000 pymino-1.2.3.2/pymino.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      873 2023-07-09 18:22:13.298650 pymino-1.2.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1344 2023-07-09 18:19:59.000000 pymino-1.2.3.2/setup.py
```

### Comparing `pymino-1.2.3.1/LICENSE` & `pymino-1.2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/PKG-INFO` & `pymino-1.2.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.2.3.1
+Version: 1.2.3.2
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
   <h1 style="color: #0d47a1; font-size: 3em;">pymino</h1>
   
   <p>
```

#### html2text {}

```diff
@@ -1,17 +1,16 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.2.3.1 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.2.3.2 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
-:: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
-LICENSE
+:: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Topic :: Software Development ::
+Libraries :: Python Modules Requires-Python: >=3.8 Description-Content-Type:
+text/markdown License-File: LICENSE
                              ****** pymino ******
 [Discord] [Libraries.io_dependency_status_for_GitHub_repo] [GitHub_last_commit]
                               [PyPI_-_Downloads]
            A Python wrapper to communicate with the Amino Apps API.
     Easily create a bot for Amino Apps using a modern, easy-to-use library.
                                **** WARNING ****
  Pymino is a fully reverse-engineered client. By using this client, you may be
```

### Comparing `pymino-1.2.3.1/README.md` & `pymino-1.2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/__init__.py` & `pymino-1.2.3.2/pymino/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __title__ = 'pymino'
 __author__ = 'cynical'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Cynical'
-__version__ = '1.2.3.1'
+__version__ = '1.2.3.2'
 __description__ = 'A Python wrapper for the aminoapps.com API'
 
 from .bot import Bot as Bot
 from .async_bot import AsyncBot as AsyncBot
 from .client import Client as Client
 from .async_client import AsyncClient as AsyncClient
```

### Comparing `pymino-1.2.3.1/pymino/async_bot.py` & `pymino-1.2.3.2/pymino/async_bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/async_client.py` & `pymino-1.2.3.2/pymino/async_client.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/bot.py` & `pymino-1.2.3.2/pymino/bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/client.py` & `pymino-1.2.3.2/pymino/client.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/ext/__init__.py` & `pymino-1.2.3.2/pymino/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/ext/account.py` & `pymino-1.2.3.2/pymino/ext/account.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/ext/async_account.py` & `pymino-1.2.3.2/pymino/ext/async_account.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/ext/async_community.py` & `pymino-1.2.3.2/pymino/ext/async_community.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,16 +130,17 @@
         >>> client.community_id = 123456789
 
         >>> @community
         >>> def my_function(self, comId: str):
         >>>     # Function code
         """
         async def community_func(*args, **kwargs) -> Any:
+
             if not args[0].userId:
-                raise NotLoggedIn("You are not logged in. Please login before using this function.")
+                raise NotLoggedIn()
             if not any([args[0].community_id, kwargs.get("comId")]):
                 raise MissingCommunityId()
             return await func(*args, **kwargs)
 
         community_func.__annotations__ = func.__annotations__
         return community_func
```

### Comparing `pymino-1.2.3.1/pymino/ext/async_context.py` & `pymino-1.2.3.2/pymino/ext/async_context.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/ext/async_event_handler.py` & `pymino-1.2.3.2/pymino/ext/async_event_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/ext/async_global_client.py` & `pymino-1.2.3.2/pymino/ext/async_global_client.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/ext/async_socket.py` & `pymino-1.2.3.2/pymino/ext/async_socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/ext/community.py` & `pymino-1.2.3.2/pymino/ext/community.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,18 +134,19 @@
         >>> @community
         >>> def my_function(self, comId: str):
         >>>     # Function code
         """
         def community_func(*args, **kwargs) -> Any:
             
             if not args[0].userId:
-                raise NotLoggedIn("You are not logged in. Please login before using this function.")
+                raise NotLoggedIn()
             if not any([args[0].community_id, kwargs.get("comId")]):
                 raise MissingCommunityId()
             return func(*args, **kwargs)
+
         community_func.__annotations__ = func.__annotations__
         return community_func
 
 
     @community
     def invite_code(self, comId: Union[str, int] = None) -> CommunityInvitation:
         """
```

### Comparing `pymino-1.2.3.1/pymino/ext/console.py` & `pymino-1.2.3.2/pymino/ext/console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/ext/context.py` & `pymino-1.2.3.2/pymino/ext/context.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/ext/dispatcher.py` & `pymino-1.2.3.2/pymino/ext/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/ext/entities/acm.py` & `pymino-1.2.3.2/pymino/ext/entities/acm.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/ext/entities/admin_log.py` & `pymino-1.2.3.2/pymino/ext/entities/admin_log.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/ext/entities/api_response.py` & `pymino-1.2.3.2/pymino/ext/entities/api_response.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/ext/entities/bubble.py` & `pymino-1.2.3.2/pymino/ext/entities/bubble.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/ext/entities/chat_threads.py` & `pymino-1.2.3.2/pymino/ext/entities/chat_threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/ext/entities/comments.py` & `pymino-1.2.3.2/pymino/ext/entities/comments.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/ext/entities/enums.py` & `pymino-1.2.3.2/pymino/ext/entities/enums.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/ext/entities/exceptions.py` & `pymino-1.2.3.2/pymino/ext/entities/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/ext/entities/general.py` & `pymino-1.2.3.2/pymino/ext/entities/general.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/ext/entities/handlers.py` & `pymino-1.2.3.2/pymino/ext/entities/handlers.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/ext/entities/link_info.py` & `pymino-1.2.3.2/pymino/ext/entities/link_info.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/ext/entities/member.py` & `pymino-1.2.3.2/pymino/ext/entities/member.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/ext/entities/messages.py` & `pymino-1.2.3.2/pymino/ext/entities/messages.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/ext/entities/notification.py` & `pymino-1.2.3.2/pymino/ext/entities/notification.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/ext/entities/sticker.py` & `pymino-1.2.3.2/pymino/ext/entities/sticker.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/ext/entities/threads.py` & `pymino-1.2.3.2/pymino/ext/entities/threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/ext/entities/userprofile.py` & `pymino-1.2.3.2/pymino/ext/entities/userprofile.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/ext/entities/wsevents.py` & `pymino-1.2.3.2/pymino/ext/entities/wsevents.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/ext/global_client.py` & `pymino-1.2.3.2/pymino/ext/global_client.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/ext/handle_queue.py` & `pymino-1.2.3.2/pymino/ext/handle_queue.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/ext/socket.py` & `pymino-1.2.3.2/pymino/ext/socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/ext/utilities/async_request_handler.py` & `pymino-1.2.3.2/pymino/ext/utilities/async_request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/ext/utilities/chat_console.py` & `pymino-1.2.3.2/pymino/ext/utilities/chat_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/ext/utilities/commands.py` & `pymino-1.2.3.2/pymino/ext/utilities/commands.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/ext/utilities/community_console.py` & `pymino-1.2.3.2/pymino/ext/utilities/community_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/ext/utilities/generate.py` & `pymino-1.2.3.2/pymino/ext/utilities/generate.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/ext/utilities/menu.py` & `pymino-1.2.3.2/pymino/ext/utilities/menu.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/ext/utilities/profile_console.py` & `pymino-1.2.3.2/pymino/ext/utilities/profile_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino/ext/utilities/request_handler.py` & `pymino-1.2.3.2/pymino/ext/utilities/request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/pymino.egg-info/PKG-INFO` & `pymino-1.2.3.2/pymino.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.2.3.1
+Version: 1.2.3.2
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
   <h1 style="color: #0d47a1; font-size: 3em;">pymino</h1>
   
   <p>
```

#### html2text {}

```diff
@@ -1,17 +1,16 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.2.3.1 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.2.3.2 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
-:: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
-LICENSE
+:: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Topic :: Software Development ::
+Libraries :: Python Modules Requires-Python: >=3.8 Description-Content-Type:
+text/markdown License-File: LICENSE
                              ****** pymino ******
 [Discord] [Libraries.io_dependency_status_for_GitHub_repo] [GitHub_last_commit]
                               [PyPI_-_Downloads]
            A Python wrapper to communicate with the Amino Apps API.
     Easily create a bot for Amino Apps using a modern, easy-to-use library.
                                **** WARNING ****
  Pymino is a fully reverse-engineered client. By using this client, you may be
```

### Comparing `pymino-1.2.3.1/pymino.egg-info/SOURCES.txt` & `pymino-1.2.3.2/pymino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.1/setup.cfg` & `pymino-1.2.3.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796d 696e 6f0d 0a76 6572 7369   = pymino..versi
-00000020: 6f6e 203d 2031 2e32 2e33 2e31 0d0a 6175  on = 1.2.3.1..au
+00000020: 6f6e 203d 2031 2e32 2e33 2e32 0d0a 6175  on = 1.2.3.2..au
 00000030: 7468 6f72 203d 2066 6f72 6576 6572 6379  thor = forevercy
 00000040: 6e69 6361 6c0d 0a61 7574 686f 725f 656d  nical..author_em
 00000050: 6169 6c20 3d20 6d65 4063 796e 6963 616c  ail = me@cynical
 00000060: 2e67 670d 0a64 6573 6372 6970 7469 6f6e  .gg..description
 00000070: 203d 2045 6173 696c 7920 6372 6561 7465   = Easily create
 00000080: 2061 2062 6f74 2066 6f72 2041 6d69 6e6f   a bot for Amino
 00000090: 2041 7070 7320 7573 696e 6720 6120 6d6f   Apps using a mo
```

### Comparing `pymino-1.2.3.1/setup.py` & `pymino-1.2.3.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,14 +33,13 @@
         "narvii-bots",
         "aminoapps",
         "amino-bot",
         "amino-bots"
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
-    python_requires=">=3.7"
+    python_requires=">=3.8"
 )
```

