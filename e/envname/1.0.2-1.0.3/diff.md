# Comparing `tmp/envname-1.0.2.tar.gz` & `tmp/envname-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "envname-1.0.2.tar", last modified: Tue Jun 13 15:50:35 2023, max compression
+gzip compressed data, was "envname-1.0.3.tar", last modified: Sun Jul  9 06:53:28 2023, max compression
```

## Comparing `envname-1.0.2.tar` & `envname-1.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 envname-1.0.2/LICENSE
--rw-r--r--   0        0        0     2137 2023-06-13 15:29:36.474108 envname-1.0.2/README.md
--rw-r--r--   0        0        0      645 2023-05-01 16:30:31.499496 envname-1.0.2/envname/__init__.py
--rw-r--r--   0        0        0      102 2023-05-01 17:24:53.385434 envname-1.0.2/envname/_envname.py
--rw-r--r--   0        0        0      583 2023-06-13 15:50:31.479672 envname-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2421 1970-01-01 00:00:00.000000 envname-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-07-09 05:47:26.637967 envname-1.0.3/LICENSE
+-rw-r--r--   0        0        0     1533 2023-07-09 05:44:41.566784 envname-1.0.3/README.md
+-rw-r--r--   0        0        0      647 2023-07-09 05:47:26.638963 envname-1.0.3/envname/__init__.py
+-rw-r--r--   0        0        0      102 2023-05-01 17:24:53.385434 envname-1.0.3/envname/_envname.py
+-rw-r--r--   0        0        0      585 2023-07-09 06:53:23.550155 envname-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1831 1970-01-01 00:00:00.000000 envname-1.0.3/PKG-INFO
```

### Comparing `envname-1.0.2/LICENSE` & `envname-1.0.3/LICENSE`

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

### Comparing `envname-1.0.2/README.md` & `envname-1.0.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -8,25 +8,23 @@
 
 ```
 pip install envname
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
 
 #### 创建环境名称
 
 （cmd）：
 
@@ -65,15 +63,7 @@
 if envname == 'aliyun_HongKong_No1':
     host = '192.168.0.127'
 else:
     host = '112.47.203.101'
 
 conn = pymysql.connect(host=host, port=3306, user='root', password='123456789')
 ```
-
-# 支持作者1元
-
-envname 是一个免费的开源项目，由个人维护。
-
-每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
-
-<img src="https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR-1rmb-max.jpg" width="200px">
```

### Comparing `envname-1.0.2/envname/__init__.py` & `envname-1.0.3/envname/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright [2023] [许灿标]
+Copyright [2023] [lcctoor.com]
 license: Apache License, Version 2.0
 email: lcctoor@outlook.com
 '''
 
 import sys
 from pathlib import Path
```

### Comparing `envname-1.0.2/pyproject.toml` & `envname-1.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "envname"
-version = "1.0.2"
+version = "1.0.3"
 description = "为运行环境设置名称"
 dependencies = []
 keywords = []
 
 readme = "README.md"
-authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
+authors = [{name = "lcctoor.com", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
 
 [project.scripts]
 envname = "envname:_parsecmd"
```

### Comparing `envname-1.0.2/PKG-INFO` & `envname-1.0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: envname
-Version: 1.0.2
+Version: 1.0.3
 Summary: 为运行环境设置名称
 Keywords: 
-Author-email: 许灿标 <lcctoor@outlook.com>
+Author-email: "lcctoor.com" <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/envname#readme
 
 # 项目描述
 
@@ -19,25 +19,23 @@
 
 ```
 pip install envname
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
 
 #### 创建环境名称
 
 （cmd）：
 
@@ -77,15 +75,7 @@
     host = '192.168.0.127'
 else:
     host = '112.47.203.101'
 
 conn = pymysql.connect(host=host, port=3306, user='root', password='123456789')
 ```
 
-# 支持作者1元
-
-envname 是一个免费的开源项目，由个人维护。
-
-每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
-
-<img src="https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR-1rmb-max.jpg" width="200px">
-
```

