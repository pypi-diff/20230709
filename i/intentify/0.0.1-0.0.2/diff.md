# Comparing `tmp/intentify-0.0.1.tar.gz` & `tmp/intentify-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intentify-0.0.1.tar", last modified: Sun Jul  9 18:26:39 2023, max compression
+gzip compressed data, was "intentify-0.0.2.tar", last modified: Sun Jul  9 18:33:45 2023, max compression
```

## Comparing `intentify-0.0.1.tar` & `intentify-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 18:26:39.948643 intentify-0.0.1/
--rw-rw-rw-   0        0        0      655 2023-07-09 18:26:39.948139 intentify-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2183 2023-07-09 18:18:34.000000 intentify-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-09 18:26:39.939162 intentify-0.0.1/intentify/
--rw-rw-rw-   0        0        0       36 2023-07-07 19:32:27.000000 intentify-0.0.1/intentify/__init__.py
--rw-rw-rw-   0        0        0     6570 2023-07-07 20:09:00.000000 intentify-0.0.1/intentify/main.py
-drwxrwxrwx   0        0        0        0 2023-07-09 18:26:39.947142 intentify-0.0.1/intentify.egg-info/
--rw-rw-rw-   0        0        0      655 2023-07-09 18:26:39.000000 intentify-0.0.1/intentify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-07-09 18:26:39.000000 intentify-0.0.1/intentify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 18:26:39.000000 intentify-0.0.1/intentify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-07-09 18:26:39.000000 intentify-0.0.1/intentify.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-09 18:26:39.000000 intentify-0.0.1/intentify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-09 18:26:39.948643 intentify-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1010 2023-07-09 18:25:21.000000 intentify-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:33:45.370852 intentify-0.0.2/
+-rw-rw-rw-   0        0        0     2753 2023-07-09 18:33:45.369852 intentify-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2183 2023-07-09 18:18:34.000000 intentify-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 18:33:45.359771 intentify-0.0.2/intentify/
+-rw-rw-rw-   0        0        0       36 2023-07-07 19:32:27.000000 intentify-0.0.2/intentify/__init__.py
+-rw-rw-rw-   0        0        0     6570 2023-07-07 20:09:00.000000 intentify-0.0.2/intentify/main.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:33:45.369852 intentify-0.0.2/intentify.egg-info/
+-rw-rw-rw-   0        0        0     2753 2023-07-09 18:33:45.000000 intentify-0.0.2/intentify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-07-09 18:33:45.000000 intentify-0.0.2/intentify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 18:33:45.000000 intentify-0.0.2/intentify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-07-09 18:33:45.000000 intentify-0.0.2/intentify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-09 18:33:45.000000 intentify-0.0.2/intentify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-09 18:33:45.370852 intentify-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1022 2023-07-09 18:32:36.000000 intentify-0.0.2/setup.py
```

### Comparing `intentify-0.0.1/README.md` & `intentify-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `intentify-0.0.1/intentify/main.py` & `intentify-0.0.2/intentify/main.py`

 * *Files identical despite different names*

### Comparing `intentify-0.0.1/setup.py` & `intentify-0.0.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from setuptools import setup, find_packages
-import os
 
-VERSION = '0.0.1'
+from pathlib import Path
+this_directory = Path(__file__).parent
+LONG_DESCRIPTION = (this_directory / "README.md").read_text()
+
+VERSION = '0.0.2'
 DESCRIPTION = 'An intent classification library for AI Models.'
-LONG_DESCRIPTION = 'A library for training and testing small to large scale intent classification models.'
 
 # Setting up
 setup(
     name="intentify",
     version=VERSION,
     author="Ice (Rishan Pancham)",
     author_email="<rishanpan@hotmail.com>",
```

