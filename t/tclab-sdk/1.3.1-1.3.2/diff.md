# Comparing `tmp/tclab-sdk-1.3.1.tar.gz` & `tmp/tclab-sdk-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tclab-sdk-1.3.1.tar", last modified: Fri Jul  7 05:44:05 2023, max compression
+gzip compressed data, was "tclab-sdk-1.3.2.tar", last modified: Sat Jul  8 09:25:24 2023, max compression
```

## Comparing `tclab-sdk-1.3.1.tar` & `tclab-sdk-1.3.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 05:44:05.407477 tclab-sdk-1.3.1/
--rw-rw-rw-   0        0        0      888 2023-07-07 05:44:05.406480 tclab-sdk-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-07-07 03:03:35.000000 tclab-sdk-1.3.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-07 05:44:05.408482 tclab-sdk-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0      946 2023-07-07 05:44:02.000000 tclab-sdk-1.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 05:44:05.375478 tclab-sdk-1.3.1/tclab/
--rw-rw-rw-   0        0        0    16593 2023-07-07 05:43:34.000000 tclab-sdk-1.3.1/tclab/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 05:44:05.403482 tclab-sdk-1.3.1/tclab_sdk.egg-info/
--rw-rw-rw-   0        0        0      888 2023-07-07 05:44:05.000000 tclab-sdk-1.3.1/tclab_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2023-07-07 05:44:05.000000 tclab-sdk-1.3.1/tclab_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 05:44:05.000000 tclab-sdk-1.3.1/tclab_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-07-07 05:44:05.000000 tclab-sdk-1.3.1/tclab_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-07 05:44:05.000000 tclab-sdk-1.3.1/tclab_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 09:25:24.195869 tclab-sdk-1.3.2/
+-rw-rw-rw-   0        0        0      888 2023-07-08 09:25:24.193869 tclab-sdk-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-07-07 03:03:35.000000 tclab-sdk-1.3.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 09:25:24.195869 tclab-sdk-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      946 2023-07-08 09:25:20.000000 tclab-sdk-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 09:25:24.077633 tclab-sdk-1.3.2/tclab/
+-rw-rw-rw-   0        0        0    16595 2023-07-08 09:24:27.000000 tclab-sdk-1.3.2/tclab/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 09:25:24.191871 tclab-sdk-1.3.2/tclab_sdk.egg-info/
+-rw-rw-rw-   0        0        0      888 2023-07-08 09:25:23.000000 tclab-sdk-1.3.2/tclab_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2023-07-08 09:25:23.000000 tclab-sdk-1.3.2/tclab_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 09:25:23.000000 tclab-sdk-1.3.2/tclab_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-08 09:25:23.000000 tclab-sdk-1.3.2/tclab_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-08 09:25:23.000000 tclab-sdk-1.3.2/tclab_sdk.egg-info/top_level.txt
```

### Comparing `tclab-sdk-1.3.1/PKG-INFO` & `tclab-sdk-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tclab-sdk
-Version: 1.3.1
+Version: 1.3.2
 Summary: TC Laboratory Central_Management_System Client Module
 Home-page: UNKNOWN
 Author: Haotian Yang
 Author-email: yht1592754117@126.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tclab-sdk-1.3.1/setup.py` & `tclab-sdk-1.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 with open("README.md", "r",encoding='utf-8') as fh:
     long_description = fh.read()
 setuptools.setup(
     name="tclab-sdk",  # 模块名称
-    version="1.3.1",  # 当前版本
+    version="1.3.2",  # 当前版本
     author="Haotian Yang",  # 作者
     author_email="yht1592754117@126.com",  # 作者邮箱
     description="TC Laboratory Central_Management_System Client Module",  # 模块简介
     long_description=long_description,  # 模块详细介绍
     long_description_content_type="text/markdown",  # 模块详细介绍格式
     packages=setuptools.find_packages(),  # 自动找到项目中导入的模块
     # 模块相关的元数据
```

### Comparing `tclab-sdk-1.3.1/tclab/__init__.py` & `tclab-sdk-1.3.2/tclab/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,15 @@
                 head = ''
                 now = ''
                 tail = function['name']
                 while len(tail):
                     if tail[0] == '.' and len(tail) > 1:
                         if now not in dir(eval(f"self{head}")):
                             exec(f"class {now}:\n    pass")
-                            exec(f"self{head}.{now}={now}")
+                            exec(f"self{head}.{now}={now}()")
                         head += f'.{now}'
                         now = ''
                         tail = tail[1:]
                     now += tail[0]
                     tail = tail[1:]
                 # 固定转发器
                 exec(
```

### Comparing `tclab-sdk-1.3.1/tclab_sdk.egg-info/PKG-INFO` & `tclab-sdk-1.3.2/tclab_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tclab-sdk
-Version: 1.3.1
+Version: 1.3.2
 Summary: TC Laboratory Central_Management_System Client Module
 Home-page: UNKNOWN
 Author: Haotian Yang
 Author-email: yht1592754117@126.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

