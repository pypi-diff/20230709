# Comparing `tmp/nonebot_adapter_kaiheila-0.2.6.tar.gz` & `tmp/nonebot_adapter_kaiheila-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_kaiheila-0.2.6.tar", max compression
+gzip compressed data, was "nonebot_adapter_kaiheila-0.2.7.tar", max compression
```

## Comparing `nonebot_adapter_kaiheila-0.2.6.tar` & `nonebot_adapter_kaiheila-0.2.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1065 2023-04-16 05:35:36.030823 nonebot_adapter_kaiheila-0.2.6/LICENSE
--rw-r--r--   0        0        0      296 2023-04-16 05:35:36.030823 nonebot_adapter_kaiheila-0.2.6/README.md
--rw-r--r--   0        0        0      359 2023-04-16 05:35:36.030823 nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/__init__.py
--rw-r--r--   0        0        0    15919 2023-04-16 05:35:36.030823 nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/adapter.py
--rw-r--r--   0        0        0       66 2023-04-16 05:35:36.030823 nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/api/__init__.py
--rw-r--r--   0        0        0       27 2023-04-16 05:35:36.030823 nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/api/client.py
--rw-r--r--   0        0        0    13445 2023-04-16 05:35:36.030823 nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/api/client.pyi
--rw-r--r--   0        0        0     4153 2023-04-16 05:35:36.030823 nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/api/handle.py
--rw-r--r--   0        0        0    12976 2023-04-16 05:35:36.030823 nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/api/model.py
--rw-r--r--   0        0        0    12338 2023-04-16 05:35:36.030823 nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/bot.py
--rw-r--r--   0        0        0      833 2023-04-16 05:35:36.030823 nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/config.py
--rw-r--r--   0        0        0    28176 2023-04-16 05:35:36.030823 nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/event.py
--rw-r--r--   0        0        0     3504 2023-04-16 05:35:36.030823 nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/exception.py
--rw-r--r--   0        0        0    12822 2023-04-16 05:35:36.030823 nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/message.py
--rw-r--r--   0        0        0      494 2023-04-16 05:35:36.030823 nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/permission.py
--rw-r--r--   0        0        0     2437 2023-04-16 05:35:36.030823 nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/utils.py
--rw-r--r--   0        0        0      749 2023-04-16 05:35:36.034823 nonebot_adapter_kaiheila-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     1090 1970-01-01 00:00:00.000000 nonebot_adapter_kaiheila-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-09 15:52:52.653429 nonebot_adapter_kaiheila-0.2.7/LICENSE
+-rw-r--r--   0        0        0      296 2023-07-09 15:52:52.653429 nonebot_adapter_kaiheila-0.2.7/README.md
+-rw-r--r--   0        0        0      359 2023-07-09 15:52:52.653429 nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/__init__.py
+-rw-r--r--   0        0        0    15919 2023-07-09 15:52:52.653429 nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/adapter.py
+-rw-r--r--   0        0        0       66 2023-07-09 15:52:52.653429 nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/api/__init__.py
+-rw-r--r--   0        0        0       27 2023-07-09 15:52:52.653429 nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/api/client.py
+-rw-r--r--   0        0        0    13589 2023-07-09 15:52:52.653429 nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/api/client.pyi
+-rw-r--r--   0        0        0     4223 2023-07-09 15:52:52.653429 nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/api/handle.py
+-rw-r--r--   0        0        0    12976 2023-07-09 15:52:52.653429 nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/api/model.py
+-rw-r--r--   0        0        0    12338 2023-07-09 15:52:52.653429 nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/bot.py
+-rw-r--r--   0        0        0      833 2023-07-09 15:52:52.653429 nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/config.py
+-rw-r--r--   0        0        0    28176 2023-07-09 15:52:52.653429 nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/event.py
+-rw-r--r--   0        0        0     3504 2023-07-09 15:52:52.653429 nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/exception.py
+-rw-r--r--   0        0        0    12822 2023-07-09 15:52:52.653429 nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/message.py
+-rw-r--r--   0        0        0      494 2023-07-09 15:52:52.653429 nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/permission.py
+-rw-r--r--   0        0        0     2437 2023-07-09 15:52:52.653429 nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/utils.py
+-rw-r--r--   0        0        0      749 2023-07-09 15:52:52.653429 nonebot_adapter_kaiheila-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     1090 1970-01-01 00:00:00.000000 nonebot_adapter_kaiheila-0.2.7/PKG-INFO
```

### Comparing `nonebot_adapter_kaiheila-0.2.6/LICENSE` & `nonebot_adapter_kaiheila-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/adapter.py` & `nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/adapter.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/api/client.pyi` & `nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/api/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -191,14 +191,21 @@
             msg_id (str, optional):
                 消息内容
             quote (str, optional):
                 回复某条消息的msgId. 如果为空,则代表删除回复,不传则无影响.
         """
         ...
 
+    async def directMessage_view(
+            self, *,
+            chat_code: str,
+            msg_id: str
+    ) -> DirectMessage:
+        ...
+
     async def gateway_index(self, *, compress: Optional[int] = ...) -> URL:
         ...
 
     async def guildEmoji_create(
             self, *,
             guild_id: str,
             emoji: Optional[bytes] = ...,
```

### Comparing `nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/api/handle.py` & `nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/api/handle.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     'direct-message/add-reaction': {'method': 'POST', 'type': None},
     'direct-message/create': {'method': 'POST', 'type': MessageCreateReturn},
     'direct-message/delete': {'method': 'POST', 'type': None},
     'direct-message/delete-reaction': {'method': 'POST', 'type': None},
     'direct-message/list': {'method': 'GET', 'type': DirectMessagesReturn},
     'direct-message/reaction-list': {'method': 'GET', 'type': List[ReactionUser]},
     'direct-message/update': {'method': 'POST', 'type': None},
+    'direct-message/view': {'method': 'GET', 'type': DirectMessage},
     'gateway/index': {'method': 'GET', 'type': URL},
     'guild-emoji/create': {'method': 'POST', 'type': None},
     'guild-emoji/delete': {'method': 'POST', 'type': None},
     'guild-emoji/list': {'method': 'GET', 'type': GuildEmojisReturn},
     'guild-emoji/update': {'method': 'POST', 'type': None},
     'guild-mute/create': {'method': 'POST', 'type': None},
     'guild-mute/delete': {'method': 'POST', 'type': None},
```

### Comparing `nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/api/model.py` & `nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/api/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/bot.py` & `nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/config.py` & `nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/event.py` & `nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/event.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/exception.py` & `nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/message.py` & `nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/utils.py` & `nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kaiheila-0.2.6/pyproject.toml` & `nonebot_adapter_kaiheila-0.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-adapter-kaiheila"
-version = "0.2.6"
+version = "0.2.7"
 description = "kaiheila adapter for nonebot2"
 authors = ["Tian-que <1605206150@qq.com>", "ssttkkl <huang.wen.long@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Tian-que/nonebot-adapter-kaiheila"
 keywords = ["bot", "khl", "kaiheila", "khlbot"]
```

### Comparing `nonebot_adapter_kaiheila-0.2.6/PKG-INFO` & `nonebot_adapter_kaiheila-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-kaiheila
-Version: 0.2.6
+Version: 0.2.7
 Summary: kaiheila adapter for nonebot2
 Home-page: https://github.com/Tian-que/nonebot-adapter-kaiheila
 License: MIT
 Keywords: bot,khl,kaiheila,khlbot
 Author: Tian-que
 Author-email: 1605206150@qq.com
 Requires-Python: >=3.9,<4.0
```

