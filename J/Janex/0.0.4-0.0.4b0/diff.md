# Comparing `tmp/Janex-0.0.4.tar.gz` & `tmp/Janex-0.0.4b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Janex-0.0.4.tar", last modified: Sun Jul  9 16:13:15 2023, max compression
+gzip compressed data, was "Janex-0.0.4b0.tar", last modified: Sun Jul  9 16:21:56 2023, max compression
```

## Comparing `Janex-0.0.4.tar` & `Janex-0.0.4b0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-09 16:13:15.560086 Janex-0.0.4/
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-09 16:13:15.556165 Janex-0.0.4/Janex/
--rw-r--r--   0 cipher     (501) staff       (20)     4968 2023-07-08 11:35:46.000000 Janex-0.0.4/Janex/Janex.py
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-09 16:13:15.559741 Janex-0.0.4/Janex/JanexSub/
--rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:07:05.000000 Janex-0.0.4/Janex/JanexSub/JanexSub.py
--rw-r--r--   0 cipher     (501) staff       (20)       15 2023-07-09 16:07:32.000000 Janex-0.0.4/Janex/JanexSub/__init__.py
--rw-r--r--   0 cipher     (501) staff       (20)       15 2023-07-09 16:07:37.000000 Janex-0.0.4/Janex/__init__.py
--rw-r--r--   0 cipher     (501) staff       (20)      260 2023-07-07 20:07:57.000000 Janex-0.0.4/Janex/chat.py
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-09 16:13:15.559446 Janex-0.0.4/Janex.egg-info/
--rw-r--r--   0 cipher     (501) staff       (20)     3470 2023-07-09 16:13:15.000000 Janex-0.0.4/Janex.egg-info/PKG-INFO
--rw-r--r--   0 cipher     (501) staff       (20)      280 2023-07-09 16:13:15.000000 Janex-0.0.4/Janex.egg-info/SOURCES.txt
--rw-r--r--   0 cipher     (501) staff       (20)        1 2023-07-09 16:13:15.000000 Janex-0.0.4/Janex.egg-info/dependency_links.txt
--rw-r--r--   0 cipher     (501) staff       (20)       12 2023-07-09 16:13:15.000000 Janex-0.0.4/Janex.egg-info/requires.txt
--rw-r--r--   0 cipher     (501) staff       (20)        6 2023-07-09 16:13:15.000000 Janex-0.0.4/Janex.egg-info/top_level.txt
--rw-r--r--   0 cipher     (501) staff       (20)     2950 2023-07-07 12:33:15.000000 Janex-0.0.4/LICENSE
--rw-r--r--   0 cipher     (501) staff       (20)     3470 2023-07-09 16:13:15.559940 Janex-0.0.4/PKG-INFO
--rw-r--r--   0 cipher     (501) staff       (20)     3065 2023-07-07 20:09:35.000000 Janex-0.0.4/README.md
--rw-r--r--   0 cipher     (501) staff       (20)     1319 2023-07-09 16:11:53.000000 Janex-0.0.4/Setup.py
--rw-r--r--   0 cipher     (501) staff       (20)       38 2023-07-09 16:13:15.560126 Janex-0.0.4/setup.cfg
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-09 16:21:56.822514 Janex-0.0.4b0/
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-09 16:21:56.819554 Janex-0.0.4b0/Janex/
+-rw-r--r--   0 cipher     (501) staff       (20)     4968 2023-07-08 11:35:46.000000 Janex-0.0.4b0/Janex/Janex.py
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-09 16:21:56.822235 Janex-0.0.4b0/Janex/JanexSub/
+-rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:07:05.000000 Janex-0.0.4b0/Janex/JanexSub/JanexSub.py
+-rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:20:34.000000 Janex-0.0.4b0/Janex/JanexSub/__init__.py
+-rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:20:32.000000 Janex-0.0.4b0/Janex/__init__.py
+-rw-r--r--   0 cipher     (501) staff       (20)      260 2023-07-07 20:07:57.000000 Janex-0.0.4b0/Janex/chat.py
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-09 16:21:56.821955 Janex-0.0.4b0/Janex.egg-info/
+-rw-r--r--   0 cipher     (501) staff       (20)     3472 2023-07-09 16:21:56.000000 Janex-0.0.4b0/Janex.egg-info/PKG-INFO
+-rw-r--r--   0 cipher     (501) staff       (20)      280 2023-07-09 16:21:56.000000 Janex-0.0.4b0/Janex.egg-info/SOURCES.txt
+-rw-r--r--   0 cipher     (501) staff       (20)        1 2023-07-09 16:21:56.000000 Janex-0.0.4b0/Janex.egg-info/dependency_links.txt
+-rw-r--r--   0 cipher     (501) staff       (20)       12 2023-07-09 16:21:56.000000 Janex-0.0.4b0/Janex.egg-info/requires.txt
+-rw-r--r--   0 cipher     (501) staff       (20)        6 2023-07-09 16:21:56.000000 Janex-0.0.4b0/Janex.egg-info/top_level.txt
+-rw-r--r--   0 cipher     (501) staff       (20)     2950 2023-07-07 12:33:15.000000 Janex-0.0.4b0/LICENSE
+-rw-r--r--   0 cipher     (501) staff       (20)     3472 2023-07-09 16:21:56.822390 Janex-0.0.4b0/PKG-INFO
+-rw-r--r--   0 cipher     (501) staff       (20)     3065 2023-07-07 20:09:35.000000 Janex-0.0.4b0/README.md
+-rw-r--r--   0 cipher     (501) staff       (20)     1324 2023-07-09 16:21:54.000000 Janex-0.0.4b0/Setup.py
+-rw-r--r--   0 cipher     (501) staff       (20)       38 2023-07-09 16:21:56.822547 Janex-0.0.4b0/setup.cfg
```

### Comparing `Janex-0.0.4/Janex/Janex.py` & `Janex-0.0.4b0/Janex/Janex.py`

 * *Files identical despite different names*

### Comparing `Janex-0.0.4/Janex.egg-info/PKG-INFO` & `Janex-0.0.4b0/Janex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Janex
-Version: 0.0.4
+Version: 0.0.4b0
 Home-page: https://github.com/Cipher58
 Download-URL: https://github.com/Cipher58/Janex/archive/refs/tags/v0.0.2-beta.tar.gz
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `Janex-0.0.4/LICENSE` & `Janex-0.0.4b0/LICENSE`

 * *Files identical despite different names*

### Comparing `Janex-0.0.4/PKG-INFO` & `Janex-0.0.4b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Janex
-Version: 0.0.4
+Version: 0.0.4b0
 Home-page: https://github.com/Cipher58
 Download-URL: https://github.com/Cipher58/Janex/archive/refs/tags/v0.0.2-beta.tar.gz
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `Janex-0.0.4/README.md` & `Janex-0.0.4b0/README.md`

 * *Files identical despite different names*

### Comparing `Janex-0.0.4/Setup.py` & `Janex-0.0.4b0/Setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setuptools.setup(
     # Here is the module name.
     name="Janex",
 
     # version of the module
-    version="0.0.4",
+    version="0.0.4.beta",
 
     # Name of Author
     author="Cipher58",
 
     download_url = 'https://github.com/Cipher58/Janex/archive/refs/tags/v0.0.2-beta.tar.gz',
 
     # your Email address
```

