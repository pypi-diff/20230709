# Comparing `tmp/WifiOrca-0.0.4.tar.gz` & `tmp/WifiOrca-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WifiOrca-0.0.4.tar", last modified: Sun Jul  9 03:11:41 2023, max compression
+gzip compressed data, was "WifiOrca-0.0.5.tar", last modified: Sun Jul  9 05:33:56 2023, max compression
```

## Comparing `WifiOrca-0.0.4.tar` & `WifiOrca-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-09 03:11:41.804472 WifiOrca-0.0.4/
--rw-r--r--   0 kali      (1000) kali      (1000)      680 2023-07-09 03:11:41.804472 WifiOrca-0.0.4/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      115 2023-07-09 03:10:20.000000 WifiOrca-0.0.4/README.md
--rw-r--r--   0 kali      (1000) kali      (1000)      748 2023-07-09 03:11:34.000000 WifiOrca-0.0.4/pyproject.toml
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-07-09 03:11:41.804472 WifiOrca-0.0.4/setup.cfg
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-09 03:11:41.804472 WifiOrca-0.0.4/src/
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-09 03:11:41.804472 WifiOrca-0.0.4/src/WifiOrca/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-07-07 21:24:23.000000 WifiOrca-0.0.4/src/WifiOrca/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)      165 2023-07-09 03:07:49.000000 WifiOrca-0.0.4/src/WifiOrca/main.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-09 03:11:41.804472 WifiOrca-0.0.4/src/WifiOrca.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)      680 2023-07-09 03:11:41.000000 WifiOrca-0.0.4/src/WifiOrca.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      249 2023-07-09 03:11:41.000000 WifiOrca-0.0.4/src/WifiOrca.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-07-09 03:11:41.000000 WifiOrca-0.0.4/src/WifiOrca.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       17 2023-07-09 03:11:41.000000 WifiOrca-0.0.4/src/WifiOrca.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        9 2023-07-09 03:11:41.000000 WifiOrca-0.0.4/src/WifiOrca.egg-info/top_level.txt
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-09 05:33:56.184456 WifiOrca-0.0.5/
+-rw-r--r--   0 kali      (1000) kali      (1000)     1130 2023-07-09 05:33:56.184456 WifiOrca-0.0.5/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      565 2023-07-09 05:33:43.000000 WifiOrca-0.0.5/README.md
+-rw-r--r--   0 kali      (1000) kali      (1000)      748 2023-07-09 03:37:58.000000 WifiOrca-0.0.5/pyproject.toml
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-07-09 05:33:56.184456 WifiOrca-0.0.5/setup.cfg
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-09 05:33:56.184456 WifiOrca-0.0.5/src/
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-09 05:33:56.184456 WifiOrca-0.0.5/src/WifiOrca/
+-rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-07-07 21:24:23.000000 WifiOrca-0.0.5/src/WifiOrca/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      314 2023-07-09 05:26:09.000000 WifiOrca-0.0.5/src/WifiOrca/main.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2227 2023-07-09 05:20:33.000000 WifiOrca-0.0.5/src/WifiOrca/reverse_shell_client.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      855 2023-07-09 05:33:40.000000 WifiOrca-0.0.5/src/WifiOrca/reverse_shell_server.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-09 05:33:56.184456 WifiOrca-0.0.5/src/WifiOrca.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     1130 2023-07-09 05:33:56.000000 WifiOrca-0.0.5/src/WifiOrca.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      323 2023-07-09 05:33:56.000000 WifiOrca-0.0.5/src/WifiOrca.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-07-09 05:33:56.000000 WifiOrca-0.0.5/src/WifiOrca.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       17 2023-07-09 05:33:56.000000 WifiOrca-0.0.5/src/WifiOrca.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        9 2023-07-09 05:33:56.000000 WifiOrca-0.0.5/src/WifiOrca.egg-info/top_level.txt
```

### Comparing `WifiOrca-0.0.4/pyproject.toml` & `WifiOrca-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "WifiOrca"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Michael Mueller", email="michael.j.mueller.pro@gmail.com" },
 ]
 description = "Wifi Orca contains free and open source tools similar to hak5! Please see github for more info!"
 readme = "README.md"
 license = { file="LICENSE.txt" }
 requires-python = ">=3.9"
```

