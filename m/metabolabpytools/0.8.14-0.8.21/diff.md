# Comparing `tmp/metabolabpytools-0.8.14.tar.gz` & `tmp/metabolabpytools-0.8.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabolabpytools-0.8.14.tar", last modified: Sat Jun  3 18:27:04 2023, max compression
+gzip compressed data, was "metabolabpytools-0.8.21.tar", last modified: Sat Jul  8 22:46:01 2023, max compression
```

## Comparing `metabolabpytools-0.8.14.tar` & `metabolabpytools-0.8.21.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-06-03 18:27:04.238984 metabolabpytools-0.8.14/
--rw-r--r--   0 ludwigc    (501) staff       (20)    35149 2023-05-22 20:46:08.000000 metabolabpytools-0.8.14/LICENSE
--rw-r--r--   0 ludwigc    (501) staff       (20)       78 2023-06-03 18:26:27.000000 metabolabpytools-0.8.14/MANIFEST.in
--rw-r--r--   0 ludwigc    (501) staff       (20)     3710 2023-06-03 18:27:04.238855 metabolabpytools-0.8.14/PKG-INFO
--rw-r--r--   0 ludwigc    (501) staff       (20)       67 2023-05-22 20:46:08.000000 metabolabpytools-0.8.14/README.md
--rw-r--r--   0 ludwigc    (501) staff       (20)     2977 2023-05-28 14:07:17.000000 metabolabpytools-0.8.14/README.rst
-drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-06-03 18:27:04.237864 metabolabpytools-0.8.14/metabolabpytools/
--rw-r--r--   0 ludwigc    (501) staff       (20)      154 2023-06-03 18:26:47.000000 metabolabpytools-0.8.14/metabolabpytools/__init__.py
--rw-r--r--   0 ludwigc    (501) staff       (20)     1893 2023-05-22 20:47:01.000000 metabolabpytools-0.8.14/metabolabpytools/analysis.py
--rw-r--r--   0 ludwigc    (501) staff       (20)     2568 2023-05-22 20:48:43.000000 metabolabpytools-0.8.14/metabolabpytools/isotopomerAnalysis.py
-drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-06-03 18:27:04.238666 metabolabpytools-0.8.14/metabolabpytools.egg-info/
--rw-r--r--   0 ludwigc    (501) staff       (20)     3710 2023-06-03 18:27:04.000000 metabolabpytools-0.8.14/metabolabpytools.egg-info/PKG-INFO
--rw-r--r--   0 ludwigc    (501) staff       (20)      362 2023-06-03 18:27:04.000000 metabolabpytools-0.8.14/metabolabpytools.egg-info/SOURCES.txt
--rw-r--r--   0 ludwigc    (501) staff       (20)        1 2023-06-03 18:27:04.000000 metabolabpytools-0.8.14/metabolabpytools.egg-info/dependency_links.txt
--rw-r--r--   0 ludwigc    (501) staff       (20)       19 2023-06-03 18:27:04.000000 metabolabpytools-0.8.14/metabolabpytools.egg-info/requires.txt
--rw-r--r--   0 ludwigc    (501) staff       (20)       17 2023-06-03 18:27:04.000000 metabolabpytools-0.8.14/metabolabpytools.egg-info/top_level.txt
--rw-r--r--   0 ludwigc    (501) staff       (20)       19 2023-06-03 18:26:57.000000 metabolabpytools-0.8.14/requirements.txt
--rw-r--r--   0 ludwigc    (501) staff       (20)       38 2023-06-03 18:27:04.239017 metabolabpytools-0.8.14/setup.cfg
--rw-r--r--   0 ludwigc    (501) staff       (20)     1507 2023-05-28 14:15:23.000000 metabolabpytools-0.8.14/setup.py
+drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-08 22:46:01.478507 metabolabpytools-0.8.21/
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079    35149 2023-06-29 16:08:10.000000 metabolabpytools-0.8.21/LICENSE
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079       78 2023-06-29 16:08:10.000000 metabolabpytools-0.8.21/MANIFEST.in
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079     3710 2023-07-08 22:46:01.478328 metabolabpytools-0.8.21/PKG-INFO
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079       67 2023-06-29 16:08:10.000000 metabolabpytools-0.8.21/README.md
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079     2977 2023-06-29 16:08:10.000000 metabolabpytools-0.8.21/README.rst
+drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-08 22:46:01.477434 metabolabpytools-0.8.21/metabolabpytools/
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079      154 2023-07-08 22:44:16.000000 metabolabpytools-0.8.21/metabolabpytools/__init__.py
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079     1893 2023-06-29 16:08:10.000000 metabolabpytools-0.8.21/metabolabpytools/analysis.py
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079    12270 2023-07-08 22:44:26.000000 metabolabpytools-0.8.21/metabolabpytools/isotopomerAnalysis.py
+drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-08 22:46:01.478140 metabolabpytools-0.8.21/metabolabpytools.egg-info/
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079     3710 2023-07-08 22:46:01.000000 metabolabpytools-0.8.21/metabolabpytools.egg-info/PKG-INFO
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079      362 2023-07-08 22:46:01.000000 metabolabpytools-0.8.21/metabolabpytools.egg-info/SOURCES.txt
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079        1 2023-07-08 22:46:01.000000 metabolabpytools-0.8.21/metabolabpytools.egg-info/dependency_links.txt
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079       19 2023-07-08 22:46:01.000000 metabolabpytools-0.8.21/metabolabpytools.egg-info/requires.txt
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079       17 2023-07-08 22:46:01.000000 metabolabpytools-0.8.21/metabolabpytools.egg-info/top_level.txt
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079       19 2023-06-29 16:08:10.000000 metabolabpytools-0.8.21/requirements.txt
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079       38 2023-07-08 22:46:01.478548 metabolabpytools-0.8.21/setup.cfg
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079     1507 2023-06-29 16:08:10.000000 metabolabpytools-0.8.21/setup.py
```

### Comparing `metabolabpytools-0.8.14/LICENSE` & `metabolabpytools-0.8.21/LICENSE`

 * *Files identical despite different names*

### Comparing `metabolabpytools-0.8.14/PKG-INFO` & `metabolabpytools-0.8.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabolabpytools
-Version: 0.8.14
+Version: 0.8.21
 Summary: Tools for metabolomics and metabolism tracing data
 Home-page: https://github.com/ludwigc/metabolabpytools
 Author: Christian Ludwig
 Author-email: C.Ludwig@bham.ac.uk 
 License: GPLv3
 Keywords: Metabolomics,Tracing,NMR,Data Processing,13C
 Platform: MacOS, Windows, UNIX
```

### Comparing `metabolabpytools-0.8.14/README.rst` & `metabolabpytools-0.8.21/README.rst`

 * *Files identical despite different names*

### Comparing `metabolabpytools-0.8.14/metabolabpytools/analysis.py` & `metabolabpytools-0.8.21/metabolabpytools/analysis.py`

 * *Files identical despite different names*

### Comparing `metabolabpytools-0.8.14/metabolabpytools.egg-info/PKG-INFO` & `metabolabpytools-0.8.21/metabolabpytools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabolabpytools
-Version: 0.8.14
+Version: 0.8.21
 Summary: Tools for metabolomics and metabolism tracing data
 Home-page: https://github.com/ludwigc/metabolabpytools
 Author: Christian Ludwig
 Author-email: C.Ludwig@bham.ac.uk 
 License: GPLv3
 Keywords: Metabolomics,Tracing,NMR,Data Processing,13C
 Platform: MacOS, Windows, UNIX
```

### Comparing `metabolabpytools-0.8.14/setup.py` & `metabolabpytools-0.8.21/setup.py`

 * *Files identical despite different names*

