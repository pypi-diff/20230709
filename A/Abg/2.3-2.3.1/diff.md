# Comparing `tmp/Abg-2.3.tar.gz` & `tmp/Abg-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Abg-2.3.tar", last modified: Thu Jul  6 12:18:43 2023, max compression
+gzip compressed data, was "Abg-2.3.1.tar", last modified: Sun Jul  9 05:18:22 2023, max compression
```

## Comparing `Abg-2.3.tar` & `Abg-2.3.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:18:43.599187 Abg-2.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:18:43.591187 Abg-2.3/Abg/
--rw-r--r--   0 root         (0) root         (0)      308 2023-07-06 12:18:28.000000 Abg-2.3/Abg/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:18:43.595187 Abg-2.3/Abg/chat_status/
--rw-r--r--   0 root         (0) root         (0)      109 2023-07-06 12:18:28.000000 Abg-2.3/Abg/chat_status/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5154 2023-07-06 12:18:28.000000 Abg-2.3/Abg/chat_status/chat_status.py
--rw-r--r--   0 root         (0) root         (0)     2348 2023-07-06 12:18:28.000000 Abg-2.3/Abg/chat_status/custom_filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:18:43.595187 Abg-2.3/Abg/helpers/
--rw-r--r--   0 root         (0) root         (0)      855 2023-07-06 12:18:28.000000 Abg-2.3/Abg/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3710 2023-07-06 12:18:28.000000 Abg-2.3/Abg/helpers/get_user.py
--rw-r--r--   0 root         (0) root         (0)     3184 2023-07-06 12:18:28.000000 Abg-2.3/Abg/helpers/helpers.py
--rw-r--r--   0 root         (0) root         (0)     1596 2023-07-06 12:18:28.000000 Abg-2.3/Abg/helpers/http_helper.py
--rw-r--r--   0 root         (0) root         (0)     2589 2023-07-06 12:18:28.000000 Abg-2.3/Abg/helpers/human_read.py
--rw-r--r--   0 root         (0) root         (0)     7351 2023-07-06 12:18:28.000000 Abg-2.3/Abg/helpers/msg_types.py
--rw-r--r--   0 root         (0) root         (0)     1279 2023-07-06 12:18:28.000000 Abg-2.3/Abg/helpers/parser.py
--rw-r--r--   0 root         (0) root         (0)     2533 2023-07-06 12:18:28.000000 Abg-2.3/Abg/helpers/pyro_progress.py
--rw-r--r--   0 root         (0) root         (0)     2834 2023-07-06 12:18:28.000000 Abg-2.3/Abg/helpers/ratelimit.py
--rw-r--r--   0 root         (0) root         (0)     5335 2023-07-06 12:18:28.000000 Abg-2.3/Abg/helpers/string.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:18:43.595187 Abg-2.3/Abg/inline/
--rw-r--r--   0 root         (0) root         (0)      274 2023-07-06 12:18:28.000000 Abg-2.3/Abg/inline/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6105 2023-07-06 12:18:28.000000 Abg-2.3/Abg/inline/inline_keyboard.py
--rw-r--r--   0 root         (0) root         (0)     4267 2023-07-06 12:18:28.000000 Abg-2.3/Abg/inline/inline_pagination_keyboard.py
--rw-r--r--   0 root         (0) root         (0)     1487 2023-07-06 12:18:28.000000 Abg-2.3/Abg/inline/reply_keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:18:43.599187 Abg-2.3/Abg/patch/
--rw-r--r--   0 root         (0) root         (0)      107 2023-07-06 12:18:28.000000 Abg-2.3/Abg/patch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:18:43.599187 Abg-2.3/Abg/patch/bound/
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-06 12:18:28.000000 Abg-2.3/Abg/patch/bound/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11979 2023-07-06 12:18:28.000000 Abg-2.3/Abg/patch/bound/message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:18:43.599187 Abg-2.3/Abg/patch/decorators/
--rw-r--r--   0 root         (0) root         (0)       95 2023-07-06 12:18:28.000000 Abg-2.3/Abg/patch/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3119 2023-07-06 12:18:28.000000 Abg-2.3/Abg/patch/decorators/callback.py
--rw-r--r--   0 root         (0) root         (0)     5406 2023-07-06 12:18:28.000000 Abg-2.3/Abg/patch/decorators/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:18:43.599187 Abg-2.3/Abg/patch/listen/
--rw-r--r--   0 root         (0) root         (0)       55 2023-07-06 12:18:28.000000 Abg-2.3/Abg/patch/listen/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12016 2023-07-06 12:18:28.000000 Abg-2.3/Abg/patch/listen/listen.py
--rw-r--r--   0 root         (0) root         (0)      776 2023-07-06 12:18:28.000000 Abg-2.3/Abg/patch/listen/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:18:43.599187 Abg-2.3/Abg/patch/methods/
--rw-r--r--   0 root         (0) root         (0)      127 2023-07-06 12:18:28.000000 Abg-2.3/Abg/patch/methods/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2172 2023-07-06 12:18:28.000000 Abg-2.3/Abg/patch/methods/edit_message_text.py
--rw-r--r--   0 root         (0) root         (0)     1713 2023-07-06 12:18:28.000000 Abg-2.3/Abg/patch/methods/send_as_file.py
--rw-r--r--   0 root         (0) root         (0)     2933 2023-07-06 12:18:28.000000 Abg-2.3/Abg/patch/methods/send_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:18:43.591187 Abg-2.3/Abg.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4842 2023-07-06 12:18:43.000000 Abg-2.3/Abg.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      999 2023-07-06 12:18:43.000000 Abg-2.3/Abg.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 12:18:43.000000 Abg-2.3/Abg.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-07-06 12:18:43.000000 Abg-2.3/Abg.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     4842 2023-07-06 12:18:43.599187 Abg-2.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2336 2023-07-06 12:18:28.000000 Abg-2.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 12:18:43.599187 Abg-2.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3004 2023-07-06 12:18:28.000000 Abg-2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 05:18:22.815145 Abg-2.3.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 05:18:22.807145 Abg-2.3.1/Abg/
+-rw-r--r--   0 root         (0) root         (0)      338 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 05:18:22.811145 Abg-2.3.1/Abg/chat_status/
+-rw-r--r--   0 root         (0) root         (0)      109 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/chat_status/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5154 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/chat_status/chat_status.py
+-rw-r--r--   0 root         (0) root         (0)     2348 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/chat_status/custom_filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 05:18:22.811145 Abg-2.3.1/Abg/helpers/
+-rw-r--r--   0 root         (0) root         (0)      855 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3710 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/helpers/get_user.py
+-rw-r--r--   0 root         (0) root         (0)     3184 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/helpers/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     1596 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/helpers/http_helper.py
+-rw-r--r--   0 root         (0) root         (0)     2589 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/helpers/human_read.py
+-rw-r--r--   0 root         (0) root         (0)     7351 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/helpers/msg_types.py
+-rw-r--r--   0 root         (0) root         (0)     1279 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/helpers/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2533 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/helpers/pyro_progress.py
+-rw-r--r--   0 root         (0) root         (0)     2834 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/helpers/ratelimit.py
+-rw-r--r--   0 root         (0) root         (0)     5335 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/helpers/string.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 05:18:22.811145 Abg-2.3.1/Abg/inline/
+-rw-r--r--   0 root         (0) root         (0)      274 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/inline/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6105 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/inline/inline_keyboard.py
+-rw-r--r--   0 root         (0) root         (0)     4267 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/inline/inline_pagination_keyboard.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/inline/reply_keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 05:18:22.811145 Abg-2.3.1/Abg/patch/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/patch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 05:18:22.811145 Abg-2.3.1/Abg/patch/bound/
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/patch/bound/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11979 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/patch/bound/message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 05:18:22.815145 Abg-2.3.1/Abg/patch/decorators/
+-rw-r--r--   0 root         (0) root         (0)       95 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/patch/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3894 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/patch/decorators/callback.py
+-rw-r--r--   0 root         (0) root         (0)     5483 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/patch/decorators/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 05:18:22.815145 Abg-2.3.1/Abg/patch/listen/
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/patch/listen/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12016 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/patch/listen/listen.py
+-rw-r--r--   0 root         (0) root         (0)      776 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/patch/listen/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 05:18:22.815145 Abg-2.3.1/Abg/patch/methods/
+-rw-r--r--   0 root         (0) root         (0)      127 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/patch/methods/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2172 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/patch/methods/edit_message_text.py
+-rw-r--r--   0 root         (0) root         (0)     1713 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/patch/methods/send_as_file.py
+-rw-r--r--   0 root         (0) root         (0)     2933 2023-07-09 05:18:01.000000 Abg-2.3.1/Abg/patch/methods/send_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 05:18:22.807145 Abg-2.3.1/Abg.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5050 2023-07-09 05:18:22.000000 Abg-2.3.1/Abg.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      999 2023-07-09 05:18:22.000000 Abg-2.3.1/Abg.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 05:18:22.000000 Abg-2.3.1/Abg.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-09 05:18:22.000000 Abg-2.3.1/Abg.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5050 2023-07-09 05:18:22.815145 Abg-2.3.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2486 2023-07-09 05:18:01.000000 Abg-2.3.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-09 05:18:22.815145 Abg-2.3.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3006 2023-07-09 05:18:01.000000 Abg-2.3.1/setup.py
```

### Comparing `Abg-2.3/Abg/chat_status/chat_status.py` & `Abg-2.3.1/Abg/chat_status/chat_status.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3/Abg/chat_status/custom_filters.py` & `Abg-2.3.1/Abg/chat_status/custom_filters.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3/Abg/helpers/__init__.py` & `Abg-2.3.1/Abg/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3/Abg/helpers/get_user.py` & `Abg-2.3.1/Abg/helpers/get_user.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3/Abg/helpers/helpers.py` & `Abg-2.3.1/Abg/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3/Abg/helpers/http_helper.py` & `Abg-2.3.1/Abg/helpers/http_helper.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3/Abg/helpers/human_read.py` & `Abg-2.3.1/Abg/helpers/human_read.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3/Abg/helpers/msg_types.py` & `Abg-2.3.1/Abg/helpers/msg_types.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3/Abg/helpers/parser.py` & `Abg-2.3.1/Abg/helpers/parser.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3/Abg/helpers/pyro_progress.py` & `Abg-2.3.1/Abg/helpers/pyro_progress.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3/Abg/helpers/ratelimit.py` & `Abg-2.3.1/Abg/helpers/ratelimit.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3/Abg/helpers/string.py` & `Abg-2.3.1/Abg/helpers/string.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3/Abg/inline/inline_keyboard.py` & `Abg-2.3.1/Abg/inline/inline_keyboard.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3/Abg/inline/inline_pagination_keyboard.py` & `Abg-2.3.1/Abg/inline/inline_pagination_keyboard.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3/Abg/inline/reply_keyboard.py` & `Abg-2.3.1/Abg/inline/reply_keyboard.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3/Abg/patch/bound/message.py` & `Abg-2.3.1/Abg/patch/bound/message.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3/Abg/patch/decorators/callback.py` & `Abg-2.3.1/Abg/patch/decorators/callback.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,34 @@
+import asyncio
 import typing
 from logging import getLogger
 
 import pyrogram
+from pyrogram.errors import (
+    ChatAdminRequired,
+    FloodWait,
+    Forbidden,
+    MessageNotModified,
+    SlowmodeWait,
+)
 from pyrogram.methods import Decorators
 
 LOGGER = getLogger(__name__)
 
 
 def callback(
     self,
     data: typing.Union[str, list],
     self_admin: typing.Union[bool, bool] = False,
     filter: typing.Union[pyrogram.filters.Filter, pyrogram.filters.Filter] = None,
     *args,
     **kwargs,
 ):
     """
-    ### `Client.callback`
+    ### `Client.on_cb("etc")`
 
     - A decorater to Register Callback Quiries in simple way and manage errors in that Function itself, alternative for `@pyrogram.Client.on_callback_query(pyrogram.filters.regex('^data.*'))`
     - Parameters:
     - data (str || list):
         - The callback query to be handled for a function
 
     - self_admin (bool) **optional**:
@@ -43,15 +51,15 @@
                 pyrogram.types.InlineKeyboardButton(
                 "Click Here",
                 "data"
                 )
             ]])
             )
 
-        @app.callback("data")
+        @app.on_cb("data")
         async def data(client, CallbackQuery):
         await CallbackQuery.answer("Hello :)", show_alert=True)
     """
     if filter:
         filter = pyrogram.filters.regex(f"^{data}.*") & args["filter"]
     else:
         filter = pyrogram.filters.regex(f"^{data}.*")
@@ -67,21 +75,35 @@
                     pyrogram.enums.ChatMemberStatus.ADMINISTRATOR,
                 ):
                     return await CallbackQuery.message.edit_text(
                         "ɪ ᴍᴜsᴛ ʙᴇ ᴀᴅᴍɪɴ ᴛᴏ ᴇxᴇᴄᴜᴛᴇ ᴛʜɪs ᴄᴏᴍᴍᴀɴᴅ"
                     )
             try:
                 await func(client, CallbackQuery)
-            except pyrogram.errors.exceptions.forbidden_403.ChatAdminRequired:
-                pass
+            except FloodWait as fw:
+                LOGGER.warning(str(fw))
+                await asyncio.sleep(fw.value)
+            except MessageNotModified:
+                LOGGER.info(
+                    "The message was not modified because you tried to edit it using the same content "
+                )
+                return await CallbackQuery.answer(
+                    "The message was not modified because you tried to edit it using the same content ",
+                    show_alert=True,
+                )
+            except (Forbidden, SlowmodeWait, ChatAdminRequired):
+                LOGGER.info(
+                    f"You cannot write in this chat: {CallbackQuery.message.chat.title} [{CallbackQuery.message.chat.id}]"
+                )
+                return await CallbackQuery.answer(
+                    "Bot need to message write permission "
+                )
             except BaseException as e:
                 LOGGER.error(f"Error Found in callback Handler : {e}")
-                return await CallbackQuery.message.edit_text(
-                    f"ᴀɴ ɪɴᴛᴇʀɴᴀʟ ᴇʀʀᴏʀ ᴏᴄᴄᴜʀʀᴇᴅ ᴡʜɪʟᴇ ᴘʀᴏᴄᴇssɪɴɢ ʏᴏᴜʀ ᴄᴏᴍᴍᴀɴᴅ\nᴇʀʀᴏʀ {e}\n"
-                )
+                return await CallbackQuery.message.edit_text(f"ᴇʀʀᴏʀ ғᴏᴜɴᴅ:\n{e}")
 
         self.add_handler(pyrogram.handlers.CallbackQueryHandler(decorator, filter))
         return decorator
 
     return wrapper
```

### Comparing `Abg-2.3/Abg/patch/decorators/command.py` & `Abg-2.3.1/Abg/patch/decorators/command.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import asyncio
 import typing
 from logging import getLogger
 
 import pyrogram
+from pyrogram.errors import ChatAdminRequired, FloodWait, Forbidden, SlowmodeWait
 from pyrogram.methods import Decorators
 
 HANDLER = ["/", "!", "~", ".", "+", "*"]
 
 LOGGER = getLogger(__name__)
 
 
@@ -20,15 +22,15 @@
     no_channel: typing.Union[bool, bool] = False,
     handler: typing.Optional[list] = None,
     filter: typing.Union[pyrogram.filters.Filter, pyrogram.filters.Filter] = None,
     *args,
     **kwargs,
 ):
     """
-    ### `tgClient.command`
+    ### `@Client.on_cmd`
     - A decorater to Register Commands in simple way and manage errors in that Function itself, alternative for `@pyrogram.Client.on_message(pyrogram.filters.command('command'))`
     - Parameters:
     - command (str || list):
         - The command to be handled for a function
 
     - group_only (bool) **optional**:
         - If True, the command will only executed in Groups only, By Default False.
@@ -107,24 +109,25 @@
                 return await message.reply_text(
                     "ᴛʜɪs ᴄᴏᴍᴍᴀɴᴅ ᴄᴀɴ ʙᴇ ᴜsᴇᴅ ɪɴ sᴜᴘᴇʀɢʀᴏᴜᴘs ᴏɴʟʏ."
                 )
             if pm_only and message.chat.type != pyrogram.enums.ChatType.PRIVATE:
                 return await message.reply_text("ᴛʜɪs ᴄᴏᴍᴍᴀɴᴅ ᴄᴀɴ ʙᴇ ᴜsᴇᴅ ɪɴ ᴘᴍs ᴏɴʟʏ.")
             try:
                 await func(client, message)
-            except pyrogram.errors.exceptions.forbidden_403.ChatWriteForbidden:
-                await client.leave_chat(message.chat.id)
+            except FloodWait as fw:
+                LOGGER.warning(str(fw))
+                await asyncio.sleep(fw.value)
+            except (Forbidden, SlowmodeWait, ChatAdminRequired):
                 LOGGER.info(
-                    f"Leaving chat : {message.chat.id}, because doesn't have admin permission."
+                    f"Leaving chat : {message.chat.title} [{message.chat.id}], because doesn't have admin permission."
                 )
+                return await client.leave_chat(message.chat.id)
             except BaseException as e:
                 LOGGER.error(f"Error found in command handler: {e}")
-                return await message.reply_text(
-                    f"ᴀɴ ɪɴᴛᴇʀɴᴀʟ ᴇʀʀᴏʀ ᴏᴄᴄᴜʀʀᴇᴅ ᴡʜɪʟᴇ ᴘʀᴏᴄᴇssɪɴɢ ʏᴏᴜʀ ᴄᴏᴍᴍᴀɴᴅ\nᴇʀʀᴏʀ {e}\n"
-                )
+                return await message.reply_text(f"ᴇʀʀᴏʀ ғᴏᴜɴᴅ:\n{e}")
 
         self.add_handler(
             pyrogram.handlers.MessageHandler(callback=decorator, filters=filter)
         )
         return decorator
 
     return wrapper
```

### Comparing `Abg-2.3/Abg/patch/listen/listen.py` & `Abg-2.3.1/Abg/patch/listen/listen.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3/Abg/patch/listen/utils.py` & `Abg-2.3.1/Abg/patch/listen/utils.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3/Abg/patch/methods/edit_message_text.py` & `Abg-2.3.1/Abg/patch/methods/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3/Abg/patch/methods/send_as_file.py` & `Abg-2.3.1/Abg/patch/methods/send_as_file.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3/Abg/patch/methods/send_message.py` & `Abg-2.3.1/Abg/patch/methods/send_message.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3/Abg.egg-info/PKG-INFO` & `Abg-2.3.1/Abg.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,58 +1,65 @@
 Metadata-Version: 2.1
 Name: Abg
-Version: 2.3
+Version: 2.3.1
 Summary: Telegram bot helpers
 Home-page: https://github.com/Abishnoi69/Abg
 Author: Abishnoi
 Author-email: Abishnoi69@Abg.org
 License: MIT
 Download-URL: https://github.com/Abishnoi69/Abg/releases/latest
 Project-URL: Tracker, https://github.com/Abishnoi69/Abg/issues
 Project-URL: Community, https://t.me/Abgpy
 Project-URL: Source, https://github.com/Abishnoi69/Abg
 Project-URL: Documentation, https://github.com/Abishnoi69/Abg/tree/master/doce
 Description: # ᴀʙɢ :->
         > 
-        ### • Conversation
+        ### • Abg
         
         ```python
         from pyrogram import filters, Client
-        from pyrogram.types import Message
+        from pyrogram.types import CallbackQuery, Message
         from Abg import patch  # type : ignore
+        from Abg.helpers import ikb
         
         app = Client("my_account")
         
         @app.on_cmd("myinfo")
         async def my_info(self: Client, ctx: Message):
             if not ctx.from_user:
                 return
             name = await ctx.chat.ask("Type Your Name")
             age = await ctx.chat.ask("Type your age")
             add = await ctx.chat.ask("Type your address")
             # you can also use : ctx.reply_text(...)
             await self.send_msg(
                 chat_id=ctx.chat.id,
                 text=f"Your name is: {name.text}\nYour age is: {age.text}\nyour address is: {add.text}",
+                reply_markup=ikb([[("ʙᴜᴛᴛᴏɴ", "hello")]]),
             )
         
+        # callback 
+        @app.on_cb("hello")
+        async def hello(c: Client, q: CallbackQuery):
+            await q.answer("Hello From Abg", show_alert=True)
+        
           app.run()
         ```
         >
         ### • User Rights 
         
         ```python
         from Abg import patch  # type : ignore
         from Abg.chat_status import adminsOnly
         from pyrogram.types import Message
         from pyrogram import Client
         
         app = Client("my_account")
         
-        @app.on_cmd("del"], group_only=True)
+        @app.on_cmd("del", group_only=True)
         @adminsOnly("can_delete_messages")
         async def del_msg(c: Client, m: Message):
             if m.reply_to_message:
                 await m.delete()
                 await c.delete_messages(
                     chat_id=m.chat.id,
                     message_ids=m.reply_to_message.id,
@@ -88,22 +95,22 @@
         
         <p><img src="https://raw.githubusercontent.com/Abishnoi69/Abg/master/doce/images/add_inline_button.png" alt="add_inline_button"></p>
         
         
         ### ɪɴsᴛᴀʟʟɪɴɢ :->
         
         ```bash
-        pip3 install Abg
+        pip install -U Abg
         ```
         
         ━━━━━━━━━━━━━━━━━━━━
         ## ɴᴏᴛᴇ :->
         
-        - This library is made for my personal Project so don't take it deeply  
-        - My Project [@AbgRobot](https://t.me/AbgRobot) / [@Exon_Robot](https://t.me/Exon_Robot) & [@ExonMusicBot](https://t.me/ExonMusicBot)
+        - This library is made for my personal Project so don't take it deeply .
+        - My Project [@GuardxRobot](https://t.me/GuardxRobot) 
         
         - ᴇɴᴊᴏʏ ʙᴀʙʏ ♡ 
         
         ━━━━━━━━━━━━━━━━━━━━ 
         
         
 Keywords: telegram bot chat messenger mtproto api client library python conversation keyboard userbot patch botapi https
```

### Comparing `Abg-2.3/Abg.egg-info/SOURCES.txt` & `Abg-2.3.1/Abg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Abg-2.3/PKG-INFO` & `Abg-2.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,58 +1,65 @@
 Metadata-Version: 2.1
 Name: Abg
-Version: 2.3
+Version: 2.3.1
 Summary: Telegram bot helpers
 Home-page: https://github.com/Abishnoi69/Abg
 Author: Abishnoi
 Author-email: Abishnoi69@Abg.org
 License: MIT
 Download-URL: https://github.com/Abishnoi69/Abg/releases/latest
 Project-URL: Tracker, https://github.com/Abishnoi69/Abg/issues
 Project-URL: Community, https://t.me/Abgpy
 Project-URL: Source, https://github.com/Abishnoi69/Abg
 Project-URL: Documentation, https://github.com/Abishnoi69/Abg/tree/master/doce
 Description: # ᴀʙɢ :->
         > 
-        ### • Conversation
+        ### • Abg
         
         ```python
         from pyrogram import filters, Client
-        from pyrogram.types import Message
+        from pyrogram.types import CallbackQuery, Message
         from Abg import patch  # type : ignore
+        from Abg.helpers import ikb
         
         app = Client("my_account")
         
         @app.on_cmd("myinfo")
         async def my_info(self: Client, ctx: Message):
             if not ctx.from_user:
                 return
             name = await ctx.chat.ask("Type Your Name")
             age = await ctx.chat.ask("Type your age")
             add = await ctx.chat.ask("Type your address")
             # you can also use : ctx.reply_text(...)
             await self.send_msg(
                 chat_id=ctx.chat.id,
                 text=f"Your name is: {name.text}\nYour age is: {age.text}\nyour address is: {add.text}",
+                reply_markup=ikb([[("ʙᴜᴛᴛᴏɴ", "hello")]]),
             )
         
+        # callback 
+        @app.on_cb("hello")
+        async def hello(c: Client, q: CallbackQuery):
+            await q.answer("Hello From Abg", show_alert=True)
+        
           app.run()
         ```
         >
         ### • User Rights 
         
         ```python
         from Abg import patch  # type : ignore
         from Abg.chat_status import adminsOnly
         from pyrogram.types import Message
         from pyrogram import Client
         
         app = Client("my_account")
         
-        @app.on_cmd("del"], group_only=True)
+        @app.on_cmd("del", group_only=True)
         @adminsOnly("can_delete_messages")
         async def del_msg(c: Client, m: Message):
             if m.reply_to_message:
                 await m.delete()
                 await c.delete_messages(
                     chat_id=m.chat.id,
                     message_ids=m.reply_to_message.id,
@@ -88,22 +95,22 @@
         
         <p><img src="https://raw.githubusercontent.com/Abishnoi69/Abg/master/doce/images/add_inline_button.png" alt="add_inline_button"></p>
         
         
         ### ɪɴsᴛᴀʟʟɪɴɢ :->
         
         ```bash
-        pip3 install Abg
+        pip install -U Abg
         ```
         
         ━━━━━━━━━━━━━━━━━━━━
         ## ɴᴏᴛᴇ :->
         
-        - This library is made for my personal Project so don't take it deeply  
-        - My Project [@AbgRobot](https://t.me/AbgRobot) / [@Exon_Robot](https://t.me/Exon_Robot) & [@ExonMusicBot](https://t.me/ExonMusicBot)
+        - This library is made for my personal Project so don't take it deeply .
+        - My Project [@GuardxRobot](https://t.me/GuardxRobot) 
         
         - ᴇɴᴊᴏʏ ʙᴀʙʏ ♡ 
         
         ━━━━━━━━━━━━━━━━━━━━ 
         
         
 Keywords: telegram bot chat messenger mtproto api client library python conversation keyboard userbot patch botapi https
```

### Comparing `Abg-2.3/README.md` & `Abg-2.3.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,52 @@
 # ᴀʙɢ :->
 > 
-### • Conversation
+### • Abg
 
 ```python
 from pyrogram import filters, Client
-from pyrogram.types import Message
+from pyrogram.types import CallbackQuery, Message
 from Abg import patch  # type : ignore
+from Abg.helpers import ikb
 
 app = Client("my_account")
 
 @app.on_cmd("myinfo")
 async def my_info(self: Client, ctx: Message):
     if not ctx.from_user:
         return
     name = await ctx.chat.ask("Type Your Name")
     age = await ctx.chat.ask("Type your age")
     add = await ctx.chat.ask("Type your address")
     # you can also use : ctx.reply_text(...)
     await self.send_msg(
         chat_id=ctx.chat.id,
         text=f"Your name is: {name.text}\nYour age is: {age.text}\nyour address is: {add.text}",
+        reply_markup=ikb([[("ʙᴜᴛᴛᴏɴ", "hello")]]),
     )
 
+# callback 
+@app.on_cb("hello")
+async def hello(c: Client, q: CallbackQuery):
+    await q.answer("Hello From Abg", show_alert=True)
+
   app.run()
 ```
 >
 ### • User Rights 
 
 ```python
 from Abg import patch  # type : ignore
 from Abg.chat_status import adminsOnly
 from pyrogram.types import Message
 from pyrogram import Client
 
 app = Client("my_account")
 
-@app.on_cmd("del"], group_only=True)
+@app.on_cmd("del", group_only=True)
 @adminsOnly("can_delete_messages")
 async def del_msg(c: Client, m: Message):
     if m.reply_to_message:
         await m.delete()
         await c.delete_messages(
             chat_id=m.chat.id,
             message_ids=m.reply_to_message.id,
@@ -75,20 +82,20 @@
 
 <p><img src="https://raw.githubusercontent.com/Abishnoi69/Abg/master/doce/images/add_inline_button.png" alt="add_inline_button"></p>
 
 
 ### ɪɴsᴛᴀʟʟɪɴɢ :->
 
 ```bash
-pip3 install Abg
+pip install -U Abg
 ```
 
 ━━━━━━━━━━━━━━━━━━━━
 ## ɴᴏᴛᴇ :->
 
-- This library is made for my personal Project so don't take it deeply  
-- My Project [@AbgRobot](https://t.me/AbgRobot) / [@Exon_Robot](https://t.me/Exon_Robot) & [@ExonMusicBot](https://t.me/ExonMusicBot)
+- This library is made for my personal Project so don't take it deeply .
+- My Project [@GuardxRobot](https://t.me/GuardxRobot) 
 
 - ᴇɴᴊᴏʏ ʙᴀʙʏ ♡ 
 
 ━━━━━━━━━━━━━━━━━━━━
```

### Comparing `Abg-2.3/setup.py` & `Abg-2.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     with open(file, encoding="utf-8") as r:
         return [i.strip() for i in r]
 """
 
 setuptools.setup(
     name="Abg",
     packages=setuptools.find_packages(),
-    version="2.3",
+    version="2.3.1",
     description="Telegram bot helpers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Abishnoi69/Abg",
     download_url="https://github.com/Abishnoi69/Abg/releases/latest",
     author="Abishnoi",
     author_email="Abishnoi69@Abg.org",
```

