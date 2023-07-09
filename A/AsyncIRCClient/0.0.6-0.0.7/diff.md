# Comparing `tmp/AsyncIRCClient-0.0.6.tar.gz` & `tmp/AsyncIRCClient-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AsyncIRCClient-0.0.6.tar", last modified: Wed Jul  5 17:15:25 2023, max compression
+gzip compressed data, was "AsyncIRCClient-0.0.7.tar", last modified: Sun Jul  9 08:47:15 2023, max compression
```

## Comparing `AsyncIRCClient-0.0.6.tar` & `AsyncIRCClient-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 17:15:25.353625 AsyncIRCClient-0.0.6/
-drwxrwxrwx   0        0        0        0 2023-07-05 17:15:25.350624 AsyncIRCClient-0.0.6/AsyncIRCClient.egg-info/
--rw-rw-rw-   0        0        0     1339 2023-07-05 17:15:25.000000 AsyncIRCClient-0.0.6/AsyncIRCClient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-07-05 17:15:25.000000 AsyncIRCClient-0.0.6/AsyncIRCClient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 17:15:25.000000 AsyncIRCClient-0.0.6/AsyncIRCClient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-05 17:15:25.000000 AsyncIRCClient-0.0.6/AsyncIRCClient.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-05 17:15:25.000000 AsyncIRCClient-0.0.6/AsyncIRCClient.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1339 2023-07-05 17:15:25.353625 AsyncIRCClient-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1152 2023-06-09 10:28:03.000000 AsyncIRCClient-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-05 17:15:25.352625 AsyncIRCClient-0.0.6/async_irc_client/
--rw-rw-rw-   0        0        0       33 2023-06-09 10:25:57.000000 AsyncIRCClient-0.0.6/async_irc_client/__init__.py
--rw-rw-rw-   0        0        0    35273 2023-07-05 17:14:41.000000 AsyncIRCClient-0.0.6/async_irc_client/async_irc_client.py
--rw-rw-rw-   0        0        0       42 2023-07-05 17:15:25.353625 AsyncIRCClient-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      460 2023-07-05 17:14:41.000000 AsyncIRCClient-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 08:47:15.542828 AsyncIRCClient-0.0.7/
+drwxrwxrwx   0        0        0        0 2023-07-09 08:47:15.538822 AsyncIRCClient-0.0.7/AsyncIRCClient.egg-info/
+-rw-rw-rw-   0        0        0     1339 2023-07-09 08:47:15.000000 AsyncIRCClient-0.0.7/AsyncIRCClient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-09 08:47:15.000000 AsyncIRCClient-0.0.7/AsyncIRCClient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 08:47:15.000000 AsyncIRCClient-0.0.7/AsyncIRCClient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-09 08:47:15.000000 AsyncIRCClient-0.0.7/AsyncIRCClient.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-09 08:47:15.000000 AsyncIRCClient-0.0.7/AsyncIRCClient.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1339 2023-07-09 08:47:15.542828 AsyncIRCClient-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1152 2023-06-09 10:28:03.000000 AsyncIRCClient-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 08:47:15.541828 AsyncIRCClient-0.0.7/async_irc_client/
+-rw-rw-rw-   0        0        0       33 2023-06-09 10:25:57.000000 AsyncIRCClient-0.0.7/async_irc_client/__init__.py
+-rw-rw-rw-   0        0        0    35307 2023-07-09 08:46:26.000000 AsyncIRCClient-0.0.7/async_irc_client/async_irc_client.py
+-rw-rw-rw-   0        0        0       42 2023-07-09 08:47:15.542828 AsyncIRCClient-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      460 2023-07-09 08:46:26.000000 AsyncIRCClient-0.0.7/setup.py
```

### Comparing `AsyncIRCClient-0.0.6/AsyncIRCClient.egg-info/PKG-INFO` & `AsyncIRCClient-0.0.7/AsyncIRCClient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AsyncIRCClient
-Version: 0.0.6
+Version: 0.0.7
 Summary: Async IRC Client
 Author: CoreTaxxe
 Author-email: coretaxxe@gmail.com
 Description-Content-Type: text/markdown
 
 # AsyncIRCClient
 Async (Twitch-) IRC client
```

### Comparing `AsyncIRCClient-0.0.6/PKG-INFO` & `AsyncIRCClient-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AsyncIRCClient
-Version: 0.0.6
+Version: 0.0.7
 Summary: Async IRC Client
 Author: CoreTaxxe
 Author-email: coretaxxe@gmail.com
 Description-Content-Type: text/markdown
 
 # AsyncIRCClient
 Async (Twitch-) IRC client
```

### Comparing `AsyncIRCClient-0.0.6/README.md` & `AsyncIRCClient-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `AsyncIRCClient-0.0.6/async_irc_client/async_irc_client.py` & `AsyncIRCClient-0.0.7/async_irc_client/async_irc_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 from asyncio import transports
 from dataclasses import dataclass, field
 from typing import Union, Callable, Any, Coroutine
 import datetime
 from loguru import logger
 
 
-def is_event_loop_running() -> bool:
+def is_event_loop_set() -> bool:
     """
-    check if asyncio has loop running
+    check if asyncio has loop set
     :return: bool
     """
     try:
-        loop: asyncio.AbstractEventLoop = asyncio.get_running_loop()
-        return loop.is_running()
+        # check if any event loop is set
+        asyncio.get_event_loop()
+        return True
     except RuntimeError as _error:
         return False
 
 
 def get_time_difference(time_str: str) -> float:
     """
     get time difference
@@ -287,23 +288,24 @@
         await self._callback()
 
     def start(self) -> None:
         """
         start timer
         :return: None
         """
-        self._task = asyncio.get_event_loop().create_task(self._wait())
+        loop: asyncio.AbstractEventLoop = asyncio.get_event_loop()
+        self._task = loop.create_task(self._wait())
 
     def cancel(self) -> None:
         """
         cancel timer
         :return: None
         """
         if self._task is None:
-            raise ValueError("Timer has not been started yet.")
+            return logger.warning("Timer has not been started yet.")
         self._task.cancel()
 
     def restart(self) -> None:
         """
         restart timer
         :return: None
         """
@@ -407,14 +409,18 @@
         self._port: int = port
         self._loop: Union[asyncio.AbstractEventLoop, None] = loop
         self._protocol: Union[AsyncIRCClientProtocol, None] = None
         self._transport: Union[transports.Transport, None] = None
         self._event_handler: dict[str, Callable] = {}
         self._is_connected: bool = False
 
+        # get event loop if none set
+        if self._loop is None:
+            self._loop = asyncio.get_event_loop() if is_event_loop_set() else asyncio.new_event_loop()
+
     def send_irc_data(self, data: str, log: bool = True) -> None:
         """
         send irc data.
         :param data: data to send
         :param log: log to console
         :return: None
         """
@@ -424,18 +430,14 @@
         self._protocol.send_irc_data(data, log)
 
     def run(self) -> None:
         """
         starts the clients mainloop
         :return: None
         """
-        # get event loop if none set
-        if self._loop is None:
-            self._loop = asyncio.get_event_loop() if is_event_loop_running() else asyncio.new_event_loop()
-
         # create task of our run method
         self._loop.create_task(self._connect_and_run(), name="InitialConnectAndRun")
         # run the loop forever
         try:
             self._loop.run_forever()
         except KeyboardInterrupt as error:
             self._stop_tasks_and_loop(error)
```

