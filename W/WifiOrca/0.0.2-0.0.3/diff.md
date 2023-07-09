# Comparing `tmp/WifiOrca-0.0.2.tar.gz` & `tmp/WifiOrca-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WifiOrca-0.0.2.tar", last modified: Sun Jul  9 02:56:26 2023, max compression
+gzip compressed data, was "WifiOrca-0.0.3.tar", last modified: Sun Jul  9 03:08:09 2023, max compression
```

## Comparing `WifiOrca-0.0.2.tar` & `WifiOrca-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-09 02:56:26.426658 WifiOrca-0.0.2/
--rw-r--r--   0 kali      (1000) kali      (1000)      648 2023-07-09 02:56:26.426658 WifiOrca-0.0.2/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      101 2023-07-07 21:24:23.000000 WifiOrca-0.0.2/README.md
--rw-r--r--   0 kali      (1000) kali      (1000)      730 2023-07-09 02:55:48.000000 WifiOrca-0.0.2/pyproject.toml
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-07-09 02:56:26.426658 WifiOrca-0.0.2/setup.cfg
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-09 02:56:26.426658 WifiOrca-0.0.2/src/
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-09 02:56:26.426658 WifiOrca-0.0.2/src/WifiOrca/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-07-07 21:24:23.000000 WifiOrca-0.0.2/src/WifiOrca/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)     4027 2023-07-09 02:56:13.000000 WifiOrca-0.0.2/src/WifiOrca/elf.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-09 02:56:26.426658 WifiOrca-0.0.2/src/WifiOrca.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)      648 2023-07-09 02:56:26.000000 WifiOrca-0.0.2/src/WifiOrca.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      248 2023-07-09 02:56:26.000000 WifiOrca-0.0.2/src/WifiOrca.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-07-09 02:56:26.000000 WifiOrca-0.0.2/src/WifiOrca.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       17 2023-07-09 02:56:26.000000 WifiOrca-0.0.2/src/WifiOrca.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        9 2023-07-09 02:56:26.000000 WifiOrca-0.0.2/src/WifiOrca.egg-info/top_level.txt
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-09 03:08:09.339741 WifiOrca-0.0.3/
+-rw-r--r--   0 kali      (1000) kali      (1000)      648 2023-07-09 03:08:09.339741 WifiOrca-0.0.3/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      101 2023-07-07 21:24:23.000000 WifiOrca-0.0.3/README.md
+-rw-r--r--   0 kali      (1000) kali      (1000)      730 2023-07-09 02:58:58.000000 WifiOrca-0.0.3/pyproject.toml
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-07-09 03:08:09.339741 WifiOrca-0.0.3/setup.cfg
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-09 03:08:09.339741 WifiOrca-0.0.3/src/
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-09 03:08:09.339741 WifiOrca-0.0.3/src/WifiOrca/
+-rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-07-07 21:24:23.000000 WifiOrca-0.0.3/src/WifiOrca/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      165 2023-07-09 03:07:49.000000 WifiOrca-0.0.3/src/WifiOrca/main.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-09 03:08:09.339741 WifiOrca-0.0.3/src/WifiOrca.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)      648 2023-07-09 03:08:09.000000 WifiOrca-0.0.3/src/WifiOrca.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      249 2023-07-09 03:08:09.000000 WifiOrca-0.0.3/src/WifiOrca.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-07-09 03:08:09.000000 WifiOrca-0.0.3/src/WifiOrca.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       17 2023-07-09 03:08:09.000000 WifiOrca-0.0.3/src/WifiOrca.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        9 2023-07-09 03:08:09.000000 WifiOrca-0.0.3/src/WifiOrca.egg-info/top_level.txt
```

### Comparing `WifiOrca-0.0.2/PKG-INFO` & `WifiOrca-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WifiOrca
-Version: 0.0.2
+Version: 0.0.3
 Summary: Wifi Orca contains free and open source tools similar to hak5! Requires nmap!
 Author-email: Michael Mueller <michael.j.mueller.pro@gmail.com>
 Project-URL: Homepage, https://github.com/Invizabel/Wifi-Orca
 Project-URL: Bug Tracker, https://github.com/Invizabel/Wifi-Orca/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `WifiOrca-0.0.2/pyproject.toml` & `WifiOrca-0.0.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "WifiOrca"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Michael Mueller", email="michael.j.mueller.pro@gmail.com" },
 ]
 description = "Wifi Orca contains free and open source tools similar to hak5! Requires nmap!"
 readme = "README.md"
 license = { file="LICENSE.txt" }
 requires-python = ">=3.9"
```

### Comparing `WifiOrca-0.0.2/src/WifiOrca.egg-info/PKG-INFO` & `WifiOrca-0.0.3/src/WifiOrca.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WifiOrca
-Version: 0.0.2
+Version: 0.0.3
 Summary: Wifi Orca contains free and open source tools similar to hak5! Requires nmap!
 Author-email: Michael Mueller <michael.j.mueller.pro@gmail.com>
 Project-URL: Homepage, https://github.com/Invizabel/Wifi-Orca
 Project-URL: Bug Tracker, https://github.com/Invizabel/Wifi-Orca/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

