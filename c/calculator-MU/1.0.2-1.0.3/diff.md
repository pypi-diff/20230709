# Comparing `tmp/calculator_MU-1.0.2.tar.gz` & `tmp/calculator_MU-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calculator_MU-1.0.2.tar", last modified: Sun Jul  9 15:24:23 2023, max compression
+gzip compressed data, was "calculator_MU-1.0.3.tar", last modified: Sun Jul  9 15:42:12 2023, max compression
```

## Comparing `calculator_MU-1.0.2.tar` & `calculator_MU-1.0.3.tar`

### file list

```diff
@@ -1,9 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 15:24:23.758804 calculator_MU-1.0.2/
--rw-rw-rw-   0        0        0      312 2023-07-09 15:24:23.757831 calculator_MU-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-09 15:24:23.756809 calculator_MU-1.0.2/calculator_MU.egg-info/
--rw-rw-rw-   0        0        0      312 2023-07-09 15:24:23.000000 calculator_MU-1.0.2/calculator_MU.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      156 2023-07-09 15:24:23.000000 calculator_MU-1.0.2/calculator_MU.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 15:24:23.000000 calculator_MU-1.0.2/calculator_MU.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 15:24:23.000000 calculator_MU-1.0.2/calculator_MU.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-09 15:24:23.758804 calculator_MU-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      436 2023-07-09 15:19:47.000000 calculator_MU-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 15:42:12.136823 calculator_MU-1.0.3/
+-rw-rw-rw-   0        0        0      312 2023-07-09 15:42:12.135824 calculator_MU-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1089 2023-07-09 15:34:41.000000 calculator_MU-1.0.3/README
+drwxrwxrwx   0        0        0        0 2023-07-09 15:42:12.134828 calculator_MU-1.0.3/calculator_MU.egg-info/
+-rw-rw-rw-   0        0        0      312 2023-07-09 15:42:12.000000 calculator_MU-1.0.3/calculator_MU.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      163 2023-07-09 15:42:12.000000 calculator_MU-1.0.3/calculator_MU.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 15:42:12.000000 calculator_MU-1.0.3/calculator_MU.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 15:42:12.000000 calculator_MU-1.0.3/calculator_MU.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-09 15:42:12.136823 calculator_MU-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      436 2023-07-09 15:42:08.000000 calculator_MU-1.0.3/setup.py
```

