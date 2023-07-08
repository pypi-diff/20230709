# Comparing `tmp/buildlackey-0.8.1.tar.gz` & `tmp/buildlackey-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildlackey-0.8.1.tar", last modified: Thu Apr 20 03:11:23 2023, max compression
+gzip compressed data, was "buildlackey-1.0.0.tar", last modified: Sat Jul  8 23:46:33 2023, max compression
```

## Comparing `buildlackey-0.8.1.tar` & `buildlackey-1.0.0.tar`

### file list

```diff
@@ -1,26 +1,33 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-20 03:11:23.900416 buildlackey-0.8.1/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2023-04-07 13:32:43.000000 buildlackey-0.8.1/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    43932 2023-04-20 03:11:23.900277 buildlackey-0.8.1/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3752 2023-04-10 18:32:21.000000 buildlackey-0.8.1/README.md
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-20 03:11:23.898061 buildlackey-0.8.1/buildlackey/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8732 2023-04-20 03:07:29.000000 buildlackey-0.8.1/buildlackey/Commands.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1224 2023-04-13 00:43:49.000000 buildlackey-0.8.1/buildlackey/Environment.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      469 2023-04-08 19:28:49.000000 buildlackey-0.8.1/buildlackey/Version.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-31 14:31:31.000000 buildlackey-0.8.1/buildlackey/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-20 03:11:23.899521 buildlackey-0.8.1/buildlackey/exceptions/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       51 2023-02-25 02:47:03.000000 buildlackey-0.8.1/buildlackey/exceptions/ProjectNotSetException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       56 2023-02-25 02:28:42.000000 buildlackey-0.8.1/buildlackey/exceptions/ProjectsBaseNotSetException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-04 01:41:26.000000 buildlackey-0.8.1/buildlackey/exceptions/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-20 03:11:23.900038 buildlackey-0.8.1/buildlackey/resources/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-04 02:21:22.000000 buildlackey-0.8.1/buildlackey/resources/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      856 2023-04-13 00:43:13.000000 buildlackey-0.8.1/buildlackey/resources/loggingConfiguration.json
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        5 2023-04-20 03:07:43.000000 buildlackey-0.8.1/buildlackey/resources/version.txt
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-20 03:11:23.898843 buildlackey-0.8.1/buildlackey.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    43932 2023-04-20 03:11:23.000000 buildlackey-0.8.1/buildlackey.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      590 2023-04-20 03:11:23.000000 buildlackey-0.8.1/buildlackey.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-04-20 03:11:23.000000 buildlackey-0.8.1/buildlackey.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      215 2023-04-20 03:11:23.000000 buildlackey-0.8.1/buildlackey.egg-info/entry_points.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       13 2023-04-20 03:11:23.000000 buildlackey-0.8.1/buildlackey.egg-info/requires.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2023-04-20 03:11:23.000000 buildlackey-0.8.1/buildlackey.egg-info/top_level.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-04-20 03:11:23.900450 buildlackey-0.8.1/setup.cfg
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1331 2023-04-10 17:51:20.000000 buildlackey-0.8.1/setup.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-07-08 23:46:33.007748 buildlackey-1.0.0/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2023-04-07 13:32:43.000000 buildlackey-1.0.0/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    43935 2023-07-08 23:46:33.007618 buildlackey-1.0.0/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3755 2023-05-14 23:46:48.000000 buildlackey-1.0.0/README.md
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-07-08 23:46:33.005318 buildlackey-1.0.0/buildlackey/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4637 2023-07-08 20:51:40.000000 buildlackey-1.0.0/buildlackey/Commands.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1959 2023-07-07 20:47:53.000000 buildlackey-1.0.0/buildlackey/Environment.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      392 2023-07-06 20:28:44.000000 buildlackey-1.0.0/buildlackey/PythonWarnings.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       44 2023-07-05 19:22:15.000000 buildlackey-1.0.0/buildlackey/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       22 2023-07-07 19:47:36.000000 buildlackey-1.0.0/buildlackey/_version.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-07-08 23:46:33.006842 buildlackey-1.0.0/buildlackey/commands/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1257 2023-07-08 00:16:15.000000 buildlackey-1.0.0/buildlackey/commands/Cleanup.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1421 2023-07-08 00:23:30.000000 buildlackey-1.0.0/buildlackey/commands/Package.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      440 2023-07-08 00:47:04.000000 buildlackey-1.0.0/buildlackey/commands/ProductionPush.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      631 2023-07-07 20:48:29.000000 buildlackey-1.0.0/buildlackey/commands/RunMypy.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2128 2023-07-07 20:50:29.000000 buildlackey-1.0.0/buildlackey/commands/RunTests.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-07-06 19:54:27.000000 buildlackey-1.0.0/buildlackey/commands/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-07-08 23:46:33.007178 buildlackey-1.0.0/buildlackey/exceptions/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       51 2023-02-25 02:47:03.000000 buildlackey-1.0.0/buildlackey/exceptions/ProjectNotSetException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       56 2023-02-25 02:28:42.000000 buildlackey-1.0.0/buildlackey/exceptions/ProjectsBaseNotSetException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-04 01:41:26.000000 buildlackey-1.0.0/buildlackey/exceptions/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-07-08 23:46:33.007359 buildlackey-1.0.0/buildlackey/resources/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-04 02:21:22.000000 buildlackey-1.0.0/buildlackey/resources/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      856 2023-04-13 00:43:13.000000 buildlackey-1.0.0/buildlackey/resources/loggingConfiguration.json
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-07-08 23:46:33.006140 buildlackey-1.0.0/buildlackey.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    43935 2023-07-08 23:46:32.000000 buildlackey-1.0.0/buildlackey.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      788 2023-07-08 23:46:33.000000 buildlackey-1.0.0/buildlackey.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-07-08 23:46:33.000000 buildlackey-1.0.0/buildlackey.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      217 2023-07-08 23:46:33.000000 buildlackey-1.0.0/buildlackey.egg-info/entry_points.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       13 2023-07-08 23:46:33.000000 buildlackey-1.0.0/buildlackey.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2023-07-08 23:46:33.000000 buildlackey-1.0.0/buildlackey.egg-info/top_level.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-07-08 23:46:33.007786 buildlackey-1.0.0/setup.cfg
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1345 2023-07-08 19:41:35.000000 buildlackey-1.0.0/setup.py
```

### Comparing `buildlackey-0.8.1/LICENSE` & `buildlackey-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `buildlackey-0.8.1/PKG-INFO` & `buildlackey-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildlackey
-Version: 0.8.1
+Version: 1.0.0
 Summary: Project Maintenance Scripts
 Home-page: https://github.com/buildlackey
 Author: Humberto A. Sanchez II
 Author-email: humberto.a.sanchez.ii@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
@@ -717,29 +717,29 @@
 export PROJECT=pyutmodel
 source pyenv-3.10.6/bin/activate
 ```
 
 
 ## Python Console Scripts
 
-VersionOverlord means to handle this problem by providing a set of Python command line scripts to automate updating the first three of the above dependency specification locations
+buildlackey means to handle this problem by providing a set of Python command line scripts to automate updating the first three of the above dependency specification locations
 
 * runtests -- queries repositories for their latest release version
 * runmypy -- creates a dependency specification for a project 
 * cleanup -- updates the supported dependency locations using the generated specification
 * deploy -- 
-* Prod push --
+* prodpush --
 
 ## Usage
 
-runtests
-runmypy
-cleanup
-deploy
-pushtoprod
+* runtests
+* runmypy
+* cleanup
+* deploy
+* prodpush
 
 ___
 
 Written by <a href="mailto:email@humberto.a.sanchez.ii@gmail.com?subject=Hello Humberto">Humberto A. Sanchez II</a>  (C) 2023
 
 ---
```

### Comparing `buildlackey-0.8.1/README.md` & `buildlackey-1.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -43,29 +43,29 @@
 export PROJECT=pyutmodel
 source pyenv-3.10.6/bin/activate
 ```
 
 
 ## Python Console Scripts
 
-VersionOverlord means to handle this problem by providing a set of Python command line scripts to automate updating the first three of the above dependency specification locations
+buildlackey means to handle this problem by providing a set of Python command line scripts to automate updating the first three of the above dependency specification locations
 
 * runtests -- queries repositories for their latest release version
 * runmypy -- creates a dependency specification for a project 
 * cleanup -- updates the supported dependency locations using the generated specification
 * deploy -- 
-* Prod push --
+* prodpush --
 
 ## Usage
 
-runtests
-runmypy
-cleanup
-deploy
-pushtoprod
+* runtests
+* runmypy
+* cleanup
+* deploy
+* prodpush
 
 ___
 
 Written by <a href="mailto:email@humberto.a.sanchez.ii@gmail.com?subject=Hello Humberto">Humberto A. Sanchez II</a>  (C) 2023
 
 ---
```

#### html2text {}

```diff
@@ -22,22 +22,22 @@
 python projects are based PROJECT - The name of the project; It should be a
 directory name ``` An example, of a PROJECTS_BASE is: ```bash export
 PROJECTS_BASE="${HOME}/PycharmProjects" ``` This should be set in your shell
 startup script. For example `.bash_profile`. The PROJECT environment variable
 should be set on a project by project basis. I recommend you use [direnv]
 (https://direnv.net) to manage these. An example of a .envrc follows: ```bash
 export PROJECT=pyutmodel source pyenv-3.10.6/bin/activate ``` ## Python Console
-Scripts VersionOverlord means to handle this problem by providing a set of
-Python command line scripts to automate updating the first three of the above
+Scripts buildlackey means to handle this problem by providing a set of Python
+command line scripts to automate updating the first three of the above
 dependency specification locations * runtests -- queries repositories for their
 latest release version * runmypy -- creates a dependency specification for a
 project * cleanup -- updates the supported dependency locations using the
-generated specification * deploy -- * Prod push -- ## Usage runtests runmypy
-cleanup deploy pushtoprod ___ Written by Humberto_A._Sanchez_II (C) 2023 --- ##
-Note For all kind of problems, requests, enhancements, bug reports, etc.,
+generated specification * deploy -- * prodpush -- ## Usage * runtests * runmypy
+* cleanup * deploy * prodpush ___ Written by Humberto_A._Sanchez_II (C) 2023 --
+- ## Note For all kind of problems, requests, enhancements, bug reports, etc.,
 please drop me an e-mail. ![Humberto's Modified Logo](https://
 raw.githubusercontent.com/wiki/hasii2011/gittodoistclone/images/
 SillyGitHub.png) I am concerned about GitHub's Copilot project I urge you to
 read about the [Give up GitHub](https://GiveUpGitHub.org) campaign from [the
 Software Freedom Conservancy](https://sfconservancy.org). While I do not
 advocate for all the issues listed there I do not like that a company like
 Microsoft may profit from open source projects. I continue to use GitHub
```

### Comparing `buildlackey-0.8.1/buildlackey/Environment.py` & `buildlackey-1.0.0/buildlackey/Environment.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,51 @@
 
 from logging import Logger
 from logging import getLogger
+from subprocess import CompletedProcess
+
+from os import chdir
 
 from os import environ as osEnvironment
+from os import sep as osSep
+
+from subprocess import run as subProcessRun
+
+from click import ClickException
+from click import clear
+from click import secho
 
 
-class EnvironmentBase:
+class Environment:
     """
 
     """
     ENV_PROJECTS_BASE: str = 'PROJECTS_BASE'
     ENV_PROJECT:       str = 'PROJECT'
 
     def __init__(self):
 
         self.ebLogger: Logger = getLogger(__name__)
 
         self._projectsBase:     str = ''
         self._projectDirectory: str = ''
 
         try:
-            self._projectsBase = osEnvironment[EnvironmentBase.ENV_PROJECTS_BASE]
+            self._projectsBase = osEnvironment[Environment.ENV_PROJECTS_BASE]
         except KeyError:
-            self.ebLogger.info(f'Project Base not set')
+            raise ClickException('Project Base not set')
         try:
-            self._projectDirectory = osEnvironment[EnvironmentBase.ENV_PROJECT]
+            self._projectDirectory = osEnvironment[Environment.ENV_PROJECT]
         except KeyError:
-            self.ebLogger.info(f'Project Directory not set')
+            raise ClickException(f'Project Directory not set')
+
+        clear()
+        secho(f'projects_base={self._projectsBase}', color=True, reverse=True)
+        secho(f'project={self._projectDirectory}', color=True, reverse=True)
+        secho('')
 
     @property
     def projectsBase(self) -> str:
         return self._projectsBase
 
     @property
     def projectDirectory(self) -> str:
@@ -44,7 +59,18 @@
             return True
 
     def validProjectDirectory(self) -> bool:
         if self._projectDirectory == '':
             return False
         else:
             return True
+
+    def _runCommand(self,  command: str) -> int:
+
+        cp: CompletedProcess = subProcessRun([command], shell=True, capture_output=False, text=True, check=False)
+
+        return cp.returncode
+
+    def _changeToProjectRoot(self):
+
+        fullPath: str = f'{self._projectsBase}{osSep}{self._projectDirectory}'
+        chdir(fullPath)
```

### Comparing `buildlackey-0.8.1/buildlackey/resources/loggingConfiguration.json` & `buildlackey-1.0.0/buildlackey/resources/loggingConfiguration.json`

 * *Files identical despite different names*

### Comparing `buildlackey-0.8.1/buildlackey.egg-info/PKG-INFO` & `buildlackey-1.0.0/buildlackey.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildlackey
-Version: 0.8.1
+Version: 1.0.0
 Summary: Project Maintenance Scripts
 Home-page: https://github.com/buildlackey
 Author: Humberto A. Sanchez II
 Author-email: humberto.a.sanchez.ii@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
@@ -717,29 +717,29 @@
 export PROJECT=pyutmodel
 source pyenv-3.10.6/bin/activate
 ```
 
 
 ## Python Console Scripts
 
-VersionOverlord means to handle this problem by providing a set of Python command line scripts to automate updating the first three of the above dependency specification locations
+buildlackey means to handle this problem by providing a set of Python command line scripts to automate updating the first three of the above dependency specification locations
 
 * runtests -- queries repositories for their latest release version
 * runmypy -- creates a dependency specification for a project 
 * cleanup -- updates the supported dependency locations using the generated specification
 * deploy -- 
-* Prod push --
+* prodpush --
 
 ## Usage
 
-runtests
-runmypy
-cleanup
-deploy
-pushtoprod
+* runtests
+* runmypy
+* cleanup
+* deploy
+* prodpush
 
 ___
 
 Written by <a href="mailto:email@humberto.a.sanchez.ii@gmail.com?subject=Hello Humberto">Humberto A. Sanchez II</a>  (C) 2023
 
 ---
```

### Comparing `buildlackey-0.8.1/buildlackey.egg-info/SOURCES.txt` & `buildlackey-1.0.0/buildlackey.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 LICENSE
 README.md
 setup.py
 buildlackey/Commands.py
 buildlackey/Environment.py
-buildlackey/Version.py
+buildlackey/PythonWarnings.py
 buildlackey/__init__.py
+buildlackey/_version.py
 buildlackey.egg-info/PKG-INFO
 buildlackey.egg-info/SOURCES.txt
 buildlackey.egg-info/dependency_links.txt
 buildlackey.egg-info/entry_points.txt
 buildlackey.egg-info/requires.txt
 buildlackey.egg-info/top_level.txt
+buildlackey/commands/Cleanup.py
+buildlackey/commands/Package.py
+buildlackey/commands/ProductionPush.py
+buildlackey/commands/RunMypy.py
+buildlackey/commands/RunTests.py
+buildlackey/commands/__init__.py
 buildlackey/exceptions/ProjectNotSetException.py
 buildlackey/exceptions/ProjectsBaseNotSetException.py
 buildlackey/exceptions/__init__.py
 buildlackey/resources/__init__.py
-buildlackey/resources/loggingConfiguration.json
-buildlackey/resources/version.txt
+buildlackey/resources/loggingConfiguration.json
```

### Comparing `buildlackey-0.8.1/setup.py` & `buildlackey-1.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import pathlib
 from setuptools import setup
 
+from buildlackey import __version__ as version
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README  = (HERE / "README.md").read_text()
 LICENSE = (HERE / 'LICENSE').read_text()
-VERSION = (HERE / 'buildlackey/resources/version.txt').read_text()
 
 setup(
     name="buildlackey",
-    version=VERSION,
+    version=version,
     author='Humberto A. Sanchez II',
     author_email='humberto.a.sanchez.ii@gmail.com',
     maintainer='Humberto A. Sanchez II',
     maintainer_email='humberto.a.sanchez.ii@gmail.com',
     description='Project Maintenance Scripts',
     long_description=README,
     long_description_content_type="text/markdown",
     license=LICENSE,
     url="https://github.com/buildlackey",
     packages=[
         'buildlackey',
+        'buildlackey.commands',
         'buildlackey.exceptions',
         'buildlackey.resources',
     ],
     package_data={
         'buildlackey.resources': ['loggingConfiguration.json', 'version.txt'],
     },
 
@@ -34,12 +35,12 @@
         'click~=8.1.3',
     ],
     entry_points={
         "console_scripts": [
             "runtests=buildlackey.Commands:runtests",
             "cleanup=buildlackey.Commands:cleanup",
             "runmypy=buildlackey.Commands:runmypy",
-            "deploy=buildlackey.Commands:deploy",
+            "package=buildlackey.Commands:package",
             "prodpush=buildlackey.Commands:prodpush",
         ]
     },
 )
```

