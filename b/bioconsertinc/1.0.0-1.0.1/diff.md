# Comparing `tmp/bioconsertinc-1.0.0.tar.gz` & `tmp/bioconsertinc-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bioconsertinc-1.0.0.tar", last modified: Sat Nov  6 01:27:07 2021, max compression
+gzip compressed data, was "bioconsertinc-1.0.1.tar", last modified: Sun Jul  9 21:25:07 2023, max compression
```

## Comparing `bioconsertinc-1.0.0.tar` & `bioconsertinc-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-11-06 01:27:07.000000 bioconsertinc-1.0.0/
--rwxrwxr-x   0 pierre    (1000) pierre    (1000)    18702 2021-11-06 00:09:24.000000 bioconsertinc-1.0.0/bioconsertinc.c
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1070 2021-11-05 18:18:30.000000 bioconsertinc-1.0.0/LICENSE
--rwxrwxr-x   0 pierre    (1000) pierre    (1000)      722 2021-11-06 00:27:46.000000 bioconsertinc-1.0.0/setup.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-11-06 01:27:07.000000 bioconsertinc-1.0.0/bioconsertinc.egg-info/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)       14 2021-11-06 01:27:07.000000 bioconsertinc-1.0.0/bioconsertinc.egg-info/top_level.txt
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        1 2021-11-06 00:27:50.000000 bioconsertinc-1.0.0/bioconsertinc.egg-info/not-zip-safe
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      262 2021-11-06 01:27:07.000000 bioconsertinc-1.0.0/bioconsertinc.egg-info/SOURCES.txt
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      329 2021-11-06 01:27:07.000000 bioconsertinc-1.0.0/bioconsertinc.egg-info/PKG-INFO
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        1 2021-11-06 01:27:07.000000 bioconsertinc-1.0.0/bioconsertinc.egg-info/dependency_links.txt
--rw-rw-r--   0 pierre    (1000) pierre    (1000)       12 2021-11-06 01:27:07.000000 bioconsertinc-1.0.0/bioconsertinc.egg-info/requires.txt
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      329 2021-11-06 01:27:07.000000 bioconsertinc-1.0.0/PKG-INFO
--rw-rw-r--   0 pierre    (1000) pierre    (1000)       38 2021-11-06 01:27:07.000000 bioconsertinc-1.0.0/setup.cfg
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      160 2021-11-06 00:01:41.000000 bioconsertinc-1.0.0/README.md
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-09 21:25:07.344143 bioconsertinc-1.0.1/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     1070 2021-11-05 18:18:30.000000 bioconsertinc-1.0.1/LICENSE
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      329 2023-07-09 21:25:07.340143 bioconsertinc-1.0.1/PKG-INFO
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      160 2021-11-06 00:01:41.000000 bioconsertinc-1.0.1/README.md
+-rwxrwxr-x   0 pierre    (1000) pierre    (1000)    18702 2021-11-06 00:09:24.000000 bioconsertinc-1.0.1/bioconsertinc.c
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-09 21:25:07.340143 bioconsertinc-1.0.1/bioconsertinc.egg-info/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      329 2023-07-09 21:25:07.000000 bioconsertinc-1.0.1/bioconsertinc.egg-info/PKG-INFO
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      262 2023-07-09 21:25:07.000000 bioconsertinc-1.0.1/bioconsertinc.egg-info/SOURCES.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        1 2023-07-09 21:25:07.000000 bioconsertinc-1.0.1/bioconsertinc.egg-info/dependency_links.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        1 2021-11-06 00:27:50.000000 bioconsertinc-1.0.1/bioconsertinc.egg-info/not-zip-safe
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       12 2023-07-09 21:25:07.000000 bioconsertinc-1.0.1/bioconsertinc.egg-info/requires.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       14 2023-07-09 21:25:07.000000 bioconsertinc-1.0.1/bioconsertinc.egg-info/top_level.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       38 2023-07-09 21:25:07.344143 bioconsertinc-1.0.1/setup.cfg
+-rwxrwxr-x   0 pierre    (1000) pierre    (1000)      694 2023-07-09 21:18:27.000000 bioconsertinc-1.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bioconsertinc-1.0.0/bioconsertinc.c` & `bioconsertinc-1.0.1/bioconsertinc.c`

 * *Files identical despite different names*

### Comparing `bioconsertinc-1.0.0/LICENSE` & `bioconsertinc-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bioconsertinc-1.0.0/setup.py` & `bioconsertinc-1.0.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from setuptools import setup, find_packages
 from distutils.extension import Extension
-import numpy 
+
+def get_numpy_include_dirs():
+    import numpy
+    return [numpy.get_include()]
 
 setup(name='bioconsertinc',
-      version='1.0.0',
+      version='1.0.1',
       description='BioConsert, c implementation',
       url='https://github.com/pierreandrieu/bioconsertinc',
       long_description='BioConsert algorithm, c implementation',
       author='Pierre Andrieu',
       author_email='pierre.andrieu@lilo.org',
       license='MIT',
-      # packages=find_packages(include=['bioconsertc', 'bioconsertc.*']),
-      ext_modules=[Extension("bioconsertinc", ["bioconsertinc.c"],
-                  include_dirs=[numpy.get_include()])],
+      ext_modules=[Extension("bioconsertinc", ["bioconsertinc.c"], include_dirs=get_numpy_include_dirs())],
       python_requires='>=3',
       zip_safe=False,
       install_requires=['numpy>=1.13'],
-      )
+)
```

