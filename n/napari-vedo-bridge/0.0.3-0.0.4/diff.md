# Comparing `tmp/napari-vedo-bridge-0.0.3.tar.gz` & `tmp/napari-vedo-bridge-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-vedo-bridge-0.0.3.tar", last modified: Tue Jul  4 07:24:39 2023, max compression
+gzip compressed data, was "napari-vedo-bridge-0.0.4.tar", last modified: Sun Jul  9 20:34:16 2023, max compression
```

## Comparing `napari-vedo-bridge-0.0.3.tar` & `napari-vedo-bridge-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:24:39.165400 napari-vedo-bridge-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-04 07:24:22.000000 napari-vedo-bridge-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-04 07:24:22.000000 napari-vedo-bridge-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-04 07:24:39.165400 napari-vedo-bridge-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-04 07:24:22.000000 napari-vedo-bridge-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-04 07:24:22.000000 napari-vedo-bridge-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-04 07:24:39.169400 napari-vedo-bridge-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:24:39.165400 napari-vedo-bridge-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:24:39.165400 napari-vedo-bridge-0.0.3/src/napari_vedo_bridge/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-04 07:24:22.000000 napari-vedo-bridge-0.0.3/src/napari_vedo_bridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-07-04 07:24:22.000000 napari-vedo-bridge-0.0.3/src/napari_vedo_bridge/_cutter_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:24:39.165400 napari-vedo-bridge-0.0.3/src/napari_vedo_bridge/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 07:24:22.000000 napari-vedo-bridge-0.0.3/src/napari_vedo_bridge/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-04 07:24:22.000000 napari-vedo-bridge-0.0.3/src/napari_vedo_bridge/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-04 07:24:22.000000 napari-vedo-bridge-0.0.3/src/napari_vedo_bridge/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-07-04 07:24:22.000000 napari-vedo-bridge-0.0.3/src/napari_vedo_bridge/vedo_extension.ui
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:24:39.165400 napari-vedo-bridge-0.0.3/src/napari_vedo_bridge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-04 07:24:39.000000 napari-vedo-bridge-0.0.3/src/napari_vedo_bridge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-04 07:24:39.000000 napari-vedo-bridge-0.0.3/src/napari_vedo_bridge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 07:24:39.000000 napari-vedo-bridge-0.0.3/src/napari_vedo_bridge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-04 07:24:39.000000 napari-vedo-bridge-0.0.3/src/napari_vedo_bridge.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-04 07:24:39.000000 napari-vedo-bridge-0.0.3/src/napari_vedo_bridge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 07:24:39.000000 napari-vedo-bridge-0.0.3/src/napari_vedo_bridge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:34:16.667851 napari-vedo-bridge-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-09 20:33:59.000000 napari-vedo-bridge-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-09 20:33:59.000000 napari-vedo-bridge-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-07-09 20:34:16.667851 napari-vedo-bridge-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-09 20:33:59.000000 napari-vedo-bridge-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-09 20:33:59.000000 napari-vedo-bridge-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-09 20:34:16.667851 napari-vedo-bridge-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:34:16.663850 napari-vedo-bridge-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:34:16.667851 napari-vedo-bridge-0.0.4/src/napari_vedo_bridge/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-09 20:33:59.000000 napari-vedo-bridge-0.0.4/src/napari_vedo_bridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-07-09 20:33:59.000000 napari-vedo-bridge-0.0.4/src/napari_vedo_bridge/_cutter_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:34:16.667851 napari-vedo-bridge-0.0.4/src/napari_vedo_bridge/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 20:33:59.000000 napari-vedo-bridge-0.0.4/src/napari_vedo_bridge/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-09 20:33:59.000000 napari-vedo-bridge-0.0.4/src/napari_vedo_bridge/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-09 20:33:59.000000 napari-vedo-bridge-0.0.4/src/napari_vedo_bridge/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-07-09 20:33:59.000000 napari-vedo-bridge-0.0.4/src/napari_vedo_bridge/vedo_extension.ui
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:34:16.667851 napari-vedo-bridge-0.0.4/src/napari_vedo_bridge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-07-09 20:34:16.000000 napari-vedo-bridge-0.0.4/src/napari_vedo_bridge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-09 20:34:16.000000 napari-vedo-bridge-0.0.4/src/napari_vedo_bridge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 20:34:16.000000 napari-vedo-bridge-0.0.4/src/napari_vedo_bridge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-09 20:34:16.000000 napari-vedo-bridge-0.0.4/src/napari_vedo_bridge.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-09 20:34:16.000000 napari-vedo-bridge-0.0.4/src/napari_vedo_bridge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-09 20:34:16.000000 napari-vedo-bridge-0.0.4/src/napari_vedo_bridge.egg-info/top_level.txt
```

### Comparing `napari-vedo-bridge-0.0.3/LICENSE` & `napari-vedo-bridge-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-vedo-bridge-0.0.3/PKG-INFO` & `napari-vedo-bridge-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 Metadata-Version: 2.1
 Name: napari-vedo-bridge
-Version: 0.0.3
+Version: 0.0.4
 Summary: Transfer mesh data between napari and vedo for interactive processing
 Author: Johannes Soltwedel, Marco Musy
 Author-email: johannes_richard.soltwedel@tu-dresden.de
 License: BSD-3-Clause
+Project-URL: Bug Tracker, https://github.com/jo-mueller/napari-vedo-bridge/issues
+Project-URL: Documentation, https://github.com/jo-mueller/napari-vedo-bridge#README.md
+Project-URL: Source Code, https://github.com/jo-mueller/napari-vedo-bridge
+Project-URL: User Support, https://github.com/jo-mueller/napari-vedo-bridge/issues
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `napari-vedo-bridge-0.0.3/README.md` & `napari-vedo-bridge-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `napari-vedo-bridge-0.0.3/pyproject.toml` & `napari-vedo-bridge-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari-vedo-bridge-0.0.3/setup.cfg` & `napari-vedo-bridge-0.0.4/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -17,14 +17,19 @@
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: Scientific/Engineering :: Image Processing
+project_urls = 
+	Bug Tracker = https://github.com/jo-mueller/napari-vedo-bridge/issues
+	Documentation = https://github.com/jo-mueller/napari-vedo-bridge#README.md
+	Source Code = https://github.com/jo-mueller/napari-vedo-bridge
+	User Support = https://github.com/jo-mueller/napari-vedo-bridge/issues
 
 [options]
 packages = find:
 install_requires = 
 	numpy
 	magicgui
 	qtpy
```

### Comparing `napari-vedo-bridge-0.0.3/src/napari_vedo_bridge/_cutter_widget.py` & `napari-vedo-bridge-0.0.4/src/napari_vedo_bridge/_cutter_widget.py`

 * *Files identical despite different names*

### Comparing `napari-vedo-bridge-0.0.3/src/napari_vedo_bridge/_tests/test_widget.py` & `napari-vedo-bridge-0.0.4/src/napari_vedo_bridge/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari-vedo-bridge-0.0.3/src/napari_vedo_bridge/vedo_extension.ui` & `napari-vedo-bridge-0.0.4/src/napari_vedo_bridge/vedo_extension.ui`

 * *Files identical despite different names*

### Comparing `napari-vedo-bridge-0.0.3/src/napari_vedo_bridge.egg-info/PKG-INFO` & `napari-vedo-bridge-0.0.4/src/napari_vedo_bridge.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 Metadata-Version: 2.1
 Name: napari-vedo-bridge
-Version: 0.0.3
+Version: 0.0.4
 Summary: Transfer mesh data between napari and vedo for interactive processing
 Author: Johannes Soltwedel, Marco Musy
 Author-email: johannes_richard.soltwedel@tu-dresden.de
 License: BSD-3-Clause
+Project-URL: Bug Tracker, https://github.com/jo-mueller/napari-vedo-bridge/issues
+Project-URL: Documentation, https://github.com/jo-mueller/napari-vedo-bridge#README.md
+Project-URL: Source Code, https://github.com/jo-mueller/napari-vedo-bridge
+Project-URL: User Support, https://github.com/jo-mueller/napari-vedo-bridge/issues
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `napari-vedo-bridge-0.0.3/src/napari_vedo_bridge.egg-info/SOURCES.txt` & `napari-vedo-bridge-0.0.4/src/napari_vedo_bridge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

