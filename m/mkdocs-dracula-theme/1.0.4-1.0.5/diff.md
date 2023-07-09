# Comparing `tmp/mkdocs-dracula-theme-1.0.4.tar.gz` & `tmp/mkdocs-dracula-theme-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-dracula-theme-1.0.4.tar", last modified: Sun Mar 26 00:41:36 2023, max compression
+gzip compressed data, was "mkdocs-dracula-theme-1.0.5.tar", last modified: Sun Jul  9 17:28:28 2023, max compression
```

## Comparing `mkdocs-dracula-theme-1.0.4.tar` & `mkdocs-dracula-theme-1.0.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 00:41:36.723472 mkdocs-dracula-theme-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-26 00:41:22.000000 mkdocs-dracula-theme-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-03-26 00:41:36.723472 mkdocs-dracula-theme-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-03-26 00:41:22.000000 mkdocs-dracula-theme-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 00:41:36.719472 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-03-26 00:41:22.000000 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/404.html
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-03-26 00:41:22.000000 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 00:41:36.719472 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-03-26 00:41:36.000000 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/__pycache__/__init__.cpython-310.pyc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 00:41:36.715472 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 00:41:36.719472 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)   220779 2023-03-26 00:41:22.000000 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/assets/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   568408 2023-03-26 00:41:23.000000 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/assets/css/bootstrap.min.css.map
--rw-r--r--   0 runner    (1001) docker     (123)    52506 2023-03-26 00:41:23.000000 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/assets/css/dracula-ui.css
--rw-r--r--   0 runner    (1001) docker     (123)   113611 2023-03-26 00:41:23.000000 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/assets/css/dracula-ui.css.map
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-03-26 00:41:23.000000 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/assets/css/mkdocs.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 00:41:36.723472 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/assets/img/
--rw-r--r--   0 runner    (1001) docker     (123)   150941 2023-03-26 00:41:23.000000 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/assets/img/dracula.png
--rw-r--r--   0 runner    (1001) docker     (123)    11147 2023-03-26 00:41:23.000000 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/assets/img/dracula.svg
--rw-r--r--   0 runner    (1001) docker     (123)    25756 2023-03-26 00:41:23.000000 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/assets/img/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 00:41:36.723472 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/assets/js/
--rw-r--r--   0 runner    (1001) docker     (123)    80599 2023-03-26 00:41:23.000000 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/assets/js/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   333974 2023-03-26 00:41:23.000000 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/assets/js/bootstrap.bundle.min.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    69916 2023-03-26 00:41:23.000000 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/assets/js/jquery-3.3.1.slim.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-03-26 00:41:23.000000 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/assets/js/mkdocs.js
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-03-26 00:41:23.000000 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/base.html
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-26 00:41:23.000000 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/main.html
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-26 00:41:23.000000 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/mkdocs_theme.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 00:41:36.723472 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-26 00:41:23.000000 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/modules/content.html
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-03-26 00:41:23.000000 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/modules/dropdown-menu.html
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-26 00:41:23.000000 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/modules/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-03-26 00:41:23.000000 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/modules/header.html
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-03-26 00:41:23.000000 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/modules/menu.html
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-03-26 00:41:23.000000 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/modules/preview.html
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-03-26 00:41:23.000000 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/modules/sidebar.html
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-03-26 00:41:23.000000 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/modules/source.html
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-03-26 00:41:23.000000 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/search.html
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-03-26 00:41:23.000000 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/searchbox.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 00:41:36.719472 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-03-26 00:41:36.000000 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-03-26 00:41:36.000000 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 00:41:36.000000 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-26 00:41:36.000000 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-26 00:41:36.000000 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-26 00:41:36.000000 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 00:41:36.000000 mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-26 00:41:36.723472 mkdocs-dracula-theme-1.0.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-03-26 00:41:23.000000 mkdocs-dracula-theme-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:28:28.872467 mkdocs-dracula-theme-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-09 17:28:15.000000 mkdocs-dracula-theme-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-09 17:28:28.872467 mkdocs-dracula-theme-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-09 17:28:15.000000 mkdocs-dracula-theme-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:28:28.868467 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-09 17:28:15.000000 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-09 17:28:15.000000 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:28:28.868467 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-09 17:28:28.000000 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/__pycache__/__init__.cpython-310.pyc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:28:28.868467 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:28:28.872467 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   220779 2023-07-09 17:28:15.000000 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/assets/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   568408 2023-07-09 17:28:15.000000 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/assets/css/bootstrap.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    52506 2023-07-09 17:28:15.000000 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/assets/css/dracula-ui.css
+-rw-r--r--   0 runner    (1001) docker     (123)   113611 2023-07-09 17:28:15.000000 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/assets/css/dracula-ui.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-07-09 17:28:15.000000 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/assets/css/mkdocs.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:28:28.872467 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/assets/img/
+-rw-r--r--   0 runner    (1001) docker     (123)   150941 2023-07-09 17:28:15.000000 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/assets/img/dracula.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11147 2023-07-09 17:28:15.000000 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/assets/img/dracula.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    25756 2023-07-09 17:28:15.000000 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/assets/img/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:28:28.872467 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    80599 2023-07-09 17:28:15.000000 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/assets/js/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   333974 2023-07-09 17:28:15.000000 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/assets/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    69916 2023-07-09 17:28:15.000000 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/assets/js/jquery-3.3.1.slim.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-09 17:28:15.000000 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/assets/js/mkdocs.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-09 17:28:15.000000 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-09 17:28:15.000000 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/main.html
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-09 17:28:15.000000 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/mkdocs_theme.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:28:28.872467 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-09 17:28:15.000000 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/modules/content.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-09 17:28:15.000000 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/modules/dropdown-menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-09 17:28:15.000000 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/modules/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-09 17:28:15.000000 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/modules/header.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-09 17:28:15.000000 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/modules/menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-09 17:28:15.000000 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/modules/preview.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-09 17:28:15.000000 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/modules/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-09 17:28:15.000000 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/modules/source.html
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-09 17:28:15.000000 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-09 17:28:15.000000 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/searchbox.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:28:28.868467 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-09 17:28:28.000000 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-09 17:28:28.000000 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 17:28:28.000000 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-09 17:28:28.000000 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-09 17:28:28.000000 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-09 17:28:28.000000 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 17:28:28.000000 mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 17:28:28.872467 mkdocs-dracula-theme-1.0.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-07-09 17:28:15.000000 mkdocs-dracula-theme-1.0.5/setup.py
```

### Comparing `mkdocs-dracula-theme-1.0.4/LICENSE` & `mkdocs-dracula-theme-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-dracula-theme-1.0.4/PKG-INFO` & `mkdocs-dracula-theme-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-dracula-theme
-Version: 1.0.4
+Version: 1.0.5
 Summary: 🧛🏻‍♂️ Dark theme for Mkdocs
 Home-page: https://github.com/dracula/mkdocs
 Author: Fernando Celmer
 Author-email: email@fernandocelmer.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mkdocs-dracula-theme-1.0.4/README.md` & `mkdocs-dracula-theme-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/__init__.py` & `mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0.4"
+__version__ = "1.0.5"
 
 __author__ = 'Fernando Celmer <email@fernandocelmer.com>'
 __copyright__ = """MIT License
 
 Copyright (c) 2023 Dracula Theme
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/__pycache__/__init__.cpython-310.pyc` & `mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Mar 26 00:41:22 2023 UTC, .py size: 1173 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-00000000: 6f0d 0d0a 0000 0000 b294 1f64 9504 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 2fee aa64 9504 0000  o......./..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0001 0000 0040 0000 0073 1000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 5a01 6402 5a02 6403 5300 2904  Z.d.Z.d.Z.d.S.).
-00000040: 7a05 312e 302e 347a 2a46 6572 6e61 6e64  z.1.0.4z*Fernand
+00000040: 7a05 312e 302e 357a 2a46 6572 6e61 6e64  z.1.0.5z*Fernand
 00000050: 6f20 4365 6c6d 6572 203c 656d 6169 6c40  o Celmer <email@
 00000060: 6665 726e 616e 646f 6365 6c6d 6572 2e63  fernandocelmer.c
 00000070: 6f6d 3e61 2d04 0000 4d49 5420 4c69 6365  om>a-...MIT Lice
 00000080: 6e73 650a 0a43 6f70 7972 6967 6874 2028  nse..Copyright (
 00000090: 6329 2032 3032 3320 4472 6163 756c 6120  c) 2023 Dracula 
 000000a0: 5468 656d 650a 0a50 6572 6d69 7373 696f  Theme..Permissio
 000000b0: 6e20 6973 2068 6572 6562 7920 6772 616e  n is hereby gran
```

### Comparing `mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/assets/css/bootstrap.min.css` & `mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/assets/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/assets/css/bootstrap.min.css.map` & `mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/assets/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/assets/css/dracula-ui.css` & `mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/assets/css/dracula-ui.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/assets/css/dracula-ui.css.map` & `mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/assets/css/dracula-ui.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/assets/css/mkdocs.css` & `mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/assets/css/mkdocs.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/assets/img/dracula.png` & `mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/assets/img/dracula.png`

 * *Files identical despite different names*

### Comparing `mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/assets/img/dracula.svg` & `mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/assets/img/dracula.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/assets/img/favicon.ico` & `mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/assets/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/assets/js/bootstrap.bundle.min.js` & `mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/assets/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/assets/js/bootstrap.bundle.min.js.map` & `mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/assets/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/assets/js/jquery-3.3.1.slim.min.js` & `mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/assets/js/jquery-3.3.1.slim.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/base.html` & `mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/base.html`

 * *Files identical despite different names*

### Comparing `mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/modules/dropdown-menu.html` & `mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/modules/dropdown-menu.html`

 * *Files identical despite different names*

### Comparing `mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/modules/header.html` & `mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/modules/header.html`

 * *Files identical despite different names*

### Comparing `mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/modules/menu.html` & `mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/modules/menu.html`

 * *Files identical despite different names*

### Comparing `mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/modules/preview.html` & `mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/modules/preview.html`

 * *Files identical despite different names*

### Comparing `mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/modules/sidebar.html` & `mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/modules/sidebar.html`

 * *Files identical despite different names*

### Comparing `mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/modules/source.html` & `mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/modules/source.html`

 * *Files identical despite different names*

### Comparing `mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme/search.html` & `mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme/search.html`

 * *Files identical despite different names*

### Comparing `mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme.egg-info/PKG-INFO` & `mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-dracula-theme
-Version: 1.0.4
+Version: 1.0.5
 Summary: 🧛🏻‍♂️ Dark theme for Mkdocs
 Home-page: https://github.com/dracula/mkdocs
 Author: Fernando Celmer
 Author-email: email@fernandocelmer.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mkdocs-dracula-theme-1.0.4/mkdocs_dracula_theme.egg-info/SOURCES.txt` & `mkdocs-dracula-theme-1.0.5/mkdocs_dracula_theme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-dracula-theme-1.0.4/setup.py` & `mkdocs-dracula-theme-1.0.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
     install_requires=[
-        'mkdocs>=1.4.2'
+        'mkdocs>=1.4.3'
     ],
     packages=["mkdocs_dracula_theme"],
     package_data={'mkdocs_dracula_theme': ['*','*/*','*/*/*']},
     include_package_data=True,
     python_requires=">=3.6",
     zip_safe=True,
     entry_points={
```

