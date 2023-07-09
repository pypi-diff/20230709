# Comparing `tmp/rstyleslice-1.4.3.tar.gz` & `tmp/rstyleslice-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rstyleslice-1.4.3.tar", last modified: Sun Jul  2 06:46:41 2023, max compression
+gzip compressed data, was "rstyleslice-1.4.4.tar", last modified: Sun Jul  9 06:54:50 2023, max compression
```

## Comparing `rstyleslice-1.4.3.tar` & `rstyleslice-1.4.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 rstyleslice-1.4.3/LICENSE
--rw-r--r--   0        0        0     3213 2023-07-02 06:31:37.593584 rstyleslice-1.4.3/README.md
--rw-r--r--   0        0        0      593 2023-07-02 06:29:08.610326 rstyleslice-1.4.3/pyproject.toml
--rw-r--r--   0        0        0       31 2023-04-10 04:03:01.139197 rstyleslice-1.4.3/rstyleslice/__init__.py
--rw-r--r--   0        0        0     5794 2023-04-25 13:10:59.200573 rstyleslice-1.4.3/rstyleslice/docs/index.md
--rw-r--r--   0        0        0     3550 1970-01-01 00:00:00.000000 rstyleslice-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-07-09 05:47:26.599959 rstyleslice-1.4.4/LICENSE
+-rw-r--r--   0        0        0     2916 2023-07-09 05:44:41.558583 rstyleslice-1.4.4/README.md
+-rw-r--r--   0        0        0      595 2023-07-09 06:54:44.459762 rstyleslice-1.4.4/pyproject.toml
+-rw-r--r--   0        0        0       31 2023-04-10 04:03:01.139197 rstyleslice-1.4.4/rstyleslice/__init__.py
+-rw-r--r--   0        0        0     5794 2023-04-25 13:10:59.200573 rstyleslice-1.4.4/rstyleslice/docs/index.md
+-rw-r--r--   0        0        0     3265 1970-01-01 00:00:00.000000 rstyleslice-1.4.4/PKG-INFO
```

### Comparing `rstyleslice-1.4.3/LICENSE` & `rstyleslice-1.4.4/LICENSE`

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

### Comparing `rstyleslice-1.4.3/README.md` & `rstyleslice-1.4.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 
 安装：`pip install rstyleslice`
 
 [教程](https://github.com/lcctoor/lccpy/blob/main/packages/rstyleslice/rstyleslice/docs/index.md)
 
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
 from rstyleslice import rslice
@@ -83,15 +83,7 @@
 obj[:]
 # >>> [111, 2, 3, 1, 2, 3, 4, 5]
 
 obj[4:100] = ['1', 2, 3, 4, 5]
 obj[:]
 # >>> [111, 2, 3, '1', 2, 3, 4, 5]
 ```
-
-# 支持作者1元
-
-rstyleslice 是一个免费的开源项目，由个人维护。
-
-每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
-
-<img src="https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg" width="200px">
```

### Comparing `rstyleslice-1.4.3/pyproject.toml` & `rstyleslice-1.4.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "rstyleslice"
-version = "1.4.3"
+version = "1.4.4"
 description = "一套符合直觉的索引和切片语法"
 dependencies = ["lccpy >=1.4.7.1"]
 keywords = ["rstyleslice", "slice"]
 
 readme = "README.md"
-authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
+authors = [{name = "lcctoor.com", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
 
 [project.urls]
 HomePage = "https://github.com/lcctoor/lccpy/tree/main/packages/rstyleslice#readme"
```

### Comparing `rstyleslice-1.4.3/rstyleslice/docs/index.md` & `rstyleslice-1.4.4/rstyleslice/docs/index.md`

 * *Files identical despite different names*

### Comparing `rstyleslice-1.4.3/PKG-INFO` & `rstyleslice-1.4.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: rstyleslice
-Version: 1.4.3
+Version: 1.4.4
 Summary: 一套符合直觉的索引和切片语法
 Keywords: rstyleslice,slice
-Author-email: 许灿标 <lcctoor@outlook.com>
+Author-email: "lcctoor.com" <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: lccpy >=1.4.7.1
 Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/rstyleslice#readme
 
 # 项目描述
@@ -26,23 +26,23 @@
 
 安装：`pip install rstyleslice`
 
 [教程](https://github.com/lcctoor/lccpy/blob/main/packages/rstyleslice/rstyleslice/docs/index.md)
 
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
 from rstyleslice import rslice
@@ -96,15 +96,7 @@
 # >>> [111, 2, 3, 1, 2, 3, 4, 5]
 
 obj[4:100] = ['1', 2, 3, 4, 5]
 obj[:]
 # >>> [111, 2, 3, '1', 2, 3, 4, 5]
 ```
 
-# 支持作者1元
-
-rstyleslice 是一个免费的开源项目，由个人维护。
-
-每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
-
-<img src="https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg" width="200px">
-
```

