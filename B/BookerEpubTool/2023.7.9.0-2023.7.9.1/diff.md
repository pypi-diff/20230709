# Comparing `tmp/BookerEpubTool-2023.7.9.0.tar.gz` & `tmp/BookerEpubTool-2023.7.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BookerEpubTool-2023.7.9.0.tar", last modified: Sun Jul  9 15:13:52 2023, max compression
+gzip compressed data, was "BookerEpubTool-2023.7.9.1.tar", last modified: Sun Jul  9 15:15:44 2023, max compression
```

## Comparing `BookerEpubTool-2023.7.9.0.tar` & `BookerEpubTool-2023.7.9.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 15:13:52.164020 BookerEpubTool-2023.7.9.0/
-drwxrwxrwx   0        0        0        0 2023-07-09 15:13:52.160021 BookerEpubTool-2023.7.9.0/BookerEpubTool/
--rw-rw-rw-   0        0        0      229 2023-07-09 14:55:30.000000 BookerEpubTool-2023.7.9.0/BookerEpubTool/__init__.py
--rw-rw-rw-   0        0        0     2725 2023-07-09 15:06:30.000000 BookerEpubTool-2023.7.9.0/BookerEpubTool/__main__.py
--rw-rw-rw-   0        0        0      708 2023-07-09 14:57:19.000000 BookerEpubTool-2023.7.9.0/BookerEpubTool/comp.py
--rw-rw-rw-   0        0        0     1200 2023-07-09 14:59:54.000000 BookerEpubTool-2023.7.9.0/BookerEpubTool/fmt.py
--rw-rw-rw-   0        0        0     4980 2023-07-09 15:05:40.000000 BookerEpubTool-2023.7.9.0/BookerEpubTool/toc.py
--rw-rw-rw-   0        0        0      890 2023-07-09 15:09:43.000000 BookerEpubTool-2023.7.9.0/BookerEpubTool/util.py
-drwxrwxrwx   0        0        0        0 2023-07-09 15:13:52.163021 BookerEpubTool-2023.7.9.0/BookerEpubTool.egg-info/
--rw-rw-rw-   0        0        0     1868 2023-07-09 15:13:52.000000 BookerEpubTool-2023.7.9.0/BookerEpubTool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      400 2023-07-09 15:13:52.000000 BookerEpubTool-2023.7.9.0/BookerEpubTool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 15:13:52.000000 BookerEpubTool-2023.7.9.0/BookerEpubTool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      105 2023-07-09 15:13:52.000000 BookerEpubTool-2023.7.9.0/BookerEpubTool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      108 2023-07-09 15:13:52.000000 BookerEpubTool-2023.7.9.0/BookerEpubTool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-09 15:13:52.000000 BookerEpubTool-2023.7.9.0/BookerEpubTool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1800 2022-04-23 14:46:34.000000 BookerEpubTool-2023.7.9.0/LICENSE
--rw-rw-rw-   0        0        0     1868 2023-07-09 15:13:52.163021 BookerEpubTool-2023.7.9.0/PKG-INFO
--rw-rw-rw-   0        0        0      631 2023-07-09 14:34:17.000000 BookerEpubTool-2023.7.9.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-09 15:13:52.164020 BookerEpubTool-2023.7.9.0/setup.cfg
--rw-rw-rw-   0        0        0     1926 2023-07-09 14:34:29.000000 BookerEpubTool-2023.7.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 15:15:44.028569 BookerEpubTool-2023.7.9.1/
+drwxrwxrwx   0        0        0        0 2023-07-09 15:15:44.024570 BookerEpubTool-2023.7.9.1/BookerEpubTool/
+-rw-rw-rw-   0        0        0      229 2023-07-09 15:15:26.000000 BookerEpubTool-2023.7.9.1/BookerEpubTool/__init__.py
+-rw-rw-rw-   0        0        0     2725 2023-07-09 15:06:30.000000 BookerEpubTool-2023.7.9.1/BookerEpubTool/__main__.py
+-rw-rw-rw-   0        0        0      708 2023-07-09 14:57:19.000000 BookerEpubTool-2023.7.9.1/BookerEpubTool/comp.py
+-rw-rw-rw-   0        0        0     1200 2023-07-09 14:59:54.000000 BookerEpubTool-2023.7.9.1/BookerEpubTool/fmt.py
+-rw-rw-rw-   0        0        0     4980 2023-07-09 15:05:40.000000 BookerEpubTool-2023.7.9.1/BookerEpubTool/toc.py
+-rw-rw-rw-   0        0        0      890 2023-07-09 15:09:43.000000 BookerEpubTool-2023.7.9.1/BookerEpubTool/util.py
+drwxrwxrwx   0        0        0        0 2023-07-09 15:15:44.027569 BookerEpubTool-2023.7.9.1/BookerEpubTool.egg-info/
+-rw-rw-rw-   0        0        0     1868 2023-07-09 15:15:43.000000 BookerEpubTool-2023.7.9.1/BookerEpubTool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      400 2023-07-09 15:15:43.000000 BookerEpubTool-2023.7.9.1/BookerEpubTool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 15:15:43.000000 BookerEpubTool-2023.7.9.1/BookerEpubTool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      105 2023-07-09 15:15:43.000000 BookerEpubTool-2023.7.9.1/BookerEpubTool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2023-07-09 15:15:43.000000 BookerEpubTool-2023.7.9.1/BookerEpubTool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-09 15:15:43.000000 BookerEpubTool-2023.7.9.1/BookerEpubTool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1800 2022-04-23 14:46:34.000000 BookerEpubTool-2023.7.9.1/LICENSE
+-rw-rw-rw-   0        0        0     1868 2023-07-09 15:15:44.027569 BookerEpubTool-2023.7.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0      631 2023-07-09 14:34:17.000000 BookerEpubTool-2023.7.9.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-09 15:15:44.028569 BookerEpubTool-2023.7.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     1926 2023-07-09 14:34:29.000000 BookerEpubTool-2023.7.9.1/setup.py
```

### Comparing `BookerEpubTool-2023.7.9.0/BookerEpubTool/__main__.py` & `BookerEpubTool-2023.7.9.1/BookerEpubTool/__main__.py`

 * *Files identical despite different names*

### Comparing `BookerEpubTool-2023.7.9.0/BookerEpubTool/comp.py` & `BookerEpubTool-2023.7.9.1/BookerEpubTool/comp.py`

 * *Files identical despite different names*

### Comparing `BookerEpubTool-2023.7.9.0/BookerEpubTool/fmt.py` & `BookerEpubTool-2023.7.9.1/BookerEpubTool/fmt.py`

 * *Files identical despite different names*

### Comparing `BookerEpubTool-2023.7.9.0/BookerEpubTool/toc.py` & `BookerEpubTool-2023.7.9.1/BookerEpubTool/toc.py`

 * *Files identical despite different names*

### Comparing `BookerEpubTool-2023.7.9.0/BookerEpubTool/util.py` & `BookerEpubTool-2023.7.9.1/BookerEpubTool/util.py`

 * *Files identical despite different names*

### Comparing `BookerEpubTool-2023.7.9.0/BookerEpubTool.egg-info/PKG-INFO` & `BookerEpubTool-2023.7.9.1/BookerEpubTool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BookerEpubTool
-Version: 2023.7.9.0
+Version: 2023.7.9.1
 Summary: iBooker/ApacheCN 知识库抓取工具
 Home-page: https://github.com/apachecn/BookerEpubTool
 Author: wizardforcel
 Author-email: wizard.z@qq.com
 Keywords: wiki,知识库,document,文档,crawler,爬虫
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `BookerEpubTool-2023.7.9.0/LICENSE` & `BookerEpubTool-2023.7.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `BookerEpubTool-2023.7.9.0/PKG-INFO` & `BookerEpubTool-2023.7.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BookerEpubTool
-Version: 2023.7.9.0
+Version: 2023.7.9.1
 Summary: iBooker/ApacheCN 知识库抓取工具
 Home-page: https://github.com/apachecn/BookerEpubTool
 Author: wizardforcel
 Author-email: wizard.z@qq.com
 Keywords: wiki,知识库,document,文档,crawler,爬虫
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `BookerEpubTool-2023.7.9.0/README.md` & `BookerEpubTool-2023.7.9.1/README.md`

 * *Files identical despite different names*

### Comparing `BookerEpubTool-2023.7.9.0/setup.py` & `BookerEpubTool-2023.7.9.1/setup.py`

 * *Files identical despite different names*

