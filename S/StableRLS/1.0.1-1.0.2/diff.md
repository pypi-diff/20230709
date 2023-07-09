# Comparing `tmp/StableRLS-1.0.1.tar.gz` & `tmp/StableRLS-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StableRLS-1.0.1.tar", last modified: Sun Jul  9 15:24:52 2023, max compression
+gzip compressed data, was "StableRLS-1.0.2.tar", last modified: Sun Jul  9 16:31:59 2023, max compression
```

## Comparing `StableRLS-1.0.1.tar` & `StableRLS-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 cao2851   (1000) cao2851   (1000)        0 2023-07-09 15:24:52.034358 StableRLS-1.0.1/
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)    35148 2023-03-21 15:46:09.000000 StableRLS-1.0.1/LICENSE.txt
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)     4686 2023-07-09 15:24:52.034358 StableRLS-1.0.1/PKG-INFO
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)     4314 2023-07-09 15:09:21.000000 StableRLS-1.0.1/README.md
-drwxrwxr-x   0 cao2851   (1000) cao2851   (1000)        0 2023-07-09 15:24:52.034358 StableRLS-1.0.1/StableRLS.egg-info/
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)     4686 2023-07-09 15:24:52.000000 StableRLS-1.0.1/StableRLS.egg-info/PKG-INFO
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)      307 2023-07-09 15:24:52.000000 StableRLS-1.0.1/StableRLS.egg-info/SOURCES.txt
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)        1 2023-07-09 15:24:52.000000 StableRLS-1.0.1/StableRLS.egg-info/dependency_links.txt
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)       37 2023-07-09 15:24:52.000000 StableRLS-1.0.1/StableRLS.egg-info/requires.txt
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)       10 2023-07-09 15:24:52.000000 StableRLS-1.0.1/StableRLS.egg-info/top_level.txt
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)       38 2023-07-09 15:24:52.034358 StableRLS-1.0.1/setup.cfg
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)      744 2023-07-09 15:24:11.000000 StableRLS-1.0.1/setup.py
-drwxrwxr-x   0 cao2851   (1000) cao2851   (1000)        0 2023-07-09 15:24:52.034358 StableRLS-1.0.1/stablerls/
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)        0 2023-03-21 15:46:09.000000 StableRLS-1.0.1/stablerls/__init__.py
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)     2918 2023-07-09 15:00:17.000000 StableRLS-1.0.1/stablerls/configreader.py
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)     2868 2023-07-09 15:00:25.000000 StableRLS-1.0.1/stablerls/createFMU.py
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)     4188 2023-07-01 15:03:04.000000 StableRLS-1.0.1/stablerls/fmutools.py
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)    17470 2023-07-01 15:03:05.000000 StableRLS-1.0.1/stablerls/gymFMU.py
+drwxrwxr-x   0 cao2851   (1000) cao2851   (1000)        0 2023-07-09 16:31:59.817880 StableRLS-1.0.2/
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)    35148 2023-03-21 15:46:09.000000 StableRLS-1.0.2/LICENSE.txt
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)     4686 2023-07-09 16:31:59.817880 StableRLS-1.0.2/PKG-INFO
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)     4314 2023-07-09 15:09:21.000000 StableRLS-1.0.2/README.md
+drwxrwxr-x   0 cao2851   (1000) cao2851   (1000)        0 2023-07-09 16:31:59.817880 StableRLS-1.0.2/StableRLS.egg-info/
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)     4686 2023-07-09 16:31:59.000000 StableRLS-1.0.2/StableRLS.egg-info/PKG-INFO
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)      328 2023-07-09 16:31:59.000000 StableRLS-1.0.2/StableRLS.egg-info/SOURCES.txt
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)        1 2023-07-09 16:31:59.000000 StableRLS-1.0.2/StableRLS.egg-info/dependency_links.txt
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)       37 2023-07-09 16:31:59.000000 StableRLS-1.0.2/StableRLS.egg-info/requires.txt
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)       10 2023-07-09 16:31:59.000000 StableRLS-1.0.2/StableRLS.egg-info/top_level.txt
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)       38 2023-07-09 16:31:59.817880 StableRLS-1.0.2/setup.cfg
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)      780 2023-07-09 16:31:51.000000 StableRLS-1.0.2/setup.py
+drwxrwxr-x   0 cao2851   (1000) cao2851   (1000)        0 2023-07-09 16:31:59.817880 StableRLS-1.0.2/stablerls/
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)        0 2023-03-21 15:46:09.000000 StableRLS-1.0.2/stablerls/__init__.py
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)     2918 2023-07-09 15:00:17.000000 StableRLS-1.0.2/stablerls/configreader.py
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)     2868 2023-07-09 15:00:25.000000 StableRLS-1.0.2/stablerls/createFMU.py
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)     4188 2023-07-01 15:03:04.000000 StableRLS-1.0.2/stablerls/fmutools.py
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)    15697 2023-05-08 13:15:04.000000 StableRLS-1.0.2/stablerls/getports.m
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)    17470 2023-07-01 15:03:05.000000 StableRLS-1.0.2/stablerls/gymFMU.py
```

### Comparing `StableRLS-1.0.1/LICENSE.txt` & `StableRLS-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `StableRLS-1.0.1/PKG-INFO` & `StableRLS-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StableRLS
-Version: 1.0.1
+Version: 1.0.2
 Summary: Simulate Simulink FMUs as Gymnasium environment
 Home-page: https://github.com/rAnnuth/stablerls
 Author: Robert Annuth
 Author-email: robert.annuth@tuhh.de
 License: LICENSE.txt
 Keywords: simulation RL reinforcement learning Simulink matlab FMU
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: StableRLS Version: 1.0.1 Summary: Simulate Simulink
+Metadata-Version: 2.1 Name: StableRLS Version: 1.0.2 Summary: Simulate Simulink
 FMUs as Gymnasium environment Home-page: https://github.com/rAnnuth/stablerls
 Author: Robert Annuth Author-email: robert.annuth@tuhh.de License: LICENSE.txt
 Keywords: simulation RL reinforcement learning Simulink matlab FMU Description-
 Content-Type: text/markdown License-File: LICENSE.txt ![](src/icon.png)
             ***** Stable Reinforcement Learning for Simulink *****
                   [Documentation_Status] [Code_style:_black]
 StableRLS is a software package to use your existing MATLAB Simulink models in
```

### Comparing `StableRLS-1.0.1/README.md` & `StableRLS-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `StableRLS-1.0.1/StableRLS.egg-info/PKG-INFO` & `StableRLS-1.0.2/StableRLS.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StableRLS
-Version: 1.0.1
+Version: 1.0.2
 Summary: Simulate Simulink FMUs as Gymnasium environment
 Home-page: https://github.com/rAnnuth/stablerls
 Author: Robert Annuth
 Author-email: robert.annuth@tuhh.de
 License: LICENSE.txt
 Keywords: simulation RL reinforcement learning Simulink matlab FMU
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: StableRLS Version: 1.0.1 Summary: Simulate Simulink
+Metadata-Version: 2.1 Name: StableRLS Version: 1.0.2 Summary: Simulate Simulink
 FMUs as Gymnasium environment Home-page: https://github.com/rAnnuth/stablerls
 Author: Robert Annuth Author-email: robert.annuth@tuhh.de License: LICENSE.txt
 Keywords: simulation RL reinforcement learning Simulink matlab FMU Description-
 Content-Type: text/markdown License-File: LICENSE.txt ![](src/icon.png)
             ***** Stable Reinforcement Learning for Simulink *****
                   [Documentation_Status] [Code_style:_black]
 StableRLS is a software package to use your existing MATLAB Simulink models in
```

### Comparing `StableRLS-1.0.1/setup.py` & `StableRLS-1.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
   name='StableRLS',
-  version='1.0.1',
+  version='1.0.2',
   author='Robert Annuth',
   author_email='robert.annuth@tuhh.de',
   packages= setuptools.find_packages(),
+  package_data={'stablerls':['*']},
   license='LICENSE.txt',
   description='Simulate Simulink FMUs as Gymnasium environment',
   long_description=long_description,
   long_description_content_type='text/markdown',
   url='https://github.com/rAnnuth/stablerls',
   keywords='simulation RL reinforcement learning Simulink matlab FMU',
   install_requires=[
```

### Comparing `StableRLS-1.0.1/stablerls/configreader.py` & `StableRLS-1.0.2/stablerls/configreader.py`

 * *Files identical despite different names*

### Comparing `StableRLS-1.0.1/stablerls/createFMU.py` & `StableRLS-1.0.2/stablerls/createFMU.py`

 * *Files identical despite different names*

### Comparing `StableRLS-1.0.1/stablerls/fmutools.py` & `StableRLS-1.0.2/stablerls/fmutools.py`

 * *Files identical despite different names*

### Comparing `StableRLS-1.0.1/stablerls/gymFMU.py` & `StableRLS-1.0.2/stablerls/gymFMU.py`

 * *Files identical despite different names*

