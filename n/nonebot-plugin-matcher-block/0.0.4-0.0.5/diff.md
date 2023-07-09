# Comparing `tmp/nonebot_plugin_matcher_block-0.0.4.tar.gz` & `tmp/nonebot_plugin_matcher_block-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_matcher_block-0.0.4.tar", last modified: Mon Jun 26 15:25:34 2023, max compression
+gzip compressed data, was "nonebot_plugin_matcher_block-0.0.5.tar", last modified: Sun Jul  9 18:20:10 2023, max compression
```

## Comparing `nonebot_plugin_matcher_block-0.0.4.tar` & `nonebot_plugin_matcher_block-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 15:25:34.909158 nonebot_plugin_matcher_block-0.0.4/
--rw-rw-rw-   0        0        0     1086 2022-12-05 12:34:39.000000 nonebot_plugin_matcher_block-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      284 2023-06-26 15:25:34.907158 nonebot_plugin_matcher_block-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-26 15:25:34.896147 nonebot_plugin_matcher_block-0.0.4/nonebot_plugin_matcher_block/
--rw-rw-rw-   0        0        0     7015 2023-06-26 15:23:03.000000 nonebot_plugin_matcher_block-0.0.4/nonebot_plugin_matcher_block/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 15:25:34.905155 nonebot_plugin_matcher_block-0.0.4/nonebot_plugin_matcher_block.egg-info/
--rw-rw-rw-   0        0        0      284 2023-06-26 15:25:34.000000 nonebot_plugin_matcher_block-0.0.4/nonebot_plugin_matcher_block.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2023-06-26 15:25:34.000000 nonebot_plugin_matcher_block-0.0.4/nonebot_plugin_matcher_block.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 15:25:34.000000 nonebot_plugin_matcher_block-0.0.4/nonebot_plugin_matcher_block.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-26 15:25:34.000000 nonebot_plugin_matcher_block-0.0.4/nonebot_plugin_matcher_block.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-06-26 15:25:34.000000 nonebot_plugin_matcher_block-0.0.4/nonebot_plugin_matcher_block.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 15:25:34.909158 nonebot_plugin_matcher_block-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      530 2023-06-26 15:25:30.000000 nonebot_plugin_matcher_block-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:20:10.388577 nonebot_plugin_matcher_block-0.0.5/
+-rw-rw-rw-   0        0        0     1086 2022-12-05 12:34:39.000000 nonebot_plugin_matcher_block-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      284 2023-07-09 18:20:10.388074 nonebot_plugin_matcher_block-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-09 18:20:10.376912 nonebot_plugin_matcher_block-0.0.5/nonebot_plugin_matcher_block/
+-rw-rw-rw-   0        0        0     6982 2023-07-09 18:17:45.000000 nonebot_plugin_matcher_block-0.0.5/nonebot_plugin_matcher_block/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:20:10.386321 nonebot_plugin_matcher_block-0.0.5/nonebot_plugin_matcher_block.egg-info/
+-rw-rw-rw-   0        0        0      284 2023-07-09 18:20:10.000000 nonebot_plugin_matcher_block-0.0.5/nonebot_plugin_matcher_block.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2023-07-09 18:20:10.000000 nonebot_plugin_matcher_block-0.0.5/nonebot_plugin_matcher_block.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 18:20:10.000000 nonebot_plugin_matcher_block-0.0.5/nonebot_plugin_matcher_block.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-09 18:20:10.000000 nonebot_plugin_matcher_block-0.0.5/nonebot_plugin_matcher_block.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-07-09 18:20:10.000000 nonebot_plugin_matcher_block-0.0.5/nonebot_plugin_matcher_block.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-09 18:20:10.388577 nonebot_plugin_matcher_block-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      530 2023-07-09 18:20:05.000000 nonebot_plugin_matcher_block-0.0.5/setup.py
```

### Comparing `nonebot_plugin_matcher_block-0.0.4/LICENSE` & `nonebot_plugin_matcher_block-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_matcher_block-0.0.4/nonebot_plugin_matcher_block/__init__.py` & `nonebot_plugin_matcher_block-0.0.5/nonebot_plugin_matcher_block/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -39,146 +39,136 @@
 if group_config_file.exists():
     with open(group_config_file, "r", encoding="utf8") as f:
         group_config = json.load(f)
 else:
     group_config = {}
 
 def is_block_group(event:GroupMessageEvent) -> bool:
-    msg = str(event.message)
-    for command in set(group_config.keys()):
-        if command.startswith("^"):
-            if re.match(re.compile(command),msg):
-                break
-            else:
-                continue
-        else:
-            if msg.startswith(command):
-                break
-            else:
-                continue
-    else:
+    msg = event.message.extract_plain_text().strip()
+    group_id = str(event.group_id)
+    if group_id not in group_config:
         return False
-    group_id = event.group_id
-    if group_id in group_config[command]:
-        return True
+    commands = group_config[group_id]
+    for command in commands:
+        if command.startswith("^") and re.match(re.compile(command),msg):
+            return True
+        elif msg.startswith(command):
+            return True
     else:
         return False
 
 cache = {}
 
 def is_block_time(event:GroupMessageEvent) -> bool:
-    msg = str(event.message)
-    for command in set(time_config.keys()):
-        if command.startswith("^"):
-            if re.match(re.compile(command),msg):
-                break
-            else:
-                continue
-        else:
-            if msg.startswith(command):
-                break
-            else:
-                continue
+    msg = event.message.extract_plain_text().strip()
+    group_id = str(event.group_id)
+    if group_id not in time_config:
+        return False
+    commands = time_config[group_id]
+    for command in commands:
+        if command.startswith("^") and re.match(re.compile(command),msg):
+            break
+        elif msg.startswith(command):
+            break
     else:
         return False
 
-    group_id = event.group_id
     user_id = event.user_id
-    cache.setdefault(group_id,{})
-    cd = time.time() - cache[group_id].get(user_id,0)
-    if cd > time_config[command]:
-        cache[group_id][user_id] = time.time()
+    usercache = cache.setdefault(group_id, {}).setdefault(user_id, {})
+    cd = time.time() - usercache.get(command, 0)
+    if cd > commands[command]:
+        usercache[command] = time.time()
         return False
     else:
-        return f"你的【{command}】冷却还有{int(time_config[command] - cd) + 1}秒"
+        return f"你的【{msg}】冷却还有{int(commands[command] - cd) + 1}秒"
 
 from nonebot.message import event_preprocessor
 from nonebot.exception import IgnoredException
 
 @event_preprocessor
 async def do_something(bot:Bot, event:GroupMessageEvent , permission = SUPERUSER | GROUP_ADMIN | GROUP_OWNER):
     if not await permission(bot,event):
         if is_block_group(event):
             raise IgnoredException("本群已屏蔽此指令")
-        if echo := is_block_time(event):
+        elif echo := is_block_time(event):
             await bot.send(event = event, message = echo)
             raise IgnoredException("用户指令正在冷却")
 
 add_block = on_command("添加阻断", permission = SUPERUSER | GROUP_ADMIN | GROUP_OWNER, priority = 5, block = True)
 
 @add_block.handle()
-async def _(matcher: Matcher, event:GroupMessageEvent, arg: Message = CommandArg()):
+async def _(event:GroupMessageEvent, arg: Message = CommandArg()):
     msg = arg.extract_plain_text().strip().split()
     if msg and len(msg) >= 2:
+        group_id = str(event.group_id)
         command = msg[0]
-        if command in ["添加阻断","解除阻断","删除阻断"]:
+        if command in {"添加阻断","解除阻断","删除阻断"}:
             await add_block.finish("不可以这么做")
         block_type = msg[1]
-        if (block_type == "时间" or block_type == "冷却") and len(msg) == 3:
+        if len(msg) == 3 and block_type in {"时间","冷却"}:
             try:
                 cd = int(msg[2])
             except:
                 await add_block.finish(f"添加阻断接受了错误的时间参数：{msg[2]}")
-            time_config[command] = cd
+            time_config.setdefault(group_id,{})[command] = cd
             with open(time_config_file, "w", encoding="utf8") as f:
                 json.dump(time_config, f, ensure_ascii=False, indent=4)
             await add_block.finish(f"指令【{command}】已设置冷却：{cd}s")
+
         elif block_type == "群":
-            group_config.setdefault(command,[])
-            group_config[command].append(event.group_id)
-            group_config[command] = list(set(group_config[command]))
-            with open(group_config_file, "w", encoding="utf8") as f:
-                json.dump(group_config, f, ensure_ascii=False, indent=4)
+            tmp = group_config.setdefault(group_id,[])
+            if command not in tmp:
+                tmp.append(command)
+                with open(group_config_file, "w", encoding="utf8") as f:
+                    json.dump(group_config, f, ensure_ascii=False, indent=4)
             await add_block.finish(f"指令【{command}】已在本群屏蔽。")
 
     await add_block.finish("添加阻断指令格式错误。")
 
 
 del_block = on_command("解除阻断",aliases={"删除阻断"}, permission = SUPERUSER | GROUP_ADMIN | GROUP_OWNER, priority = 5, block = True)
 
 @del_block.handle()
 async def _(matcher: Matcher, event:GroupMessageEvent, arg: Message = CommandArg()):
     msg = arg.extract_plain_text().strip().split()
     if msg and len(msg) == 2:
+        group_id = str(event.group_id)
         command = msg[0]
         block_type = msg[1]
-        if block_type == "时间" or block_type == "冷却":
-            if command in time_config.keys():
-                del time_config[command]
+        if block_type in {"时间","冷却"}:
+            if group_id in time_config and command in time_config[group_id]:
+                del time_config[group_id][command]
                 with open(time_config_file, "w", encoding="utf8") as f:
                     json.dump(time_config, f, ensure_ascii=False, indent=4)
                 await del_block.finish(f"指令【{command}】已解除冷却限制。")
             else:
                 await del_block.finish(f"指令【{command}】没有设置冷却。")
-        elif block_type == "群":
-            group_id = event.group_id
-            if command in group_config.keys():
-                if group_id in group_config[command]:
-                    group_config[command].remove(group_id)
-                    with open(group_config_file, "w", encoding="utf8") as f:
-                        json.dump(group_config, f, ensure_ascii=False, indent=4)
-                    await del_block.finish(f"指令【{command}】已解除屏蔽。")
-
-            await del_block.finish(f"指令【{command}】未屏蔽。")
+        if block_type == "群":
+            if group_id in group_config and command in group_config[group_id]:
+                group_config[group_id].remove(command)
+                with open(group_config_file, "w", encoding="utf8") as f:
+                    json.dump(group_config, f, ensure_ascii=False, indent=4)
+                await del_block.finish(f"指令【{command}】已解除屏蔽。")
+            else:
+                await del_block.finish(f"指令【{command}】未屏蔽。")
 
     await del_block.finish("解除阻断指令格式错误。")
 
 show_block = on_command("查看阻断", permission = SUPERUSER | GROUP_ADMIN | GROUP_OWNER, priority = 5, block = True)
 
 @show_block.handle()
 async def _(matcher: Matcher, event:GroupMessageEvent):
-    group_id = event.group_id
+    group_id = str(event.group_id)
     msg = ""
-    for command in set(group_config.keys()):
-        if group_id in group_config[command]:
-            msg += f"【{command}】：屏蔽\n"
-    for command in set(time_config.keys()):
-        msg += f"【{command}】：{time_config[command]}s\n"
-
-    await show_block.finish(msg[:-1])
+    if group_id in group_config:
+        msg += "".join([f"【{command}】：屏蔽\n" for command in group_config[group_id]])
+    if group_id in time_config:
+        msg += "".join([f"【{command}】：{cd}s\n" for command,cd in time_config[group_id].items()])
+    msg = msg[:-1] if msg else "本群没有阻断。"
+    await show_block.finish(msg)
 
 from nonebot import get_driver
 
 driver = get_driver()
 bots = driver.bots
 
 history = []
```

### Comparing `nonebot_plugin_matcher_block-0.0.4/setup.py` & `nonebot_plugin_matcher_block-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_namespace_packages
 
 setup(
 name='nonebot_plugin_matcher_block',
-version='0.0.4',
+version='0.0.5',
 description='通用指令阻断',
 #long_description=open('README.md','r').read(),
 author='karisaya',
 author_email='1048827424@qq.com',
 license='MIT license',
 include_package_data=True,
 packages=find_namespace_packages(include=["nonebot_plugin_matcher_block"]),
```

