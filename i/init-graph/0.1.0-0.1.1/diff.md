# Comparing `tmp/init_graph-0.1.0.tar.gz` & `tmp/init_graph-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "init_graph-0.1.0.tar", max compression
+gzip compressed data, was "init_graph-0.1.1.tar", max compression
```

## Comparing `init_graph-0.1.0.tar` & `init_graph-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-07-09 18:32:52.461549 init_graph-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-09 18:32:52.461478 init_graph-0.1.0/init_graph/__init__.py
--rw-r--r--   0        0        0       52 2023-07-09 18:37:18.858878 init_graph-0.1.0/init_graph/__main__.py
--rw-r--r--   0        0        0     1543 2023-07-09 19:13:54.408679 init_graph-0.1.0/init_graph/chapters.py
--rw-r--r--   0        0        0     1236 2023-07-09 18:41:18.437157 init_graph-0.1.0/init_graph/choice_option.py
--rw-r--r--   0        0        0     2749 2023-07-09 19:19:54.590729 init_graph-0.1.0/init_graph/graph.py
--rw-r--r--   0        0        0     3915 2023-07-09 19:23:18.557572 init_graph-0.1.0/init_graph/main.py
--rw-r--r--   0        0        0      390 2023-07-09 18:35:20.031628 init_graph-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      332 1970-01-01 00:00:00.000000 init_graph-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-09 18:32:52.461549 init_graph-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-09 18:32:52.461478 init_graph-0.1.1/init_graph/__init__.py
+-rw-r--r--   0        0        0       52 2023-07-09 18:37:18.858878 init_graph-0.1.1/init_graph/__main__.py
+-rw-r--r--   0        0        0     1543 2023-07-09 19:13:54.408679 init_graph-0.1.1/init_graph/chapters.py
+-rw-r--r--   0        0        0     1236 2023-07-09 18:41:18.437157 init_graph-0.1.1/init_graph/choice_option.py
+-rw-r--r--   0        0        0     2749 2023-07-09 19:19:54.590729 init_graph-0.1.1/init_graph/graph.py
+-rw-r--r--   0        0        0     3920 2023-07-09 19:27:14.040630 init_graph-0.1.1/init_graph/main.py
+-rw-r--r--   0        0        0      428 2023-07-09 19:27:48.811154 init_graph-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      370 1970-01-01 00:00:00.000000 init_graph-0.1.1/PKG-INFO
```

### Comparing `init_graph-0.1.0/init_graph/chapters.py` & `init_graph-0.1.1/init_graph/chapters.py`

 * *Files identical despite different names*

### Comparing `init_graph-0.1.0/init_graph/choice_option.py` & `init_graph-0.1.1/init_graph/choice_option.py`

 * *Files identical despite different names*

### Comparing `init_graph-0.1.0/init_graph/graph.py` & `init_graph-0.1.1/init_graph/graph.py`

 * *Files identical despite different names*

### Comparing `init_graph-0.1.0/init_graph/main.py` & `init_graph-0.1.1/init_graph/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import time
 
 
 from .chapters import chapters_list
 from .graph import Graph
 from .choice_option import ChoiceOption
 
-path_parent = os.environ["TEX_PARENT_PATH"] 
+path_parent = os.environ["TEX_PARENT_PATH_MATHS"]
 
 eqn_number_without_database = f'{int(time.strftime("%H%M%S%d%m%Y")):14}'
 
 link = r"""
 \def\gdrive{Link}
 """
```

