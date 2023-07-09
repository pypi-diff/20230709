# Comparing `tmp/ns_asphalt9-0.0.9.tar.gz` & `tmp/ns_asphalt9-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ns_asphalt9-0.0.9.tar", last modified: Thu Jul  6 11:44:14 2023, max compression
+gzip compressed data, was "dist/ns_asphalt9-0.1.0.tar", last modified: Sun Jul  9 05:11:24 2023, max compression
```

## Comparing `ns_asphalt9-0.0.9.tar` & `ns_asphalt9-0.1.0.tar`

### file list

```diff
@@ -1,50 +1,48 @@
-drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-07-06 11:44:14.631823 ns_asphalt9-0.0.9/
--rw-r--r--   0 neo.sun    (502) staff       (20)    35149 2023-04-10 06:16:35.000000 ns_asphalt9-0.0.9/LICENSE
--rw-r--r--   0 neo.sun    (502) staff       (20)      180 2023-06-30 07:35:13.000000 ns_asphalt9-0.0.9/MANIFEST.in
--rw-r--r--   0 neo.sun    (502) staff       (20)     2020 2023-07-06 11:44:14.631929 ns_asphalt9-0.0.9/PKG-INFO
--rw-r--r--   0 neo.sun    (502) staff       (20)     1041 2023-05-04 03:01:57.000000 ns_asphalt9-0.0.9/README.md
-drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-07-06 11:44:14.621548 ns_asphalt9-0.0.9/ns_asphalt9/
-drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-07-06 11:44:14.625921 ns_asphalt9-0.0.9/ns_asphalt9/core/
--rw-r--r--   0 neo.sun    (502) staff       (20)       20 2023-06-30 07:48:40.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/__init__.py
-drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-07-06 11:44:14.627311 ns_asphalt9-0.0.9/ns_asphalt9/core/actions/
--rw-r--r--   0 neo.sun    (502) staff       (20)      222 2023-07-03 09:32:26.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/actions/__init__.py
--rw-r--r--   0 neo.sun    (502) staff       (20)      477 2023-07-03 09:32:06.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/actions/common.py
--rw-r--r--   0 neo.sun    (502) staff       (20)     4033 2023-07-03 02:07:26.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/actions/enter_page.py
--rw-r--r--   0 neo.sun    (502) staff       (20)     3917 2023-07-03 02:07:26.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/actions/process_race.py
--rw-r--r--   0 neo.sun    (502) staff       (20)     3777 2023-07-03 02:07:26.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/actions/select_car.py
--rw-r--r--   0 neo.sun    (502) staff       (20)      706 2023-06-28 08:30:50.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/cache.py
--rw-r--r--   0 neo.sun    (502) staff       (20)     3037 2023-07-03 02:10:16.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/consts.py
--rw-r--r--   0 neo.sun    (502) staff       (20)     2146 2023-06-30 07:54:21.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/controller.py
--rw-r--r--   0 neo.sun    (502) staff       (20)      634 2023-07-03 02:07:26.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/globals.py
-drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-07-06 11:44:14.627622 ns_asphalt9-0.0.9/ns_asphalt9/core/gui/
--rw-r--r--   0 neo.sun    (502) staff       (20)        0 2023-06-26 05:07:57.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/gui/__init__.py
--rw-r--r--   0 neo.sun    (502) staff       (20)    18706 2023-07-03 02:07:26.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/gui/app.py
-drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-07-06 11:44:14.629697 ns_asphalt9-0.0.9/ns_asphalt9/core/gui/images/
--rw-r--r--   0 neo.sun    (502) staff       (20)     3097 2023-06-26 08:14:33.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/gui/images/help.png
--rw-r--r--   0 neo.sun    (502) staff       (20)     2900 2023-06-26 08:18:26.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/gui/images/home.png
--rw-r--r--   0 neo.sun    (502) staff       (20)   202347 2023-06-26 05:17:10.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/gui/images/logo.png
--rw-r--r--   0 neo.sun    (502) staff       (20)     3159 2023-06-26 08:11:35.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/gui/images/settings.png
--rw-r--r--   0 neo.sun    (502) staff       (20)     1530 2023-06-30 07:54:36.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/ocr.py
--rw-r--r--   0 neo.sun    (502) staff       (20)     1841 2023-07-03 02:07:26.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/page_factory.py
--rw-r--r--   0 neo.sun    (502) staff       (20)    13007 2023-07-06 11:42:30.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/pages.py
--rw-r--r--   0 neo.sun    (502) staff       (20)      265 2023-06-29 06:50:43.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/screenshot.py
--rw-r--r--   0 neo.sun    (502) staff       (20)     2572 2023-07-03 02:07:26.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/tasks.py
-drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-07-06 11:44:14.631293 ns_asphalt9-0.0.9/ns_asphalt9/core/utils/
--rw-r--r--   0 neo.sun    (502) staff       (20)        0 2023-06-25 08:40:05.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/utils/__init__.py
--rw-r--r--   0 neo.sun    (502) staff       (20)     1016 2023-06-30 07:53:42.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/utils/decorator.py
--rw-r--r--   0 neo.sun    (502) staff       (20)      459 2023-06-25 08:40:05.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/utils/fetch_cars.py
--rw-r--r--   0 neo.sun    (502) staff       (20)     1993 2023-06-30 07:53:54.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/utils/log.py
--rw-r--r--   0 neo.sun    (502) staff       (20)      862 2023-06-30 07:54:03.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/utils/timer.py
--rw-r--r--   0 neo.sun    (502) staff       (20)     5558 2023-07-03 02:07:26.000000 ns_asphalt9-0.0.9/ns_asphalt9/main.py
-drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-07-06 11:44:14.622895 ns_asphalt9-0.0.9/ns_asphalt9.egg-info/
--rw-r--r--   0 neo.sun    (502) staff       (20)     2020 2023-07-06 11:44:14.000000 ns_asphalt9-0.0.9/ns_asphalt9.egg-info/PKG-INFO
--rw-r--r--   0 neo.sun    (502) staff       (20)     1187 2023-07-06 11:44:14.000000 ns_asphalt9-0.0.9/ns_asphalt9.egg-info/SOURCES.txt
--rw-r--r--   0 neo.sun    (502) staff       (20)        1 2023-07-06 11:44:14.000000 ns_asphalt9-0.0.9/ns_asphalt9.egg-info/dependency_links.txt
--rw-r--r--   0 neo.sun    (502) staff       (20)       54 2023-07-06 11:44:14.000000 ns_asphalt9-0.0.9/ns_asphalt9.egg-info/entry_points.txt
--rw-r--r--   0 neo.sun    (502) staff       (20)        1 2023-06-30 07:09:01.000000 ns_asphalt9-0.0.9/ns_asphalt9.egg-info/not-zip-safe
--rw-r--r--   0 neo.sun    (502) staff       (20)      107 2023-07-06 11:44:14.000000 ns_asphalt9-0.0.9/ns_asphalt9.egg-info/requires.txt
--rw-r--r--   0 neo.sun    (502) staff       (20)       12 2023-07-06 11:44:14.000000 ns_asphalt9-0.0.9/ns_asphalt9.egg-info/top_level.txt
--rw-r--r--   0 neo.sun    (502) staff       (20)     1299 2023-07-06 11:44:14.632329 ns_asphalt9-0.0.9/setup.cfg
--rw-r--r--   0 neo.sun    (502) staff       (20)      387 2023-06-30 03:30:00.000000 ns_asphalt9-0.0.9/setup.py
-drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-07-06 11:44:14.631577 ns_asphalt9-0.0.9/tests/
--rw-r--r--   0 neo.sun    (502) staff       (20)     1204 2023-06-29 06:52:40.000000 ns_asphalt9-0.0.9/tests/test_ocr.py
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-09 05:11:24.000000 ns_asphalt9-0.1.0/
+-rw-r--r--   0 sunhao     (501) staff       (20)    35149 2023-04-09 01:28:45.000000 ns_asphalt9-0.1.0/LICENSE
+-rw-r--r--   0 sunhao     (501) staff       (20)      180 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.0/MANIFEST.in
+-rw-r--r--   0 sunhao     (501) staff       (20)     2276 2023-07-09 05:11:24.000000 ns_asphalt9-0.1.0/PKG-INFO
+-rw-r--r--   0 sunhao     (501) staff       (20)     1041 2023-05-15 13:28:06.000000 ns_asphalt9-0.1.0/README.md
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-09 05:11:24.000000 ns_asphalt9-0.1.0/ns_asphalt9/
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-09 05:11:24.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/
+-rw-r--r--   0 sunhao     (501) staff       (20)       20 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/__init__.py
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-09 05:11:24.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/actions/
+-rw-r--r--   0 sunhao     (501) staff       (20)      244 2023-07-09 03:22:53.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/actions/__init__.py
+-rw-r--r--   0 sunhao     (501) staff       (20)      477 2023-07-09 03:17:56.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/actions/common.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     4539 2023-07-09 03:22:39.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/actions/enter_page.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     3917 2023-07-02 12:56:49.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/actions/process_race.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     3777 2023-07-02 02:37:32.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/actions/select_car.py
+-rw-r--r--   0 sunhao     (501) staff       (20)      706 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/cache.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     3072 2023-07-09 03:21:21.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/consts.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     2146 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/controller.py
+-rw-r--r--   0 sunhao     (501) staff       (20)      634 2023-07-02 02:35:24.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/globals.py
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-09 05:11:24.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/gui/
+-rw-r--r--   0 sunhao     (501) staff       (20)        0 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/gui/__init__.py
+-rw-r--r--   0 sunhao     (501) staff       (20)    21684 2023-07-09 03:40:27.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/gui/app.py
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-09 05:11:24.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/gui/images/
+-rw-r--r--   0 sunhao     (501) staff       (20)     3097 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/gui/images/help.png
+-rw-r--r--   0 sunhao     (501) staff       (20)     2900 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/gui/images/home.png
+-rw-r--r--   0 sunhao     (501) staff       (20)   202347 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/gui/images/logo.png
+-rw-r--r--   0 sunhao     (501) staff       (20)     3159 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/gui/images/settings.png
+-rw-r--r--   0 sunhao     (501) staff       (20)     1530 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/ocr.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     1841 2023-07-01 12:06:18.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/page_factory.py
+-rw-r--r--   0 sunhao     (501) staff       (20)    13348 2023-07-09 04:52:32.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/pages.py
+-rw-r--r--   0 sunhao     (501) staff       (20)      265 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/screenshot.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     2728 2023-07-09 04:10:27.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/tasks.py
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-09 05:11:24.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/utils/
+-rw-r--r--   0 sunhao     (501) staff       (20)        0 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/utils/__init__.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     1016 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/utils/decorator.py
+-rw-r--r--   0 sunhao     (501) staff       (20)      459 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/utils/fetch_cars.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     1993 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/utils/log.py
+-rw-r--r--   0 sunhao     (501) staff       (20)      862 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/utils/timer.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     5558 2023-07-02 12:12:57.000000 ns_asphalt9-0.1.0/ns_asphalt9/main.py
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-09 05:11:24.000000 ns_asphalt9-0.1.0/ns_asphalt9.egg-info/
+-rw-r--r--   0 sunhao     (501) staff       (20)     2276 2023-07-09 05:11:24.000000 ns_asphalt9-0.1.0/ns_asphalt9.egg-info/PKG-INFO
+-rw-r--r--   0 sunhao     (501) staff       (20)     1169 2023-07-09 05:11:24.000000 ns_asphalt9-0.1.0/ns_asphalt9.egg-info/SOURCES.txt
+-rw-r--r--   0 sunhao     (501) staff       (20)        1 2023-07-09 05:11:24.000000 ns_asphalt9-0.1.0/ns_asphalt9.egg-info/dependency_links.txt
+-rw-r--r--   0 sunhao     (501) staff       (20)       55 2023-07-09 05:11:24.000000 ns_asphalt9-0.1.0/ns_asphalt9.egg-info/entry_points.txt
+-rw-r--r--   0 sunhao     (501) staff       (20)        1 2023-07-02 12:38:46.000000 ns_asphalt9-0.1.0/ns_asphalt9.egg-info/not-zip-safe
+-rw-r--r--   0 sunhao     (501) staff       (20)      107 2023-07-09 05:11:24.000000 ns_asphalt9-0.1.0/ns_asphalt9.egg-info/requires.txt
+-rw-r--r--   0 sunhao     (501) staff       (20)       12 2023-07-09 05:11:24.000000 ns_asphalt9-0.1.0/ns_asphalt9.egg-info/top_level.txt
+-rw-r--r--   0 sunhao     (501) staff       (20)     1299 2023-07-09 05:11:24.000000 ns_asphalt9-0.1.0/setup.cfg
+-rw-r--r--   0 sunhao     (501) staff       (20)      387 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `ns_asphalt9-0.0.9/LICENSE` & `ns_asphalt9-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.9/PKG-INFO` & `ns_asphalt9-0.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 Metadata-Version: 2.1
 Name: ns_asphalt9
-Version: 0.0.9
+Version: 0.1.0
 Summary: Asphalt 9 daily task handling tool based on NXBT and V4L2.
 Home-page: https://pypi.python.org/pypi/ns_asphalt9
 Author: codehai
 Author-email: wmpksb@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Code, https://github.com/codehai/ns_asphalt9
 Project-URL: Issue tracker, https://github.com/codehai/ns_asphalt9/issues
+Description: # ns_asphalt9 
+        
+        基于nxbt和v4l2实现了闭环控制的Asphalt9日常任务处理工具。
+        
+        
+        ### 硬件依赖
+            
+        1. **[HDMI采集卡(必选)](https://u.jd.com/bizS2eh)** 
+           
+           用于switch画面输入到虚拟机
+        
+        2. **蓝牙(必选)**
+           
+           用于模拟手柄向switch发消息,Linux环境下可用本机蓝牙，Mac，Windows，群晖虚拟机请买usb蓝牙，注意群晖请需要适用于群晖的免驱蓝牙。
+        
+        3. **[HDMI分配器一分二 一进二出(可选)](https://u.jd.com/bqzn2Ek )** 
+           
+           同时输出switch到显示器和采集卡，方便debug
+        
+        
+        ### 使用教程
+        
+        [Wiki](https://github.com/codehai/ns_asphalt9/wiki)
+        
+        
+        ### 免责声明
+        
+        ns_asphalt为python学习交流的开源非营利项目，仅作为程序员之间相互学交流之用，使用需严格遵守开源许可协议。严禁用于商业用途，禁止使用ns_asphalt进行任何盈利活动。对一切非法使用所产生的后果，我们概不负责。
+        
+        
+        ### 许可证
+        
+        ![GitHub](https://img.shields.io/github/license/codehai/ns_asphalt9.svg)
+        
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >= 3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# ns_asphalt9 
-
-基于nxbt和v4l2实现了闭环控制的Asphalt9日常任务处理工具。
-
-
-### 硬件依赖
-    
-1. **[HDMI采集卡(必选)](https://u.jd.com/bizS2eh)** 
-   
-   用于switch画面输入到虚拟机
-
-2. **蓝牙(必选)**
-   
-   用于模拟手柄向switch发消息,Linux环境下可用本机蓝牙，Mac，Windows，群晖虚拟机请买usb蓝牙，注意群晖请需要适用于群晖的免驱蓝牙。
-
-3. **[HDMI分配器一分二 一进二出(可选)](https://u.jd.com/bqzn2Ek )** 
-   
-   同时输出switch到显示器和采集卡，方便debug
-
-
-### 使用教程
-
-[Wiki](https://github.com/codehai/ns_asphalt9/wiki)
-
-
-### 免责声明
-
-ns_asphalt为python学习交流的开源非营利项目，仅作为程序员之间相互学交流之用，使用需严格遵守开源许可协议。严禁用于商业用途，禁止使用ns_asphalt进行任何盈利活动。对一切非法使用所产生的后果，我们概不负责。
-
-
-### 许可证
-
-![GitHub](https://img.shields.io/github/license/codehai/ns_asphalt9.svg)
```

### Comparing `ns_asphalt9-0.0.9/README.md` & `ns_asphalt9-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.9/ns_asphalt9/core/actions/enter_page.py` & `ns_asphalt9-0.1.0/ns_asphalt9/core/actions/enter_page.py`

 * *Files 21% similar despite different names*

```diff
@@ -59,43 +59,65 @@
     page = ocr_screen()
     if in_series(page, mode):
         pass
     else:
         raise Exception(f"Failed to access {mode}, current page = {page.name}")
 
 
-@retry(max_attempts=3)
-def enter_carhunt(page=None):
-    """进入寻车"""
+def _enter_carhunt(page=None, mode=0):
+    """进入寻车/传奇寻车
+    0 寻车
+    1 传奇寻车
+    """
+    if mode == 0:
+        page_name = consts.carhunt
+        config_key = "寻车"
+        page_feature = "CAR HUNT(?!\sRIOT)"
+    else:
+        page_name = consts.legendary_hunt
+        config_key = "传奇寻车"
+        page_feature = "LEGENDARY HUNT(?!\sRIOT)"
     if page:
         logger.info(f"page = {page}, page.name = {page.name}")
-    if page and page.name == consts.carhunt:
+    if page and page.name == page_name:
         return
     reset_to_career()
     pro.press_group([Buttons.ZL] * 5, 0.5)
     pro.press_group([Buttons.A], 2)
-    pro.press_group([Buttons.ZR] * globals.CONFIG["寻车"]["寻车位置"], 0.5)
+    pro.press_group([Buttons.ZR] * globals.CONFIG[config_key]["寻车位置"], 0.5)
     time.sleep(1)
     page = ocr_screen()
-    if page.has_text("CAR HUNT(?!\sRIOT)"):
+    if page.has_text(page_feature):
         pro.press_a()
     else:
         pro.press_group([Buttons.ZL] * 12, 0)
         for i in range(20):
             pro.press_group([Buttons.ZR], 0.5)
             page = ocr_screen()
-            if page.has_text("CAR HUNT(?!\sRIOT)"):
-                globals.CONFIG["寻车"]["寻车位置"] = i + 1
+            if page.has_text(page_feature):
+                globals.CONFIG[config_key]["寻车位置"] = i + 1
                 pro.press_a()
                 break
         else:
             raise Exception(f"Failed to access carhunt, current page = {page.name}")
 
 
 @retry(max_attempts=3)
+def enter_carhunt(page=None):
+    """进入寻车"""
+    _enter_carhunt(page)
+
+
+@retry(max_attempts=3)
+def enter_legend_carhunt(page=None):
+    """进入传奇寻车"""
+    _enter_carhunt(page, 1)
+
+
+@retry(max_attempts=3)
 def free_pack(page=None):
     """领卡"""
     reset_to_career()
     pro.press_group([Buttons.DPAD_DOWN] * 3, 0.2)
     pro.press_group([Buttons.DPAD_LEFT] * 8, 0.2)
     pro.press_group([Buttons.A], 0.5)
     pro.press_group([Buttons.DPAD_UP], 0.5)
```

### Comparing `ns_asphalt9-0.0.9/ns_asphalt9/core/actions/process_race.py` & `ns_asphalt9-0.1.0/ns_asphalt9/core/actions/process_race.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.9/ns_asphalt9/core/actions/select_car.py` & `ns_asphalt9-0.1.0/ns_asphalt9/core/actions/select_car.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.9/ns_asphalt9/core/cache.py` & `ns_asphalt9-0.1.0/ns_asphalt9/core/cache.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.9/ns_asphalt9/core/consts.py` & `ns_asphalt9-0.1.0/ns_asphalt9/core/consts.py`

 * *Files 6% similar despite different names*

```diff
@@ -102,14 +102,15 @@
 }
 
 car_hunt_zh = "寻车"
 world_series_zh = "多人一"
 other_series_zh = "多人二"
 free_pack_zh = "免费抽卡"
 prix_pack_zh = "大奖赛抽卡"
+legendary_hunt_zh = "传奇寻车"
 
 
 class Mode:
     car_hunt = "CAR HUNT"
     world_series = "WORLD SERIES"
     limited_series = "LIMITED SERIES"
     trial_series = "TRIAL SERIES"
```

### Comparing `ns_asphalt9-0.0.9/ns_asphalt9/core/controller.py` & `ns_asphalt9-0.1.0/ns_asphalt9/core/controller.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.9/ns_asphalt9/core/globals.py` & `ns_asphalt9-0.1.0/ns_asphalt9/core/globals.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.9/ns_asphalt9/core/gui/app.py` & `ns_asphalt9-0.1.0/ns_asphalt9/core/gui/app.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self.settings_data = None
         self.config_file = f"{config_name}.json"
         if os.path.exists(self.config_file):
             with open(self.config_file, "r") as file:
                 self.settings_data = json.load(file)
 
         self.title("A9 AUTO")
-        self.geometry("700x450")
+        self.geometry("700x550")
 
         # set grid layout 1x2
         self.grid_rowconfigure(0, weight=1)
         self.grid_columnconfigure(1, weight=1)
 
         # load images with light and dark mode image
         image_path = os.path.join(os.path.dirname(os.path.realpath(__file__)), "images")
@@ -103,15 +103,15 @@
 
         # create home frame
         self.home_frame = customtkinter.CTkFrame(
             self, corner_radius=0, fg_color="transparent"
         )
         self.home_frame.grid_columnconfigure(0, weight=1)
 
-        self.textbox = customtkinter.CTkTextbox(self.home_frame, width=250, height=360)
+        self.textbox = customtkinter.CTkTextbox(self.home_frame, width=250, height=460)
         self.textbox.grid(row=0, column=0, padx=(20, 20), pady=(20, 20), sticky="nsew")
 
         self.entry = customtkinter.CTkEntry(
             self.home_frame, placeholder_text="Please input command."
         )
         self.entry.bind("<Return>", self.on_entry_enter)
         self.entry.grid(
@@ -121,15 +121,15 @@
         self.setting_modules = {}
 
         # create settings frame
         self.settings = customtkinter.CTkScrollableFrame(
             self, corner_radius=0, fg_color="transparent"
         )
 
-        for row, label_text in enumerate(["模式", "任务", "多一", "多二", "寻车", "大奖赛"]):
+        for row, label_text in enumerate(["模式", "任务", "多一", "多二", "寻车", "传奇寻车", "大奖赛"]):
             label = customtkinter.CTkLabel(master=self.settings, text=f"{label_text}:")
             label.grid(
                 row=row,
                 column=0,
                 columnspan=1,
                 padx=10,
                 pady=(20 if row == 0 else 10, 10),
@@ -138,40 +138,41 @@
 
         # 模式配置
         self.mode = tkinter.StringVar()
         self.mode_buttons = customtkinter.CTkSegmentedButton(
             self.settings,
             variable=self.mode,
             command=self.save_settings,
-            values=["多人一", "多人二", "寻车"],
+            values=["多人一", "多人二", "寻车", "传奇寻车"],
         )
         self.mode_buttons.grid(
             row=0, column=1, padx=(20, 10), pady=(20, 10), sticky="ew"
         )
         if self.settings_data:
             self.mode_buttons.set(self.settings_data["模式"])
         self.setting_modules["模式"] = self.mode_buttons
 
         # 任务配置
         tasks_frame = customtkinter.CTkFrame(self.settings, width=340)
         tasks_frame.grid(row=1, column=1, padx=(20, 0), pady=(20, 0), sticky="nsew")
-        tasks = [("免费抽卡", ["180", "240"]), ("大奖赛抽卡", ["240"]), ("寻车", ["10"])]
+        tasks = [("免费抽卡", ["180", "240"]), ("大奖赛抽卡", ["240"]), ("寻车", ["10"]), ("传奇寻车", ["10"])]
         self.setting_modules["任务"] = []
         for row, (task, values) in enumerate(tasks):
             task_box = customtkinter.CTkCheckBox(
                 master=tasks_frame, text=task, command=self.save_settings
             )
             task_box.grid(row=row, column=1, pady=(10, 10), padx=(20, 0), sticky="ew")
 
             task_combobox = customtkinter.CTkComboBox(
                 tasks_frame, values=values, width=100, command=self.save_settings
             )
             task_combobox.grid(row=row, column=2, padx=(20, 100), pady=(10, 10))
 
-            if self.settings_data:
+            if self.settings_data and row < len(self.settings_data["任务"]):
+
                 if self.settings_data["任务"][row]["运行"]:
                     task_box.select()
                 task_combobox.set(self.settings_data["任务"][row]["间隔"])
 
             self.setting_modules["任务"].append(
                 {"名称": task, "运行": task_box, "间隔": task_combobox}
             )
@@ -232,15 +233,15 @@
                     height=28,
                     command=self.save_settings,
                 )
 
                 option2 = customtkinter.CTkOptionMenu(
                     self.tabview.tab(tab_name),
                     dynamic_resizing=False,
-                    values=[str(i) for i in range(0, 20)],
+                    values=[str(i) for i in range(0, 30)],
                     width=100,
                     height=28,
                     command=self.save_settings,
                 )
 
                 option1.grid(row=r + 2, column=1, padx=(10, 10), pady=(10, 10))
                 option2.grid(row=r + 2, column=2, padx=(10, 10), pady=(10, 10))
@@ -283,15 +284,15 @@
                 height=28,
                 command=self.save_settings,
             )
 
             option2 = customtkinter.CTkOptionMenu(
                 mp2_settings_frame,
                 dynamic_resizing=False,
-                values=[str(i) for i in range(0, 20)],
+                values=[str(i) for i in range(0, 30)],
                 width=100,
                 height=28,
                 command=self.save_settings,
             )
 
             option1.grid(row=r + 2, column=1, padx=(10, 10), pady=(10, 10))
             option2.grid(row=r + 2, column=2, padx=(10, 10), pady=(10, 10))
@@ -352,34 +353,106 @@
                 height=28,
                 command=self.save_settings,
             )
 
             option2 = customtkinter.CTkOptionMenu(
                 carhunt_setting_frame,
                 dynamic_resizing=False,
-                values=[str(i) for i in range(0, 20)],
+                values=[str(i) for i in range(0, 30)],
                 width=100,
                 height=28,
                 command=self.save_settings,
             )
 
             option1.grid(row=r + 3, column=1, padx=(10, 10), pady=(10, 10))
             option2.grid(row=r + 3, column=2, padx=(10, 10), pady=(10, 10))
 
             if self.settings_data:
                 option1.set(self.settings_data["寻车"]["车库位置"][r]["row"])
                 option2.set(self.settings_data["寻车"]["车库位置"][r]["col"])
 
             self.setting_modules["寻车"]["车库位置"].append({"row": option1, "col": option2})
 
+        # 传奇寻车配置
+        self.setting_modules["传奇寻车"] = {}
+        carhunt_setting_frame = customtkinter.CTkFrame(self.settings, width=340)
+        carhunt_setting_frame.grid(
+            row=5, column=1, columnspan=2, padx=(20, 0), pady=(20, 20), sticky="nsew"
+        )
+
+        car_hunt_position = customtkinter.CTkLabel(
+            master=carhunt_setting_frame, text="寻车位置:"
+        )
+        car_hunt_position.grid(row=1, column=0, padx=(15, 10), pady=(10, 10))
+        position_option = customtkinter.CTkOptionMenu(
+            carhunt_setting_frame,
+            dynamic_resizing=False,
+            values=[str(i) for i in range(0, 20)],
+            width=100,
+            height=28,
+            command=self.save_settings,
+        )
+
+        position_option.grid(row=1, column=1, padx=(10, 10), pady=(10, 10))
+
+        if self.settings_data and "传奇寻车" in self.settings_data:
+            position_option.set(self.settings_data["传奇寻车"]["寻车位置"])
+        self.setting_modules["传奇寻车"]["寻车位置"] = position_option
+
+        self.setting_modules["传奇寻车"]["车库位置"] = []
+        car_position = customtkinter.CTkLabel(
+            master=carhunt_setting_frame, text="车库位置:"
+        )
+
+        car_position.grid(row=2, column=0, padx=(15, 10), pady=(10, 10))
+
+        row = customtkinter.CTkLabel(master=carhunt_setting_frame, text="row")
+
+        row.grid(row=2, column=1, padx=(0, 0), pady=(10, 10), sticky="nsew")
+
+        col = customtkinter.CTkLabel(master=carhunt_setting_frame, text="col")
+
+        col.grid(row=2, column=2, padx=(0, 10), pady=(10, 10), sticky="nsew")
+
+        for r in range(6):
+            option1 = customtkinter.CTkOptionMenu(
+                carhunt_setting_frame,
+                dynamic_resizing=False,
+                values=[str(i) for i in range(0, 3)],
+                width=100,
+                height=28,
+                command=self.save_settings,
+            )
+
+            option2 = customtkinter.CTkOptionMenu(
+                carhunt_setting_frame,
+                dynamic_resizing=False,
+                values=[str(i) for i in range(0, 30)],
+                width=100,
+                height=28,
+                command=self.save_settings,
+            )
+
+            option1.grid(row=r + 3, column=1, padx=(10, 10), pady=(10, 10))
+            option2.grid(row=r + 3, column=2, padx=(10, 10), pady=(10, 10))
+
+            try:
+                if self.settings_data and "传奇寻车" in self.settings_data:
+                    option1.set(self.settings_data["传奇寻车"]["车库位置"][r]["row"])
+                    option2.set(self.settings_data["传奇寻车"]["车库位置"][r]["col"])
+            except IndexError:
+                pass
+
+            self.setting_modules["寻车"]["车库位置"].append({"row": option1, "col": option2})
+
         # 大奖赛配置
         self.setting_modules["大奖赛"] = {}
         prix_setting_frame = customtkinter.CTkFrame(self.settings, width=340)
         prix_setting_frame.grid(
-            row=5, column=1, columnspan=2, padx=(20, 0), pady=(20, 20), sticky="nsew"
+            row=6, column=1, columnspan=2, padx=(20, 0), pady=(20, 20), sticky="nsew"
         )
 
         prix_position = customtkinter.CTkLabel(
             master=prix_setting_frame, text="位置:"
         )
         prix_position.grid(row=1, column=0, padx=(15, 10), pady=(10, 10))
         prix_position_option = customtkinter.CTkOptionMenu(
```

### Comparing `ns_asphalt9-0.0.9/ns_asphalt9/core/gui/images/help.png` & `ns_asphalt9-0.1.0/ns_asphalt9/core/gui/images/help.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.9/ns_asphalt9/core/gui/images/home.png` & `ns_asphalt9-0.1.0/ns_asphalt9/core/gui/images/home.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.9/ns_asphalt9/core/gui/images/logo.png` & `ns_asphalt9-0.1.0/ns_asphalt9/core/gui/images/logo.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.9/ns_asphalt9/core/gui/images/settings.png` & `ns_asphalt9-0.1.0/ns_asphalt9/core/gui/images/settings.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.9/ns_asphalt9/core/ocr.py` & `ns_asphalt9-0.1.0/ns_asphalt9/core/ocr.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.9/ns_asphalt9/core/page_factory.py` & `ns_asphalt9-0.1.0/ns_asphalt9/core/page_factory.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.9/ns_asphalt9/core/pages.py` & `ns_asphalt9-0.1.0/ns_asphalt9/core/pages.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,19 +141,26 @@
 
 
 @cache_decorator("page")
 class MultiPlayer(Page):
     """多人首页"""
 
     name = consts.multi_player
-    feature = "WORLD SERIES.*(LIMITED|TRIAL) SERIES"
+    feature = "WORLD SERIES|LIMITED SERIES|TRIAL SERIES"
     part_match = False
 
     action = staticmethod(actions.enter_series)
 
+    @classmethod
+    def calc_weight(cls, text: str) -> int:
+        match_count = len(re.findall(cls.feature, text))
+        if match_count >= 2:
+            match_count = 10
+        return match_count
+
 
 @cache_decorator("page")
 class WorldSeries(Page):
     """多人一"""
 
     name = consts.world_series
     feature = "WORLD SERIES|MY POSITION|SERIES SCORE|NEXT MILESTONE|LEADERBOARD|PLAY"
@@ -221,17 +228,20 @@
 
 
 @cache_decorator("page")
 class LegendaryHunt(Page):
     """通行证寻车"""
 
     name = consts.legendary_hunt
-    feature = "LEGENDARY HUNT"
+    feature = "LEGENDARY HUNT:.*CAR HUNT EVENT PACK"
     part_match = False
 
+    action = staticmethod(pro.press_button)
+    args = (Buttons.A, 3)
+
 
 @cache_decorator("page")
 class Tickets(Page):
     """购买票"""
 
     name = consts.tickets
     feature = "TICKETS"
@@ -563,12 +573,13 @@
     part_match = False
     action = staticmethod(pro.press_button)
     args = (Buttons.B,)
 
     @classmethod
     def calc_weight(cls, text: str) -> int:
         match_count = len(re.findall(cls.feature, text))
-        if "ENDS IN" in text:
-            match_count = 0
-        else:
-            match_count = 10
+        if match_count:
+            if "ENDS IN" in text:
+                match_count = 0
+            else:
+                match_count = 10
         return match_count
```

### Comparing `ns_asphalt9-0.0.9/ns_asphalt9/core/tasks.py` & `ns_asphalt9-0.1.0/ns_asphalt9/core/tasks.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,15 +39,17 @@
 
         if page.name not in [
             consts.world_series,
             consts.limited_series,
             consts.trial_series,
             consts.carhunt,
             consts.card_pack,
-            consts.legend_pass
+            consts.legend_pass,
+            consts.legendary_hunt,
+            consts.daily_events
         ]:
             return False
 
         if globals.task_queue.empty():
             if cls.status == consts.TaskStatus.done:
                 cls.task_enter(globals.CONFIG["模式"], page=page)
                 cls.status = consts.TaskStatus.default
@@ -69,13 +71,15 @@
             actions.enter_series(mode=task, page=page)
         if task == consts.car_hunt_zh:
             actions.enter_carhunt(page=page)
         if task == consts.free_pack_zh:
             actions.free_pack()
         if task == consts.prix_pack_zh:
             actions.prix_pack()
+        if task == consts.legendary_hunt_zh:
+            actions.enter_legend_carhunt()
 
     @classmethod
     def set_done(cls) -> None:
         if cls.status == consts.TaskStatus.start:
             cls.status = consts.TaskStatus.done
             cls.current_task = ""
```

### Comparing `ns_asphalt9-0.0.9/ns_asphalt9/core/utils/decorator.py` & `ns_asphalt9-0.1.0/ns_asphalt9/core/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.9/ns_asphalt9/core/utils/log.py` & `ns_asphalt9-0.1.0/ns_asphalt9/core/utils/log.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.9/ns_asphalt9/core/utils/timer.py` & `ns_asphalt9-0.1.0/ns_asphalt9/core/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.9/ns_asphalt9/main.py` & `ns_asphalt9-0.1.0/ns_asphalt9/main.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.9/ns_asphalt9.egg-info/PKG-INFO` & `ns_asphalt9-0.1.0/ns_asphalt9.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 Metadata-Version: 2.1
 Name: ns-asphalt9
-Version: 0.0.9
+Version: 0.1.0
 Summary: Asphalt 9 daily task handling tool based on NXBT and V4L2.
 Home-page: https://pypi.python.org/pypi/ns_asphalt9
 Author: codehai
 Author-email: wmpksb@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Code, https://github.com/codehai/ns_asphalt9
 Project-URL: Issue tracker, https://github.com/codehai/ns_asphalt9/issues
+Description: # ns_asphalt9 
+        
+        基于nxbt和v4l2实现了闭环控制的Asphalt9日常任务处理工具。
+        
+        
+        ### 硬件依赖
+            
+        1. **[HDMI采集卡(必选)](https://u.jd.com/bizS2eh)** 
+           
+           用于switch画面输入到虚拟机
+        
+        2. **蓝牙(必选)**
+           
+           用于模拟手柄向switch发消息,Linux环境下可用本机蓝牙，Mac，Windows，群晖虚拟机请买usb蓝牙，注意群晖请需要适用于群晖的免驱蓝牙。
+        
+        3. **[HDMI分配器一分二 一进二出(可选)](https://u.jd.com/bqzn2Ek )** 
+           
+           同时输出switch到显示器和采集卡，方便debug
+        
+        
+        ### 使用教程
+        
+        [Wiki](https://github.com/codehai/ns_asphalt9/wiki)
+        
+        
+        ### 免责声明
+        
+        ns_asphalt为python学习交流的开源非营利项目，仅作为程序员之间相互学交流之用，使用需严格遵守开源许可协议。严禁用于商业用途，禁止使用ns_asphalt进行任何盈利活动。对一切非法使用所产生的后果，我们概不负责。
+        
+        
+        ### 许可证
+        
+        ![GitHub](https://img.shields.io/github/license/codehai/ns_asphalt9.svg)
+        
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >= 3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# ns_asphalt9 
-
-基于nxbt和v4l2实现了闭环控制的Asphalt9日常任务处理工具。
-
-
-### 硬件依赖
-    
-1. **[HDMI采集卡(必选)](https://u.jd.com/bizS2eh)** 
-   
-   用于switch画面输入到虚拟机
-
-2. **蓝牙(必选)**
-   
-   用于模拟手柄向switch发消息,Linux环境下可用本机蓝牙，Mac，Windows，群晖虚拟机请买usb蓝牙，注意群晖请需要适用于群晖的免驱蓝牙。
-
-3. **[HDMI分配器一分二 一进二出(可选)](https://u.jd.com/bqzn2Ek )** 
-   
-   同时输出switch到显示器和采集卡，方便debug
-
-
-### 使用教程
-
-[Wiki](https://github.com/codehai/ns_asphalt9/wiki)
-
-
-### 免责声明
-
-ns_asphalt为python学习交流的开源非营利项目，仅作为程序员之间相互学交流之用，使用需严格遵守开源许可协议。严禁用于商业用途，禁止使用ns_asphalt进行任何盈利活动。对一切非法使用所产生的后果，我们概不负责。
-
-
-### 许可证
-
-![GitHub](https://img.shields.io/github/license/codehai/ns_asphalt9.svg)
```

### Comparing `ns_asphalt9-0.0.9/ns_asphalt9.egg-info/SOURCES.txt` & `ns_asphalt9-0.1.0/ns_asphalt9.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -32,9 +32,8 @@
 ns_asphalt9/core/gui/images/home.png
 ns_asphalt9/core/gui/images/logo.png
 ns_asphalt9/core/gui/images/settings.png
 ns_asphalt9/core/utils/__init__.py
 ns_asphalt9/core/utils/decorator.py
 ns_asphalt9/core/utils/fetch_cars.py
 ns_asphalt9/core/utils/log.py
-ns_asphalt9/core/utils/timer.py
-tests/test_ocr.py
+ns_asphalt9/core/utils/timer.py
```

### Comparing `ns_asphalt9-0.0.9/setup.cfg` & `ns_asphalt9-0.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nxbt
-version = 0.0.9
+version = 0.1.0
 author = codehai
 author-email = wmpksb@gmail.com
 project_urls = 
 	Code = https://github.com/codehai/ns_asphalt9
 	Issue tracker = https://github.com/codehai/ns_asphalt9/issues
 license = GNU General Public License v3 (GPLv3)
 license-file = LICENSE
```

