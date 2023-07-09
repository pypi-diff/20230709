# Comparing `tmp/dtstools-0.0.7.tar.gz` & `tmp/dtstools-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtstools-0.0.7.tar", last modified: Sun Jul  9 14:27:13 2023, max compression
+gzip compressed data, was "dtstools-0.0.8.tar", last modified: Sun Jul  9 14:32:39 2023, max compression
```

## Comparing `dtstools-0.0.7.tar` & `dtstools-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 reginaldosilva   (501) staff       (20)        0 2023-07-09 14:27:13.746198 dtstools-0.0.7/
--rw-r--r--   0 reginaldosilva   (501) staff       (20)     1072 2023-06-17 11:23:10.000000 dtstools-0.0.7/LICENSE
--rw-r--r--   0 reginaldosilva   (501) staff       (20)    11384 2023-07-09 14:27:13.745690 dtstools-0.0.7/PKG-INFO
--rw-r--r--   0 reginaldosilva   (501) staff       (20)     9395 2023-07-09 14:20:50.000000 dtstools-0.0.7/README.md
--rw-r--r--   0 reginaldosilva   (501) staff       (20)      865 2023-07-09 14:20:55.000000 dtstools-0.0.7/pyproject.toml
--rw-r--r--   0 reginaldosilva   (501) staff       (20)       38 2023-07-09 14:27:13.746355 dtstools-0.0.7/setup.cfg
-drwxr-xr-x   0 reginaldosilva   (501) staff       (20)        0 2023-07-09 14:27:13.739888 dtstools-0.0.7/src/
-drwxr-xr-x   0 reginaldosilva   (501) staff       (20)        0 2023-07-09 14:27:13.742288 dtstools-0.0.7/src/dtstools/
--rw-r--r--   0 reginaldosilva   (501) staff       (20)        0 2023-06-09 17:32:34.000000 dtstools-0.0.7/src/dtstools/__init__.py
--rw-r--r--   0 reginaldosilva   (501) staff       (20)    10653 2023-07-09 14:22:23.000000 dtstools-0.0.7/src/dtstools/dtsTable.py
-drwxr-xr-x   0 reginaldosilva   (501) staff       (20)        0 2023-07-09 14:27:13.744922 dtstools-0.0.7/src/dtstools.egg-info/
--rw-r--r--   0 reginaldosilva   (501) staff       (20)    11384 2023-07-09 14:27:13.000000 dtstools-0.0.7/src/dtstools.egg-info/PKG-INFO
--rw-r--r--   0 reginaldosilva   (501) staff       (20)      226 2023-07-09 14:27:13.000000 dtstools-0.0.7/src/dtstools.egg-info/SOURCES.txt
--rw-r--r--   0 reginaldosilva   (501) staff       (20)        1 2023-07-09 14:27:13.000000 dtstools-0.0.7/src/dtstools.egg-info/dependency_links.txt
--rw-r--r--   0 reginaldosilva   (501) staff       (20)        9 2023-07-09 14:27:13.000000 dtstools-0.0.7/src/dtstools.egg-info/top_level.txt
+drwxr-xr-x   0 reginaldosilva   (501) staff       (20)        0 2023-07-09 14:32:39.885433 dtstools-0.0.8/
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)     1072 2023-06-17 11:23:10.000000 dtstools-0.0.8/LICENSE
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)    11384 2023-07-09 14:32:39.884881 dtstools-0.0.8/PKG-INFO
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)     9395 2023-07-09 14:32:07.000000 dtstools-0.0.8/README.md
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)      865 2023-07-09 14:32:11.000000 dtstools-0.0.8/pyproject.toml
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)       38 2023-07-09 14:32:39.885571 dtstools-0.0.8/setup.cfg
+drwxr-xr-x   0 reginaldosilva   (501) staff       (20)        0 2023-07-09 14:32:39.880105 dtstools-0.0.8/src/
+drwxr-xr-x   0 reginaldosilva   (501) staff       (20)        0 2023-07-09 14:32:39.882003 dtstools-0.0.8/src/dtstools/
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)        0 2023-06-09 17:32:34.000000 dtstools-0.0.8/src/dtstools/__init__.py
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)    10654 2023-07-09 14:32:19.000000 dtstools-0.0.8/src/dtstools/dtsTable.py
+drwxr-xr-x   0 reginaldosilva   (501) staff       (20)        0 2023-07-09 14:32:39.884139 dtstools-0.0.8/src/dtstools.egg-info/
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)    11384 2023-07-09 14:32:39.000000 dtstools-0.0.8/src/dtstools.egg-info/PKG-INFO
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)      226 2023-07-09 14:32:39.000000 dtstools-0.0.8/src/dtstools.egg-info/SOURCES.txt
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)        1 2023-07-09 14:32:39.000000 dtstools-0.0.8/src/dtstools.egg-info/dependency_links.txt
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)        9 2023-07-09 14:32:39.000000 dtstools-0.0.8/src/dtstools.egg-info/top_level.txt
```

### Comparing `dtstools-0.0.7/LICENSE` & `dtstools-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dtstools-0.0.7/PKG-INFO` & `dtstools-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtstools
-Version: 0.0.7
+Version: 0.0.8
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
-  <a title="Version: 0.0.7" href="https://github.com/reginaldosilva27/dtstools" target="_blank">
-    <img alt="Version: 0.0.7" src="https://img.shields.io/badge/version-0.0.7-blue.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgAQMAAABJtOi3AAAABlBMVEUAAAD///+l2Z/dAAAAAXRSTlMAQObYZgAAACNJREFUCNdjIACY//+BEp9hhM3hAzYQwoBIAqEDYQrCZLwAAGlFKxU1nF9cAAAAAElFTkSuQmCC&cacheSeconds=2592000&style=flat-square" />
+  <a title="Version: 0.0.8" href="https://github.com/reginaldosilva27/dtstools" target="_blank">
+    <img alt="Version: 0.0.8" src="https://img.shields.io/badge/version-0.0.8-blue.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgAQMAAABJtOi3AAAABlBMVEUAAAD///+l2Z/dAAAAAXRSTlMAQObYZgAAACNJREFUCNdjIACY//+BEp9hhM3hAzYQwoBIAqEDYQrCZLwAAGlFKxU1nF9cAAAAAElFTkSuQmCC&cacheSeconds=2592000&style=flat-square" />
   </a>
     <a title="License: MIT" href="https://github.com/reginaldosilva27/dtstools" target="_blank">
     <img alt="License: MIT" src="https://img.shields.io/badge/license-MIT-yellow.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgAQMAAABJtOi3AAAABlBMVEUAAAD///+l2Z/dAAAAAXRSTlMAQObYZgAAAHpJREFUCNdjYOD/wMDAUP+PgYHxhzwDA/MB5gMM7AwMDxj4GBgKGGQYGCyAEEgbMDDwAAWAwmk8958xpIOI5zKH2RmOyhxmZjguAiKmgIgtQOIYmFgCIp4AlaQ9OczGkJYCJEAGgI0CGwo2HmwR2Eqw5SBnNIAdBHYaAJb6KLM15W/CAAAAAElFTkSuQmCC&style=flat-square" />
   </a>
     <a href="Spark" title="Platform" target="_blank">
     <img alt="GitLab" src="https://img.shields.io/badge/platform-spark-red" />
   </a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dtstools Version: 0.0.7 Summary: This package aims
+Metadata-Version: 2.1 Name: dtstools Version: 0.0.8 Summary: This package aims
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
-                   [Version:_0.0.7] [License:_MIT] [GitLab]
+                   [Version:_0.0.8] [License:_MIT] [GitLab]
 [https://static.wixstatic.com/media/
 a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]
                      DTSTOOLS: Help with your Delta Lake
                    *** Library created by Data_In_Action ***
 ``` ##### ###### ##### ###### ### ### #### ##### ## ## ## ## ## ## ## ## ## ##
 ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ##### ## ## ## ## ## ##
 ##### ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ##
```

### Comparing `dtstools-0.0.7/README.md` & `dtstools-0.0.8/README.md`

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
-  <a title="Version: 0.0.7" href="https://github.com/reginaldosilva27/dtstools" target="_blank">
-    <img alt="Version: 0.0.7" src="https://img.shields.io/badge/version-0.0.7-blue.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgAQMAAABJtOi3AAAABlBMVEUAAAD///+l2Z/dAAAAAXRSTlMAQObYZgAAACNJREFUCNdjIACY//+BEp9hhM3hAzYQwoBIAqEDYQrCZLwAAGlFKxU1nF9cAAAAAElFTkSuQmCC&cacheSeconds=2592000&style=flat-square" />
+  <a title="Version: 0.0.8" href="https://github.com/reginaldosilva27/dtstools" target="_blank">
+    <img alt="Version: 0.0.8" src="https://img.shields.io/badge/version-0.0.8-blue.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgAQMAAABJtOi3AAAABlBMVEUAAAD///+l2Z/dAAAAAXRSTlMAQObYZgAAACNJREFUCNdjIACY//+BEp9hhM3hAzYQwoBIAqEDYQrCZLwAAGlFKxU1nF9cAAAAAElFTkSuQmCC&cacheSeconds=2592000&style=flat-square" />
   </a>
     <a title="License: MIT" href="https://github.com/reginaldosilva27/dtstools" target="_blank">
     <img alt="License: MIT" src="https://img.shields.io/badge/license-MIT-yellow.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgAQMAAABJtOi3AAAABlBMVEUAAAD///+l2Z/dAAAAAXRSTlMAQObYZgAAAHpJREFUCNdjYOD/wMDAUP+PgYHxhzwDA/MB5gMM7AwMDxj4GBgKGGQYGCyAEEgbMDDwAAWAwmk8958xpIOI5zKH2RmOyhxmZjguAiKmgIgtQOIYmFgCIp4AlaQ9OczGkJYCJEAGgI0CGwo2HmwR2Eqw5SBnNIAdBHYaAJb6KLM15W/CAAAAAElFTkSuQmCC&style=flat-square" />
   </a>
     <a href="Spark" title="Platform" target="_blank">
     <img alt="GitLab" src="https://img.shields.io/badge/platform-spark-red" />
   </a>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
                   [Homepage] [Contributing] [Slack] [GitHub]
-                   [Version:_0.0.7] [License:_MIT] [GitLab]
+                   [Version:_0.0.8] [License:_MIT] [GitLab]
 [https://static.wixstatic.com/media/
 a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]
                      DTSTOOLS: Help with your Delta Lake
                    *** Library created by Data_In_Action ***
 ``` ##### ###### ##### ###### ### ### #### ##### ## ## ## ## ## ## ## ## ## ##
 ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ##### ## ## ## ## ## ##
 ##### ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ##
```

### Comparing `dtstools-0.0.7/pyproject.toml` & `dtstools-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dtstools"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Reginaldo Silva", email="reginaldo.silva@dataside.com.br" },
 ]
 description = "This package aims to provide features for working with Delta Lake."
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
```

### Comparing `dtstools-0.0.7/src/dtstools/dtsTable.py` & `dtstools-0.0.8/src/dtstools/dtsTable.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
             ) op left join
             (
             select 
                 operation,
                 max(timestamp) earliest,
                 min(timestamp) oldest,
                 count(*) ocurrences , 
-                concat("every ",IF(ABS(int(round(date_diff(max(timestamp),min(timestamp)) / count(*),0))) = 0,1,ABS(int(round(date_diff(max(timestamp),min(timestamp)) / count(*),0))))," days") estimated_frequency
+                concat("every ",IF(ABS(int(round(date_diff(max(timestamp),min(timestamp)) / count(*),0))) = 0,1,ABS(int(round(date_diff(max(timestamp),min(timestamp)) / count(*),0))))," days") estimated_frequency,
                 case when operation in('VACUUM START') then Concat('retentionHours - ',int(NVL(last(operationParameters.specifiedRetentionMillis),last(operationParameters.defaultRetentionMillis)) / 1000 / 60 / 60)) 
                     when operation in('OPTIMIZE') then Concat('zOrderBy - ',last(operationParameters.zOrderBy)) 
                     else 'None' end params,
                 case when operation in('VACUUM START') then Concat('TotalDeletedFiles - ',sum(bigint(operationMetrics.numFilesToDelete)),' - TotalRemovedSizeGB - ',round(sum(bigint(operationMetrics.sizeOfDataToDelete)) / 1024 / 1024 / 1024,2)) 
                     when operation in('OPTIMIZE') then Concat('TotalRemovedFiles - ',sum(bigint(operationMetrics.numRemovedFiles)),' - TotalnumAddedFiles - ',round(sum(bigint(operationMetrics.numAddedFiles)))) 
                     else 'None' end metrics
             from vwMaintenance where operation in ('VACUUM START','OPTIMIZE')
@@ -164,15 +164,15 @@
         df_return.withColumn('dateLog',lit(f'{datetime.today()}')).display()
     except Exception as e:
         print(f"###### Error to load tableName {tableName} - {e}######")
 
 
 # Function to get help about
 def Help():
-    print("v0.0.7")
+    print("v0.0.8")
     print("""____  ______ __ ______  ___    ___  __    __  """)
     print('|| \\\\ | || |(( \| || | // \\\\  // \\\\ ||   (( \ ')
     print("""||  ))  ||   \\\\   ||  ((   ))((   ))||    \\\\  """)
     print("""||_//   ||  \_))  ||   \\\\_//  \\\\_// ||__|\_)) """)
     print("")
     print("------------------------------------------------------")
     print("Function tableSize(database, tableName)")
```

### Comparing `dtstools-0.0.7/src/dtstools.egg-info/PKG-INFO` & `dtstools-0.0.8/src/dtstools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtstools
-Version: 0.0.7
+Version: 0.0.8
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
-  <a title="Version: 0.0.7" href="https://github.com/reginaldosilva27/dtstools" target="_blank">
-    <img alt="Version: 0.0.7" src="https://img.shields.io/badge/version-0.0.7-blue.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgAQMAAABJtOi3AAAABlBMVEUAAAD///+l2Z/dAAAAAXRSTlMAQObYZgAAACNJREFUCNdjIACY//+BEp9hhM3hAzYQwoBIAqEDYQrCZLwAAGlFKxU1nF9cAAAAAElFTkSuQmCC&cacheSeconds=2592000&style=flat-square" />
+  <a title="Version: 0.0.8" href="https://github.com/reginaldosilva27/dtstools" target="_blank">
+    <img alt="Version: 0.0.8" src="https://img.shields.io/badge/version-0.0.8-blue.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgAQMAAABJtOi3AAAABlBMVEUAAAD///+l2Z/dAAAAAXRSTlMAQObYZgAAACNJREFUCNdjIACY//+BEp9hhM3hAzYQwoBIAqEDYQrCZLwAAGlFKxU1nF9cAAAAAElFTkSuQmCC&cacheSeconds=2592000&style=flat-square" />
   </a>
     <a title="License: MIT" href="https://github.com/reginaldosilva27/dtstools" target="_blank">
     <img alt="License: MIT" src="https://img.shields.io/badge/license-MIT-yellow.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgAQMAAABJtOi3AAAABlBMVEUAAAD///+l2Z/dAAAAAXRSTlMAQObYZgAAAHpJREFUCNdjYOD/wMDAUP+PgYHxhzwDA/MB5gMM7AwMDxj4GBgKGGQYGCyAEEgbMDDwAAWAwmk8958xpIOI5zKH2RmOyhxmZjguAiKmgIgtQOIYmFgCIp4AlaQ9OczGkJYCJEAGgI0CGwo2HmwR2Eqw5SBnNIAdBHYaAJb6KLM15W/CAAAAAElFTkSuQmCC&style=flat-square" />
   </a>
     <a href="Spark" title="Platform" target="_blank">
     <img alt="GitLab" src="https://img.shields.io/badge/platform-spark-red" />
   </a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dtstools Version: 0.0.7 Summary: This package aims
+Metadata-Version: 2.1 Name: dtstools Version: 0.0.8 Summary: This package aims
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
-                   [Version:_0.0.7] [License:_MIT] [GitLab]
+                   [Version:_0.0.8] [License:_MIT] [GitLab]
 [https://static.wixstatic.com/media/
 a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]
                      DTSTOOLS: Help with your Delta Lake
                    *** Library created by Data_In_Action ***
 ``` ##### ###### ##### ###### ### ### #### ##### ## ## ## ## ## ## ## ## ## ##
 ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ##### ## ## ## ## ## ##
 ##### ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ##
```

