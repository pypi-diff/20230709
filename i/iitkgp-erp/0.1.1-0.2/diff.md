# Comparing `tmp/iitkgp-erp-0.1.1.tar.gz` & `tmp/iitkgp-erp-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iitkgp-erp-0.1.1.tar", last modified: Sun Jul  9 11:03:05 2023, max compression
+gzip compressed data, was "iitkgp-erp-0.2.tar", last modified: Sun Jul  9 15:12:11 2023, max compression
```

## Comparing `iitkgp-erp-0.1.1.tar` & `iitkgp-erp-0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 proffapt   (501) staff       (20)        0 2023-07-09 11:03:05.852616 iitkgp-erp-0.1.1/
--rw-r--r--   0 proffapt   (501) staff       (20)     1314 2023-07-09 08:27:13.000000 iitkgp-erp-0.1.1/LICENSE.txt
--rw-r--r--   0 proffapt   (501) staff       (20)      249 2023-07-09 11:03:05.852440 iitkgp-erp-0.1.1/PKG-INFO
-drwxr-xr-x   0 proffapt   (501) staff       (20)        0 2023-07-09 11:03:05.852171 iitkgp-erp-0.1.1/iitkgp_erp.egg-info/
--rw-r--r--   0 proffapt   (501) staff       (20)      249 2023-07-09 11:03:05.000000 iitkgp-erp-0.1.1/iitkgp_erp.egg-info/PKG-INFO
--rw-r--r--   0 proffapt   (501) staff       (20)      189 2023-07-09 11:03:05.000000 iitkgp-erp-0.1.1/iitkgp_erp.egg-info/SOURCES.txt
--rw-r--r--   0 proffapt   (501) staff       (20)        1 2023-07-09 11:03:05.000000 iitkgp-erp-0.1.1/iitkgp_erp.egg-info/dependency_links.txt
--rw-r--r--   0 proffapt   (501) staff       (20)       79 2023-07-09 11:03:05.000000 iitkgp-erp-0.1.1/iitkgp_erp.egg-info/requires.txt
--rw-r--r--   0 proffapt   (501) staff       (20)        1 2023-07-09 11:03:05.000000 iitkgp-erp-0.1.1/iitkgp_erp.egg-info/top_level.txt
--rw-r--r--   0 proffapt   (501) staff       (20)       38 2023-07-09 11:03:05.852675 iitkgp-erp-0.1.1/setup.cfg
--rw-r--r--   0 proffapt   (501) staff       (20)      473 2023-07-09 11:03:03.000000 iitkgp-erp-0.1.1/setup.py
+drwxr-xr-x   0 proffapt   (501) staff       (20)        0 2023-07-09 15:12:11.633885 iitkgp-erp-0.2/
+-rw-r--r--   0 proffapt   (501) staff       (20)     1314 2023-07-09 08:27:13.000000 iitkgp-erp-0.2/LICENSE.txt
+-rw-r--r--   0 proffapt   (501) staff       (20)      247 2023-07-09 15:12:11.633716 iitkgp-erp-0.2/PKG-INFO
+drwxr-xr-x   0 proffapt   (501) staff       (20)        0 2023-07-09 15:12:11.633460 iitkgp-erp-0.2/iitkgp_erp.egg-info/
+-rw-r--r--   0 proffapt   (501) staff       (20)      247 2023-07-09 15:12:11.000000 iitkgp-erp-0.2/iitkgp_erp.egg-info/PKG-INFO
+-rw-r--r--   0 proffapt   (501) staff       (20)      189 2023-07-09 15:12:11.000000 iitkgp-erp-0.2/iitkgp_erp.egg-info/SOURCES.txt
+-rw-r--r--   0 proffapt   (501) staff       (20)        1 2023-07-09 15:12:11.000000 iitkgp-erp-0.2/iitkgp_erp.egg-info/dependency_links.txt
+-rw-r--r--   0 proffapt   (501) staff       (20)      108 2023-07-09 15:12:11.000000 iitkgp-erp-0.2/iitkgp_erp.egg-info/requires.txt
+-rw-r--r--   0 proffapt   (501) staff       (20)        1 2023-07-09 15:12:11.000000 iitkgp-erp-0.2/iitkgp_erp.egg-info/top_level.txt
+-rw-r--r--   0 proffapt   (501) staff       (20)       38 2023-07-09 15:12:11.633949 iitkgp-erp-0.2/setup.cfg
+-rw-r--r--   0 proffapt   (501) staff       (20)      555 2023-07-09 15:12:11.000000 iitkgp-erp-0.2/setup.py
```

### Comparing `iitkgp-erp-0.1.1/LICENSE.txt` & `iitkgp-erp-0.2/LICENSE.txt`

 * *Files identical despite different names*

