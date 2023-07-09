# Comparing `tmp/coolmongo-1.3.4.tar.gz` & `tmp/coolmongo-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolmongo-1.3.4.tar", last modified: Sun Jul  2 06:46:07 2023, max compression
+gzip compressed data, was "coolmongo-1.3.5.tar", last modified: Sun Jul  9 06:52:08 2023, max compression
```

## Comparing `coolmongo-1.3.4.tar` & `coolmongo-1.3.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 coolmongo-1.3.4/LICENSE
--rw-r--r--   0        0        0     4901 2023-07-02 06:08:05.248699 coolmongo-1.3.4/README.md
--rw-r--r--   0        0        0       29 2023-04-10 03:54:46.072863 coolmongo-1.3.4/coolmongo/__init__.py
--rw-r--r--   0        0        0    18005 2023-05-25 16:58:30.727299 coolmongo-1.3.4/coolmongo/docs/index.md
--rw-r--r--   0        0        0      595 2023-07-02 06:06:59.671803 coolmongo-1.3.4/pyproject.toml
--rw-r--r--   0        0        0     5187 1970-01-01 00:00:00.000000 coolmongo-1.3.4/PKG-INFO
+-rw-r--r--   0        0        0    10955 2023-07-09 05:47:26.656963 coolmongo-1.3.5/LICENSE
+-rw-r--r--   0        0        0     4606 2023-07-09 05:44:41.568778 coolmongo-1.3.5/README.md
+-rw-r--r--   0        0        0       29 2023-04-10 03:54:46.072863 coolmongo-1.3.5/coolmongo/__init__.py
+-rw-r--r--   0        0        0    18005 2023-05-25 16:58:30.727299 coolmongo-1.3.5/coolmongo/docs/index.md
+-rw-r--r--   0        0        0      597 2023-07-09 06:52:03.799347 coolmongo-1.3.5/pyproject.toml
+-rw-r--r--   0        0        0     4904 1970-01-01 00:00:00.000000 coolmongo-1.3.5/PKG-INFO
```

### Comparing `coolmongo-1.3.4/LICENSE` & `coolmongo-1.3.5/LICENSE`

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

### Comparing `coolmongo-1.3.4/README.md` & `coolmongo-1.3.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 
 安装：`pip install coolmongo`
 
 [教程](https://github.com/lcctoor/lccpy/blob/main/packages/coolmongo/coolmongo/docs/index.md)
 
 # Bug提交、功能提议
 
-您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg)、[技术交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) 与我联系。
+您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) 与我联系。
 
 # 关于作者
 
-作者：许灿标
+作者：lcctoor.com
 
 邮箱：lcctoor@outlook.com
 
-[主页](https://lcctoor.github.io/me/) | [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) | [Python技术交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg)
+[主页](https://lcctoor.github.io/me/) | [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) | [Python交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) | [捐赠](https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg)
 
 # 教程预览
 
 #### 导入
 
 ```python
 from pymongo import MongoClient
@@ -130,15 +130,7 @@
 
 | 代码             | 解释                                               |
 | ---------------- | -------------------------------------------------- |
 | mup.inc(1)       | 自增1                                              |
 | mup.inc(-1)      | 自减1                                              |
 | mup.add(1, 2, 3) | 向列表字段添加元素，仅当被添加的元素不存在时才添加 |
 | ...              | ...                                                |
-
-# 支持作者1元
-
-coolmongo 是一个免费的开源项目，由个人维护。
-
-每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
-
-<img src="https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg" width="200px">
```

### Comparing `coolmongo-1.3.4/coolmongo/docs/index.md` & `coolmongo-1.3.5/coolmongo/docs/index.md`

 * *Files identical despite different names*

### Comparing `coolmongo-1.3.4/pyproject.toml` & `coolmongo-1.3.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "coolmongo"
-version = "1.3.4"
+version = "1.3.5"
 description = "史上最优雅的 MongoDB ORM"
 dependencies = ["lccpy >=1.4.7.1"]
 keywords = ["coolmongo", "pymongo", "mongodb", "orm"]
 
 readme = "README.md"
-authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
+authors = [{name = "lcctoor.com", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
 
 [project.urls]
 HomePage = "https://github.com/lcctoor/lccpy/tree/main/packages/coolmongo#readme"
```

### Comparing `coolmongo-1.3.4/PKG-INFO` & `coolmongo-1.3.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: coolmongo
-Version: 1.3.4
+Version: 1.3.5
 Summary: 史上最优雅的 MongoDB ORM
 Keywords: coolmongo,pymongo,mongodb,orm
-Author-email: 许灿标 <lcctoor@outlook.com>
+Author-email: "lcctoor.com" <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: lccpy >=1.4.7.1
 Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/coolmongo#readme
 
 # 项目描述
@@ -18,23 +18,23 @@
 
 安装：`pip install coolmongo`
 
 [教程](https://github.com/lcctoor/lccpy/blob/main/packages/coolmongo/coolmongo/docs/index.md)
 
 # Bug提交、功能提议
 
-您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg)、[技术交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) 与我联系。
+您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) 与我联系。
 
 # 关于作者
 
-作者：许灿标
+作者：lcctoor.com
 
 邮箱：lcctoor@outlook.com
 
-[主页](https://lcctoor.github.io/me/) | [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) | [Python技术交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg)
+[主页](https://lcctoor.github.io/me/) | [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) | [Python交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) | [捐赠](https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg)
 
 # 教程预览
 
 #### 导入
 
 ```python
 from pymongo import MongoClient
@@ -143,15 +143,7 @@
 | 代码             | 解释                                               |
 | ---------------- | -------------------------------------------------- |
 | mup.inc(1)       | 自增1                                              |
 | mup.inc(-1)      | 自减1                                              |
 | mup.add(1, 2, 3) | 向列表字段添加元素，仅当被添加的元素不存在时才添加 |
 | ...              | ...                                                |
 
-# 支持作者1元
-
-coolmongo 是一个免费的开源项目，由个人维护。
-
-每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
-
-<img src="https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg" width="200px">
-
```

