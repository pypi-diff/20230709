# Comparing `tmp/task2a-1.0.5.tar.gz` & `tmp/task2a-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "task2a-1.0.5.tar", max compression
+gzip compressed data, was "task2a-1.0.6.tar", max compression
```

## Comparing `task2a-1.0.5.tar` & `task2a-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      466 2023-07-08 14:31:48.331141 task2a-1.0.5/LICENSE
--rw-r--r--   0        0        0      318 2023-07-07 02:48:43.371622 task2a-1.0.5/pwgen/__init__.py
--rw-r--r--   0        0        0      112 2023-07-07 02:48:43.371622 task2a-1.0.5/pwgen/__main__.py
--rw-r--r--   0        0        0       23 2023-07-08 14:55:03.254233 task2a-1.0.5/pwgen/__version__.py
--rw-r--r--   0        0        0       73 2023-07-07 02:48:43.372616 task2a-1.0.5/pwgen/cli/__init__.py
--rw-r--r--   0        0        0      112 2023-07-07 02:48:43.372616 task2a-1.0.5/pwgen/cli/__main__.py
--rw-r--r--   0        0        0     4614 2023-07-07 02:48:43.373616 task2a-1.0.5/pwgen/cli/cli.py
--rw-r--r--   0        0        0     8361 2023-07-07 02:48:43.373616 task2a-1.0.5/pwgen/pwgen.py
--rw-r--r--   0        0        0       93 2023-07-07 02:48:43.374623 task2a-1.0.5/pwgen/showcase/__init__.py
--rw-r--r--   0        0        0      132 2023-07-07 02:48:43.374623 task2a-1.0.5/pwgen/showcase/__main__.py
--rw-r--r--   0        0        0       99 2023-07-07 02:48:43.374623 task2a-1.0.5/pwgen/showcase/pattern-list-error.txt
--rw-r--r--   0        0        0      175 2023-07-07 02:48:43.374623 task2a-1.0.5/pwgen/showcase/pattern-list.txt
--rw-r--r--   0        0        0    19900 2023-07-07 02:48:43.375617 task2a-1.0.5/pwgen/showcase/showcase.py
--rw-r--r--   0        0        0      464 2023-07-08 14:54:53.554281 task2a-1.0.5/pyproject.toml
--rw-r--r--   0        0        0    37308 2023-07-08 14:50:33.812561 task2a-1.0.5/README.md
--rw-r--r--   0        0        0    37105 1970-01-01 00:00:00.000000 task2a-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0      466 2023-07-08 14:31:48.331141 task2a-1.0.6/LICENSE
+-rw-r--r--   0        0        0      318 2023-07-07 02:48:43.371622 task2a-1.0.6/pwgen/__init__.py
+-rw-r--r--   0        0        0      112 2023-07-07 02:48:43.371622 task2a-1.0.6/pwgen/__main__.py
+-rw-r--r--   0        0        0       23 2023-07-09 09:07:17.243436 task2a-1.0.6/pwgen/__version__.py
+-rw-r--r--   0        0        0       73 2023-07-07 02:48:43.372616 task2a-1.0.6/pwgen/cli/__init__.py
+-rw-r--r--   0        0        0      112 2023-07-07 02:48:43.372616 task2a-1.0.6/pwgen/cli/__main__.py
+-rw-r--r--   0        0        0     4614 2023-07-07 02:48:43.373616 task2a-1.0.6/pwgen/cli/cli.py
+-rw-r--r--   0        0        0     8365 2023-07-08 17:58:50.053775 task2a-1.0.6/pwgen/pwgen.py
+-rw-r--r--   0        0        0       93 2023-07-07 02:48:43.374623 task2a-1.0.6/pwgen/showcase/__init__.py
+-rw-r--r--   0        0        0      132 2023-07-07 02:48:43.374623 task2a-1.0.6/pwgen/showcase/__main__.py
+-rw-r--r--   0        0        0       99 2023-07-07 02:48:43.374623 task2a-1.0.6/pwgen/showcase/pattern-list-error.txt
+-rw-r--r--   0        0        0      175 2023-07-07 02:48:43.374623 task2a-1.0.6/pwgen/showcase/pattern-list.txt
+-rw-r--r--   0        0        0    19898 2023-07-09 09:07:01.939357 task2a-1.0.6/pwgen/showcase/showcase.py
+-rw-r--r--   0        0        0      464 2023-07-09 09:07:17.238442 task2a-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0    37308 2023-07-08 14:50:33.812561 task2a-1.0.6/README.md
+-rw-r--r--   0        0        0    37105 1970-01-01 00:00:00.000000 task2a-1.0.6/PKG-INFO
```

### Comparing `task2a-1.0.5/pwgen/cli/cli.py` & `task2a-1.0.6/pwgen/cli/cli.py`

 * *Files identical despite different names*

### Comparing `task2a-1.0.5/pwgen/pwgen.py` & `task2a-1.0.6/pwgen/pwgen.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,16 +114,16 @@
 def generate_password_from_pattern(pattern: str) -> str:
     if type(pattern) is not str:  # Initial checks
         logger.error(f'Incorrect pattern {pattern}. String expected.')
         return ''
     elif not pattern:
         logger.error(f'Pattern cannot be empty')
         return ''
-    elif pattern.find(' ') != -1:
-        logger.error(f'You cannot use space symbol in pattern ({pattern})')
+    # elif pattern.find(' ') != -1:
+    #     logger.error(f'You cannot use space symbol in pattern ({pattern})')
 
     # Convert \{ \} \[ \] to the { } [ ]. It could be an error, but it's a minor error. Just sanitize string.
     n_pattern = pattern.replace('\\{', '{').replace('\\}', '}').replace('\\[', '[').replace('\\]', ']')
 
     if n_pattern[0] == '{':
         logger.error(f'Incorrect utilization of braces in the pattern ({pattern}) due to braces cannot come first')
         return ''
```

### Comparing `task2a-1.0.5/pwgen/showcase/showcase.py` & `task2a-1.0.6/pwgen/showcase/showcase.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         'validation': lambda val: True if val.isdigit() else 'Please, provide a number',
     },
     'f': {
         'descr': 'f',
         'type': 'path',
         'message': 'Which file would you like to use?',
         'validation': lambda val: True if val else 'Please, provide a path to the file',
-        'default': f'{os.path.dirname(os.path.abspath(__file__))}\\pattern-list.txt',
+        'default': f'{os.path.dirname(os.path.abspath(__file__))}/pattern-list.txt',
         'filter': lambda val: f'"{val}"' if val else val,
     },
     'f_out': {
         'descr': 'f',
         'type': 'path',
         'message': 'In which file would you like to write generated passwords (it may be new)?',
         'validation': lambda val: True if val else 'Please specify the path to the file',
@@ -78,15 +78,15 @@
         'filter': lambda val: f'"{val}"' if val else val,
     },
     'f_err': {
         'descr': 'f',
         'type': 'path',
         'message': 'Which file would you like to use?',
         'validation': lambda val: True if val else 'Please, provide a path to the file',
-        'default': f'{os.path.dirname(os.path.abspath(__file__))}\\pattern-list-error.txt',
+        'default': f'{os.path.dirname(os.path.abspath(__file__))}/pattern-list-error.txt',
         'filter': lambda val: f'"{val}"' if val else val,
     },
     'c': {
         'descr': 'c',
         'type': 'text',
         'message': 'What amount of passwords would you like to get?',
         'default': '1',
```

### Comparing `task2a-1.0.5/README.md` & `task2a-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `task2a-1.0.5/PKG-INFO` & `task2a-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: task2a
-Version: 1.0.5
+Version: 1.0.6
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
-Metadata-Version: 2.1 Name: task2a Version: 1.0.5 Summary: License: MIT Author:
+Metadata-Version: 2.1 Name: task2a Version: 1.0.6 Summary: License: MIT Author:
 Bill.Avramenko Author-email: billavramenko@gmail.com Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-Dist:
 questionary (>=1.10.0,<2.0.0) Description-Content-Type: text/markdown
                     [EPAM_DevOps-7_Internal_Lab_title_logo]
                               Password generator.
```

