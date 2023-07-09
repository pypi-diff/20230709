# Comparing `tmp/ddcci_plasmoid_backend-0.1.5.tar.gz` & `tmp/ddcci_plasmoid_backend-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddcci_plasmoid_backend-0.1.5.tar", max compression
+gzip compressed data, was "ddcci_plasmoid_backend-0.1.6.tar", max compression
```

## Comparing `ddcci_plasmoid_backend-0.1.5.tar` & `ddcci_plasmoid_backend-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1008 2023-04-16 10:57:22.596457 ddcci_plasmoid_backend-0.1.5/README.md
--rw-r--r--   0        0        0     3132 2023-04-16 10:14:42.667713 ddcci_plasmoid_backend-0.1.5/ddcci_plasmoid_backend/Node.py
--rw-r--r--   0        0        0     3419 2023-04-16 10:14:42.667713 ddcci_plasmoid_backend-0.1.5/ddcci_plasmoid_backend/Node_test.py
--rw-r--r--   0        0        0      889 2023-04-11 20:59:26.588299 ddcci_plasmoid_backend-0.1.5/ddcci_plasmoid_backend/__init__.py
--rw-r--r--   0        0        0     3568 2023-04-15 11:26:35.695349 ddcci_plasmoid_backend-0.1.5/ddcci_plasmoid_backend/__main__.py
--rw-r--r--   0        0        0     6132 2023-04-12 12:46:00.782718 ddcci_plasmoid_backend-0.1.5/ddcci_plasmoid_backend/ddcci.py
--rw-r--r--   0        0        0     1967 2023-04-12 12:46:00.786051 ddcci_plasmoid_backend-0.1.5/ddcci_plasmoid_backend/ddcci_test.py
--rw-r--r--   0        0        0     1064 2023-04-16 11:03:51.161773 ddcci_plasmoid_backend-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1947 1970-01-01 00:00:00.000000 ddcci_plasmoid_backend-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-07-09 14:37:55.376673 ddcci_plasmoid_backend-0.1.6/README.md
+-rw-r--r--   0        0        0     3092 2023-07-09 19:15:28.751390 ddcci_plasmoid_backend-0.1.6/ddcci_plasmoid_backend/Node.py
+-rw-r--r--   0        0        0     3414 2023-07-09 19:13:27.762362 ddcci_plasmoid_backend-0.1.6/ddcci_plasmoid_backend/Node_test.py
+-rw-r--r--   0        0        0     1107 2023-07-09 14:37:55.376673 ddcci_plasmoid_backend-0.1.6/ddcci_plasmoid_backend/__init__.py
+-rw-r--r--   0        0        0     4943 2023-07-09 18:57:19.866568 ddcci_plasmoid_backend-0.1.6/ddcci_plasmoid_backend/__main__.py
+-rw-r--r--   0        0        0     6474 2023-07-09 21:25:05.904713 ddcci_plasmoid_backend-0.1.6/ddcci_plasmoid_backend/ddcci.py
+-rw-r--r--   0        0        0     1099 2023-07-09 21:47:10.541095 ddcci_plasmoid_backend-0.1.6/ddcci_plasmoid_backend/ddcci_test.py
+-rw-r--r--   0        0        0     1465 2023-07-09 21:49:41.461229 ddcci_plasmoid_backend-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2020 1970-01-01 00:00:00.000000 ddcci_plasmoid_backend-0.1.6/PKG-INFO
```

### Comparing `ddcci_plasmoid_backend-0.1.5/README.md` & `ddcci_plasmoid_backend-0.1.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # KDE Plasma Widget for external monitor brightness adjustment
 
-![Screenshot](./banner.png)
+![Screenshot](https://raw.githubusercontent.com/davidhi7/ddcci-plasmoid/main/screenshots/banner.png)
 
 * This widget allows you to adjust the brightness of external monitors. We accomplish that using [DDC/CI](https://en.wikipedia.org/wiki/Display_Data_Channel#DDC/CI), a protocol that allows your computer to control monitors and change options like the brightness or contrast.
 * A seamless integration into the Plasma desktop is a major goal of this project. The widget is versatile and can be used as a standalone widget or integrated into the system tray.
 * Notebook monitors are currently unsupported because they use different interfaces to communicate with the operating system.
 
 ## Requirements
```

### Comparing `ddcci_plasmoid_backend-0.1.5/ddcci_plasmoid_backend/Node.py` & `ddcci_plasmoid_backend-0.1.6/ddcci_plasmoid_backend/Node.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from __future__ import annotations
 
 from dataclasses import field
-from typing import Optional, Dict
 
 
 class Node:
-    parent: Optional[Node]
+    parent: Node | None
     indentation: int
     key: str
     value: str
     children: list[Node] = field(default_factory=list)
 
-    child_by_key: Dict[str, Node]
+    child_by_key: dict[str, Node]
 
-    def __init__(self, parent: Optional[Node], indentation: int, key: str = '', value: str = ''):
+    def __init__(self, parent: Node | None, indentation: int, key: str = '', value: str = ''):
         """
         Create a new node and set it as the child of the parent.
         """
         self.parent = parent
         self.key = key
         self.value = value
         self.indentation = indentation
```

### Comparing `ddcci_plasmoid_backend-0.1.5/ddcci_plasmoid_backend/Node_test.py` & `ddcci_plasmoid_backend-0.1.6/ddcci_plasmoid_backend/Node_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
                 'children': []
             }
         ]
     }
 
 
 def test_parse_indented_text_basic():
-    with open('fixtures/basic/indented.txt', 'r') as file:
+    with open('fixtures/basic/indented.txt') as file:
         lines = file.read().split('\n')
     node = Node.parse_indented_text(lines).to_dict()
 
     assert node == {
         'key': '',
         'value': '',
         'indentation': -1,
```

### Comparing `ddcci_plasmoid_backend-0.1.5/ddcci_plasmoid_backend/__init__.py` & `ddcci_plasmoid_backend-0.1.6/ddcci_plasmoid_backend/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 import argparse
+import pathlib
 
 
 def get_parser() -> argparse.ArgumentParser:
     argument_parser = argparse.ArgumentParser(prog='plasma-ddcci-backend')
     argument_parser.add_argument(
         '-d', '--debug',
         action='store_true',
-        help='Run in debug mode'
+        help='Print debug messages to stdout'
+    )
+    argument_parser.add_argument(
+        '--debug-log',
+        action='store',
+        type=pathlib.Path,
+        metavar='LOG_FILE',
+        help='Write debug messages to LOG_FILE'
     )
     sub_parsers = argument_parser.add_subparsers(
         title='commands',
         dest='command',
         required=True
     )
     sub_parsers.add_parser('version')
```

### Comparing `ddcci_plasmoid_backend-0.1.5/ddcci_plasmoid_backend/__main__.py` & `ddcci_plasmoid_backend-0.1.6/ddcci_plasmoid_backend/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,52 +1,84 @@
+from __future__ import annotations
+
 import asyncio
+import getpass
 import json
 import logging
-import os
+import re
 import subprocess
 import sys
 import tempfile
 from importlib.metadata import version
 from pathlib import Path
 from typing import NoReturn
 
 import fasteners
 
 from ddcci_plasmoid_backend import ddcci
 from ddcci_plasmoid_backend.__init__ import get_parser
 
 
+def get_ddcutil_version() -> str:
+    result = subprocess.run(['ddcutil', '--version'], check=True, stdout=subprocess.PIPE)
+    # First line of ddcutil output contains the version
+    version_line = result.stdout.decode().split('\n')[0]
+    # Remove all characters from this line except for points followed by a number
+    # This is supposed to extract the version (x.y.z) from the string
+    return re.sub(r'(?!\.\d)\D', '', version_line)
+
+
 def main():
     arguments = vars(get_parser().parse_args())
 
-    logging.basicConfig(format='%(levelname)s %(name)s: %(message)s',
-                        level=logging.DEBUG if arguments['debug'] else logging.INFO)
+    logging_formatter = logging.Formatter('%(levelname)s %(name)s: %(message)s')
+
+    logging.getLogger().setLevel(logging.DEBUG)
+    stream_handler = logging.StreamHandler(sys.stdout)
+    stream_handler.setFormatter(logging_formatter)
+    stream_handler.setLevel(logging.DEBUG if arguments['debug'] else logging.INFO)
+    logging.getLogger().addHandler(stream_handler)
+
+    if arguments['debug_log']:
+        log_path: Path = arguments['debug_log']
+        # Fail if log_path exists but is not a file
+        if not log_path.is_file() and log_path.exists():
+            logging.debug('`LOG_FILE` must be a valid file')
+        else:
+            logging.debug(f'Writing logs to file {log_path}')
+            file_handler = logging.FileHandler(log_path)
+            file_handler.setFormatter(logging_formatter)
+            file_handler.setLevel(logging.DEBUG)
+            logging.getLogger().addHandler(file_handler)
+
     # supress log message `DEBUG asyncio: Using selector: EpollSelector`
     logging.getLogger('asyncio').setLevel(logging.WARNING)
     logger = logging.getLogger(__name__)
-    logger.debug(f'Running version {version("ddcci-plasmoid-backend")} in debug mode')
+    logger.debug(f'backend version: {version("ddcci-plasmoid-backend")}')
+    logger.debug(f'ddcutil version: {get_ddcutil_version()}')
 
     def handle_error(error: str | subprocess.CalledProcessError) -> NoReturn:
         if isinstance(error, subprocess.CalledProcessError):
-            error = err.stderr if err.stderr else err.stdout
+            error = error.stderr if error.stderr else error.stdout
         print(json.dumps({
             'command': arguments['command'],
             'error': error.replace('\n', ' ')
         }))
         sys.exit(1)
 
-    logger.debug(f'Command: {arguments["command"]}')
+    logger.debug(f'argv: {" ".join(sys.argv)}')
 
     if arguments['command'] == 'version':
         print(version('ddcci-plasmoid-backend'))
         sys.exit(0)
 
     # include the username in the lock file. Otherwise, if user A creates a lock, user B may not have the permissions
     # to access the lock file and this program will fail until the lock file is deleted.
-    with fasteners.InterProcessLock(Path(tempfile.gettempdir()) / f'ddcci_plasmoid_backend-{os.getlogin()}.lock'):
+    # Using `os.getlogin()` may fail on some configurations (#19)
+    with fasteners.InterProcessLock(Path(tempfile.gettempdir()) / f'ddcci_plasmoid_backend-{getpass.getuser()}.lock'):
         if arguments['command'] == 'detect':
             try:
                 result = asyncio.run(ddcci.detect())
             except subprocess.CalledProcessError as err:
                 logger.debug(err)
                 handle_error(err)
             except Exception as err:
```

### Comparing `ddcci_plasmoid_backend-0.1.5/ddcci_plasmoid_backend/ddcci.py` & `ddcci_plasmoid_backend-0.1.6/ddcci_plasmoid_backend/ddcci.py`

 * *Files 7% similar despite different names*

```diff
@@ -115,15 +115,19 @@
     return int(re.search(r'\d+', node.key).group())
 
 
 # Wrap sync and async subprocess calls for mocking
 def subprocess_wrapper(cmd: str) -> CommandOutput:
     logger.debug('Execute command: `' + cmd + '`')
     proc = subprocess.run(cmd.split(' '), capture_output=True)
-    stdout = proc.stdout.decode()
+    # Fix #32
+    stdout = proc.stdout.decode().replace(
+        '(is_nvidia_einval_bug          ) nvida/i2c-dev bug encountered. Forcing future io I2C_IO_STRATEGY_FILEIO. '
+        'Retrying\n', ''
+    )
     stderr = proc.stderr.decode()
     command_output = {
         'returnCode': proc.returncode,
         'stdout': stdout,
         'stderr': stderr,
     }
 
@@ -135,15 +139,19 @@
 
 async def async_subprocess_wrapper(cmd: str) -> CommandOutput:
     logger.debug('Execute command: `' + cmd + '`')
     proc = await asyncio.subprocess.create_subprocess_shell(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
     # it's safe to assume that the return code is not None at this point
     return_code: int = 1 if proc.returncode is None else proc.returncode
     stdout, stderr = await proc.communicate()
-    stdout = stdout.decode()
+    # Fix #32
+    stdout = stdout.decode().replace(
+        '(is_nvidia_einval_bug          ) nvida/i2c-dev bug encountered. Forcing future io I2C_IO_STRATEGY_FILEIO. '
+        'Retrying\n', ''
+    )
     stderr = stderr.decode()
     command_output = {
         'returnCode': return_code,
         'stdout': stdout,
         'stderr': stderr,
     }
```

### Comparing `ddcci_plasmoid_backend-0.1.5/PKG-INFO` & `ddcci_plasmoid_backend-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddcci-plasmoid-backend
-Version: 0.1.5
+Version: 0.1.6
 Summary: Backend for ddcci-plasmoid
 Home-page: https://github.com/davidhi7/ddcci-plasmoid
 License: MIT
 Keywords: ddcci,brightmess,widget,kde,plasma
 Author: David Himmelstoß
 Author-email: 77309510+davidhi7@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
@@ -19,15 +19,15 @@
 Classifier: Topic :: System :: Hardware
 Requires-Dist: fasteners (>=0.18,<0.19)
 Project-URL: Repository, https://github.com/davidhi7/ddcci-plasmoid
 Description-Content-Type: text/markdown
 
 # KDE Plasma Widget for external monitor brightness adjustment
 
-![Screenshot](./banner.png)
+![Screenshot](https://raw.githubusercontent.com/davidhi7/ddcci-plasmoid/main/screenshots/banner.png)
 
 * This widget allows you to adjust the brightness of external monitors. We accomplish that using [DDC/CI](https://en.wikipedia.org/wiki/Display_Data_Channel#DDC/CI), a protocol that allows your computer to control monitors and change options like the brightness or contrast.
 * A seamless integration into the Plasma desktop is a major goal of this project. The widget is versatile and can be used as a standalone widget or integrated into the system tray.
 * Notebook monitors are currently unsupported because they use different interfaces to communicate with the operating system.
 
 ## Requirements
```

