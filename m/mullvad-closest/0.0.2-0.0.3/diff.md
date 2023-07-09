# Comparing `tmp/mullvad-closest-0.0.2.tar.gz` & `tmp/mullvad-closest-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mullvad-closest-0.0.2.tar", last modified: Sun Jul  9 20:25:11 2023, max compression
+gzip compressed data, was "mullvad-closest-0.0.3.tar", last modified: Sun Jul  9 20:28:21 2023, max compression
```

## Comparing `mullvad-closest-0.0.2.tar` & `mullvad-closest-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 ay        (1000) ay        (1000)        0 2023-07-09 20:25:11.655424 mullvad-closest-0.0.2/
--rw-rw-r--   0 ay        (1000) ay        (1000)     1211 2023-07-09 19:45:01.000000 mullvad-closest-0.0.2/LICENSE
--rw-rw-r--   0 ay        (1000) ay        (1000)       17 2023-07-09 20:22:15.000000 mullvad-closest-0.0.2/MANIFEST.in
--rw-rw-r--   0 ay        (1000) ay        (1000)     3877 2023-07-09 20:25:11.655424 mullvad-closest-0.0.2/PKG-INFO
--rw-rw-r--   0 ay        (1000) ay        (1000)     3565 2023-07-09 20:23:50.000000 mullvad-closest-0.0.2/README.md
-drwxrwxr-x   0 ay        (1000) ay        (1000)        0 2023-07-09 20:25:11.655424 mullvad-closest-0.0.2/mullvad_closest/
--rw-rw-r--   0 ay        (1000) ay        (1000)       22 2023-07-09 20:24:35.000000 mullvad-closest-0.0.2/mullvad_closest/__init__.py
--rw-rw-r--   0 ay        (1000) ay        (1000)     1437 2023-07-09 19:45:01.000000 mullvad-closest-0.0.2/mullvad_closest/cli.py
--rw-rw-r--   0 ay        (1000) ay        (1000)     5160 2023-07-09 19:45:01.000000 mullvad-closest-0.0.2/mullvad_closest/utils.py
-drwxrwxr-x   0 ay        (1000) ay        (1000)        0 2023-07-09 20:25:11.655424 mullvad-closest-0.0.2/mullvad_closest.egg-info/
--rw-rw-r--   0 ay        (1000) ay        (1000)     3877 2023-07-09 20:25:11.000000 mullvad-closest-0.0.2/mullvad_closest.egg-info/PKG-INFO
--rw-rw-r--   0 ay        (1000) ay        (1000)      365 2023-07-09 20:25:11.000000 mullvad-closest-0.0.2/mullvad_closest.egg-info/SOURCES.txt
--rw-rw-r--   0 ay        (1000) ay        (1000)        1 2023-07-09 20:25:11.000000 mullvad-closest-0.0.2/mullvad_closest.egg-info/dependency_links.txt
--rw-rw-r--   0 ay        (1000) ay        (1000)       61 2023-07-09 20:25:11.000000 mullvad-closest-0.0.2/mullvad_closest.egg-info/entry_points.txt
--rw-rw-r--   0 ay        (1000) ay        (1000)       36 2023-07-09 20:25:11.000000 mullvad-closest-0.0.2/mullvad_closest.egg-info/requires.txt
--rw-rw-r--   0 ay        (1000) ay        (1000)       16 2023-07-09 20:25:11.000000 mullvad-closest-0.0.2/mullvad_closest.egg-info/top_level.txt
--rw-rw-r--   0 ay        (1000) ay        (1000)      582 2023-07-09 19:45:01.000000 mullvad-closest-0.0.2/pyproject.toml
--rw-rw-r--   0 ay        (1000) ay        (1000)       38 2023-07-09 20:25:11.655424 mullvad-closest-0.0.2/setup.cfg
--rw-rw-r--   0 ay        (1000) ay        (1000)      866 2023-07-09 19:45:01.000000 mullvad-closest-0.0.2/setup.py
+drwxrwxr-x   0 ay        (1000) ay        (1000)        0 2023-07-09 20:28:21.318765 mullvad-closest-0.0.3/
+-rw-rw-r--   0 ay        (1000) ay        (1000)     1211 2023-07-09 19:45:01.000000 mullvad-closest-0.0.3/LICENSE
+-rw-rw-r--   0 ay        (1000) ay        (1000)       25 2023-07-09 20:28:04.000000 mullvad-closest-0.0.3/MANIFEST.in
+-rw-rw-r--   0 ay        (1000) ay        (1000)     3877 2023-07-09 20:28:21.318765 mullvad-closest-0.0.3/PKG-INFO
+-rw-rw-r--   0 ay        (1000) ay        (1000)     3565 2023-07-09 20:23:50.000000 mullvad-closest-0.0.3/README.md
+drwxrwxr-x   0 ay        (1000) ay        (1000)        0 2023-07-09 20:28:21.318765 mullvad-closest-0.0.3/mullvad_closest/
+-rw-rw-r--   0 ay        (1000) ay        (1000)       22 2023-07-09 20:28:13.000000 mullvad-closest-0.0.3/mullvad_closest/__init__.py
+-rw-rw-r--   0 ay        (1000) ay        (1000)     1437 2023-07-09 19:45:01.000000 mullvad-closest-0.0.3/mullvad_closest/cli.py
+-rw-rw-r--   0 ay        (1000) ay        (1000)     5160 2023-07-09 19:45:01.000000 mullvad-closest-0.0.3/mullvad_closest/utils.py
+drwxrwxr-x   0 ay        (1000) ay        (1000)        0 2023-07-09 20:28:21.318765 mullvad-closest-0.0.3/mullvad_closest.egg-info/
+-rw-rw-r--   0 ay        (1000) ay        (1000)     3877 2023-07-09 20:28:21.000000 mullvad-closest-0.0.3/mullvad_closest.egg-info/PKG-INFO
+-rw-rw-r--   0 ay        (1000) ay        (1000)      382 2023-07-09 20:28:21.000000 mullvad-closest-0.0.3/mullvad_closest.egg-info/SOURCES.txt
+-rw-rw-r--   0 ay        (1000) ay        (1000)        1 2023-07-09 20:28:21.000000 mullvad-closest-0.0.3/mullvad_closest.egg-info/dependency_links.txt
+-rw-rw-r--   0 ay        (1000) ay        (1000)       61 2023-07-09 20:28:21.000000 mullvad-closest-0.0.3/mullvad_closest.egg-info/entry_points.txt
+-rw-rw-r--   0 ay        (1000) ay        (1000)       36 2023-07-09 20:28:21.000000 mullvad-closest-0.0.3/mullvad_closest.egg-info/requires.txt
+-rw-rw-r--   0 ay        (1000) ay        (1000)       16 2023-07-09 20:28:21.000000 mullvad-closest-0.0.3/mullvad_closest.egg-info/top_level.txt
+-rw-rw-r--   0 ay        (1000) ay        (1000)      582 2023-07-09 19:45:01.000000 mullvad-closest-0.0.3/pyproject.toml
+-rw-rw-r--   0 ay        (1000) ay        (1000)       36 2023-07-09 19:45:01.000000 mullvad-closest-0.0.3/requirements.txt
+-rw-rw-r--   0 ay        (1000) ay        (1000)       38 2023-07-09 20:28:21.318765 mullvad-closest-0.0.3/setup.cfg
+-rw-rw-r--   0 ay        (1000) ay        (1000)      866 2023-07-09 19:45:01.000000 mullvad-closest-0.0.3/setup.py
```

### Comparing `mullvad-closest-0.0.2/LICENSE` & `mullvad-closest-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mullvad-closest-0.0.2/PKG-INFO` & `mullvad-closest-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mullvad-closest
-Version: 0.0.2
+Version: 0.0.3
 Summary: Find Mullvad servers with the lowest latency at your location
 Home-page: https://github.com/Ch00k/mullvad-closest
 Author: Andrii Yurchuk
 Author-email: ay@mntw.re
 License: Unlicense
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mullvad-closest-0.0.2/README.md` & `mullvad-closest-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mullvad-closest-0.0.2/mullvad_closest/cli.py` & `mullvad-closest-0.0.3/mullvad_closest/cli.py`

 * *Files identical despite different names*

### Comparing `mullvad-closest-0.0.2/mullvad_closest/utils.py` & `mullvad-closest-0.0.3/mullvad_closest/utils.py`

 * *Files identical despite different names*

### Comparing `mullvad-closest-0.0.2/mullvad_closest.egg-info/PKG-INFO` & `mullvad-closest-0.0.3/mullvad_closest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mullvad-closest
-Version: 0.0.2
+Version: 0.0.3
 Summary: Find Mullvad servers with the lowest latency at your location
 Home-page: https://github.com/Ch00k/mullvad-closest
 Author: Andrii Yurchuk
 Author-email: ay@mntw.re
 License: Unlicense
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mullvad-closest-0.0.2/pyproject.toml` & `mullvad-closest-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mullvad-closest-0.0.2/setup.py` & `mullvad-closest-0.0.3/setup.py`

 * *Files identical despite different names*

