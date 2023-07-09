# Comparing `tmp/increment-1.3.3.tar.gz` & `tmp/increment-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "increment-1.3.3.tar", last modified: Tue Jun 13 15:50:55 2023, max compression
+gzip compressed data, was "increment-1.3.4.tar", last modified: Sun Jul  9 06:53:47 2023, max compression
```

## Comparing `increment-1.3.3.tar` & `increment-1.3.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 increment-1.3.3/LICENSE
--rw-r--r--   0        0        0     1824 2023-06-13 15:29:36.474108 increment-1.3.3/README.md
--rw-r--r--   0        0        0       29 2023-04-10 04:01:47.110396 increment-1.3.3/increment.py
--rw-r--r--   0        0        0      608 2023-06-13 15:50:51.747320 increment-1.3.3/pyproject.toml
--rw-r--r--   0        0        0     2200 1970-01-01 00:00:00.000000 increment-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-07-09 05:47:26.656963 increment-1.3.4/LICENSE
+-rw-r--r--   0        0        0     1218 2023-07-09 05:44:41.558583 increment-1.3.4/README.md
+-rw-r--r--   0        0        0       29 2023-04-10 04:01:47.110396 increment-1.3.4/increment.py
+-rw-r--r--   0        0        0      610 2023-07-09 06:53:41.700858 increment-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 increment-1.3.4/PKG-INFO
```

### Comparing `increment-1.3.3/LICENSE` & `increment-1.3.4/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
       defend, and hold each Contributor harmless for any liability
       incurred by, or claims asserted against, such Contributor by reason
       of your accepting any such warranty or additional liability.
 
    END OF TERMS AND CONDITIONS
    
 
-   Copyright [2023] [许灿标]
+   Copyright [2023] [lcctoor.com]
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `increment-1.3.3/pyproject.toml` & `increment-1.3.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "increment"
-version = "1.3.3"
+version = "1.3.4"
 description = "分布式主键生成器，支持多机器|多进程|多线程并发生成"
 dependencies = ["lccpy >=1.4.7"]
 keywords = ["increment"]
 
 readme = "README.md"
-authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
+authors = [{name = "lcctoor.com", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
 
 [project.urls]
 HomePage = "https://github.com/lcctoor/lccpy/tree/main/packages/increment#readme"
```

