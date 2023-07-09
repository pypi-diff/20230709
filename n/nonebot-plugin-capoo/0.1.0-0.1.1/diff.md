# Comparing `tmp/nonebot_plugin_capoo-0.1.0.tar.gz` & `tmp/nonebot_plugin_capoo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_capoo-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_capoo-0.1.1.tar", max compression
```

## Comparing `nonebot_plugin_capoo-0.1.0.tar` & `nonebot_plugin_capoo-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-07-09 07:51:43.958368 nonebot_plugin_capoo-0.1.0/LICENSE
--rw-r--r--   0        0        0     3589 2023-07-09 07:51:43.958368 nonebot_plugin_capoo-0.1.0/README.md
--rw-r--r--   0        0        0     4468 2023-07-09 07:51:43.958368 nonebot_plugin_capoo-0.1.0/nonebot_plugin_capoo/__init__.py
--rw-r--r--   0        0        0      520 2023-07-09 07:51:43.958368 nonebot_plugin_capoo-0.1.0/nonebot_plugin_capoo/config.py
--rw-r--r--   0        0        0     2240 2023-07-09 07:51:43.958368 nonebot_plugin_capoo-0.1.0/nonebot_plugin_capoo/download.py
--rw-r--r--   0        0        0      576 2023-07-09 07:51:43.958368 nonebot_plugin_capoo-0.1.0/nonebot_plugin_capoo/sqlite.py
--rw-r--r--   0        0        0      599 2023-07-09 07:51:43.958368 nonebot_plugin_capoo-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4441 1970-01-01 00:00:00.000000 nonebot_plugin_capoo-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-09 10:46:20.018078 nonebot_plugin_capoo-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3840 2023-07-09 10:46:20.018078 nonebot_plugin_capoo-0.1.1/README.md
+-rw-r--r--   0        0        0     4478 2023-07-09 10:46:20.022078 nonebot_plugin_capoo-0.1.1/nonebot_plugin_capoo/__init__.py
+-rw-r--r--   0        0        0      520 2023-07-09 10:46:20.022078 nonebot_plugin_capoo-0.1.1/nonebot_plugin_capoo/config.py
+-rw-r--r--   0        0        0     2805 2023-07-09 10:46:20.022078 nonebot_plugin_capoo-0.1.1/nonebot_plugin_capoo/download.py
+-rw-r--r--   0        0        0      469 2023-07-09 10:46:20.022078 nonebot_plugin_capoo-0.1.1/nonebot_plugin_capoo/sqlite.py
+-rw-r--r--   0        0        0      599 2023-07-09 10:46:20.022078 nonebot_plugin_capoo-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4692 1970-01-01 00:00:00.000000 nonebot_plugin_capoo-0.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_capoo-0.1.0/LICENSE` & `nonebot_plugin_capoo-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_capoo-0.1.0/README.md` & `nonebot_plugin_capoo-0.1.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -88,17 +88,23 @@
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | `capoo` | 群员 | 否 | 群聊 | 随机发送一张 capoo 的表情包 |
 | `添加capoo` | 超管 | 否 | 群聊 | 让 bot 存储图片 |
 
 注意 `添加capoo` 指令在配置项 `capoo_download` 为 False 时将不生效。
 
-`添加capoo` 指令会将图片储存至 `data/capoo/your_picture` 下。
+`添加capoo` 指令会将图片储存至 `data/capoo/your_picture` 下，你可以放置图片在这个文件夹里面，插件启动后会检验这里面的图片文件。
 
 ### 效果图
+#### `capoo` 指令
 <img src="./docs/preview.jpg" style="zoom:30%;" />
 
+#### `添加capoo` 指令
+<img src="./docs/preview2.jpg" style="zoom:30%;" />
+
+<img src="./docs/preview3.jpg" style="zoom:30%;" />
+
 ## TODO
 - [x] 指令触发 bot 发送图片
 - [x] 在 QQ 上让 bot 存储 capoo 图片
 - [x] 每次存储图片，判断图片是否已经存在，避免重复加入
 - [ ] 指定某个序号的图片发送
```

#### html2text {}

```diff
@@ -27,11 +27,14 @@
 å¾æºéä¸è½½ãä½ ä¹å¯ä»¥èªè¡æå¨ä¸è½½ï¼æ¾ç½®å¨ä½ ç bot
 é¡¹ç®æ ¹ç®å½ä¸ç `data/capoo/picture` æä»¶å¤¹ä¸ã ## ð ä½¿ç¨ ###
 æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:---
 -:|:----:|:----:| | `capoo` | ç¾¤å | å¦ | ç¾¤è | éæºåéä¸å¼  capoo
 çè¡¨æå | | `æ·»å capoo` | è¶ç®¡ | å¦ | ç¾¤è | è®© bot å­å¨å¾ç |
 æ³¨æ `æ·»å capoo` æä»¤å¨éç½®é¡¹ `capoo_download` ä¸º False
 æ¶å°ä¸çæã `æ·»å capoo` æä»¤ä¼å°å¾çå¨å­è³ `data/capoo/
-your_picture` ä¸ã ### ææå¾ [./docs/preview.jpg] ## TODO - [x]
-æä»¤è§¦å bot åéå¾ç - [x] å¨ QQ ä¸è®© bot å­å¨ capoo å¾ç - [x]
+your_picture`
+ä¸ï¼ä½ å¯ä»¥æ¾ç½®å¾çå¨è¿ä¸ªæä»¶å¤¹éé¢ï¼æä»¶å¯å¨åä¼æ£éªè¿éé¢çå¾çæä»¶ã
+### ææå¾ #### `capoo` æä»¤ [./docs/preview.jpg] #### `æ·»å capoo`
+æä»¤ [./docs/preview2.jpg] [./docs/preview3.jpg] ## TODO - [x] æä»¤è§¦å
+bot åéå¾ç - [x] å¨ QQ ä¸è®© bot å­å¨ capoo å¾ç - [x]
 æ¯æ¬¡å­å¨å¾çï¼å¤æ­å¾çæ¯å¦å·²ç»å­å¨ï¼é¿åéå¤å å¥ - [ ]
 æå®æä¸ªåºå·çå¾çåé
```

### Comparing `nonebot_plugin_capoo-0.1.0/nonebot_plugin_capoo/__init__.py` & `nonebot_plugin_capoo-0.1.1/nonebot_plugin_capoo/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,20 +61,20 @@
             resp = await client.get(f"https://git.acwing.com/HuParry/capoo/-/raw/master/capoo ({random.randint(1, capoo_list_len)}).gif", timeout=5.0)
         picbytes = BytesIO(resp.content).getvalue()
         try:
             await picture.send(MessageSegment.image(picbytes))
         except:
             await picture.send(f'capoo出不来了，稍后再试试吧~')
 
-add = on_fullmatch('添加capoo', permission=SUPERUSER, priority=1, block=True)
+def reply_rule():
+    return capoo_download
+
+add = on_fullmatch('添加capoo', rule=reply_rule, permission=SUPERUSER, priority=1, block=True)
 @add.got("pic", prompt="请发送图片！")
 async def add_pic(pic_list: Message = Arg('pic')):
-    if capoo_download == False:
-        return
-    
     conn = sqlite3.connect(capoo_path / 'md5.db')
     cursor = conn.cursor()
     cursor.execute('''
         CREATE TABLE IF NOT EXISTS Picture (
             md5 TEXT PRIMARY KEY,
             img_url TEXT
         )
```

### Comparing `nonebot_plugin_capoo-0.1.0/nonebot_plugin_capoo/config.py` & `nonebot_plugin_capoo-0.1.1/nonebot_plugin_capoo/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_capoo-0.1.0/nonebot_plugin_capoo/download.py` & `nonebot_plugin_capoo-0.1.1/nonebot_plugin_capoo/download.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import asyncio
 import httpx
 
 from nonebot.log import logger
-from nonebot import get_driver
 import sqlite3
 import hashlib
 import os
 from .sqlite import check_md5
 from .config import capoo_pic_path, capoo_path, \
-    capoo_filename, capoo_pic, capoo_pic2_path
+    capoo_filename, capoo_pic, capoo_pic2_path, capoo_pic2
 
 capoo_list_len = 456
 async def download_url(url: str) -> bytes:
     async with httpx.AsyncClient() as client:
         for i in range(3):
             try:
                 resp = await client.get(url, timeout=20)
@@ -47,21 +46,33 @@
         )
     ''')
 
     for i in range(1, capoo_list_len + 1) :
         file_name = capoo_filename.format(index=str(i))
         file_path = capoo_pic_path / file_name
         if file_path.exists():
+            with file_path.open("rb") as f:
+                data = f.read()
+            fmd5 = hashlib.md5(data).hexdigest()
+            check_md5(conn, cursor, fmd5, f"{capoo_pic}/{capoo_filename.format(index=str(i))}")
             continue
         logger.info(f"Downloading {file_name} ...")
         try:
             data = await download_resources(file_name)
             fmd5 = hashlib.md5(data).hexdigest()
             
             if (not check_md5(conn, cursor, fmd5, f"{capoo_pic}/{capoo_filename.format(index=str(i))}")) :
+                logger.info(f"文件夹中有相同的图片，本张照片跳过")
                 continue
 
             with file_path.open("wb") as f:
                 f.write(data)
 
         except Exception as e:
-            logger.warning(str(e))
+            logger.warning(str(e))
+    
+    capoo_pic2_list = os.listdir(str(capoo_pic2_path))
+    for file_name in capoo_pic2_list:
+        with file_path.open("rb") as f:
+            data = f.read()
+        fmd5 = hashlib.md5(data).hexdigest()
+        check_md5(conn, cursor, fmd5, f"{capoo_pic2}/{file_name}")
```

### Comparing `nonebot_plugin_capoo-0.1.0/pyproject.toml` & `nonebot_plugin_capoo-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-capoo"
-version = "0.1.0"
+version = "0.1.1"
 description = "一个发送 capoo 表情包的插件"
 authors = ["HuParry <huparry@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_capoo"}]
 homepage = "https://github.com/HuParry/nonebot-plugin-capoo"
 repository = "https://github.com/HuParry/nonebot-plugin-capoo"
```

### Comparing `nonebot_plugin_capoo-0.1.0/PKG-INFO` & `nonebot_plugin_capoo-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-capoo
-Version: 0.1.0
+Version: 0.1.1
 Summary: 一个发送 capoo 表情包的插件
 Home-page: https://github.com/HuParry/nonebot-plugin-capoo
 License: MIT
 Author: HuParry
 Author-email: huparry@outlook.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -110,17 +110,23 @@
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | `capoo` | 群员 | 否 | 群聊 | 随机发送一张 capoo 的表情包 |
 | `添加capoo` | 超管 | 否 | 群聊 | 让 bot 存储图片 |
 
 注意 `添加capoo` 指令在配置项 `capoo_download` 为 False 时将不生效。
 
-`添加capoo` 指令会将图片储存至 `data/capoo/your_picture` 下。
+`添加capoo` 指令会将图片储存至 `data/capoo/your_picture` 下，你可以放置图片在这个文件夹里面，插件启动后会检验这里面的图片文件。
 
 ### 效果图
+#### `capoo` 指令
 <img src="./docs/preview.jpg" style="zoom:30%;" />
 
+#### `添加capoo` 指令
+<img src="./docs/preview2.jpg" style="zoom:30%;" />
+
+<img src="./docs/preview3.jpg" style="zoom:30%;" />
+
 ## TODO
 - [x] 指令触发 bot 发送图片
 - [x] 在 QQ 上让 bot 存储 capoo 图片
 - [x] 每次存储图片，判断图片是否已经存在，避免重复加入
 - [ ] 指定某个序号的图片发送
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-capoo Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-capoo Version: 0.1.1 Summary:
 ä¸ä¸ªåé capoo è¡¨æåçæä»¶ Home-page: https://github.com/HuParry/
 nonebot-plugin-capoo License: MIT Author: HuParry Author-email:
 huparry@outlook.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: asyncio
@@ -39,11 +39,14 @@
 å¾æºéä¸è½½ãä½ ä¹å¯ä»¥èªè¡æå¨ä¸è½½ï¼æ¾ç½®å¨ä½ ç bot
 é¡¹ç®æ ¹ç®å½ä¸ç `data/capoo/picture` æä»¶å¤¹ä¸ã ## ð ä½¿ç¨ ###
 æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:---
 -:|:----:|:----:| | `capoo` | ç¾¤å | å¦ | ç¾¤è | éæºåéä¸å¼  capoo
 çè¡¨æå | | `æ·»å capoo` | è¶ç®¡ | å¦ | ç¾¤è | è®© bot å­å¨å¾ç |
 æ³¨æ `æ·»å capoo` æä»¤å¨éç½®é¡¹ `capoo_download` ä¸º False
 æ¶å°ä¸çæã `æ·»å capoo` æä»¤ä¼å°å¾çå¨å­è³ `data/capoo/
-your_picture` ä¸ã ### ææå¾ [./docs/preview.jpg] ## TODO - [x]
-æä»¤è§¦å bot åéå¾ç - [x] å¨ QQ ä¸è®© bot å­å¨ capoo å¾ç - [x]
+your_picture`
+ä¸ï¼ä½ å¯ä»¥æ¾ç½®å¾çå¨è¿ä¸ªæä»¶å¤¹éé¢ï¼æä»¶å¯å¨åä¼æ£éªè¿éé¢çå¾çæä»¶ã
+### ææå¾ #### `capoo` æä»¤ [./docs/preview.jpg] #### `æ·»å capoo`
+æä»¤ [./docs/preview2.jpg] [./docs/preview3.jpg] ## TODO - [x] æä»¤è§¦å
+bot åéå¾ç - [x] å¨ QQ ä¸è®© bot å­å¨ capoo å¾ç - [x]
 æ¯æ¬¡å­å¨å¾çï¼å¤æ­å¾çæ¯å¦å·²ç»å­å¨ï¼é¿åéå¤å å¥ - [ ]
 æå®æä¸ªåºå·çå¾çåé
```

