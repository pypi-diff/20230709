# Comparing `tmp/cooltime-1.0.tar.gz` & `tmp/cooltime-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cooltime-1.0.tar", last modified: Sun Jun 25 12:28:56 2023, max compression
+gzip compressed data, was "cooltime-1.0.1.tar", last modified: Sun Jul  9 06:52:50 2023, max compression
```

## Comparing `cooltime-1.0.tar` & `cooltime-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 cooltime-1.0/LICENSE
--rw-r--r--   0        0        0     3869 2023-06-25 11:59:24.697569 cooltime-1.0/README.md
--rw-r--r--   0        0        0       28 2023-06-25 08:04:00.811074 cooltime-1.0/cooltime.py
--rw-r--r--   0        0        0      555 2023-06-25 12:28:48.503755 cooltime-1.0/pyproject.toml
--rw-r--r--   0        0        0     4162 1970-01-01 00:00:00.000000 cooltime-1.0/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-07-09 05:47:26.656963 cooltime-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3511 2023-07-09 05:44:41.566784 cooltime-1.0.1/README.md
+-rw-r--r--   0        0        0       28 2023-06-25 08:04:00.811074 cooltime-1.0.1/cooltime.py
+-rw-r--r--   0        0        0      559 2023-07-09 06:52:44.343597 cooltime-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3818 1970-01-01 00:00:00.000000 cooltime-1.0.1/PKG-INFO
```

### Comparing `cooltime-1.0/LICENSE` & `cooltime-1.0.1/LICENSE`

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

### Comparing `cooltime-1.0/README.md` & `cooltime-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,106 +1,111 @@
-# 项目描述
-
-人性化的时间模块。
-
-# 安装
-
-```
-pip install cooltime
-```
-
-# Bug提交、功能提议
-
-您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg)、[技术交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) 与我联系。
-
-# 关于作者
-
-作者：许灿标
-
-邮箱：lcctoor@outlook.com
-
-[主页](https://lcctoor.github.io/me/) | [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) | [Python技术交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg)
-
-# 教程
-
-#### 导入
-
-```python
-from cooltime import cooltime
-```
-
-#### 生成时间
-
-```python
-t1 = cooltime()  # 生成1个当前时间
-t2 = cooltime.random()  # 生成1个随机时间
-t3 = cooltime(1687271066.000028)  # 从时间戳生成, 精确到毫秒
-t4 = cooltime(1687271066)  # 从时间戳生成, 精确到秒
-t5 = cooltime(t3)  # 从 cooltime 生成
-t6 = cooltime('2023-06-20 22:24:26.000028')  # 从字符串生成, 精确到毫秒
-t7 = cooltime('2023-06-20 22:24:26')  # 从字符串生成, 精确到秒
-t8 = cooltime('2023-06-20 22:24')  # 从字符串生成, 精确到分
-t9 = cooltime('2023-06-20 22')  # 从字符串生成, 精确到时
-t10 = cooltime('2023-06-20')  # 从字符串生成, 精确到日
-t11 = cooltime([2023, 6, 20, 22, 24, 26, 28])  # 从其它类型生成, 如: list, tuple, datetime, time.localtime ……
-```
-
-注：
-
-1、从字符串生成时，生成器会执行 `re.findall('\d+', text)[:7]` 提取前 7 个数字串来生成时间。因此字符串的格式可为任意，比如：`2023/06/20/22/24/26/000028` 、`2023_06_20_22_24_26_000028` 。
-
-2、从 时间戳、cooltime、字符串 以外的其它类型生成时，生成器会先执行 `str(obj)` 将对象转化成字符串，然后按处理字符串的方式生成。
-
-#### 将时间转化为其它类型
-
-| 语法                             | 返回                         | 描述                         |
-| -------------------------------- | ---------------------------- | ---------------------------- |
-| int( t3 )                        | 1687271066                   | 转化为时间戳，精确到秒       |
-| float( t3 )                      | 1687271066.000028            | 转化为时间戳，精确到毫秒     |
-| t3.date( )                       | '2023-06-20'                 | 提取日期字符串               |
-| str( t3 )                        | '2023-06-20 22:24:26.000028' | 转化为时间字符串，精确到毫秒 |
-| t3.floor( )                      | '2023-06-20 22:24:26'        | 转化为时间字符串，精确到秒   |
-| t3.strftime("%Y-%m-%d %H:%M:%S") | '2023-06-20 22:24:26'        | 按指定格式转化为时间字符串   |
-| t3.strftime("%Y_%m_%d %H_%M_%S") | '2023_06_20 22_24_26'        | 按指定格式转化为时间字符串   |
-
-#### 比较时间大小
-
-```python
-# == 号
-assert t3 == t5 == t6 == t11
-assert t4 == t7
-
-# > 号
-assert t6 > t7 > t8 > t9 > t10
-
-# < 号
-assert t10 < t9 < t8 < t7 < t6
-
-# >= 号
-assert t3 >= t5 >= t6 >= t11
-assert t4 >= t7
-assert t6 >= t7 >= t8 >= t9 >= t10
-
-# <= 号
-assert t3 <= t5 <= t6 <= t11
-assert t4 <= t7
-assert t10 <= t9 <= t8 <= t7 <= t6
-```
-
-#### 时间的增量操作
-
-```python
-t26 = cooltime('2023-06-20 22:24:26')
-t23 = t26 - 3  # 增量单位为秒
-t29 = t26 + 3
-print(t23)  # 2023-06-20 22:24:23
-print(t29)  # 2023-06-20 22:24:29
-print(t23 < t26 < t29)  # True
-```
-
-# 支持作者1元
-
-cooltime 是一个免费的开源项目，由个人维护。
-
-每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
-
-<img src="https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg" width="200px">
+Metadata-Version: 2.1
+Name: cooltime
+Version: 1.0.1
+Summary: 人性化的时间模块
+Keywords: cooltime
+Author-email: "lcctoor.com" <lcctoor@outlook.com>
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Dist: lccpy >=1.4.7.1
+Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/cooltime#readme
+
+# 项目描述
+
+人性化的时间模块。
+
+# 安装
+
+```
+pip install cooltime
+```
+
+# Bug提交、功能提议
+
+您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) 与我联系。
+
+# 关于作者
+
+作者：lcctoor.com
+
+邮箱：lcctoor@outlook.com
+
+[主页](https://lcctoor.github.io/me/) | [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) | [Python交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) | [捐赠](https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg)
+
+# 教程
+
+#### 导入
+
+```python
+from cooltime import cooltime
+```
+
+#### 生成时间
+
+```python
+t1 = cooltime()  # 生成1个当前时间
+t2 = cooltime.random()  # 生成1个随机时间
+t3 = cooltime(1687271066.000028)  # 从时间戳生成
+t4 = cooltime(1687271066)  # 从时间戳生成, 精确到秒
+t5 = cooltime(t3)  # 从 cooltime 生成
+t6 = cooltime('2023-06-20 22:24:26.000028')  # 从字符串生成
+t7 = cooltime('2023-06-20 22:24:26')  # 从字符串生成, 精确到秒
+t8 = cooltime('2023-06-20 22:24')  # 从字符串生成, 精确到分
+t9 = cooltime('2023-06-20 22')  # 从字符串生成, 精确到时
+t10 = cooltime('2023-06-20')  # 从字符串生成, 精确到日
+t11 = cooltime([2023, 6, 20, 22, 24, 26, 28])  # 从其它类型生成, 如: list, tuple, datetime, time.localtime ……
+```
+
+注：
+
+1、从字符串生成时，生成器会执行 `re.findall('\d+', text)[:7]` 提取前 7 个数字串来生成时间。因此字符串的格式可为任意，比如：`2023/06/20/22/24/26/000028` 、`2023_06_20_22_24_26_000028` 。
+
+2、从 时间戳、cooltime、字符串 以外的其它类型生成时，生成器会先执行 `str(obj)` 将对象转化成字符串，然后按处理字符串的方式生成。
+
+#### 将时间转化为其它类型
+
+| 语法                             | 返回                         | 描述                       |
+| -------------------------------- | ---------------------------- | -------------------------- |
+| float( t3 )                      | 1687271066.000028            | 转化为时间戳               |
+| int( t3 )                        | 1687271066                   | 转化为时间戳，精确到秒     |
+| t3.date( )                       | '2023-06-20'                 | 提取日期字符串             |
+| str( t3 )                        | '2023-06-20 22:24:26.000028' | 转化为时间字符串           |
+| t3.floor( )                      | '2023-06-20 22:24:26'        | 转化为时间字符串，精确到秒 |
+| t3.strftime("%Y-%m-%d %H:%M:%S") | '2023-06-20 22:24:26'        | 按指定格式转化为时间字符串 |
+| t3.strftime("%Y_%m_%d %H_%M_%S") | '2023_06_20 22_24_26'        | 按指定格式转化为时间字符串 |
+
+#### 比较时间大小
+
+```python
+# == 号
+assert t3 == t5 == t6 == t11
+assert t4 == t7
+
+# > 号
+assert t6 > t7 > t8 > t9 > t10
+
+# < 号
+assert t10 < t9 < t8 < t7 < t6
+
+# >= 号
+assert t3 >= t5 >= t6 >= t11
+assert t4 >= t7
+assert t6 >= t7 >= t8 >= t9 >= t10
+
+# <= 号
+assert t3 <= t5 <= t6 <= t11
+assert t4 <= t7
+assert t10 <= t9 <= t8 <= t7 <= t6
+```
+
+#### 时间的增量操作
+
+```python
+t26 = cooltime('2023-06-20 22:24:26')
+t23 = t26 - 3  # 增量单位为秒
+t29 = t26 + 3
+print(t23)  # 2023-06-20 22:24:23
+print(t29)  # 2023-06-20 22:24:29
+print(t23 < t26 < t29)  # True
+```
+
```

