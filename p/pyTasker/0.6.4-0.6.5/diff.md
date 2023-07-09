# Comparing `tmp/pyTasker-0.6.4.tar.gz` & `tmp/pyTasker-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyTasker-0.6.4.tar", last modified: Sun Jul  9 13:02:06 2023, max compression
+gzip compressed data, was "pyTasker-0.6.5.tar", last modified: Sun Jul  9 13:10:38 2023, max compression
```

## Comparing `pyTasker-0.6.4.tar` & `pyTasker-0.6.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 13:02:06.044669 pyTasker-0.6.4/
--rw-rw-rw-   0        0        0      305 2023-07-08 17:38:54.000000 pyTasker-0.6.4/.gitignore
--rw-rw-rw-   0        0        0     1115 2022-03-07 21:04:39.000000 pyTasker-0.6.4/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0      733 2022-03-07 21:04:39.000000 pyTasker-0.6.4/CHANGELOG.md
--rw-rw-rw-   0        0        0    35746 2022-02-03 21:25:58.000000 pyTasker-0.6.4/LICENSE
--rw-rw-rw-   0        0        0     7532 2023-07-09 13:02:06.044669 pyTasker-0.6.4/PKG-INFO
--rw-rw-rw-   0        0        0     6460 2023-07-08 17:38:54.000000 pyTasker-0.6.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-09 13:02:06.010665 pyTasker-0.6.4/Tasker/
--rw-rw-rw-   0        0        0      569 2023-07-08 17:38:54.000000 pyTasker-0.6.4/Tasker/__init__.py
--rw-rw-rw-   0        0        0     3109 2023-07-08 17:38:54.000000 pyTasker-0.6.4/Tasker/__main__.py
--rw-rw-rw-   0        0        0       23 2023-07-09 13:01:14.000000 pyTasker-0.6.4/Tasker/__version__.py
--rw-rw-rw-   0        0        0     3554 2023-07-08 17:38:54.000000 pyTasker-0.6.4/Tasker/cli.py
--rw-rw-rw-   0        0        0     2712 2023-07-08 17:38:54.000000 pyTasker-0.6.4/Tasker/common.py
--rw-rw-rw-   0        0        0     2578 2022-03-07 21:04:39.000000 pyTasker-0.6.4/Tasker/inspector.py
--rw-rw-rw-   0        0        0    15270 2023-07-08 17:38:54.000000 pyTasker-0.6.4/Tasker/operations.py
--rw-rw-rw-   0        0        0    27430 2023-07-09 12:56:49.000000 pyTasker-0.6.4/Tasker/parser.py
--rw-rw-rw-   0        0        0     1315 2022-03-07 21:04:39.000000 pyTasker-0.6.4/Tasker/parser_test.py
--rw-rw-rw-   0        0        0    17710 2023-07-08 17:38:54.000000 pyTasker-0.6.4/Tasker/templater.py
--rw-rw-rw-   0        0        0     6979 2023-07-09 12:59:48.000000 pyTasker-0.6.4/Tasker/types.py
-drwxrwxrwx   0        0        0        0 2023-07-09 13:02:06.040667 pyTasker-0.6.4/pyTasker.egg-info/
--rw-rw-rw-   0        0        0     7532 2023-07-09 13:02:05.000000 pyTasker-0.6.4/pyTasker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      568 2023-07-09 13:02:05.000000 pyTasker-0.6.4/pyTasker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 13:02:05.000000 pyTasker-0.6.4/pyTasker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-07-09 13:02:05.000000 pyTasker-0.6.4/pyTasker.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       58 2023-07-09 13:02:05.000000 pyTasker-0.6.4/pyTasker.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-09 13:02:05.000000 pyTasker-0.6.4/pyTasker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      268 2022-03-07 21:04:39.000000 pyTasker-0.6.4/pyproject.toml
--rw-rw-rw-   0        0        0      113 2023-07-08 17:38:54.000000 pyTasker-0.6.4/requirements.txt
--rw-rw-rw-   0        0        0      191 2023-07-09 13:02:06.046663 pyTasker-0.6.4/setup.cfg
--rw-rw-rw-   0        0        0     1787 2023-07-09 13:01:19.000000 pyTasker-0.6.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-09 13:02:06.043666 pyTasker-0.6.4/static/
--rw-rw-rw-   0        0        0   424108 2022-02-03 21:25:58.000000 pyTasker-0.6.4/static/Copy PDFs then zip.png
--rw-rw-rw-   0        0        0   136520 2022-02-03 21:25:58.000000 pyTasker-0.6.4/static/Copy PDFs.png
+drwxrwxrwx   0        0        0        0 2023-07-09 13:10:38.144856 pyTasker-0.6.5/
+-rw-rw-rw-   0        0        0      305 2023-07-08 17:38:54.000000 pyTasker-0.6.5/.gitignore
+-rw-rw-rw-   0        0        0     1115 2022-03-07 21:04:39.000000 pyTasker-0.6.5/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0      733 2022-03-07 21:04:39.000000 pyTasker-0.6.5/CHANGELOG.md
+-rw-rw-rw-   0        0        0    35746 2022-02-03 21:25:58.000000 pyTasker-0.6.5/LICENSE
+-rw-rw-rw-   0        0        0     7532 2023-07-09 13:10:38.145856 pyTasker-0.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6460 2023-07-08 17:38:54.000000 pyTasker-0.6.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 13:10:38.117856 pyTasker-0.6.5/Tasker/
+-rw-rw-rw-   0        0        0      569 2023-07-08 17:38:54.000000 pyTasker-0.6.5/Tasker/__init__.py
+-rw-rw-rw-   0        0        0     3109 2023-07-08 17:38:54.000000 pyTasker-0.6.5/Tasker/__main__.py
+-rw-rw-rw-   0        0        0       23 2023-07-09 13:09:19.000000 pyTasker-0.6.5/Tasker/__version__.py
+-rw-rw-rw-   0        0        0     3554 2023-07-08 17:38:54.000000 pyTasker-0.6.5/Tasker/cli.py
+-rw-rw-rw-   0        0        0     2712 2023-07-08 17:38:54.000000 pyTasker-0.6.5/Tasker/common.py
+-rw-rw-rw-   0        0        0     2578 2022-03-07 21:04:39.000000 pyTasker-0.6.5/Tasker/inspector.py
+-rw-rw-rw-   0        0        0    15270 2023-07-08 17:38:54.000000 pyTasker-0.6.5/Tasker/operations.py
+-rw-rw-rw-   0        0        0    27271 2023-07-09 13:09:59.000000 pyTasker-0.6.5/Tasker/parser.py
+-rw-rw-rw-   0        0        0     1315 2022-03-07 21:04:39.000000 pyTasker-0.6.5/Tasker/parser_test.py
+-rw-rw-rw-   0        0        0    17710 2023-07-08 17:38:54.000000 pyTasker-0.6.5/Tasker/templater.py
+-rw-rw-rw-   0        0        0     6988 2023-07-09 13:08:50.000000 pyTasker-0.6.5/Tasker/types.py
+drwxrwxrwx   0        0        0        0 2023-07-09 13:10:38.140853 pyTasker-0.6.5/pyTasker.egg-info/
+-rw-rw-rw-   0        0        0     7532 2023-07-09 13:10:37.000000 pyTasker-0.6.5/pyTasker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      568 2023-07-09 13:10:37.000000 pyTasker-0.6.5/pyTasker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 13:10:37.000000 pyTasker-0.6.5/pyTasker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-09 13:10:37.000000 pyTasker-0.6.5/pyTasker.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       58 2023-07-09 13:10:37.000000 pyTasker-0.6.5/pyTasker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-09 13:10:37.000000 pyTasker-0.6.5/pyTasker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      268 2022-03-07 21:04:39.000000 pyTasker-0.6.5/pyproject.toml
+-rw-rw-rw-   0        0        0      113 2023-07-08 17:38:54.000000 pyTasker-0.6.5/requirements.txt
+-rw-rw-rw-   0        0        0      191 2023-07-09 13:10:38.146859 pyTasker-0.6.5/setup.cfg
+-rw-rw-rw-   0        0        0     1787 2023-07-09 13:09:13.000000 pyTasker-0.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 13:10:38.143854 pyTasker-0.6.5/static/
+-rw-rw-rw-   0        0        0   424108 2022-02-03 21:25:58.000000 pyTasker-0.6.5/static/Copy PDFs then zip.png
+-rw-rw-rw-   0        0        0   136520 2022-02-03 21:25:58.000000 pyTasker-0.6.5/static/Copy PDFs.png
```

### Comparing `pyTasker-0.6.4/.pre-commit-config.yaml` & `pyTasker-0.6.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.4/CHANGELOG.md` & `pyTasker-0.6.5/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.4/LICENSE` & `pyTasker-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.4/PKG-INFO` & `pyTasker-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTasker
-Version: 0.6.4
+Version: 0.6.5
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
-Metadata-Version: 2.1 Name: pyTasker Version: 0.6.4 Summary: Run pipelines on
+Metadata-Version: 2.1 Name: pyTasker Version: 0.6.5 Summary: Run pipelines on
 your own computer for better automation Home-page: https://github.com/
 carlossilva2/pyTasker Author: Carlos Silva Author-email:
 carlos.miguel.silva@protonmail.com License: GPLv3 Project-URL: Source, https://
 github.com/carlossilva2/pyTasker Project-URL: Documentation, https://
 cmsilva.gitbook.io/pytasker/ Platform: UNKNOWN Classifier: Development Status
 :: 4 - Beta Classifier: Environment :: Console Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: GNU General Public License v3
```

### Comparing `pyTasker-0.6.4/README.md` & `pyTasker-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.4/Tasker/__init__.py` & `pyTasker-0.6.5/Tasker/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.4/Tasker/__main__.py` & `pyTasker-0.6.5/Tasker/__main__.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.4/Tasker/cli.py` & `pyTasker-0.6.5/Tasker/cli.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.4/Tasker/common.py` & `pyTasker-0.6.5/Tasker/common.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.4/Tasker/inspector.py` & `pyTasker-0.6.5/Tasker/inspector.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.4/Tasker/operations.py` & `pyTasker-0.6.5/Tasker/operations.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.4/Tasker/parser.py` & `pyTasker-0.6.5/Tasker/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,25 +46,23 @@
         self.abort_exit = abort_exit
         self.execution = {}
         t = Timer()
         t.start()
         self.supported_os = ["Windows"]  # List of Tasker supported OSes
         self.logger = logger
         if task not in self.list_all_tasks():
-            self.abort(f"'{task}' InstructionSet was not found", abort=abort_exit)
+            self.abort(f"'{task}' InstructionSet was not found")
         self.warn_user()
         self.__first_execution_routine()
         self.task: InstructionSet = json.load(
             open(f"{self.default_location}/{task}.tasker.json", "r")
         )
         analysis = self.__analyse_keys()
         if not analysis[0]:
-            self.abort(
-                f'{analysis[3]} "{analysis[1]}" in {analysis[2]}', abort=abort_exit
-            )
+            self.abort(f'{analysis[3]} "{analysis[1]}" in {analysis[2]}')
         self.__optional_parameters()
         self.settings = self.__get_configs()
         # load extensions
         self.extensions: List[CustomOperation] = self.__load_extensions()
         self.__change_relative_locations(self.settings["current_location"])
         self.__executed_tasks: List[Task] = []
         self.__operation_stack: List[OperationType] = []
@@ -106,17 +104,17 @@
                 pass
             elif ans.lower() == "n":
                 sys.exit(0)
             else:
                 self.logger.error("Answer not allowed. Aborting...")
                 sys.exit(1)
 
-    def abort(self, reason: str, abort: bool = False) -> None:
+    def abort(self, reason: str) -> None:
         self.logger.error(reason)
-        if abort:
+        if self.abort_exit:
             sys.exit(1)
 
     def __execute(self, task: Task) -> bool:
         try:
             self.__check_destination_path(task, DESTINATION_CHECK_MAP[task["operation"]])
             if task["operation"] == "copy":
                 c = Copy(self, task, self.logger)
@@ -154,15 +152,14 @@
                 ex = next(
                     (e for e in self.extensions if e["summon"] == task["extension_name"]),
                     None,
                 )
                 if ex is None:
                     self.abort(
                         f"No executable found with name {chalk.red(task['extension_name'])}",
-                        self.abort_exit,
                     )
                 function: OperationType = ex["executable"].Extension(
                     self, task, self.logger
                 )
                 self.__operation_stack.append(function)
                 function.execute()
             else:
@@ -309,15 +306,14 @@
         for extension in self.settings["extensions"]:
             try:
                 spec: OperationType = importer(f"{extension['file'].replace('.py', '')}", extension["path"]).load_module()  # type: ignore
                 modules.append(CustomOperation(executable=spec, summon=extension["name"]))
             except Exception:
                 self.abort(
                     f"There was a problem importing {chalk.yellow(extension['name'])} Custom Extension. Please revise code implementation",
-                    self.abort_exit,
                 )
         return modules
 
     # Static Methods
 
     @staticmethod
     def do_config() -> None:
```

### Comparing `pyTasker-0.6.4/Tasker/parser_test.py` & `pyTasker-0.6.5/Tasker/parser_test.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.4/Tasker/templater.py` & `pyTasker-0.6.5/Tasker/templater.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.4/Tasker/types.py` & `pyTasker-0.6.5/Tasker/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,14 +192,15 @@
     extensions: List[Extension]
     alias: List[Alias]
 
 
 class ParserType:
 
     system: str
+    abort_exit: bool
     task: InstructionSet
     logger: Logger
     settings: Settings
     execution: Dict[str, Union[float, str]]
     supported_os: List[str]
     extensions: list
     default_location: str
@@ -208,15 +209,15 @@
 
     def execute(self) -> None:
         pass
 
     def warn_user(self) -> None:
         pass
 
-    def abort(self, reason: str, abort: bool) -> None:
+    def abort(self, reason: str) -> None:
         pass
 
     def __execute(self, task: Task) -> bool:
         return True
 
     def __check_destination_path(self, task: Task) -> None:
         pass
```

### Comparing `pyTasker-0.6.4/pyTasker.egg-info/PKG-INFO` & `pyTasker-0.6.5/pyTasker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTasker
-Version: 0.6.4
+Version: 0.6.5
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
-Metadata-Version: 2.1 Name: pyTasker Version: 0.6.4 Summary: Run pipelines on
+Metadata-Version: 2.1 Name: pyTasker Version: 0.6.5 Summary: Run pipelines on
 your own computer for better automation Home-page: https://github.com/
 carlossilva2/pyTasker Author: Carlos Silva Author-email:
 carlos.miguel.silva@protonmail.com License: GPLv3 Project-URL: Source, https://
 github.com/carlossilva2/pyTasker Project-URL: Documentation, https://
 cmsilva.gitbook.io/pytasker/ Platform: UNKNOWN Classifier: Development Status
 :: 4 - Beta Classifier: Environment :: Console Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: GNU General Public License v3
```

### Comparing `pyTasker-0.6.4/pyTasker.egg-info/SOURCES.txt` & `pyTasker-0.6.5/pyTasker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.4/setup.py` & `pyTasker-0.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 setup(
     author="Carlos Silva",
     author_email="carlos.miguel.silva@protonmail.com",
     name="pyTasker",
     description="Run pipelines on your own computer for better automation",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="0.6.4",
+    version="0.6.5",
     url="https://github.com/carlossilva2/pyTasker",
     packages=find_packages(),
     license="GPLv3",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Intended Audience :: Developers",
```

### Comparing `pyTasker-0.6.4/static/Copy PDFs then zip.png` & `pyTasker-0.6.5/static/Copy PDFs then zip.png`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.4/static/Copy PDFs.png` & `pyTasker-0.6.5/static/Copy PDFs.png`

 * *Files identical despite different names*

