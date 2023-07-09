# Comparing `tmp/openai2-1.5.8.tar.gz` & `tmp/openai2-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai2-1.5.8.tar", last modified: Sat Jun 24 14:47:15 2023, max compression
+gzip compressed data, was "openai2-1.5.9.tar", last modified: Sun Jul  9 06:54:30 2023, max compression
```

## Comparing `openai2-1.5.8.tar` & `openai2-1.5.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    10953 2023-03-07 16:01:05.491907 openai2-1.5.8/LICENSE
--rw-r--r--   0        0        0     3090 2023-06-23 03:29:02.608130 openai2-1.5.8/README.md
--rw-r--r--   0        0        0     1083 2020-12-22 18:45:03.000000 openai2-1.5.8/openai2/Dependent Packages/openai/LICENSE
--rw-r--r--   0        0        0       23 2023-05-28 06:12:32.856591 openai2-1.5.8/openai2/__init__.py
--rw-r--r--   0        0        0     2576 2023-05-28 05:05:03.581780 openai2-1.5.8/openai2/_core.py
--rw-r--r--   0        0        0      637 2023-06-24 14:46:37.857272 openai2-1.5.8/pyproject.toml
--rw-r--r--   0        0        0     3456 1970-01-01 00:00:00.000000 openai2-1.5.8/PKG-INFO
+-rw-r--r--   0        0        0    10955 2023-07-09 05:47:26.599959 openai2-1.5.9/LICENSE
+-rw-r--r--   0        0        0     2892 2023-07-09 06:43:46.227787 openai2-1.5.9/README.md
+-rw-r--r--   0        0        0     1083 2020-12-22 18:45:03.000000 openai2-1.5.9/openai2/Dependent Packages/openai/LICENSE
+-rw-r--r--   0        0        0       23 2023-05-28 06:12:32.856591 openai2-1.5.9/openai2/__init__.py
+-rw-r--r--   0        0        0     2578 2023-07-09 05:47:26.599959 openai2-1.5.9/openai2/_core.py
+-rw-r--r--   0        0        0      639 2023-07-09 06:54:25.759703 openai2-1.5.9/pyproject.toml
+-rw-r--r--   0        0        0     3264 1970-01-01 00:00:00.000000 openai2-1.5.9/PKG-INFO
```

### Comparing `openai2-1.5.8/LICENSE` & `openai2-1.5.9/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
       defend, and hold each Contributor harmless for any liability
       incurred by, or claims asserted against, such Contributor by reason
       of your accepting any such warranty or additional liability.
 
    END OF TERMS AND CONDITIONS
    
 
-   Copyright [2023] [许灿标]
+   Copyright [2023] [lcctoor.com]
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `openai2-1.5.8/README.md` & `openai2-1.5.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,22 @@
 
 # 获取api_key
 
 [获取链接1](https://platform.openai.com/account/api-keys)
 
 [获取链接2](https://www.baidu.com/s?wd=%E8%8E%B7%E5%8F%96%20openai%20api_key)
 
+# 关于作者
+
+作者：lcctoor.com
+
+邮箱：lcctoor@outlook.com
+
+[主页](https://lcctoor.github.io/me/) | [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) | [Python交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) | [捐赠](https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg)
+
 # 教程
 
 #### 导入
 
 ```python
 from openai2 import Chat
 ```
@@ -95,18 +103,8 @@
 
 #### 更多方法
 
 openai2.Chat 底层调用了 [openai.ChatCompletion.create](https://platform.openai.com/docs/api-reference/chat/create?lang=python)，在实例化时，支持 openai.ChatCompletion.create 的所有参数，例如：`Chat(api_key=api_key, model="gpt-3.5-turbo", max_tokens=100)` 。
 
 # Bug提交、功能提议
 
-您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg)、[技术交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) 与我联系。
-
-# 关于作者
-
-作者：许灿标
-
-邮箱：lcctoor@outlook.com
-
-[主页](https://lcctoor.github.io/me/) | [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) | [微信公众号](https://lcctoor.github.io/me/author/WechatSubscribeQRAndSearch-max.png) | [Python技术交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg)
-
-开源项目：[让Python更简单一点](https://github.com/lcctoor/lccpy#readme)
+您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) 与我联系。
```

### Comparing `openai2-1.5.8/openai2/Dependent Packages/openai/LICENSE` & `openai2-1.5.9/openai2/Dependent Packages/openai/LICENSE`

 * *Files identical despite different names*

### Comparing `openai2-1.5.8/openai2/_core.py` & `openai2-1.5.9/openai2/_core.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright [2023] [许灿标]
+Copyright [2023] [lcctoor.com]
 license: Apache License, Version 2.0
 email: lcctoor@outlook.com
 '''
 
 from json import dumps as jsonDumps
 from json import loads as jsonLoads
 from pathlib import Path
```

### Comparing `openai2-1.5.8/PKG-INFO` & `openai2-1.5.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: openai2
-Version: 1.5.8
+Version: 1.5.9
 Summary: 根据 openai 官方接口 ‘openai’ 改造的 ‘openai2’ ，比官方接口更好用一点
 Keywords: openai2,openai
-Author-email: 许灿标 <lcctoor@outlook.com>
+Author-email: "lcctoor.com" <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: openai >=0.27.0
 Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/openai2#readme
 
 # 项目描述
@@ -22,14 +22,22 @@
 
 # 获取api_key
 
 [获取链接1](https://platform.openai.com/account/api-keys)
 
 [获取链接2](https://www.baidu.com/s?wd=%E8%8E%B7%E5%8F%96%20openai%20api_key)
 
+# 关于作者
+
+作者：lcctoor.com
+
+邮箱：lcctoor@outlook.com
+
+[主页](https://lcctoor.github.io/me/) | [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) | [Python交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) | [捐赠](https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg)
+
 # 教程
 
 #### 导入
 
 ```python
 from openai2 import Chat
 ```
@@ -107,19 +115,9 @@
 
 #### 更多方法
 
 openai2.Chat 底层调用了 [openai.ChatCompletion.create](https://platform.openai.com/docs/api-reference/chat/create?lang=python)，在实例化时，支持 openai.ChatCompletion.create 的所有参数，例如：`Chat(api_key=api_key, model="gpt-3.5-turbo", max_tokens=100)` 。
 
 # Bug提交、功能提议
 
-您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg)、[技术交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) 与我联系。
-
-# 关于作者
-
-作者：许灿标
-
-邮箱：lcctoor@outlook.com
-
-[主页](https://lcctoor.github.io/me/) | [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) | [微信公众号](https://lcctoor.github.io/me/author/WechatSubscribeQRAndSearch-max.png) | [Python技术交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg)
-
-开源项目：[让Python更简单一点](https://github.com/lcctoor/lccpy#readme)
+您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) 与我联系。
```

