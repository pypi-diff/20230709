# Comparing `tmp/djangoloco-0.1.tar.gz` & `tmp/djangoloco-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangoloco-0.1.tar", last modified: Sun Jul  9 08:43:29 2023, max compression
+gzip compressed data, was "djangoloco-1.0.tar", last modified: Sun Jul  9 08:57:41 2023, max compression
```

## Comparing `djangoloco-0.1.tar` & `djangoloco-1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 thisfro    (501) staff       (20)        0 2023-07-09 08:43:29.588743 djangoloco-0.1/
--rw-r--r--   0 thisfro    (501) staff       (20)     1494 2023-07-08 22:08:11.000000 djangoloco-0.1/LICENSE
--rw-r--r--   0 thisfro    (501) staff       (20)       64 2023-07-08 22:08:52.000000 djangoloco-0.1/MANIFEST.in
--rw-r--r--   0 thisfro    (501) staff       (20)     1759 2023-07-09 08:43:29.588851 djangoloco-0.1/PKG-INFO
--rw-r--r--   0 thisfro    (501) staff       (20)      721 2023-07-08 22:19:14.000000 djangoloco-0.1/README.md
-drwxr-xr-x   0 thisfro    (501) staff       (20)        0 2023-07-09 08:43:29.586046 djangoloco-0.1/djangoloco/
--rw-r--r--   0 thisfro    (501) staff       (20)        0 2023-07-08 21:27:20.000000 djangoloco-0.1/djangoloco/__init__.py
--rw-r--r--   0 thisfro    (501) staff       (20)       63 2023-07-08 21:27:20.000000 djangoloco-0.1/djangoloco/admin.py
--rw-r--r--   0 thisfro    (501) staff       (20)      152 2023-07-08 21:27:24.000000 djangoloco-0.1/djangoloco/apps.py
-drwxr-xr-x   0 thisfro    (501) staff       (20)        0 2023-07-09 08:43:29.581760 djangoloco-0.1/djangoloco/management/
-drwxr-xr-x   0 thisfro    (501) staff       (20)        0 2023-07-09 08:43:29.588249 djangoloco-0.1/djangoloco/management/commands/
--rw-r--r--   0 thisfro    (501) staff       (20)     2042 2023-07-08 21:39:11.000000 djangoloco-0.1/djangoloco/management/commands/loco.py
-drwxr-xr-x   0 thisfro    (501) staff       (20)        0 2023-07-09 08:43:29.588592 djangoloco-0.1/djangoloco/migrations/
--rw-r--r--   0 thisfro    (501) staff       (20)        0 2023-07-08 21:27:20.000000 djangoloco-0.1/djangoloco/migrations/__init__.py
--rw-r--r--   0 thisfro    (501) staff       (20)       57 2023-07-08 21:27:20.000000 djangoloco-0.1/djangoloco/models.py
--rw-r--r--   0 thisfro    (501) staff       (20)       60 2023-07-08 21:27:20.000000 djangoloco-0.1/djangoloco/tests.py
--rw-r--r--   0 thisfro    (501) staff       (20)       63 2023-07-08 21:27:20.000000 djangoloco-0.1/djangoloco/views.py
-drwxr-xr-x   0 thisfro    (501) staff       (20)        0 2023-07-09 08:43:29.588062 djangoloco-0.1/djangoloco.egg-info/
--rw-r--r--   0 thisfro    (501) staff       (20)     1759 2023-07-09 08:43:29.000000 djangoloco-0.1/djangoloco.egg-info/PKG-INFO
--rw-r--r--   0 thisfro    (501) staff       (20)      428 2023-07-09 08:43:29.000000 djangoloco-0.1/djangoloco.egg-info/SOURCES.txt
--rw-r--r--   0 thisfro    (501) staff       (20)        1 2023-07-09 08:43:29.000000 djangoloco-0.1/djangoloco.egg-info/dependency_links.txt
--rw-r--r--   0 thisfro    (501) staff       (20)       12 2023-07-09 08:43:29.000000 djangoloco-0.1/djangoloco.egg-info/requires.txt
--rw-r--r--   0 thisfro    (501) staff       (20)       11 2023-07-09 08:43:29.000000 djangoloco-0.1/djangoloco.egg-info/top_level.txt
--rw-r--r--   0 thisfro    (501) staff       (20)       88 2023-07-08 21:42:28.000000 djangoloco-0.1/pyproject.toml
--rw-r--r--   0 thisfro    (501) staff       (20)     1041 2023-07-09 08:43:29.589200 djangoloco-0.1/setup.cfg
--rw-r--r--   0 thisfro    (501) staff       (20)       38 2023-07-09 08:41:28.000000 djangoloco-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:57:41.380066 djangoloco-1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-09 08:57:29.000000 djangoloco-1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-09 08:57:29.000000 djangoloco-1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-09 08:57:41.380066 djangoloco-1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-09 08:57:29.000000 djangoloco-1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:57:41.376066 djangoloco-1.0/djangoloco/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 08:57:29.000000 djangoloco-1.0/djangoloco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-09 08:57:29.000000 djangoloco-1.0/djangoloco/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-09 08:57:29.000000 djangoloco-1.0/djangoloco/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:57:41.376066 djangoloco-1.0/djangoloco/management/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:57:41.380066 djangoloco-1.0/djangoloco/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-09 08:57:29.000000 djangoloco-1.0/djangoloco/management/commands/loco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:57:41.380066 djangoloco-1.0/djangoloco/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 08:57:29.000000 djangoloco-1.0/djangoloco/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-09 08:57:29.000000 djangoloco-1.0/djangoloco/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-09 08:57:29.000000 djangoloco-1.0/djangoloco/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-09 08:57:29.000000 djangoloco-1.0/djangoloco/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:57:41.380066 djangoloco-1.0/djangoloco.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-09 08:57:41.000000 djangoloco-1.0/djangoloco.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-09 08:57:41.000000 djangoloco-1.0/djangoloco.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 08:57:41.000000 djangoloco-1.0/djangoloco.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-09 08:57:41.000000 djangoloco-1.0/djangoloco.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-09 08:57:41.000000 djangoloco-1.0/djangoloco.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-09 08:57:29.000000 djangoloco-1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-09 08:57:41.380066 djangoloco-1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 08:57:29.000000 djangoloco-1.0/setup.py
```

### Comparing `djangoloco-0.1/LICENSE` & `djangoloco-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `djangoloco-0.1/PKG-INFO` & `djangoloco-1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangoloco
-Version: 0.1
+Version: 1.0
 Summary: A simple management command to get translations from localise.biz (Loco) for your django app.
 Home-page: https://github.com/thisfro/djangoloco
 Author: Jannis Portmann
 Author-email: jannis@thisfro.ch
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `djangoloco-0.1/README.md` & `djangoloco-1.0/README.md`

 * *Files identical despite different names*

### Comparing `djangoloco-0.1/djangoloco/management/commands/loco.py` & `djangoloco-1.0/djangoloco/management/commands/loco.py`

 * *Files identical despite different names*

### Comparing `djangoloco-0.1/djangoloco.egg-info/PKG-INFO` & `djangoloco-1.0/djangoloco.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangoloco
-Version: 0.1
+Version: 1.0
 Summary: A simple management command to get translations from localise.biz (Loco) for your django app.
 Home-page: https://github.com/thisfro/djangoloco
 Author: Jannis Portmann
 Author-email: jannis@thisfro.ch
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `djangoloco-0.1/setup.cfg` & `djangoloco-1.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = djangoloco
-version = 0.1
+version = 1.0
 description = A simple management command to get translations from localise.biz (Loco) for your django app.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/thisfro/djangoloco
 author = Jannis Portmann
 author_email = jannis@thisfro.ch
 license = BSD-3-Clause
```

