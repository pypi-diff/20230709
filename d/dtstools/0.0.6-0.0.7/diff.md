# Comparing `tmp/dtstools-0.0.6.tar.gz` & `tmp/dtstools-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtstools-0.0.6.tar", last modified: Thu Jul  6 15:14:57 2023, max compression
+gzip compressed data, was "dtstools-0.0.7.tar", last modified: Sun Jul  9 14:27:13 2023, max compression
```

## Comparing `dtstools-0.0.6.tar` & `dtstools-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 reginaldosilva   (501) staff       (20)        0 2023-07-06 15:14:57.816619 dtstools-0.0.6/
--rw-r--r--   0 reginaldosilva   (501) staff       (20)     1072 2023-06-17 11:23:10.000000 dtstools-0.0.6/LICENSE
--rw-r--r--   0 reginaldosilva   (501) staff       (20)    11384 2023-07-06 15:14:57.815814 dtstools-0.0.6/PKG-INFO
--rw-r--r--   0 reginaldosilva   (501) staff       (20)     9395 2023-07-06 15:09:30.000000 dtstools-0.0.6/README.md
--rw-r--r--   0 reginaldosilva   (501) staff       (20)      865 2023-07-06 15:07:43.000000 dtstools-0.0.6/pyproject.toml
--rw-r--r--   0 reginaldosilva   (501) staff       (20)       38 2023-07-06 15:14:57.816776 dtstools-0.0.6/setup.cfg
-drwxr-xr-x   0 reginaldosilva   (501) staff       (20)        0 2023-07-06 15:14:57.810357 dtstools-0.0.6/src/
-drwxr-xr-x   0 reginaldosilva   (501) staff       (20)        0 2023-07-06 15:14:57.812370 dtstools-0.0.6/src/dtstools/
--rw-r--r--   0 reginaldosilva   (501) staff       (20)        0 2023-06-09 17:32:34.000000 dtstools-0.0.6/src/dtstools/__init__.py
--rw-r--r--   0 reginaldosilva   (501) staff       (20)    10490 2023-07-06 15:07:37.000000 dtstools-0.0.6/src/dtstools/dtsTable.py
-drwxr-xr-x   0 reginaldosilva   (501) staff       (20)        0 2023-07-06 15:14:57.814954 dtstools-0.0.6/src/dtstools.egg-info/
--rw-r--r--   0 reginaldosilva   (501) staff       (20)    11384 2023-07-06 15:14:57.000000 dtstools-0.0.6/src/dtstools.egg-info/PKG-INFO
--rw-r--r--   0 reginaldosilva   (501) staff       (20)      226 2023-07-06 15:14:57.000000 dtstools-0.0.6/src/dtstools.egg-info/SOURCES.txt
--rw-r--r--   0 reginaldosilva   (501) staff       (20)        1 2023-07-06 15:14:57.000000 dtstools-0.0.6/src/dtstools.egg-info/dependency_links.txt
--rw-r--r--   0 reginaldosilva   (501) staff       (20)        9 2023-07-06 15:14:57.000000 dtstools-0.0.6/src/dtstools.egg-info/top_level.txt
+drwxr-xr-x   0 reginaldosilva   (501) staff       (20)        0 2023-07-09 14:27:13.746198 dtstools-0.0.7/
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)     1072 2023-06-17 11:23:10.000000 dtstools-0.0.7/LICENSE
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)    11384 2023-07-09 14:27:13.745690 dtstools-0.0.7/PKG-INFO
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)     9395 2023-07-09 14:20:50.000000 dtstools-0.0.7/README.md
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)      865 2023-07-09 14:20:55.000000 dtstools-0.0.7/pyproject.toml
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)       38 2023-07-09 14:27:13.746355 dtstools-0.0.7/setup.cfg
+drwxr-xr-x   0 reginaldosilva   (501) staff       (20)        0 2023-07-09 14:27:13.739888 dtstools-0.0.7/src/
+drwxr-xr-x   0 reginaldosilva   (501) staff       (20)        0 2023-07-09 14:27:13.742288 dtstools-0.0.7/src/dtstools/
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)        0 2023-06-09 17:32:34.000000 dtstools-0.0.7/src/dtstools/__init__.py
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)    10653 2023-07-09 14:22:23.000000 dtstools-0.0.7/src/dtstools/dtsTable.py
+drwxr-xr-x   0 reginaldosilva   (501) staff       (20)        0 2023-07-09 14:27:13.744922 dtstools-0.0.7/src/dtstools.egg-info/
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)    11384 2023-07-09 14:27:13.000000 dtstools-0.0.7/src/dtstools.egg-info/PKG-INFO
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)      226 2023-07-09 14:27:13.000000 dtstools-0.0.7/src/dtstools.egg-info/SOURCES.txt
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)        1 2023-07-09 14:27:13.000000 dtstools-0.0.7/src/dtstools.egg-info/dependency_links.txt
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)        9 2023-07-09 14:27:13.000000 dtstools-0.0.7/src/dtstools.egg-info/top_level.txt
```

### Comparing `dtstools-0.0.6/LICENSE` & `dtstools-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dtstools-0.0.6/PKG-INFO` & `dtstools-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtstools
-Version: 0.0.6
+Version: 0.0.7
 Summary: This package aims to provide features for working with Delta Lake.
 Author-email: Reginaldo Silva <reginaldo.silva@dataside.com.br>
 License: MIT License
         
         Copyright (c) 2023 Reginaldo Silva
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -48,16 +48,16 @@
     <img alt="Slack" src="https://img.shields.io/badge/Slack-Chat-e01e5a?logo=slack&logoColor=white&style=for-the-badge" />
   </a>
   <a href="https://github.com/reginaldosilva27/dtstools" title="GitHub" target="_blank">
     <img alt="GitHub" src="https://img.shields.io/badge/Mirror-GitHub-333333?logo=github&style=for-the-badge" />
   </a>
 </div>
 <div align="center">
-  <a title="Version: 0.0.6" href="https://github.com/reginaldosilva27/dtstools" target="_blank">
-    <img alt="Version: 0.0.6" src="https://img.shields.io/badge/version-0.0.6-blue.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgAQMAAABJtOi3AAAABlBMVEUAAAD///+l2Z/dAAAAAXRSTlMAQObYZgAAACNJREFUCNdjIACY//+BEp9hhM3hAzYQwoBIAqEDYQrCZLwAAGlFKxU1nF9cAAAAAElFTkSuQmCC&cacheSeconds=2592000&style=flat-square" />
+  <a title="Version: 0.0.7" href="https://github.com/reginaldosilva27/dtstools" target="_blank">
+    <img alt="Version: 0.0.7" src="https://img.shields.io/badge/version-0.0.7-blue.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgAQMAAABJtOi3AAAABlBMVEUAAAD///+l2Z/dAAAAAXRSTlMAQObYZgAAACNJREFUCNdjIACY//+BEp9hhM3hAzYQwoBIAqEDYQrCZLwAAGlFKxU1nF9cAAAAAElFTkSuQmCC&cacheSeconds=2592000&style=flat-square" />
   </a>
     <a title="License: MIT" href="https://github.com/reginaldosilva27/dtstools" target="_blank">
     <img alt="License: MIT" src="https://img.shields.io/badge/license-MIT-yellow.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgAQMAAABJtOi3AAAABlBMVEUAAAD///+l2Z/dAAAAAXRSTlMAQObYZgAAAHpJREFUCNdjYOD/wMDAUP+PgYHxhzwDA/MB5gMM7AwMDxj4GBgKGGQYGCyAEEgbMDDwAAWAwmk8958xpIOI5zKH2RmOyhxmZjguAiKmgIgtQOIYmFgCIp4AlaQ9OczGkJYCJEAGgI0CGwo2HmwR2Eqw5SBnNIAdBHYaAJb6KLM15W/CAAAAAElFTkSuQmCC&style=flat-square" />
   </a>
     <a href="Spark" title="Platform" target="_blank">
     <img alt="GitLab" src="https://img.shields.io/badge/platform-spark-red" />
   </a>
@@ -98,15 +98,15 @@
 <a href="#introducion" style="width:100%"><img style="width:100%" src="https://static.wixstatic.com/media/a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png" /></a>
 
 ## Introduction
 
 | version | date | description |
 |-----------|-------|----------|
 | `v0.0.4` | 2023-06-17 | Basic features |
-| `v0.0.6` | 2023-07-06 | Introduce lastMaintenance function |
+| `v0.0.7` | 2023-07-06 | Introduce lastMaintenance function |
 
 > This package aims to provide functionality to work with Delta Lake.
 >
 > Facilitating the visualization of the actual size (Storage) of your Delta tables and their maintenance (Vacuum and Optimize)
 
 > Below are the steps performed in order of execution:
 1. Executed a **describe detail** to get the current location and size
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dtstools Version: 0.0.6 Summary: This package aims
+Metadata-Version: 2.1 Name: dtstools Version: 0.0.7 Summary: This package aims
 to provide features for working with Delta Lake. Author-email: Reginaldo Silva
 silva@dataside.com.br> License: MIT License Copyright (c) 2023 Reginaldo Silva
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
@@ -19,15 +19,15 @@
 reginaldosilva27/dtstools Project-URL: README, https://www.datainaction.dev/
 blog Project-URL: Dataside, https://www.dataside.com.br Keywords:
 tableSize,tableMaintenance,help,deltaLake,Spark,Databricks,Fabric Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
                   [Homepage] [Contributing] [Slack] [GitHub]
-                   [Version:_0.0.6] [License:_MIT] [GitLab]
+                   [Version:_0.0.7] [License:_MIT] [GitLab]
 [https://static.wixstatic.com/media/
 a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]
                      DTSTOOLS: Help with your Delta Lake
                    *** Library created by Data_In_Action ***
 ``` ##### ###### ##### ###### ### ### #### ##### ## ## ## ## ## ## ## ## ## ##
 ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ##### ## ## ## ## ## ##
 ##### ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ##
@@ -36,15 +36,15 @@
 [Introduction](#introducion) - [How to use dtstools](#how-to-use-dtstools) -
 [How to use tableSize](#how-to-use-tableSize) - [How to use tableMaintenance]
 (#how-to-use-tableMaintenance) - [How to use LastMaintenance](#last-
 maintenance) - [Future implementations](#future-implementations) - [Notes]
 (#notes) - [References](#references) [https://static.wixstatic.com/media/
 a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png] ## Introduction | version |
 date | description | |-----------|-------|----------| | `v0.0.4` | 2023-06-17 |
-Basic features | | `v0.0.6` | 2023-07-06 | Introduce lastMaintenance function |
+Basic features | | `v0.0.7` | 2023-07-06 | Introduce lastMaintenance function |
 > This package aims to provide functionality to work with Delta Lake. > >
 Facilitating the visualization of the actual size (Storage) of your Delta
 tables and their maintenance (Vacuum and Optimize) > Below are the steps
 performed in order of execution: 1. Executed a **describe detail** to get the
 current location and size 2. A scan (dbutils.fs.ls) is performed on the Storage
 folders recursively to calculate the space used in the Storage, excluding the
 _delta_logs, with this we can calculate an average of how much can be released
```

### Comparing `dtstools-0.0.6/README.md` & `dtstools-0.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
     <img alt="Slack" src="https://img.shields.io/badge/Slack-Chat-e01e5a?logo=slack&logoColor=white&style=for-the-badge" />
   </a>
   <a href="https://github.com/reginaldosilva27/dtstools" title="GitHub" target="_blank">
     <img alt="GitHub" src="https://img.shields.io/badge/Mirror-GitHub-333333?logo=github&style=for-the-badge" />
   </a>
 </div>
 <div align="center">
-  <a title="Version: 0.0.6" href="https://github.com/reginaldosilva27/dtstools" target="_blank">
-    <img alt="Version: 0.0.6" src="https://img.shields.io/badge/version-0.0.6-blue.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgAQMAAABJtOi3AAAABlBMVEUAAAD///+l2Z/dAAAAAXRSTlMAQObYZgAAACNJREFUCNdjIACY//+BEp9hhM3hAzYQwoBIAqEDYQrCZLwAAGlFKxU1nF9cAAAAAElFTkSuQmCC&cacheSeconds=2592000&style=flat-square" />
+  <a title="Version: 0.0.7" href="https://github.com/reginaldosilva27/dtstools" target="_blank">
+    <img alt="Version: 0.0.7" src="https://img.shields.io/badge/version-0.0.7-blue.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgAQMAAABJtOi3AAAABlBMVEUAAAD///+l2Z/dAAAAAXRSTlMAQObYZgAAACNJREFUCNdjIACY//+BEp9hhM3hAzYQwoBIAqEDYQrCZLwAAGlFKxU1nF9cAAAAAElFTkSuQmCC&cacheSeconds=2592000&style=flat-square" />
   </a>
     <a title="License: MIT" href="https://github.com/reginaldosilva27/dtstools" target="_blank">
     <img alt="License: MIT" src="https://img.shields.io/badge/license-MIT-yellow.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgAQMAAABJtOi3AAAABlBMVEUAAAD///+l2Z/dAAAAAXRSTlMAQObYZgAAAHpJREFUCNdjYOD/wMDAUP+PgYHxhzwDA/MB5gMM7AwMDxj4GBgKGGQYGCyAEEgbMDDwAAWAwmk8958xpIOI5zKH2RmOyhxmZjguAiKmgIgtQOIYmFgCIp4AlaQ9OczGkJYCJEAGgI0CGwo2HmwR2Eqw5SBnNIAdBHYaAJb6KLM15W/CAAAAAElFTkSuQmCC&style=flat-square" />
   </a>
     <a href="Spark" title="Platform" target="_blank">
     <img alt="GitLab" src="https://img.shields.io/badge/platform-spark-red" />
   </a>
@@ -59,15 +59,15 @@
 <a href="#introducion" style="width:100%"><img style="width:100%" src="https://static.wixstatic.com/media/a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png" /></a>
 
 ## Introduction
 
 | version | date | description |
 |-----------|-------|----------|
 | `v0.0.4` | 2023-06-17 | Basic features |
-| `v0.0.6` | 2023-07-06 | Introduce lastMaintenance function |
+| `v0.0.7` | 2023-07-06 | Introduce lastMaintenance function |
 
 > This package aims to provide functionality to work with Delta Lake.
 >
 > Facilitating the visualization of the actual size (Storage) of your Delta tables and their maintenance (Vacuum and Optimize)
 
 > Below are the steps performed in order of execution:
 1. Executed a **describe detail** to get the current location and size
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
                   [Homepage] [Contributing] [Slack] [GitHub]
-                   [Version:_0.0.6] [License:_MIT] [GitLab]
+                   [Version:_0.0.7] [License:_MIT] [GitLab]
 [https://static.wixstatic.com/media/
 a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]
                      DTSTOOLS: Help with your Delta Lake
                    *** Library created by Data_In_Action ***
 ``` ##### ###### ##### ###### ### ### #### ##### ## ## ## ## ## ## ## ## ## ##
 ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ##### ## ## ## ## ## ##
 ##### ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ##
@@ -12,15 +12,15 @@
 [Introduction](#introducion) - [How to use dtstools](#how-to-use-dtstools) -
 [How to use tableSize](#how-to-use-tableSize) - [How to use tableMaintenance]
 (#how-to-use-tableMaintenance) - [How to use LastMaintenance](#last-
 maintenance) - [Future implementations](#future-implementations) - [Notes]
 (#notes) - [References](#references) [https://static.wixstatic.com/media/
 a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png] ## Introduction | version |
 date | description | |-----------|-------|----------| | `v0.0.4` | 2023-06-17 |
-Basic features | | `v0.0.6` | 2023-07-06 | Introduce lastMaintenance function |
+Basic features | | `v0.0.7` | 2023-07-06 | Introduce lastMaintenance function |
 > This package aims to provide functionality to work with Delta Lake. > >
 Facilitating the visualization of the actual size (Storage) of your Delta
 tables and their maintenance (Vacuum and Optimize) > Below are the steps
 performed in order of execution: 1. Executed a **describe detail** to get the
 current location and size 2. A scan (dbutils.fs.ls) is performed on the Storage
 folders recursively to calculate the space used in the Storage, excluding the
 _delta_logs, with this we can calculate an average of how much can be released
```

### Comparing `dtstools-0.0.6/pyproject.toml` & `dtstools-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dtstools"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Reginaldo Silva", email="reginaldo.silva@dataside.com.br" },
 ]
 description = "This package aims to provide features for working with Delta Lake."
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
```

### Comparing `dtstools-0.0.6/src/dtstools/dtsTable.py` & `dtstools-0.0.7/src/dtstools/dtsTable.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,29 +133,29 @@
         spark.sql(f"describe history {database}.{tableName}").createOrReplaceTempView("vwMaintenance")
         df_return = spark.sql("""
             Select 
             replace(op.operation,'VACUUM START','VACUUM') operation, 
             NVL(his.earliest,'Never') earliest, 
             NVL(his.oldest,'Never') oldest, 
             NVL(his.ocurrences,0) ocurrences, 
-            NVL(his.frequency,'No schedule') frequency,
+            NVL(his.estimated_frequency,'No schedule') estimated_frequency,
             NVL(his.params,0) params,
             NVL(his.metrics,'None') metrics
             from (
                 Select 'VACUUM START' as operation Union All
                 Select 'OPTIMIZE' 
             ) op left join
             (
             select 
                 operation,
                 max(timestamp) earliest,
                 min(timestamp) oldest,
                 count(*) ocurrences , 
-                concat("average ",ABS(int(round(date_diff(max(timestamp),min(timestamp)) / count(*),0))),"xday") frequency,
-                case when operation in('VACUUM START') then Concat('retentionHours - ',int(last(operationParameters.specifiedRetentionMillis) / 1000 / 60 / 60)) 
+                concat("every ",IF(ABS(int(round(date_diff(max(timestamp),min(timestamp)) / count(*),0))) = 0,1,ABS(int(round(date_diff(max(timestamp),min(timestamp)) / count(*),0))))," days") estimated_frequency
+                case when operation in('VACUUM START') then Concat('retentionHours - ',int(NVL(last(operationParameters.specifiedRetentionMillis),last(operationParameters.defaultRetentionMillis)) / 1000 / 60 / 60)) 
                     when operation in('OPTIMIZE') then Concat('zOrderBy - ',last(operationParameters.zOrderBy)) 
                     else 'None' end params,
                 case when operation in('VACUUM START') then Concat('TotalDeletedFiles - ',sum(bigint(operationMetrics.numFilesToDelete)),' - TotalRemovedSizeGB - ',round(sum(bigint(operationMetrics.sizeOfDataToDelete)) / 1024 / 1024 / 1024,2)) 
                     when operation in('OPTIMIZE') then Concat('TotalRemovedFiles - ',sum(bigint(operationMetrics.numRemovedFiles)),' - TotalnumAddedFiles - ',round(sum(bigint(operationMetrics.numAddedFiles)))) 
                     else 'None' end metrics
             from vwMaintenance where operation in ('VACUUM START','OPTIMIZE')
             group by operation
@@ -164,15 +164,15 @@
         df_return.withColumn('dateLog',lit(f'{datetime.today()}')).display()
     except Exception as e:
         print(f"###### Error to load tableName {tableName} - {e}######")
 
 
 # Function to get help about
 def Help():
-    print("v0.0.6")
+    print("v0.0.7")
     print("""____  ______ __ ______  ___    ___  __    __  """)
     print('|| \\\\ | || |(( \| || | // \\\\  // \\\\ ||   (( \ ')
     print("""||  ))  ||   \\\\   ||  ((   ))((   ))||    \\\\  """)
     print("""||_//   ||  \_))  ||   \\\\_//  \\\\_// ||__|\_)) """)
     print("")
     print("------------------------------------------------------")
     print("Function tableSize(database, tableName)")
```

### Comparing `dtstools-0.0.6/src/dtstools.egg-info/PKG-INFO` & `dtstools-0.0.7/src/dtstools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtstools
-Version: 0.0.6
+Version: 0.0.7
 Summary: This package aims to provide features for working with Delta Lake.
 Author-email: Reginaldo Silva <reginaldo.silva@dataside.com.br>
 License: MIT License
         
         Copyright (c) 2023 Reginaldo Silva
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -48,16 +48,16 @@
     <img alt="Slack" src="https://img.shields.io/badge/Slack-Chat-e01e5a?logo=slack&logoColor=white&style=for-the-badge" />
   </a>
   <a href="https://github.com/reginaldosilva27/dtstools" title="GitHub" target="_blank">
     <img alt="GitHub" src="https://img.shields.io/badge/Mirror-GitHub-333333?logo=github&style=for-the-badge" />
   </a>
 </div>
 <div align="center">
-  <a title="Version: 0.0.6" href="https://github.com/reginaldosilva27/dtstools" target="_blank">
-    <img alt="Version: 0.0.6" src="https://img.shields.io/badge/version-0.0.6-blue.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgAQMAAABJtOi3AAAABlBMVEUAAAD///+l2Z/dAAAAAXRSTlMAQObYZgAAACNJREFUCNdjIACY//+BEp9hhM3hAzYQwoBIAqEDYQrCZLwAAGlFKxU1nF9cAAAAAElFTkSuQmCC&cacheSeconds=2592000&style=flat-square" />
+  <a title="Version: 0.0.7" href="https://github.com/reginaldosilva27/dtstools" target="_blank">
+    <img alt="Version: 0.0.7" src="https://img.shields.io/badge/version-0.0.7-blue.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgAQMAAABJtOi3AAAABlBMVEUAAAD///+l2Z/dAAAAAXRSTlMAQObYZgAAACNJREFUCNdjIACY//+BEp9hhM3hAzYQwoBIAqEDYQrCZLwAAGlFKxU1nF9cAAAAAElFTkSuQmCC&cacheSeconds=2592000&style=flat-square" />
   </a>
     <a title="License: MIT" href="https://github.com/reginaldosilva27/dtstools" target="_blank">
     <img alt="License: MIT" src="https://img.shields.io/badge/license-MIT-yellow.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgAQMAAABJtOi3AAAABlBMVEUAAAD///+l2Z/dAAAAAXRSTlMAQObYZgAAAHpJREFUCNdjYOD/wMDAUP+PgYHxhzwDA/MB5gMM7AwMDxj4GBgKGGQYGCyAEEgbMDDwAAWAwmk8958xpIOI5zKH2RmOyhxmZjguAiKmgIgtQOIYmFgCIp4AlaQ9OczGkJYCJEAGgI0CGwo2HmwR2Eqw5SBnNIAdBHYaAJb6KLM15W/CAAAAAElFTkSuQmCC&style=flat-square" />
   </a>
     <a href="Spark" title="Platform" target="_blank">
     <img alt="GitLab" src="https://img.shields.io/badge/platform-spark-red" />
   </a>
@@ -98,15 +98,15 @@
 <a href="#introducion" style="width:100%"><img style="width:100%" src="https://static.wixstatic.com/media/a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png" /></a>
 
 ## Introduction
 
 | version | date | description |
 |-----------|-------|----------|
 | `v0.0.4` | 2023-06-17 | Basic features |
-| `v0.0.6` | 2023-07-06 | Introduce lastMaintenance function |
+| `v0.0.7` | 2023-07-06 | Introduce lastMaintenance function |
 
 > This package aims to provide functionality to work with Delta Lake.
 >
 > Facilitating the visualization of the actual size (Storage) of your Delta tables and their maintenance (Vacuum and Optimize)
 
 > Below are the steps performed in order of execution:
 1. Executed a **describe detail** to get the current location and size
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dtstools Version: 0.0.6 Summary: This package aims
+Metadata-Version: 2.1 Name: dtstools Version: 0.0.7 Summary: This package aims
 to provide features for working with Delta Lake. Author-email: Reginaldo Silva
 silva@dataside.com.br> License: MIT License Copyright (c) 2023 Reginaldo Silva
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
@@ -19,15 +19,15 @@
 reginaldosilva27/dtstools Project-URL: README, https://www.datainaction.dev/
 blog Project-URL: Dataside, https://www.dataside.com.br Keywords:
 tableSize,tableMaintenance,help,deltaLake,Spark,Databricks,Fabric Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
                   [Homepage] [Contributing] [Slack] [GitHub]
-                   [Version:_0.0.6] [License:_MIT] [GitLab]
+                   [Version:_0.0.7] [License:_MIT] [GitLab]
 [https://static.wixstatic.com/media/
 a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]
                      DTSTOOLS: Help with your Delta Lake
                    *** Library created by Data_In_Action ***
 ``` ##### ###### ##### ###### ### ### #### ##### ## ## ## ## ## ## ## ## ## ##
 ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ##### ## ## ## ## ## ##
 ##### ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ##
@@ -36,15 +36,15 @@
 [Introduction](#introducion) - [How to use dtstools](#how-to-use-dtstools) -
 [How to use tableSize](#how-to-use-tableSize) - [How to use tableMaintenance]
 (#how-to-use-tableMaintenance) - [How to use LastMaintenance](#last-
 maintenance) - [Future implementations](#future-implementations) - [Notes]
 (#notes) - [References](#references) [https://static.wixstatic.com/media/
 a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png] ## Introduction | version |
 date | description | |-----------|-------|----------| | `v0.0.4` | 2023-06-17 |
-Basic features | | `v0.0.6` | 2023-07-06 | Introduce lastMaintenance function |
+Basic features | | `v0.0.7` | 2023-07-06 | Introduce lastMaintenance function |
 > This package aims to provide functionality to work with Delta Lake. > >
 Facilitating the visualization of the actual size (Storage) of your Delta
 tables and their maintenance (Vacuum and Optimize) > Below are the steps
 performed in order of execution: 1. Executed a **describe detail** to get the
 current location and size 2. A scan (dbutils.fs.ls) is performed on the Storage
 folders recursively to calculate the space used in the Storage, excluding the
 _delta_logs, with this we can calculate an average of how much can be released
```

