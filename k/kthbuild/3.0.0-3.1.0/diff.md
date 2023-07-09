# Comparing `tmp/kthbuild-3.0.0.tar.gz` & `tmp/kthbuild-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kthbuild-3.0.0.tar", last modified: Fri Jun 16 10:40:42 2023, max compression
+gzip compressed data, was "kthbuild-3.1.0.tar", last modified: Sun Jul  9 20:00:55 2023, max compression
```

## Comparing `kthbuild-3.0.0.tar` & `kthbuild-3.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 10:40:42.519691 kthbuild-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-06-16 10:40:17.000000 kthbuild-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1796 2023-06-16 10:40:42.519691 kthbuild-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      432 2023-06-16 10:40:17.000000 kthbuild-3.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 10:40:42.519691 kthbuild-3.0.0/kthbuild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1796 2023-06-16 10:40:42.000000 kthbuild-3.0.0/kthbuild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      198 2023-06-16 10:40:42.000000 kthbuild-3.0.0/kthbuild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-06-16 10:40:42.000000 kthbuild-3.0.0/kthbuild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-06-16 10:40:42.000000 kthbuild-3.0.0/kthbuild.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-16 10:40:42.000000 kthbuild-3.0.0/kthbuild.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)    45558 2023-06-16 10:40:17.000000 kthbuild-3.0.0/kthbuild.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-16 10:40:42.519691 kthbuild-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4874 2023-06-16 10:40:17.000000 kthbuild-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-09 20:00:55.255719 kthbuild-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-07-09 20:00:32.000000 kthbuild-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1796 2023-07-09 20:00:55.255719 kthbuild-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      432 2023-07-09 20:00:32.000000 kthbuild-3.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-09 20:00:55.255719 kthbuild-3.1.0/kthbuild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1796 2023-07-09 20:00:55.000000 kthbuild-3.1.0/kthbuild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      198 2023-07-09 20:00:55.000000 kthbuild-3.1.0/kthbuild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-07-09 20:00:55.000000 kthbuild-3.1.0/kthbuild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-09 20:00:55.000000 kthbuild-3.1.0/kthbuild.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-09 20:00:55.000000 kthbuild-3.1.0/kthbuild.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    45726 2023-07-09 20:00:32.000000 kthbuild-3.1.0/kthbuild.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-09 20:00:55.255719 kthbuild-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4874 2023-07-09 20:00:32.000000 kthbuild-3.1.0/setup.py
```

### Comparing `kthbuild-3.0.0/LICENSE` & `kthbuild-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kthbuild-3.0.0/PKG-INFO` & `kthbuild-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kthbuild
-Version: 3.0.0
+Version: 3.1.0
 Summary: Knuth node build tools
 Home-page: https://github.com/k-nuth/kthbuild
 Author: Fernando Pelliccioni
 Author-email: fpelliccioni@gmail.com
 License: MIT
 Keywords: knuth kth crypto bitcoin btc bch cash build tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `kthbuild-3.0.0/kthbuild.egg-info/PKG-INFO` & `kthbuild-3.1.0/kthbuild.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kthbuild
-Version: 3.0.0
+Version: 3.1.0
 Summary: Knuth node build tools
 Home-page: https://github.com/k-nuth/kthbuild
 Author: Fernando Pelliccioni
 Author-email: fpelliccioni@gmail.com
 License: MIT
 Keywords: knuth kth crypto bitcoin btc bch cash build tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `kthbuild-3.0.0/kthbuild.py` & `kthbuild-3.1.0/kthbuild.py`

 * *Files 0% similar despite different names*

```diff
@@ -764,21 +764,25 @@
 
 class KnuthConanFileV2(ConanFile):
     def config_options(self):
         # ConanFile.config_options(self)
 
         if self.settings.arch != "x86_64":
             self.output.info("march_id is disabled for architectures other than x86_64, your architecture: %s" % (self.settings.arch,))
-            self.options.remove("march_id")
-            self.options.remove("march_strategy")
+            # self.options.remove("march_id")
+            # self.options.remove("march_strategy")
+            del self.options.march_id
+            del self.options.march_strategy
 
         if self.settings.compiler == "msvc":
-            self.options.remove("fPIC")
+            # self.options.remove("fPIC")
+            del self.options.fPIC
             if self.is_shared:
-                self.options.remove("shared")
+                # self.options.remove("shared")
+                del self.options.shared
 
     def validate(self, pure_c=False):
         # self.output.info(f"validate() self.march_data: {self.march_data}")
         # self.output.info(f"validate() self.march_from_cpuid: {self.march_from_cpuid}")
 
         # ConanFile.validate(self)
```

### Comparing `kthbuild-3.0.0/setup.py` & `kthbuild-3.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import subprocess
 import os
 import platform
 
 __title__ = "kthbuild"
 __summary__ = "Knuth node build tools"
 __uri__ = "https://github.com/k-nuth/kthbuild"
-__version__ = "3.0.0"
+__version__ = "3.1.0"
 __author__ = "Fernando Pelliccioni"
 __email__ = "fpelliccioni@gmail.com"
 __license__ = "MIT"
 __copyright__ = "Copyright (c) 2019-2023 Knuth Project"
 
 
 install_requires = [
```

