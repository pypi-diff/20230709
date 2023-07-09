# Comparing `tmp/Janex-0.0.4rc0.tar.gz` & `tmp/Janex-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Janex-0.0.4rc0.tar", last modified: Sun Jul  9 16:32:48 2023, max compression
+gzip compressed data, was "Janex-0.0.5.tar", last modified: Sun Jul  9 16:35:26 2023, max compression
```

## Comparing `Janex-0.0.4rc0.tar` & `Janex-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-09 16:32:48.647762 Janex-0.0.4rc0/
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-09 16:32:48.639689 Janex-0.0.4rc0/Janex/
--rw-r--r--   0 cipher     (501) staff       (20)     4968 2023-07-08 11:35:46.000000 Janex-0.0.4rc0/Janex/JanexCode.py
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-09 16:32:48.647448 Janex-0.0.4rc0/Janex/JanexSub/
--rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:07:05.000000 Janex-0.0.4rc0/Janex/JanexSub/JanexSub.py
--rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:20:34.000000 Janex-0.0.4rc0/Janex/JanexSub/__init__.py
--rw-r--r--   0 cipher     (501) staff       (20)       24 2023-07-09 16:31:28.000000 Janex-0.0.4rc0/Janex/__init__.py
--rw-r--r--   0 cipher     (501) staff       (20)      260 2023-07-07 20:07:57.000000 Janex-0.0.4rc0/Janex/chat.py
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-09 16:32:48.647144 Janex-0.0.4rc0/Janex.egg-info/
--rw-r--r--   0 cipher     (501) staff       (20)     3473 2023-07-09 16:32:48.000000 Janex-0.0.4rc0/Janex.egg-info/PKG-INFO
--rw-r--r--   0 cipher     (501) staff       (20)      284 2023-07-09 16:32:48.000000 Janex-0.0.4rc0/Janex.egg-info/SOURCES.txt
--rw-r--r--   0 cipher     (501) staff       (20)        1 2023-07-09 16:32:48.000000 Janex-0.0.4rc0/Janex.egg-info/dependency_links.txt
--rw-r--r--   0 cipher     (501) staff       (20)       12 2023-07-09 16:32:48.000000 Janex-0.0.4rc0/Janex.egg-info/requires.txt
--rw-r--r--   0 cipher     (501) staff       (20)        6 2023-07-09 16:32:48.000000 Janex-0.0.4rc0/Janex.egg-info/top_level.txt
--rw-r--r--   0 cipher     (501) staff       (20)     2950 2023-07-07 12:33:15.000000 Janex-0.0.4rc0/LICENSE
--rw-r--r--   0 cipher     (501) staff       (20)     3473 2023-07-09 16:32:48.647623 Janex-0.0.4rc0/PKG-INFO
--rw-r--r--   0 cipher     (501) staff       (20)     3065 2023-07-07 20:09:35.000000 Janex-0.0.4rc0/README.md
--rw-r--r--   0 cipher     (501) staff       (20)     1321 2023-07-09 16:32:46.000000 Janex-0.0.4rc0/Setup.py
--rw-r--r--   0 cipher     (501) staff       (20)       38 2023-07-09 16:32:48.647798 Janex-0.0.4rc0/setup.cfg
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-09 16:35:26.238361 Janex-0.0.5/
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-09 16:35:26.232660 Janex-0.0.5/Janex/
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-09 16:35:26.237966 Janex-0.0.5/Janex/JanexSub/
+-rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:07:05.000000 Janex-0.0.5/Janex/JanexSub/JanexSub.py
+-rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:20:34.000000 Janex-0.0.5/Janex/JanexSub/__init__.py
+-rw-r--r--   0 cipher     (501) staff       (20)     4968 2023-07-09 16:34:28.000000 Janex-0.0.5/Janex/__init__.py
+-rw-r--r--   0 cipher     (501) staff       (20)      260 2023-07-07 20:07:57.000000 Janex-0.0.5/Janex/chat.py
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-09 16:35:26.237460 Janex-0.0.5/Janex.egg-info/
+-rw-r--r--   0 cipher     (501) staff       (20)     3470 2023-07-09 16:35:26.000000 Janex-0.0.5/Janex.egg-info/PKG-INFO
+-rw-r--r--   0 cipher     (501) staff       (20)      265 2023-07-09 16:35:26.000000 Janex-0.0.5/Janex.egg-info/SOURCES.txt
+-rw-r--r--   0 cipher     (501) staff       (20)        1 2023-07-09 16:35:26.000000 Janex-0.0.5/Janex.egg-info/dependency_links.txt
+-rw-r--r--   0 cipher     (501) staff       (20)       12 2023-07-09 16:35:26.000000 Janex-0.0.5/Janex.egg-info/requires.txt
+-rw-r--r--   0 cipher     (501) staff       (20)        6 2023-07-09 16:35:26.000000 Janex-0.0.5/Janex.egg-info/top_level.txt
+-rw-r--r--   0 cipher     (501) staff       (20)     2950 2023-07-07 12:33:15.000000 Janex-0.0.5/LICENSE
+-rw-r--r--   0 cipher     (501) staff       (20)     3470 2023-07-09 16:35:26.238179 Janex-0.0.5/PKG-INFO
+-rw-r--r--   0 cipher     (501) staff       (20)     3065 2023-07-07 20:09:35.000000 Janex-0.0.5/README.md
+-rw-r--r--   0 cipher     (501) staff       (20)     1319 2023-07-09 16:35:23.000000 Janex-0.0.5/Setup.py
+-rw-r--r--   0 cipher     (501) staff       (20)       38 2023-07-09 16:35:26.238402 Janex-0.0.5/setup.cfg
```

### Comparing `Janex-0.0.4rc0/Janex/JanexCode.py` & `Janex-0.0.5/Janex/__init__.py`

 * *Files identical despite different names*

### Comparing `Janex-0.0.4rc0/Janex.egg-info/PKG-INFO` & `Janex-0.0.5/Janex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Janex
-Version: 0.0.4rc0
+Version: 0.0.5
 Home-page: https://github.com/Cipher58
 Download-URL: https://github.com/Cipher58/Janex/archive/refs/tags/v0.0.2-beta.tar.gz
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `Janex-0.0.4rc0/LICENSE` & `Janex-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Janex-0.0.4rc0/PKG-INFO` & `Janex-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Janex
-Version: 0.0.4rc0
+Version: 0.0.5
 Home-page: https://github.com/Cipher58
 Download-URL: https://github.com/Cipher58/Janex/archive/refs/tags/v0.0.2-beta.tar.gz
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `Janex-0.0.4rc0/README.md` & `Janex-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `Janex-0.0.4rc0/Setup.py` & `Janex-0.0.5/Setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setuptools.setup(
     # Here is the module name.
     name="Janex",
 
     # version of the module
-    version="0.0.4.c",
+    version="0.0.5",
 
     # Name of Author
     author="Cipher58",
 
     download_url = 'https://github.com/Cipher58/Janex/archive/refs/tags/v0.0.2-beta.tar.gz',
 
     # your Email address
```

