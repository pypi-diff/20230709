# Comparing `tmp/runweb-0.3.1.tar.gz` & `tmp/runweb-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runweb-0.3.1.tar", last modified: Fri Jul  7 06:21:48 2023, max compression
+gzip compressed data, was "runweb-0.4.0.tar", last modified: Sun Jul  9 14:28:13 2023, max compression
```

## Comparing `runweb-0.3.1.tar` & `runweb-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0    11341 2023-07-07 06:21:31.797731 runweb-0.3.1/LICENSE
--rw-r--r--   0        0        0      729 2023-07-07 06:21:31.797731 runweb-0.3.1/README.md
--rw-r--r--   0        0        0     1230 2023-07-07 06:21:48.217938 runweb-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-07 06:21:31.797731 runweb-0.3.1/runweb/__init__.py
--rw-r--r--   0        0        0       29 2023-07-07 06:21:31.797731 runweb-0.3.1/runweb/__main__.py
--rw-r--r--   0        0        0       22 2023-07-07 06:21:31.797731 runweb-0.3.1/runweb/__version__.py
--rw-r--r--   0        0        0     3573 2023-07-07 06:21:31.797731 runweb-0.3.1/runweb/main.py
--rw-r--r--   0        0        0     2171 2023-07-07 06:21:31.797731 runweb-0.3.1/runweb/multiprocess.py
--rw-r--r--   0        0        0     1640 2023-07-07 06:21:31.797731 runweb-0.3.1/runweb/parse.py
--rw-r--r--   0        0        0        0 2023-07-07 06:21:31.797731 runweb-0.3.1/runweb/runner/__init__.py
--rw-r--r--   0        0        0      837 2023-07-07 06:21:31.797731 runweb-0.3.1/runweb/runner/uvicorn.py
--rw-r--r--   0        0        0      814 2023-07-07 06:21:31.801731 runweb-0.3.1/runweb/runner/waitress.py
--rw-r--r--   0        0        0        0 2023-07-07 06:21:31.801731 runweb-0.3.1/tests/__init__.py
--rw-r--r--   0        0        0      930 2023-07-07 06:21:31.801731 runweb-0.3.1/tests/test_uvicorn.py
--rw-r--r--   0        0        0      934 2023-07-07 06:21:31.801731 runweb-0.3.1/tests/test_waitress.py
--rw-r--r--   0        0        0      866 2023-07-07 06:21:31.801731 runweb-0.3.1/tests/utils.py
--rw-r--r--   0        0        0     1484 1970-01-01 00:00:00.000000 runweb-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-07-09 14:27:53.096817 runweb-0.4.0/LICENSE
+-rw-r--r--   0        0        0      729 2023-07-09 14:27:53.096817 runweb-0.4.0/README.md
+-rw-r--r--   0        0        0     1295 2023-07-09 14:28:13.704990 runweb-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-09 14:27:53.096817 runweb-0.4.0/runweb/__init__.py
+-rw-r--r--   0        0        0       29 2023-07-09 14:27:53.096817 runweb-0.4.0/runweb/__main__.py
+-rw-r--r--   0        0        0       22 2023-07-09 14:27:53.096817 runweb-0.4.0/runweb/__version__.py
+-rw-r--r--   0        0        0      147 2023-07-09 14:27:53.096817 runweb-0.4.0/runweb/logging.py
+-rw-r--r--   0        0        0     3572 2023-07-09 14:27:53.096817 runweb-0.4.0/runweb/main.py
+-rw-r--r--   0        0        0     2205 2023-07-09 14:27:53.096817 runweb-0.4.0/runweb/multiprocess.py
+-rw-r--r--   0        0        0     1640 2023-07-09 14:27:53.096817 runweb-0.4.0/runweb/parse.py
+-rw-r--r--   0        0        0        0 2023-07-09 14:27:53.096817 runweb-0.4.0/runweb/runner/__init__.py
+-rw-r--r--   0        0        0     1006 2023-07-09 14:27:53.096817 runweb-0.4.0/runweb/runner/uvicorn.py
+-rw-r--r--   0        0        0      983 2023-07-09 14:27:53.096817 runweb-0.4.0/runweb/runner/waitress.py
+-rw-r--r--   0        0        0        0 2023-07-09 14:27:53.096817 runweb-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0      930 2023-07-09 14:27:53.096817 runweb-0.4.0/tests/test_uvicorn.py
+-rw-r--r--   0        0        0      934 2023-07-09 14:27:53.096817 runweb-0.4.0/tests/test_waitress.py
+-rw-r--r--   0        0        0      866 2023-07-09 14:27:53.096817 runweb-0.4.0/tests/utils.py
+-rw-r--r--   0        0        0     1484 1970-01-01 00:00:00.000000 runweb-0.4.0/PKG-INFO
```

### Comparing `runweb-0.3.1/LICENSE` & `runweb-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `runweb-0.3.1/README.md` & `runweb-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `runweb-0.3.1/pyproject.toml` & `runweb-0.4.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "click>=8.1.3",
 ]
 description = "Run web server with one command."
 dynamic = []
 name = "runweb"
 readme = "README.md"
 requires-python = ">=3.7"
-version = "0.3.1"
+version = "0.4.0"
 
 [project.license]
 text = "Apache-2.0"
 
 [project.optional-dependencies]
 tui = [
     "trogon>=0.4.0",
@@ -56,12 +56,20 @@
 
 [tool.pdm.scripts.test]
 shell = "pytest tests"
 
 [tool.pdm.scripts.push-tag]
 shell = "git add runweb/__version__.py && git commit -m v`pdm show --version` && git tag v`pdm show --version` && git push && git push --tags"
 
+[tool.ruff]
+select = [
+    "F",
+    "E",
+    "W",
+    "I001",
+]
+
 [build-system]
 build-backend = "pdm.backend"
 requires = [
     "pdm-backend",
 ]
```

### Comparing `runweb-0.3.1/runweb/main.py` & `runweb-0.4.0/runweb/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Union
 
 import click
 
 from .parse import parse_application
 
-
 SERVERS = {"wsgi": {}, "asgi": {}}
 
 try:
     from .runner.waitress import wsgi as wsgi_waitress
 except ImportError:
     pass
 else:
```

### Comparing `runweb-0.3.1/runweb/multiprocess.py` & `runweb-0.4.0/runweb/multiprocess.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 import signal
 import threading
 from multiprocessing.context import SpawnProcess
 from typing import Callable
 
 import click
 
+from .logging import logger
+
 
 def multiprocess(workers_num: int, create_process: Callable[[], SpawnProcess]) -> None:
     should_exit = threading.Event()
 
-    click.echo(
+    logger.info(
         "Started parent process [{}]".format(
             click.style(str(os.getpid()), fg="cyan", bold=True)
         )
     )
 
     for sig in (
         signal.SIGINT,  # Sent by Ctrl+C.
@@ -26,30 +28,30 @@
 
     processes: list[SpawnProcess] = []
 
     def create_child() -> SpawnProcess:
         process = create_process()
         processes.append(process)
         process.start()
-        click.echo(
+        logger.info(
             "Started child process [{}]".format(
                 click.style(str(process.pid), fg="cyan", bold=True)
             )
         )
         return process
 
     for _ in range(workers_num):
         create_child()
 
     while not should_exit.wait(0.5):
         for idx, process in enumerate(tuple(processes)):
             if process.is_alive():
                 continue
 
-            click.echo(
+            logger.info(
                 "Child process [{}] died unexpectedly".format(
                     click.style(str(process.pid), fg="cyan", bold=True)
                 )
             )
             del processes[idx]
             create_child()
 
@@ -60,19 +62,19 @@
         if os.name == "nt":
             # Windows doesn't support SIGTERM.
             os.kill(process.pid, signal.CTRL_BREAK_EVENT)
         else:
             os.kill(process.pid, signal.SIGTERM)
 
     for process in processes:
-        click.echo(
+        logger.info(
             "Waiting for child process [{}] to terminate".format(
                 click.style(str(process.pid), fg="cyan", bold=True)
             )
         )
         process.join()
 
-    click.echo(
+    logger.info(
         "Stopped parent process [{}]".format(
             click.style(str(os.getpid()), fg="cyan", bold=True)
         )
     )
```

### Comparing `runweb-0.3.1/runweb/parse.py` & `runweb-0.4.0/runweb/parse.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import importlib
+import ipaddress
 import os
 import socket
-import ipaddress
 from functools import reduce
 from typing import Any
 
 import click
 
 
 def parse_bind(value: str) -> socket.socket:
```

### Comparing `runweb-0.3.1/runweb/runner/uvicorn.py` & `runweb-0.4.0/runweb/runner/waitress.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 import multiprocessing
-
 from typing import Union
 
-from uvicorn import Server, Config
+import click
+from waitress import create_server
 
-from ..parse import parse_application, parse_bind
+from ..logging import logger
 from ..multiprocess import multiprocess
+from ..parse import parse_application, parse_bind
 
 spawn = multiprocessing.get_context("spawn")
 
 
 def singleprocess(application: str, bind_address: str) -> None:
-    config = Config(parse_application(application))
-    server = Server(config)
-    server.run([parse_bind(bind_address)])
+    server = create_server(
+        parse_application(application),
+        sockets=[parse_bind(bind_address)],
+    )
+    server.run()
 
 
-def asgi(bind_address: str, application: str, workers_num: Union[int, None]) -> None:
-    parse_application(application)
+def wsgi(bind_address: str, application: str, workers_num: Union[int, None]) -> None:
     parse_bind(bind_address).close()
 
+    logger.info(
+        "Binding to {}".format(
+            click.style(bind_address, fg="green", bold=True),
+        )
+    )
+
     if workers_num is None:
         singleprocess(application, bind_address)
     else:
         multiprocess(
             workers_num,
             lambda: spawn.Process(
                 target=singleprocess, args=(application, bind_address)
```

### Comparing `runweb-0.3.1/tests/test_uvicorn.py` & `runweb-0.4.0/tests/test_uvicorn.py`

 * *Files identical despite different names*

### Comparing `runweb-0.3.1/tests/test_waitress.py` & `runweb-0.4.0/tests/test_waitress.py`

 * *Files identical despite different names*

### Comparing `runweb-0.3.1/tests/utils.py` & `runweb-0.4.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `runweb-0.3.1/PKG-INFO` & `runweb-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runweb
-Version: 0.3.1
+Version: 0.4.0
 Summary: Run web server with one command.
 Author-Email: abersheeran <me@abersheeran.com>
 License: Apache-2.0
 Requires-Python: >=3.7
 Requires-Dist: click>=8.1.3
 Requires-Dist: trogon>=0.4.0; extra == "tui"
 Requires-Dist: waitress; extra == "waitress"
```

