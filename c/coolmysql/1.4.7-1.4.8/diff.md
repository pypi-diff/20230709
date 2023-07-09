# Comparing `tmp/coolmysql-1.4.7.tar.gz` & `tmp/coolmysql-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolmysql-1.4.7.tar", last modified: Sun Jul  2 06:46:18 2023, max compression
+gzip compressed data, was "coolmysql-1.4.8.tar", last modified: Sun Jul  9 06:52:29 2023, max compression
```

## Comparing `coolmysql-1.4.7.tar` & `coolmysql-1.4.8.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 coolmysql-1.4.7/LICENSE
--rw-r--r--   0        0        0     4128 2023-07-02 06:09:23.077760 coolmysql-1.4.7/README.md
--rw-r--r--   0        0        0       29 2023-04-10 03:59:45.387315 coolmysql-1.4.7/coolmysql/__init__.py
--rw-r--r--   0        0        0    18748 2023-06-14 09:13:53.682433 coolmysql-1.4.7/coolmysql/docs/index.md
--rw-r--r--   0        0        0      603 2023-07-02 06:08:34.041733 coolmysql-1.4.7/pyproject.toml
--rw-r--r--   0        0        0     4417 1970-01-01 00:00:00.000000 coolmysql-1.4.7/PKG-INFO
+-rw-r--r--   0        0        0    10955 2023-07-09 05:47:26.656963 coolmysql-1.4.8/LICENSE
+-rw-r--r--   0        0        0     3833 2023-07-09 05:44:41.571802 coolmysql-1.4.8/README.md
+-rw-r--r--   0        0        0     1070 2013-11-27 14:43:24.000000 coolmysql-1.4.8/coolmysql/Dependent Packages/pymysql/LICENSE
+-rw-r--r--   0        0        0       86 2023-06-13 11:57:21.279654 coolmysql-1.4.8/coolmysql/__init__.py
+-rw-r--r--   0        0        0    23082 2023-07-09 06:02:16.006639 coolmysql-1.4.8/coolmysql/_core.py
+-rw-r--r--   0        0        0    18748 2023-06-14 09:13:53.682433 coolmysql-1.4.8/coolmysql/docs/index.md
+-rw-r--r--   0        0        0      597 2023-07-09 06:52:25.076919 coolmysql-1.4.8/pyproject.toml
+-rw-r--r--   0        0        0     4126 1970-01-01 00:00:00.000000 coolmysql-1.4.8/PKG-INFO
```

### Comparing `coolmysql-1.4.7/LICENSE` & `coolmysql-1.4.8/LICENSE`

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

### Comparing `coolmysql-1.4.7/README.md` & `coolmysql-1.4.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 
 安装：`pip install coolmysql`
 
 [教程](https://github.com/lcctoor/lccpy/blob/main/packages/coolmysql/coolmysql/docs/index.md)
 
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
 from pymysql import connect
@@ -132,15 +132,7 @@
 data
 # >>> [{'姓名': '小一'}]
 
 data, cursor = sheet.execute('update 希望小学 set 爱好="Python" limit 3')
 cursor.rowcount
 # >>> 3
 ```
-
-# 支持作者1元
-
-coolmysql 是一个免费的开源项目，由个人维护。
-
-每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
-
-<img src="https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg" width="200px">
```

### Comparing `coolmysql-1.4.7/coolmysql/docs/index.md` & `coolmysql-1.4.8/coolmysql/docs/index.md`

 * *Files identical despite different names*

### Comparing `coolmysql-1.4.7/pyproject.toml` & `coolmysql-1.4.8/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "coolmysql"
-version = "1.4.7"
+version = "1.4.8"
 description = "史上最优雅的 mysql ORM"
-dependencies = ["lccpy >=1.4.7.1"]
+dependencies = ["pymysql"]
 keywords = ["coolmysql", "pymysql", "mysql", "aiomysql", "orm"]
 
 readme = "README.md"
-authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
+authors = [{name = "lcctoor.com", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
 
 [project.urls]
 HomePage = "https://github.com/lcctoor/lccpy/tree/main/packages/coolmysql#readme"
```

### Comparing `coolmysql-1.4.7/PKG-INFO` & `coolmysql-1.4.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: coolmysql
-Version: 1.4.7
+Version: 1.4.8
 Summary: 史上最优雅的 mysql ORM
 Keywords: coolmysql,pymysql,mysql,aiomysql,orm
-Author-email: 许灿标 <lcctoor@outlook.com>
+Author-email: "lcctoor.com" <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: lccpy >=1.4.7.1
+Requires-Dist: pymysql
 Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/coolmysql#readme
 
 # 项目描述
 
 史上最优雅的 mysql ORM 。
 
 # 安装与教程
 
 安装：`pip install coolmysql`
 
 [教程](https://github.com/lcctoor/lccpy/blob/main/packages/coolmysql/coolmysql/docs/index.md)
 
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
 from pymysql import connect
@@ -145,15 +145,7 @@
 # >>> [{'姓名': '小一'}]
 
 data, cursor = sheet.execute('update 希望小学 set 爱好="Python" limit 3')
 cursor.rowcount
 # >>> 3
 ```
 
-# 支持作者1元
-
-coolmysql 是一个免费的开源项目，由个人维护。
-
-每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
-
-<img src="https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg" width="200px">
-
```

