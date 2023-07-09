# Comparing `tmp/coolapi-1.0.1.tar.gz` & `tmp/coolapi-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolapi-1.0.1.tar", last modified: Tue Jun 13 15:43:39 2023, max compression
+gzip compressed data, was "coolapi-1.0.2.tar", last modified: Sun Jul  9 06:51:13 2023, max compression
```

## Comparing `coolapi-1.0.1.tar` & `coolapi-1.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 coolapi-1.0.1/LICENSE
--rw-r--r--   0        0        0     5330 2023-06-13 15:29:36.475109 coolapi-1.0.1/README.md
--rw-r--r--   0        0        0       27 2023-06-12 17:15:32.722578 coolapi-1.0.1/coolapi.py
--rw-r--r--   0        0        0      619 2023-06-13 15:43:29.448879 coolapi-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     5601 1970-01-01 00:00:00.000000 coolapi-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-07-09 05:47:26.657966 coolapi-1.0.2/LICENSE
+-rw-r--r--   0        0        0     4726 2023-07-09 05:44:41.573781 coolapi-1.0.2/README.md
+-rw-r--r--   0        0        0       27 2023-06-12 17:15:32.722578 coolapi-1.0.2/coolapi.py
+-rw-r--r--   0        0        0      621 2023-07-09 06:51:05.798923 coolapi-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5011 1970-01-01 00:00:00.000000 coolapi-1.0.2/PKG-INFO
```

### Comparing `coolapi-1.0.1/LICENSE` & `coolapi-1.0.2/LICENSE`

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

### Comparing `coolapi-1.0.1/README.md` & `coolapi-1.0.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -6,25 +6,23 @@
 
 ```
 pip install coolapi
 ```
 
 # Bug提交、功能提议
 
-您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR-max.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/lccpy/WechatReadersGroupQR-original.jpg) 与我联系。
+您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) 与我联系。
 
 # 关于作者
 
-作者：许灿标
+作者：lcctoor.com
 
 邮箱：lcctoor@outlook.com
 
-[主页](https://github.com/lcctoor/me#readme) | [微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR-max.jpg) | [微信公众号](https://raw.githubusercontent.com/lcctoor/me/main/author/WechatSubscribeQRAndSearch-max.png) | [Python技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/lccpy/WechatReadersGroupQR-original.jpg)
-
-开源项目：[让Python更简单一点](https://github.com/lcctoor/lccpy#readme)
+[主页](https://lcctoor.github.io/me/) | [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) | [Python交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) | [捐赠](https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg)
 
 # 教程
 
 #### 导入
 
 ```python
 import asyncio
@@ -160,15 +158,7 @@
 #### 更多用法
 
 coolapi 是对 tornado 的二次封装，其中：
 
 1、coolapi.handler（视图类）继承自 [tornado.web.RequestHandler](https://www.tornadoweb.org/en/stable/web.html#request-handlers)，可使用 tornado.web.RequestHandler 的任何功能。
 
 2、creat_server 支持 [tornado.web.Application](https://www.tornadoweb.org/en/stable/web.html#tornado.web.Application) 的所有参数。
-
-# 支持作者1元
-
-coolapi 是一个免费的开源项目，由个人维护。
-
-每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
-
-<img src="https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR-1rmb-max.jpg" width="200px">
```

### Comparing `coolapi-1.0.1/pyproject.toml` & `coolapi-1.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "coolapi"
-version = "1.0.1"
+version = "1.0.2"
 description = "简单好用的异步 web 框架"
 dependencies = ["lccpy >=1.4.7"]
 keywords = ["coolapi", "tornado", "flask", "fastapi", "django", "aiohttp", "web"]
 
 readme = "README.md"
-authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
+authors = [{name = "lcctoor.com", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
 
 [project.urls]
 HomePage = "https://github.com/lcctoor/lccpy/tree/main/packages/coolapi#readme"
```

### Comparing `coolapi-1.0.1/PKG-INFO` & `coolapi-1.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: coolapi
-Version: 1.0.1
+Version: 1.0.2
 Summary: 简单好用的异步 web 框架
 Keywords: coolapi,tornado,flask,fastapi,django,aiohttp,web
-Author-email: 许灿标 <lcctoor@outlook.com>
+Author-email: "lcctoor.com" <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: lccpy >=1.4.7
 Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/coolapi#readme
 
 # 项目描述
@@ -18,25 +18,23 @@
 
 ```
 pip install coolapi
 ```
 
 # Bug提交、功能提议
 
-您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR-max.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/lccpy/WechatReadersGroupQR-original.jpg) 与我联系。
+您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) 与我联系。
 
 # 关于作者
 
-作者：许灿标
+作者：lcctoor.com
 
 邮箱：lcctoor@outlook.com
 
-[主页](https://github.com/lcctoor/me#readme) | [微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR-max.jpg) | [微信公众号](https://raw.githubusercontent.com/lcctoor/me/main/author/WechatSubscribeQRAndSearch-max.png) | [Python技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/lccpy/WechatReadersGroupQR-original.jpg)
-
-开源项目：[让Python更简单一点](https://github.com/lcctoor/lccpy#readme)
+[主页](https://lcctoor.github.io/me/) | [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) | [Python交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) | [捐赠](https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg)
 
 # 教程
 
 #### 导入
 
 ```python
 import asyncio
@@ -173,15 +171,7 @@
 
 coolapi 是对 tornado 的二次封装，其中：
 
 1、coolapi.handler（视图类）继承自 [tornado.web.RequestHandler](https://www.tornadoweb.org/en/stable/web.html#request-handlers)，可使用 tornado.web.RequestHandler 的任何功能。
 
 2、creat_server 支持 [tornado.web.Application](https://www.tornadoweb.org/en/stable/web.html#tornado.web.Application) 的所有参数。
 
-# 支持作者1元
-
-coolapi 是一个免费的开源项目，由个人维护。
-
-每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
-
-<img src="https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR-1rmb-max.jpg" width="200px">
-
```

