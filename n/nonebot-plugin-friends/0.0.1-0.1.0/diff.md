# Comparing `tmp/nonebot_plugin_friends-0.0.1.tar.gz` & `tmp/nonebot_plugin_friends-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_friends-0.0.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_friends-0.1.0.tar", max compression
```

## Comparing `nonebot_plugin_friends-0.0.1.tar` & `nonebot_plugin_friends-0.1.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1089 2023-07-01 09:08:41.165535 nonebot_plugin_friends-0.0.1/LICENSE
--rw-r--r--   0        0        0     5366 2023-07-02 14:54:19.592652 nonebot_plugin_friends-0.0.1/nonebot_plugin_friends/__init__.py
--rw-r--r--   0        0        0      864 2023-07-02 13:36:36.711075 nonebot_plugin_friends-0.0.1/nonebot_plugin_friends/config.py
--rw-r--r--   0        0        0     1957 2023-07-02 14:53:58.897692 nonebot_plugin_friends-0.0.1/nonebot_plugin_friends/utils.py
--rw-r--r--   0        0        0      994 2023-07-02 11:09:56.289402 nonebot_plugin_friends-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1801 2023-07-02 12:55:28.107975 nonebot_plugin_friends-0.0.1/README.md
--rw-r--r--   0        0        0     2654 1970-01-01 00:00:00.000000 nonebot_plugin_friends-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-07-01 09:08:41.165535 nonebot_plugin_friends-0.1.0/LICENSE
+-rw-r--r--   0        0        0     5347 2023-07-09 13:56:11.538687 nonebot_plugin_friends-0.1.0/nonebot_plugin_friends/__init__.py
+-rw-r--r--   0        0        0     1256 2023-07-09 12:50:10.684895 nonebot_plugin_friends-0.1.0/nonebot_plugin_friends/config.py
+-rw-r--r--   0        0        0     6580 2023-07-09 13:51:45.559350 nonebot_plugin_friends-0.1.0/nonebot_plugin_friends/event.py
+-rw-r--r--   0        0        0      919 2023-07-09 13:02:12.031759 nonebot_plugin_friends-0.1.0/nonebot_plugin_friends/utils.py
+-rw-r--r--   0        0        0      994 2023-07-09 13:52:36.832855 nonebot_plugin_friends-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2175 2023-07-09 13:58:11.810945 nonebot_plugin_friends-0.1.0/README.md
+-rw-r--r--   0        0        0     3018 1970-01-01 00:00:00.000000 nonebot_plugin_friends-0.1.0/PKG-INFO
```

### Comparing `nonebot_plugin_friends-0.0.1/LICENSE` & `nonebot_plugin_friends-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_friends-0.0.1/pyproject.toml` & `nonebot_plugin_friends-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_friends"
-version = "0.0.1"
+version = "0.1.0"
 description = "Nonebot2插件处理好友申请"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_friends"
 repository = "https://github.com/Agnes4m/nonebot_plugin_friends"
 keywords = ["maimai", "nonebot2", "plugin"]
```

### Comparing `nonebot_plugin_friends-0.0.1/PKG-INFO` & `nonebot_plugin_friends-0.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-friends
-Version: 0.0.1
+Version: 0.1.0
 Summary: Nonebot2插件处理好友申请
 Home-page: https://github.com/Agnes4m/nonebot_plugin_friends
 License: MIT
 Keywords: maimai,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.8,<4.0
@@ -47,26 +47,36 @@
 </a>
     <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
     <img src="https://img.shields.io/badge/nonebot-2.0.0-red.svg" alt="NoneBot">
 </div>
 
 ## 指令
 
+### 好友申请（权限为master_id|SUPERUSER）
+
 - (被动) —— 接受好友请求
 - 同意 —— 同意最近一次好友请求
 - 同意[number] —— 同意指定qq号添加好友
+- (回复消息)同意 —— 同意改申请的对象
+
+### 群聊申请(权限为群主|管理|master_id|SUPERUSER)
+
+- (被动) —— 接受群聊申请
+- 同意[number] —— 同意指定qq号添加好友
+- (回复消息)同意 —— 同意改申请的对象
 
 ## env配置
 
 不知道可以不写
 知道就按下面参数改添加到env中
 
-    bot_nickname: str= '宁宁'
-    master_nickname: str = '主人'
+    bot_nickname = '宁宁'
+    master_nickname = '主人'
     master_id = ['114514']
+    group_request = True      # 开启群聊申请处理
 
 
 ## 🙈 其他
 
 - 本项目仅供学习使用，请勿用于商业用途，喜欢该项目可以Star或者提供PR
 - [爱发电](https://afdian.net/a/agnes_digital)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-friends Version: 0.0.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-friends Version: 0.1.0 Summary:
 Nonebot2æä»¶å¤çå¥½åç³è¯· Home-page: https://github.com/Agnes4m/
 nonebot_plugin_friends License: MIT Keywords: maimai,nonebot2,plugin Author:
 Agnes_Digital Author-email: Z735803792@163.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
@@ -10,14 +10,19 @@
 Python :: 3.11 Requires-Dist: nonebot-adapter-onebot (>=2.1.3,<3.0.0) Requires-
 Dist: nonebot2 (>=2.0.0,<3.0.0) Project-URL: Repository, https://github.com/
 Agnes4m/nonebot_plugin_friends Description-Content-Type: text/markdown
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
  # nonebot_plugin_friends __â¨Nonebotåæå¥½åâ¨__ [GitHub_stars] [GitHub
                issues] [QQ_Chat_Group] [pypi] [python] [NoneBot]
-## æä»¤ - (è¢«å¨) ââ æ¥åå¥½åè¯·æ± - åæ ââ
-åææè¿ä¸æ¬¡å¥½åè¯·æ± - åæ[number] ââ
-åææå®qqå·æ·»å å¥½å ## envéç½® ä¸ç¥éå¯ä»¥ä¸å
-ç¥éå°±æä¸é¢åæ°æ¹æ·»å å°envä¸­ bot_nickname: str= 'å®å®'
-master_nickname: str = 'ä¸»äºº' master_id = ['114514'] ## ð å¶ä» -
+## æä»¤ ### å¥½åç³è¯·ï¼æéä¸ºmaster_id|SUPERUSERï¼ - (è¢«å¨) ââ
+æ¥åå¥½åè¯·æ± - åæ ââ åææè¿ä¸æ¬¡å¥½åè¯·æ± - åæ
+[number] ââ åææå®qqå·æ·»å å¥½å - (åå¤æ¶æ¯)åæ ââ
+åææ¹ç³è¯·çå¯¹è±¡ ### ç¾¤èç³è¯·
+(æéä¸ºç¾¤ä¸»|ç®¡ç|master_id|SUPERUSER) - (è¢«å¨) ââ
+æ¥åç¾¤èç³è¯· - åæ[number] ââ åææå®qqå·æ·»å å¥½å -
+(åå¤æ¶æ¯)åæ ââ åææ¹ç³è¯·çå¯¹è±¡ ## envéç½®
+ä¸ç¥éå¯ä»¥ä¸å ç¥éå°±æä¸é¢åæ°æ¹æ·»å å°envä¸­ bot_nickname =
+'å®å®' master_nickname = 'ä¸»äºº' master_id = ['114514'] group_request = True
+# å¼å¯ç¾¤èç³è¯·å¤ç ## ð å¶ä» -
 æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨éï¼åæ¬¢è¯¥é¡¹ç®å¯ä»¥Staræèæä¾PR
 - [ç±åçµ](https://afdian.net/a/agnes_digital)
```

