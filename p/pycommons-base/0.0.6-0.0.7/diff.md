# Comparing `tmp/pycommons_base-0.0.6.tar.gz` & `tmp/pycommons_base-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycommons_base-0.0.6.tar", max compression
+gzip compressed data, was "pycommons_base-0.0.7.tar", max compression
```

## Comparing `pycommons_base-0.0.6.tar` & `pycommons_base-0.0.7.tar`

### file list

```diff
@@ -1,35 +1,37 @@
--rw-r--r--   0        0        0    11346 2023-06-30 10:20:07.019579 pycommons_base-0.0.6/LICENSE
--rw-r--r--   0        0        0     1082 2023-06-30 10:20:07.019579 pycommons_base-0.0.6/README.md
--rw-r--r--   0        0        0      431 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/__init__.py
--rw-r--r--   0        0        0      153 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/atomic/__init__.py
--rw-r--r--   0        0        0     1348 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/atomic/atomic.py
--rw-r--r--   0        0        0     1136 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/atomic/boolean.py
--rw-r--r--   0        0        0     1791 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/atomic/integer.py
--rw-r--r--   0        0        0     5648 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/char.py
--rw-r--r--   0        0        0      235 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/container/__init__.py
--rw-r--r--   0        0        0     3191 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/container/boolean.py
--rw-r--r--   0        0        0     3100 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/container/container.py
--rw-r--r--   0        0        0     4334 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/container/integer.py
--rw-r--r--   0        0        0     4733 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/container/optional.py
--rw-r--r--   0        0        0      427 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/exception/__init__.py
--rw-r--r--   0        0        0      607 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/function/__init__.py
--rw-r--r--   0        0        0     1266 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/function/comparator.py
--rw-r--r--   0        0        0     2451 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/function/consumer.py
--rw-r--r--   0        0        0     1089 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/function/function.py
--rw-r--r--   0        0        0      215 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/function/interface.py
--rw-r--r--   0        0        0     4570 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/function/predicate.py
--rw-r--r--   0        0        0     1752 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/function/runnable.py
--rw-r--r--   0        0        0     2051 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/function/supplier.py
--rw-r--r--   0        0        0       41 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/maps/__init__.py
--rw-r--r--   0        0        0     6975 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/maps/maps.py
--rw-r--r--   0        0        0      144 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/streams/__init__.py
--rw-r--r--   0        0        0     6823 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/streams/iterator.py
--rw-r--r--   0        0        0     2264 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/streams/stream.py
--rw-r--r--   0        0        0      725 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/streams/streams.py
--rw-r--r--   0        0        0      987 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/synchronized.py
--rw-r--r--   0        0        0      112 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/utils/__init__.py
--rw-r--r--   0        0        0     1458 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/utils/objectutils.py
--rw-r--r--   0        0        0      119 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/base/utils/utils.py
--rw-r--r--   0        0        0        0 2023-06-30 10:20:07.023579 pycommons_base-0.0.6/pycommons/py.typed
--rw-r--r--   0        0        0     1821 2023-06-30 10:20:21.443592 pycommons_base-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1860 1970-01-01 00:00:00.000000 pycommons_base-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-07-09 19:27:23.669166 pycommons_base-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1082 2023-07-09 19:27:23.669166 pycommons_base-0.0.7/README.md
+-rw-r--r--   0        0        0      572 2023-07-09 19:27:23.673167 pycommons_base-0.0.7/pycommons/base/__init__.py
+-rw-r--r--   0        0        0      153 2023-07-09 19:27:23.673167 pycommons_base-0.0.7/pycommons/base/atomic/__init__.py
+-rw-r--r--   0        0        0     1348 2023-07-09 19:27:23.673167 pycommons_base-0.0.7/pycommons/base/atomic/atomic.py
+-rw-r--r--   0        0        0     1136 2023-07-09 19:27:23.673167 pycommons_base-0.0.7/pycommons/base/atomic/boolean.py
+-rw-r--r--   0        0        0     1791 2023-07-09 19:27:23.673167 pycommons_base-0.0.7/pycommons/base/atomic/integer.py
+-rw-r--r--   0        0        0     5648 2023-07-09 19:27:23.673167 pycommons_base-0.0.7/pycommons/base/char.py
+-rw-r--r--   0        0        0      235 2023-07-09 19:27:23.673167 pycommons_base-0.0.7/pycommons/base/container/__init__.py
+-rw-r--r--   0        0        0     3191 2023-07-09 19:27:23.673167 pycommons_base-0.0.7/pycommons/base/container/boolean.py
+-rw-r--r--   0        0        0     3100 2023-07-09 19:27:23.673167 pycommons_base-0.0.7/pycommons/base/container/container.py
+-rw-r--r--   0        0        0     4334 2023-07-09 19:27:23.673167 pycommons_base-0.0.7/pycommons/base/container/integer.py
+-rw-r--r--   0        0        0     4733 2023-07-09 19:27:23.673167 pycommons_base-0.0.7/pycommons/base/container/optional.py
+-rw-r--r--   0        0        0      427 2023-07-09 19:27:23.673167 pycommons_base-0.0.7/pycommons/base/exception/__init__.py
+-rw-r--r--   0        0        0      607 2023-07-09 19:27:23.673167 pycommons_base-0.0.7/pycommons/base/function/__init__.py
+-rw-r--r--   0        0        0     1266 2023-07-09 19:27:23.673167 pycommons_base-0.0.7/pycommons/base/function/comparator.py
+-rw-r--r--   0        0        0     2451 2023-07-09 19:27:23.673167 pycommons_base-0.0.7/pycommons/base/function/consumer.py
+-rw-r--r--   0        0        0     1089 2023-07-09 19:27:23.673167 pycommons_base-0.0.7/pycommons/base/function/function.py
+-rw-r--r--   0        0        0      215 2023-07-09 19:27:23.673167 pycommons_base-0.0.7/pycommons/base/function/interface.py
+-rw-r--r--   0        0        0     4570 2023-07-09 19:27:23.673167 pycommons_base-0.0.7/pycommons/base/function/predicate.py
+-rw-r--r--   0        0        0     1752 2023-07-09 19:27:23.673167 pycommons_base-0.0.7/pycommons/base/function/runnable.py
+-rw-r--r--   0        0        0     2051 2023-07-09 19:27:23.673167 pycommons_base-0.0.7/pycommons/base/function/supplier.py
+-rw-r--r--   0        0        0       41 2023-07-09 19:27:23.673167 pycommons_base-0.0.7/pycommons/base/maps/__init__.py
+-rw-r--r--   0        0        0     6975 2023-07-09 19:27:23.673167 pycommons_base-0.0.7/pycommons/base/maps/maps.py
+-rw-r--r--   0        0        0      144 2023-07-09 19:27:23.673167 pycommons_base-0.0.7/pycommons/base/streams/__init__.py
+-rw-r--r--   0        0        0     6823 2023-07-09 19:27:23.673167 pycommons_base-0.0.7/pycommons/base/streams/iterator.py
+-rw-r--r--   0        0        0     2264 2023-07-09 19:27:23.673167 pycommons_base-0.0.7/pycommons/base/streams/stream.py
+-rw-r--r--   0        0        0      725 2023-07-09 19:27:23.673167 pycommons_base-0.0.7/pycommons/base/streams/streams.py
+-rw-r--r--   0        0        0      987 2023-07-09 19:27:23.673167 pycommons_base-0.0.7/pycommons/base/synchronized.py
+-rw-r--r--   0        0        0       64 2023-07-09 19:27:23.673167 pycommons_base-0.0.7/pycommons/base/threading/__init__.py
+-rw-r--r--   0        0        0     4287 2023-07-09 19:27:23.673167 pycommons_base-0.0.7/pycommons/base/threading/context.py
+-rw-r--r--   0        0        0      112 2023-07-09 19:27:23.673167 pycommons_base-0.0.7/pycommons/base/utils/__init__.py
+-rw-r--r--   0        0        0     1458 2023-07-09 19:27:23.673167 pycommons_base-0.0.7/pycommons/base/utils/objectutils.py
+-rw-r--r--   0        0        0      119 2023-07-09 19:27:23.673167 pycommons_base-0.0.7/pycommons/base/utils/utils.py
+-rw-r--r--   0        0        0        0 2023-07-09 19:27:23.673167 pycommons_base-0.0.7/pycommons/py.typed
+-rw-r--r--   0        0        0     1817 2023-07-09 19:27:36.717379 pycommons_base-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1856 1970-01-01 00:00:00.000000 pycommons_base-0.0.7/PKG-INFO
```

### Comparing `pycommons_base-0.0.6/LICENSE` & `pycommons_base-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.6/README.md` & `pycommons_base-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.6/pycommons/base/atomic/atomic.py` & `pycommons_base-0.0.7/pycommons/base/atomic/atomic.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.6/pycommons/base/atomic/boolean.py` & `pycommons_base-0.0.7/pycommons/base/atomic/boolean.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.6/pycommons/base/atomic/integer.py` & `pycommons_base-0.0.7/pycommons/base/atomic/integer.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.6/pycommons/base/char.py` & `pycommons_base-0.0.7/pycommons/base/char.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.6/pycommons/base/container/boolean.py` & `pycommons_base-0.0.7/pycommons/base/container/boolean.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.6/pycommons/base/container/container.py` & `pycommons_base-0.0.7/pycommons/base/container/container.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.6/pycommons/base/container/integer.py` & `pycommons_base-0.0.7/pycommons/base/container/integer.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.6/pycommons/base/container/optional.py` & `pycommons_base-0.0.7/pycommons/base/container/optional.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.6/pycommons/base/function/__init__.py` & `pycommons_base-0.0.7/pycommons/base/function/__init__.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.6/pycommons/base/function/comparator.py` & `pycommons_base-0.0.7/pycommons/base/function/comparator.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.6/pycommons/base/function/consumer.py` & `pycommons_base-0.0.7/pycommons/base/function/consumer.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.6/pycommons/base/function/function.py` & `pycommons_base-0.0.7/pycommons/base/function/function.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.6/pycommons/base/function/predicate.py` & `pycommons_base-0.0.7/pycommons/base/function/predicate.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.6/pycommons/base/function/runnable.py` & `pycommons_base-0.0.7/pycommons/base/function/runnable.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.6/pycommons/base/function/supplier.py` & `pycommons_base-0.0.7/pycommons/base/function/supplier.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.6/pycommons/base/maps/maps.py` & `pycommons_base-0.0.7/pycommons/base/maps/maps.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.6/pycommons/base/streams/iterator.py` & `pycommons_base-0.0.7/pycommons/base/streams/iterator.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.6/pycommons/base/streams/stream.py` & `pycommons_base-0.0.7/pycommons/base/streams/stream.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.6/pycommons/base/streams/streams.py` & `pycommons_base-0.0.7/pycommons/base/streams/streams.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.6/pycommons/base/synchronized.py` & `pycommons_base-0.0.7/pycommons/base/synchronized.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.6/pycommons/base/utils/objectutils.py` & `pycommons_base-0.0.7/pycommons/base/utils/objectutils.py`

 * *Files identical despite different names*

### Comparing `pycommons_base-0.0.6/pyproject.toml` & `pycommons_base-0.0.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool]
 
 [tool.poetry]
 name = "pycommons.base"
-version = "0.0.6"
-homepage = "https://github.com/shashankrnr32/pycommons-base"
+version = "0.0.7"
+homepage = "https://github.com/pycommons/pycommons-base"
 description = "Python Commons Base"
 authors = ["Shashank Sharma <shashankrnr32@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
     'License :: OSI Approved :: Apache Software License',
     'Natural Language :: English',
@@ -53,15 +53,15 @@
 disable = "C0103, C0116, C0114, C0115, R0801, R0903"
 max-public-methods = 50
 max-args = 8
 max-locals = 20
 min-public-method = 0
 
 [tool.pytest.ini_options]
-addopts = "--cov=pycommons --cov-branch --cov-report term-missing --cov-report xml -vv --color=yes --cov-fail-under 45"
+addopts = "--cov=pycommons --cov-branch --cov-report term-missing --cov-report xml -vv --color=yes --cov-fail-under 60"
 python_files = "tests.py test_*.py *_tests.py *Test.py"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.mypy.overrides]
```

### Comparing `pycommons_base-0.0.6/PKG-INFO` & `pycommons_base-0.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pycommons-base
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python Commons Base
-Home-page: https://github.com/shashankrnr32/pycommons-base
+Home-page: https://github.com/pycommons/pycommons-base
 License: Apache-2.0
 Author: Shashank Sharma
 Author-email: shashankrnr32@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

