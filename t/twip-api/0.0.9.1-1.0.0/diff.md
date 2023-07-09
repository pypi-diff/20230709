# Comparing `tmp/twip_api-0.0.9.1-py3-none-any.whl.zip` & `tmp/twip_api-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,12 @@
-Zip file size: 6876 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat       36 b- defN 22-Jan-25 17:01 twip/__init__.py
--rw-rw-rw-  2.0 fat     2200 b- defN 22-Jan-30 09:27 twip/example.py
--rw-rw-rw-  2.0 fat    10724 b- defN 22-Jan-30 09:31 twip/twip.py
--rw-rw-rw-  2.0 fat     1087 b- defN 22-Jan-30 09:37 twip_api-0.0.9.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4081 b- defN 22-Jan-30 09:37 twip_api-0.0.9.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Jan-30 09:37 twip_api-0.0.9.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 22-Jan-30 09:37 twip_api-0.0.9.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      613 b- defN 22-Jan-30 09:37 twip_api-0.0.9.1.dist-info/RECORD
-8 files, 18838 bytes uncompressed, 5812 bytes compressed:  69.1%
+Zip file size: 6964 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat       38 b- defN 23-Jul-09 18:28 twip/__init__.py
+-rw-rw-rw-  2.0 fat     3060 b- defN 23-Jul-09 18:32 twip/data_convert.py
+-rw-rw-rw-  2.0 fat      694 b- defN 23-Jul-09 18:32 twip/example.py
+-rw-rw-rw-  2.0 fat     2857 b- defN 23-Jul-09 18:28 twip/models.py
+-rw-rw-rw-  2.0 fat     5175 b- defN 23-Jul-09 18:32 twip/twip.py
+-rw-rw-rw-  2.0 fat     1087 b- defN 23-Jul-09 19:37 twip_api-1.0.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3403 b- defN 23-Jul-09 19:37 twip_api-1.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-09 19:37 twip_api-1.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-09 19:37 twip_api-1.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      749 b- defN 23-Jul-09 19:37 twip_api-1.0.0.dist-info/RECORD
+10 files, 17160 bytes uncompressed, 5700 bytes compressed:  66.8%
```

## zipnote {}

```diff
@@ -1,25 +1,31 @@
 Filename: twip/__init__.py
 Comment: 
 
+Filename: twip/data_convert.py
+Comment: 
+
 Filename: twip/example.py
 Comment: 
 
+Filename: twip/models.py
+Comment: 
+
 Filename: twip/twip.py
 Comment: 
 
-Filename: twip_api-0.0.9.1.dist-info/LICENSE
+Filename: twip_api-1.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: twip_api-0.0.9.1.dist-info/METADATA
+Filename: twip_api-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: twip_api-0.0.9.1.dist-info/WHEEL
+Filename: twip_api-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: twip_api-0.0.9.1.dist-info/top_level.txt
+Filename: twip_api-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: twip_api-0.0.9.1.dist-info/RECORD
+Filename: twip_api-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## twip/__init__.py

 * *Ordering differences only*

```diff
@@ -1,3 +1,3 @@
-name = "twip"
+from .twip import *
 
-from .twip import *
+name = "twip"
```

## twip/example.py

```diff
@@ -1,71 +1,29 @@
-import twip
+from twip import Twip, Donate, Follow, Subscribe, Hosting, Cheer, Sound, Slotmachine
 
-Twip = twip.Twip()
 
-@Twip.event
-def on_ready():
-    print("Twip is ready!")
-
-@Twip.event
-def on_donate(ctx):
-    print("===on_donate===")
-    print(f"id : {ctx.id}")
-    print(f"nickname : {ctx.nickname}")
-    print(f"amount : {ctx.amount}")
-    print(f"comment : {ctx.comment}")
-    print(f"watcher_id : {ctx.watcher_id}")
-    print(f"subbed : {ctx.subbed}")
-    print(f"repeat : {ctx.repeat}")
-    print(f"ttstype : {ctx.tts_type}")
-    print(f"ttsurl : {ctx.tts_url}")
-    print(f"slotmachine.items : {ctx.slotmachine.items}")
-    print(f"slotmachine.result : {ctx.slotmachine.result}")
-    print(f"slotmachine.reward_id : {ctx.slotmachine.reward_id}")
-    print(f"slotmachine.sound : {ctx.slotmachine.sound}")
-    print(f"slotmachine.point : {ctx.slotmachine.point}")
-    print(f"slotmachine.duration : {ctx.slotmachine.duration}")
-    print(f"effect : {ctx.effect}")
-    print(f"variation_id : {ctx.variation_id}")
-
-@Twip.event
-def on_subscribe(ctx):
-    print("===on_subscribe===")
-    print(f"username : {ctx.username}")
-    print(f"months : {ctx.months}")
-    print(f"message : {ctx.message}")
-    print(f"method : {ctx.method}")
-    print(f"repeat : {ctx.repeat}")
-    print(f"variation_id : {ctx.variation_id}")
-    
-@Twip.event
-def on_hosting(ctx):
-    print("===on_hosting===")
-    print(f"username : {ctx.username}")
-    print(f"viewers : {ctx.viewers}")
-    print(f"repeat : {ctx.repeat}")
-    print(f"variation_id : {ctx.variation_id}")
-    
-@Twip.event
-def on_cheer(ctx):
-    print("===on_cheer===")
-    print(f"nickname : {ctx.nickname}")
-    print(f"amount : {ctx.amount}")
-    print(f"comment : {ctx.comment}")
-    print(f"repeat : {ctx.repeat}")
-    print(f"variation_id : {ctx.variation_id}")
-    
-@Twip.event
-def on_follow(ctx):
-    print("===on_follow===")
-    print(f"nickname : {ctx.nickname}")
-    print(f"repeat : {ctx.repeat}")
-    print(f"variation_id : {ctx.variation_id}")
-
-@Twip.event
-def on_sound(ctx):
-    print("===on_sound===")
-    print(f"type : {ctx.type}")
-    print(f"url : {ctx.url}")
-    print(f"volume : {ctx.volume}")
+class MyTwip(Twip):
+    def on_ready(self):
+        print("Twip is ready!")
 
-Twip.run("your alert box id", "your twip api token")
+    def on_donate(self, donate: Donate):
+        print(donate)
+
+    def on_follow(self, follow: Follow):
+        print(follow)
+
+    def on_subscribe(self, subscribe: Subscribe):
+        print(subscribe)
+
+    def on_hosting(self, hosting: Hosting):
+        print(hosting)
+
+    def on_cheer(self, cheer: Cheer):
+        print(cheer)
+
+    def on_sound(self, sound: Sound):
+        print(sound)
+
+
+if __name__ == "__main__":
+    myTwip = MyTwip()
+    myTwip.run("your alert box id", "your twip api token")
```

## twip/twip.py

```diff
@@ -1,270 +1,131 @@
-from lib2to3.pgen2 import token
 import websocket
 from json import loads
 from requests import get
 from re import search
 from urllib import parse
 from warnings import warn, filterwarnings
+from models import Donate, Follow, Subscribe, Hosting, Cheer, Sound, Slotmachine
+from data_convert import convert_donate, convert_follow, convert_subscribe, convert_hosting, convert_cheer, convert_sound
 
-class Twip:
+
+class TwipBase():
+    def on_ready(self) -> None:
+        pass
+
+    def on_donate(self, donate: Donate) -> None:
+        pass
+
+    def on_follow(self, follow: Follow) -> None:
+        pass
+
+    def on_subscribe(self, subscribe: Subscribe) -> None:
+        pass
+
+    def on_hosting(self, hosting: Hosting) -> None:
+        pass
+
+    def on_cheer(self, cheer: Cheer) -> None:
+        pass
+
+    def on_sound(self, sound: Sound) -> None:
+        pass
+
+
+class Twip(TwipBase):
     def __init__(self):
         self.id = None
         self.version = None
         self.token = None
         self.sio = websocket.WebSocketApp(
             None,
             on_message=self.on_message,
             on_ping=self.on_ping,
             on_error=self.on_error,
             on_close=self.on_close
         )
         self.ping_interval = 20
         self.ping_timeout = 10
         self.ping_payload = "2"
-        self.events = {}
         self.__is_ready = False
         self.token_crawl = False
-        
-    class Donate:
-        def __init__(self):
-            self.type = "donate"
-            self.id = None
-            self.nickname = None
-            self.amount = None
-            self.comment = None
-            self.watcher_id = None
-            self.subbed = None
-            self.repeat = None
-            self.tts_type = None
-            self.tts_url = None
-            self.slotmachine = self.Slotmachine()
-            self.effect = None
-            self.variation_id = None
-    
-        class Slotmachine:
-            def __init__(self):
-                self.items = None
-                self.result = None
-                self.reward_id = 2
-                self.sound = None
-                self.point = None
-                self.duration = None
-    
-    class Follow:
-        def __init__(self):
-            self.nickname = None
-            self.repeat = None
-            self.variation_id = None
-
-    class Subscribe:
-        def __init__(self):
-            self.username = None
-            self.months = None
-            self.message = None
-            self.method = None
-            self.repeat = None
-            self.variation_id = None
-    
-    class Hosting:
-        def __init__(self):
-            self.username = None
-            self.viewers = None
-            self.repeat = None
-            self.variation_id = None
-    
-    class Cheer:
-        def __init__(self):
-            self.nickname = None
-            self.amount = None
-            self.comment = None
-            self.repeat = None
-            self.variation_id = None
-    
-    class Sound:
-        def __init__(self):
-            self.type = None
-            self.volume = None
-            self.url = None
-    
-    def event(self, func):
-        if func.__name__[:3] != "on_":
-            raise Exception("Event name must start with 'on_'")
-        self.events[self.__event_name_convert(func.__name__)] = func
-
-    @staticmethod
-    def __event_name_convert(name: str) -> str:
-        if name == "on_donate":
-            return "new donate"
-        elif name == "on_follow":
-            return "new follow"
-        elif name == "on_subscribe":
-            return "new sub"
-        elif name == "on_hosting":
-            return "new hosting"
-        elif name == "on_cheer":
-            return "new cheer"
-        elif name == "on_sound":
-            return "sound"
-        elif name == "on_ready":
-            return "on_ready"
-        else:
-            raise Exception("Event name must be one of the following: on_donate, on_follow, on_subscribe, on_hosting, on_cheer, on_sound, on_ready")
 
-    @staticmethod
-    def __data_convert(data: list):
-        data_type = data[0]
-        if data_type == "new donate":
-            data_value = data[1]
-            donate = Twip.Donate()
-            
-            donate.id = data_value.get("_id")
-            donate.nickname = data_value.get("nickname")
-            donate.amount = data_value.get("amount")
-            donate.comment = data_value.get("comment")
-            donate.watcher_id = data_value.get("watcher_id")
-            donate.subbed = data_value.get("subbed")
-            donate.repeat = data_value.get("repeat")
-            donate.tts_type = data_value.get("ttstype")
-            donate.tts_url = data_value.get("ttsurl")
-            if data_value.get("slotmachine_data") != None:
-                donate.slotmachine.items = data_value.get("slotmachine_data").get("items")
-                donate.slotmachine.result = data_value.get("slotmachine_data").get("gotcha")
-                donate.slotmachine.sound = data_value.get("slotmachine_data").get("config").get("sound")
-                donate.slotmachine.point = data_value.get("slotmachine_data").get("config").get("point")
-                donate.slotmachine.duration = data_value.get("slotmachine_data").get("config").get("duration")
-            donate.effect = data_value.get("effect")
-            donate.variation_id = data_value.get("variation_id")
-            
-            return donate
-        
-        elif data_type == "new follow":
-            data_value = data[1]
-            follow = Twip.Follow()
-            
-            follow.nickname = data_value.get("nickname")
-            follow.repeat = data_value.get("repeat")
-            follow.variation_id = data_value.get("variation_id")
-            
-            return follow
-        
-        elif data_type == "new sub":
-            data_value = data[1]
-            subscribe = Twip.Subscribe()
-            
-            subscribe.username = data_value.get("username")
-            subscribe.months = data_value.get("months")
-            subscribe.message = data_value.get("message")
-            subscribe.method = data_value.get("method")
-            subscribe.repeat = data_value.get("repeat")
-            subscribe.variation_id = data_value.get("variation_id")
-            
-            return subscribe
-        
-        elif data_type == "new hosting":
-            data_value = data[1]
-            hosting = Twip.Hosting()
-            
-            hosting.username = data_value.get("username")
-            hosting.viewers = data_value.get("viewers")
-            hosting.repeat = data_value.get("repeat")
-            hosting.variation_id = data_value.get("variation_id")
-            
-            return hosting
-        
-        elif data_type == "new cheer":
-            data_value = data[1]
-            cheer = Twip.Cheer()
-            
-            cheer.nickname = data_value.get("nickname")
-            cheer.amount = data_value.get("amount")
-            cheer.comment = data_value.get("comment")
-            cheer.repeat = data_value.get("repeat")
-            cheer.variation_id = data_value.get("variation_id")
-            
-            return cheer
-        
-        # The type comes in as 'sound:play' or 'sound:stop'
-        elif data_type[:6] == "sound:":
-            if len(data) == 2:
-                data_value = data[1]
-                sound = Twip.Sound()
-                
-                sound.type = data_type[6:]
-                sound.volume = data_value.get("volume")
-                sound.url = data_value.get("url")
-            else:
-                sound = Twip.Sound()
-                sound.type = data_type[6:]
-                
-            return sound
-        
-        else:
-            return None
-    
     def on_message(self, wsapp, message):
         # 0 open Sent from the server when new transport is opened (recheck)
         if message[0] == "0":
             wsapp.send(message)
-            #on_ready event
-            if self.__is_ready == False and self.events.get("on_ready") != None:
-                self.events.get("on_ready")()
+            # on_ready event
+            if self.__is_ready == False:
                 self.__is_ready = True
+                self.on_ready()
+
         elif message[:2] == "42":
             result = loads(message[2:])
-            if result[0] in self.events.keys():
-                self.events[result[0]](self.__data_convert(result))
-            # The type comes in as 'sound:play' or 'sound:stop'
-            elif result[0][:5] in self.events.keys() and result[0][:5] == "sound" :
-                self.events[result[0][:5]](self.__data_convert(result))
- 
+            if result[0] == "new donate":
+                self.on_donate(convert_donate(result))
+            elif result[0] == "new follow":
+                self.on_follow(convert_follow(result))
+            elif result[0] == "new sub":
+                self.on_subscribe(convert_subscribe(result))
+            elif result[0] == "new hosting":
+                self.on_hosting(convert_hosting(result))
+            elif result[0] == "new cheer":
+                self.on_cheer(convert_cheer(result))
+            elif result[0] == "sound:play":
+                self.on_sound(convert_sound(result))
+            elif result[0] == "sound:stop":
+                self.on_sound(convert_sound(result))
+
     def on_ping(self, wsapp):
         wsapp.send(self.ping_payload)
-        
+
     def on_close(self, wsapp, code, reason):
         # Because crawled tokens have time out, set the url to be valid by crawling again.
         if self.token_crawl == True:
             response = get(f"https://twip.kr/widgets/alertbox/"+self.id)
-            self.token = search(r"window.__TOKEN__ = '(.+);", response.text).group()[20:-2]
+            self.token = search(r"window.__TOKEN__ = '(.+);",
+                                response.text).group()[20:-2]
             self.sio.url = f"wss://io.mytwip.net/socket.io/?alertbox_key={self.id}&version={self.version}&{parse.urlencode([('token', self.token)], doseq = True)}&transport=websocket"
-            
+
         self.sio.run_forever(
             ping_interval=self.ping_interval,
             ping_timeout=self.ping_timeout,
             ping_payload=self.ping_payload
-            )
-        
+        )
+
     def on_error(self, wsapp, error):
         raise Exception(error)
-    
+
     def run(self, alert_id: str, api_token: str = None, token_crawl: bool = False) -> None:
         """alert_id : The back of twip's the alert box url
         ex) https://twip.kr/widgets/alertbox/1A2B3CXXXX -> 1A2B3CXXXX
-        
+
         api_token : You can get it from the bottom of https://twip.kr/dashboard/security
-        
+
         token_crawl : If you don't have api_token, set this to True
         """
-        
+
         self.id = alert_id
         response = get(f"https://twip.kr/widgets/alertbox/"+self.id)
-        
-        self.version = search(r"version: '\d{1,3}.\d{1,3}.\d{1,3}',", response.text).group()[10:-2]
+
+        self.version = search(
+            r"version: '\d{1,3}.\d{1,3}.\d{1,3}',", response.text).group()[10:-2]
         self.token_crawl = token_crawl
-        
+
         if api_token == None:
             if token_crawl == True:
                 filterwarnings("always")
                 warn("You don't enter api_token so you get token from alert box url. This token has expiration date and is not recommended. Please visit the page below and issue API Token: https://twip.kr/dashboard/security.", Warning)
-                self.token = search(r"window.__TOKEN__ = '(.+);", response.text).group()[20:-2]
+                self.token = search(
+                    r"window.__TOKEN__ = '(.+);", response.text).group()[20:-2]
             else:
-                raise(Exception("You don't enter api_token and token_crawl option is False. Please visit the page below and issue API Token: https://twip.kr/dashboard/security.\n\nIf you want to run with alert_id only, set token_crawl option to True"))
+                raise (Exception("You don't enter api_token and token_crawl option is False. Please visit the page below and issue API Token: https://twip.kr/dashboard/security.\n\nIf you want to run with alert_id only, set token_crawl option to True"))
         else:
             self.token = api_token
-        
+
         self.sio.url = f"wss://io.mytwip.net/socket.io/?alertbox_key={alert_id}&version={self.version}&{parse.urlencode([('token', self.token)], doseq = True)}&transport=websocket"
-        
+
         self.sio.run_forever(
             ping_interval=self.ping_interval,
             ping_timeout=self.ping_timeout,
             ping_payload=self.ping_payload
-            )
+        )
```

## Comparing `twip_api-0.0.9.1.dist-info/LICENSE` & `twip_api-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `twip_api-0.0.9.1.dist-info/RECORD` & `twip_api-1.0.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-twip/__init__.py,sha256=Icg_Kv9uymYZAp51sDMYykxjMxb4VEEvuFe8sR8y9Zg,36
-twip/example.py,sha256=mc1uXTyiC78rpgmS9iFFARZ_R1u1_5eunYGxlbUDFYE,2200
-twip/twip.py,sha256=-06zOpRrAbutAMKl9Vico-9M7BRCmTN6rR7RyXp3QLk,10724
-twip_api-0.0.9.1.dist-info/LICENSE,sha256=hrXRt6D6Eazwv6fLb0L_ye_721aKj4shPNAQAVFJa2U,1087
-twip_api-0.0.9.1.dist-info/METADATA,sha256=8plwBa923pdi7wwRCF-rxf1pQ_vbvEyVPHzhq_hPT1Y,4081
-twip_api-0.0.9.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-twip_api-0.0.9.1.dist-info/top_level.txt,sha256=OfaQCH5CQNIEv8dpOTre741XZurOuyRytxT9GOpapWI,5
-twip_api-0.0.9.1.dist-info/RECORD,,
+twip/__init__.py,sha256=_hJMUBUww99jKvdQugbcGnL0oQu1fkw6k4kmosYj8qQ,38
+twip/data_convert.py,sha256=_kQO8IHOhyaTGPFBc11ubPVOgewsFaeFCHlCJBlIYlk,3060
+twip/example.py,sha256=ZPoAplmtQ_cLJZ0iQO5eEtnmtihMG-Y2tUKjaiFCutE,694
+twip/models.py,sha256=giB1q-qek_2qnTzvtqCHENSnb9n-JTap14NwXNZTl-k,2857
+twip/twip.py,sha256=9ReaG0i1dy4xPp31OhfxhSktJNlfFPgZxIMoGEzr2-A,5175
+twip_api-1.0.0.dist-info/LICENSE,sha256=hrXRt6D6Eazwv6fLb0L_ye_721aKj4shPNAQAVFJa2U,1087
+twip_api-1.0.0.dist-info/METADATA,sha256=0ux4hNWMKDxftIVt6kjbTiS2KZGKJer4c399s_rAICE,3403
+twip_api-1.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+twip_api-1.0.0.dist-info/top_level.txt,sha256=OfaQCH5CQNIEv8dpOTre741XZurOuyRytxT9GOpapWI,5
+twip_api-1.0.0.dist-info/RECORD,,
```

