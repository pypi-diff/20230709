# Comparing `tmp/nb_log_file_handler-0.1.tar.gz` & `tmp/nb_log_file_handler-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nb_log_file_handler-0.1.tar", last modified: Sun Jul  9 14:25:00 2023, max compression
+gzip compressed data, was "nb_log_file_handler-0.2.tar", last modified: Sun Jul  9 14:34:47 2023, max compression
```

## Comparing `nb_log_file_handler-0.1.tar` & `nb_log_file_handler-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 14:25:00.873056 nb_log_file_handler-0.1/
--rw-rw-rw-   0        0        0     5108 2023-07-09 14:25:00.872049 nb_log_file_handler-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4274 2023-07-09 14:24:32.000000 nb_log_file_handler-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-09 14:25:00.849039 nb_log_file_handler-0.1/nb_log_file_handler/
--rw-rw-rw-   0        0        0      769 2023-07-09 13:51:38.000000 nb_log_file_handler-0.1/nb_log_file_handler/__init__.py
--rw-rw-rw-   0        0        0     6282 2023-07-09 13:55:16.000000 nb_log_file_handler-0.1/nb_log_file_handler/rotate_file_writter.py
-drwxrwxrwx   0        0        0        0 2023-07-09 14:25:00.868040 nb_log_file_handler-0.1/nb_log_file_handler.egg-info/
--rw-rw-rw-   0        0        0     5108 2023-07-09 14:25:00.000000 nb_log_file_handler-0.1/nb_log_file_handler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-07-09 14:25:00.000000 nb_log_file_handler-0.1/nb_log_file_handler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 14:25:00.000000 nb_log_file_handler-0.1/nb_log_file_handler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-07-09 14:25:00.000000 nb_log_file_handler-0.1/nb_log_file_handler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-09 14:25:00.874044 nb_log_file_handler-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1937 2023-07-09 14:24:32.000000 nb_log_file_handler-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 14:34:47.915376 nb_log_file_handler-0.2/
+-rw-rw-rw-   0        0        0     5788 2023-07-09 14:34:47.913352 nb_log_file_handler-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4954 2023-07-09 14:34:19.000000 nb_log_file_handler-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 14:34:47.879331 nb_log_file_handler-0.2/nb_log_file_handler/
+-rw-rw-rw-   0        0        0      769 2023-07-09 13:51:38.000000 nb_log_file_handler-0.2/nb_log_file_handler/__init__.py
+-rw-rw-rw-   0        0        0     6282 2023-07-09 13:55:16.000000 nb_log_file_handler-0.2/nb_log_file_handler/rotate_file_writter.py
+drwxrwxrwx   0        0        0        0 2023-07-09 14:34:47.895344 nb_log_file_handler-0.2/nb_log_file_handler.egg-info/
+-rw-rw-rw-   0        0        0     5788 2023-07-09 14:34:47.000000 nb_log_file_handler-0.2/nb_log_file_handler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-07-09 14:34:47.000000 nb_log_file_handler-0.2/nb_log_file_handler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 14:34:47.000000 nb_log_file_handler-0.2/nb_log_file_handler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-07-09 14:34:47.000000 nb_log_file_handler-0.2/nb_log_file_handler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-09 14:34:47.915376 nb_log_file_handler-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1938 2023-07-09 14:34:42.000000 nb_log_file_handler-0.2/setup.py
```

### Comparing `nb_log_file_handler-0.1/PKG-INFO` & `nb_log_file_handler-0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb_log_file_handler
-Version: 0.1
+Version: 0.2
 Summary: multi process safe log file handler,both time and size rotate，benchmark fast than concurrent_log_handler 100 times
 Home-page: https://github.com/ydf0509/nb_log_file_handler
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
@@ -20,21 +20,28 @@
 Description-Content-Type: text/markdown
 
 # nb_log_file_handler
 
 multi process safe log file handler,both time and size rotate，benchmark fast than concurrent_log_handler 100 times
 
 
-nb_log_file_handler 是多进程安全切割，同时按时间和大小切割的FileHandler
+nb_log_file_handler 是多进程安全切割，同时按时间和大小切割的FileHandler,性能远超 concurrent_log_handler.ConcurrentRotatingFileHandler
 
 
 ## 安装
 
 pip install nb_log_file_handler
 
+## nb_log_file_handler 实现原理，
+
+nb_log_file_handler 在win上采用每隔0.1秒批量写入文件，atexit钩子对程序即将结束后的剩余待写入的消息写到文件中。
+linux的文件io性能本身比较好，加上fork 子进程不支持 atexit 触发执行，所以linux上使用单个消息就写入。
+
+nb_log_file_handler 性能远超 concurrent_log_handler.ConcurrentRotatingFileHandler
+
 ## 1、nb_log_file_handler使用方式：
 
 代码如下，和filehandler用法相同，导入 NbLogFileHandler
 
 ```python
 import multiprocessing
 import logging
@@ -53,16 +60,20 @@
 
 def f():
     for i in range(10000):
         logger.info(f'{i}aaaaa'*20)
 ```
 
 
+## 2、各种按文件/时间大小切割的fileHander对比，
 
-## 2、对比logging内置的 logging.handlers.RotatingFileHandler
+为了测试多进程按文件大小切割安全的复现，所以所有maxBytes按照1000*1000字节，即1M进行切割。
+
+
+### 2.1、对比logging内置的 logging.handlers.RotatingFileHandler
 
 logging.handlers.RotatingFileHandler 多进程按大小切割完全不可行，切割时候疯狂报错
 
 ```python
 
 import multiprocessing
 import logging.handlers
@@ -98,17 +109,17 @@
 会疯狂报错，因为进程a在达到大小切割改名日志文件时候，进程b并不知情，报错如下：
 ```
 PermissionError: [WinError 32] 另一个程序正在使用此文件，进程无法访问。: 'D:\\codes\\nb_log_file_handler\\tests_nb_log_file_handler\\xx4.log' -> 'D:\\codes\\nb_log_file_handler\\tests_nb_log_file_handler\\xx4.log.1'
 ```
 
 所以一般多进程写入同一个日志文件，并支持切割，那么久不能使用logging自带的RotatingFileHandler，要使用第三方包的filehandler。
 
-## 3、对比小有名气的多进程切割安全的三方包 concurrent_log_handler
+### 2.2、对比小有名气的多进程切割安全的三方包 concurrent_log_handler
 
-from concurrent_log_handler import ConcurrentRotatingFileHandler
+concurrent_log_handler.ConcurrentRotatingFileHandler
 
 ```python
 
 
 import multiprocessing
 import logging
 import time
@@ -138,15 +149,15 @@
     for p in ps:
         p.join()
     print(time.time()-t1)
 ```
 
 concurrent_log_handler这个包在windows上性能无法忍受，10进程写入10000次需要263秒，性能惨不忍睹。这个包在linux上性能还可以接受。
 
-## 4、 nb_log_file_handler.NbLogFileHandler 按散件和大小多进程安全切割，性能远远的暴击 concurrent_log_handler
+### 2.3、 nb_log_file_handler.NbLogFileHandler 按时间和大小多进程安全切割，性能远远的暴击 concurrent_log_handler
 
 ```python
 
 
 import multiprocessing
 import logging
 import time
```

### Comparing `nb_log_file_handler-0.1/README.md` & `nb_log_file_handler-0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 # nb_log_file_handler
 
 multi process safe log file handler,both time and size rotate，benchmark fast than concurrent_log_handler 100 times
 
 
-nb_log_file_handler 是多进程安全切割，同时按时间和大小切割的FileHandler
+nb_log_file_handler 是多进程安全切割，同时按时间和大小切割的FileHandler,性能远超 concurrent_log_handler.ConcurrentRotatingFileHandler
 
 
 ## 安装
 
 pip install nb_log_file_handler
 
+## nb_log_file_handler 实现原理，
+
+nb_log_file_handler 在win上采用每隔0.1秒批量写入文件，atexit钩子对程序即将结束后的剩余待写入的消息写到文件中。
+linux的文件io性能本身比较好，加上fork 子进程不支持 atexit 触发执行，所以linux上使用单个消息就写入。
+
+nb_log_file_handler 性能远超 concurrent_log_handler.ConcurrentRotatingFileHandler
+
 ## 1、nb_log_file_handler使用方式：
 
 代码如下，和filehandler用法相同，导入 NbLogFileHandler
 
 ```python
 import multiprocessing
 import logging
@@ -32,16 +39,20 @@
 
 def f():
     for i in range(10000):
         logger.info(f'{i}aaaaa'*20)
 ```
 
 
+## 2、各种按文件/时间大小切割的fileHander对比，
 
-## 2、对比logging内置的 logging.handlers.RotatingFileHandler
+为了测试多进程按文件大小切割安全的复现，所以所有maxBytes按照1000*1000字节，即1M进行切割。
+
+
+### 2.1、对比logging内置的 logging.handlers.RotatingFileHandler
 
 logging.handlers.RotatingFileHandler 多进程按大小切割完全不可行，切割时候疯狂报错
 
 ```python
 
 import multiprocessing
 import logging.handlers
@@ -77,17 +88,17 @@
 会疯狂报错，因为进程a在达到大小切割改名日志文件时候，进程b并不知情，报错如下：
 ```
 PermissionError: [WinError 32] 另一个程序正在使用此文件，进程无法访问。: 'D:\\codes\\nb_log_file_handler\\tests_nb_log_file_handler\\xx4.log' -> 'D:\\codes\\nb_log_file_handler\\tests_nb_log_file_handler\\xx4.log.1'
 ```
 
 所以一般多进程写入同一个日志文件，并支持切割，那么久不能使用logging自带的RotatingFileHandler，要使用第三方包的filehandler。
 
-## 3、对比小有名气的多进程切割安全的三方包 concurrent_log_handler
+### 2.2、对比小有名气的多进程切割安全的三方包 concurrent_log_handler
 
-from concurrent_log_handler import ConcurrentRotatingFileHandler
+concurrent_log_handler.ConcurrentRotatingFileHandler
 
 ```python
 
 
 import multiprocessing
 import logging
 import time
@@ -117,15 +128,15 @@
     for p in ps:
         p.join()
     print(time.time()-t1)
 ```
 
 concurrent_log_handler这个包在windows上性能无法忍受，10进程写入10000次需要263秒，性能惨不忍睹。这个包在linux上性能还可以接受。
 
-## 4、 nb_log_file_handler.NbLogFileHandler 按散件和大小多进程安全切割，性能远远的暴击 concurrent_log_handler
+### 2.3、 nb_log_file_handler.NbLogFileHandler 按时间和大小多进程安全切割，性能远远的暴击 concurrent_log_handler
 
 ```python
 
 
 import multiprocessing
 import logging
 import time
```

### Comparing `nb_log_file_handler-0.1/nb_log_file_handler/__init__.py` & `nb_log_file_handler-0.2/nb_log_file_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `nb_log_file_handler-0.1/nb_log_file_handler/rotate_file_writter.py` & `nb_log_file_handler-0.2/nb_log_file_handler/rotate_file_writter.py`

 * *Files identical despite different names*

### Comparing `nb_log_file_handler-0.1/nb_log_file_handler.egg-info/PKG-INFO` & `nb_log_file_handler-0.2/nb_log_file_handler.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-log-file-handler
-Version: 0.1
+Version: 0.2
 Summary: multi process safe log file handler,both time and size rotate，benchmark fast than concurrent_log_handler 100 times
 Home-page: https://github.com/ydf0509/nb_log_file_handler
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
@@ -20,21 +20,28 @@
 Description-Content-Type: text/markdown
 
 # nb_log_file_handler
 
 multi process safe log file handler,both time and size rotate，benchmark fast than concurrent_log_handler 100 times
 
 
-nb_log_file_handler 是多进程安全切割，同时按时间和大小切割的FileHandler
+nb_log_file_handler 是多进程安全切割，同时按时间和大小切割的FileHandler,性能远超 concurrent_log_handler.ConcurrentRotatingFileHandler
 
 
 ## 安装
 
 pip install nb_log_file_handler
 
+## nb_log_file_handler 实现原理，
+
+nb_log_file_handler 在win上采用每隔0.1秒批量写入文件，atexit钩子对程序即将结束后的剩余待写入的消息写到文件中。
+linux的文件io性能本身比较好，加上fork 子进程不支持 atexit 触发执行，所以linux上使用单个消息就写入。
+
+nb_log_file_handler 性能远超 concurrent_log_handler.ConcurrentRotatingFileHandler
+
 ## 1、nb_log_file_handler使用方式：
 
 代码如下，和filehandler用法相同，导入 NbLogFileHandler
 
 ```python
 import multiprocessing
 import logging
@@ -53,16 +60,20 @@
 
 def f():
     for i in range(10000):
         logger.info(f'{i}aaaaa'*20)
 ```
 
 
+## 2、各种按文件/时间大小切割的fileHander对比，
 
-## 2、对比logging内置的 logging.handlers.RotatingFileHandler
+为了测试多进程按文件大小切割安全的复现，所以所有maxBytes按照1000*1000字节，即1M进行切割。
+
+
+### 2.1、对比logging内置的 logging.handlers.RotatingFileHandler
 
 logging.handlers.RotatingFileHandler 多进程按大小切割完全不可行，切割时候疯狂报错
 
 ```python
 
 import multiprocessing
 import logging.handlers
@@ -98,17 +109,17 @@
 会疯狂报错，因为进程a在达到大小切割改名日志文件时候，进程b并不知情，报错如下：
 ```
 PermissionError: [WinError 32] 另一个程序正在使用此文件，进程无法访问。: 'D:\\codes\\nb_log_file_handler\\tests_nb_log_file_handler\\xx4.log' -> 'D:\\codes\\nb_log_file_handler\\tests_nb_log_file_handler\\xx4.log.1'
 ```
 
 所以一般多进程写入同一个日志文件，并支持切割，那么久不能使用logging自带的RotatingFileHandler，要使用第三方包的filehandler。
 
-## 3、对比小有名气的多进程切割安全的三方包 concurrent_log_handler
+### 2.2、对比小有名气的多进程切割安全的三方包 concurrent_log_handler
 
-from concurrent_log_handler import ConcurrentRotatingFileHandler
+concurrent_log_handler.ConcurrentRotatingFileHandler
 
 ```python
 
 
 import multiprocessing
 import logging
 import time
@@ -138,15 +149,15 @@
     for p in ps:
         p.join()
     print(time.time()-t1)
 ```
 
 concurrent_log_handler这个包在windows上性能无法忍受，10进程写入10000次需要263秒，性能惨不忍睹。这个包在linux上性能还可以接受。
 
-## 4、 nb_log_file_handler.NbLogFileHandler 按散件和大小多进程安全切割，性能远远的暴击 concurrent_log_handler
+### 2.3、 nb_log_file_handler.NbLogFileHandler 按时间和大小多进程安全切割，性能远远的暴击 concurrent_log_handler
 
 ```python
 
 
 import multiprocessing
 import logging
 import time
```

### Comparing `nb_log_file_handler-0.1/setup.py` & `nb_log_file_handler-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 install_requires = [
 
 ]
 
 
 setup(
     name='nb_log_file_handler',  #
-    version="0.1",
+    version="0.2",
     description=(
         'multi process safe log file handler,both time and size rotate，benchmark fast than concurrent_log_handler 100 times'
     ),
     keywords=["logging", "logger", "multiprocess file handler", ],
     # long_description=open('README.md', 'r',encoding='utf8').read(),
     long_description_content_type="text/markdown",
     long_description=open(filepath, 'r', encoding='utf8').read(),
@@ -50,14 +50,14 @@
 """
 打包上传
 python setup.py sdist upload -r pypi
 
 
 
 
-python setup.py sdist & python -m  twine upload dist/nb_log_file_handler-0.1.tar.gz
+python setup.py sdist && python -m  twine upload dist/nb_log_file_handler-0.2.tar.gz
 
 twine upload dist/*
 
 
 python -m pip install nb_log_file_handler --upgrade -i https://pypi.org/simple   # 及时的方式，不用等待 阿里云 豆瓣 同步
 """
```

