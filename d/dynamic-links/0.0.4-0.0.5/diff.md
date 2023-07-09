# Comparing `tmp/dynamic-links-0.0.4.tar.gz` & `tmp/dynamic-links-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic-links-0.0.4.tar", last modified: Mon Jul  3 09:46:18 2023, max compression
+gzip compressed data, was "dynamic-links-0.0.5.tar", last modified: Sun Jul  9 04:52:45 2023, max compression
```

## Comparing `dynamic-links-0.0.4.tar` & `dynamic-links-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 pic        (501) staff       (20)        0 2023-07-03 09:46:18.585344 dynamic-links-0.0.4/
--rw-r--r--   0 pic        (501) staff       (20)     5443 2023-07-03 09:46:18.585104 dynamic-links-0.0.4/PKG-INFO
--rw-r--r--   0 pic        (501) staff       (20)     5170 2023-07-03 09:44:30.000000 dynamic-links-0.0.4/README.md
-drwxr-xr-x   0 pic        (501) staff       (20)        0 2023-07-03 09:46:18.583977 dynamic-links-0.0.4/dlframe/
--rw-r--r--   0 pic        (501) staff       (20)     2630 2023-06-27 04:59:53.000000 dynamic-links-0.0.4/dlframe/CalculationNode.py
--rw-r--r--   0 pic        (501) staff       (20)     1924 2023-06-27 03:29:25.000000 dynamic-links-0.0.4/dlframe/CalculationNodeManager.py
--rw-r--r--   0 pic        (501) staff       (20)     2048 2023-06-27 04:00:46.000000 dynamic-links-0.0.4/dlframe/ExecutionNode.py
--rw-r--r--   0 pic        (501) staff       (20)      939 2023-06-27 05:19:42.000000 dynamic-links-0.0.4/dlframe/Logger.py
--rw-r--r--   0 pic        (501) staff       (20)     5174 2023-07-03 09:42:34.000000 dynamic-links-0.0.4/dlframe/WebManager.py
--rw-r--r--   0 pic        (501) staff       (20)      141 2023-06-26 17:09:16.000000 dynamic-links-0.0.4/dlframe/__init__.py
-drwxr-xr-x   0 pic        (501) staff       (20)        0 2023-07-03 09:46:18.584667 dynamic-links-0.0.4/dynamic_links.egg-info/
--rw-r--r--   0 pic        (501) staff       (20)     5443 2023-07-03 09:46:18.000000 dynamic-links-0.0.4/dynamic_links.egg-info/PKG-INFO
--rw-r--r--   0 pic        (501) staff       (20)      348 2023-07-03 09:46:18.000000 dynamic-links-0.0.4/dynamic_links.egg-info/SOURCES.txt
--rw-r--r--   0 pic        (501) staff       (20)        1 2023-07-03 09:46:18.000000 dynamic-links-0.0.4/dynamic_links.egg-info/dependency_links.txt
--rw-r--r--   0 pic        (501) staff       (20)       30 2023-07-03 09:46:18.000000 dynamic-links-0.0.4/dynamic_links.egg-info/requires.txt
--rw-r--r--   0 pic        (501) staff       (20)        8 2023-07-03 09:46:18.000000 dynamic-links-0.0.4/dynamic_links.egg-info/top_level.txt
--rw-r--r--   0 pic        (501) staff       (20)       38 2023-07-03 09:46:18.585407 dynamic-links-0.0.4/setup.cfg
--rw-r--r--   0 pic        (501) staff       (20)      682 2023-07-03 09:44:51.000000 dynamic-links-0.0.4/setup.py
+drwxr-xr-x   0 pic        (501) staff       (20)        0 2023-07-09 04:52:45.732798 dynamic-links-0.0.5/
+-rw-r--r--   0 pic        (501) staff       (20)     6301 2023-07-09 04:52:45.732662 dynamic-links-0.0.5/PKG-INFO
+-rw-r--r--   0 pic        (501) staff       (20)     6028 2023-07-09 04:44:56.000000 dynamic-links-0.0.5/README.md
+drwxr-xr-x   0 pic        (501) staff       (20)        0 2023-07-09 04:52:45.731752 dynamic-links-0.0.5/dlframe/
+-rw-r--r--   0 pic        (501) staff       (20)     2614 2023-07-08 17:27:46.000000 dynamic-links-0.0.5/dlframe/CalculationNode.py
+-rw-r--r--   0 pic        (501) staff       (20)     3958 2023-07-09 04:46:22.000000 dynamic-links-0.0.5/dlframe/CalculationNodeManager.py
+-rw-r--r--   0 pic        (501) staff       (20)     2048 2023-06-27 04:00:46.000000 dynamic-links-0.0.5/dlframe/ExecutionNode.py
+-rw-r--r--   0 pic        (501) staff       (20)      939 2023-06-27 05:19:42.000000 dynamic-links-0.0.5/dlframe/Logger.py
+-rw-r--r--   0 pic        (501) staff       (20)     5277 2023-07-08 16:20:45.000000 dynamic-links-0.0.5/dlframe/WebManager.py
+-rw-r--r--   0 pic        (501) staff       (20)      141 2023-06-26 17:09:16.000000 dynamic-links-0.0.5/dlframe/__init__.py
+drwxr-xr-x   0 pic        (501) staff       (20)        0 2023-07-09 04:52:45.732473 dynamic-links-0.0.5/dynamic_links.egg-info/
+-rw-r--r--   0 pic        (501) staff       (20)     6301 2023-07-09 04:52:45.000000 dynamic-links-0.0.5/dynamic_links.egg-info/PKG-INFO
+-rw-r--r--   0 pic        (501) staff       (20)      348 2023-07-09 04:52:45.000000 dynamic-links-0.0.5/dynamic_links.egg-info/SOURCES.txt
+-rw-r--r--   0 pic        (501) staff       (20)        1 2023-07-09 04:52:45.000000 dynamic-links-0.0.5/dynamic_links.egg-info/dependency_links.txt
+-rw-r--r--   0 pic        (501) staff       (20)       30 2023-07-09 04:52:45.000000 dynamic-links-0.0.5/dynamic_links.egg-info/requires.txt
+-rw-r--r--   0 pic        (501) staff       (20)        8 2023-07-09 04:52:45.000000 dynamic-links-0.0.5/dynamic_links.egg-info/top_level.txt
+-rw-r--r--   0 pic        (501) staff       (20)       38 2023-07-09 04:52:45.732840 dynamic-links-0.0.5/setup.cfg
+-rw-r--r--   0 pic        (501) staff       (20)      682 2023-07-09 04:48:53.000000 dynamic-links-0.0.5/setup.py
```

### Comparing `dynamic-links-0.0.4/PKG-INFO` & `dynamic-links-0.0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: dynamic-links
-Version: 0.0.4
-Summary: a calculation framework
-Home-page: https://github.com/picpic2013/dlframe-back
-Author: PIC
-Author-email: picpic2019@gmail.com
-License: MIT
-Requires-Python: >=3.8, <4
-Description-Content-Type: text/markdown
-
 # Dynamic Links
 
 ## 安装方法
 
 ~~~bash
 pip install dynamic-links
 ~~~
@@ -36,64 +25,116 @@
 def f2(x):
     print('f2', x)
 
 # 定义元素管理器
 with WebManager() as manager:
     
     # 定义元素 + 定义元素可选的 python 对象
-    func = manager.register_element('func', {
-        'f1': f1, 
-        'f2': f2
+    func = manager.register('func', {
+        'function1': f1, 
+        'function2': f2
     })
 
     # 定义框架执行逻辑
     func('test')
 ~~~
 
 运行程序，即可通过[前端](https://picpic2013.github.io/dlframe-front/)选择执行 `f1` 或 `f2`。
 
+### 另一个例子
+
+~~~python
+from dlframe import WebManager
+
+manager = WebManager()
+
+# 定义元素可选的 python 对象
+@manager.register('func', 'function1')
+# 也可 @manager.register('func') 会自动以 f1 作为选项名称
+def f1(x):
+    print('f1', x)
+
+# 定义元素可选的 python 对象
+@manager.register('func', 'function2')
+def f2(x):
+    print('f2', x)
+
+# 定义元素管理器
+with manager:
+    
+    # 定义元素
+    func = manager['func']
+
+    # 定义框架执行逻辑
+    func('test')
+~~~
+
+与上一个例子完全等价。
+
+### 又一个例子
+~~~python
+from dlframe import WebManager
+
+def f1(x):
+    print('f1', x)
+
+def f2(x):
+    print('f2', x)
+
+# 定义元素管理器
+with WebManager() as manager:
+    # 定义元素可选的 python 对象
+    manager.register('func', 'function1', f1)
+    manager.register('func', 'function2', f2)
+
+    # 定义元素
+    func = manager['func']
+
+    # 定义框架执行逻辑
+    func('test')
+~~~
+
+与上一个例子完全等价。
+
 ### 更复杂的例子
 
 Dynamic Links 可以很方便地构建 benchmark 等应用。例如，如果要实现一个机器学习算法的简易框架，评估不同模型在不同参数下的各种指标，可以编写如下程序：
 
 ~~~python
 from dlframe import WebManager
 
 # 定义元素管理器
 with WebManager() as manager:
 
     # 定义元素 + 定义元素可选的 python 对象
-    dataset = manager.register_element('数据集', {
+    dataset = manager.register('数据集', {
         'iris': IrisDataset(), 
         'watermelon': WatermelonDataset()
     })
-    split_ratio = manager.register_element('数据分割比例', {
+    split_ratio = manager.register('数据分割比例', {
         '10%': 0.1, '30%': 0.3
     })
-    Splitter = manager.register_element('数据分割器', {
+    Splitter = manager.register('数据分割器', {
         'k-fold': KFoldSplitter, 'random': RandomSplitter
     })
-    learning_rate = manager.register_element('模型学习率', {
-        'low': 1e-3, 'high': 1e-1
-    })
-    Model = manager.register_element('模型', {
-        'cnn': CnnModel, 
-        'resnet': ResnetModel
+    Model = manager.register('模型', {
+        'decision-tree': DecisionTreeModel, 
+        'svm': SVMModel
     })
-    judger = manager.register_element('评价指标', {
+    judger = manager.register('评价指标', {
         'accuracy': AccuracyJudger(), 'f1': F1ScoreJudger()
     })
 
     # 定义框架执行逻辑
     splitter = Splitter(split_ratio)
     train_data_test_data = splitter.split(dataset)
     train_data = train_data_test_data[0]
     test_data = train_data_test_data[1]
     
-    model = Model(learning_rate)
+    model = Model()
     model.train(train_data)
     y_hat = model.test(test_data)
 
     judger.judge(y_hat, test_data)
 
 ~~~
 
@@ -190,8 +231,8 @@
     pass
 ~~~
 
 ## 关于前端
 
 本框架仅提供 WebSocket 服务，不提供页面显示。需配合[前端](https://picpic2013.github.io/dlframe-front/)使用。前端代码开源在[仓库](https://github.com/picpic2013/dlframe-front.git)。
 
-注意！由于底层使用 `ws`，对于某些浏览器，可能无法通过安全检查，从而导致前后端无法连接。请禁用相关安全策略后重试。
+注意！由于底层使用 `ws`，对于某些浏览器，可能无法通过安全检查，从而导致前后端无法连接。请禁用相关安全策略后重试。
```

### Comparing `dynamic-links-0.0.4/README.md` & `dynamic-links-0.0.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: dynamic-links
+Version: 0.0.5
+Summary: a calculation framework
+Home-page: https://github.com/picpic2013/dlframe-back
+Author: PIC
+Author-email: picpic2019@gmail.com
+License: MIT
+Requires-Python: >=3.8, <4
+Description-Content-Type: text/markdown
+
 # Dynamic Links
 
 ## 安装方法
 
 ~~~bash
 pip install dynamic-links
 ~~~
@@ -25,64 +36,116 @@
 def f2(x):
     print('f2', x)
 
 # 定义元素管理器
 with WebManager() as manager:
     
     # 定义元素 + 定义元素可选的 python 对象
-    func = manager.register_element('func', {
-        'f1': f1, 
-        'f2': f2
+    func = manager.register('func', {
+        'function1': f1, 
+        'function2': f2
     })
 
     # 定义框架执行逻辑
     func('test')
 ~~~
 
 运行程序，即可通过[前端](https://picpic2013.github.io/dlframe-front/)选择执行 `f1` 或 `f2`。
 
+### 另一个例子
+
+~~~python
+from dlframe import WebManager
+
+manager = WebManager()
+
+# 定义元素可选的 python 对象
+@manager.register('func', 'function1')
+# 也可 @manager.register('func') 会自动以 f1 作为选项名称
+def f1(x):
+    print('f1', x)
+
+# 定义元素可选的 python 对象
+@manager.register('func', 'function2')
+def f2(x):
+    print('f2', x)
+
+# 定义元素管理器
+with manager:
+    
+    # 定义元素
+    func = manager['func']
+
+    # 定义框架执行逻辑
+    func('test')
+~~~
+
+与上一个例子完全等价。
+
+### 又一个例子
+~~~python
+from dlframe import WebManager
+
+def f1(x):
+    print('f1', x)
+
+def f2(x):
+    print('f2', x)
+
+# 定义元素管理器
+with WebManager() as manager:
+    # 定义元素可选的 python 对象
+    manager.register('func', 'function1', f1)
+    manager.register('func', 'function2', f2)
+
+    # 定义元素
+    func = manager['func']
+
+    # 定义框架执行逻辑
+    func('test')
+~~~
+
+与上一个例子完全等价。
+
 ### 更复杂的例子
 
 Dynamic Links 可以很方便地构建 benchmark 等应用。例如，如果要实现一个机器学习算法的简易框架，评估不同模型在不同参数下的各种指标，可以编写如下程序：
 
 ~~~python
 from dlframe import WebManager
 
 # 定义元素管理器
 with WebManager() as manager:
 
     # 定义元素 + 定义元素可选的 python 对象
-    dataset = manager.register_element('数据集', {
+    dataset = manager.register('数据集', {
         'iris': IrisDataset(), 
         'watermelon': WatermelonDataset()
     })
-    split_ratio = manager.register_element('数据分割比例', {
+    split_ratio = manager.register('数据分割比例', {
         '10%': 0.1, '30%': 0.3
     })
-    Splitter = manager.register_element('数据分割器', {
+    Splitter = manager.register('数据分割器', {
         'k-fold': KFoldSplitter, 'random': RandomSplitter
     })
-    learning_rate = manager.register_element('模型学习率', {
-        'low': 1e-3, 'high': 1e-1
-    })
-    Model = manager.register_element('模型', {
-        'cnn': CnnModel, 
-        'resnet': ResnetModel
+    Model = manager.register('模型', {
+        'decision-tree': DecisionTreeModel, 
+        'svm': SVMModel
     })
-    judger = manager.register_element('评价指标', {
+    judger = manager.register('评价指标', {
         'accuracy': AccuracyJudger(), 'f1': F1ScoreJudger()
     })
 
     # 定义框架执行逻辑
     splitter = Splitter(split_ratio)
     train_data_test_data = splitter.split(dataset)
     train_data = train_data_test_data[0]
     test_data = train_data_test_data[1]
     
-    model = Model(learning_rate)
+    model = Model()
     model.train(train_data)
     y_hat = model.test(test_data)
 
     judger.judge(y_hat, test_data)
 
 ~~~
 
@@ -179,8 +242,8 @@
     pass
 ~~~
 
 ## 关于前端
 
 本框架仅提供 WebSocket 服务，不提供页面显示。需配合[前端](https://picpic2013.github.io/dlframe-front/)使用。前端代码开源在[仓库](https://github.com/picpic2013/dlframe-front.git)。
 
-注意！由于底层使用 `ws`，对于某些浏览器，可能无法通过安全检查，从而导致前后端无法连接。请禁用相关安全策略后重试。
+注意！由于底层使用 `ws`，对于某些浏览器，可能无法通过安全检查，从而导致前后端无法连接。请禁用相关安全策略后重试。
```

### Comparing `dynamic-links-0.0.4/dlframe/CalculationNode.py` & `dynamic-links-0.0.5/dlframe/CalculationNode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 class CalculationNode:
-    def __init__(self, attr_name: str, node_manager, last_node=None, element_dict: dict=None, is_root_node=False, *args, **kwargs) -> None:
+    def __init__(self, attr_name: str, node_manager, last_node=None, element_dict: dict=None, is_root_node=False) -> None:
         self.is_root_node = is_root_node
         
         self.attr_name = attr_name
         self.last_nodes = [last_node] if last_node is not None else []
         self.next_nodes = []
         self.node_manager = node_manager
         self.element_dict = element_dict
         
         self.is_function = False
         self.is_init_function = False
         self.function_args = []
         self.function_kwargs = {}
 
-        self.node_manager.register_node(self)
+        self.node_manager._register_node(self)
     
     def __call__(self, *args, **kwargs):
         all_args = []
         for arg in args:
             if type(arg) is not CalculationNode:
                 arg = CalculationNode(str(arg), self.node_manager, None, {str(arg): arg}, is_root_node=True)
             all_args.append(arg)
```

### Comparing `dynamic-links-0.0.4/dlframe/ExecutionNode.py` & `dynamic-links-0.0.5/dlframe/ExecutionNode.py`

 * *Files identical despite different names*

### Comparing `dynamic-links-0.0.4/dlframe/Logger.py` & `dynamic-links-0.0.5/dlframe/Logger.py`

 * *Files identical despite different names*

### Comparing `dynamic-links-0.0.4/dlframe/WebManager.py` & `dynamic-links-0.0.5/dlframe/WebManager.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,15 +38,19 @@
         return self
     
     def __exit__(self, exc_type, exc_val, exc_tb):
         if exc_type is not None:
             raise exc_val
         self.start(self.host, self.port)
 
-    def start(self, host='0.0.0.0', port=8765) -> None:
+    def start(self, host=None, port=None) -> None:
+        if host is None:
+            host = self.host
+        if port is None:
+            port = self.port
         event_loop = asyncio.new_event_loop()
         asyncio.set_event_loop(event_loop)
         async def onRecv(socket, path):
             msgIdx = -1
             sendSocket = SendSocket(socket)
             async for message in socket:
                 msgIdx += 1
```

### Comparing `dynamic-links-0.0.4/dynamic_links.egg-info/PKG-INFO` & `dynamic-links-0.0.5/dynamic_links.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-links
-Version: 0.0.4
+Version: 0.0.5
 Summary: a calculation framework
 Home-page: https://github.com/picpic2013/dlframe-back
 Author: PIC
 Author-email: picpic2019@gmail.com
 License: MIT
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
@@ -36,64 +36,116 @@
 def f2(x):
     print('f2', x)
 
 # 定义元素管理器
 with WebManager() as manager:
     
     # 定义元素 + 定义元素可选的 python 对象
-    func = manager.register_element('func', {
-        'f1': f1, 
-        'f2': f2
+    func = manager.register('func', {
+        'function1': f1, 
+        'function2': f2
     })
 
     # 定义框架执行逻辑
     func('test')
 ~~~
 
 运行程序，即可通过[前端](https://picpic2013.github.io/dlframe-front/)选择执行 `f1` 或 `f2`。
 
+### 另一个例子
+
+~~~python
+from dlframe import WebManager
+
+manager = WebManager()
+
+# 定义元素可选的 python 对象
+@manager.register('func', 'function1')
+# 也可 @manager.register('func') 会自动以 f1 作为选项名称
+def f1(x):
+    print('f1', x)
+
+# 定义元素可选的 python 对象
+@manager.register('func', 'function2')
+def f2(x):
+    print('f2', x)
+
+# 定义元素管理器
+with manager:
+    
+    # 定义元素
+    func = manager['func']
+
+    # 定义框架执行逻辑
+    func('test')
+~~~
+
+与上一个例子完全等价。
+
+### 又一个例子
+~~~python
+from dlframe import WebManager
+
+def f1(x):
+    print('f1', x)
+
+def f2(x):
+    print('f2', x)
+
+# 定义元素管理器
+with WebManager() as manager:
+    # 定义元素可选的 python 对象
+    manager.register('func', 'function1', f1)
+    manager.register('func', 'function2', f2)
+
+    # 定义元素
+    func = manager['func']
+
+    # 定义框架执行逻辑
+    func('test')
+~~~
+
+与上一个例子完全等价。
+
 ### 更复杂的例子
 
 Dynamic Links 可以很方便地构建 benchmark 等应用。例如，如果要实现一个机器学习算法的简易框架，评估不同模型在不同参数下的各种指标，可以编写如下程序：
 
 ~~~python
 from dlframe import WebManager
 
 # 定义元素管理器
 with WebManager() as manager:
 
     # 定义元素 + 定义元素可选的 python 对象
-    dataset = manager.register_element('数据集', {
+    dataset = manager.register('数据集', {
         'iris': IrisDataset(), 
         'watermelon': WatermelonDataset()
     })
-    split_ratio = manager.register_element('数据分割比例', {
+    split_ratio = manager.register('数据分割比例', {
         '10%': 0.1, '30%': 0.3
     })
-    Splitter = manager.register_element('数据分割器', {
+    Splitter = manager.register('数据分割器', {
         'k-fold': KFoldSplitter, 'random': RandomSplitter
     })
-    learning_rate = manager.register_element('模型学习率', {
-        'low': 1e-3, 'high': 1e-1
-    })
-    Model = manager.register_element('模型', {
-        'cnn': CnnModel, 
-        'resnet': ResnetModel
+    Model = manager.register('模型', {
+        'decision-tree': DecisionTreeModel, 
+        'svm': SVMModel
     })
-    judger = manager.register_element('评价指标', {
+    judger = manager.register('评价指标', {
         'accuracy': AccuracyJudger(), 'f1': F1ScoreJudger()
     })
 
     # 定义框架执行逻辑
     splitter = Splitter(split_ratio)
     train_data_test_data = splitter.split(dataset)
     train_data = train_data_test_data[0]
     test_data = train_data_test_data[1]
     
-    model = Model(learning_rate)
+    model = Model()
     model.train(train_data)
     y_hat = model.test(test_data)
 
     judger.judge(y_hat, test_data)
 
 ~~~
```

### Comparing `dynamic-links-0.0.4/setup.py` & `dynamic-links-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 with open(os.path.join(here, 'README.md'), 'r',encoding='UTF-8') as mdFile:
     long_description = mdFile.read()
 
 setup(
     name='dynamic-links', 
-    version='0.0.4', 
+    version='0.0.5', 
     packages=['dlframe'], 
     url='https://github.com/picpic2013/dlframe-back', 
     license='MIT', 
     author='PIC', 
     author_email='picpic2019@gmail.com', 
     description='a calculation framework', 
     long_description=long_description,
```

