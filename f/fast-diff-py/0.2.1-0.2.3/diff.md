# Comparing `tmp/fast_diff_py-0.2.1.tar.gz` & `tmp/fast_diff_py-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_diff_py-0.2.1.tar", last modified: Sat Jul  8 23:39:09 2023, max compression
+gzip compressed data, was "fast_diff_py-0.2.3.tar", last modified: Sun Jul  9 00:06:25 2023, max compression
```

## Comparing `fast_diff_py-0.2.1.tar` & `fast_diff_py-0.2.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-08 23:39:09.436659 fast_diff_py-0.2.1/
--rwxrwxrwx   0 root         (0) root         (0)     1070 2023-02-17 16:03:58.000000 fast_diff_py-0.2.1/LICENSE.txt
--rwxrwxrwx   0 root         (0) root         (0)    10092 2023-07-08 23:39:09.436827 fast_diff_py-0.2.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     7894 2023-07-06 21:38:13.000000 fast_diff_py-0.2.1/README.md
--rwxrwxrwx   0 root         (0) root         (0)     1108 2023-07-08 23:35:01.000000 fast_diff_py-0.2.1/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)      977 2023-07-08 23:39:09.437245 fast_diff_py-0.2.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      579 2023-07-08 23:37:02.000000 fast_diff_py-0.2.1/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-08 23:39:09.430388 fast_diff_py-0.2.1/src/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-08 23:39:09.434930 fast_diff_py-0.2.1/src/fast_diff_py/
--rwxrwxrwx   0 root         (0) root         (0)      114 2023-07-08 11:57:20.000000 fast_diff_py-0.2.1/src/fast_diff_py/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    17697 2023-07-08 13:11:54.000000 fast_diff_py-0.2.1/src/fast_diff_py/child_processes.py
--rwxrwxrwx   0 root         (0) root         (0)    13893 2023-07-07 14:48:21.000000 fast_diff_py-0.2.1/src/fast_diff_py/config.py
--rwxrwxrwx   0 root         (0) root         (0)    23138 2023-07-08 05:26:18.000000 fast_diff_py-0.2.1/src/fast_diff_py/cpu_image_processor.py
--rwxrwxrwx   0 root         (0) root         (0)    16005 2023-07-08 05:26:18.000000 fast_diff_py-0.2.1/src/fast_diff_py/database.py
--rwxrwxrwx   0 root         (0) root         (0)    12143 2023-07-06 21:38:13.000000 fast_diff_py-0.2.1/src/fast_diff_py/datatransfer.py
--rwxrwxrwx   0 root         (0) root         (0)     9588 2023-07-08 13:43:56.000000 fast_diff_py-0.2.1/src/fast_diff_py/dif.py
--rwxrwxrwx   0 root         (0) root         (0)    67447 2023-07-08 13:42:47.000000 fast_diff_py-0.2.1/src/fast_diff_py/fastDif.py
--rwxrwxrwx   0 root         (0) root         (0)    31323 2023-07-08 05:26:18.000000 fast_diff_py-0.2.1/src/fast_diff_py/fast_diff_base.py
--rwxrwxrwx   0 root         (0) root         (0)     2585 2023-07-08 05:26:18.000000 fast_diff_py-0.2.1/src/fast_diff_py/gpu_image_processor.py
--rwxrwxrwx   0 root         (0) root         (0)    39101 2023-07-08 05:26:18.000000 fast_diff_py-0.2.1/src/fast_diff_py/mariadb_database.py
--rwxrwxrwx   0 root         (0) root         (0)    38244 2023-07-08 05:26:18.000000 fast_diff_py-0.2.1/src/fast_diff_py/sql_database.py
--rwxrwxrwx   0 root         (0) root         (0)     4727 2023-07-06 21:38:13.000000 fast_diff_py-0.2.1/src/fast_diff_py/utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-08 23:39:09.436491 fast_diff_py-0.2.1/src/fast_diff_py.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)    10092 2023-07-08 23:39:09.000000 fast_diff_py-0.2.1/src/fast_diff_py.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      753 2023-07-08 23:39:09.000000 fast_diff_py-0.2.1/src/fast_diff_py.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-08 23:39:09.000000 fast_diff_py-0.2.1/src/fast_diff_py.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       46 2023-07-08 23:39:09.000000 fast_diff_py-0.2.1/src/fast_diff_py.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-08 16:58:08.000000 fast_diff_py-0.2.1/src/fast_diff_py.egg-info/not-zip-safe
--rwxrwxrwx   0 root         (0) root         (0)       81 2023-07-08 23:39:09.000000 fast_diff_py-0.2.1/src/fast_diff_py.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       13 2023-07-08 23:39:09.000000 fast_diff_py-0.2.1/src/fast_diff_py.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-09 00:06:25.710291 fast_diff_py-0.2.3/
+-rwxrwxrwx   0 root         (0) root         (0)     1070 2023-02-17 16:03:58.000000 fast_diff_py-0.2.3/LICENSE.txt
+-rwxrwxrwx   0 root         (0) root         (0)    10092 2023-07-09 00:06:25.710471 fast_diff_py-0.2.3/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     7894 2023-07-06 21:38:13.000000 fast_diff_py-0.2.3/README.md
+-rwxrwxrwx   0 root         (0) root         (0)     1108 2023-07-09 00:06:00.000000 fast_diff_py-0.2.3/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)      977 2023-07-09 00:06:25.710993 fast_diff_py-0.2.3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      579 2023-07-09 00:06:00.000000 fast_diff_py-0.2.3/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-09 00:06:25.691645 fast_diff_py-0.2.3/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-09 00:06:25.708773 fast_diff_py-0.2.3/src/fast_diff_py/
+-rwxrwxrwx   0 root         (0) root         (0)      114 2023-07-08 11:57:20.000000 fast_diff_py-0.2.3/src/fast_diff_py/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    17697 2023-07-08 13:11:54.000000 fast_diff_py-0.2.3/src/fast_diff_py/child_processes.py
+-rwxrwxrwx   0 root         (0) root         (0)    13893 2023-07-07 14:48:21.000000 fast_diff_py-0.2.3/src/fast_diff_py/config.py
+-rwxrwxrwx   0 root         (0) root         (0)    23138 2023-07-08 05:26:18.000000 fast_diff_py-0.2.3/src/fast_diff_py/cpu_image_processor.py
+-rwxrwxrwx   0 root         (0) root         (0)    16005 2023-07-08 05:26:18.000000 fast_diff_py-0.2.3/src/fast_diff_py/database.py
+-rwxrwxrwx   0 root         (0) root         (0)    12143 2023-07-06 21:38:13.000000 fast_diff_py-0.2.3/src/fast_diff_py/datatransfer.py
+-rwxrwxrwx   0 root         (0) root         (0)     9991 2023-07-09 00:02:02.000000 fast_diff_py-0.2.3/src/fast_diff_py/dif.py
+-rwxrwxrwx   0 root         (0) root         (0)    67447 2023-07-08 13:42:47.000000 fast_diff_py-0.2.3/src/fast_diff_py/fastDif.py
+-rwxrwxrwx   0 root         (0) root         (0)    31323 2023-07-08 05:26:18.000000 fast_diff_py-0.2.3/src/fast_diff_py/fast_diff_base.py
+-rwxrwxrwx   0 root         (0) root         (0)     2585 2023-07-08 05:26:18.000000 fast_diff_py-0.2.3/src/fast_diff_py/gpu_image_processor.py
+-rwxrwxrwx   0 root         (0) root         (0)    39101 2023-07-08 05:26:18.000000 fast_diff_py-0.2.3/src/fast_diff_py/mariadb_database.py
+-rwxrwxrwx   0 root         (0) root         (0)    38244 2023-07-08 05:26:18.000000 fast_diff_py-0.2.3/src/fast_diff_py/sql_database.py
+-rwxrwxrwx   0 root         (0) root         (0)     4727 2023-07-06 21:38:13.000000 fast_diff_py-0.2.3/src/fast_diff_py/utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-09 00:06:25.710132 fast_diff_py-0.2.3/src/fast_diff_py.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)    10092 2023-07-09 00:06:25.000000 fast_diff_py-0.2.3/src/fast_diff_py.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      753 2023-07-09 00:06:25.000000 fast_diff_py-0.2.3/src/fast_diff_py.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-09 00:06:25.000000 fast_diff_py-0.2.3/src/fast_diff_py.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       46 2023-07-09 00:06:25.000000 fast_diff_py-0.2.3/src/fast_diff_py.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-08 16:58:08.000000 fast_diff_py-0.2.3/src/fast_diff_py.egg-info/not-zip-safe
+-rwxrwxrwx   0 root         (0) root         (0)       81 2023-07-09 00:06:25.000000 fast_diff_py-0.2.3/src/fast_diff_py.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       13 2023-07-09 00:06:25.000000 fast_diff_py-0.2.3/src/fast_diff_py.egg-info/top_level.txt
```

### Comparing `fast_diff_py-0.2.1/LICENSE.txt` & `fast_diff_py-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fast_diff_py-0.2.1/PKG-INFO` & `fast_diff_py-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fast_diff_py
-Version: 0.2.1
+Version: 0.2.3
 Summary: Multithreaded implementation of difpy with progress retention.
 Home-page: https://github.com/AliSot2000/Fast-Image-Deduplicator
-Download-URL: https://github.com/AliSot2000/Fast-Image-Deduplicator/archive/refs/tags/v0.2.1.tar.gz
+Download-URL: https://github.com/AliSot2000/Fast-Image-Deduplicator/archive/refs/tags/v0.2.3.tar.gz
 Author: Elise Landman
 Author-email: Alexander Sotoudeh <alisot200@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Elise Landman
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `fast_diff_py-0.2.1/README.md` & `fast_diff_py-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `fast_diff_py-0.2.1/pyproject.toml` & `fast_diff_py-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "fast_diff_py"
 readme = "README.md"
-version = "0.2.1"
+version = "0.2.3"
 description = "Multithreaded implementation of difpy with progress retention."
 requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 keywords = ['python', 'image deduplicator', 'fast image deduplicator']
 authors = [
     {name = "Alexander Sotoudeh", email="alisot200@gmail.com"},
     {name = "Elise Landman"}
```

### Comparing `fast_diff_py-0.2.1/setup.cfg` & `fast_diff_py-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `fast_diff_py-0.2.1/setup.py` & `fast_diff_py-0.2.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 from distutils.core import setup
 setup(
   # packages = ['fast_diff_py'],   # Chose the same as "name"
-  version = '0.2.1',      # Start with a small number and increase it with every change you make
+  version = '0.2.3',      # Start with a small number and increase it with every change you make
   url = 'https://github.com/AliSot2000/Fast-Image-Deduplicator',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/AliSot2000/Fast-Image-Deduplicator/archive/refs/tags/v0.2.1.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/AliSot2000/Fast-Image-Deduplicator/archive/refs/tags/v0.2.3.tar.gz',    # I explain this later on
   keywords = ['python', 'image deduplicator', 'fast image deduplicator'],   # Keywords that define your package best
 )
```

### Comparing `fast_diff_py-0.2.1/src/fast_diff_py/child_processes.py` & `fast_diff_py-0.2.3/src/fast_diff_py/child_processes.py`

 * *Files identical despite different names*

### Comparing `fast_diff_py-0.2.1/src/fast_diff_py/config.py` & `fast_diff_py-0.2.3/src/fast_diff_py/config.py`

 * *Files identical despite different names*

### Comparing `fast_diff_py-0.2.1/src/fast_diff_py/cpu_image_processor.py` & `fast_diff_py-0.2.3/src/fast_diff_py/cpu_image_processor.py`

 * *Files identical despite different names*

### Comparing `fast_diff_py-0.2.1/src/fast_diff_py/database.py` & `fast_diff_py-0.2.3/src/fast_diff_py/database.py`

 * *Files identical despite different names*

### Comparing `fast_diff_py-0.2.1/src/fast_diff_py/datatransfer.py` & `fast_diff_py-0.2.3/src/fast_diff_py/datatransfer.py`

 * *Files identical despite different names*

### Comparing `fast_diff_py-0.2.1/src/fast_diff_py/dif.py` & `fast_diff_py-0.2.3/src/fast_diff_py/dif.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from datetime import datetime
 import os
 import time
 import argparse
 import json
 import warnings
-import fastDif
+import fast_diff_py.fastDif as fastDif
 warnings.filterwarnings('ignore')
 
 
 def build_low_quality_and_delete(res: dict, del_img: bool = False):
     deleted = 0
     low_quality = []
     # delete lower quality images
@@ -73,27 +73,42 @@
             stats["similarity_grade"] = similarity
         stats["similarity_mse"] = parse_similarity(similarity)
         stats["total_files_searched"] = total_searched
         stats["total_dupl_sim_found"] = total_found
         return stats
 
 
-# Parameters for when launching fast_diff_py via CLI
-if __name__ == "__main__":    
+def main():
+    """
+    Perform entire action of the script.
+    :return:
+    """
     # set CLI arguments
-    parser = argparse.ArgumentParser(description='Find duplicate or similar images on your computer with fast_diff_py - https://github.com/elisemercury/Duplicate-Image-Finder')
+    parser = argparse.ArgumentParser(
+        description='Find duplicate or similar images on your computer with fast_diff_py - https://github.com/elisemercury/Duplicate-Image-Finder')
     parser.add_argument("-A", "--directory_A", type=str, help='Directory to search for images.', required=True)
-    parser.add_argument("-B", "--directory_B", type=str, help='(optional) Second directory to search for images.', required=False, nargs='?', default=None)
-    parser.add_argument("-Z", "--output_directory", type=str, help='(optional) Output directory for the fast_diff_py result files. Default is working dir.', required=False, nargs='?', default=None)
-    parser.add_argument("-s", "--similarity", type=type_str_int, help='(optional) Similarity grade.', required=False, nargs='?', default='normal')
-    parser.add_argument("-px", "--px_size", type=int, help='(optional) Compression size of images in pixels.', required=False, nargs='?', default=50)
-    parser.add_argument("-p", "--show_progress", type=bool, help='(optional) Shows the real-time progress of fast_diff_py.', required=False, nargs='?', choices=[True, False], default=True)
-    parser.add_argument("-o", "--show_output", type=bool, help='(optional) Shows the comapred images in real-time.', required=False, nargs='?', choices=[True, False], default=False)
-    parser.add_argument("-d", "--delete", type=bool, help='(optional) Deletes all duplicate images with lower quality.', required=False, nargs='?', choices=[True, False], default=False)
-    parser.add_argument("-D", "--silent_del", type=bool, help='(optional) Supresses the user confirmation when deleting images.', required=False, nargs='?', choices=[True, False], default=False)
+    parser.add_argument("-B", "--directory_B", type=str, help='(optional) Second directory to search for images.',
+                        required=False, nargs='?', default=None)
+    parser.add_argument("-Z", "--output_directory", type=str,
+                        help='(optional) Output directory for the fast_diff_py result files. Default is working dir.',
+                        required=False, nargs='?', default=None)
+    parser.add_argument("-s", "--similarity", type=type_str_int, help='(optional) Similarity grade.', required=False,
+                        nargs='?', default='normal')
+    parser.add_argument("-px", "--px_size", type=int, help='(optional) Compression size of images in pixels.',
+                        required=False, nargs='?', default=50)
+    parser.add_argument("-p", "--show_progress", type=bool,
+                        help='(optional) Shows the real-time progress of fast_diff_py.', required=False, nargs='?',
+                        choices=[True, False], default=True)
+    parser.add_argument("-o", "--show_output", type=bool, help='(optional) Shows the comapred images in real-time.',
+                        required=False, nargs='?', choices=[True, False], default=False)
+    parser.add_argument("-d", "--delete", type=bool, help='(optional) Deletes all duplicate images with lower quality.',
+                        required=False, nargs='?', choices=[True, False], default=False)
+    parser.add_argument("-D", "--silent_del", type=bool,
+                        help='(optional) Supresses the user confirmation when deleting images.', required=False,
+                        nargs='?', choices=[True, False], default=False)
     args = parser.parse_args()
 
     use_existing = False
     # verify first if there exists already a config that was in progress.
     if fastDif.test_existing_config():
         while True:
             resp = input("A Config exists from a previous run - do you want to finish it first [y,n]")
@@ -160,15 +175,15 @@
 
     if config.state == "indexed_dirs" or config.state == "first_loop_in_progress":
         fdp.first_loop_iteration()
 
     if fdp.stop_received:
         exit(0)
 
-    if config.state == "first_loop_done" or config.state=="second_loop_in_progress":
+    if config.state == "first_loop_done" or config.state == "second_loop_in_progress":
         fdp.second_loop_iteration(
             similarity_threshold=parse_similarity(config.cli_args["similarity"]),
             make_diff_plots=config.cli_args["show_output"],
             diff_location=os.path.join(os.path.dirname(__file__), "diff_plots")
         )
         print(f"Comparison images located at {os.path.join(os.path.dirname(__file__), 'diff_plots')}")
 
@@ -202,15 +217,15 @@
                 dir_b=config.p_root_dir_b,
                 similarity=config.cli_args["similarity"],
                 start=start, end=stop,
                 total_found=len(results),
                 total_searched=comp)
 
     # create filenames for the output files
-    timestamp =str(time.time()).replace(".", "_")
+    timestamp = str(time.time()).replace(".", "_")
     result_file = "difPy_results_" + timestamp + ".json"
     lq_file = "difPy_lower_quality_" + timestamp + ".txt"
     stats_file = "difPy_stats_" + timestamp + ".json"
 
     if config.cli_args["output_directory"] is not None:
         t_dir = config.cli_args["output_directory"]
     else:
@@ -224,8 +239,13 @@
 
     with open(os.path.join(t_dir, lq_file), "w") as file:
         file.writelines(low_quality)
 
     with open(os.path.join(t_dir, stats_file), "w") as file:
         json.dump(sts, file)
 
-    print(f"""\nSaved fast_diff_py results into folder {t_dir} and filenames:\n{result_file} \n{lq_file} \n{stats_file}""")
+    print(
+        f"""\nSaved fast_diff_py results into folder {t_dir} and filenames:\n{result_file} \n{lq_file} \n{stats_file}""")
+
+# Parameters for when launching fast_diff_py via CLI
+if __name__ == "__main__":    
+    main()
```

### Comparing `fast_diff_py-0.2.1/src/fast_diff_py/fastDif.py` & `fast_diff_py-0.2.3/src/fast_diff_py/fastDif.py`

 * *Files identical despite different names*

### Comparing `fast_diff_py-0.2.1/src/fast_diff_py/fast_diff_base.py` & `fast_diff_py-0.2.3/src/fast_diff_py/fast_diff_base.py`

 * *Files identical despite different names*

### Comparing `fast_diff_py-0.2.1/src/fast_diff_py/gpu_image_processor.py` & `fast_diff_py-0.2.3/src/fast_diff_py/gpu_image_processor.py`

 * *Files identical despite different names*

### Comparing `fast_diff_py-0.2.1/src/fast_diff_py/mariadb_database.py` & `fast_diff_py-0.2.3/src/fast_diff_py/mariadb_database.py`

 * *Files identical despite different names*

### Comparing `fast_diff_py-0.2.1/src/fast_diff_py/sql_database.py` & `fast_diff_py-0.2.3/src/fast_diff_py/sql_database.py`

 * *Files identical despite different names*

### Comparing `fast_diff_py-0.2.1/src/fast_diff_py/utils.py` & `fast_diff_py-0.2.3/src/fast_diff_py/utils.py`

 * *Files identical despite different names*

### Comparing `fast_diff_py-0.2.1/src/fast_diff_py.egg-info/PKG-INFO` & `fast_diff_py-0.2.3/src/fast_diff_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fast-diff-py
-Version: 0.2.1
+Version: 0.2.3
 Summary: Multithreaded implementation of difpy with progress retention.
 Home-page: https://github.com/AliSot2000/Fast-Image-Deduplicator
-Download-URL: https://github.com/AliSot2000/Fast-Image-Deduplicator/archive/refs/tags/v0.2.1.tar.gz
+Download-URL: https://github.com/AliSot2000/Fast-Image-Deduplicator/archive/refs/tags/v0.2.3.tar.gz
 Author: Elise Landman
 Author-email: Alexander Sotoudeh <alisot200@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Elise Landman
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `fast_diff_py-0.2.1/src/fast_diff_py.egg-info/SOURCES.txt` & `fast_diff_py-0.2.3/src/fast_diff_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

