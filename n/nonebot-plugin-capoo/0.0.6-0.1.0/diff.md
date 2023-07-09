# Comparing `tmp/nonebot_plugin_capoo-0.0.6.tar.gz` & `tmp/nonebot_plugin_capoo-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_capoo-0.0.6.tar", max compression
+gzip compressed data, was "nonebot_plugin_capoo-0.1.0.tar", max compression
```

## Comparing `nonebot_plugin_capoo-0.0.6.tar` & `nonebot_plugin_capoo-0.1.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-07-07 17:53:00.934953 nonebot_plugin_capoo-0.0.6/LICENSE
--rw-r--r--   0        0        0     2395 2023-07-07 17:53:00.934953 nonebot_plugin_capoo-0.0.6/README.md
--rw-r--r--   0        0        0     2345 2023-07-07 17:53:00.934953 nonebot_plugin_capoo-0.0.6/nonebot_plugin_capoo/__init__.py
--rw-r--r--   0        0        0      249 2023-07-07 17:53:00.934953 nonebot_plugin_capoo-0.0.6/nonebot_plugin_capoo/config.py
--rw-r--r--   0        0        0     1491 2023-07-07 17:53:00.934953 nonebot_plugin_capoo-0.0.6/nonebot_plugin_capoo/download.py
--rw-r--r--   0        0        0      599 2023-07-07 17:53:00.934953 nonebot_plugin_capoo-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3247 1970-01-01 00:00:00.000000 nonebot_plugin_capoo-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-09 07:51:43.958368 nonebot_plugin_capoo-0.1.0/LICENSE
+-rw-r--r--   0        0        0     3589 2023-07-09 07:51:43.958368 nonebot_plugin_capoo-0.1.0/README.md
+-rw-r--r--   0        0        0     4468 2023-07-09 07:51:43.958368 nonebot_plugin_capoo-0.1.0/nonebot_plugin_capoo/__init__.py
+-rw-r--r--   0        0        0      520 2023-07-09 07:51:43.958368 nonebot_plugin_capoo-0.1.0/nonebot_plugin_capoo/config.py
+-rw-r--r--   0        0        0     2240 2023-07-09 07:51:43.958368 nonebot_plugin_capoo-0.1.0/nonebot_plugin_capoo/download.py
+-rw-r--r--   0        0        0      576 2023-07-09 07:51:43.958368 nonebot_plugin_capoo-0.1.0/nonebot_plugin_capoo/sqlite.py
+-rw-r--r--   0        0        0      599 2023-07-09 07:51:43.958368 nonebot_plugin_capoo-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4441 1970-01-01 00:00:00.000000 nonebot_plugin_capoo-0.1.0/PKG-INFO
```

### Comparing `nonebot_plugin_capoo-0.0.6/LICENSE` & `nonebot_plugin_capoo-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_capoo-0.0.6/nonebot_plugin_capoo/download.py` & `nonebot_plugin_capoo-0.1.0/nonebot_plugin_capoo/download.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import asyncio
 import httpx
-from pathlib import Path
+
 from nonebot.log import logger
 from nonebot import get_driver
+import sqlite3
+import hashlib
+import os
+from .sqlite import check_md5
+from .config import capoo_pic_path, capoo_path, \
+    capoo_filename, capoo_pic, capoo_pic2_path
 
-capoo_path = Path() / "data" / "capoo"
 capoo_list_len = 456
 async def download_url(url: str) -> bytes:
     async with httpx.AsyncClient() as client:
         for i in range(3):
             try:
                 resp = await client.get(url, timeout=20)
                 resp.raise_for_status()
@@ -22,23 +27,41 @@
 def resource_url(path: str) -> str:
     return f"https://git.acwing.com/HuParry/capoo/-/raw/master/{path}"
 
 async def download_resources(path: str) -> bytes:
     return await download_url(resource_url(path))
 
 async def check_resources():
-    if capoo_path.exists():
-        return
-    logger.info(f"未找到capoo文件夹，准备创建/data/capoo文件夹...")
-    capoo_path.mkdir(parents=True, exist_ok=True)
+    if not capoo_pic_path.exists():
+        logger.info(f"未找到capoo文件夹，准备创建/capoo/picture文件夹...")
+        capoo_pic_path.mkdir(parents=True, exist_ok=True)
+    
+    if not capoo_pic2_path.exists():
+        logger.info(f"未找到capoo2文件夹，准备创建/capoo/your_picture文件夹...")
+        capoo_pic2_path.mkdir(parents=True, exist_ok=True)
+    conn = sqlite3.connect(capoo_path / 'md5.db')
+    cursor = conn.cursor()
+    cursor.execute('''
+        CREATE TABLE IF NOT EXISTS Picture (
+            md5 TEXT PRIMARY KEY,
+            img_url TEXT
+        )
+    ''')
+
     for i in range(1, capoo_list_len + 1) :
-        file_name = f"capoo ({i}).gif"
-        file_path = capoo_path / file_name
+        file_name = capoo_filename.format(index=str(i))
+        file_path = capoo_pic_path / file_name
         if file_path.exists():
             continue
         logger.info(f"Downloading {file_name} ...")
         try:
             data = await download_resources(file_name)
+            fmd5 = hashlib.md5(data).hexdigest()
+            
+            if (not check_md5(conn, cursor, fmd5, f"{capoo_pic}/{capoo_filename.format(index=str(i))}")) :
+                continue
+
             with file_path.open("wb") as f:
                 f.write(data)
+
         except Exception as e:
             logger.warning(str(e))
```

### Comparing `nonebot_plugin_capoo-0.0.6/pyproject.toml` & `nonebot_plugin_capoo-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-capoo"
-version = "0.0.6"
+version = "0.1.0"
 description = "一个发送 capoo 表情包的插件"
 authors = ["HuParry <huparry@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_capoo"}]
 homepage = "https://github.com/HuParry/nonebot-plugin-capoo"
 repository = "https://github.com/HuParry/nonebot-plugin-capoo"
```

### Comparing `nonebot_plugin_capoo-0.0.6/PKG-INFO` & `nonebot_plugin_capoo-0.1.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-capoo
-Version: 0.0.6
+Version: 0.1.0
 Summary: 一个发送 capoo 表情包的插件
 Home-page: https://github.com/HuParry/nonebot-plugin-capoo
 License: MIT
 Author: HuParry
 Author-email: huparry@outlook.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -43,14 +43,18 @@
 
 </div>
 
 ## 📖 介绍
 
 capoo 实在是太可爱了，所以我收集了几百张 capoo 的表情包。这个插件用于让 bot 发送 capoo 的表清包。
 
+一开始的版本只能简单地从我的图源里发送表情包，在 v0.1.0 后迎来了重大更新：超级用户可以在群聊里发送指令让 bot 存储表情包。并且插件会判断这个表情包在本地的图片文件夹里是否出现过，这样能避免重复加入某张图片。
+
+随机发送图片是利用的 sqlite3 库里的随机选择指令。
+
 ## 💿 安装
 
 <details>
 <summary>使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
     nb plugin install nonebot-plugin-capoo
@@ -90,19 +94,33 @@
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
 
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
-| capoo_download | 否 | False | 是否开启本地图片存储，Ture为开启本地图片存储 |
+| capoo_download | 否 | False | 是否开启本地图片存储，True为开启本地图片存储 |
+
+图源在 [AC Git](https://git.acwing.com/HuParry/capoo) 上，是国内的远程代码库站点，所以不用担心被墙了而发不出图片。
+
+假如你开启了本地图片存储，插件会自己从 [AC Git](https://git.acwing.com/HuParry/capoo) 图源里下载。你也可以自行手动下载，放置在你的 bot 项目根目录下的 `data/capoo/picture` 文件夹下。
 
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | `capoo` | 群员 | 否 | 群聊 | 随机发送一张 capoo 的表情包 |
+| `添加capoo` | 超管 | 否 | 群聊 | 让 bot 存储图片 |
+
+注意 `添加capoo` 指令在配置项 `capoo_download` 为 False 时将不生效。
+
+`添加capoo` 指令会将图片储存至 `data/capoo/your_picture` 下。
 
 ### 效果图
 <img src="./docs/preview.jpg" style="zoom:30%;" />
 
+## TODO
+- [x] 指令触发 bot 发送图片
+- [x] 在 QQ 上让 bot 存储 capoo 图片
+- [x] 每次存储图片，判断图片是否已经存在，避免重复加入
+- [ ] 指定某个序号的图片发送
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-capoo Version: 0.0.6 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-capoo Version: 0.1.0 Summary:
 ä¸ä¸ªåé capoo è¡¨æåçæä»¶ Home-page: https://github.com/HuParry/
 nonebot-plugin-capoo License: MIT Author: HuParry Author-email:
 huparry@outlook.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: asyncio
@@ -11,23 +11,39 @@
 Project-URL: Repository, https://github.com/HuParry/nonebot-plugin-capoo
 Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
        # nonebot-plugin-capoo _â¨ ä¸ä¸ªåéæä»¤å°±è½è®©ä½ ç bot
     ååºå¯ç±ç capoo çå¾ççæä»¶ â¨_ [license] [pypi] [python]
 ## ð ä»ç» capoo å®å¨æ¯å¤ªå¯ç±äºï¼æä»¥ææ¶éäºå ç¾å¼  capoo
-çè¡¨æåãè¿ä¸ªæä»¶ç¨äºè®© bot åé capoo çè¡¨æ¸åã ## ð¿
+çè¡¨æåãè¿ä¸ªæä»¶ç¨äºè®© bot åé capoo çè¡¨æ¸åã
+ä¸å¼å§ççæ¬åªè½ç®åå°ä»æçå¾æºéåéè¡¨æåï¼å¨ v0.1.0
+åè¿æ¥äºéå¤§æ´æ°ï¼è¶çº§ç¨æ·å¯ä»¥å¨ç¾¤èéåéæä»¤è®© bot
+å­å¨è¡¨æåãå¹¶ä¸æä»¶ä¼å¤æ­è¿ä¸ªè¡¨æåå¨æ¬å°çå¾çæä»¶å¤¹éæ¯å¦åºç°è¿ï¼è¿æ ·è½é¿åéå¤å å¥æå¼ å¾çã
+éæºåéå¾çæ¯å©ç¨ç sqlite3 åºéçéæºéæ©æä»¤ã ## ð¿
 å®è£  ä½¿ç¨ nb-cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-capoo
 ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip pip install nonebot-plugin-capoo   pdm pdm add nonebot-plugin-capoo
 poetry poetry add nonebot-plugin-capoo   conda conda install nonebot-plugin-
 capoo  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `
 [tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_capoo"]  ##
 âï¸ éç½® å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
 é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | capoo_download | å¦ |
-False | æ¯å¦å¼å¯æ¬å°å¾çå­å¨ï¼Tureä¸ºå¼å¯æ¬å°å¾çå­å¨ | ##
-ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:---
---:|:----:|:----:|:----:|:----:| | `capoo` | ç¾¤å | å¦ | ç¾¤è |
-éæºåéä¸å¼  capoo çè¡¨æå | ### ææå¾ [./docs/preview.jpg]
+False | æ¯å¦å¼å¯æ¬å°å¾çå­å¨ï¼Trueä¸ºå¼å¯æ¬å°å¾çå­å¨ |
+å¾æºå¨ [AC Git](https://git.acwing.com/HuParry/capoo)
+ä¸ï¼æ¯å½åçè¿ç¨ä»£ç åºç«ç¹ï¼æä»¥ä¸ç¨æå¿è¢«å¢äºèåä¸åºå¾çã
+åå¦ä½ å¼å¯äºæ¬å°å¾çå­å¨ï¼æä»¶ä¼èªå·±ä» [AC Git](https://
+git.acwing.com/HuParry/capoo)
+å¾æºéä¸è½½ãä½ ä¹å¯ä»¥èªè¡æå¨ä¸è½½ï¼æ¾ç½®å¨ä½ ç bot
+é¡¹ç®æ ¹ç®å½ä¸ç `data/capoo/picture` æä»¶å¤¹ä¸ã ## ð ä½¿ç¨ ###
+æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:---
+-:|:----:|:----:| | `capoo` | ç¾¤å | å¦ | ç¾¤è | éæºåéä¸å¼  capoo
+çè¡¨æå | | `æ·»å capoo` | è¶ç®¡ | å¦ | ç¾¤è | è®© bot å­å¨å¾ç |
+æ³¨æ `æ·»å capoo` æä»¤å¨éç½®é¡¹ `capoo_download` ä¸º False
+æ¶å°ä¸çæã `æ·»å capoo` æä»¤ä¼å°å¾çå¨å­è³ `data/capoo/
+your_picture` ä¸ã ### ææå¾ [./docs/preview.jpg] ## TODO - [x]
+æä»¤è§¦å bot åéå¾ç - [x] å¨ QQ ä¸è®© bot å­å¨ capoo å¾ç - [x]
+æ¯æ¬¡å­å¨å¾çï¼å¤æ­å¾çæ¯å¦å·²ç»å­å¨ï¼é¿åéå¤å å¥ - [ ]
+æå®æä¸ªåºå·çå¾çåé
```

