# Comparing `tmp/bioconsertinc-1.0.1.tar.gz` & `tmp/bioconsertinc-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioconsertinc-1.0.1.tar", last modified: Sun Jul  9 21:25:07 2023, max compression
+gzip compressed data, was "bioconsertinc-1.0.2.tar", last modified: Sun Jul  9 21:35:49 2023, max compression
```

## Comparing `bioconsertinc-1.0.1.tar` & `bioconsertinc-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-09 21:25:07.344143 bioconsertinc-1.0.1/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1070 2021-11-05 18:18:30.000000 bioconsertinc-1.0.1/LICENSE
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      329 2023-07-09 21:25:07.340143 bioconsertinc-1.0.1/PKG-INFO
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      160 2021-11-06 00:01:41.000000 bioconsertinc-1.0.1/README.md
--rwxrwxr-x   0 pierre    (1000) pierre    (1000)    18702 2021-11-06 00:09:24.000000 bioconsertinc-1.0.1/bioconsertinc.c
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-09 21:25:07.340143 bioconsertinc-1.0.1/bioconsertinc.egg-info/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      329 2023-07-09 21:25:07.000000 bioconsertinc-1.0.1/bioconsertinc.egg-info/PKG-INFO
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      262 2023-07-09 21:25:07.000000 bioconsertinc-1.0.1/bioconsertinc.egg-info/SOURCES.txt
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        1 2023-07-09 21:25:07.000000 bioconsertinc-1.0.1/bioconsertinc.egg-info/dependency_links.txt
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        1 2021-11-06 00:27:50.000000 bioconsertinc-1.0.1/bioconsertinc.egg-info/not-zip-safe
--rw-rw-r--   0 pierre    (1000) pierre    (1000)       12 2023-07-09 21:25:07.000000 bioconsertinc-1.0.1/bioconsertinc.egg-info/requires.txt
--rw-rw-r--   0 pierre    (1000) pierre    (1000)       14 2023-07-09 21:25:07.000000 bioconsertinc-1.0.1/bioconsertinc.egg-info/top_level.txt
--rw-rw-r--   0 pierre    (1000) pierre    (1000)       38 2023-07-09 21:25:07.344143 bioconsertinc-1.0.1/setup.cfg
--rwxrwxr-x   0 pierre    (1000) pierre    (1000)      694 2023-07-09 21:18:27.000000 bioconsertinc-1.0.1/setup.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-09 21:35:49.377018 bioconsertinc-1.0.2/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     1070 2021-11-05 18:18:30.000000 bioconsertinc-1.0.2/LICENSE
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      329 2023-07-09 21:35:49.377018 bioconsertinc-1.0.2/PKG-INFO
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      160 2021-11-06 00:01:41.000000 bioconsertinc-1.0.2/README.md
+-rwxrwxr-x   0 pierre    (1000) pierre    (1000)    18702 2021-11-06 00:09:24.000000 bioconsertinc-1.0.2/bioconsertinc.c
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-09 21:35:49.377018 bioconsertinc-1.0.2/bioconsertinc.egg-info/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      329 2023-07-09 21:35:49.000000 bioconsertinc-1.0.2/bioconsertinc.egg-info/PKG-INFO
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      277 2023-07-09 21:35:49.000000 bioconsertinc-1.0.2/bioconsertinc.egg-info/SOURCES.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        1 2023-07-09 21:35:49.000000 bioconsertinc-1.0.2/bioconsertinc.egg-info/dependency_links.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        1 2021-11-06 00:27:50.000000 bioconsertinc-1.0.2/bioconsertinc.egg-info/not-zip-safe
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       12 2023-07-09 21:35:49.000000 bioconsertinc-1.0.2/bioconsertinc.egg-info/requires.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       14 2023-07-09 21:35:49.000000 bioconsertinc-1.0.2/bioconsertinc.egg-info/top_level.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       99 2023-07-09 21:34:35.000000 bioconsertinc-1.0.2/pyproject.toml
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       38 2023-07-09 21:35:49.377018 bioconsertinc-1.0.2/setup.cfg
+-rwxrwxr-x   0 pierre    (1000) pierre    (1000)      694 2023-07-09 21:34:48.000000 bioconsertinc-1.0.2/setup.py
```

### Comparing `bioconsertinc-1.0.1/LICENSE` & `bioconsertinc-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bioconsertinc-1.0.1/bioconsertinc.c` & `bioconsertinc-1.0.2/bioconsertinc.c`

 * *Files identical despite different names*

### Comparing `bioconsertinc-1.0.1/setup.py` & `bioconsertinc-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from distutils.extension import Extension
 
 def get_numpy_include_dirs():
     import numpy
     return [numpy.get_include()]
 
 setup(name='bioconsertinc',
-      version='1.0.1',
+      version='1.0.2',
       description='BioConsert, c implementation',
       url='https://github.com/pierreandrieu/bioconsertinc',
       long_description='BioConsert algorithm, c implementation',
       author='Pierre Andrieu',
       author_email='pierre.andrieu@lilo.org',
       license='MIT',
       ext_modules=[Extension("bioconsertinc", ["bioconsertinc.c"], include_dirs=get_numpy_include_dirs())],
```

