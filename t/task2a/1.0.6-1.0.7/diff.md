# Comparing `tmp/task2a-1.0.6.tar.gz` & `tmp/task2a-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "task2a-1.0.6.tar", max compression
+gzip compressed data, was "task2a-1.0.7.tar", max compression
```

## Comparing `task2a-1.0.6.tar` & `task2a-1.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      466 2023-07-08 14:31:48.331141 task2a-1.0.6/LICENSE
--rw-r--r--   0        0        0      318 2023-07-07 02:48:43.371622 task2a-1.0.6/pwgen/__init__.py
--rw-r--r--   0        0        0      112 2023-07-07 02:48:43.371622 task2a-1.0.6/pwgen/__main__.py
--rw-r--r--   0        0        0       23 2023-07-09 09:07:17.243436 task2a-1.0.6/pwgen/__version__.py
--rw-r--r--   0        0        0       73 2023-07-07 02:48:43.372616 task2a-1.0.6/pwgen/cli/__init__.py
--rw-r--r--   0        0        0      112 2023-07-07 02:48:43.372616 task2a-1.0.6/pwgen/cli/__main__.py
--rw-r--r--   0        0        0     4614 2023-07-07 02:48:43.373616 task2a-1.0.6/pwgen/cli/cli.py
--rw-r--r--   0        0        0     8365 2023-07-08 17:58:50.053775 task2a-1.0.6/pwgen/pwgen.py
--rw-r--r--   0        0        0       93 2023-07-07 02:48:43.374623 task2a-1.0.6/pwgen/showcase/__init__.py
--rw-r--r--   0        0        0      132 2023-07-07 02:48:43.374623 task2a-1.0.6/pwgen/showcase/__main__.py
--rw-r--r--   0        0        0       99 2023-07-07 02:48:43.374623 task2a-1.0.6/pwgen/showcase/pattern-list-error.txt
--rw-r--r--   0        0        0      175 2023-07-07 02:48:43.374623 task2a-1.0.6/pwgen/showcase/pattern-list.txt
--rw-r--r--   0        0        0    19898 2023-07-09 09:07:01.939357 task2a-1.0.6/pwgen/showcase/showcase.py
--rw-r--r--   0        0        0      464 2023-07-09 09:07:17.238442 task2a-1.0.6/pyproject.toml
--rw-r--r--   0        0        0    37308 2023-07-08 14:50:33.812561 task2a-1.0.6/README.md
--rw-r--r--   0        0        0    37105 1970-01-01 00:00:00.000000 task2a-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0      466 2023-07-08 14:31:48.331141 task2a-1.0.7/LICENSE
+-rw-r--r--   0        0        0      318 2023-07-07 02:48:43.371622 task2a-1.0.7/pwgen/__init__.py
+-rw-r--r--   0        0        0      112 2023-07-07 02:48:43.371622 task2a-1.0.7/pwgen/__main__.py
+-rw-r--r--   0        0        0       23 2023-07-09 09:41:08.173542 task2a-1.0.7/pwgen/__version__.py
+-rw-r--r--   0        0        0       73 2023-07-07 02:48:43.372616 task2a-1.0.7/pwgen/cli/__init__.py
+-rw-r--r--   0        0        0      112 2023-07-07 02:48:43.372616 task2a-1.0.7/pwgen/cli/__main__.py
+-rw-r--r--   0        0        0     4614 2023-07-07 02:48:43.373616 task2a-1.0.7/pwgen/cli/cli.py
+-rw-r--r--   0        0        0     8365 2023-07-08 17:58:50.053775 task2a-1.0.7/pwgen/pwgen.py
+-rw-r--r--   0        0        0       93 2023-07-07 02:48:43.374623 task2a-1.0.7/pwgen/showcase/__init__.py
+-rw-r--r--   0        0        0      132 2023-07-07 02:48:43.374623 task2a-1.0.7/pwgen/showcase/__main__.py
+-rw-r--r--   0        0        0       99 2023-07-07 02:48:43.374623 task2a-1.0.7/pwgen/showcase/pattern-list-error.txt
+-rw-r--r--   0        0        0      175 2023-07-07 02:48:43.374623 task2a-1.0.7/pwgen/showcase/pattern-list.txt
+-rw-r--r--   0        0        0    20398 2023-07-09 09:40:26.981355 task2a-1.0.7/pwgen/showcase/showcase.py
+-rw-r--r--   0        0        0      464 2023-07-09 09:41:08.167543 task2a-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0    37308 2023-07-08 14:50:33.812561 task2a-1.0.7/README.md
+-rw-r--r--   0        0        0    37105 1970-01-01 00:00:00.000000 task2a-1.0.7/PKG-INFO
```

### Comparing `task2a-1.0.6/pwgen/cli/cli.py` & `task2a-1.0.7/pwgen/cli/cli.py`

 * *Files identical despite different names*

### Comparing `task2a-1.0.6/pwgen/pwgen.py` & `task2a-1.0.7/pwgen/pwgen.py`

 * *Files identical despite different names*

### Comparing `task2a-1.0.6/pwgen/showcase/showcase.py` & `task2a-1.0.7/pwgen/showcase/showcase.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import argparse
 import os
+import platform
 import subprocess
 import sys
 import time
 from typing import Dict, List
 
 import questionary
 import select
@@ -30,14 +31,23 @@
        ██    ██   ██ ██      ██  ██           ██ ██   ██            
        ██    ███████ ███████ █████        █████  ███████            
        ██    ██   ██      ██ ██  ██      ██      ██   ██            
        ██    ██   ██ ███████ ██   ██     ███████ ██   ██
 '''
 
 
+# Determine the platform
+current_platform = platform.system()
+
+# Set the Python command based on the platform
+if current_platform == 'Windows':
+    python_command = 'python -m'
+else:
+    python_command = 'python3 -m'
+
 select_style = questionary.Style([
     #     ('default', "bg:#ffffff fg:#000000"),
     # ('selected', 'bg:#336699 fg:#ffffff'),
     ('highlighted', '#008888'),
     ('pointer', '#008888'),
     # ('question', 'fg:#009b06'),
     ('qmark', 'fg:#009b06'),
@@ -112,143 +122,143 @@
 OPTIONS: Dict[str, Dict[str, str | List[Dict] | Dict[str, Dict[str, str | List[Dict]]]]] = {
     'charset': {
         'descr': 'character sets',
         'options': {
             'charset_default': {
                 'descr': 'default charset',
                 'command': 'pwgen -n{} -c{} {}',
-                'module_command': 'python -m pwgen -n{} -c{} {}',
+                'module_command': f'{python_command} pwgen -n{{}} -c{{}} {{}}',
                 'arguments': [OPTIONS_ARGUMENTS['n'], OPTIONS_ARGUMENTS['c'], OPTIONS_ARGUMENTS['v'], ],
             },
             'charset_custom': {
                 'descr': 'custom charset based on default',
                 'command': 'pwgen -S dp -n{} -c{} {}',
-                'module_command': 'python -m pwgen -S dp -n{} -c{} {}',
+                'module_command': f'{python_command} pwgen -S dp -n{{}} -c{{}} {{}}',
                 'arguments': [OPTIONS_ARGUMENTS['n'], OPTIONS_ARGUMENTS['c'], OPTIONS_ARGUMENTS['v'], ],
             },
             'charset_additional': {
                 'descr': 'custom charset with additional symbols',
                 'command': 'pwgen -S "u\\@\\$\\%\\&\\#\\*\\!" -n{} -c{} {}',
-                'module_command': 'python -m pwgen -S "u\\@\\$\\%\\&\\#\\*\\!" -n{} -c{} {}',
+                'module_command': f'{python_command} pwgen -S "u\\@\\$\\%\\&\\#\\*\\!" -n{{}} -c{{}} {{}}',
                 'arguments': [OPTIONS_ARGUMENTS['n'], OPTIONS_ARGUMENTS['c'], OPTIONS_ARGUMENTS['v'], ],
             },
             'charset_exclusions': {
                 'descr': 'custom charset with exclusions',
                 'command': 'pwgen -S "Ld^l^\\4^\\5^\\6^\\7^\\8" -n{} -c{} {}',
-                'module_command': 'python -m pwgen -S "Ld^l^\\4^\\5^\\6^\\7^\\8" -n{} -c{} {}',
+                'module_command': f'{python_command} pwgen -S "Ld^l^\\4^\\5^\\6^\\7^\\8" -n{{}} -c{{}} {{}}',
                 'arguments': [OPTIONS_ARGUMENTS['n'], OPTIONS_ARGUMENTS['c'], OPTIONS_ARGUMENTS['v'], ],
             },
         },
     },
     'pattern': {
         'descr': 'pattern-based approach',
         'options': {
             'pattern_default': {
                 'descr': 'pattern based on a default charset',
                 'command': 'pwgen -t uupllddL -c{} {} {}',
-                'module_command': 'python -m pwgen -t uupllddL -c{} {} {}',
+                'module_command': f'{python_command} pwgen -t uupllddL -c{{}} {{}} {{}}',
                 'arguments': [OPTIONS_ARGUMENTS['c'], OPTIONS_ARGUMENTS['p'], OPTIONS_ARGUMENTS['v'], ],
             },
             'pattern_multiply': {
                 'descr': 'pattern with placeholder multiplication',
                 'command': 'pwgen -t u{{2}}p{{5}}l{{2}}d{{2}}L -c{} {} {}',
-                'module_command': 'python -m pwgen -t u{{2}}p{{5}}l{{2}}d{{2}}L -c{} {} {}',
+                'module_command': f'{python_command} pwgen -t u{{2}}p{{5}}l{{2}}d{{2}}L -c{{}} {{}} {{}}',
                 'arguments': [OPTIONS_ARGUMENTS['c'], OPTIONS_ARGUMENTS['p'], OPTIONS_ARGUMENTS['v'], ],
             },
             'pattern_specific': {
                 'descr': 'pattern with a specific symbol placeholder',
                 'command': 'pwgen -t "u{{4}}d{{3}}\\-l{{2}}" -c{} {} {}',
-                'module_command': 'python -m pwgen -t "u{{4}}d{{3}}\\-l{{2}}" -c{} {} {}',
+                'module_command': f'{python_command} pwgen -t "u{{4}}d{{3}}\\-l{{2}}" -c{{}} {{}} {{}}',
                 'arguments': [OPTIONS_ARGUMENTS['c'], OPTIONS_ARGUMENTS['p'], OPTIONS_ARGUMENTS['v'], ],
             },
             'pattern_custom_charset': {
                 'descr': 'pattern with a custom charset placeholder',
                 'command': 'pwgen -t u{{4}}[pd]{{3}}l{{2}} -c{} {} {}',
-                'module_command': 'python -m pwgen -t u{{4}}[pd]{{3}}l{{2}} -c{} {} {}',
+                'module_command': f'{python_command} pwgen -t u{{4}}[pd]{{3}}l{{2}} -c{{}} {{}} {{}}',
                 'arguments': [OPTIONS_ARGUMENTS['c'], OPTIONS_ARGUMENTS['p'], OPTIONS_ARGUMENTS['v'], ],
             },
             'pattern_custom_charset_specific': {
                 'descr': 'pattern with a custom charset with a specific symbol placeholder',
                 'command': 'pwgen -t "u{{4}}[pd\\@\\$\\%\\&\\#\\*\\!]{{3}}l{{2}}" -c{} {} {}',
-                'module_command': 'python -m pwgen -t "u{{4}}[pd\\@\\$\\%\\&\\#\\*\\!]{{3}}l{{2}}" -c{} {} {}',
+                'module_command': f'{python_command} pwgen -t "u{{4}}[pd\\@\\$\\%\\&\\#\\*\\!]{{3}}l{{2}}" -c{{}} {{}} {{}}',
                 'arguments': [OPTIONS_ARGUMENTS['c'], OPTIONS_ARGUMENTS['p'], OPTIONS_ARGUMENTS['v'], ],
             },
             'pattern_custom_charset_exclusions': {
                 'descr': 'pattern with a custom charset placeholder with exclusions',
                 'command': 'pwgen -t "u{{4}}[Ld^l^\\4^\\5^\\6^\\7^\\8]{{3}}l{{2}}" -c{} {} {}',
-                'module_command': 'python -m pwgen -t "u{{4}}[Ld^l^\\4^\\5^\\6^\\7^\\8]{{3}}l{{2}}" -c{} {} {}',
+                'module_command': f'{python_command} pwgen -t "u{{4}}[Ld^l^\\4^\\5^\\6^\\7^\\8]{{3}}l{{2}}" -c{{}} {{}} {{}}',
                 'arguments': [OPTIONS_ARGUMENTS['c'], OPTIONS_ARGUMENTS['p'], OPTIONS_ARGUMENTS['v'], ],
             },
             'pattern_complex': {
                 'descr': 'complex pattern',
                 'command':
                     'pwgen -t "u{{4}}\\-[Ld^l^\\4^\\5^\\6^\\7^\\8\\@\\$\\%\\&\\#\\*\\!]{{3}}l{{2}}" -c{} {} {}',
                 'module_command':
-                    'python -m pwgen -t "u{{4}}\\-[Ld^l^\\4^\\5^\\6^\\7^\\8\\@\\$\\%\\&\\#\\*\\!]{{3}}l{{2}}" -c{} {} {}',
+                    f'{python_command} pwgen -t "u{{4}}\\-[Ld^l^\\4^\\5^\\6^\\7^\\8\\@\\$\\%\\&\\#\\*\\!]{{3}}l{{2}}" -c{{}} {{}} {{}}',
                 'arguments': [OPTIONS_ARGUMENTS['c'], OPTIONS_ARGUMENTS['p'], OPTIONS_ARGUMENTS['v'], ],
             },
         },
     },
     'file': {
         'descr': 'pattern from a file',
         'command': 'pwgen -f {} -c{} {} {}',
-        'module_command': 'python -m pwgen -f {} -c{} {} {}',
+        'module_command': f'{python_command} pwgen -f {{}} -c{{}} {{}} {{}}',
         'arguments': [OPTIONS_ARGUMENTS['f'], OPTIONS_ARGUMENTS['c'],
                       OPTIONS_ARGUMENTS['p'], OPTIONS_ARGUMENTS['v'], ],
     },
     'pipe': {
         'descr': 'pipes with the pwgen command',
         'options': {
             'pipe_stdin': {
                 'descr': 'pipe stdin from a file',
                 'command': 'cat {} | pwgen -c{} {} {}',
-                'module_command': 'cat {} | python -m pwgen -c{} {} {}',
+                'module_command': f'cat {{}} | {python_command} pwgen -c{{}} {{}} {{}}',
                 'arguments': [OPTIONS_ARGUMENTS['f'], OPTIONS_ARGUMENTS['c'],
                               OPTIONS_ARGUMENTS['p'], OPTIONS_ARGUMENTS['v'], ],
             },
             'pipe_stdout': {
                 'descr': 'pipe stdout to a file',
                 'command': 'pwgen -S "Ld^l^\\4^\\5^\\6^\\7^\\8" -n{} -c{} {} > {}',
-                'module_command': 'python -m pwgen -S "Ld^l^\\4^\\5^\\6^\\7^\\8" -n{} -c{} {} > {}',
+                'module_command': f'{python_command} pwgen -S "Ld^l^\\4^\\5^\\6^\\7^\\8" -n{{}} -c{{}} {{}} > {{}}',
                 'arguments': [OPTIONS_ARGUMENTS['n'], OPTIONS_ARGUMENTS['c'],
                               OPTIONS_ARGUMENTS['v'], OPTIONS_ARGUMENTS['f_out'], ],
             },
             'pipe_stderr': {
                 'descr': 'pipe stderr to a file',
                 'command': 'pwgen -S "Ld^l^\\4^\\5^\\6^\\7^\\8" {} 2> {}',
-                'module_command': 'python -m pwgen -S "Ld^l^\\4^\\5^\\6^\\7^\\8" {} 2> {}',
+                'module_command': f'{python_command} pwgen -S "Ld^l^\\4^\\5^\\6^\\7^\\8" {{}} 2> {{}}',
                 'arguments': [OPTIONS_ARGUMENTS['v'], OPTIONS_ARGUMENTS['f_log'], ],
             },
             'pipe_complex': {
                 'descr': 'complex pipe with a sort command',
                 'command': 'echo u{{4}}[Ld^l^\\4^\\5^\\6^\\7^\\8]{{3}}l{{2}} | pwgen -c6 {} | sort -r',
-                'module_command': 'echo u{{4}}[Ld^l^\\4^\\5^\\6^\\7^\\8]{{3}}l{{2}} | python -m pwgen -c6 {} | sort -r',
+                'module_command': f'echo u{{4}}[Ld^l^\\4^\\5^\\6^\\7^\\8]{{3}}l{{2}} | {python_command} pwgen -c6 {{}} | sort -r',
                 'arguments': [OPTIONS_ARGUMENTS['v'], ],
             },
         }
     },
     'with_errors': {
         'descr': 'patterns and character sets with errors',
         'options': {
             'charset_error': {
                 'descr': 'custom charset with an error',
                 'command': 'pwgen -S "Ld^lwkr^\\4^\\5^\\6^\\7^\\8" {}',
-                'module_command': 'python -m pwgen -S "Ld^lwkr^\\4^\\5^\\6^\\7^\\8" {}',
+                'module_command': f'{python_command} pwgen -S "Ld^lwkr^\\4^\\5^\\6^\\7^\\8" {{}}',
                 'arguments': [OPTIONS_ARGUMENTS['v'], ],
             },
             'pattern_error': {
                 'descr': 'pattern with an error placeholder',
                 'command': 'pwgen -t "{{5}}Ld^l^\\4^\\5^\\6^\\7^\\8" {}',
-                'module_command': 'python -m pwgen -t "{{5}}Ld^l^\\4^\\5^\\6^\\7^\\8" {}',
+                'module_command': f'{python_command} pwgen -t "{{5}}Ld^l^\\4^\\5^\\6^\\7^\\8" {{}}',
                 'arguments': [OPTIONS_ARGUMENTS['v'], ],
             },
             'file_error': {
                 'descr': 'pattern with errors from a file',
                 'command': 'pwgen -f {} {}',
-                'module_command': 'python -m pwgen -f {} {}',
+                'module_command': f'{python_command} pwgen -f {{}} {{}}',
                 'arguments': [OPTIONS_ARGUMENTS['f_err'], OPTIONS_ARGUMENTS['v'], ],
             },
         }
     },
 }
 
 questions = [
```

### Comparing `task2a-1.0.6/README.md` & `task2a-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `task2a-1.0.6/PKG-INFO` & `task2a-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: task2a
-Version: 1.0.6
+Version: 1.0.7
 Summary: 
 License: MIT
 Author: Bill.Avramenko
 Author-email: billavramenko@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: task2a Version: 1.0.6 Summary: License: MIT Author:
+Metadata-Version: 2.1 Name: task2a Version: 1.0.7 Summary: License: MIT Author:
 Bill.Avramenko Author-email: billavramenko@gmail.com Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-Dist:
 questionary (>=1.10.0,<2.0.0) Description-Content-Type: text/markdown
                     [EPAM_DevOps-7_Internal_Lab_title_logo]
                               Password generator.
```

