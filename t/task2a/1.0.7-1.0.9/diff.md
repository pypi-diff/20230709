# Comparing `tmp/task2a-1.0.7.tar.gz` & `tmp/task2a-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "task2a-1.0.7.tar", max compression
+gzip compressed data, was "task2a-1.0.9.tar", max compression
```

## Comparing `task2a-1.0.7.tar` & `task2a-1.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      466 2023-07-08 14:31:48.331141 task2a-1.0.7/LICENSE
--rw-r--r--   0        0        0      318 2023-07-07 02:48:43.371622 task2a-1.0.7/pwgen/__init__.py
--rw-r--r--   0        0        0      112 2023-07-07 02:48:43.371622 task2a-1.0.7/pwgen/__main__.py
--rw-r--r--   0        0        0       23 2023-07-09 09:41:08.173542 task2a-1.0.7/pwgen/__version__.py
--rw-r--r--   0        0        0       73 2023-07-07 02:48:43.372616 task2a-1.0.7/pwgen/cli/__init__.py
--rw-r--r--   0        0        0      112 2023-07-07 02:48:43.372616 task2a-1.0.7/pwgen/cli/__main__.py
--rw-r--r--   0        0        0     4614 2023-07-07 02:48:43.373616 task2a-1.0.7/pwgen/cli/cli.py
--rw-r--r--   0        0        0     8365 2023-07-08 17:58:50.053775 task2a-1.0.7/pwgen/pwgen.py
--rw-r--r--   0        0        0       93 2023-07-07 02:48:43.374623 task2a-1.0.7/pwgen/showcase/__init__.py
--rw-r--r--   0        0        0      132 2023-07-07 02:48:43.374623 task2a-1.0.7/pwgen/showcase/__main__.py
--rw-r--r--   0        0        0       99 2023-07-07 02:48:43.374623 task2a-1.0.7/pwgen/showcase/pattern-list-error.txt
--rw-r--r--   0        0        0      175 2023-07-07 02:48:43.374623 task2a-1.0.7/pwgen/showcase/pattern-list.txt
--rw-r--r--   0        0        0    20398 2023-07-09 09:40:26.981355 task2a-1.0.7/pwgen/showcase/showcase.py
--rw-r--r--   0        0        0      464 2023-07-09 09:41:08.167543 task2a-1.0.7/pyproject.toml
--rw-r--r--   0        0        0    37308 2023-07-08 14:50:33.812561 task2a-1.0.7/README.md
--rw-r--r--   0        0        0    37105 1970-01-01 00:00:00.000000 task2a-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0      466 2023-07-08 14:31:48.331141 task2a-1.0.9/LICENSE
+-rw-r--r--   0        0        0      318 2023-07-07 02:48:43.371622 task2a-1.0.9/pwgen/__init__.py
+-rw-r--r--   0        0        0      112 2023-07-07 02:48:43.371622 task2a-1.0.9/pwgen/__main__.py
+-rw-r--r--   0        0        0       23 2023-07-09 17:26:14.017024 task2a-1.0.9/pwgen/__version__.py
+-rw-r--r--   0        0        0       73 2023-07-07 02:48:43.372616 task2a-1.0.9/pwgen/cli/__init__.py
+-rw-r--r--   0        0        0      112 2023-07-07 02:48:43.372616 task2a-1.0.9/pwgen/cli/__main__.py
+-rw-r--r--   0        0        0     4614 2023-07-07 02:48:43.373616 task2a-1.0.9/pwgen/cli/cli.py
+-rw-r--r--   0        0        0     8365 2023-07-08 17:58:50.053775 task2a-1.0.9/pwgen/pwgen.py
+-rw-r--r--   0        0        0       93 2023-07-07 02:48:43.374623 task2a-1.0.9/pwgen/showcase/__init__.py
+-rw-r--r--   0        0        0      132 2023-07-07 02:48:43.374623 task2a-1.0.9/pwgen/showcase/__main__.py
+-rw-r--r--   0        0        0       99 2023-07-07 02:48:43.374623 task2a-1.0.9/pwgen/showcase/pattern-list-error.txt
+-rw-r--r--   0        0        0      175 2023-07-09 17:21:49.870912 task2a-1.0.9/pwgen/showcase/pattern-list.txt
+-rw-r--r--   0        0        0    20398 2023-07-09 09:40:26.981355 task2a-1.0.9/pwgen/showcase/showcase.py
+-rw-r--r--   0        0        0      667 2023-07-09 17:26:14.006028 task2a-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0    37308 2023-07-08 14:50:33.812561 task2a-1.0.9/README.md
+-rw-r--r--   0        0        0    37290 1970-01-01 00:00:00.000000 task2a-1.0.9/PKG-INFO
```

### Comparing `task2a-1.0.7/pwgen/cli/cli.py` & `task2a-1.0.9/pwgen/cli/cli.py`

 * *Files identical despite different names*

### Comparing `task2a-1.0.7/pwgen/pwgen.py` & `task2a-1.0.9/pwgen/pwgen.py`

 * *Files identical despite different names*

### Comparing `task2a-1.0.7/pwgen/showcase/showcase.py` & `task2a-1.0.9/pwgen/showcase/showcase.py`

 * *Files identical despite different names*

### Comparing `task2a-1.0.7/README.md` & `task2a-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `task2a-1.0.7/PKG-INFO` & `task2a-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: task2a
-Version: 1.0.7
-Summary: 
+Version: 1.0.9
+Summary: Password generation CLI and library
+Home-page: https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/task2a
 License: MIT
 Author: Bill.Avramenko
 Author-email: billavramenko@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
+Project-URL: Repository, https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/task2a
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://gitlab.com/Bill-EPAM-DevOpsInt2023/devops-7-avramenko-bill">
     <img src="https://gitlab.com/EPAM-DevOpsInt2023/devops-7-assets/-/raw/ecd2eb07b44c03c4bcdf5493b45fe46238a12e14/shared/images/title-logo-origin.svg" alt="EPAM DevOps-7 Internal Lab title logo" width="100%" height="300px">
   </a>
 </p>
```

#### html2text {}

```diff
@@ -1,13 +1,16 @@
-Metadata-Version: 2.1 Name: task2a Version: 1.0.7 Summary: License: MIT Author:
-Bill.Avramenko Author-email: billavramenko@gmail.com Requires-Python:
->=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-Dist:
-questionary (>=1.10.0,<2.0.0) Description-Content-Type: text/markdown
+Metadata-Version: 2.1 Name: task2a Version: 1.0.9 Summary: Password generation
+CLI and library Home-page: https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/
+task2a License: MIT Author: Bill.Avramenko Author-email:
+billavramenko@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
+Approved :: MIT License Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Requires-Dist: questionary (>=1.10.0,<2.0.0)
+Project-URL: Repository, https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/
+task2a Description-Content-Type: text/markdown
                     [EPAM_DevOps-7_Internal_Lab_title_logo]
                               Password generator.
                           Module 2: Python. Task 2A.
                  [PYPI_v.]  [License]  [License]  [Python_v.] 
 ## Preface This project contains a solution to one of the tasks of the EPAM
 DevOps Initial Internal Training Course #7 in 2023. Detailed information about
 the course, as well as reports on each of the completed tasks (including this
```

