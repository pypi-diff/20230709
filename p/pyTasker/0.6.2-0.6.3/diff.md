# Comparing `tmp/pyTasker-0.6.2.tar.gz` & `tmp/pyTasker-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyTasker-0.6.2.tar", last modified: Sat Jul  8 17:41:26 2023, max compression
+gzip compressed data, was "pyTasker-0.6.3.tar", last modified: Sun Jul  9 12:57:55 2023, max compression
```

## Comparing `pyTasker-0.6.2.tar` & `pyTasker-0.6.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 17:41:26.703878 pyTasker-0.6.2/
--rw-rw-rw-   0        0        0      305 2023-07-08 17:38:54.000000 pyTasker-0.6.2/.gitignore
--rw-rw-rw-   0        0        0     1115 2022-03-07 21:04:39.000000 pyTasker-0.6.2/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0      733 2022-03-07 21:04:39.000000 pyTasker-0.6.2/CHANGELOG.md
--rw-rw-rw-   0        0        0    35746 2022-02-03 21:25:58.000000 pyTasker-0.6.2/LICENSE
--rw-rw-rw-   0        0        0     7532 2023-07-08 17:41:26.704880 pyTasker-0.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     6460 2023-07-08 17:38:54.000000 pyTasker-0.6.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-08 17:41:26.687873 pyTasker-0.6.2/Tasker/
--rw-rw-rw-   0        0        0      569 2023-07-08 17:38:54.000000 pyTasker-0.6.2/Tasker/__init__.py
--rw-rw-rw-   0        0        0     3109 2023-07-08 17:38:54.000000 pyTasker-0.6.2/Tasker/__main__.py
--rw-rw-rw-   0        0        0       23 2023-07-08 17:40:40.000000 pyTasker-0.6.2/Tasker/__version__.py
--rw-rw-rw-   0        0        0     3554 2023-07-08 17:38:54.000000 pyTasker-0.6.2/Tasker/cli.py
--rw-rw-rw-   0        0        0     2712 2023-07-08 17:38:54.000000 pyTasker-0.6.2/Tasker/common.py
--rw-rw-rw-   0        0        0     2578 2022-03-07 21:04:39.000000 pyTasker-0.6.2/Tasker/inspector.py
--rw-rw-rw-   0        0        0    15270 2023-07-08 17:38:54.000000 pyTasker-0.6.2/Tasker/operations.py
--rw-rw-rw-   0        0        0    27172 2023-07-08 17:38:54.000000 pyTasker-0.6.2/Tasker/parser.py
--rw-rw-rw-   0        0        0     1315 2022-03-07 21:04:39.000000 pyTasker-0.6.2/Tasker/parser_test.py
--rw-rw-rw-   0        0        0    17710 2023-07-08 17:38:54.000000 pyTasker-0.6.2/Tasker/templater.py
--rw-rw-rw-   0        0        0     6966 2023-07-08 17:38:54.000000 pyTasker-0.6.2/Tasker/types.py
-drwxrwxrwx   0        0        0        0 2023-07-08 17:41:26.698878 pyTasker-0.6.2/pyTasker.egg-info/
--rw-rw-rw-   0        0        0     7532 2023-07-08 17:41:26.000000 pyTasker-0.6.2/pyTasker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      568 2023-07-08 17:41:26.000000 pyTasker-0.6.2/pyTasker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 17:41:26.000000 pyTasker-0.6.2/pyTasker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-07-08 17:41:26.000000 pyTasker-0.6.2/pyTasker.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       58 2023-07-08 17:41:26.000000 pyTasker-0.6.2/pyTasker.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-08 17:41:26.000000 pyTasker-0.6.2/pyTasker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      268 2022-03-07 21:04:39.000000 pyTasker-0.6.2/pyproject.toml
--rw-rw-rw-   0        0        0      113 2023-07-08 17:38:54.000000 pyTasker-0.6.2/requirements.txt
--rw-rw-rw-   0        0        0      191 2023-07-08 17:41:26.705876 pyTasker-0.6.2/setup.cfg
--rw-rw-rw-   0        0        0     1787 2023-07-08 17:40:40.000000 pyTasker-0.6.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 17:41:26.702882 pyTasker-0.6.2/static/
--rw-rw-rw-   0        0        0   424108 2022-02-03 21:25:58.000000 pyTasker-0.6.2/static/Copy PDFs then zip.png
--rw-rw-rw-   0        0        0   136520 2022-02-03 21:25:58.000000 pyTasker-0.6.2/static/Copy PDFs.png
+drwxrwxrwx   0        0        0        0 2023-07-09 12:57:55.472913 pyTasker-0.6.3/
+-rw-rw-rw-   0        0        0      305 2023-07-08 17:38:54.000000 pyTasker-0.6.3/.gitignore
+-rw-rw-rw-   0        0        0     1115 2022-03-07 21:04:39.000000 pyTasker-0.6.3/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0      733 2022-03-07 21:04:39.000000 pyTasker-0.6.3/CHANGELOG.md
+-rw-rw-rw-   0        0        0    35746 2022-02-03 21:25:58.000000 pyTasker-0.6.3/LICENSE
+-rw-rw-rw-   0        0        0     7532 2023-07-09 12:57:55.472913 pyTasker-0.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6460 2023-07-08 17:38:54.000000 pyTasker-0.6.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 12:57:55.426913 pyTasker-0.6.3/Tasker/
+-rw-rw-rw-   0        0        0      569 2023-07-08 17:38:54.000000 pyTasker-0.6.3/Tasker/__init__.py
+-rw-rw-rw-   0        0        0     3109 2023-07-08 17:38:54.000000 pyTasker-0.6.3/Tasker/__main__.py
+-rw-rw-rw-   0        0        0       23 2023-07-09 12:55:45.000000 pyTasker-0.6.3/Tasker/__version__.py
+-rw-rw-rw-   0        0        0     3554 2023-07-08 17:38:54.000000 pyTasker-0.6.3/Tasker/cli.py
+-rw-rw-rw-   0        0        0     2712 2023-07-08 17:38:54.000000 pyTasker-0.6.3/Tasker/common.py
+-rw-rw-rw-   0        0        0     2578 2022-03-07 21:04:39.000000 pyTasker-0.6.3/Tasker/inspector.py
+-rw-rw-rw-   0        0        0    15270 2023-07-08 17:38:54.000000 pyTasker-0.6.3/Tasker/operations.py
+-rw-rw-rw-   0        0        0    27430 2023-07-09 12:56:49.000000 pyTasker-0.6.3/Tasker/parser.py
+-rw-rw-rw-   0        0        0     1315 2022-03-07 21:04:39.000000 pyTasker-0.6.3/Tasker/parser_test.py
+-rw-rw-rw-   0        0        0    17710 2023-07-08 17:38:54.000000 pyTasker-0.6.3/Tasker/templater.py
+-rw-rw-rw-   0        0        0     6966 2023-07-08 17:38:54.000000 pyTasker-0.6.3/Tasker/types.py
+drwxrwxrwx   0        0        0        0 2023-07-09 12:57:55.466911 pyTasker-0.6.3/pyTasker.egg-info/
+-rw-rw-rw-   0        0        0     7532 2023-07-09 12:57:55.000000 pyTasker-0.6.3/pyTasker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      568 2023-07-09 12:57:55.000000 pyTasker-0.6.3/pyTasker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 12:57:55.000000 pyTasker-0.6.3/pyTasker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-09 12:57:55.000000 pyTasker-0.6.3/pyTasker.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       58 2023-07-09 12:57:55.000000 pyTasker-0.6.3/pyTasker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-09 12:57:55.000000 pyTasker-0.6.3/pyTasker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      268 2022-03-07 21:04:39.000000 pyTasker-0.6.3/pyproject.toml
+-rw-rw-rw-   0        0        0      113 2023-07-08 17:38:54.000000 pyTasker-0.6.3/requirements.txt
+-rw-rw-rw-   0        0        0      191 2023-07-09 12:57:55.474915 pyTasker-0.6.3/setup.cfg
+-rw-rw-rw-   0        0        0     1787 2023-07-09 12:55:40.000000 pyTasker-0.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 12:57:55.471915 pyTasker-0.6.3/static/
+-rw-rw-rw-   0        0        0   424108 2022-02-03 21:25:58.000000 pyTasker-0.6.3/static/Copy PDFs then zip.png
+-rw-rw-rw-   0        0        0   136520 2022-02-03 21:25:58.000000 pyTasker-0.6.3/static/Copy PDFs.png
```

### Comparing `pyTasker-0.6.2/.pre-commit-config.yaml` & `pyTasker-0.6.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.2/CHANGELOG.md` & `pyTasker-0.6.3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.2/LICENSE` & `pyTasker-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.2/PKG-INFO` & `pyTasker-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTasker
-Version: 0.6.2
+Version: 0.6.3
 Summary: Run pipelines on your own computer for better automation
 Home-page: https://github.com/carlossilva2/pyTasker
 Author: Carlos Silva
 Author-email: carlos.miguel.silva@protonmail.com
 License: GPLv3
 Project-URL: Source, https://github.com/carlossilva2/pyTasker
 Project-URL: Documentation, https://cmsilva.gitbook.io/pytasker/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyTasker Version: 0.6.2 Summary: Run pipelines on
+Metadata-Version: 2.1 Name: pyTasker Version: 0.6.3 Summary: Run pipelines on
 your own computer for better automation Home-page: https://github.com/
 carlossilva2/pyTasker Author: Carlos Silva Author-email:
 carlos.miguel.silva@protonmail.com License: GPLv3 Project-URL: Source, https://
 github.com/carlossilva2/pyTasker Project-URL: Documentation, https://
 cmsilva.gitbook.io/pytasker/ Platform: UNKNOWN Classifier: Development Status
 :: 4 - Beta Classifier: Environment :: Console Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: GNU General Public License v3
```

### Comparing `pyTasker-0.6.2/README.md` & `pyTasker-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.2/Tasker/__init__.py` & `pyTasker-0.6.3/Tasker/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.2/Tasker/__main__.py` & `pyTasker-0.6.3/Tasker/__main__.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.2/Tasker/cli.py` & `pyTasker-0.6.3/Tasker/cli.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.2/Tasker/common.py` & `pyTasker-0.6.3/Tasker/common.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.2/Tasker/inspector.py` & `pyTasker-0.6.3/Tasker/inspector.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.2/Tasker/operations.py` & `pyTasker-0.6.3/Tasker/operations.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.2/Tasker/parser.py` & `pyTasker-0.6.3/Tasker/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,30 +38,33 @@
     Settings,
     Task,
 )
 
 
 @implements(ParserType)
 class Parser(ParserType):
-    def __init__(self, task: str, logger: Logger) -> None:
+    def __init__(self, task: str, logger: Logger, abort_exit: bool = False) -> None:
+        self.abort_exit = abort_exit
         self.execution = {}
         t = Timer()
         t.start()
         self.supported_os = ["Windows"]  # List of Tasker supported OSes
         self.logger = logger
         if task not in self.list_all_tasks():
-            self.abort(f"'{task}' InstructionSet was not found")
+            self.abort(f"'{task}' InstructionSet was not found", abort=abort_exit)
         self.warn_user()
         self.__first_execution_routine()
         self.task: InstructionSet = json.load(
             open(f"{self.default_location}/{task}.tasker.json", "r")
         )
         analysis = self.__analyse_keys()
         if not analysis[0]:
-            self.abort(f'{analysis[3]} "{analysis[1]}" in {analysis[2]}')
+            self.abort(
+                f'{analysis[3]} "{analysis[1]}" in {analysis[2]}', abort=abort_exit
+            )
         self.__optional_parameters()
         self.settings = self.__get_configs()
         # load extensions
         self.extensions: List[CustomOperation] = self.__load_extensions()
         self.__change_relative_locations(self.settings["current_location"])
         self.__executed_tasks: List[Task] = []
         self.__operation_stack: List[OperationType] = []
@@ -103,17 +106,18 @@
                 pass
             elif ans.lower() == "n":
                 sys.exit(0)
             else:
                 self.logger.error("Answer not allowed. Aborting...")
                 sys.exit(1)
 
-    def abort(self, reason: str) -> None:
+    def abort(self, reason: str, abort: bool = False) -> None:
         self.logger.error(reason)
-        sys.exit(1)
+        if abort:
+            sys.exit(1)
 
     def __execute(self, task: Task) -> bool:
         try:
             self.__check_destination_path(task, DESTINATION_CHECK_MAP[task["operation"]])
             if task["operation"] == "copy":
                 c = Copy(self, task, self.logger)
                 self.__operation_stack.append(c)
@@ -149,15 +153,16 @@
             elif task["operation"] == "custom":
                 ex = next(
                     (e for e in self.extensions if e["summon"] == task["extension_name"]),
                     None,
                 )
                 if ex is None:
                     self.abort(
-                        f"No executable found with name {chalk.red(task['extension_name'])}"
+                        f"No executable found with name {chalk.red(task['extension_name'])}",
+                        self.abort_exit,
                     )
                 function: OperationType = ex["executable"].Extension(
                     self, task, self.logger
                 )
                 self.__operation_stack.append(function)
                 function.execute()
             else:
@@ -303,15 +308,16 @@
         modules: List[CustomOperation] = []
         for extension in self.settings["extensions"]:
             try:
                 spec: OperationType = importer(f"{extension['file'].replace('.py', '')}", extension["path"]).load_module()  # type: ignore
                 modules.append(CustomOperation(executable=spec, summon=extension["name"]))
             except Exception:
                 self.abort(
-                    f"There was a problem importing {chalk.yellow(extension['name'])} Custom Extension. Please revise code implementation"
+                    f"There was a problem importing {chalk.yellow(extension['name'])} Custom Extension. Please revise code implementation",
+                    self.abort_exit,
                 )
         return modules
 
     # Static Methods
 
     @staticmethod
     def do_config() -> None:
```

### Comparing `pyTasker-0.6.2/Tasker/parser_test.py` & `pyTasker-0.6.3/Tasker/parser_test.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.2/Tasker/templater.py` & `pyTasker-0.6.3/Tasker/templater.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.2/Tasker/types.py` & `pyTasker-0.6.3/Tasker/types.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.2/pyTasker.egg-info/PKG-INFO` & `pyTasker-0.6.3/pyTasker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTasker
-Version: 0.6.2
+Version: 0.6.3
 Summary: Run pipelines on your own computer for better automation
 Home-page: https://github.com/carlossilva2/pyTasker
 Author: Carlos Silva
 Author-email: carlos.miguel.silva@protonmail.com
 License: GPLv3
 Project-URL: Source, https://github.com/carlossilva2/pyTasker
 Project-URL: Documentation, https://cmsilva.gitbook.io/pytasker/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyTasker Version: 0.6.2 Summary: Run pipelines on
+Metadata-Version: 2.1 Name: pyTasker Version: 0.6.3 Summary: Run pipelines on
 your own computer for better automation Home-page: https://github.com/
 carlossilva2/pyTasker Author: Carlos Silva Author-email:
 carlos.miguel.silva@protonmail.com License: GPLv3 Project-URL: Source, https://
 github.com/carlossilva2/pyTasker Project-URL: Documentation, https://
 cmsilva.gitbook.io/pytasker/ Platform: UNKNOWN Classifier: Development Status
 :: 4 - Beta Classifier: Environment :: Console Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: GNU General Public License v3
```

### Comparing `pyTasker-0.6.2/pyTasker.egg-info/SOURCES.txt` & `pyTasker-0.6.3/pyTasker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.2/setup.py` & `pyTasker-0.6.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 setup(
     author="Carlos Silva",
     author_email="carlos.miguel.silva@protonmail.com",
     name="pyTasker",
     description="Run pipelines on your own computer for better automation",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="0.6.2",
+    version="0.6.3",
     url="https://github.com/carlossilva2/pyTasker",
     packages=find_packages(),
     license="GPLv3",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Intended Audience :: Developers",
```

### Comparing `pyTasker-0.6.2/static/Copy PDFs then zip.png` & `pyTasker-0.6.3/static/Copy PDFs then zip.png`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.2/static/Copy PDFs.png` & `pyTasker-0.6.3/static/Copy PDFs.png`

 * *Files identical despite different names*

