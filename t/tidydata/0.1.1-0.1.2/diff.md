# Comparing `tmp/tidydata-0.1.1.tar.gz` & `tmp/tidydata-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidydata-0.1.1.tar", max compression
+gzip compressed data, was "tidydata-0.1.2.tar", max compression
```

## Comparing `tidydata-0.1.1.tar` & `tidydata-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      116 2023-06-21 13:25:39.956791 tidydata-0.1.1/README.md
--rw-r--r--   0        0        0      667 2023-07-09 14:21:28.704727 tidydata-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        2 2023-06-19 10:17:46.976922 tidydata-0.1.1/tidydata/__init__.py
--rw-r--r--   0        0        0       77 2023-06-19 10:17:46.976922 tidydata-0.1.1/tidydata/__main__.py
--rw-r--r--   0        0        0     1483 2023-06-30 09:11:54.490828 tidydata-0.1.1/tidydata/cli.py
--rw-r--r--   0        0        0    17287 2023-07-08 11:37:17.902116 tidydata-0.1.1/tidydata/config.py
--rw-r--r--   0        0        0    22749 2023-07-07 15:25:00.545473 tidydata-0.1.1/tidydata/core.py
--rw-r--r--   0        0        0     7218 2023-07-08 12:01:21.412965 tidydata-0.1.1/tidydata/variable.py
--rw-r--r--   0        0        0      851 1970-01-01 00:00:00.000000 tidydata-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      116 2023-06-21 13:25:39.956791 tidydata-0.1.2/README.md
+-rw-r--r--   0        0        0      687 2023-07-09 14:28:14.510691 tidydata-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        2 2023-06-19 10:17:46.976922 tidydata-0.1.2/tidydata/__init__.py
+-rw-r--r--   0        0        0       77 2023-06-19 10:17:46.976922 tidydata-0.1.2/tidydata/__main__.py
+-rw-r--r--   0        0        0     1483 2023-06-30 09:11:54.490828 tidydata-0.1.2/tidydata/cli.py
+-rw-r--r--   0        0        0    17287 2023-07-08 11:37:17.902116 tidydata-0.1.2/tidydata/config.py
+-rw-r--r--   0        0        0    22749 2023-07-07 15:25:00.545473 tidydata-0.1.2/tidydata/core.py
+-rw-r--r--   0        0        0     7218 2023-07-08 12:01:21.412965 tidydata-0.1.2/tidydata/variable.py
+-rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 tidydata-0.1.2/PKG-INFO
```

### Comparing `tidydata-0.1.1/pyproject.toml` & `tidydata-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tidydata"
-version = "0.1.1"
+version = "0.1.2"
 description = "Data cleaner"
 authors = ["Kyrie He <kyrie1218@163.com>"]
 readme = "README.md"
 
 [[tool.poetry.source]]
 name = "tsinghua"
 url = "https://mirrors.tuna.tsinghua.edu.cn/pypi/web/simple/"
@@ -19,14 +19,15 @@
 pydantic = "^1.10.7"
 pyarrow = "^12.0.0"
 typeguard = "^4.0.0"
 click = "^8.1.3"
 rich = "^13.4.1"
 duckdb = "^0.8.0"
 openpyxl = "^3.1.2"
+sqlparse = "^0.4.4"
 
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.2"
 
 [build-system]
```

### Comparing `tidydata-0.1.1/tidydata/cli.py` & `tidydata-0.1.2/tidydata/cli.py`

 * *Files identical despite different names*

### Comparing `tidydata-0.1.1/tidydata/config.py` & `tidydata-0.1.2/tidydata/config.py`

 * *Files identical despite different names*

### Comparing `tidydata-0.1.1/tidydata/core.py` & `tidydata-0.1.2/tidydata/core.py`

 * *Files identical despite different names*

### Comparing `tidydata-0.1.1/tidydata/variable.py` & `tidydata-0.1.2/tidydata/variable.py`

 * *Files identical despite different names*

### Comparing `tidydata-0.1.1/PKG-INFO` & `tidydata-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidydata
-Version: 0.1.1
+Version: 0.1.2
 Summary: Data cleaner
 Author: Kyrie He
 Author-email: kyrie1218@163.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
@@ -13,14 +13,15 @@
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: pyarrow (>=12.0.0,<13.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
 Requires-Dist: rich (>=13.4.1,<14.0.0)
+Requires-Dist: sqlparse (>=0.4.4,<0.5.0)
 Requires-Dist: typeguard (>=4.0.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 硬件要求： 16G内存 (取决于需要导入的数据)
 系统： Linux
 python： 3.11+
 stata: 17+
```

