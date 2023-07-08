# Comparing `tmp/botoplus-0.4.2.tar.gz` & `tmp/botoplus-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botoplus-0.4.2.tar", last modified: Wed Jan  4 02:05:01 2023, max compression
+gzip compressed data, was "botoplus-0.5.0.tar", last modified: Sat Jul  8 22:19:38 2023, max compression
```

## Comparing `botoplus-0.4.2.tar` & `botoplus-0.5.0.tar`

### file list

```diff
@@ -1,26 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-04 02:05:01.062326 botoplus-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-01-04 02:04:46.000000 botoplus-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     6994 2023-01-04 02:05:01.058326 botoplus-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6706 2023-01-04 02:04:46.000000 botoplus-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-04 02:05:01.058326 botoplus-0.4.2/botoplus/
--rw-r--r--   0 runner    (1001) docker     (122)       31 2023-01-04 02:04:46.000000 botoplus-0.4.2/botoplus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      255 2023-01-04 02:04:46.000000 botoplus-0.4.2/botoplus/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2733 2023-01-04 02:04:46.000000 botoplus-0.4.2/botoplus/account.py
--rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-01-04 02:04:46.000000 botoplus-0.4.2/botoplus/botoplus.py
--rw-r--r--   0 runner    (1001) docker     (122)     5490 2023-01-04 02:04:46.000000 botoplus-0.4.2/botoplus/cdk.py
--rw-r--r--   0 runner    (1001) docker     (122)     2306 2023-01-04 02:04:46.000000 botoplus-0.4.2/botoplus/cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (122)     2489 2023-01-04 02:04:46.000000 botoplus-0.4.2/botoplus/identity.py
--rw-r--r--   0 runner    (1001) docker     (122)     2404 2023-01-04 02:04:46.000000 botoplus-0.4.2/botoplus/paginator.py
--rw-r--r--   0 runner    (1001) docker     (122)     2619 2023-01-04 02:04:46.000000 botoplus-0.4.2/botoplus/paginators.py
--rw-r--r--   0 runner    (1001) docker     (122)     2496 2023-01-04 02:04:46.000000 botoplus-0.4.2/botoplus/region.py
--rw-r--r--   0 runner    (1001) docker     (122)     3243 2023-01-04 02:04:46.000000 botoplus-0.4.2/botoplus/securityhub.py
--rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-01-04 02:04:46.000000 botoplus-0.4.2/botoplus/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-04 02:05:01.058326 botoplus-0.4.2/botoplus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6994 2023-01-04 02:05:01.000000 botoplus-0.4.2/botoplus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      478 2023-01-04 02:05:01.000000 botoplus-0.4.2/botoplus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-04 02:05:01.000000 botoplus-0.4.2/botoplus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       51 2023-01-04 02:05:01.000000 botoplus-0.4.2/botoplus.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-01-04 02:05:01.000000 botoplus-0.4.2/botoplus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-01-04 02:05:01.000000 botoplus-0.4.2/botoplus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-01-04 02:05:01.062326 botoplus-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      737 2023-01-04 02:04:46.000000 botoplus-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:19:38.656268 botoplus-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-08 22:19:23.000000 botoplus-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-08 22:19:38.656268 botoplus-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-08 22:19:23.000000 botoplus-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:19:38.656268 botoplus-0.5.0/botoplus/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-08 22:19:23.000000 botoplus-0.5.0/botoplus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-07-08 22:19:23.000000 botoplus-0.5.0/botoplus/botoplus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:19:38.656268 botoplus-0.5.0/botoplus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-08 22:19:38.000000 botoplus-0.5.0/botoplus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-08 22:19:38.000000 botoplus-0.5.0/botoplus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 22:19:38.000000 botoplus-0.5.0/botoplus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-08 22:19:38.000000 botoplus-0.5.0/botoplus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-08 22:19:38.000000 botoplus-0.5.0/botoplus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 22:19:38.656268 botoplus-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-08 22:19:23.000000 botoplus-0.5.0/setup.py
```

### Comparing `botoplus-0.4.2/LICENSE` & `botoplus-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `botoplus-0.4.2/setup.py` & `botoplus-0.5.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,27 +4,22 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name = "botoplus",
     version = __version__,
-    description = "Threat Hunting Toolkit",
+    description = "Python Library for Jupyter Notebooks",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/botoplus/botoplus",
     author = "botoplus",
     author_email = "hello@botoplus.com",
     license = "Apache-2.0",
     packages = ["botoplus"],
     install_requires = [
         "aws-sso-lib",
         "boto3",
         "typer[all]"
     ],
-    entry_points = {
-        "console_scripts": [
-            "botoplus=botoplus.botoplus:app"
-        ],
-    },
     python_requires = ">=3.7",
 )
```

