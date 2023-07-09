# Comparing `tmp/yadoma-59.0.tar.gz` & `tmp/yadoma-59.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yadoma-59.0.tar", last modified: Sun Jul  9 20:26:02 2023, max compression
+gzip compressed data, was "yadoma-59.0.post1.tar", last modified: Sun Jul  9 20:44:55 2023, max compression
```

## Comparing `yadoma-59.0.tar` & `yadoma-59.0.post1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ingo      (1000) ingo      (1001)        0 2023-07-09 20:26:02.967034 yadoma-59.0/
--rw-rw-r--   0 ingo      (1000) ingo      (1001)    11358 2022-07-28 09:11:39.000000 yadoma-59.0/LICENSE
--rw-rw-r--   0 ingo      (1000) ingo      (1001)     2579 2023-07-09 20:26:02.967034 yadoma-59.0/PKG-INFO
--rw-rw-r--   0 ingo      (1000) ingo      (1001)     2294 2023-07-09 20:14:26.000000 yadoma-59.0/README.rst
--rw-rw-r--   0 ingo      (1000) ingo      (1001)      137 2023-07-08 22:55:04.000000 yadoma-59.0/pyproject.toml
--rw-rw-r--   0 ingo      (1000) ingo      (1001)      559 2023-07-09 20:26:02.967034 yadoma-59.0/setup.cfg
--rw-rw-r--   0 ingo      (1000) ingo      (1001)       91 2023-07-08 21:17:22.000000 yadoma-59.0/setup.py
-drwxrwxr-x   0 ingo      (1000) ingo      (1001)        0 2023-07-09 20:26:02.963034 yadoma-59.0/src/
-drwxrwxr-x   0 ingo      (1000) ingo      (1001)        0 2023-07-09 20:26:02.963034 yadoma-59.0/src/main/
-drwxrwxr-x   0 ingo      (1000) ingo      (1001)        0 2023-07-09 20:26:02.963034 yadoma-59.0/src/main/python/
-drwxrwxr-x   0 ingo      (1000) ingo      (1001)        0 2023-07-09 20:26:02.963034 yadoma-59.0/src/main/python/yadoma/
--rw-rw-r--   0 ingo      (1000) ingo      (1001)       27 2023-07-08 22:55:04.000000 yadoma-59.0/src/main/python/yadoma/__init__.py
--rw-rw-r--   0 ingo      (1000) ingo      (1001)     3882 2023-07-08 21:37:43.000000 yadoma-59.0/src/main/python/yadoma/main.py
-drwxrwxr-x   0 ingo      (1000) ingo      (1001)        0 2023-07-09 20:26:02.967034 yadoma-59.0/src/main/python/yadoma.egg-info/
--rw-rw-r--   0 ingo      (1000) ingo      (1001)     2579 2023-07-09 20:26:02.000000 yadoma-59.0/src/main/python/yadoma.egg-info/PKG-INFO
--rw-rw-r--   0 ingo      (1000) ingo      (1001)      396 2023-07-09 20:26:02.000000 yadoma-59.0/src/main/python/yadoma.egg-info/SOURCES.txt
--rw-rw-r--   0 ingo      (1000) ingo      (1001)        1 2023-07-09 20:26:02.000000 yadoma-59.0/src/main/python/yadoma.egg-info/dependency_links.txt
--rw-rw-r--   0 ingo      (1000) ingo      (1001)       44 2023-07-09 20:26:02.000000 yadoma-59.0/src/main/python/yadoma.egg-info/entry_points.txt
--rw-rw-r--   0 ingo      (1000) ingo      (1001)       14 2023-07-09 20:26:02.000000 yadoma-59.0/src/main/python/yadoma.egg-info/requires.txt
--rw-rw-r--   0 ingo      (1000) ingo      (1001)        7 2023-07-09 20:26:02.000000 yadoma-59.0/src/main/python/yadoma.egg-info/top_level.txt
+drwxrwxr-x   0 ingo      (1000) ingo      (1001)        0 2023-07-09 20:44:55.750514 yadoma-59.0.post1/
+-rw-rw-r--   0 ingo      (1000) ingo      (1001)    11358 2022-07-28 09:11:39.000000 yadoma-59.0.post1/LICENSE
+-rw-rw-r--   0 ingo      (1000) ingo      (1001)     2774 2023-07-09 20:44:55.750514 yadoma-59.0.post1/PKG-INFO
+-rw-rw-r--   0 ingo      (1000) ingo      (1001)     2483 2023-07-09 20:39:39.000000 yadoma-59.0.post1/README.rst
+-rw-rw-r--   0 ingo      (1000) ingo      (1001)      137 2023-07-08 22:55:04.000000 yadoma-59.0.post1/pyproject.toml
+-rw-rw-r--   0 ingo      (1000) ingo      (1001)      565 2023-07-09 20:44:55.750514 yadoma-59.0.post1/setup.cfg
+-rw-rw-r--   0 ingo      (1000) ingo      (1001)       91 2023-07-08 21:17:22.000000 yadoma-59.0.post1/setup.py
+drwxrwxr-x   0 ingo      (1000) ingo      (1001)        0 2023-07-09 20:44:55.746514 yadoma-59.0.post1/src/
+drwxrwxr-x   0 ingo      (1000) ingo      (1001)        0 2023-07-09 20:44:55.746514 yadoma-59.0.post1/src/main/
+drwxrwxr-x   0 ingo      (1000) ingo      (1001)        0 2023-07-09 20:44:55.746514 yadoma-59.0.post1/src/main/python/
+drwxrwxr-x   0 ingo      (1000) ingo      (1001)        0 2023-07-09 20:44:55.750514 yadoma-59.0.post1/src/main/python/yadoma/
+-rw-rw-r--   0 ingo      (1000) ingo      (1001)       27 2023-07-08 22:55:04.000000 yadoma-59.0.post1/src/main/python/yadoma/__init__.py
+-rw-rw-r--   0 ingo      (1000) ingo      (1001)     3882 2023-07-08 21:37:43.000000 yadoma-59.0.post1/src/main/python/yadoma/main.py
+drwxrwxr-x   0 ingo      (1000) ingo      (1001)        0 2023-07-09 20:44:55.750514 yadoma-59.0.post1/src/main/python/yadoma.egg-info/
+-rw-rw-r--   0 ingo      (1000) ingo      (1001)     2774 2023-07-09 20:44:55.000000 yadoma-59.0.post1/src/main/python/yadoma.egg-info/PKG-INFO
+-rw-rw-r--   0 ingo      (1000) ingo      (1001)      396 2023-07-09 20:44:55.000000 yadoma-59.0.post1/src/main/python/yadoma.egg-info/SOURCES.txt
+-rw-rw-r--   0 ingo      (1000) ingo      (1001)        1 2023-07-09 20:44:55.000000 yadoma-59.0.post1/src/main/python/yadoma.egg-info/dependency_links.txt
+-rw-rw-r--   0 ingo      (1000) ingo      (1001)       44 2023-07-09 20:44:55.000000 yadoma-59.0.post1/src/main/python/yadoma.egg-info/entry_points.txt
+-rw-rw-r--   0 ingo      (1000) ingo      (1001)       14 2023-07-09 20:44:55.000000 yadoma-59.0.post1/src/main/python/yadoma.egg-info/requires.txt
+-rw-rw-r--   0 ingo      (1000) ingo      (1001)        7 2023-07-09 20:44:55.000000 yadoma-59.0.post1/src/main/python/yadoma.egg-info/top_level.txt
```

### Comparing `yadoma-59.0/LICENSE` & `yadoma-59.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `yadoma-59.0/PKG-INFO` & `yadoma-59.0.post1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: yadoma
-Version: 59.0
+Version: 59.0.post1
 Summary: Yet another dotfile manager
 Author: N.V. Haenel & Ingo Fruend
 Author-email: github@ingofruend.net
 License: APACHE v2.0
 Keywords: dotfiles,config management
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 Edit 2023: yadoma was written by @esc a couple of years ago and ended up no
 longer maintained. It seemed that I was the only user, so I'm taking over
 maintenance. However, given the simplicity of the tool, I kept everything
 largely the same, including this README. Hence, "I" refers to @esc rather than
-myself.
+myself. However, I'm changing the build process to tox (instead of the old
+pybuilder), because pybuilder seemed to have problems with environment
+separation that I wasn't able to just quickly fix.
 
 ===================================
 yadoma: yet another dotfile manager
 ===================================
 
 This is my personal take on a dotfile-manager.
```

### Comparing `yadoma-59.0/README.rst` & `yadoma-59.0.post1/src/main/python/yadoma.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,25 @@
+Metadata-Version: 2.1
+Name: yadoma
+Version: 59.0.post1
+Summary: Yet another dotfile manager
+Author: N.V. Haenel & Ingo Fruend
+Author-email: github@ingofruend.net
+License: APACHE v2.0
+Keywords: dotfiles,config management
+Classifier: Programming Language :: Python :: 3
+License-File: LICENSE
+
 Edit 2023: yadoma was written by @esc a couple of years ago and ended up no
 longer maintained. It seemed that I was the only user, so I'm taking over
 maintenance. However, given the simplicity of the tool, I kept everything
 largely the same, including this README. Hence, "I" refers to @esc rather than
-myself.
+myself. However, I'm changing the build process to tox (instead of the old
+pybuilder), because pybuilder seemed to have problems with environment
+separation that I wasn't able to just quickly fix.
 
 ===================================
 yadoma: yet another dotfile manager
 ===================================
 
 This is my personal take on a dotfile-manager.
```

### Comparing `yadoma-59.0/setup.cfg` & `yadoma-59.0.post1/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = yadoma
-version = 59.0
+version = 59.0.post1
 author = N.V. Haenel & Ingo Fruend
 author_email = github@ingofruend.net
 description = Yet another dotfile manager
 long_description = file: README.rst
 keywords = dotfiles, config management
 license = APACHE v2.0
 classifiers =
```

### Comparing `yadoma-59.0/src/main/python/yadoma/main.py` & `yadoma-59.0.post1/src/main/python/yadoma/main.py`

 * *Files identical despite different names*

### Comparing `yadoma-59.0/src/main/python/yadoma.egg-info/PKG-INFO` & `yadoma-59.0.post1/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,14 @@
-Metadata-Version: 2.1
-Name: yadoma
-Version: 59.0
-Summary: Yet another dotfile manager
-Author: N.V. Haenel & Ingo Fruend
-Author-email: github@ingofruend.net
-License: APACHE v2.0
-Keywords: dotfiles,config management
-Classifier: Programming Language :: Python :: 3
-License-File: LICENSE
-
 Edit 2023: yadoma was written by @esc a couple of years ago and ended up no
 longer maintained. It seemed that I was the only user, so I'm taking over
 maintenance. However, given the simplicity of the tool, I kept everything
 largely the same, including this README. Hence, "I" refers to @esc rather than
-myself.
+myself. However, I'm changing the build process to tox (instead of the old
+pybuilder), because pybuilder seemed to have problems with environment
+separation that I wasn't able to just quickly fix.
 
 ===================================
 yadoma: yet another dotfile manager
 ===================================
 
 This is my personal take on a dotfile-manager.
```

