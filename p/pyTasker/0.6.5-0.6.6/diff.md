# Comparing `tmp/pyTasker-0.6.5.tar.gz` & `tmp/pyTasker-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyTasker-0.6.5.tar", last modified: Sun Jul  9 13:10:38 2023, max compression
+gzip compressed data, was "pyTasker-0.6.6.tar", last modified: Sun Jul  9 13:15:14 2023, max compression
```

## Comparing `pyTasker-0.6.5.tar` & `pyTasker-0.6.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 13:10:38.144856 pyTasker-0.6.5/
--rw-rw-rw-   0        0        0      305 2023-07-08 17:38:54.000000 pyTasker-0.6.5/.gitignore
--rw-rw-rw-   0        0        0     1115 2022-03-07 21:04:39.000000 pyTasker-0.6.5/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0      733 2022-03-07 21:04:39.000000 pyTasker-0.6.5/CHANGELOG.md
--rw-rw-rw-   0        0        0    35746 2022-02-03 21:25:58.000000 pyTasker-0.6.5/LICENSE
--rw-rw-rw-   0        0        0     7532 2023-07-09 13:10:38.145856 pyTasker-0.6.5/PKG-INFO
--rw-rw-rw-   0        0        0     6460 2023-07-08 17:38:54.000000 pyTasker-0.6.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-09 13:10:38.117856 pyTasker-0.6.5/Tasker/
--rw-rw-rw-   0        0        0      569 2023-07-08 17:38:54.000000 pyTasker-0.6.5/Tasker/__init__.py
--rw-rw-rw-   0        0        0     3109 2023-07-08 17:38:54.000000 pyTasker-0.6.5/Tasker/__main__.py
--rw-rw-rw-   0        0        0       23 2023-07-09 13:09:19.000000 pyTasker-0.6.5/Tasker/__version__.py
--rw-rw-rw-   0        0        0     3554 2023-07-08 17:38:54.000000 pyTasker-0.6.5/Tasker/cli.py
--rw-rw-rw-   0        0        0     2712 2023-07-08 17:38:54.000000 pyTasker-0.6.5/Tasker/common.py
--rw-rw-rw-   0        0        0     2578 2022-03-07 21:04:39.000000 pyTasker-0.6.5/Tasker/inspector.py
--rw-rw-rw-   0        0        0    15270 2023-07-08 17:38:54.000000 pyTasker-0.6.5/Tasker/operations.py
--rw-rw-rw-   0        0        0    27271 2023-07-09 13:09:59.000000 pyTasker-0.6.5/Tasker/parser.py
--rw-rw-rw-   0        0        0     1315 2022-03-07 21:04:39.000000 pyTasker-0.6.5/Tasker/parser_test.py
--rw-rw-rw-   0        0        0    17710 2023-07-08 17:38:54.000000 pyTasker-0.6.5/Tasker/templater.py
--rw-rw-rw-   0        0        0     6988 2023-07-09 13:08:50.000000 pyTasker-0.6.5/Tasker/types.py
-drwxrwxrwx   0        0        0        0 2023-07-09 13:10:38.140853 pyTasker-0.6.5/pyTasker.egg-info/
--rw-rw-rw-   0        0        0     7532 2023-07-09 13:10:37.000000 pyTasker-0.6.5/pyTasker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      568 2023-07-09 13:10:37.000000 pyTasker-0.6.5/pyTasker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 13:10:37.000000 pyTasker-0.6.5/pyTasker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-07-09 13:10:37.000000 pyTasker-0.6.5/pyTasker.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       58 2023-07-09 13:10:37.000000 pyTasker-0.6.5/pyTasker.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-09 13:10:37.000000 pyTasker-0.6.5/pyTasker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      268 2022-03-07 21:04:39.000000 pyTasker-0.6.5/pyproject.toml
--rw-rw-rw-   0        0        0      113 2023-07-08 17:38:54.000000 pyTasker-0.6.5/requirements.txt
--rw-rw-rw-   0        0        0      191 2023-07-09 13:10:38.146859 pyTasker-0.6.5/setup.cfg
--rw-rw-rw-   0        0        0     1787 2023-07-09 13:09:13.000000 pyTasker-0.6.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-09 13:10:38.143854 pyTasker-0.6.5/static/
--rw-rw-rw-   0        0        0   424108 2022-02-03 21:25:58.000000 pyTasker-0.6.5/static/Copy PDFs then zip.png
--rw-rw-rw-   0        0        0   136520 2022-02-03 21:25:58.000000 pyTasker-0.6.5/static/Copy PDFs.png
+drwxrwxrwx   0        0        0        0 2023-07-09 13:15:14.739399 pyTasker-0.6.6/
+-rw-rw-rw-   0        0        0      305 2023-07-08 17:38:54.000000 pyTasker-0.6.6/.gitignore
+-rw-rw-rw-   0        0        0     1115 2022-03-07 21:04:39.000000 pyTasker-0.6.6/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0      733 2022-03-07 21:04:39.000000 pyTasker-0.6.6/CHANGELOG.md
+-rw-rw-rw-   0        0        0    35746 2022-02-03 21:25:58.000000 pyTasker-0.6.6/LICENSE
+-rw-rw-rw-   0        0        0     7532 2023-07-09 13:15:14.739399 pyTasker-0.6.6/PKG-INFO
+-rw-rw-rw-   0        0        0     6460 2023-07-08 17:38:54.000000 pyTasker-0.6.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 13:15:14.712398 pyTasker-0.6.6/Tasker/
+-rw-rw-rw-   0        0        0      569 2023-07-08 17:38:54.000000 pyTasker-0.6.6/Tasker/__init__.py
+-rw-rw-rw-   0        0        0     3109 2023-07-08 17:38:54.000000 pyTasker-0.6.6/Tasker/__main__.py
+-rw-rw-rw-   0        0        0       23 2023-07-09 13:14:09.000000 pyTasker-0.6.6/Tasker/__version__.py
+-rw-rw-rw-   0        0        0     3554 2023-07-08 17:38:54.000000 pyTasker-0.6.6/Tasker/cli.py
+-rw-rw-rw-   0        0        0     2712 2023-07-08 17:38:54.000000 pyTasker-0.6.6/Tasker/common.py
+-rw-rw-rw-   0        0        0     2578 2022-03-07 21:04:39.000000 pyTasker-0.6.6/Tasker/inspector.py
+-rw-rw-rw-   0        0        0    15270 2023-07-08 17:38:54.000000 pyTasker-0.6.6/Tasker/operations.py
+-rw-rw-rw-   0        0        0    27340 2023-07-09 13:13:58.000000 pyTasker-0.6.6/Tasker/parser.py
+-rw-rw-rw-   0        0        0     1315 2022-03-07 21:04:39.000000 pyTasker-0.6.6/Tasker/parser_test.py
+-rw-rw-rw-   0        0        0    17710 2023-07-08 17:38:54.000000 pyTasker-0.6.6/Tasker/templater.py
+-rw-rw-rw-   0        0        0     6988 2023-07-09 13:08:50.000000 pyTasker-0.6.6/Tasker/types.py
+drwxrwxrwx   0        0        0        0 2023-07-09 13:15:14.735399 pyTasker-0.6.6/pyTasker.egg-info/
+-rw-rw-rw-   0        0        0     7532 2023-07-09 13:15:14.000000 pyTasker-0.6.6/pyTasker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      568 2023-07-09 13:15:14.000000 pyTasker-0.6.6/pyTasker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 13:15:14.000000 pyTasker-0.6.6/pyTasker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-09 13:15:14.000000 pyTasker-0.6.6/pyTasker.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       58 2023-07-09 13:15:14.000000 pyTasker-0.6.6/pyTasker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-09 13:15:14.000000 pyTasker-0.6.6/pyTasker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      268 2022-03-07 21:04:39.000000 pyTasker-0.6.6/pyproject.toml
+-rw-rw-rw-   0        0        0      113 2023-07-08 17:38:54.000000 pyTasker-0.6.6/requirements.txt
+-rw-rw-rw-   0        0        0      191 2023-07-09 13:15:14.741398 pyTasker-0.6.6/setup.cfg
+-rw-rw-rw-   0        0        0     1787 2023-07-09 13:14:07.000000 pyTasker-0.6.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 13:15:14.738398 pyTasker-0.6.6/static/
+-rw-rw-rw-   0        0        0   424108 2022-02-03 21:25:58.000000 pyTasker-0.6.6/static/Copy PDFs then zip.png
+-rw-rw-rw-   0        0        0   136520 2022-02-03 21:25:58.000000 pyTasker-0.6.6/static/Copy PDFs.png
```

### Comparing `pyTasker-0.6.5/.pre-commit-config.yaml` & `pyTasker-0.6.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.5/CHANGELOG.md` & `pyTasker-0.6.6/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.5/LICENSE` & `pyTasker-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.5/PKG-INFO` & `pyTasker-0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTasker
-Version: 0.6.5
+Version: 0.6.6
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
-Metadata-Version: 2.1 Name: pyTasker Version: 0.6.5 Summary: Run pipelines on
+Metadata-Version: 2.1 Name: pyTasker Version: 0.6.6 Summary: Run pipelines on
 your own computer for better automation Home-page: https://github.com/
 carlossilva2/pyTasker Author: Carlos Silva Author-email:
 carlos.miguel.silva@protonmail.com License: GPLv3 Project-URL: Source, https://
 github.com/carlossilva2/pyTasker Project-URL: Documentation, https://
 cmsilva.gitbook.io/pytasker/ Platform: UNKNOWN Classifier: Development Status
 :: 4 - Beta Classifier: Environment :: Console Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: GNU General Public License v3
```

### Comparing `pyTasker-0.6.5/README.md` & `pyTasker-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.5/Tasker/__init__.py` & `pyTasker-0.6.6/Tasker/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.5/Tasker/__main__.py` & `pyTasker-0.6.6/Tasker/__main__.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.5/Tasker/cli.py` & `pyTasker-0.6.6/Tasker/cli.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.5/Tasker/common.py` & `pyTasker-0.6.6/Tasker/common.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.5/Tasker/inspector.py` & `pyTasker-0.6.6/Tasker/inspector.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.5/Tasker/operations.py` & `pyTasker-0.6.6/Tasker/operations.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.5/Tasker/parser.py` & `pyTasker-0.6.6/Tasker/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,16 @@
                 self.logger.error("Answer not allowed. Aborting...")
                 sys.exit(1)
 
     def abort(self, reason: str) -> None:
         self.logger.error(reason)
         if self.abort_exit:
             sys.exit(1)
+        else:
+            raise Exception("Aborting due to error")
 
     def __execute(self, task: Task) -> bool:
         try:
             self.__check_destination_path(task, DESTINATION_CHECK_MAP[task["operation"]])
             if task["operation"] == "copy":
                 c = Copy(self, task, self.logger)
                 self.__operation_stack.append(c)
```

### Comparing `pyTasker-0.6.5/Tasker/parser_test.py` & `pyTasker-0.6.6/Tasker/parser_test.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.5/Tasker/templater.py` & `pyTasker-0.6.6/Tasker/templater.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.5/Tasker/types.py` & `pyTasker-0.6.6/Tasker/types.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.5/pyTasker.egg-info/PKG-INFO` & `pyTasker-0.6.6/pyTasker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTasker
-Version: 0.6.5
+Version: 0.6.6
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
-Metadata-Version: 2.1 Name: pyTasker Version: 0.6.5 Summary: Run pipelines on
+Metadata-Version: 2.1 Name: pyTasker Version: 0.6.6 Summary: Run pipelines on
 your own computer for better automation Home-page: https://github.com/
 carlossilva2/pyTasker Author: Carlos Silva Author-email:
 carlos.miguel.silva@protonmail.com License: GPLv3 Project-URL: Source, https://
 github.com/carlossilva2/pyTasker Project-URL: Documentation, https://
 cmsilva.gitbook.io/pytasker/ Platform: UNKNOWN Classifier: Development Status
 :: 4 - Beta Classifier: Environment :: Console Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: GNU General Public License v3
```

### Comparing `pyTasker-0.6.5/pyTasker.egg-info/SOURCES.txt` & `pyTasker-0.6.6/pyTasker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.5/setup.py` & `pyTasker-0.6.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 setup(
     author="Carlos Silva",
     author_email="carlos.miguel.silva@protonmail.com",
     name="pyTasker",
     description="Run pipelines on your own computer for better automation",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="0.6.5",
+    version="0.6.6",
     url="https://github.com/carlossilva2/pyTasker",
     packages=find_packages(),
     license="GPLv3",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Intended Audience :: Developers",
```

### Comparing `pyTasker-0.6.5/static/Copy PDFs then zip.png` & `pyTasker-0.6.6/static/Copy PDFs then zip.png`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.5/static/Copy PDFs.png` & `pyTasker-0.6.6/static/Copy PDFs.png`

 * *Files identical despite different names*

