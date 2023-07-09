# Comparing `tmp/EDEMDSPTFEB23-0.0.6.tar.gz` & `tmp/EDEMDSPTFEB23-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EDEMDSPTFEB23-0.0.6.tar", last modified: Sun Jul  9 20:47:19 2023, max compression
+gzip compressed data, was "EDEMDSPTFEB23-0.0.7.tar", last modified: Sun Jul  9 20:53:38 2023, max compression
```

## Comparing `EDEMDSPTFEB23-0.0.6.tar` & `EDEMDSPTFEB23-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 20:47:19.485661 EDEMDSPTFEB23-0.0.6/
-drwxrwxrwx   0        0        0        0 2023-07-09 20:47:19.465657 EDEMDSPTFEB23-0.0.6/EDEMDSPTFEB23/
-drwxrwxrwx   0        0        0        0 2023-07-09 20:47:19.484661 EDEMDSPTFEB23-0.0.6/EDEMDSPTFEB23/clasificador/
--rw-rw-rw-   0        0        0       29 2023-07-09 20:38:54.000000 EDEMDSPTFEB23-0.0.6/EDEMDSPTFEB23/clasificador/__init__.py
--rw-rw-rw-   0        0        0     5502 2023-07-09 20:40:10.000000 EDEMDSPTFEB23-0.0.6/EDEMDSPTFEB23/clasificador/clasificador.py
-drwxrwxrwx   0        0        0        0 2023-07-09 20:47:19.481661 EDEMDSPTFEB23-0.0.6/EDEMDSPTFEB23.egg-info/
--rw-rw-rw-   0        0        0      180 2023-07-09 20:47:19.000000 EDEMDSPTFEB23-0.0.6/EDEMDSPTFEB23.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-07-09 20:47:19.000000 EDEMDSPTFEB23-0.0.6/EDEMDSPTFEB23.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 20:47:19.000000 EDEMDSPTFEB23-0.0.6/EDEMDSPTFEB23.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-07-09 20:47:19.000000 EDEMDSPTFEB23-0.0.6/EDEMDSPTFEB23.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-09 20:47:19.000000 EDEMDSPTFEB23-0.0.6/EDEMDSPTFEB23.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       49 2023-07-05 09:28:28.000000 EDEMDSPTFEB23-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      180 2023-07-09 20:47:19.485661 EDEMDSPTFEB23-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       96 2023-07-09 20:37:05.000000 EDEMDSPTFEB23-0.0.6/README.md
--rw-rw-rw-   0        0        0       85 2023-07-09 20:47:19.487663 EDEMDSPTFEB23-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      295 2023-07-09 20:45:30.000000 EDEMDSPTFEB23-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 20:53:38.134143 EDEMDSPTFEB23-0.0.7/
+drwxrwxrwx   0        0        0        0 2023-07-09 20:53:38.109017 EDEMDSPTFEB23-0.0.7/EDEMDSPTFEB23/
+drwxrwxrwx   0        0        0        0 2023-07-09 20:53:38.132141 EDEMDSPTFEB23-0.0.7/EDEMDSPTFEB23/clasificador/
+-rw-rw-rw-   0        0        0       29 2023-07-09 20:38:54.000000 EDEMDSPTFEB23-0.0.7/EDEMDSPTFEB23/clasificador/__init__.py
+-rw-rw-rw-   0        0        0     5502 2023-07-09 20:40:10.000000 EDEMDSPTFEB23-0.0.7/EDEMDSPTFEB23/clasificador/clasificador.py
+drwxrwxrwx   0        0        0        0 2023-07-09 20:53:38.129141 EDEMDSPTFEB23-0.0.7/EDEMDSPTFEB23.egg-info/
+-rw-rw-rw-   0        0        0      180 2023-07-09 20:53:38.000000 EDEMDSPTFEB23-0.0.7/EDEMDSPTFEB23.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-07-09 20:53:38.000000 EDEMDSPTFEB23-0.0.7/EDEMDSPTFEB23.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 20:53:38.000000 EDEMDSPTFEB23-0.0.7/EDEMDSPTFEB23.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-07-09 20:53:38.000000 EDEMDSPTFEB23-0.0.7/EDEMDSPTFEB23.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-09 20:53:38.000000 EDEMDSPTFEB23-0.0.7/EDEMDSPTFEB23.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       49 2023-07-05 09:28:28.000000 EDEMDSPTFEB23-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      180 2023-07-09 20:53:38.134143 EDEMDSPTFEB23-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       96 2023-07-09 20:37:05.000000 EDEMDSPTFEB23-0.0.7/README.md
+-rw-rw-rw-   0        0        0       85 2023-07-09 20:53:38.136142 EDEMDSPTFEB23-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      284 2023-07-09 20:53:10.000000 EDEMDSPTFEB23-0.0.7/setup.py
```

### Comparing `EDEMDSPTFEB23-0.0.6/EDEMDSPTFEB23/clasificador/clasificador.py` & `EDEMDSPTFEB23-0.0.7/EDEMDSPTFEB23/clasificador/clasificador.py`

 * *Files identical despite different names*

