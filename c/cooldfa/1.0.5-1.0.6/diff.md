# Comparing `tmp/cooldfa-1.0.5.tar.gz` & `tmp/cooldfa-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cooldfa-1.0.5.tar", last modified: Tue Jun 13 15:47:02 2023, max compression
+gzip compressed data, was "cooldfa-1.0.6.tar", last modified: Sun Jul  9 06:51:37 2023, max compression
```

## Comparing `cooldfa-1.0.5.tar` & `cooldfa-1.0.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 cooldfa-1.0.5/LICENSE
--rw-r--r--   0        0        0     2118 2023-06-13 15:29:36.475109 cooldfa-1.0.5/README.md
--rw-r--r--   0        0        0       39 2023-04-03 14:28:11.266714 cooldfa-1.0.5/cooldfa/__init__.py
--rw-r--r--   0        0        0     3661 2023-04-30 01:06:28.124524 cooldfa-1.0.5/cooldfa/_cooldfa.py
--rw-r--r--   0        0        0   478756 2023-04-30 19:24:41.305728 cooldfa-1.0.5/cooldfa/_words/others.json
--rw-r--r--   0        0        0    23188 2023-04-30 19:24:41.308762 cooldfa-1.0.5/cooldfa/_words/politics.json
--rw-r--r--   0        0        0    10325 2023-04-30 19:24:41.311777 cooldfa-1.0.5/cooldfa/_words/sex.json
--rw-r--r--   0        0        0   262857 2023-04-30 19:24:41.330728 cooldfa-1.0.5/cooldfa/_words/url.json
--rw-r--r--   0        0        0     4015 2023-04-30 19:24:41.331729 cooldfa-1.0.5/cooldfa/_words/violence.json
--rw-r--r--   0        0        0      559 2023-06-13 15:46:56.960978 cooldfa-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     2423 1970-01-01 00:00:00.000000 cooldfa-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-07-09 05:47:26.657966 cooldfa-1.0.6/LICENSE
+-rw-r--r--   0        0        0     1514 2023-07-09 05:44:41.573781 cooldfa-1.0.6/README.md
+-rw-r--r--   0        0        0       39 2023-04-03 14:28:11.266714 cooldfa-1.0.6/cooldfa/__init__.py
+-rw-r--r--   0        0        0     3663 2023-07-09 05:47:26.657966 cooldfa-1.0.6/cooldfa/_cooldfa.py
+-rw-r--r--   0        0        0   478756 2023-04-30 19:24:41.305728 cooldfa-1.0.6/cooldfa/_words/others.json
+-rw-r--r--   0        0        0    23188 2023-04-30 19:24:41.308762 cooldfa-1.0.6/cooldfa/_words/politics.json
+-rw-r--r--   0        0        0    10325 2023-04-30 19:24:41.311777 cooldfa-1.0.6/cooldfa/_words/sex.json
+-rw-r--r--   0        0        0   262857 2023-04-30 19:24:41.330728 cooldfa-1.0.6/cooldfa/_words/url.json
+-rw-r--r--   0        0        0     4015 2023-04-30 19:24:41.331729 cooldfa-1.0.6/cooldfa/_words/violence.json
+-rw-r--r--   0        0        0      561 2023-07-09 06:51:29.375709 cooldfa-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1833 1970-01-01 00:00:00.000000 cooldfa-1.0.6/PKG-INFO
```

### Comparing `cooldfa-1.0.5/LICENSE` & `cooldfa-1.0.6/LICENSE`

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

### Comparing `cooldfa-1.0.5/README.md` & `cooldfa-1.0.6/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -6,25 +6,23 @@
 
 ```
 pip install cooldfa
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
 from cooldfa import dfa
@@ -67,15 +65,7 @@
     preset_words.politics,  # 政治类
     preset_words.sex,  # 色情类
     preset_words.violence,  # 暴力类
     preset_words.url,  # 网址
     preset_words.others,  # 其它
 )
 ```
-
-# 支持作者1元
-
-cooldfa 是一个免费的开源项目，由个人维护。
-
-每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
-
-<img src="https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR-1rmb-max.jpg" width="200px">
```

### Comparing `cooldfa-1.0.5/cooldfa/_cooldfa.py` & `cooldfa-1.0.6/cooldfa/_cooldfa.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright [2023] [许灿标]
+Copyright [2023] [lcctoor.com]
 license: Apache License, Version 2.0
 email: lcctoor@outlook.com
 '''
 
 from copy import deepcopy
 from json import loads
 from pathlib import Path
```

### Comparing `cooldfa-1.0.5/cooldfa/_words/others.json` & `cooldfa-1.0.6/cooldfa/_words/others.json`

 * *Files identical despite different names*

### Comparing `cooldfa-1.0.5/cooldfa/_words/politics.json` & `cooldfa-1.0.6/cooldfa/_words/politics.json`

 * *Files identical despite different names*

### Comparing `cooldfa-1.0.5/cooldfa/_words/sex.json` & `cooldfa-1.0.6/cooldfa/_words/sex.json`

 * *Files identical despite different names*

### Comparing `cooldfa-1.0.5/cooldfa/_words/url.json` & `cooldfa-1.0.6/cooldfa/_words/url.json`

 * *Files identical despite different names*

### Comparing `cooldfa-1.0.5/cooldfa/_words/violence.json` & `cooldfa-1.0.6/cooldfa/_words/violence.json`

 * *Files identical despite different names*

### Comparing `cooldfa-1.0.5/pyproject.toml` & `cooldfa-1.0.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "cooldfa"
-version = "1.0.5"
+version = "1.0.6"
 description = "基于 DFA 算法的敏感词检测器"
 dependencies = []
 keywords = ["cooldfa", "dfa"]
 
 readme = "README.md"
-authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
+authors = [{name = "lcctoor.com", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.10"
 
 [project.urls]
 HomePage = "https://github.com/lcctoor/lccpy/tree/main/packages/cooldfa#readme"
```

### Comparing `cooldfa-1.0.5/PKG-INFO` & `cooldfa-1.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cooldfa
-Version: 1.0.5
+Version: 1.0.6
 Summary: 基于 DFA 算法的敏感词检测器
 Keywords: cooldfa,dfa
-Author-email: 许灿标 <lcctoor@outlook.com>
+Author-email: "lcctoor.com" <lcctoor@outlook.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/cooldfa#readme
 
 # 项目描述
 
@@ -17,25 +17,23 @@
 
 ```
 pip install cooldfa
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
 from cooldfa import dfa
@@ -79,15 +77,7 @@
     preset_words.sex,  # 色情类
     preset_words.violence,  # 暴力类
     preset_words.url,  # 网址
     preset_words.others,  # 其它
 )
 ```
 
-# 支持作者1元
-
-cooldfa 是一个免费的开源项目，由个人维护。
-
-每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
-
-<img src="https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR-1rmb-max.jpg" width="200px">
-
```

