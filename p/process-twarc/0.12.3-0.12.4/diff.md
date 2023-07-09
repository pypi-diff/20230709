# Comparing `tmp/process-twarc-0.12.3.tar.gz` & `tmp/process-twarc-0.12.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "process-twarc-0.12.3.tar", last modified: Sun Jul  9 11:58:06 2023, max compression
+gzip compressed data, was "process-twarc-0.12.4.tar", last modified: Sun Jul  9 15:58:47 2023, max compression
```

## Comparing `process-twarc-0.12.3.tar` & `process-twarc-0.12.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 11:58:06.697283 process-twarc-0.12.3/
--rw-rw-rw-   0        0        0     1077 2023-07-07 10:42:07.000000 process-twarc-0.12.3/LICENSE.txt
--rw-rw-rw-   0        0        0      693 2023-07-09 11:58:06.697283 process-twarc-0.12.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-07 10:42:22.000000 process-twarc-0.12.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-09 11:58:06.682736 process-twarc-0.12.3/process_twarc/
--rw-rw-rw-   0        0        0        0 2023-07-07 10:27:29.000000 process-twarc-0.12.3/process_twarc/__init__.py
--rw-rw-rw-   0        0        0     8470 2023-07-09 11:55:09.000000 process-twarc-0.12.3/process_twarc/util.py
-drwxrwxrwx   0        0        0        0 2023-07-09 11:58:06.696278 process-twarc-0.12.3/process_twarc.egg-info/
--rw-rw-rw-   0        0        0      693 2023-07-09 11:58:06.000000 process-twarc-0.12.3/process_twarc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-07-09 11:58:06.000000 process-twarc-0.12.3/process_twarc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 11:58:06.000000 process-twarc-0.12.3/process_twarc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-07-09 11:58:06.000000 process-twarc-0.12.3/process_twarc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-09 11:58:06.000000 process-twarc-0.12.3/process_twarc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       56 2023-07-09 11:58:06.698338 process-twarc-0.12.3/setup.cfg
--rw-rw-rw-   0        0        0      976 2023-07-09 11:57:58.000000 process-twarc-0.12.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 15:58:47.237306 process-twarc-0.12.4/
+-rw-rw-rw-   0        0        0     1077 2023-07-07 10:42:07.000000 process-twarc-0.12.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      693 2023-07-09 15:58:47.237306 process-twarc-0.12.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-07 10:42:22.000000 process-twarc-0.12.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 15:58:47.227293 process-twarc-0.12.4/process_twarc/
+-rw-rw-rw-   0        0        0        0 2023-07-07 10:27:29.000000 process-twarc-0.12.4/process_twarc/__init__.py
+-rw-rw-rw-   0        0        0     8173 2023-07-09 15:58:02.000000 process-twarc-0.12.4/process_twarc/util.py
+drwxrwxrwx   0        0        0        0 2023-07-09 15:58:47.236288 process-twarc-0.12.4/process_twarc.egg-info/
+-rw-rw-rw-   0        0        0      693 2023-07-09 15:58:47.000000 process-twarc-0.12.4/process_twarc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-07-09 15:58:47.000000 process-twarc-0.12.4/process_twarc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 15:58:47.000000 process-twarc-0.12.4/process_twarc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-07-09 15:58:47.000000 process-twarc-0.12.4/process_twarc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-09 15:58:47.000000 process-twarc-0.12.4/process_twarc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       56 2023-07-09 15:58:47.238288 process-twarc-0.12.4/setup.cfg
+-rw-rw-rw-   0        0        0      976 2023-07-09 15:58:36.000000 process-twarc-0.12.4/setup.py
```

### Comparing `process-twarc-0.12.3/LICENSE.txt` & `process-twarc-0.12.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `process-twarc-0.12.3/PKG-INFO` & `process-twarc-0.12.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: process-twarc
-Version: 0.12.3
+Version: 0.12.4
 Summary: Tools for tranforming raw data from Twarc2 to structured data for Masked Language Modeling.
 Home-page: https://github.com/user/Lone-Wolfgang
 Author: Jordan Wolfgang Klein
 Author-email: jordan.klein.21@um.edu.mt
 License: MIT
 Keywords: Twitter,Deduplication,Tokenization,Language Modeling
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `process-twarc-0.12.3/process_twarc/util.py` & `process-twarc-0.12.4/process_twarc/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -77,14 +77,17 @@
         file_path (str): Path to the parquet file.
         output_type (str, defaults to "pd"): Type of the output data structure. Either "pd" for pandas DataFrame or "Dataset" for custom Dataset.
         columns (str or list, optional): Columns to load. If provided, only load the specified columns.
 
     Returns:
         object: Loaded data structure.
     """
+    if isinstance(columns, str):
+        columns = list(columns)
+
     if output_type == "pd":
         if columns:
             dataset = pd.read_parquet(file_path, columns=columns)
         else:
             dataset = pd.read_parquet(file_path)
     elif output_type == "Dataset":
         if columns:
@@ -93,81 +96,71 @@
             table = pq.read_table(file_path)
         dataset = Dataset(table)
     else:
         raise ValueError("Please input a valid output type. Either 'pd' or 'Dataset'.")
 
     return dataset
 
-def load_dataset(file_path: str, output_type: str = "pd", columns=None, masks=None):
+def load_dataset(file_path: str, output_type: str = "pd", columns=None, masks=None, drop_mask_columns=True):
     """
     Load a data structure of the selected type from a parquet file and apply optional masking.
 
     Args:
         file_path (str): Path to the parquet file.
         output_type (str, defaults to "pd"): Type of the output data structure. Either "pd" for pandas DataFrame or "Dataset" for custom Dataset.
         columns (str or list, optional): Columns to load. If provided, only load the specified columns.
         masks (str or list, optional): Mask column(s) to apply and remove rows where the mask is True.
 
     Returns:
         object: Loaded data structure.
     """
-    dataset = load_parquet(file_path, output_type, columns)
-
-    if masks is not None:
+    if masks:
         if isinstance(masks, str):
             masks = [masks]
-        
-        if output_type == "pd":
-            for mask in masks:
-                dataset = dataset[~dataset[mask]]
-        elif output_type == "Dataset":
-            for mask in masks:
-                dataset = dataset.filter(~dataset[mask])
-        else:
-            raise ValueError("Please input a valid output type. Either 'pd' or 'Dataset'.")
+        load_type = "pd"
+        dataset = load_parquet(file_path, load_type, columns)
+        mask = dataset[masks].any(axis=1)
+        dataset = dataset[~mask].reset_index(drop=True)
+
+        if drop_mask_columns:
+            dataset = dataset.drop(columns=masks)
+
+        if output_type == "Dataset":
+            dataset = Dataset(pa.Table.from_pandas(dataset))
+        return dataset
 
-    return dataset
+    else:
+        dataset = load_parquet(file_path, load_type, columns)
+        return dataset
 
-import pandas as pd
-import pyarrow.parquet as pq
 
-def concat_dataset(file_paths, output_type="pd", columns=None, masks=None):
+def concat_dataset(file_paths, output_type="pd", columns=None, masks=None, drop_mask_columns=True):
     """
     Concatenate multiple datasets from parquet files and apply optional masking.
 
     Args:
         file_paths (list[str]): Paths to the parquet files.
         output_type (str, defaults to "pd"): Type of the output data structure. Either "pd" for pandas DataFrame or "Dataset" for custom Dataset.
         columns (str or list[str], optional): Columns to load. If provided, only load the specified columns.
         masks (str or list[str], optional): Mask column(s) to apply and remove rows where the mask is True.
 
     Returns:
         object: Concatenated and optionally masked data structure.
     """
     datasets = []
+
+    if columns and masks:
+        columns = list(set(columns+masks))
     
     for file_path in tqdm(file_paths, desc = "Loading dataset"):
-        dataset = load_parquet(file_path, output_type, columns)
+        dataset = load_dataset(file_path, output_type, columns, masks, drop_mask_columns)
         datasets.append(dataset)
     
     concatenated = pd.concat(datasets) if output_type == "pd" else concatenate_datasets(datasets)
     
-    if masks is not None:
-        if isinstance(masks, str):
-            masks = [masks]
-        
-        if output_type == "pd":
-            for mask in masks:
-                concatenated = concatenated[~concatenated[mask]]
-        elif output_type == "Dataset":
-            for mask in masks:
-                concatenated = concatenated.filter(~concatenated[mask])
-        else:
-            raise ValueError("Please input a valid output type. Either 'pd' or 'Dataset'.")
-    
     return concatenated
 
 def get_output_path(file_path:str, output_dir:str, file_type:str=""):
     """
     Generate a new file path for transforming data from one filetype to another.
 
     Given the original file path and the destination folder, generate a new file path
@@ -227,11 +220,7 @@
 
     def modify(example):
         example[column] = function(example[column])
         return example
 
     new_dataset = dataset.map(modify)
     return new_dataset
-
-
-
-
```

### Comparing `process-twarc-0.12.3/process_twarc.egg-info/PKG-INFO` & `process-twarc-0.12.4/process_twarc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: process-twarc
-Version: 0.12.3
+Version: 0.12.4
 Summary: Tools for tranforming raw data from Twarc2 to structured data for Masked Language Modeling.
 Home-page: https://github.com/user/Lone-Wolfgang
 Author: Jordan Wolfgang Klein
 Author-email: jordan.klein.21@um.edu.mt
 License: MIT
 Keywords: Twitter,Deduplication,Tokenization,Language Modeling
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `process-twarc-0.12.3/setup.py` & `process-twarc-0.12.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'process-twarc',         
   packages = ['process_twarc'],   
-  version = '0.12.3',
+  version = '0.12.4',
   license='MIT',
   description = 'Tools for tranforming raw data from Twarc2 to structured data for Masked Language Modeling.',   # Give a short description about your library
   author = 'Jordan Wolfgang Klein',
   author_email = 'jordan.klein.21@um.edu.mt',
   url = 'https://github.com/user/Lone-Wolfgang',
   keywords = ['Twitter', 'Deduplication', "Tokenization", "Language Modeling"],
   install_requires=[
```

