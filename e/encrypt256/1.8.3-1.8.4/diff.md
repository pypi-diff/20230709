# Comparing `tmp/encrypt256-1.8.3.tar.gz` & `tmp/encrypt256-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encrypt256-1.8.3.tar", last modified: Tue Jun 13 15:50:01 2023, max compression
+gzip compressed data, was "encrypt256-1.8.4.tar", last modified: Sun Jul  9 06:53:09 2023, max compression
```

## Comparing `encrypt256-1.8.3.tar` & `encrypt256-1.8.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    10951 2023-02-14 11:47:56.900367 encrypt256-1.8.3/LICENSE
--rw-r--r--   0        0        0     2491 2023-06-13 15:29:36.475109 encrypt256-1.8.3/README.md
--rw-r--r--   0        0        0       30 2023-04-10 04:00:30.884575 encrypt256-1.8.3/encrypt256.py
--rw-r--r--   0        0        0      616 2023-06-13 15:49:57.671735 encrypt256-1.8.3/pyproject.toml
--rw-r--r--   0        0        0     2854 1970-01-01 00:00:00.000000 encrypt256-1.8.3/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-07-09 05:47:26.656963 encrypt256-1.8.4/LICENSE
+-rw-r--r--   0        0        0     1884 2023-07-09 05:44:41.563781 encrypt256-1.8.4/README.md
+-rw-r--r--   0        0        0       30 2023-04-10 04:00:30.884575 encrypt256-1.8.4/encrypt256.py
+-rw-r--r--   0        0        0      618 2023-07-09 06:53:05.135943 encrypt256-1.8.4/pyproject.toml
+-rw-r--r--   0        0        0     2261 1970-01-01 00:00:00.000000 encrypt256-1.8.4/PKG-INFO
```

### Comparing `encrypt256-1.8.3/LICENSE` & `encrypt256-1.8.4/LICENSE`

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

### Comparing `encrypt256-1.8.3/README.md` & `encrypt256-1.8.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -12,25 +12,23 @@
 
 ```
 pip install encrypt256
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
 from encrypt256 import Encrypt256
@@ -71,15 +69,7 @@
 当发生以下情况时，会解密失败并报错：
 
 1、密钥错误。
 
 2、由于密文被篡改，导致 AES 算法解密失败。
 
 3、由于密文被篡改，虽然 AES 算法解密成功，但校验值错误。
-
-# 支持作者1元
-
-encrypt256 是一个免费的开源项目，由个人维护。
-
-每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
-
-<img src="https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR-1rmb-max.jpg" width="200px">
```

### Comparing `encrypt256-1.8.3/pyproject.toml` & `encrypt256-1.8.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "encrypt256"
-version = "1.8.3"
+version = "1.8.4"
 description = "str 型和 bytes 型数据加密器"
 dependencies = ["lccpy >=1.4.7"]
 keywords = ["encrypt256", "encrypt", "AES", "pycryptodome", "Crypto"]
 
 readme = "README.md"
-authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
+authors = [{name = "lcctoor.com", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
 
 [project.urls]
 HomePage = "https://github.com/lcctoor/lccpy/tree/main/packages/encrypt256#readme"
```

### Comparing `encrypt256-1.8.3/PKG-INFO` & `encrypt256-1.8.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: encrypt256
-Version: 1.8.3
+Version: 1.8.4
 Summary: str 型和 bytes 型数据加密器
 Keywords: encrypt256,encrypt,AES,pycryptodome,Crypto
-Author-email: 许灿标 <lcctoor@outlook.com>
+Author-email: "lcctoor.com" <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: lccpy >=1.4.7
 Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/encrypt256#readme
 
 # 项目描述
@@ -24,25 +24,23 @@
 
 ```
 pip install encrypt256
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
 from encrypt256 import Encrypt256
@@ -84,15 +82,7 @@
 
 1、密钥错误。
 
 2、由于密文被篡改，导致 AES 算法解密失败。
 
 3、由于密文被篡改，虽然 AES 算法解密成功，但校验值错误。
 
-# 支持作者1元
-
-encrypt256 是一个免费的开源项目，由个人维护。
-
-每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
-
-<img src="https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR-1rmb-max.jpg" width="200px">
-
```

