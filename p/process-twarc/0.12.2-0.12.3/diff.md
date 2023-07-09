# Comparing `tmp/process-twarc-0.12.2.tar.gz` & `tmp/process-twarc-0.12.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "process-twarc-0.12.2.tar", last modified: Sun Jul  9 11:52:30 2023, max compression
+gzip compressed data, was "process-twarc-0.12.3.tar", last modified: Sun Jul  9 11:58:06 2023, max compression
```

## Comparing `process-twarc-0.12.2.tar` & `process-twarc-0.12.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 11:52:30.488215 process-twarc-0.12.2/
--rw-rw-rw-   0        0        0     1077 2023-07-07 10:42:07.000000 process-twarc-0.12.2/LICENSE.txt
--rw-rw-rw-   0        0        0      693 2023-07-09 11:52:30.488215 process-twarc-0.12.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-07 10:42:22.000000 process-twarc-0.12.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-09 11:52:30.481276 process-twarc-0.12.2/process_twarc/
--rw-rw-rw-   0        0        0        0 2023-07-07 10:27:29.000000 process-twarc-0.12.2/process_twarc/__init__.py
--rw-rw-rw-   0        0        0     8471 2023-07-09 11:42:16.000000 process-twarc-0.12.2/process_twarc/util.py
-drwxrwxrwx   0        0        0        0 2023-07-09 11:52:30.487211 process-twarc-0.12.2/process_twarc.egg-info/
--rw-rw-rw-   0        0        0      693 2023-07-09 11:52:30.000000 process-twarc-0.12.2/process_twarc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-07-09 11:52:30.000000 process-twarc-0.12.2/process_twarc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 11:52:30.000000 process-twarc-0.12.2/process_twarc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-07-09 11:52:30.000000 process-twarc-0.12.2/process_twarc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-09 11:52:30.000000 process-twarc-0.12.2/process_twarc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       56 2023-07-09 11:52:30.489720 process-twarc-0.12.2/setup.cfg
--rw-rw-rw-   0        0        0      976 2023-07-09 11:51:47.000000 process-twarc-0.12.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 11:58:06.697283 process-twarc-0.12.3/
+-rw-rw-rw-   0        0        0     1077 2023-07-07 10:42:07.000000 process-twarc-0.12.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      693 2023-07-09 11:58:06.697283 process-twarc-0.12.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-07 10:42:22.000000 process-twarc-0.12.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 11:58:06.682736 process-twarc-0.12.3/process_twarc/
+-rw-rw-rw-   0        0        0        0 2023-07-07 10:27:29.000000 process-twarc-0.12.3/process_twarc/__init__.py
+-rw-rw-rw-   0        0        0     8470 2023-07-09 11:55:09.000000 process-twarc-0.12.3/process_twarc/util.py
+drwxrwxrwx   0        0        0        0 2023-07-09 11:58:06.696278 process-twarc-0.12.3/process_twarc.egg-info/
+-rw-rw-rw-   0        0        0      693 2023-07-09 11:58:06.000000 process-twarc-0.12.3/process_twarc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-07-09 11:58:06.000000 process-twarc-0.12.3/process_twarc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 11:58:06.000000 process-twarc-0.12.3/process_twarc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-07-09 11:58:06.000000 process-twarc-0.12.3/process_twarc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-09 11:58:06.000000 process-twarc-0.12.3/process_twarc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       56 2023-07-09 11:58:06.698338 process-twarc-0.12.3/setup.cfg
+-rw-rw-rw-   0        0        0      976 2023-07-09 11:57:58.000000 process-twarc-0.12.3/setup.py
```

### Comparing `process-twarc-0.12.2/LICENSE.txt` & `process-twarc-0.12.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `process-twarc-0.12.2/PKG-INFO` & `process-twarc-0.12.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: process-twarc
-Version: 0.12.2
+Version: 0.12.3
 Summary: Tools for tranforming raw data from Twarc2 to structured data for Masked Language Modeling.
 Home-page: https://github.com/user/Lone-Wolfgang
 Author: Jordan Wolfgang Klein
 Author-email: jordan.klein.21@um.edu.mt
 License: MIT
 Keywords: Twitter,Deduplication,Tokenization,Language Modeling
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `process-twarc-0.12.2/process_twarc/util.py` & `process-twarc-0.12.3/process_twarc/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
     """
     datasets = []
     
     for file_path in tqdm(file_paths, desc = "Loading dataset"):
         dataset = load_parquet(file_path, output_type, columns)
         datasets.append(dataset)
     
-    concatenated = pd.concat(datasets) if output_type == "pd" else concatenate_datasets(datasets))
+    concatenated = pd.concat(datasets) if output_type == "pd" else concatenate_datasets(datasets)
     
     if masks is not None:
         if isinstance(masks, str):
             masks = [masks]
         
         if output_type == "pd":
             for mask in masks:
```

### Comparing `process-twarc-0.12.2/process_twarc.egg-info/PKG-INFO` & `process-twarc-0.12.3/process_twarc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: process-twarc
-Version: 0.12.2
+Version: 0.12.3
 Summary: Tools for tranforming raw data from Twarc2 to structured data for Masked Language Modeling.
 Home-page: https://github.com/user/Lone-Wolfgang
 Author: Jordan Wolfgang Klein
 Author-email: jordan.klein.21@um.edu.mt
 License: MIT
 Keywords: Twitter,Deduplication,Tokenization,Language Modeling
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `process-twarc-0.12.2/setup.py` & `process-twarc-0.12.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'process-twarc',         
   packages = ['process_twarc'],   
-  version = '0.12.2',
+  version = '0.12.3',
   license='MIT',
   description = 'Tools for tranforming raw data from Twarc2 to structured data for Masked Language Modeling.',   # Give a short description about your library
   author = 'Jordan Wolfgang Klein',
   author_email = 'jordan.klein.21@um.edu.mt',
   url = 'https://github.com/user/Lone-Wolfgang',
   keywords = ['Twitter', 'Deduplication', "Tokenization", "Language Modeling"],
   install_requires=[
```

