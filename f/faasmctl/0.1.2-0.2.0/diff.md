# Comparing `tmp/faasmctl-0.1.2.tar.gz` & `tmp/faasmctl-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faasmctl-0.1.2.tar", last modified: Thu Jul  6 17:00:35 2023, max compression
+gzip compressed data, was "faasmctl-0.2.0.tar", last modified: Sun Jul  9 17:59:40 2023, max compression
```

## Comparing `faasmctl-0.1.2.tar` & `faasmctl-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:00:35.455517 faasmctl-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-06 17:00:26.000000 faasmctl-0.1.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-06 17:00:35.455517 faasmctl-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-06 17:00:26.000000 faasmctl-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:00:35.451517 faasmctl-0.1.2/faasmctl/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-06 17:00:26.000000 faasmctl-0.1.2/faasmctl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-06 17:00:26.000000 faasmctl-0.1.2/faasmctl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:00:35.455517 faasmctl-0.1.2/faasmctl/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-06 17:00:26.000000 faasmctl-0.1.2/faasmctl/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-06 17:00:26.000000 faasmctl-0.1.2/faasmctl/tasks/flush.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:00:35.455517 faasmctl-0.1.2/faasmctl/util/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-06 17:00:26.000000 faasmctl-0.1.2/faasmctl/util/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-06 17:00:26.000000 faasmctl-0.1.2/faasmctl/util/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:00:35.455517 faasmctl-0.1.2/faasmctl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-06 17:00:35.000000 faasmctl-0.1.2/faasmctl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-06 17:00:35.000000 faasmctl-0.1.2/faasmctl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 17:00:35.000000 faasmctl-0.1.2/faasmctl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-06 17:00:35.000000 faasmctl-0.1.2/faasmctl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 17:00:35.000000 faasmctl-0.1.2/faasmctl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 17:00:35.000000 faasmctl-0.1.2/faasmctl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-06 17:00:26.000000 faasmctl-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 17:00:35.455517 faasmctl-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:59:40.503262 faasmctl-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-09 17:59:31.000000 faasmctl-0.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-09 17:59:40.503262 faasmctl-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-09 17:59:31.000000 faasmctl-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:59:40.499262 faasmctl-0.2.0/faasmctl/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-09 17:59:31.000000 faasmctl-0.2.0/faasmctl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-09 17:59:31.000000 faasmctl-0.2.0/faasmctl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:59:40.499262 faasmctl-0.2.0/faasmctl/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-09 17:59:31.000000 faasmctl-0.2.0/faasmctl/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-09 17:59:31.000000 faasmctl-0.2.0/faasmctl/tasks/flush.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-09 17:59:31.000000 faasmctl-0.2.0/faasmctl/tasks/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-09 17:59:31.000000 faasmctl-0.2.0/faasmctl/tasks/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:59:40.503262 faasmctl-0.2.0/faasmctl/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-09 17:59:31.000000 faasmctl-0.2.0/faasmctl/util/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-09 17:59:31.000000 faasmctl-0.2.0/faasmctl/util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-09 17:59:31.000000 faasmctl-0.2.0/faasmctl/util/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-09 17:59:31.000000 faasmctl-0.2.0/faasmctl/util/faasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-09 17:59:31.000000 faasmctl-0.2.0/faasmctl/util/flush.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-07-09 17:59:31.000000 faasmctl-0.2.0/faasmctl/util/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-09 17:59:31.000000 faasmctl-0.2.0/faasmctl/util/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-09 17:59:31.000000 faasmctl-0.2.0/faasmctl/util/planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-09 17:59:31.000000 faasmctl-0.2.0/faasmctl/util/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-09 17:59:31.000000 faasmctl-0.2.0/faasmctl/util/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-09 17:59:31.000000 faasmctl-0.2.0/faasmctl/util/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:59:40.499262 faasmctl-0.2.0/faasmctl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-09 17:59:40.000000 faasmctl-0.2.0/faasmctl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-09 17:59:40.000000 faasmctl-0.2.0/faasmctl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 17:59:40.000000 faasmctl-0.2.0/faasmctl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-09 17:59:40.000000 faasmctl-0.2.0/faasmctl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-09 17:59:40.000000 faasmctl-0.2.0/faasmctl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-09 17:59:40.000000 faasmctl-0.2.0/faasmctl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-09 17:59:31.000000 faasmctl-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 17:59:40.503262 faasmctl-0.2.0/setup.cfg
```

### Comparing `faasmctl-0.1.2/LICENSE.md` & `faasmctl-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `faasmctl-0.1.2/PKG-INFO` & `faasmctl-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faasmctl
-Version: 0.1.2
+Version: 0.2.0
 Summary: Command line tool to deploy, manage, and interact with Faasm
 Author-email: Faasm Team <foo@bar.com>
 Project-URL: Homepage, https://github.com/faasm/faasmctl
 Project-URL: Bug Tracker, https://github.com/faasm/faasmctl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -17,15 +17,15 @@
 running [Faasm](https://github.com/faasm/faasm) cluster.
 
 ## Install
 
 To install `faasmctl` you need a working `pip` (virtual-)environment. Then:
 
 ```bash
-pip install faasmctl==0.1.2
+pip install faasmctl==0.2.0
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.1.2/README.md` & `faasmctl-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 running [Faasm](https://github.com/faasm/faasm) cluster.
 
 ## Install
 
 To install `faasmctl` you need a working `pip` (virtual-)environment. Then:
 
 ```bash
-pip install faasmctl==0.1.2
+pip install faasmctl==0.2.0
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.1.2/faasmctl.egg-info/PKG-INFO` & `faasmctl-0.2.0/faasmctl.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faasmctl
-Version: 0.1.2
+Version: 0.2.0
 Summary: Command line tool to deploy, manage, and interact with Faasm
 Author-email: Faasm Team <foo@bar.com>
 Project-URL: Homepage, https://github.com/faasm/faasmctl
 Project-URL: Bug Tracker, https://github.com/faasm/faasmctl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -17,15 +17,15 @@
 running [Faasm](https://github.com/faasm/faasm) cluster.
 
 ## Install
 
 To install `faasmctl` you need a working `pip` (virtual-)environment. Then:
 
 ```bash
-pip install faasmctl==0.1.2
+pip install faasmctl==0.2.0
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.1.2/pyproject.toml` & `faasmctl-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "faasmctl"
-version = "0.1.2"
+version = "0.2.0"
 authors = [
   { name="Faasm Team", email="foo@bar.com" },
 ]
 description = "Command line tool to deploy, manage, and interact with Faasm"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "invoke == 2.1.3",
+    "requests == 2.31.0",
+    "protobuf == 4.23.4",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/faasm/faasmctl"
 "Bug Tracker" = "https://github.com/faasm/faasmctl/issues"
 
 [project.scripts]
```

