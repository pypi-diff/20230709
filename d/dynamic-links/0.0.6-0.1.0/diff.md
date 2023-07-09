# Comparing `tmp/dynamic-links-0.0.6.tar.gz` & `tmp/dynamic-links-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic-links-0.0.6.tar", last modified: Sun Jul  9 05:44:31 2023, max compression
+gzip compressed data, was "dynamic-links-0.1.0.tar", last modified: Sun Jul  9 07:00:01 2023, max compression
```

## Comparing `dynamic-links-0.0.6.tar` & `dynamic-links-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 pic        (501) staff       (20)        0 2023-07-09 05:44:31.509507 dynamic-links-0.0.6/
--rw-r--r--   0 pic        (501) staff       (20)     6301 2023-07-09 05:44:31.509358 dynamic-links-0.0.6/PKG-INFO
--rw-r--r--   0 pic        (501) staff       (20)     6028 2023-07-09 04:44:56.000000 dynamic-links-0.0.6/README.md
-drwxr-xr-x   0 pic        (501) staff       (20)        0 2023-07-09 05:44:31.508453 dynamic-links-0.0.6/dlframe/
--rw-r--r--   0 pic        (501) staff       (20)     2645 2023-07-09 05:06:10.000000 dynamic-links-0.0.6/dlframe/CalculationNode.py
--rw-r--r--   0 pic        (501) staff       (20)     4034 2023-07-09 05:32:50.000000 dynamic-links-0.0.6/dlframe/CalculationNodeManager.py
--rw-r--r--   0 pic        (501) staff       (20)     2048 2023-06-27 04:00:46.000000 dynamic-links-0.0.6/dlframe/ExecutionNode.py
--rw-r--r--   0 pic        (501) staff       (20)      939 2023-06-27 05:19:42.000000 dynamic-links-0.0.6/dlframe/Logger.py
--rw-r--r--   0 pic        (501) staff       (20)     5277 2023-07-08 16:20:45.000000 dynamic-links-0.0.6/dlframe/WebManager.py
--rw-r--r--   0 pic        (501) staff       (20)      141 2023-06-26 17:09:16.000000 dynamic-links-0.0.6/dlframe/__init__.py
-drwxr-xr-x   0 pic        (501) staff       (20)        0 2023-07-09 05:44:31.509166 dynamic-links-0.0.6/dynamic_links.egg-info/
--rw-r--r--   0 pic        (501) staff       (20)     6301 2023-07-09 05:44:31.000000 dynamic-links-0.0.6/dynamic_links.egg-info/PKG-INFO
--rw-r--r--   0 pic        (501) staff       (20)      348 2023-07-09 05:44:31.000000 dynamic-links-0.0.6/dynamic_links.egg-info/SOURCES.txt
--rw-r--r--   0 pic        (501) staff       (20)        1 2023-07-09 05:44:31.000000 dynamic-links-0.0.6/dynamic_links.egg-info/dependency_links.txt
--rw-r--r--   0 pic        (501) staff       (20)       30 2023-07-09 05:44:31.000000 dynamic-links-0.0.6/dynamic_links.egg-info/requires.txt
--rw-r--r--   0 pic        (501) staff       (20)        8 2023-07-09 05:44:31.000000 dynamic-links-0.0.6/dynamic_links.egg-info/top_level.txt
--rw-r--r--   0 pic        (501) staff       (20)       38 2023-07-09 05:44:31.509556 dynamic-links-0.0.6/setup.cfg
--rw-r--r--   0 pic        (501) staff       (20)      682 2023-07-09 05:09:12.000000 dynamic-links-0.0.6/setup.py
+drwxr-xr-x   0 pic        (501) staff       (20)        0 2023-07-09 07:00:01.501501 dynamic-links-0.1.0/
+-rw-r--r--   0 pic        (501) staff       (20)     8593 2023-07-09 07:00:01.501268 dynamic-links-0.1.0/PKG-INFO
+-rw-r--r--   0 pic        (501) staff       (20)     8320 2023-07-09 06:53:12.000000 dynamic-links-0.1.0/README.md
+drwxr-xr-x   0 pic        (501) staff       (20)        0 2023-07-09 07:00:01.500230 dynamic-links-0.1.0/dlframe/
+-rw-r--r--   0 pic        (501) staff       (20)     2645 2023-07-09 05:06:10.000000 dynamic-links-0.1.0/dlframe/CalculationNode.py
+-rw-r--r--   0 pic        (501) staff       (20)     4034 2023-07-09 05:32:50.000000 dynamic-links-0.1.0/dlframe/CalculationNodeManager.py
+-rw-r--r--   0 pic        (501) staff       (20)     2048 2023-06-27 04:00:46.000000 dynamic-links-0.1.0/dlframe/ExecutionNode.py
+-rw-r--r--   0 pic        (501) staff       (20)      939 2023-06-27 05:19:42.000000 dynamic-links-0.1.0/dlframe/Logger.py
+-rw-r--r--   0 pic        (501) staff       (20)     5369 2023-07-09 06:58:58.000000 dynamic-links-0.1.0/dlframe/RecursiveWarpper.py
+-rw-r--r--   0 pic        (501) staff       (20)     6141 2023-07-09 06:55:50.000000 dynamic-links-0.1.0/dlframe/TimeWarpper.py
+-rw-r--r--   0 pic        (501) staff       (20)     5277 2023-07-08 16:20:45.000000 dynamic-links-0.1.0/dlframe/WebManager.py
+-rw-r--r--   0 pic        (501) staff       (20)      274 2023-07-09 06:55:19.000000 dynamic-links-0.1.0/dlframe/__init__.py
+drwxr-xr-x   0 pic        (501) staff       (20)        0 2023-07-09 07:00:01.500969 dynamic-links-0.1.0/dynamic_links.egg-info/
+-rw-r--r--   0 pic        (501) staff       (20)     8593 2023-07-09 07:00:01.000000 dynamic-links-0.1.0/dynamic_links.egg-info/PKG-INFO
+-rw-r--r--   0 pic        (501) staff       (20)      399 2023-07-09 07:00:01.000000 dynamic-links-0.1.0/dynamic_links.egg-info/SOURCES.txt
+-rw-r--r--   0 pic        (501) staff       (20)        1 2023-07-09 07:00:01.000000 dynamic-links-0.1.0/dynamic_links.egg-info/dependency_links.txt
+-rw-r--r--   0 pic        (501) staff       (20)       30 2023-07-09 07:00:01.000000 dynamic-links-0.1.0/dynamic_links.egg-info/requires.txt
+-rw-r--r--   0 pic        (501) staff       (20)        8 2023-07-09 07:00:01.000000 dynamic-links-0.1.0/dynamic_links.egg-info/top_level.txt
+-rw-r--r--   0 pic        (501) staff       (20)       38 2023-07-09 07:00:01.501555 dynamic-links-0.1.0/setup.cfg
+-rw-r--r--   0 pic        (501) staff       (20)      682 2023-07-09 06:59:02.000000 dynamic-links-0.1.0/setup.py
```

### Comparing `dynamic-links-0.0.6/PKG-INFO` & `dynamic-links-0.1.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-links
-Version: 0.0.6
+Version: 0.1.0
 Summary: a calculation framework
 Home-page: https://github.com/picpic2013/dlframe-back
 Author: PIC
 Author-email: picpic2019@gmail.com
 License: MIT
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
@@ -243,7 +243,108 @@
 ~~~
 
 ## 关于前端
 
 本框架仅提供 WebSocket 服务，不提供页面显示。需配合[前端](https://picpic2013.github.io/dlframe-front/)使用。前端代码开源在[仓库](https://github.com/picpic2013/dlframe-front.git)。
 
 注意！由于底层使用 `ws`，对于某些浏览器，可能无法通过安全检查，从而导致前后端无法连接。请禁用相关安全策略后重试。
+
+## 其它工具
+
+### PIC_Timer
+~~~ python
+# example 1
+# function timer
+print('='*50, 'example 1', '='*50)
+@PICTimer
+def f1():
+    for _ in range(100000):
+        b = _
+
+f1()
+
+# example 2
+# with code block
+print('='*50, 'example 2', '='*50)
+with PICTimer.getTimer('example2') as t:
+    for _ in range(1, 100000):
+        if _ % 20000 == 0:
+            t.showTime()
+        bb = _
+
+# example 3
+print('='*50, 'example 3', '='*50)
+
+timer = PICTimer.getTimer('example3') 
+timer.startTimer()                    
+# or `timer = PICTimer.getTimer('example3', autoStart=True)`
+
+for idx in range(3):
+    for _ in range(1, 100000):
+        if _ % 20000 == 0:
+            timer.showTime("stage_" + str(_))
+        bb = _
+    timer.forceShowTime() # you can output results before summary
+timer.summary()
+
+# example 4
+# create sub-timer
+print('='*50, 'example 4', '='*50)
+timer = PICTimer.getTimer('example4', autoStart=True)
+for idx in range(3):
+    subTimer = timer.getTimer('sub_' + str(idx), autoStart=True)
+    for _ in range(1, 100000):
+        if _ % 20000 == 0:
+            subTimer.showTime("stage_" + str(_))
+        bb = _
+    timer.showTime()
+timer.summary()
+~~~
+
+### make_recursive_func
+~~~ python
+# dict args
+arg1 = {idx: 'arg1_k_'+str(idx) for idx in range(3)}
+arg2 = {idx: 'arg2_k_'+str(idx) for idx in range(3)}
+
+# list args
+arg1 = [_ for _ in range(10)]
+arg2 = [_ for _ in range(10)]
+
+# tuple / generator args
+arg1 = (_ for _ in range(10))
+arg2 = (_ for _ in range(10))
+
+# non-iterable args
+arg1 = 0
+arg2 = 1
+
+# mutiple args
+arg1 = {idx: ['arg1_k_'+str(idx)+'_l_'+str(_) for _ in range(2)] for idx in range(3)}
+arg2 = {idx: ['arg2_k_'+str(idx)+'_l_'+str(_) for _ in range(2)] for idx in range(3)}
+
+@make_recursive_func
+def f1(x, base):
+    return base.format(x)
+
+@make_recursive_func
+def f2(x, y, base):
+    return base.format(x, y)
+
+@make_recursive_func
+def f3(x, y, base1, base2):
+    return base1.format(x), base2.format(y)
+
+@make_multi_return_recursive_func
+def f4(x, y, base1, base2):
+    return base1.format(x), base2.format(y)
+
+res1 = f1(arg1, base="arg1: {}")
+res2 = f2(arg1, arg2, base="arg1: {}, arg2: {}")
+res3 = f3(arg1, arg2, base1="arg1: {}", base2=" arg2: {}")
+res4 = f4(arg1, arg2, base1="arg1: {}", base2=" arg2: {}")
+
+print(res1)
+print(res2)
+print(res3)
+print(res4)
+~~~
```

### Comparing `dynamic-links-0.0.6/dlframe/CalculationNode.py` & `dynamic-links-0.1.0/dlframe/CalculationNode.py`

 * *Files identical despite different names*

### Comparing `dynamic-links-0.0.6/dlframe/CalculationNodeManager.py` & `dynamic-links-0.1.0/dlframe/CalculationNodeManager.py`

 * *Files identical despite different names*

### Comparing `dynamic-links-0.0.6/dlframe/ExecutionNode.py` & `dynamic-links-0.1.0/dlframe/ExecutionNode.py`

 * *Files identical despite different names*

### Comparing `dynamic-links-0.0.6/dlframe/Logger.py` & `dynamic-links-0.1.0/dlframe/Logger.py`

 * *Files identical despite different names*

### Comparing `dynamic-links-0.0.6/dlframe/WebManager.py` & `dynamic-links-0.1.0/dlframe/WebManager.py`

 * *Files identical despite different names*

### Comparing `dynamic-links-0.0.6/dynamic_links.egg-info/PKG-INFO` & `dynamic-links-0.1.0/dynamic_links.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-links
-Version: 0.0.6
+Version: 0.1.0
 Summary: a calculation framework
 Home-page: https://github.com/picpic2013/dlframe-back
 Author: PIC
 Author-email: picpic2019@gmail.com
 License: MIT
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
@@ -243,7 +243,108 @@
 ~~~
 
 ## 关于前端
 
 本框架仅提供 WebSocket 服务，不提供页面显示。需配合[前端](https://picpic2013.github.io/dlframe-front/)使用。前端代码开源在[仓库](https://github.com/picpic2013/dlframe-front.git)。
 
 注意！由于底层使用 `ws`，对于某些浏览器，可能无法通过安全检查，从而导致前后端无法连接。请禁用相关安全策略后重试。
+
+## 其它工具
+
+### PIC_Timer
+~~~ python
+# example 1
+# function timer
+print('='*50, 'example 1', '='*50)
+@PICTimer
+def f1():
+    for _ in range(100000):
+        b = _
+
+f1()
+
+# example 2
+# with code block
+print('='*50, 'example 2', '='*50)
+with PICTimer.getTimer('example2') as t:
+    for _ in range(1, 100000):
+        if _ % 20000 == 0:
+            t.showTime()
+        bb = _
+
+# example 3
+print('='*50, 'example 3', '='*50)
+
+timer = PICTimer.getTimer('example3') 
+timer.startTimer()                    
+# or `timer = PICTimer.getTimer('example3', autoStart=True)`
+
+for idx in range(3):
+    for _ in range(1, 100000):
+        if _ % 20000 == 0:
+            timer.showTime("stage_" + str(_))
+        bb = _
+    timer.forceShowTime() # you can output results before summary
+timer.summary()
+
+# example 4
+# create sub-timer
+print('='*50, 'example 4', '='*50)
+timer = PICTimer.getTimer('example4', autoStart=True)
+for idx in range(3):
+    subTimer = timer.getTimer('sub_' + str(idx), autoStart=True)
+    for _ in range(1, 100000):
+        if _ % 20000 == 0:
+            subTimer.showTime("stage_" + str(_))
+        bb = _
+    timer.showTime()
+timer.summary()
+~~~
+
+### make_recursive_func
+~~~ python
+# dict args
+arg1 = {idx: 'arg1_k_'+str(idx) for idx in range(3)}
+arg2 = {idx: 'arg2_k_'+str(idx) for idx in range(3)}
+
+# list args
+arg1 = [_ for _ in range(10)]
+arg2 = [_ for _ in range(10)]
+
+# tuple / generator args
+arg1 = (_ for _ in range(10))
+arg2 = (_ for _ in range(10))
+
+# non-iterable args
+arg1 = 0
+arg2 = 1
+
+# mutiple args
+arg1 = {idx: ['arg1_k_'+str(idx)+'_l_'+str(_) for _ in range(2)] for idx in range(3)}
+arg2 = {idx: ['arg2_k_'+str(idx)+'_l_'+str(_) for _ in range(2)] for idx in range(3)}
+
+@make_recursive_func
+def f1(x, base):
+    return base.format(x)
+
+@make_recursive_func
+def f2(x, y, base):
+    return base.format(x, y)
+
+@make_recursive_func
+def f3(x, y, base1, base2):
+    return base1.format(x), base2.format(y)
+
+@make_multi_return_recursive_func
+def f4(x, y, base1, base2):
+    return base1.format(x), base2.format(y)
+
+res1 = f1(arg1, base="arg1: {}")
+res2 = f2(arg1, arg2, base="arg1: {}, arg2: {}")
+res3 = f3(arg1, arg2, base1="arg1: {}", base2=" arg2: {}")
+res4 = f4(arg1, arg2, base1="arg1: {}", base2=" arg2: {}")
+
+print(res1)
+print(res2)
+print(res3)
+print(res4)
+~~~
```

### Comparing `dynamic-links-0.0.6/setup.py` & `dynamic-links-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 with open(os.path.join(here, 'README.md'), 'r',encoding='UTF-8') as mdFile:
     long_description = mdFile.read()
 
 setup(
     name='dynamic-links', 
-    version='0.0.6', 
+    version='0.1.0', 
     packages=['dlframe'], 
     url='https://github.com/picpic2013/dlframe-back', 
     license='MIT', 
     author='PIC', 
     author_email='picpic2019@gmail.com', 
     description='a calculation framework', 
     long_description=long_description,
```

