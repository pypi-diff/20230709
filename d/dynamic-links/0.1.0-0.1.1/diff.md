# Comparing `tmp/dynamic-links-0.1.0.tar.gz` & `tmp/dynamic-links-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic-links-0.1.0.tar", last modified: Sun Jul  9 07:00:01 2023, max compression
+gzip compressed data, was "dynamic-links-0.1.1.tar", last modified: Sun Jul  9 17:41:21 2023, max compression
```

## Comparing `dynamic-links-0.1.0.tar` & `dynamic-links-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 pic        (501) staff       (20)        0 2023-07-09 07:00:01.501501 dynamic-links-0.1.0/
--rw-r--r--   0 pic        (501) staff       (20)     8593 2023-07-09 07:00:01.501268 dynamic-links-0.1.0/PKG-INFO
--rw-r--r--   0 pic        (501) staff       (20)     8320 2023-07-09 06:53:12.000000 dynamic-links-0.1.0/README.md
-drwxr-xr-x   0 pic        (501) staff       (20)        0 2023-07-09 07:00:01.500230 dynamic-links-0.1.0/dlframe/
--rw-r--r--   0 pic        (501) staff       (20)     2645 2023-07-09 05:06:10.000000 dynamic-links-0.1.0/dlframe/CalculationNode.py
--rw-r--r--   0 pic        (501) staff       (20)     4034 2023-07-09 05:32:50.000000 dynamic-links-0.1.0/dlframe/CalculationNodeManager.py
--rw-r--r--   0 pic        (501) staff       (20)     2048 2023-06-27 04:00:46.000000 dynamic-links-0.1.0/dlframe/ExecutionNode.py
--rw-r--r--   0 pic        (501) staff       (20)      939 2023-06-27 05:19:42.000000 dynamic-links-0.1.0/dlframe/Logger.py
--rw-r--r--   0 pic        (501) staff       (20)     5369 2023-07-09 06:58:58.000000 dynamic-links-0.1.0/dlframe/RecursiveWarpper.py
--rw-r--r--   0 pic        (501) staff       (20)     6141 2023-07-09 06:55:50.000000 dynamic-links-0.1.0/dlframe/TimeWarpper.py
--rw-r--r--   0 pic        (501) staff       (20)     5277 2023-07-08 16:20:45.000000 dynamic-links-0.1.0/dlframe/WebManager.py
--rw-r--r--   0 pic        (501) staff       (20)      274 2023-07-09 06:55:19.000000 dynamic-links-0.1.0/dlframe/__init__.py
-drwxr-xr-x   0 pic        (501) staff       (20)        0 2023-07-09 07:00:01.500969 dynamic-links-0.1.0/dynamic_links.egg-info/
--rw-r--r--   0 pic        (501) staff       (20)     8593 2023-07-09 07:00:01.000000 dynamic-links-0.1.0/dynamic_links.egg-info/PKG-INFO
--rw-r--r--   0 pic        (501) staff       (20)      399 2023-07-09 07:00:01.000000 dynamic-links-0.1.0/dynamic_links.egg-info/SOURCES.txt
--rw-r--r--   0 pic        (501) staff       (20)        1 2023-07-09 07:00:01.000000 dynamic-links-0.1.0/dynamic_links.egg-info/dependency_links.txt
--rw-r--r--   0 pic        (501) staff       (20)       30 2023-07-09 07:00:01.000000 dynamic-links-0.1.0/dynamic_links.egg-info/requires.txt
--rw-r--r--   0 pic        (501) staff       (20)        8 2023-07-09 07:00:01.000000 dynamic-links-0.1.0/dynamic_links.egg-info/top_level.txt
--rw-r--r--   0 pic        (501) staff       (20)       38 2023-07-09 07:00:01.501555 dynamic-links-0.1.0/setup.cfg
--rw-r--r--   0 pic        (501) staff       (20)      682 2023-07-09 06:59:02.000000 dynamic-links-0.1.0/setup.py
+drwxr-xr-x   0 pic        (501) staff       (20)        0 2023-07-09 17:41:21.801169 dynamic-links-0.1.1/
+-rw-r--r--   0 pic        (501) staff       (20)     8610 2023-07-09 17:41:21.800954 dynamic-links-0.1.1/PKG-INFO
+-rw-r--r--   0 pic        (501) staff       (20)     8318 2023-07-09 17:40:14.000000 dynamic-links-0.1.1/README.md
+drwxr-xr-x   0 pic        (501) staff       (20)        0 2023-07-09 17:41:21.799916 dynamic-links-0.1.1/dlframe/
+-rw-r--r--   0 pic        (501) staff       (20)     2645 2023-07-09 05:06:10.000000 dynamic-links-0.1.1/dlframe/CalculationNode.py
+-rw-r--r--   0 pic        (501) staff       (20)     4034 2023-07-09 15:01:07.000000 dynamic-links-0.1.1/dlframe/CalculationNodeManager.py
+-rw-r--r--   0 pic        (501) staff       (20)     2048 2023-06-27 04:00:46.000000 dynamic-links-0.1.1/dlframe/ExecutionNode.py
+-rw-r--r--   0 pic        (501) staff       (20)      939 2023-07-09 15:17:01.000000 dynamic-links-0.1.1/dlframe/Logger.py
+-rw-r--r--   0 pic        (501) staff       (20)     5369 2023-07-09 06:58:58.000000 dynamic-links-0.1.1/dlframe/RecursiveWarpper.py
+-rw-r--r--   0 pic        (501) staff       (20)     6141 2023-07-09 06:55:50.000000 dynamic-links-0.1.1/dlframe/TimeWarpper.py
+-rw-r--r--   0 pic        (501) staff       (20)     5277 2023-07-08 16:20:45.000000 dynamic-links-0.1.1/dlframe/WebManager.py
+-rw-r--r--   0 pic        (501) staff       (20)      274 2023-07-09 06:55:19.000000 dynamic-links-0.1.1/dlframe/__init__.py
+drwxr-xr-x   0 pic        (501) staff       (20)        0 2023-07-09 17:41:21.800657 dynamic-links-0.1.1/dynamic_links.egg-info/
+-rw-r--r--   0 pic        (501) staff       (20)     8610 2023-07-09 17:41:21.000000 dynamic-links-0.1.1/dynamic_links.egg-info/PKG-INFO
+-rw-r--r--   0 pic        (501) staff       (20)      399 2023-07-09 17:41:21.000000 dynamic-links-0.1.1/dynamic_links.egg-info/SOURCES.txt
+-rw-r--r--   0 pic        (501) staff       (20)        1 2023-07-09 17:41:21.000000 dynamic-links-0.1.1/dynamic_links.egg-info/dependency_links.txt
+-rw-r--r--   0 pic        (501) staff       (20)       30 2023-07-09 17:41:21.000000 dynamic-links-0.1.1/dynamic_links.egg-info/requires.txt
+-rw-r--r--   0 pic        (501) staff       (20)        8 2023-07-09 17:41:21.000000 dynamic-links-0.1.1/dynamic_links.egg-info/top_level.txt
+-rw-r--r--   0 pic        (501) staff       (20)       38 2023-07-09 17:41:21.801226 dynamic-links-0.1.1/setup.cfg
+-rw-r--r--   0 pic        (501) staff       (20)      682 2023-07-09 17:40:23.000000 dynamic-links-0.1.1/setup.py
```

### Comparing `dynamic-links-0.1.0/PKG-INFO` & `dynamic-links-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: dynamic-links
-Version: 0.1.0
+Version: 0.1.1
 Summary: a calculation framework
 Home-page: https://github.com/picpic2013/dlframe-back
 Author: PIC
 Author-email: picpic2019@gmail.com
 License: MIT
+Platform: UNKNOWN
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 
 # Dynamic Links
 
 ## 安装方法
 
@@ -179,15 +180,15 @@
 # logger 支持打印文字
 logger.print('str1', 'str2', end='\t')
 
 # logger 支持显示图片
 logger.imshow(
     np.random.randint(
         0, 256, (100, 100, 3), 
-        dtype=np。uint8
+        dtype=np.uint8
     )
 )
 ~~~
 
 ### 并行模块
 
 框架默认按照定义的框架执行逻辑顺序执行，您也可以通过`parallel=True`手动开启并行执行(TODO: 目前仅为单线程)。此时，本框架会按照定义逻辑的拓扑排序执行代码。对于拓扑排序结果相同的，不保证执行的先后顺序。例如：
@@ -344,7 +345,8 @@
 res4 = f4(arg1, arg2, base1="arg1: {}", base2=" arg2: {}")
 
 print(res1)
 print(res2)
 print(res3)
 print(res4)
 ~~~
+
```

### Comparing `dynamic-links-0.1.0/README.md` & `dynamic-links-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
 # logger 支持打印文字
 logger.print('str1', 'str2', end='\t')
 
 # logger 支持显示图片
 logger.imshow(
     np.random.randint(
         0, 256, (100, 100, 3), 
-        dtype=np。uint8
+        dtype=np.uint8
     )
 )
 ~~~
 
 ### 并行模块
 
 框架默认按照定义的框架执行逻辑顺序执行，您也可以通过`parallel=True`手动开启并行执行(TODO: 目前仅为单线程)。此时，本框架会按照定义逻辑的拓扑排序执行代码。对于拓扑排序结果相同的，不保证执行的先后顺序。例如：
```

### Comparing `dynamic-links-0.1.0/dlframe/CalculationNode.py` & `dynamic-links-0.1.1/dlframe/CalculationNode.py`

 * *Files identical despite different names*

### Comparing `dynamic-links-0.1.0/dlframe/CalculationNodeManager.py` & `dynamic-links-0.1.1/dlframe/CalculationNodeManager.py`

 * *Files identical despite different names*

### Comparing `dynamic-links-0.1.0/dlframe/ExecutionNode.py` & `dynamic-links-0.1.1/dlframe/ExecutionNode.py`

 * *Files identical despite different names*

### Comparing `dynamic-links-0.1.0/dlframe/Logger.py` & `dynamic-links-0.1.1/dlframe/Logger.py`

 * *Files identical despite different names*

### Comparing `dynamic-links-0.1.0/dlframe/RecursiveWarpper.py` & `dynamic-links-0.1.1/dlframe/RecursiveWarpper.py`

 * *Files identical despite different names*

### Comparing `dynamic-links-0.1.0/dlframe/TimeWarpper.py` & `dynamic-links-0.1.1/dlframe/TimeWarpper.py`

 * *Files identical despite different names*

### Comparing `dynamic-links-0.1.0/dlframe/WebManager.py` & `dynamic-links-0.1.1/dlframe/WebManager.py`

 * *Files identical despite different names*

### Comparing `dynamic-links-0.1.0/dynamic_links.egg-info/PKG-INFO` & `dynamic-links-0.1.1/dynamic_links.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: dynamic-links
-Version: 0.1.0
+Version: 0.1.1
 Summary: a calculation framework
 Home-page: https://github.com/picpic2013/dlframe-back
 Author: PIC
 Author-email: picpic2019@gmail.com
 License: MIT
+Platform: UNKNOWN
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 
 # Dynamic Links
 
 ## 安装方法
 
@@ -179,15 +180,15 @@
 # logger 支持打印文字
 logger.print('str1', 'str2', end='\t')
 
 # logger 支持显示图片
 logger.imshow(
     np.random.randint(
         0, 256, (100, 100, 3), 
-        dtype=np。uint8
+        dtype=np.uint8
     )
 )
 ~~~
 
 ### 并行模块
 
 框架默认按照定义的框架执行逻辑顺序执行，您也可以通过`parallel=True`手动开启并行执行(TODO: 目前仅为单线程)。此时，本框架会按照定义逻辑的拓扑排序执行代码。对于拓扑排序结果相同的，不保证执行的先后顺序。例如：
@@ -344,7 +345,8 @@
 res4 = f4(arg1, arg2, base1="arg1: {}", base2=" arg2: {}")
 
 print(res1)
 print(res2)
 print(res3)
 print(res4)
 ~~~
+
```

### Comparing `dynamic-links-0.1.0/setup.py` & `dynamic-links-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 with open(os.path.join(here, 'README.md'), 'r',encoding='UTF-8') as mdFile:
     long_description = mdFile.read()
 
 setup(
     name='dynamic-links', 
-    version='0.1.0', 
+    version='0.1.1', 
     packages=['dlframe'], 
     url='https://github.com/picpic2013/dlframe-back', 
     license='MIT', 
     author='PIC', 
     author_email='picpic2019@gmail.com', 
     description='a calculation framework', 
     long_description=long_description,
```

