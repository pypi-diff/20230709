# Comparing `tmp/seedwork_python-0.1.0.tar.gz` & `tmp/seedwork_python-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seedwork_python-0.1.0.tar", max compression
+gzip compressed data, was "seedwork_python-0.1.1.tar", max compression
```

## Comparing `seedwork_python-0.1.0.tar` & `seedwork_python-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0     1066 2023-07-08 14:25:12.259881 seedwork_python-0.1.0/LICENSE
--rw-r--r--   0        0        0      258 2023-07-08 14:25:12.270606 seedwork_python-0.1.0/README.md
--rw-r--r--   0        0        0     1578 2023-07-09 00:08:24.205968 seedwork_python-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-04 14:12:17.070490 seedwork_python-0.1.0/seedwork/__init__.py
--rw-r--r--   0        0        0       52 2023-07-07 11:49:36.263799 seedwork_python-0.1.0/seedwork/application/__init__.py
--rw-r--r--   0        0        0      115 2023-07-08 05:10:39.020400 seedwork_python-0.1.0/seedwork/application/command.py
--rw-r--r--   0        0        0      195 2023-07-04 00:24:30.486852 seedwork_python-0.1.0/seedwork/domain/__init__.py
--rw-r--r--   0        0        0      237 2023-07-08 12:38:37.709567 seedwork_python-0.1.0/seedwork/domain/aggregate_root.py
--rw-r--r--   0        0        0     1112 2023-07-08 12:40:08.210080 seedwork_python-0.1.0/seedwork/domain/entity.py
--rw-r--r--   0        0        0      496 2023-07-03 11:32:45.559964 seedwork_python-0.1.0/seedwork/domain/enumeration.py
--rw-r--r--   0        0        0      102 2023-07-03 11:32:45.560059 seedwork_python-0.1.0/seedwork/domain/event.py
--rw-r--r--   0        0        0        0 2023-07-08 11:20:04.255707 seedwork_python-0.1.0/seedwork/domain/repository/__init__.py
--rw-r--r--   0        0        0     1175 2023-07-08 12:26:02.006849 seedwork_python-0.1.0/seedwork/domain/repository/generic.py
--rw-r--r--   0        0        0      202 2023-07-08 11:13:57.483175 seedwork_python-0.1.0/seedwork/domain/repository/repository.py
--rw-r--r--   0        0        0      702 2023-07-05 11:09:01.743339 seedwork_python-0.1.0/seedwork/domain/unit_of_work.py
--rw-r--r--   0        0        0      114 2023-07-03 11:32:45.560142 seedwork_python-0.1.0/seedwork/domain/value_object.py
--rw-r--r--   0        0        0        0 2023-07-06 11:16:26.140518 seedwork_python-0.1.0/seedwork/infrastructure/__init__.py
--rw-r--r--   0        0        0       49 2023-07-07 12:26:02.202328 seedwork_python-0.1.0/seedwork/infrastructure/logging/__init__.py
--rw-r--r--   0        0        0      149 2023-07-07 12:46:45.930202 seedwork_python-0.1.0/seedwork/infrastructure/logging/logger.py
--rw-r--r--   0        0        0        0 2023-07-06 11:16:26.140575 seedwork_python-0.1.0/seedwork/infrastructure/persistence/__init__.py
--rw-r--r--   0        0        0      152 2023-07-06 11:16:26.140685 seedwork_python-0.1.0/seedwork/infrastructure/persistence/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      191 2023-07-06 11:16:26.140773 seedwork_python-0.1.0/seedwork/infrastructure/persistence/sqlalchemy/repository.py
--rw-r--r--   0        0        0      933 2023-07-06 11:16:26.140861 seedwork_python-0.1.0/seedwork/infrastructure/persistence/sqlalchemy/unit_of_work.py
--rw-r--r--   0        0        0      318 2023-07-08 12:13:02.552819 seedwork_python-0.1.0/seedwork/typings.py
--rw-r--r--   0        0        0     1118 1970-01-01 00:00:00.000000 seedwork_python-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-08 14:25:12.259881 seedwork_python-0.1.1/LICENSE
+-rw-r--r--   0        0        0      373 2021-07-16 00:27:15.175286 seedwork_python-0.1.1/README.md
+-rw-r--r--   0        0        0     1616 2023-07-09 00:51:20.263109 seedwork_python-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-04 14:12:17.070490 seedwork_python-0.1.1/seedwork/__init__.py
+-rw-r--r--   0        0        0       52 2023-07-07 11:49:36.263799 seedwork_python-0.1.1/seedwork/application/__init__.py
+-rw-r--r--   0        0        0      115 2023-07-08 05:10:39.020400 seedwork_python-0.1.1/seedwork/application/command.py
+-rw-r--r--   0        0        0      195 2023-07-04 00:24:30.486852 seedwork_python-0.1.1/seedwork/domain/__init__.py
+-rw-r--r--   0        0        0      237 2023-07-08 12:38:37.709567 seedwork_python-0.1.1/seedwork/domain/aggregate_root.py
+-rw-r--r--   0        0        0     1112 2023-07-08 12:40:08.210080 seedwork_python-0.1.1/seedwork/domain/entity.py
+-rw-r--r--   0        0        0      496 2023-07-03 11:32:45.559964 seedwork_python-0.1.1/seedwork/domain/enumeration.py
+-rw-r--r--   0        0        0      102 2023-07-03 11:32:45.560059 seedwork_python-0.1.1/seedwork/domain/event.py
+-rw-r--r--   0        0        0        0 2023-07-08 11:20:04.255707 seedwork_python-0.1.1/seedwork/domain/repository/__init__.py
+-rw-r--r--   0        0        0     1175 2023-07-08 12:26:02.006849 seedwork_python-0.1.1/seedwork/domain/repository/generic.py
+-rw-r--r--   0        0        0      202 2023-07-08 11:13:57.483175 seedwork_python-0.1.1/seedwork/domain/repository/repository.py
+-rw-r--r--   0        0        0      702 2023-07-05 11:09:01.743339 seedwork_python-0.1.1/seedwork/domain/unit_of_work.py
+-rw-r--r--   0        0        0      114 2023-07-03 11:32:45.560142 seedwork_python-0.1.1/seedwork/domain/value_object.py
+-rw-r--r--   0        0        0        0 2023-07-06 11:16:26.140518 seedwork_python-0.1.1/seedwork/infrastructure/__init__.py
+-rw-r--r--   0        0        0       49 2023-07-07 12:26:02.202328 seedwork_python-0.1.1/seedwork/infrastructure/logging/__init__.py
+-rw-r--r--   0        0        0      149 2023-07-07 12:46:45.930202 seedwork_python-0.1.1/seedwork/infrastructure/logging/logger.py
+-rw-r--r--   0        0        0        0 2023-07-06 11:16:26.140575 seedwork_python-0.1.1/seedwork/infrastructure/persistence/__init__.py
+-rw-r--r--   0        0        0      152 2023-07-06 11:16:26.140685 seedwork_python-0.1.1/seedwork/infrastructure/persistence/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      191 2023-07-06 11:16:26.140773 seedwork_python-0.1.1/seedwork/infrastructure/persistence/sqlalchemy/repository.py
+-rw-r--r--   0        0        0      933 2023-07-06 11:16:26.140861 seedwork_python-0.1.1/seedwork/infrastructure/persistence/sqlalchemy/unit_of_work.py
+-rw-r--r--   0        0        0        0 2023-07-09 00:50:53.962442 seedwork_python-0.1.1/seedwork/py.typed
+-rw-r--r--   0        0        0      318 2023-07-08 12:13:02.552819 seedwork_python-0.1.1/seedwork/typings.py
+-rw-r--r--   0        0        0     1233 1970-01-01 00:00:00.000000 seedwork_python-0.1.1/PKG-INFO
```

### Comparing `seedwork_python-0.1.0/LICENSE` & `seedwork_python-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `seedwork_python-0.1.0/pyproject.toml` & `seedwork_python-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seedwork-python"
-version = "0.1.0"
+version = "0.1.1"
 description = "Python seedwork library."
 license = "MIT"
 authors = ["Huang Kai <h1770360848@outlook.com>"]
 maintainers = ["Huang Kai <h1770360848@outlook.com>"]
 readme = "README.md"
 repository = "https://github.com/Huangkai1008/seedwork-python"
 classifiers = [
@@ -13,14 +13,15 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11"
 ]
 packages = [
     { include = "seedwork" },
+    { include = "seedwork/py.typed"},
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
 sqlalchemy = {version = "^2.0.18", extras = ["mypy"]}
 pydantic = "^2.0.2"
```

### Comparing `seedwork_python-0.1.0/seedwork/domain/entity.py` & `seedwork_python-0.1.1/seedwork/domain/entity.py`

 * *Files identical despite different names*

### Comparing `seedwork_python-0.1.0/seedwork/domain/repository/generic.py` & `seedwork_python-0.1.1/seedwork/domain/repository/generic.py`

 * *Files identical despite different names*

### Comparing `seedwork_python-0.1.0/seedwork/domain/unit_of_work.py` & `seedwork_python-0.1.1/seedwork/domain/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `seedwork_python-0.1.0/seedwork/infrastructure/persistence/sqlalchemy/unit_of_work.py` & `seedwork_python-0.1.1/seedwork/infrastructure/persistence/sqlalchemy/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `seedwork_python-0.1.0/PKG-INFO` & `seedwork_python-0.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seedwork-python
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python seedwork library.
 Home-page: https://github.com/Huangkai1008/seedwork-python
 License: MIT
 Author: Huang Kai
 Author-email: h1770360848@outlook.com
 Maintainer: Huang Kai
 Maintainer-email: h1770360848@outlook.com
@@ -21,23 +21,26 @@
 Project-URL: Repository, https://github.com/Huangkai1008/seedwork-python
 Description-Content-Type: text/markdown
 
 # seedwork-python
 
 Python seedwork library.
 
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
 ## Table of Contents
 
 - [Requirements](#requirements)
 - [Installation](#installation)
 - [Usage](#usage)
 - [License](#license)
 
 ## Requirements
 
+
 ## Installation
 
 ## Usage
 
 ## License
 [MIT @ Huang Kai](./LICENSE)
```

