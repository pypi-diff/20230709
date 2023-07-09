# Comparing `tmp/PyOfficeRobot-0.1.8.tar.gz` & `tmp/PyOfficeRobot-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyOfficeRobot-0.1.8.tar", last modified: Mon May  1 08:24:22 2023, max compression
+gzip compressed data, was "PyOfficeRobot-0.1.9.tar", last modified: Wed Jul  5 16:44:55 2023, max compression
```

## Comparing `PyOfficeRobot-0.1.8.tar` & `PyOfficeRobot-0.1.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 08:24:22.552180 PyOfficeRobot-0.1.8/
--rw-rw-rw-   0        0        0     1093 2022-09-09 17:29:26.000000 PyOfficeRobot-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     8321 2023-05-01 08:24:22.553178 PyOfficeRobot-0.1.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-01 08:24:22.466407 PyOfficeRobot-0.1.8/PyOfficeRobot/
--rw-rw-rw-   0        0        0      195 2023-04-27 13:53:55.000000 PyOfficeRobot-0.1.8/PyOfficeRobot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 08:24:22.512179 PyOfficeRobot-0.1.8/PyOfficeRobot/api/
--rw-rw-rw-   0        0        0        0 2022-09-09 17:57:22.000000 PyOfficeRobot-0.1.8/PyOfficeRobot/api/__init__.py
--rw-rw-rw-   0        0        0     3834 2023-03-19 10:39:04.000000 PyOfficeRobot-0.1.8/PyOfficeRobot/api/chat.py
--rw-rw-rw-   0        0        0     6984 2023-04-17 13:43:21.000000 PyOfficeRobot-0.1.8/PyOfficeRobot/api/file.py
--rw-rw-rw-   0        0        0     9379 2023-04-27 13:42:29.000000 PyOfficeRobot-0.1.8/PyOfficeRobot/api/friend.py
--rw-rw-rw-   0        0        0      727 2023-05-01 08:21:55.000000 PyOfficeRobot-0.1.8/PyOfficeRobot/api/group.py
-drwxrwxrwx   0        0        0        0 2023-05-01 08:24:22.518181 PyOfficeRobot-0.1.8/PyOfficeRobot/core/
--rw-rw-rw-   0        0        0    13556 2023-04-26 14:23:30.000000 PyOfficeRobot-0.1.8/PyOfficeRobot/core/WeChatType.py
--rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 PyOfficeRobot-0.1.8/PyOfficeRobot/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 08:24:22.526179 PyOfficeRobot-0.1.8/PyOfficeRobot/core/group/
--rw-rw-rw-   0        0        0     3880 2023-04-27 14:56:15.000000 PyOfficeRobot-0.1.8/PyOfficeRobot/core/group/Start.py
--rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 PyOfficeRobot-0.1.8/PyOfficeRobot/core/group/__init__.py
--rw-rw-rw-   0        0        0     2612 2023-04-16 14:37:30.000000 PyOfficeRobot-0.1.8/PyOfficeRobot/core/group/ui_file_py.py
-drwxrwxrwx   0        0        0        0 2023-05-01 08:24:22.531180 PyOfficeRobot-0.1.8/PyOfficeRobot/lib/
--rw-rw-rw-   0        0        0      117 2023-03-19 07:06:10.000000 PyOfficeRobot-0.1.8/PyOfficeRobot/lib/CONST.py
--rw-rw-rw-   0        0        0        0 2022-09-12 08:16:33.000000 PyOfficeRobot-0.1.8/PyOfficeRobot/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 08:24:22.538175 PyOfficeRobot-0.1.8/PyOfficeRobot/lib/dec/
--rw-rw-rw-   0        0        0        0 2022-09-14 15:03:44.000000 PyOfficeRobot-0.1.8/PyOfficeRobot/lib/dec/__init__.py
--rw-rw-rw-   0        0        0      385 2022-09-14 15:03:44.000000 PyOfficeRobot-0.1.8/PyOfficeRobot/lib/dec/act_dec.py
-drwxrwxrwx   0        0        0        0 2023-05-01 08:24:22.542179 PyOfficeRobot-0.1.8/PyOfficeRobot/lib/decorator_utils/
--rw-rw-rw-   0        0        0        0 2023-01-31 14:24:33.000000 PyOfficeRobot-0.1.8/PyOfficeRobot/lib/decorator_utils/__init__.py
--rw-rw-rw-   0        0        0     2523 2023-05-01 08:22:39.000000 PyOfficeRobot-0.1.8/PyOfficeRobot/lib/decorator_utils/instruction_url.py
-drwxrwxrwx   0        0        0        0 2023-05-01 08:24:22.497179 PyOfficeRobot-0.1.8/PyOfficeRobot.egg-info/
--rw-rw-rw-   0        0        0     8321 2023-05-01 08:24:22.000000 PyOfficeRobot-0.1.8/PyOfficeRobot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      867 2023-05-01 08:24:22.000000 PyOfficeRobot-0.1.8/PyOfficeRobot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 08:24:22.000000 PyOfficeRobot-0.1.8/PyOfficeRobot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-01 08:16:52.000000 PyOfficeRobot-0.1.8/PyOfficeRobot.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       77 2023-05-01 08:24:22.000000 PyOfficeRobot-0.1.8/PyOfficeRobot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-01 08:24:22.000000 PyOfficeRobot-0.1.8/PyOfficeRobot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7741 2023-04-29 12:53:26.000000 PyOfficeRobot-0.1.8/README.md
--rw-rw-rw-   0        0        0      838 2023-05-01 08:24:22.556173 PyOfficeRobot-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 PyOfficeRobot-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 08:24:22.550176 PyOfficeRobot-0.1.8/tests/
--rw-rw-rw-   0        0        0      193 2023-02-13 13:41:39.000000 PyOfficeRobot-0.1.8/tests/__init__.py
--rw-rw-rw-   0        0        0       13 2023-04-17 13:43:22.000000 PyOfficeRobot-0.1.8/tests/chat.py
--rw-rw-rw-   0        0        0     1293 2023-05-01 08:14:58.000000 PyOfficeRobot-0.1.8/tests/test_file.py
+drwxrwxrwx   0        0        0        0 2023-07-05 16:44:55.262033 PyOfficeRobot-0.1.9/
+-rw-rw-rw-   0        0        0     1093 2022-09-09 17:29:26.000000 PyOfficeRobot-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     8670 2023-07-05 16:44:55.262033 PyOfficeRobot-0.1.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-05 16:44:55.169182 PyOfficeRobot-0.1.9/PyOfficeRobot/
+-rw-rw-rw-   0        0        0      195 2023-04-27 13:53:55.000000 PyOfficeRobot-0.1.9/PyOfficeRobot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 16:44:55.222570 PyOfficeRobot-0.1.9/PyOfficeRobot/api/
+-rw-rw-rw-   0        0        0        0 2022-09-09 17:57:22.000000 PyOfficeRobot-0.1.9/PyOfficeRobot/api/__init__.py
+-rw-rw-rw-   0        0        0     3808 2023-07-05 16:25:11.000000 PyOfficeRobot-0.1.9/PyOfficeRobot/api/chat.py
+-rw-rw-rw-   0        0        0     6802 2023-07-05 16:43:25.000000 PyOfficeRobot-0.1.9/PyOfficeRobot/api/file.py
+-rw-rw-rw-   0        0        0     9386 2023-05-06 15:30:38.000000 PyOfficeRobot-0.1.9/PyOfficeRobot/api/friend.py
+-rw-rw-rw-   0        0        0      727 2023-05-01 08:21:55.000000 PyOfficeRobot-0.1.9/PyOfficeRobot/api/group.py
+drwxrwxrwx   0        0        0        0 2023-07-05 16:44:55.227094 PyOfficeRobot-0.1.9/PyOfficeRobot/core/
+-rw-rw-rw-   0        0        0    13639 2023-07-05 16:33:09.000000 PyOfficeRobot-0.1.9/PyOfficeRobot/core/WeChatType.py
+-rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 PyOfficeRobot-0.1.9/PyOfficeRobot/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 16:44:55.237614 PyOfficeRobot-0.1.9/PyOfficeRobot/core/group/
+-rw-rw-rw-   0        0        0     3880 2023-04-27 14:56:15.000000 PyOfficeRobot-0.1.9/PyOfficeRobot/core/group/Start.py
+-rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 PyOfficeRobot-0.1.9/PyOfficeRobot/core/group/__init__.py
+-rw-rw-rw-   0        0        0     2612 2023-04-16 14:37:30.000000 PyOfficeRobot-0.1.9/PyOfficeRobot/core/group/ui_file_py.py
+drwxrwxrwx   0        0        0        0 2023-07-05 16:44:55.242631 PyOfficeRobot-0.1.9/PyOfficeRobot/lib/
+-rw-rw-rw-   0        0        0      117 2023-03-19 07:06:10.000000 PyOfficeRobot-0.1.9/PyOfficeRobot/lib/CONST.py
+-rw-rw-rw-   0        0        0        0 2022-09-12 08:16:33.000000 PyOfficeRobot-0.1.9/PyOfficeRobot/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 16:44:55.246627 PyOfficeRobot-0.1.9/PyOfficeRobot/lib/dec/
+-rw-rw-rw-   0        0        0        0 2022-09-14 15:03:44.000000 PyOfficeRobot-0.1.9/PyOfficeRobot/lib/dec/__init__.py
+-rw-rw-rw-   0        0        0      385 2022-09-14 15:03:44.000000 PyOfficeRobot-0.1.9/PyOfficeRobot/lib/dec/act_dec.py
+drwxrwxrwx   0        0        0        0 2023-07-05 16:44:55.253165 PyOfficeRobot-0.1.9/PyOfficeRobot/lib/decorator_utils/
+-rw-rw-rw-   0        0        0        0 2023-01-31 14:24:33.000000 PyOfficeRobot-0.1.9/PyOfficeRobot/lib/decorator_utils/__init__.py
+-rw-rw-rw-   0        0        0     2530 2023-06-10 16:27:20.000000 PyOfficeRobot-0.1.9/PyOfficeRobot/lib/decorator_utils/instruction_url.py
+drwxrwxrwx   0        0        0        0 2023-07-05 16:44:55.210970 PyOfficeRobot-0.1.9/PyOfficeRobot.egg-info/
+-rw-rw-rw-   0        0        0     8670 2023-07-05 16:44:54.000000 PyOfficeRobot-0.1.9/PyOfficeRobot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      867 2023-07-05 16:44:55.000000 PyOfficeRobot-0.1.9/PyOfficeRobot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 16:44:54.000000 PyOfficeRobot-0.1.9/PyOfficeRobot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-05 16:15:01.000000 PyOfficeRobot-0.1.9/PyOfficeRobot.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       77 2023-07-05 16:44:54.000000 PyOfficeRobot-0.1.9/PyOfficeRobot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-05 16:44:54.000000 PyOfficeRobot-0.1.9/PyOfficeRobot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8090 2023-07-05 16:43:25.000000 PyOfficeRobot-0.1.9/README.md
+-rw-rw-rw-   0        0        0      838 2023-07-05 16:44:55.271574 PyOfficeRobot-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 PyOfficeRobot-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 16:44:55.260591 PyOfficeRobot-0.1.9/tests/
+-rw-rw-rw-   0        0        0      193 2023-02-13 13:41:39.000000 PyOfficeRobot-0.1.9/tests/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-07 03:03:24.000000 PyOfficeRobot-0.1.9/tests/chat.py
+-rw-rw-rw-   0        0        0     1299 2023-05-07 03:00:06.000000 PyOfficeRobot-0.1.9/tests/test_file.py
```

### Comparing `PyOfficeRobot-0.1.8/LICENSE` & `PyOfficeRobot-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.8/PKG-INFO` & `PyOfficeRobot-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyOfficeRobot
-Version: 0.1.8
+Version: 0.1.9
 Summary: pip install PyOfficeRobot
 Home-page: https://www.python-office.com/office/robot.html
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/PyOfficeRobot/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/README.md
@@ -42,31 +42,29 @@
   </a>
 
 </p>
 
 
 
 
-
-
 # 又一个微信聊天机器人横空出世了，人人可用！
 
 
 之前给大家分享过一个微信机器人：[一个15分钟的视频，教你用Python创建自己的微信聊天机器人！](http://t.cn/A66p30bI)
 
-但是之前这个机器人，需要基于网页版才能用；然而很多朋友的微信，是不能登录网页版微信的。
+但是之前这个机器人，需要基于网页版才能用(有网页版微信的同学，还可以去继续用)；然而很多朋友的微信，是不能登录网页版微信的。
 
 > 有没有一种微信机器人，任何人的微信都可以用，不需要网页微信功能呢？
 
 
 在经过技术检索和开发以后，支持所有微信使用的：**PyOfficeRobot**来啦~
 
 ## 1、安装PyOfficeRobot
 
-1行命令，安装PyOfficeRobot这个库
+1行命令，安装PyOfficeRobot这个库。[安装视频](https://www.bilibili.com/video/BV1Xa411u7yU/)
 ```
 pip install -i https://mirrors.aliyun.com/pypi/simple/ PyOfficeRobot -U
 ```
 
 ## 2、视频教程
 
 - ⭐全套源码：[Github](https://github.com/CoderWanFeng/PyOfficeRobot)
@@ -103,14 +101,19 @@
 
 ## 3、功能Demo
 
 我最近开源了这个库的全部源代码，功能正在开发中，欢迎大家参与开发~
 
 - [演示代码](https://github.com/CoderWanFeng/PyOfficeRobot/tree/main/demo)
 
+## 4、开发者
+
+| 昵称      | 贡献                    | 时间             |
+|---------|-----------------------|----------------|
+| 雷杰 | 解决了微信更新后，不能发送消息和文件的问题 | 2023/7/6 00：30 |
 
 ---
 
 ![](https://python-office-1300615378.cos.ap-chongqing.myqcloud.com/python-office-qr.jpg)
 
 
 ## ⭐Star
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyOfficeRobot Version: 0.1.8 Summary: pip install
+Metadata-Version: 2.1 Name: PyOfficeRobot Version: 0.1.9 Summary: pip install
 PyOfficeRobot Home-page: https://www.python-office.com/office/robot.html
 Author: CoderWanFeng Author-email: 1957875073@qq.com License: MIT Project-URL:
 Bug Tracker, https://github.com/CoderWanFeng/PyOfficeRobot/issues Project-URL:
 Documentation, https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/
 README.md Project-URL: Source Code, https://github.com/CoderWanFeng/
 PyOfficeRobot Platform: any Requires-Python: >=3.6 Description-Content-Type:
 text/markdown License-File: LICENSE
@@ -13,20 +13,22 @@
 [github_star] [gitee_star] [https://img.shields.io/badge/QQ-163434413-orange]
  [https://img.shields.io/badge/%E5%BE%AE%E4%BF%A1-%E4%BA%A4%E6%B5%81%E7%BE%A4-
                                  brightgreen]
 # åä¸ä¸ªå¾®ä¿¡èå¤©æºå¨äººæ¨ªç©ºåºä¸äºï¼äººäººå¯ç¨ï¼
 ä¹åç»å¤§å®¶åäº«è¿ä¸ä¸ªå¾®ä¿¡æºå¨äººï¼
 [ä¸ä¸ª15åéçè§é¢ï¼æä½ ç¨Pythonåå»ºèªå·±çå¾®ä¿¡èå¤©æºå¨äººï¼]
 (http://t.cn/A66p30bI)
-ä½æ¯ä¹åè¿ä¸ªæºå¨äººï¼éè¦åºäºç½é¡µçæè½ç¨ï¼ç¶èå¾å¤æåçå¾®ä¿¡ï¼æ¯ä¸è½ç»å½ç½é¡µçå¾®ä¿¡çã
+ä½æ¯ä¹åè¿ä¸ªæºå¨äººï¼éè¦åºäºç½é¡µçæè½ç¨
+(æç½é¡µçå¾®ä¿¡çåå­¦ï¼è¿å¯ä»¥å»ç»§ç»­ç¨)ï¼ç¶èå¾å¤æåçå¾®ä¿¡ï¼æ¯ä¸è½ç»å½ç½é¡µçå¾®ä¿¡çã
 >
 ææ²¡æä¸ç§å¾®ä¿¡æºå¨äººï¼ä»»ä½äººçå¾®ä¿¡é½å¯ä»¥ç¨ï¼ä¸éè¦ç½é¡µå¾®ä¿¡åè½å¢ï¼
 å¨ç»è¿ææ¯æ£ç´¢åå¼åä»¥åï¼æ¯æææå¾®ä¿¡ä½¿ç¨çï¼**PyOfficeRobot**æ¥å¦~
-## 1ãå®è£PyOfficeRobot 1è¡å½ä»¤ï¼å®è£PyOfficeRobotè¿ä¸ªåº ``` pip
-install -i https://mirrors.aliyun.com/pypi/simple/ PyOfficeRobot -U ``` ##
+## 1ãå®è£PyOfficeRobot 1è¡å½ä»¤ï¼å®è£PyOfficeRobotè¿ä¸ªåºã
+[å®è£è§é¢](https://www.bilibili.com/video/BV1Xa411u7yU/) ``` pip install -
+i https://mirrors.aliyun.com/pypi/simple/ PyOfficeRobot -U ``` ##
 2ãè§é¢æç¨ - â­å¨å¥æºç ï¼[Github](https://github.com/CoderWanFeng/
 PyOfficeRobot) | åè½è¯´æ | è§é¢ |ä»£ç  | | -------------- | -------- |-
 ------- | | ð¥001-é¡¹ç®åå¸ | [ç¹æç´è¾¾](https://www.bilibili.com/
 video/BV1Xa411u7yU) |[ç¹æç´è¾¾](https://mp.weixin.qq.com/s/
 6slx8hyv_WuK7v5Nzt3XKQ) | | 002-èªå¨åæ¶æ¯ | [ç¹æç´è¾¾](https://
 www.bilibili.com/video/BV1Jt4y1j7F1) |[ç¹æç´è¾¾](https://github.com/
 CoderWanFeng/PyOfficeRobot/blob/main/demo/001-message.py) | | 003-
@@ -63,18 +65,21 @@
 HJfLZILUOWn4TK8qk3DL9w) | | âwxpy-24å°æ¶ï¼åå°è¿è¡ | [ç¹æç´è¾¾]
 (https://www.bilibili.com/video/BV11L411L7oi/) |[ç¹æç´è¾¾](https://
 mp.weixin.qq.com/s/ubJ1OhOFVKfFVT8sBNZ0pg) | | ä¼ä¸å¾®ä¿¡æºå¨äºº | |
 [ç¹æç´è¾¾](https://mp.weixin.qq.com/s/mt-ONvz0DdhbMB96eTZDKA) | ##
 3ãåè½Demo
 ææè¿å¼æºäºè¿ä¸ªåºçå¨é¨æºä»£ç ï¼åè½æ­£å¨å¼åä¸­ï¼æ¬¢è¿å¤§å®¶åä¸å¼å~
 - [æ¼ç¤ºä»£ç ](https://github.com/CoderWanFeng/PyOfficeRobot/tree/main/demo)
---- ![](https://python-office-1300615378.cos.ap-chongqing.myqcloud.com/python-
-office-qr.jpg) ## â­Star [![Stargazers over time](https://starchart.cc/
-CoderWanFeng/PyOfficeRobot.svg)](https://starchart.cc/CoderWanFeng/
-PyOfficeRobot) ## ðæå±èµæ
+## 4ãå¼åè | æµç§° | è´¡ç® | æ¶é´ | |---------|----------------------
+-|----------------| | é·æ° |
+è§£å³äºå¾®ä¿¡æ´æ°åï¼ä¸è½åéæ¶æ¯åæä»¶çé®é¢ | 2023/7/
+6 00ï¼30 | --- ![](https://python-office-1300615378.cos.ap-
+chongqing.myqcloud.com/python-office-qr.jpg) ## â­Star [![Stargazers over
+time](https://starchart.cc/CoderWanFeng/PyOfficeRobot.svg)](https://
+starchart.cc/CoderWanFeng/PyOfficeRobot) ## ðæå±èµæ
         [https://website-python-1300615378.cos.ap-nanjing.myqcloud.com/
         %E5%BC%95%E5%AF%BC%E8%B6%85%E9%93%BE%E6%8E%A5%2Fauto-work.jpg]
         [https://website-python-1300615378.cos.ap-nanjing.myqcloud.com/
           %E5%BC%95%E5%AF%BC%E8%B6%85%E9%93%BE%E6%8E%A5%2Febook.jpg]
         [https://website-python-1300615378.cos.ap-nanjing.myqcloud.com/
          %E5%BC%95%E5%AF%BC%E8%B6%85%E9%93%BE%E6%8E%A5%2Fproject.jpg]
         [https://website-python-1300615378.cos.ap-nanjing.myqcloud.com/
```

### Comparing `PyOfficeRobot-0.1.8/PyOfficeRobot/api/chat.py` & `PyOfficeRobot-0.1.9/PyOfficeRobot/api/chat.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,17 +18,17 @@
     :param who:
     :param message:
     :return:
     """
 
     # 获取会话列表
     wx.GetSessionList()
-    wx.ChatWith(who)  # 打开`文件传输助手`聊天窗口
+    wx.ChatWith(who)  # 打开`who`聊天窗口
     # for i in range(10):
-    wx.SendMsg(message)  # 向`文件传输助手`发送消息：你好~
+    wx.SendMsg(message,who)  # 向`who`发送消息：你好~
 
 
 @instruction
 def chat_by_keywords(who, keywords):
     wx.GetSessionList()  # 获取会话列表
     wx.ChatWith(who)  # 打开`who`聊天窗口
     temp_msg = ''
```

### Comparing `PyOfficeRobot-0.1.8/PyOfficeRobot/api/file.py` & `PyOfficeRobot-0.1.9/PyOfficeRobot/api/file.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,18 +9,17 @@
 def send_file(who, file):
     """
     发送任意类型的文件
     :param who:
     :param file: 文件路径
     :return:
     """
-    # 向某人发送文件（以`文件传输助手`为例，发送三个不同类型文件）
-    wx.ChatWith(who)  # 打开`文件传输助手`聊天窗口
-    # wx.SendFiles(file)  # 向`文件传输助手`发送上述三个文件
-    wx.test_SendFiles(filepath=file)  # 向`文件传输助手`发送上述三个文件
+    wx.ChatWith(who)  # 打开聊天窗口
+    # wx.SendFiles(file)
+    wx.test_SendFiles(filepath=file, who=who)  # 添加who参数：雷杰
 
     # 注：为保证发送文件稳定性，首次发送文件可能花费时间较长，后续调用会缩短发送时间
 
 
 import uiautomation as uia
 
 """ isinstance()函数知识点:
```

### Comparing `PyOfficeRobot-0.1.8/PyOfficeRobot/api/friend.py` & `PyOfficeRobot-0.1.9/PyOfficeRobot/api/friend.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from pywinauto.controls.uiawrapper import UIAWrapper
 from pywinauto.keyboard import send_keys
 from pywinauto.uia_element_info import UIAElementInfo
 
 from PyOfficeRobot.lib.decorator_utils.instruction_url import instruction
 
 
-def Carry_TXL(App_Object, Hello_Str, Tel_Number, notes):
+def _Carry_TXL(App_Object, Hello_Str, Tel_Number, notes):
     """
     该函数为申请好友验证时的函数胡\n
     :param App_Object: 微信窗口操作对象
     :param Hello_Str: 打招呼的字符串
     :param Tel_Number: 备注名,用于备注该用户的手机号码
     :param notes: 备注名
     :return: None
@@ -67,15 +67,15 @@
 
 
 def Get_NowTime():
     "【当前时间：%s-%s-%s-：%s:%s:%s】正在读取第%s行数据,该公司的联系电话有如下:\n【%s】"
     return time.strftime("%Y-%m-%d %H:%M:%S", time.localtime())
 
 
-def FindFriend(WX_Windows, Tel_Number, ErrorCount):
+def _find_friend(WX_Windows, Tel_Number, ErrorCount):
     """
     该函数用于在进入通讯录界面,输入手机号码一系列的操作\n
     :param WX_Windows: 微信窗口对象
     :param Tel_Number: 需要搜索的手机号码
     :param ErrorCount:
     :return:
     """
@@ -136,15 +136,15 @@
             print("\t\t %s提示:当前遍历号码[ %s ]已经是微信好友" % (Get_NowTime(), Tel_Number))
             print("\t\t %s提示:当前遍历号码[ %s ]已经是微信好友" % (Get_NowTime(), Tel_Number))
 
         return False
     # </editor-fold>
 
 
-def Open_TXL(Button_LT_Wrapper, Button_TXL_Wrapper, Button_SC_Wrapper, Button_EXE_Wrapper):
+def _Open_TXL(Button_LT_Wrapper, Button_TXL_Wrapper, Button_SC_Wrapper, Button_EXE_Wrapper):
     # <editor-fold desc="代码块 : 进入通讯录界面">
     """
     该函数为打开通讯录界面\n
     :return:
     """
     print("提示:当前正在进入通讯录界面")
     Button_SC_Wrapper.draw_outline(colour="red", thickness=5)
@@ -197,21 +197,21 @@
     Button_TXL_Wrapper = Button_TXL.wrapper_object()
     Button_SC_Wrapper = Button_SC.wrapper_object()
     Button_EXE_Wrapper = Button_EXE.wrapper_object()
 
     Count = 1
     # </editor-fold>
     for num in num_notes.keys():
-        Open_TXL(Button_LT_Wrapper, Button_TXL_Wrapper, Button_SC_Wrapper, Button_EXE_Wrapper)
-        result = FindFriend(WX_Windows=WX_Windows, Tel_Number=num, ErrorCount=Count)
-        Carry_TXL(App_Object=WX_Windows, Hello_Str=msg,
+        _Open_TXL(Button_LT_Wrapper, Button_TXL_Wrapper, Button_SC_Wrapper, Button_EXE_Wrapper)
+        result = _find_friend(WX_Windows=WX_Windows, Tel_Number=num, ErrorCount=Count)
+        _Carry_TXL(App_Object=WX_Windows, Hello_Str=msg,
                   Tel_Number=num, notes=num_notes[num])
 
 
 if __name__ == "__main__":
     msg = "你好，我是程序员晚枫，全网同名。"
     # num_list = ['15603052573', '19112440257']
     num_notes = {
-        # '15603052573': '北京-晚枫-学生',
-        '19112440257': '上海-晚枫-乞丐',
+        # 'CoderWanFeng': '北京-晚枫-学生',
+        'hdylw1024': '上海-晚枫-乞丐',
     }
     add(msg=msg, num_notes=num_notes)
```

### Comparing `PyOfficeRobot-0.1.8/PyOfficeRobot/api/group.py` & `PyOfficeRobot-0.1.9/PyOfficeRobot/api/group.py`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.8/PyOfficeRobot/core/WeChatType.py` & `PyOfficeRobot-0.1.9/PyOfficeRobot/core/WeChatType.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
         return Dict
 
 
 class WeChat:
     def __init__(self):
         self.UiaAPI = uia.WindowControl(ClassName='WeChatMainWndForPC')
         self.SessionList = self.UiaAPI.ListControl(Name='会话')
-        self.EditMsg = self.UiaAPI.EditControl(Name='输入')
+        # self.EditMsg = self.UiaAPI.EditControl(Name='编辑')
         self.SearchBox = self.UiaAPI.EditControl(Name='搜索')
         self.MsgList = self.UiaAPI.ListControl(Name='消息')
         self.SessionItemList = []
 
     def GetSessionList(self, reset=False):
         '''获取当前会话列表，更新会话列表'''
         self.SessionItem = self.SessionList.ListItemControl()
@@ -199,20 +199,21 @@
         rollresult = roll_to()
         if rollresult:
             return 1
         else:
             self.Search(who)
             return roll_to(RollTimes=1)
 
-    def SendMsg(self, msg, clear=True):
+    def SendMsg(self, msg, who, clear=True):
         '''向当前窗口发送消息
         msg : 要发送的消息
         clear : 是否清除当前已编辑内容
         '''
         self.UiaAPI.SwitchToThisWindow()
+        self.EditMsg = self.UiaAPI.EditControl(Name=who)
         if clear:
             self.EditMsg.SendKeys('{Ctrl}a', waitTime=0)
         self.EditMsg.SendKeys(msg, waitTime=0)
         self.EditMsg.SendKeys('{Enter}', waitTime=0)
 
     def SendFiles(self, *filepath, not_exists='ignore'):
         """向当前聊天窗口发送文件
@@ -254,17 +255,17 @@
             copydata = COPYDICT[i].replace(b'<EditElement type="0" pasteType="0"><![CDATA[ ]]></EditElement>',
                                            key.encode()).replace(b'type="0"', b'type="3"')
             wc.SetClipboardData(int(i), copydata)
         wc.CloseClipboard()
         self.SendClipboard()
         return 1
 
-    def SendClipboard(self):
+    def SendClipboard(self, who):
         '''向当前聊天页面发送剪贴板复制的内容'''
-        self.SendMsg('{Ctrl}v')
+        self.SendMsg('{Ctrl}v', who)
 
     @property
     def GetAllMessage(self):
         '''获取当前窗口中加载的所有聊天记录'''
         MsgDocker = []
         MsgItems = self.MsgList.GetChildren()
         for MsgItem in MsgItems:
@@ -302,15 +303,15 @@
 
     def SavePic(self, savepath=None, filename=None):
         WxUtils.SavePic()
         # Pic = uia.WindowControl(ClassName='ImagePreviewWnd', Name='图片查看')
 
     ################################微信发文件崩溃 https://blog.csdn.net/weixin_45081575/article/details/126810748
 
-    def test_SendFiles(self, filepath, not_exists='ignore'):
+    def test_SendFiles(self, filepath, who, not_exists='ignore'):
         """向当前聊天窗口发送文件
         not_exists: 如果未找到指定文件，继续或终止程序
         filepath: 要复制文件的绝对路径"""
         if not Path(filepath).exists():
             raise BaseException(f'你指定的文件不存在，请检查filepath后，重新运行：{filepath}')
 
         class DROPFILES(Structure):
@@ -345,9 +346,9 @@
         pDropFiles.fWide = True
         matedata = bytes(pDropFiles)
         filepath = str(Path(filepath).absolute())
         filename = [r"%s" % filepath]
         setClipboardFiles(filename)
 
         # wc.CloseClipboard()
-        self.SendClipboard()
+        self.SendClipboard(who)
         return 1
```

### Comparing `PyOfficeRobot-0.1.8/PyOfficeRobot/core/group/Start.py` & `PyOfficeRobot-0.1.9/PyOfficeRobot/core/group/Start.py`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.8/PyOfficeRobot/core/group/ui_file_py.py` & `PyOfficeRobot-0.1.9/PyOfficeRobot/core/group/ui_file_py.py`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.8/PyOfficeRobot/lib/decorator_utils/instruction_url.py` & `PyOfficeRobot-0.1.9/PyOfficeRobot/lib/decorator_utils/instruction_url.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         func_filename = os.path.basename(func.__code__.co_filename)  # 取出方法所在的文件名
         # 如果有这个文件，并且已经配置了方法名对应的说明链接，则打印出来
         if func_filename in instruction_file_dict.keys() and instruction_file_dict[func_filename][func.__name__]:
             print(SPLIT_LINE)
             print('【PyOfficeRobot，微信机器人全部功能】：https://www.python-office.com/office/robot.html')
             print(SPLIT_LINE)
             print(
-                f'正在运行：office.{os.path.basename(func_filename)[:-3]}.{func.__name__} , 这个方法的使用说明：{instruction_file_dict[func_filename][func.__name__]}')
+                f'正在运行：PyOfficeRobot.{os.path.basename(func_filename)[:-3]}.{func.__name__} , 这个方法的使用说明：{instruction_file_dict[func_filename][func.__name__]}')
             print(SPLIT_LINE)
         instruction_res = func(*args, **kwargs)
         return instruction_res
 
     return instruction_wrapper
```

### Comparing `PyOfficeRobot-0.1.8/PyOfficeRobot.egg-info/PKG-INFO` & `PyOfficeRobot-0.1.9/PyOfficeRobot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyOfficeRobot
-Version: 0.1.8
+Version: 0.1.9
 Summary: pip install PyOfficeRobot
 Home-page: https://www.python-office.com/office/robot.html
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/PyOfficeRobot/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/README.md
@@ -42,31 +42,29 @@
   </a>
 
 </p>
 
 
 
 
-
-
 # 又一个微信聊天机器人横空出世了，人人可用！
 
 
 之前给大家分享过一个微信机器人：[一个15分钟的视频，教你用Python创建自己的微信聊天机器人！](http://t.cn/A66p30bI)
 
-但是之前这个机器人，需要基于网页版才能用；然而很多朋友的微信，是不能登录网页版微信的。
+但是之前这个机器人，需要基于网页版才能用(有网页版微信的同学，还可以去继续用)；然而很多朋友的微信，是不能登录网页版微信的。
 
 > 有没有一种微信机器人，任何人的微信都可以用，不需要网页微信功能呢？
 
 
 在经过技术检索和开发以后，支持所有微信使用的：**PyOfficeRobot**来啦~
 
 ## 1、安装PyOfficeRobot
 
-1行命令，安装PyOfficeRobot这个库
+1行命令，安装PyOfficeRobot这个库。[安装视频](https://www.bilibili.com/video/BV1Xa411u7yU/)
 ```
 pip install -i https://mirrors.aliyun.com/pypi/simple/ PyOfficeRobot -U
 ```
 
 ## 2、视频教程
 
 - ⭐全套源码：[Github](https://github.com/CoderWanFeng/PyOfficeRobot)
@@ -103,14 +101,19 @@
 
 ## 3、功能Demo
 
 我最近开源了这个库的全部源代码，功能正在开发中，欢迎大家参与开发~
 
 - [演示代码](https://github.com/CoderWanFeng/PyOfficeRobot/tree/main/demo)
 
+## 4、开发者
+
+| 昵称      | 贡献                    | 时间             |
+|---------|-----------------------|----------------|
+| 雷杰 | 解决了微信更新后，不能发送消息和文件的问题 | 2023/7/6 00：30 |
 
 ---
 
 ![](https://python-office-1300615378.cos.ap-chongqing.myqcloud.com/python-office-qr.jpg)
 
 
 ## ⭐Star
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyOfficeRobot Version: 0.1.8 Summary: pip install
+Metadata-Version: 2.1 Name: PyOfficeRobot Version: 0.1.9 Summary: pip install
 PyOfficeRobot Home-page: https://www.python-office.com/office/robot.html
 Author: CoderWanFeng Author-email: 1957875073@qq.com License: MIT Project-URL:
 Bug Tracker, https://github.com/CoderWanFeng/PyOfficeRobot/issues Project-URL:
 Documentation, https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/
 README.md Project-URL: Source Code, https://github.com/CoderWanFeng/
 PyOfficeRobot Platform: any Requires-Python: >=3.6 Description-Content-Type:
 text/markdown License-File: LICENSE
@@ -13,20 +13,22 @@
 [github_star] [gitee_star] [https://img.shields.io/badge/QQ-163434413-orange]
  [https://img.shields.io/badge/%E5%BE%AE%E4%BF%A1-%E4%BA%A4%E6%B5%81%E7%BE%A4-
                                  brightgreen]
 # åä¸ä¸ªå¾®ä¿¡èå¤©æºå¨äººæ¨ªç©ºåºä¸äºï¼äººäººå¯ç¨ï¼
 ä¹åç»å¤§å®¶åäº«è¿ä¸ä¸ªå¾®ä¿¡æºå¨äººï¼
 [ä¸ä¸ª15åéçè§é¢ï¼æä½ ç¨Pythonåå»ºèªå·±çå¾®ä¿¡èå¤©æºå¨äººï¼]
 (http://t.cn/A66p30bI)
-ä½æ¯ä¹åè¿ä¸ªæºå¨äººï¼éè¦åºäºç½é¡µçæè½ç¨ï¼ç¶èå¾å¤æåçå¾®ä¿¡ï¼æ¯ä¸è½ç»å½ç½é¡µçå¾®ä¿¡çã
+ä½æ¯ä¹åè¿ä¸ªæºå¨äººï¼éè¦åºäºç½é¡µçæè½ç¨
+(æç½é¡µçå¾®ä¿¡çåå­¦ï¼è¿å¯ä»¥å»ç»§ç»­ç¨)ï¼ç¶èå¾å¤æåçå¾®ä¿¡ï¼æ¯ä¸è½ç»å½ç½é¡µçå¾®ä¿¡çã
 >
 ææ²¡æä¸ç§å¾®ä¿¡æºå¨äººï¼ä»»ä½äººçå¾®ä¿¡é½å¯ä»¥ç¨ï¼ä¸éè¦ç½é¡µå¾®ä¿¡åè½å¢ï¼
 å¨ç»è¿ææ¯æ£ç´¢åå¼åä»¥åï¼æ¯æææå¾®ä¿¡ä½¿ç¨çï¼**PyOfficeRobot**æ¥å¦~
-## 1ãå®è£PyOfficeRobot 1è¡å½ä»¤ï¼å®è£PyOfficeRobotè¿ä¸ªåº ``` pip
-install -i https://mirrors.aliyun.com/pypi/simple/ PyOfficeRobot -U ``` ##
+## 1ãå®è£PyOfficeRobot 1è¡å½ä»¤ï¼å®è£PyOfficeRobotè¿ä¸ªåºã
+[å®è£è§é¢](https://www.bilibili.com/video/BV1Xa411u7yU/) ``` pip install -
+i https://mirrors.aliyun.com/pypi/simple/ PyOfficeRobot -U ``` ##
 2ãè§é¢æç¨ - â­å¨å¥æºç ï¼[Github](https://github.com/CoderWanFeng/
 PyOfficeRobot) | åè½è¯´æ | è§é¢ |ä»£ç  | | -------------- | -------- |-
 ------- | | ð¥001-é¡¹ç®åå¸ | [ç¹æç´è¾¾](https://www.bilibili.com/
 video/BV1Xa411u7yU) |[ç¹æç´è¾¾](https://mp.weixin.qq.com/s/
 6slx8hyv_WuK7v5Nzt3XKQ) | | 002-èªå¨åæ¶æ¯ | [ç¹æç´è¾¾](https://
 www.bilibili.com/video/BV1Jt4y1j7F1) |[ç¹æç´è¾¾](https://github.com/
 CoderWanFeng/PyOfficeRobot/blob/main/demo/001-message.py) | | 003-
@@ -63,18 +65,21 @@
 HJfLZILUOWn4TK8qk3DL9w) | | âwxpy-24å°æ¶ï¼åå°è¿è¡ | [ç¹æç´è¾¾]
 (https://www.bilibili.com/video/BV11L411L7oi/) |[ç¹æç´è¾¾](https://
 mp.weixin.qq.com/s/ubJ1OhOFVKfFVT8sBNZ0pg) | | ä¼ä¸å¾®ä¿¡æºå¨äºº | |
 [ç¹æç´è¾¾](https://mp.weixin.qq.com/s/mt-ONvz0DdhbMB96eTZDKA) | ##
 3ãåè½Demo
 ææè¿å¼æºäºè¿ä¸ªåºçå¨é¨æºä»£ç ï¼åè½æ­£å¨å¼åä¸­ï¼æ¬¢è¿å¤§å®¶åä¸å¼å~
 - [æ¼ç¤ºä»£ç ](https://github.com/CoderWanFeng/PyOfficeRobot/tree/main/demo)
---- ![](https://python-office-1300615378.cos.ap-chongqing.myqcloud.com/python-
-office-qr.jpg) ## â­Star [![Stargazers over time](https://starchart.cc/
-CoderWanFeng/PyOfficeRobot.svg)](https://starchart.cc/CoderWanFeng/
-PyOfficeRobot) ## ðæå±èµæ
+## 4ãå¼åè | æµç§° | è´¡ç® | æ¶é´ | |---------|----------------------
+-|----------------| | é·æ° |
+è§£å³äºå¾®ä¿¡æ´æ°åï¼ä¸è½åéæ¶æ¯åæä»¶çé®é¢ | 2023/7/
+6 00ï¼30 | --- ![](https://python-office-1300615378.cos.ap-
+chongqing.myqcloud.com/python-office-qr.jpg) ## â­Star [![Stargazers over
+time](https://starchart.cc/CoderWanFeng/PyOfficeRobot.svg)](https://
+starchart.cc/CoderWanFeng/PyOfficeRobot) ## ðæå±èµæ
         [https://website-python-1300615378.cos.ap-nanjing.myqcloud.com/
         %E5%BC%95%E5%AF%BC%E8%B6%85%E9%93%BE%E6%8E%A5%2Fauto-work.jpg]
         [https://website-python-1300615378.cos.ap-nanjing.myqcloud.com/
           %E5%BC%95%E5%AF%BC%E8%B6%85%E9%93%BE%E6%8E%A5%2Febook.jpg]
         [https://website-python-1300615378.cos.ap-nanjing.myqcloud.com/
          %E5%BC%95%E5%AF%BC%E8%B6%85%E9%93%BE%E6%8E%A5%2Fproject.jpg]
         [https://website-python-1300615378.cos.ap-nanjing.myqcloud.com/
```

### Comparing `PyOfficeRobot-0.1.8/PyOfficeRobot.egg-info/SOURCES.txt` & `PyOfficeRobot-0.1.9/PyOfficeRobot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.8/README.md` & `PyOfficeRobot-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,31 +26,29 @@
   </a>
 
 </p>
 
 
 
 
-
-
 # 又一个微信聊天机器人横空出世了，人人可用！
 
 
 之前给大家分享过一个微信机器人：[一个15分钟的视频，教你用Python创建自己的微信聊天机器人！](http://t.cn/A66p30bI)
 
-但是之前这个机器人，需要基于网页版才能用；然而很多朋友的微信，是不能登录网页版微信的。
+但是之前这个机器人，需要基于网页版才能用(有网页版微信的同学，还可以去继续用)；然而很多朋友的微信，是不能登录网页版微信的。
 
 > 有没有一种微信机器人，任何人的微信都可以用，不需要网页微信功能呢？
 
 
 在经过技术检索和开发以后，支持所有微信使用的：**PyOfficeRobot**来啦~
 
 ## 1、安装PyOfficeRobot
 
-1行命令，安装PyOfficeRobot这个库
+1行命令，安装PyOfficeRobot这个库。[安装视频](https://www.bilibili.com/video/BV1Xa411u7yU/)
 ```
 pip install -i https://mirrors.aliyun.com/pypi/simple/ PyOfficeRobot -U
 ```
 
 ## 2、视频教程
 
 - ⭐全套源码：[Github](https://github.com/CoderWanFeng/PyOfficeRobot)
@@ -87,14 +85,19 @@
 
 ## 3、功能Demo
 
 我最近开源了这个库的全部源代码，功能正在开发中，欢迎大家参与开发~
 
 - [演示代码](https://github.com/CoderWanFeng/PyOfficeRobot/tree/main/demo)
 
+## 4、开发者
+
+| 昵称      | 贡献                    | 时间             |
+|---------|-----------------------|----------------|
+| 雷杰 | 解决了微信更新后，不能发送消息和文件的问题 | 2023/7/6 00：30 |
 
 ---
 
 ![](https://python-office-1300615378.cos.ap-chongqing.myqcloud.com/python-office-qr.jpg)
 
 
 ## ⭐Star
```

#### html2text {}

```diff
@@ -5,20 +5,22 @@
 [github_star] [gitee_star] [https://img.shields.io/badge/QQ-163434413-orange]
  [https://img.shields.io/badge/%E5%BE%AE%E4%BF%A1-%E4%BA%A4%E6%B5%81%E7%BE%A4-
                                  brightgreen]
 # åä¸ä¸ªå¾®ä¿¡èå¤©æºå¨äººæ¨ªç©ºåºä¸äºï¼äººäººå¯ç¨ï¼
 ä¹åç»å¤§å®¶åäº«è¿ä¸ä¸ªå¾®ä¿¡æºå¨äººï¼
 [ä¸ä¸ª15åéçè§é¢ï¼æä½ ç¨Pythonåå»ºèªå·±çå¾®ä¿¡èå¤©æºå¨äººï¼]
 (http://t.cn/A66p30bI)
-ä½æ¯ä¹åè¿ä¸ªæºå¨äººï¼éè¦åºäºç½é¡µçæè½ç¨ï¼ç¶èå¾å¤æåçå¾®ä¿¡ï¼æ¯ä¸è½ç»å½ç½é¡µçå¾®ä¿¡çã
+ä½æ¯ä¹åè¿ä¸ªæºå¨äººï¼éè¦åºäºç½é¡µçæè½ç¨
+(æç½é¡µçå¾®ä¿¡çåå­¦ï¼è¿å¯ä»¥å»ç»§ç»­ç¨)ï¼ç¶èå¾å¤æåçå¾®ä¿¡ï¼æ¯ä¸è½ç»å½ç½é¡µçå¾®ä¿¡çã
 >
 ææ²¡æä¸ç§å¾®ä¿¡æºå¨äººï¼ä»»ä½äººçå¾®ä¿¡é½å¯ä»¥ç¨ï¼ä¸éè¦ç½é¡µå¾®ä¿¡åè½å¢ï¼
 å¨ç»è¿ææ¯æ£ç´¢åå¼åä»¥åï¼æ¯æææå¾®ä¿¡ä½¿ç¨çï¼**PyOfficeRobot**æ¥å¦~
-## 1ãå®è£PyOfficeRobot 1è¡å½ä»¤ï¼å®è£PyOfficeRobotè¿ä¸ªåº ``` pip
-install -i https://mirrors.aliyun.com/pypi/simple/ PyOfficeRobot -U ``` ##
+## 1ãå®è£PyOfficeRobot 1è¡å½ä»¤ï¼å®è£PyOfficeRobotè¿ä¸ªåºã
+[å®è£è§é¢](https://www.bilibili.com/video/BV1Xa411u7yU/) ``` pip install -
+i https://mirrors.aliyun.com/pypi/simple/ PyOfficeRobot -U ``` ##
 2ãè§é¢æç¨ - â­å¨å¥æºç ï¼[Github](https://github.com/CoderWanFeng/
 PyOfficeRobot) | åè½è¯´æ | è§é¢ |ä»£ç  | | -------------- | -------- |-
 ------- | | ð¥001-é¡¹ç®åå¸ | [ç¹æç´è¾¾](https://www.bilibili.com/
 video/BV1Xa411u7yU) |[ç¹æç´è¾¾](https://mp.weixin.qq.com/s/
 6slx8hyv_WuK7v5Nzt3XKQ) | | 002-èªå¨åæ¶æ¯ | [ç¹æç´è¾¾](https://
 www.bilibili.com/video/BV1Jt4y1j7F1) |[ç¹æç´è¾¾](https://github.com/
 CoderWanFeng/PyOfficeRobot/blob/main/demo/001-message.py) | | 003-
@@ -55,18 +57,21 @@
 HJfLZILUOWn4TK8qk3DL9w) | | âwxpy-24å°æ¶ï¼åå°è¿è¡ | [ç¹æç´è¾¾]
 (https://www.bilibili.com/video/BV11L411L7oi/) |[ç¹æç´è¾¾](https://
 mp.weixin.qq.com/s/ubJ1OhOFVKfFVT8sBNZ0pg) | | ä¼ä¸å¾®ä¿¡æºå¨äºº | |
 [ç¹æç´è¾¾](https://mp.weixin.qq.com/s/mt-ONvz0DdhbMB96eTZDKA) | ##
 3ãåè½Demo
 ææè¿å¼æºäºè¿ä¸ªåºçå¨é¨æºä»£ç ï¼åè½æ­£å¨å¼åä¸­ï¼æ¬¢è¿å¤§å®¶åä¸å¼å~
 - [æ¼ç¤ºä»£ç ](https://github.com/CoderWanFeng/PyOfficeRobot/tree/main/demo)
---- ![](https://python-office-1300615378.cos.ap-chongqing.myqcloud.com/python-
-office-qr.jpg) ## â­Star [![Stargazers over time](https://starchart.cc/
-CoderWanFeng/PyOfficeRobot.svg)](https://starchart.cc/CoderWanFeng/
-PyOfficeRobot) ## ðæå±èµæ
+## 4ãå¼åè | æµç§° | è´¡ç® | æ¶é´ | |---------|----------------------
+-|----------------| | é·æ° |
+è§£å³äºå¾®ä¿¡æ´æ°åï¼ä¸è½åéæ¶æ¯åæä»¶çé®é¢ | 2023/7/
+6 00ï¼30 | --- ![](https://python-office-1300615378.cos.ap-
+chongqing.myqcloud.com/python-office-qr.jpg) ## â­Star [![Stargazers over
+time](https://starchart.cc/CoderWanFeng/PyOfficeRobot.svg)](https://
+starchart.cc/CoderWanFeng/PyOfficeRobot) ## ðæå±èµæ
         [https://website-python-1300615378.cos.ap-nanjing.myqcloud.com/
         %E5%BC%95%E5%AF%BC%E8%B6%85%E9%93%BE%E6%8E%A5%2Fauto-work.jpg]
         [https://website-python-1300615378.cos.ap-nanjing.myqcloud.com/
           %E5%BC%95%E5%AF%BC%E8%B6%85%E9%93%BE%E6%8E%A5%2Febook.jpg]
         [https://website-python-1300615378.cos.ap-nanjing.myqcloud.com/
          %E5%BC%95%E5%AF%BC%E8%B6%85%E9%93%BE%E6%8E%A5%2Fproject.jpg]
         [https://website-python-1300615378.cos.ap-nanjing.myqcloud.com/
```

### Comparing `PyOfficeRobot-0.1.8/setup.cfg` & `PyOfficeRobot-0.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2050 794f 6666 6963 6552 6f62 6f74   = PyOfficeRobot
 00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 312e  ..version = 0.1.
-00000030: 380d 0a64 6573 6372 6970 7469 6f6e 203d  8..description =
+00000030: 390d 0a64 6573 6372 6970 7469 6f6e 203d  9..description =
 00000040: 2070 6970 2069 6e73 7461 6c6c 2050 794f   pip install PyO
 00000050: 6666 6963 6552 6f62 6f74 0d0a 6c6f 6e67  fficeRobot..long
 00000060: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000070: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000080: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000090: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
 000000a0: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a75  text/markdown..u
```

### Comparing `PyOfficeRobot-0.1.8/tests/test_file.py` & `PyOfficeRobot-0.1.9/tests/test_file.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import unittest
 
 from PyOfficeRobot.api import file, group
-
 from PyOfficeRobot.api.chat import *
 from PyOfficeRobot.api.file import *
 
 keywords = {
     '你好': "在干嘛？"
 }
 
 
 class TestFile(unittest.TestCase):
     def test_send_file(self):
         send_file(who='文件传输助手', file=r'./test_files/0816.jpg')
 
     def test_chat_by_keyword(self):
-        chat_by_keywords(who='程序员晚枫', keywords=keywords)
+
+        chat_by_keywords(who='每天进步一点点', keywords=keywords)
 
     def test_receive_message(self):
         receive_message(who='程序员晚枫')
 
     def test_sm_by_time(self):
         send_message_by_time(who='每天进步一点点', message='你好', time='17:38')
```

