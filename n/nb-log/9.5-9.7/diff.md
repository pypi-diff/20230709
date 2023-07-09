# Comparing `tmp/nb_log-9.5.tar.gz` & `tmp/nb_log-9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nb_log-9.5.tar", last modified: Mon Jul  3 14:55:46 2023, max compression
+gzip compressed data, was "nb_log-9.7.tar", last modified: Sun Jul  9 07:29:18 2023, max compression
```

## Comparing `nb_log-9.5.tar` & `nb_log-9.7.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 14:55:45.996933 nb_log-9.5/
--rw-rw-rw-   0        0        0    30393 2023-07-03 14:55:45.994934 nb_log-9.5/PKG-INFO
--rw-rw-rw-   0        0        0    29460 2023-07-03 13:46:53.000000 nb_log-9.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 14:55:45.969928 nb_log-9.5/nb_log/
--rw-rw-rw-   0        0        0     3192 2023-07-02 07:24:38.000000 nb_log-9.5/nb_log/__init__.py
--rw-rw-rw-   0        0        0     2990 2023-07-03 14:54:51.000000 nb_log-9.5/nb_log/file_write.py
--rw-rw-rw-   0        0        0    50714 2023-07-03 14:15:08.000000 nb_log-9.5/nb_log/handlers.py
--rw-rw-rw-   0        0        0    49868 2022-09-12 12:13:59.000000 nb_log-9.5/nb_log/handlers0000.py
--rw-rw-rw-   0        0        0    30839 2023-07-03 14:18:09.000000 nb_log-9.5/nb_log/log_manager.py
--rw-rw-rw-   0        0        0     6409 2023-07-02 07:15:56.000000 nb_log-9.5/nb_log/monkey_print.py
--rw-rw-rw-   0        0        0      853 2023-07-01 05:26:36.000000 nb_log-9.5/nb_log/monkey_std_filter_words.py
--rw-rw-rw-   0        0        0      819 2023-07-02 07:15:56.000000 nb_log-9.5/nb_log/monkey_sys_std.py
--rw-rw-rw-   0        0        0    10586 2023-07-03 14:31:09.000000 nb_log-9.5/nb_log/nb_log_config_default.py
--rw-rw-rw-   0        0        0     4328 2023-06-30 14:23:45.000000 nb_log-9.5/nb_log/nb_logger.py
--rw-rw-rw-   0        0        0     6066 2023-07-03 14:08:57.000000 nb_log-9.5/nb_log/set_nb_log_config.py
--rw-rw-rw-   0        0        0     1854 2023-07-03 14:03:16.000000 nb_log-9.5/nb_log/simple_print.py
-drwxrwxrwx   0        0        0        0 2023-07-03 14:55:45.990934 nb_log-9.5/nb_log.egg-info/
--rw-rw-rw-   0        0        0    30393 2023-07-03 14:55:45.000000 nb_log-9.5/nb_log.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      456 2023-07-03 14:55:45.000000 nb_log-9.5/nb_log.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 14:55:45.000000 nb_log-9.5/nb_log.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      210 2023-07-03 14:55:45.000000 nb_log-9.5/nb_log.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-03 14:55:45.000000 nb_log-9.5/nb_log.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 14:55:45.997936 nb_log-9.5/setup.cfg
--rw-rw-rw-   0        0        0     2376 2023-07-03 14:55:42.000000 nb_log-9.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 07:29:18.504090 nb_log-9.7/
+-rw-rw-rw-   0        0        0    30393 2023-07-09 07:29:18.502088 nb_log-9.7/PKG-INFO
+-rw-rw-rw-   0        0        0    29460 2023-07-03 13:46:53.000000 nb_log-9.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 07:29:18.481082 nb_log-9.7/nb_log/
+-rw-rw-rw-   0        0        0     3192 2023-07-02 07:24:38.000000 nb_log-9.7/nb_log/__init__.py
+-rw-rw-rw-   0        0        0     3423 2023-07-06 13:56:36.000000 nb_log-9.7/nb_log/file_write.py
+-rw-rw-rw-   0        0        0    51493 2023-07-09 06:01:38.000000 nb_log-9.7/nb_log/handlers.py
+-rw-rw-rw-   0        0        0    49868 2022-09-12 12:13:59.000000 nb_log-9.7/nb_log/handlers0000.py
+-rw-rw-rw-   0        0        0    31273 2023-07-09 05:58:10.000000 nb_log-9.7/nb_log/log_manager.py
+-rw-rw-rw-   0        0        0     6764 2023-07-09 06:17:13.000000 nb_log-9.7/nb_log/monkey_print.py
+-rw-rw-rw-   0        0        0      853 2023-07-01 05:26:36.000000 nb_log-9.7/nb_log/monkey_std_filter_words.py
+-rw-rw-rw-   0        0        0     2350 2023-07-09 06:34:51.000000 nb_log-9.7/nb_log/monkey_sys_std.py
+-rw-rw-rw-   0        0        0    10816 2023-07-09 07:23:29.000000 nb_log-9.7/nb_log/nb_log_config_default.py
+-rw-rw-rw-   0        0        0     5127 2023-07-06 13:55:43.000000 nb_log-9.7/nb_log/nb_logger.py
+-rw-rw-rw-   0        0        0     6260 2023-07-09 07:15:13.000000 nb_log-9.7/nb_log/rotate_file_writter.py
+-rw-rw-rw-   0        0        0     6066 2023-07-03 14:08:57.000000 nb_log-9.7/nb_log/set_nb_log_config.py
+-rw-rw-rw-   0        0        0     2067 2023-07-09 04:17:03.000000 nb_log-9.7/nb_log/simple_print.py
+drwxrwxrwx   0        0        0        0 2023-07-09 07:29:18.499089 nb_log-9.7/nb_log.egg-info/
+-rw-rw-rw-   0        0        0    30393 2023-07-09 07:29:18.000000 nb_log-9.7/nb_log.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      486 2023-07-09 07:29:18.000000 nb_log-9.7/nb_log.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 07:29:18.000000 nb_log-9.7/nb_log.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      210 2023-07-09 07:29:18.000000 nb_log-9.7/nb_log.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-09 07:29:18.000000 nb_log-9.7/nb_log.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-09 07:29:18.505088 nb_log-9.7/setup.cfg
+-rw-rw-rw-   0        0        0     2376 2023-07-09 07:29:09.000000 nb_log-9.7/setup.py
```

### Comparing `nb_log-9.5/PKG-INFO` & `nb_log-9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb_log
-Version: 9.5
+Version: 9.7
 Summary: very sharp color display,monkey patch bulitin print  and high-performance multiprocess safe roating file handler,other handlers includeing dintalk ,email,kafka,elastic and so on 
 Home-page: https://github.com/ydf0509/nb_log
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
```

### Comparing `nb_log-9.5/README.md` & `nb_log-9.7/README.md`

 * *Files identical despite different names*

### Comparing `nb_log-9.5/nb_log/__init__.py` & `nb_log-9.7/nb_log/__init__.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.5/nb_log/file_write.py` & `nb_log-9.7/nb_log/file_write.py`

 * *Files 8% similar despite different names*

```diff
@@ -77,8 +77,13 @@
 
 class StdFileWritter(FileWritter):
     _lock = threading.Lock()
     need_write_2_file = False if nb_log_config_default.SYS_STD_FILE_NAME in (None, '') else True
 
 
 if __name__ == '__main__':
-    FileWritter('test_file', '/test_dir2').write_2_file('哈哈哈')
+    fw = FileWritter('test_file3', '/test_dir2')
+    t1 = time.time()
+    for i in range(10000):
+        fw.write_2_file(''' 11:18:13  "D:\codes\nb_log\tests\test_use_curretn_dir_config\test_s_print2.py:9"  <module>  2023-07-05 10:48:35 - lalala - "D:/codes/funboost/test_frame/test_nb_log/log_example.py:15" - <module> - ERROR - 粉红色说明代码有错误。 粉红色说明代码有错误。 粉红色说明代码有错误。 粉红色说明代码有错误。
+  ''')
+    print(time.time()-t1)
```

### Comparing `nb_log-9.5/nb_log/handlers.py` & `nb_log-9.7/nb_log/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,41 +8,43 @@
 import os
 import threading
 import traceback
 import socket
 import datetime
 import json
 import time
+import typing
 
 from collections import OrderedDict
 from pathlib import Path
 from queue import Queue, Empty
 # noinspection PyPackageRequirements
 from kafka import KafkaProducer
 # from elasticsearch import Elasticsearch, helpers  # 性能导入时间消耗2秒,实例化时候再导入。
 from threading import Lock, Thread
 import pymongo
-from elasticsearch import Elasticsearch
 import requests
 import logging
 from logging import handlers
 from concurrent_log_handler import ConcurrentRotatingFileHandler  # 需要安装。concurrent-log-handler==0.9.1
 # noinspection PyUnresolvedReferences
 from logging.handlers import WatchedFileHandler
 # noinspection PyPackageRequirements
 from nb_filelock import FileLock
 from pythonjsonlogger.jsonlogger import JsonFormatter
 from nb_log import nb_log_config_default
-from nb_log import nb_print
+from nb_log.monkey_print import nb_print
+from nb_log.rotate_file_writter import OsFileWritter
 
 very_nb_print = nb_print
 os_name = os.name
 
 host_name = socket.gethostname()
 
+
 class MongoHandler(logging.Handler):
     """
     一个mongodb的log handler,支持日志按loggername创建不同的集合写入mongodb中
     """
 
     # msg_pattern = re.compile('(\d+-\d+-\d+ \d+:\d+:\d+) - (\S*?) - (\S*?) - (\d+) - (\S*?) - ([\s\S]*)')
 
@@ -327,15 +329,17 @@
     def __init__(self, elastic_hosts: list, elastic_port, index_prefix='pylog-'):
         """
         :param elastic_hosts:  es的ip地址，数组类型
         :param elastic_port：  es端口
         :param index_prefix: index名字前缀。
         """
         logging.Handler.__init__(self)
-        self._es_client = Elasticsearch(elastic_hosts,)
+        from elasticsearch import Elasticsearch, helpers
+        self._helpers = helpers
+        self._es_client = Elasticsearch(elastic_hosts, )
         self._index_prefix = index_prefix
         t = Thread(target=self._do_bulk_op)
         t.setDaemon(True)
         t.start()
 
     @classmethod
     def __add_task_to_bulk(cls, task):
@@ -354,15 +358,15 @@
             try:
                 if self.__class__.task_queue.qsize() > 10000:
                     very_nb_print('防止意外日志积累太多了，不插入es了。')
                     self.__clear_bulk_task()
                     return
                 tasks = list(self.__class__.task_queue.queue)
                 self.__clear_bulk_task()
-                helpers.bulk(self._es_client, tasks)
+                self._helpers.bulk(self._es_client, tasks)
                 self.__class__.last_es_op_time = time.time()
             except Exception as e:
                 very_nb_print(e)
             finally:
                 time.sleep(self.ES_INTERVAL_SECONDS)
 
     def emit(self, record):
@@ -650,29 +654,29 @@
 
     @classmethod
     def _emit_all_file_handler(cls):
         while True:
             for hr in cls.file_handler_list:
                 # very_nb_print(hr.buffer_msgs_queue.qsize())
                 hr.rollover_and_do_write()
-            time.sleep(1)
+            time.sleep(0.1)
 
     @classmethod
     def start_emit_all_file_handler(cls):
         pass
         Thread(target=cls._emit_all_file_handler, daemon=True).start()
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.buffer_msgs_queue = Queue()
+        self.buffer_msgs_queue = queue.SimpleQueue()
         atexit.register(self._when_exit)  # 如果程序属于立马就能结束的，需要在程序结束前执行这个钩子，防止不到最后一秒的日志没记录到。
         self.file_handler_list.append(self)
         if not self.has_start_emit_all_file_handler:
-            self.start_emit_all_file_handler()
             self.__class__.has_start_emit_all_file_handler = True
+            self.start_emit_all_file_handler()
 
     def _when_exit(self):
         pass
         self.rollover_and_do_write()
 
     def emit(self, record):
         """
@@ -693,16 +697,16 @@
 
     def _rollover_and_do_write(self):
         buffer_msgs = ''
         while True:
             try:
                 msg = self.buffer_msgs_queue.get(block=False)
                 buffer_msgs += msg + '\n'
-                if len(buffer_msgs) > 10000 * 1000:
-                    break
+                # if len(buffer_msgs) > 1000 * 1000 * 100:
+                #     break
             except Empty:
                 break
         if buffer_msgs:
             try:
                 self._do_lock()
                 try:
                     if self.shouldRollover(None):
@@ -725,15 +729,15 @@
     file_handler_list = []
     has_start_emit_all_file_handler_process_id_set = set()  # 这个linux和windwos都兼容，windwos是多进程每个进程的变量has_start_emit_all_file_handler是独立的。linux是共享的。
     __lock_for_rotate = Lock()
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.buffer_msgs_queue = Queue()
-        atexit.register(self._when_exit)  # 如果程序属于立马就能结束的，需要在程序结束前执行这个钩子，防止不到最后一秒的日志没记录到。
+        atexit.register(self._when_exit)  # 如果程序属于立马就能结束的，需要在程序结束前执行这个钩子，防止不到最后一秒的日志没记录到。   有个弊端 at_exit 不能在子进程生效，所以不用这个类
         self.file_handler_list.append(self)
         if os.getpid() not in self.has_start_emit_all_file_handler_process_id_set:
             self.start_emit_all_file_handler()
             self.__class__.has_start_emit_all_file_handler_process_id_set.add(os.getpid())
 
     def rollover_and_do_write(self, ):
         # very_nb_print(self.buffer_msgs_queue.qsize())
@@ -1176,10 +1180,24 @@
                 print(f'删除成功 {r}')
             except (PermissionError, FileNotFoundError) as e:
                 print(e)
 
 
 ConcurrentDayRotatingFileHandler = ConcurrentDayRotatingFileHandlerWin if os_name == 'nt' else ConcurrentDayRotatingFileHandlerLinux
 
+
 # ConcurrentDayRotatingFileHandler = ConcurrentSecondRotatingFileHandlerLinux
 #
 # print(ConcurrentDayRotatingFileHandler)
+
+
+class BothDayAndSizeRotatingFileHandler(logging.Handler):
+    def __init__(self, file_name: typing.Optional[str], log_path='/pythonlogs', max_bytes=1000 * 1000 * 1000, back_count=10):
+        init_kwargs = copy.copy(locals())
+        init_kwargs.pop('self')
+        init_kwargs.pop('__class__')
+        super().__init__()
+        self.os_file_writter = OsFileWritter(**init_kwargs)
+
+    def emit(self, record: logging.LogRecord) -> None:
+        msg = self.format(record)
+        self.os_file_writter.write_2_file(msg + '\n')
```

### Comparing `nb_log-9.5/nb_log/handlers0000.py` & `nb_log-9.7/nb_log/handlers0000.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.5/nb_log/log_manager.py` & `nb_log-9.7/nb_log/log_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,16 +199,14 @@
 
 
 def check_log_level(log_level: int):
     if log_level not in LOG_LEVEL_LIST:
         raise ValueError(f'你设置的日志级别不正确,你设置的级别是 {log_level} ，日志级别必须是 {LOG_LEVEL_LIST} 其中之一')
 
 
-
-
 # noinspection PyMissingOrEmptyDocstring,PyPep8
 class LogManager(object):
     """
     一个日志管理类，用于创建logger和添加handler，支持将日志打印到控制台打印和写入日志文件和mongodb和邮件。
     """
     logger_name_list = []
     logger_list = []
@@ -304,16 +302,16 @@
         # else:
         #     self._logger_level = self._logger_level
         self._is_add_stream_handler = is_add_stream_handler
         self._do_not_use_color_handler = do_not_use_color_handler
         self._log_path = log_path
         self._log_filename = log_filename
         self._log_file_size = log_file_size
-        if log_file_handler_type not in (None, 1, 2, 3, 4, 5):
-            raise ValueError("log_file_handler_type的值必须设置为 1 2 3 4 5这5个数字")
+        if log_file_handler_type not in (None, 1, 2, 3, 4, 5,6):
+            raise ValueError("log_file_handler_type的值必须设置为 1 2 3 4 5 6 这几个数字")
         self._log_file_handler_type = log_file_handler_type or nb_log_config_default.LOG_FILE_HANDLER_TYPE
         self._mongo_url = mongo_url
         self._is_add_elastic_handler = is_add_elastic_handler
         self._is_add_kafka_handler = is_add_kafka_handler
         self._ding_talk_token = ding_talk_token
         self._ding_talk_time_interval = ding_talk_time_interval
         self._mail_handler_config = mail_handler_config
@@ -383,15 +381,16 @@
 
         # REMIND 添加多进程安全切片的文件日志
         if not (self._judge_logger_has_handler_type(ConcurrentRotatingFileHandler) or
                 self._judge_logger_has_handler_type(ConcurrentRotatingFileHandlerWithBufferInitiativeWindwos) or
                 self._judge_logger_has_handler_type(ConcurrentRotatingFileHandlerWithBufferInitiativeLinux) or
                 self._judge_logger_has_handler_type(ConcurrentDayRotatingFileHandler) or
                 self._judge_logger_has_handler_type(FileHandler) or
-                self._judge_logger_has_handler_type(ConcurrentRotatingFileHandler)
+                self._judge_logger_has_handler_type(ConcurrentRotatingFileHandler) or
+                self._judge_logger_has_handler_type(BothDayAndSizeRotatingFileHandler)
         ) and all([self._log_path, self._log_filename]):
             if not os.path.exists(self._log_path):
                 os.makedirs(self._log_path, exist_ok=True)
             log_file = os.path.join(self._log_path, self._log_filename)
             file_handler = None
             if self._log_file_handler_type == 1:
                 if os_name == 'nt':
@@ -416,14 +415,17 @@
             elif self._log_file_handler_type == 3:
                 file_handler = FileHandler(log_file, mode='a', encoding='utf-8')
             elif self._log_file_handler_type == 5:
                 file_handler = ConcurrentRotatingFileHandler(log_file,
                                                              maxBytes=self._log_file_size * 1024 * 1024,
                                                              backupCount=nb_log_config_default.LOG_FILE_BACKUP_COUNT,
                                                              encoding="utf-8")
+            elif self._log_file_handler_type == 6:
+                file_handler = BothDayAndSizeRotatingFileHandler(file_name=self._log_filename, log_path=self._log_path,
+                                                                 back_count=nb_log_config_default.LOG_FILE_BACKUP_COUNT, max_bytes=self._log_file_size * 1024 * 1024)
             file_handler.setLevel(self._logger_level)
             self.__add_a_hanlder(file_handler)
 
         # REMIND 添加mongo日志。
         if not self._judge_logger_has_handler_type(MongoHandler) and self._mongo_url:
             handler = MongoHandler(self._mongo_url)
             handler.setLevel(self._logger_level)
```

### Comparing `nb_log-9.5/nb_log/monkey_print.py` & `nb_log-9.7/nb_log/monkey_print.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 """
 import multiprocessing
 import os
 import sys
 import time
 import traceback
 from nb_log import nb_log_config_default
-from nb_log.file_write import PrintFileWritter
+# from nb_log.file_write import PrintFileWritter
+from nb_log.rotate_file_writter import OsFileWritter
 
 print_raw = print
 WORD_COLOR = 37
 
 
 def stdout_write(msg: str):
     sys.stdout.write(msg)
@@ -25,15 +26,15 @@
 def stderr_write(msg: str):
     sys.stderr.write(msg)
     sys.stderr.flush()
 
 
 print_wrtie_file_name = os.environ.get('PRINT_WRTIE_FILE_NAME', None) or nb_log_config_default.PRINT_WRTIE_FILE_NAME
 
-print_file_writter = PrintFileWritter(print_wrtie_file_name)
+print_file_writter = OsFileWritter(print_wrtie_file_name, back_count=nb_log_config_default.LOG_FILE_BACKUP_COUNT, max_bytes=nb_log_config_default.LOG_FILE_SIZE * 1024 * 1024)
 
 
 def _print_with_file_line(*args, sep=' ', end='\n', file=None, flush=True, sys_getframe_n=2):
     args = (str(arg) for arg in args)  # REMIND 防止是数字不能被join
     args_str = sep.join(args) + end
     # stdout_write(f'56:{file}')
     if file == sys.stderr:
@@ -41,27 +42,30 @@
         print_file_writter.write_2_file(args_str)
     elif file in [sys.stdout, None]:
         # 获取被调用函数在被调用时所处代码行数
         fra = sys._getframe(sys_getframe_n)
         line = fra.f_lineno
         file_name = fra.f_code.co_filename
         fun = fra.f_code.co_name
+        now_str= time.strftime("%Y-%m-%d %H:%M:%S")
+        # mtime = time.gmtime()
+        # now_str = f'{mtime.tm_year}-{mtime.tm_mon}-{mtime.tm_mday} {mtime.tm_hour}:{mtime.tm_min}:{mtime.tm_sec}'
         # sys.stdout.write(f'"{__file__}:{sys._getframe().f_lineno}"    {x}\n')
         if nb_log_config_default.DEFAULUT_USE_COLOR_HANDLER:
             if nb_log_config_default.DISPLAY_BACKGROUD_COLOR_IN_CONSOLE:
                 stdout_write(
-                    f'\033[0;34m{time.strftime("%H:%M:%S")}  "{file_name}:{line}" {fun}  \033[0;{WORD_COLOR};44m{args_str}\033[0m \033[0m')  # 36  93 96 94
+                    f'\033[0;34m{now_str}  "{file_name}:{line}" -{fun}-[print]-  \033[0;{WORD_COLOR};44m{args_str[:-1]}\033[0m \033[0m\n')  # 36  93 96 94
             else:
                 stdout_write(
-                    f'\033[0;{WORD_COLOR};34m{time.strftime("%H:%M:%S")}  "{file_name}:{line}" {fun}  {args_str}  \033[0m')  # 36  93 96 94
+                    f'\033[0;{WORD_COLOR};34m{now_str}  "{file_name}:{line}" -{fun}-[print]-  {args_str[:-1]}  \033[0m\n')  # 36  93 96 94
             # sys.stdout.write(f'\033[0;30;44m"{file_name}:{line}"  {time.strftime("%H:%M:%S")}  {"".join(args)}\033[0m\n')
         else:
             stdout_write(
-                f'{time.strftime("%H:%M:%S")}  "{file_name}:{line}"  {fun} {args_str} ')
-        print_file_writter.write_2_file(f'{time.strftime("%H:%M:%S")}  "{file_name}:{line}" {fun} {args_str} ')  # 36  93 96 94
+                f'{now_str}  "{file_name}:{line}"  -{fun}-[print]- {args_str} ')
+        print_file_writter.write_2_file(f'{now_str}  "{file_name}:{line}" -{fun}-[print]- {args_str} ')  # 36  93 96 94
     else:  # 例如traceback模块的print_exception函数 file的入参是   <_io.StringIO object at 0x00000264F2F065E8>，必须把内容重定向到这个对象里面，否则exception日志记录不了错误堆栈。
         print_raw(args_str, sep=sep, end=end, file=file)
         print_file_writter.write_2_file(args_str)
 
 
 # noinspection PyProtectedMember,PyUnusedLocal,PyIncorrectDocstring,DuplicatedCode
 def nb_print(*args, sep=' ', end='\n', file=None, flush=True):
```

### Comparing `nb_log-9.5/nb_log/monkey_std_filter_words.py` & `nb_log-9.7/nb_log/monkey_std_filter_words.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.5/nb_log/nb_log_config_default.py` & `nb_log-9.7/nb_log/nb_log_config_default.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,16 @@
 # 如果你设置了环境变量，export PRINT_WRTIE_FILE_NAME="my_proj.print" (linux临时环境变量语法，windows语法自己百度这里不举例),那就优先使用环境变量中设置的文件名字，而不是nb_log_config.py中设置的名字
 PRINT_WRTIE_FILE_NAME = Path(sys.path[1]).name + '.print'
 
 # 项目中的所有标准输出（不仅包括print，还包括了streamHandler日志）都写入到这个文件。自动每天一个文件， 2023-06-30.my_proj.std,生成的文件位置在定义的LOG_PATH
 # 如果你设置了环境变量，export SYS_STD_FILE_NAME="my_proj.std"  (linux临时环境变量语法，windows语法自己百度这里不举例),那就优先使用环境变量中设置的文件名字，，而不是nb_log_config.py中设置的名字
 SYS_STD_FILE_NAME = Path(sys.path[1]).name + '.std'
 
+USE_BULK_STDOUT_ON_WINDOWS = True
+
 DEFAULUT_USE_COLOR_HANDLER = True  # 是否默认使用有彩的日志。
 DISPLAY_BACKGROUD_COLOR_IN_CONSOLE = True  # 在控制台是否显示彩色块状的日志。为False则不使用大块的背景颜色。
 AUTO_PATCH_PRINT = True  # 是否自动打print的猴子补丁，如果打了猴子补丁，print自动变色和可点击跳转。
 SHOW_PYCHARM_COLOR_SETINGS = True  # 有的人很反感启动代码时候提示教你怎么优化pycahrm控制台颜色，可以把这里设置为False
 
 DEFAULT_ADD_MULTIPROCESSING_SAFE_ROATING_FILE_HANDLER = False  # 是否默认同时将日志记录到记log文件记事本中，就是用户不指定 log_filename的值，会自动写入日志命名空间.log文件中。
 LOG_FILE_SIZE = 100  # 单位是M,每个文件的切片大小，超过多少后就自动切割
@@ -87,23 +89,24 @@
 LOG_PATH = '/pythonlogs'  # 默认的日志文件夹,如果不写明磁盘名，则是项目代码所在磁盘的根目录下的/pythonlogs
 # LOG_PATH = Path(__file__).absolute().parent / Path("pythonlogs")   #这么配置就会自动在你项目的根目录下创建pythonlogs文件夹了并写入。
 if os.name == 'posix':  # linux非root用户和mac用户无法操作 /pythonlogs 文件夹，没有权限，默认修改为   home/[username]  下面了。例如你的linux用户名是  xiaomin，那么默认会创建并在 /home/xiaomin/pythonlogs文件夹下写入日志文件。
     home_path = os.environ.get("HOME", '/')  # 这个是获取linux系统的当前用户的主目录，不需要亲自设置
     LOG_PATH = Path(home_path) / Path('pythonlogs')  # linux mac 权限很严格，非root权限不能在/pythonlogs写入，修改一下默认值。
 # print('LOG_PATH:',LOG_PATH)
 
-LOG_FILE_HANDLER_TYPE = 1  # 1 2 3 4 5
+LOG_FILE_HANDLER_TYPE = 6  # 1 2 3 4 5 6
 """
 LOG_FILE_HANDLER_TYPE 这个值可以设置为 1 2 3 4 5 四种值，
 1为使用多进程安全按日志文件大小切割的文件日志,这是本人实现的批量写入日志，减少操作文件锁次数，测试10进程快速写入文件，win上性能比第5种提高了100倍，linux提升5倍
 2为多进程安全按天自动切割的文件日志，同一个文件，每天生成一个新的日志文件。日志文件名字后缀自动加上日期。
 3为不自动切割的单个文件的日志(不切割文件就不会出现所谓进程安不安全的问题) 
 4为 WatchedFileHandler，这个是需要在linux下才能使用，需要借助lograte外力进行日志文件的切割，多进程安全。
 5 为第三方的concurrent_log_handler.ConcurrentRotatingFileHandler按日志文件大小切割的文件日志，
    这个是采用了文件锁，多进程安全切割，文件锁在linux上使用fcntl性能还行，win上使用win32con性能非常惨。按大小切割建议不要选第5个个filehandler而是选择第1个。
+6 BothDayAndSizeRotatingFileHandler 使用本人完全彻底开发的，同时按照时间和大小切割，无论是文件的大小、还是时间达到了需要切割的条件就切割。
 """
 
 LOG_LEVEL_FILTER = logging.DEBUG  # 默认日志级别，低于此级别的日志不记录了。例如设置为INFO，那么logger.debug的不会记录，只会记录logger.info以上级别的。
 # 强烈不建议调高这里的级别为INFO，日志是有命名空间的，单独提高打印啰嗦的日志命名空间的日志级别就可以了，不要全局提高日志级别。
 # https://nb-log-doc.readthedocs.io/zh_CN/latest/articles/c9.html#id2  文档9.5里面讲了几百次 python logging的命名空间的作用了，有些人到现在还不知道日志的name作用。
 
 # 屏蔽的字符串显示，用 if in {打印信息} 来判断实现的,如果打印的消息中包括 FILTER_WORDS_PRINT 数组中的任何一个字符串，那么消息就不执行打印。
```

### Comparing `nb_log-9.5/nb_log/nb_logger.py` & `nb_log-9.7/nb_log/nb_logger.py`

 * *Files 16% similar despite different names*

```diff
@@ -32,14 +32,27 @@
 
 '''
 有的人手痒，非要封装nb_log,那么封装时候调用原生日志的 info() 务必要传入  extra={'sys_getframe_n': 3}
 如果你不传递 extra={'sys_getframe_n': 3} ，那么 废物日志类().info('啊啊啊啊') ，显示是第 x2 行打印的日志，而不是第 y行打印的日志。
 '''
 
 class NbLogger(logging.Logger):
+
+    """
+    写 NbLogger 实在python3.7测试的，python3.9以后官方已经加了stacklevel入参。
+    20230705 现在经过github cpython的源码核实，在python3.9版本中
+    def _log(self, level, msg, args, exc_info=None, extra=None, stack_info=False,
+             stacklevel=1):
+
+    def findCaller(self, stack_info=False, stacklevel=1):
+
+    用户可以传递 stacklevel 了，本NbLogger是适配python3.6 3.7 3.8版本, Nblogger 的 sys_getframe_n 入参就是 stacklevel的意义。
+    说明我的思维和python官方人员想到一起去了，3.9以后的logging包debug ingo error等 支持修改查找调用堆栈的深度层级，防止用户封装了debug info warnring 等后，日志模板获取的 文件名 行号是错误深度层级的。。
+
+    """
     def _log(self, level, msg, args, exc_info=None, extra=None, stack_info=False):
         """
         Low-level logging routine which creates a LogRecord and then calls
         all the handlers of this logger to handle the record.
         """
 
         sys_getframe_n =2
```

### Comparing `nb_log-9.5/nb_log/set_nb_log_config.py` & `nb_log-9.7/nb_log/set_nb_log_config.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.5/nb_log/simple_print.py` & `nb_log-9.7/nb_log/simple_print.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,12 @@
+import atexit
+import os
+import queue
 import sys
+import threading
 import time
 import multiprocessing
 
 print_raw = print
 WORD_COLOR = 37
 
 
@@ -12,35 +16,42 @@
 
 
 def stderr_write(msg: str):
     sys.stderr.write(msg)
     sys.stderr.flush()
 
 
+
 def _sprint(*args, sep=' ', end='\n', file=None, flush=True, sys_getframe_n=2, ):
     args = (str(arg) for arg in args)  # REMIND 防止是数字不能被join
     args_str = sep.join(args) + end
     # stdout_write(f'56:{file}')
     if file == sys.stderr:
         stderr_write(args_str)  # 如 threading 模块第926行，打印线程错误，希望保持原始的红色错误方式，不希望转成蓝色。
     elif file in [sys.stdout, None]:
         # 获取被调用函数在被调用时所处代码行数
         fra = sys._getframe(sys_getframe_n)
         line = fra.f_lineno
         file_name = fra.f_code.co_filename
         fun = fra.f_code.co_name
         # sys.stdout.write(f'"{__file__}:{sys._getframe().f_lineno}"    {x}\n')
-        stdout_write(f'{time.strftime("%H:%M:%S")}  "{file_name}:{line}"  {fun} {args_str} ')
+        msg = f'{time.strftime("%H:%M:%S")}  "{file_name}:{line}"  - {fun} - {args_str}'
+        stdout_write(msg)
     else:  # 例如traceback模块的print_exception函数 file的入参是   <_io.StringIO object at 0x00000264F2F065E8>，必须把内容重定向到这个对象里面，否则exception日志记录不了错误堆栈。
         print_raw(args_str, sep=sep, end=end, file=file)
 
 
-def sprint(*args, sep=' ', end='\n', file=None, flush=True, sys_getframe_n=1, only_print_on_main_process=False):
+def sprint(*args, sep=' ', end='\n', file=None, flush=True, sys_getframe_n=2, only_print_on_main_process=False):
     if only_print_on_main_process:
         if multiprocessing.process.current_process().name == 'MainProcess':
             _sprint(*args, sep=sep, end=end, file=file, flush=flush, sys_getframe_n=2)
     else:
-        _sprint(*args, sep=sep, end=end, file=file, flush=flush, sys_getframe_n=2)
+        _sprint(*args, sep=sep, end=end, file=file, flush=flush, sys_getframe_n=sys_getframe_n)
 
 
 if __name__ == '__main__':
-    sprint('欢欢')
+    str1 = 'O(∩_∩)O哈哈' * 40
+    t1 = time.time()
+    for i in range(10000):
+        sprint(str1)
+
+    print(time.time() - t1)
```

### Comparing `nb_log-9.5/nb_log.egg-info/PKG-INFO` & `nb_log-9.7/nb_log.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-log
-Version: 9.5
+Version: 9.7
 Summary: very sharp color display,monkey patch bulitin print  and high-performance multiprocess safe roating file handler,other handlers includeing dintalk ,email,kafka,elastic and so on 
 Home-page: https://github.com/ydf0509/nb_log
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
```

### Comparing `nb_log-9.5/setup.py` & `nb_log-9.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ]
 
 if os.name == 'nt':
     install_requires.append('pywin32')
 
 setup(
     name='nb_log',  #
-    version="9.5",
+    version="9.7",
     description=(
         'very sharp color display,monkey patch bulitin print  and high-performance multiprocess safe roating file handler,other handlers includeing dintalk ,email,kafka,elastic and so on '
     ),
     keywords=["logging", "logger", "multiprocess file handler", "color handler"],
     # long_description=open('README.md', 'r',encoding='utf8').read(),
     long_description_content_type="text/markdown",
     long_description=open(filepath, 'r', encoding='utf8').read(),
@@ -63,14 +63,14 @@
 """
 打包上传
 python setup.py sdist upload -r pypi
 
 
 
 python setup.py sdist & twine upload dist/nb_log-6.0.tar.gz
-python setup.py sdist & python -m  twine upload dist/nb_log-9.5.tar.gz
+python setup.py sdist & python -m  twine upload dist/nb_log-9.7.tar.gz
 
 twine upload dist/*
 
 
 python -m pip install nb_log --upgrade -i https://pypi.org/simple   # 及时的方式，不用等待 阿里云 豆瓣 同步
 """
```

