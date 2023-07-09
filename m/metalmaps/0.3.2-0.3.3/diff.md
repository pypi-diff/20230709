# Comparing `tmp/metalmaps-0.3.2.tar.gz` & `tmp/metalmaps-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metalmaps-0.3.2.tar", last modified: Sun Jul  9 18:10:33 2023, max compression
+gzip compressed data, was "metalmaps-0.3.3.tar", last modified: Sun Jul  9 18:27:28 2023, max compression
```

## Comparing `metalmaps-0.3.2.tar` & `metalmaps-0.3.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2023-07-09 18:10:33.824156 metalmaps-0.3.2/
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     7651 2023-07-08 09:30:26.000000 metalmaps-0.3.2/LICENSE.txt
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)       55 2023-07-09 18:10:20.000000 metalmaps-0.3.2/MANIFEST.in
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)    13489 2023-07-09 18:10:33.824156 metalmaps-0.3.2/PKG-INFO
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     3871 2023-07-09 16:41:51.000000 metalmaps-0.3.2/README.md
-drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2023-07-09 18:10:33.820155 metalmaps-0.3.2/metalmaps/
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     2177 2023-07-09 12:43:23.000000 metalmaps-0.3.2/metalmaps/__init__.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)       22 2023-07-09 18:10:02.000000 metalmaps-0.3.2/metalmaps/__version__.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     3379 2023-07-09 16:17:38.000000 metalmaps-0.3.2/metalmaps/colors.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     2073 2023-07-09 12:43:23.000000 metalmaps-0.3.2/metalmaps/make_cmap.py
-drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2023-07-09 18:10:33.824156 metalmaps-0.3.2/metalmaps.egg-info/
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)    13489 2023-07-09 18:10:33.000000 metalmaps-0.3.2/metalmaps.egg-info/PKG-INFO
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      302 2023-07-09 18:10:33.000000 metalmaps-0.3.2/metalmaps.egg-info/SOURCES.txt
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)        1 2023-07-09 18:10:33.000000 metalmaps-0.3.2/metalmaps.egg-info/dependency_links.txt
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)       11 2023-07-09 18:10:33.000000 metalmaps-0.3.2/metalmaps.egg-info/requires.txt
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)       10 2023-07-09 18:10:33.000000 metalmaps-0.3.2/metalmaps.egg-info/top_level.txt
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     1199 2023-07-09 18:10:02.000000 metalmaps-0.3.2/pyproject.toml
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)       38 2023-07-09 18:10:33.824156 metalmaps-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:27:28.942510 metalmaps-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-07-09 18:27:16.000000 metalmaps-0.3.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-09 18:27:16.000000 metalmaps-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13496 2023-07-09 18:27:28.942510 metalmaps-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-07-09 18:27:16.000000 metalmaps-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:27:28.938510 metalmaps-0.3.3/metalmaps/
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-09 18:27:16.000000 metalmaps-0.3.3/metalmaps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-09 18:27:16.000000 metalmaps-0.3.3/metalmaps/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-09 18:27:16.000000 metalmaps-0.3.3/metalmaps/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-09 18:27:16.000000 metalmaps-0.3.3/metalmaps/make_cmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:27:28.942510 metalmaps-0.3.3/metalmaps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13496 2023-07-09 18:27:28.000000 metalmaps-0.3.3/metalmaps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-09 18:27:28.000000 metalmaps-0.3.3/metalmaps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 18:27:28.000000 metalmaps-0.3.3/metalmaps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-09 18:27:28.000000 metalmaps-0.3.3/metalmaps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-09 18:27:28.000000 metalmaps-0.3.3/metalmaps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-09 18:27:16.000000 metalmaps-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 18:27:28.942510 metalmaps-0.3.3/setup.cfg
```

### Comparing `metalmaps-0.3.2/LICENSE.txt` & `metalmaps-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `metalmaps-0.3.2/PKG-INFO` & `metalmaps-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalmaps
-Version: 0.3.2
+Version: 0.3.3
 Summary: Metal and rock inspired Matplotlib colormaps.
 Author-email: Mladen Ivkovic <mladen.ivkovic@hotmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -164,15 +164,15 @@
         General Public License ever published by the Free Software Foundation.
         
           If the Library as you received it specifies that a proxy can decide
         whether future versions of the GNU Lesser General Public License shall
         apply, that proxy's public statement of acceptance of any version is
         permanent authorization for you to choose that version for the
         Library.
-Project-URL: Homepage, https://github.com/mivkov/metalmaps
+Project-URL: Homepage, https://github.com/mladenivkovic/metalmaps
 Project-URL: Gallery, https://mladenivkovic.github.io/metalmaps/metalmaps.html
 Keywords: metal,rock,colormap,matplotlib
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `metalmaps-0.3.2/README.md` & `metalmaps-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `metalmaps-0.3.2/metalmaps/__init__.py` & `metalmaps-0.3.3/metalmaps/__init__.py`

 * *Files identical despite different names*

### Comparing `metalmaps-0.3.2/metalmaps/colors.py` & `metalmaps-0.3.3/metalmaps/colors.py`

 * *Files identical despite different names*

### Comparing `metalmaps-0.3.2/metalmaps/make_cmap.py` & `metalmaps-0.3.3/metalmaps/make_cmap.py`

 * *Files identical despite different names*

### Comparing `metalmaps-0.3.2/metalmaps.egg-info/PKG-INFO` & `metalmaps-0.3.3/metalmaps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalmaps
-Version: 0.3.2
+Version: 0.3.3
 Summary: Metal and rock inspired Matplotlib colormaps.
 Author-email: Mladen Ivkovic <mladen.ivkovic@hotmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -164,15 +164,15 @@
         General Public License ever published by the Free Software Foundation.
         
           If the Library as you received it specifies that a proxy can decide
         whether future versions of the GNU Lesser General Public License shall
         apply, that proxy's public statement of acceptance of any version is
         permanent authorization for you to choose that version for the
         Library.
-Project-URL: Homepage, https://github.com/mivkov/metalmaps
+Project-URL: Homepage, https://github.com/mladenivkovic/metalmaps
 Project-URL: Gallery, https://mladenivkovic.github.io/metalmaps/metalmaps.html
 Keywords: metal,rock,colormap,matplotlib
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `metalmaps-0.3.2/pyproject.toml` & `metalmaps-0.3.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.setuptools]
 packages = ["metalmaps"]
 
 [project]
 name = "metalmaps"
 description="Metal and rock inspired Matplotlib colormaps."
 readme = "README.md"
-version = "0.3.2"
+version = "0.3.3"
 authors= [
     { name = "Mladen Ivkovic", email="mladen.ivkovic@hotmail.com"},
     ]
 license = { file = "LICENSE.txt" }
 classifiers=[
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -21,19 +21,19 @@
     "Operating System :: OS Independent"
 ]
 keywords = [ "metal", "rock", "colormap", "matplotlib" ]
 dependencies=[ "matplotlib" ]
 
 
 [project.urls]
-"Homepage" = "https://github.com/mivkov/metalmaps"
+"Homepage" = "https://github.com/mladenivkovic/metalmaps"
 "Gallery" = "https://mladenivkovic.github.io/metalmaps/metalmaps.html"
 
 [tool.bumpver]
-current_version = "0.3.2"
+current_version = "0.3.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

