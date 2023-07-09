# Comparing `tmp/channel_box-0.5.1.5-py3-none-any.whl.zip` & `tmp/channel_box-0.5.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 7342 bytes, number of entries: 10
+Zip file size: 7369 bytes, number of entries: 10
 -rw-rw-r--  2.0 unx       48 b- defN 23-Jun-07 06:56 channel_box/__init__.py
--rw-rw-r--  2.0 unx     5724 b- defN 23-Jun-07 09:06 channel_box/src.py
+-rw-rw-r--  2.0 unx     5765 b- defN 23-Jul-09 19:09 channel_box/src.py
 -rw-rw-r--  2.0 unx        0 b- defN 20-Jul-19 15:17 example/channel/__init__.py
 -rw-rw-r--  2.0 unx      599 b- defN 23-Jun-07 07:55 example/channel/urls.py
 -rw-rw-r--  2.0 unx     6393 b- defN 23-Jun-07 08:13 example/channel/views.py
--rwxr-xr-x  2.0 unx     1094 b- defN 23-Jun-07 09:09 channel_box-0.5.1.5.dist-info/LICENSE
--rw-rw-r--  2.0 unx     3045 b- defN 23-Jun-07 09:09 channel_box-0.5.1.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-07 09:09 channel_box-0.5.1.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx       20 b- defN 23-Jun-07 09:09 channel_box-0.5.1.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      810 b- defN 23-Jun-07 09:09 channel_box-0.5.1.5.dist-info/RECORD
-10 files, 17825 bytes uncompressed, 5952 bytes compressed:  66.6%
+-rwxr-xr-x  2.0 unx     1094 b- defN 23-Jul-09 19:13 channel_box-0.5.1.7.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3052 b- defN 23-Jul-09 19:13 channel_box-0.5.1.7.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-09 19:13 channel_box-0.5.1.7.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       20 b- defN 23-Jul-09 19:13 channel_box-0.5.1.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      810 b- defN 23-Jul-09 19:13 channel_box-0.5.1.7.dist-info/RECORD
+10 files, 17873 bytes uncompressed, 5979 bytes compressed:  66.5%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: example/channel/urls.py
 Comment: 
 
 Filename: example/channel/views.py
 Comment: 
 
-Filename: channel_box-0.5.1.5.dist-info/LICENSE
+Filename: channel_box-0.5.1.7.dist-info/LICENSE
 Comment: 
 
-Filename: channel_box-0.5.1.5.dist-info/METADATA
+Filename: channel_box-0.5.1.7.dist-info/METADATA
 Comment: 
 
-Filename: channel_box-0.5.1.5.dist-info/WHEEL
+Filename: channel_box-0.5.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: channel_box-0.5.1.5.dist-info/top_level.txt
+Filename: channel_box-0.5.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: channel_box-0.5.1.5.dist-info/RECORD
+Filename: channel_box-0.5.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## channel_box/src.py

```diff
@@ -6,14 +6,30 @@
 import uuid
 import logging
 from typing import Any
 from enum import Enum
 from starlette.websockets import WebSocket
 
 
+class ChannelAddStatus(Enum):
+    ADDED = 1
+    EXIST = 2 
+
+
+class ChannelRemoveStatus(Enum):
+    CHANNEL_REMOVED = 1
+    GROUP_REMOVED = 2
+    DOES_NOT_EXIST = 3 
+
+
+class GroupSendStatus(Enum):
+    GROUP_SEND = 1
+    NO_SUCH_GROUP = 2
+
+
 class Channel:
     """ 
     Channel class - active user channel (adapter to starlette.websockets.WebSocket).
 
     websocket: WebSocket # Starlette websocket instance (see starlette documentation)
     expires: int -> Channel ttl in seconds
     encoding: str [json, text, bytes] -> Encoding of sending data
@@ -72,48 +88,39 @@
     _GROUPS: dict = {}
     _GROUPS_HISTORY: dict = {}
     _HISTORY_SIZE: int = os.getenv("CHANNEL_BOX_HISTORY_SIZE", 1_048_576)
  
     @classmethod  
     async def channel_add(cls, group_name: str, channel: Channel) -> Enum:
 
-        class Status(Enum):
-            ADDED = 1
-            EXIST = 2 
-
         if group_name not in cls._GROUPS:
             cls._GROUPS[group_name] = {}
-            status = Status.ADDED
+            status = ChannelAddStatus.ADDED
         else:
-            status = Status.EXIST  
+            status = ChannelAddStatus.EXIST  
 
         cls._GROUPS[group_name][channel] = 1
         return status
     
     @classmethod  
     async def channel_remove(cls, group_name: str, channel: Channel) -> Enum:
 
-        class Status(Enum):
-            CHANNEL_REMOVED = 1
-            GROUP_REMOVED = 2
-            DOES_NOT_EXIST = 3 
-
         if channel in cls._GROUPS.get(group_name, {}):
             try:
                 del cls._GROUPS[group_name][channel]
-                status = Status.CHANNEL_REMOVED 
+                status = ChannelRemoveStatus.CHANNEL_REMOVED 
             except:
-                status = Status.DOES_NOT_EXIST    
+                status = ChannelRemoveStatus.DOES_NOT_EXIST    
 
         if not any(cls._GROUPS.get(group_name, {})):
             try:
                 del cls._GROUPS[group_name]
-                status = Status.GROUP_REMOVED 
+                status = ChannelRemoveStatus.GROUP_REMOVED 
             except:
-                status = Status.DOES_NOT_EXIST 
+                status = ChannelRemoveStatus.DOES_NOT_EXIST 
 
         await cls._clean_expired()
         return status
 
     @classmethod
     async def groups(cls) -> dict:
         return cls._GROUPS
@@ -122,28 +129,24 @@
     async def groups_flush(cls) -> True:
         cls._GROUPS = {}
         return True
     
     @classmethod
     async def group_send(cls, group_name: str="", payload: dict={}, history: bool=False, **kwargs) -> Enum:
         
-        class Status(Enum):
-            CHANNEL_SEND = 1
-            NO_SUCH_GROUP = 2
-
         if history:
             cls._GROUPS_HISTORY.setdefault(group_name, [])
             cls._GROUPS_HISTORY[group_name].append({"payload": payload, "uuid": uuid.uuid4(), "datetime": datetime.datetime.now()})
             if sys.getsizeof(cls._GROUPS_HISTORY[group_name]) > cls._HISTORY_SIZE:  
                 cls._GROUPS_HISTORY[group_name] = []
 
-        status = Status.NO_SUCH_GROUP 
+        status = GroupSendStatus.NO_SUCH_GROUP 
         for channel in cls._GROUPS.get(group_name, {}):
             await channel.send(payload)
-            status = Status.CHANNEL_SEND 
+            status = GroupSendStatus.GROUP_SEND 
 
         return status
 
     @classmethod
     async def history(cls, group_name: str="") -> dict: 
         return cls._GROUPS_HISTORY.get(group_name, {}) if group_name else cls._GROUPS_HISTORY
     
@@ -157,16 +160,16 @@
         for group_name in list(cls._GROUPS):        
             for channel in cls._GROUPS.get(group_name, {}):
                 _is_expired = await channel._is_expired()
                 if _is_expired:
                     try:
                         del cls._GROUPS[group_name][channel]
                     except:
-                        logging.debug("no such channel")
+                        logging.debug("No such channel")
             if not any(cls._GROUPS.get(group_name, {})):
                 try:
                     del cls._GROUPS[group_name]
                 except Exception as e:
-                    logging.debug("no such group")
+                    logging.debug("No such group")
```

## Comparing `channel_box-0.5.1.5.dist-info/LICENSE` & `channel_box-0.5.1.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `channel_box-0.5.1.5.dist-info/METADATA` & `channel_box-0.5.1.7.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: channel-box
-Version: 0.5.1.5
+Version: 0.5.1.7
 Summary: ChannelBox it is a package for Starlette framework that allows you to make named webscoket channels.
 Home-page: https://github.com/Sobolev5/channel-box
 Author: Sobolev Andrey
 Author-email: email.asobolev@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -63,35 +63,35 @@
 
 ## Setup channel 
 ```python
 from starlette.endpoints import WebSocketEndpoint
 from channel_box import Channel, ChannelBox
 
 class WsChatEndpoint(WebSocketEndpoint):
-    
+
     async def on_connect(self, websocket):
         group_name = websocket.query_params.get("group_name")  # group name */ws?group_name=MyChat
         if group_name:
             channel = Channel(websocket, expires=60*60, encoding="json") # define user channel
-            channel = await ChannelBox.channel_add(group_name, channel) # add channel to named group
+            channel = await ChannelBox.channel_add(group_name, channel) # add user channel to named group
         await websocket.accept()
 
     async def on_receive(self, websocket, data):
         data = json.loads(data)
         message = data["message"]
         username = data["username"]     
 
         if message.strip():
             payload = {
                 "username": username,
                 "message": message,
             }
             group_name = websocket.query_params.get("group_name")
             if group_name:
-                await ChannelBox.group_send(group_name, payload) # send to all channels
+                await ChannelBox.group_send(group_name, payload) # send to all users channels
 ```
 
 ## Send messages 
 Send message to any channel from any part of your code:
 ```python
 from channel_box import ChannelBox
```

## Comparing `channel_box-0.5.1.5.dist-info/RECORD` & `channel_box-0.5.1.7.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 channel_box/__init__.py,sha256=IQ6PdTXL75hv4rFxJ0Mjns30mHJIX_UFUp28JwsU6CY,48
-channel_box/src.py,sha256=vNjWM0H1HFlyO-yBR-hra9MXu2kG8H7-vfGL3qZ-AN0,5724
+channel_box/src.py,sha256=iyWXOhuD0qkgYATYayGwYo28B_UtGZkxthCA2yr111A,5765
 example/channel/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 example/channel/urls.py,sha256=R_FB2kG6cMHa_OferyJSll7ixYcnIvxqSTKgjuQFmiI,599
 example/channel/views.py,sha256=JS7xGVULStUowWxpm_-x9jEGrZGf37bL_yrKBz2Z8yk,6393
-channel_box-0.5.1.5.dist-info/LICENSE,sha256=BvmWh0aXPp8jrD0GS25NwyJ321UbcQ7KIui9wAmwVD0,1094
-channel_box-0.5.1.5.dist-info/METADATA,sha256=wlCq-at3L5u7EKja64dqbDrcG1RhYwI5BipRcWLzZx8,3045
-channel_box-0.5.1.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-channel_box-0.5.1.5.dist-info/top_level.txt,sha256=mjnxqFEWVz6Q-V_iwda7dXI5euFqxEJoqnhuKt-k6sI,20
-channel_box-0.5.1.5.dist-info/RECORD,,
+channel_box-0.5.1.7.dist-info/LICENSE,sha256=BvmWh0aXPp8jrD0GS25NwyJ321UbcQ7KIui9wAmwVD0,1094
+channel_box-0.5.1.7.dist-info/METADATA,sha256=vmK6hw7tkC9Ikdy6W_yblA5FzbpudQwoHwkZYrPac9s,3052
+channel_box-0.5.1.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+channel_box-0.5.1.7.dist-info/top_level.txt,sha256=mjnxqFEWVz6Q-V_iwda7dXI5euFqxEJoqnhuKt-k6sI,20
+channel_box-0.5.1.7.dist-info/RECORD,,
```

