# Comparing `tmp/hermite-function-0.9.9.tar.gz` & `tmp/hermite-function-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hermite-function-0.9.9.tar", last modified: Sun Jul  9 15:25:38 2023, max compression
+gzip compressed data, was "hermite-function-1.0.tar", last modified: Sun Jul  9 15:34:43 2023, max compression
```

## Comparing `hermite-function-0.9.9.tar` & `hermite-function-1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 15:25:38.975150 hermite-function-0.9.9/
--rw-rw-rw-   0        0        0     7237 2023-07-09 15:24:16.000000 hermite-function-0.9.9/HermiteFunction.py
--rw-rw-rw-   0        0        0     1073 2023-07-09 15:24:16.000000 hermite-function-0.9.9/LICENSE
--rw-rw-rw-   0        0        0     9732 2023-07-09 15:25:38.973702 hermite-function-0.9.9/PKG-INFO
--rw-rw-rw-   0        0        0     9006 2023-07-09 15:24:16.000000 hermite-function-0.9.9/README.md
-drwxrwxrwx   0        0        0        0 2023-07-09 15:25:38.972582 hermite-function-0.9.9/hermite_function.egg-info/
--rw-rw-rw-   0        0        0     9732 2023-07-09 15:25:38.000000 hermite-function-0.9.9/hermite_function.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-07-09 15:25:38.000000 hermite-function-0.9.9/hermite_function.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 15:25:38.000000 hermite-function-0.9.9/hermite_function.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-07-09 15:25:38.000000 hermite-function-0.9.9/hermite_function.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-09 15:25:38.000000 hermite-function-0.9.9/hermite_function.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-09 15:25:38.975797 hermite-function-0.9.9/setup.cfg
--rw-rw-rw-   0        0        0      837 2023-07-09 15:25:08.000000 hermite-function-0.9.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 15:34:43.132084 hermite-function-1.0/
+-rw-rw-rw-   0        0        0     1094 2022-12-12 09:43:07.000000 hermite-function-1.0/LICENSE
+-rw-rw-rw-   0        0        0     5098 2023-07-09 15:34:43.129076 hermite-function-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4617 2023-07-09 15:32:47.000000 hermite-function-1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 15:34:43.129076 hermite-function-1.0/hermite_function.egg-info/
+-rw-rw-rw-   0        0        0     5098 2023-07-09 15:34:43.000000 hermite-function-1.0/hermite_function.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-07-09 15:34:43.000000 hermite-function-1.0/hermite_function.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 15:34:43.000000 hermite-function-1.0/hermite_function.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-09 15:34:43.000000 hermite-function-1.0/hermite_function.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-09 15:34:43.000000 hermite-function-1.0/hermite_function.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4687 2023-07-09 15:31:04.000000 hermite-function-1.0/hermitefunction.py
+-rw-rw-rw-   0        0        0       42 2023-07-09 15:34:43.132855 hermite-function-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      845 2023-07-09 15:33:45.000000 hermite-function-1.0/setup.py
```

