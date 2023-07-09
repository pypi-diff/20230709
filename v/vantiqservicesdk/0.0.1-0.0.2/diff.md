# Comparing `tmp/vantiqservicesdk-0.0.1.tar.gz` & `tmp/vantiqservicesdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantiqservicesdk-0.0.1.tar", last modified: Fri Jul  7 16:46:14 2023, max compression
+gzip compressed data, was "vantiqservicesdk-0.0.2.tar", last modified: Sun Jul  9 16:16:40 2023, max compression
```

## Comparing `vantiqservicesdk-0.0.1.tar` & `vantiqservicesdk-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 16:46:14.569189 vantiqservicesdk-0.0.1/
--rw-rw-rw-   0        0        0     1098 2023-07-07 14:53:00.000000 vantiqservicesdk-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2593 2023-07-07 16:46:14.569189 vantiqservicesdk-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      885 2023-07-07 14:53:00.000000 vantiqservicesdk-0.0.1/README.md
--rw-rw-rw-   0        0        0       82 2023-07-06 01:15:42.000000 vantiqservicesdk-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      775 2023-07-07 16:46:14.570154 vantiqservicesdk-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-07 16:46:14.554154 vantiqservicesdk-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-07 16:46:14.554154 vantiqservicesdk-0.0.1/src/main/
-drwxrwxrwx   0        0        0        0 2023-07-07 16:46:14.567188 vantiqservicesdk-0.0.1/src/main/python/
-drwxrwxrwx   0        0        0        0 2023-07-07 16:46:14.566153 vantiqservicesdk-0.0.1/src/main/python/vantiqservicesdk.egg-info/
--rw-rw-rw-   0        0        0     2593 2023-07-07 16:46:14.000000 vantiqservicesdk-0.0.1/src/main/python/vantiqservicesdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      636 2023-07-07 16:46:14.000000 vantiqservicesdk-0.0.1/src/main/python/vantiqservicesdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 16:46:14.000000 vantiqservicesdk-0.0.1/src/main/python/vantiqservicesdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 16:46:14.000000 vantiqservicesdk-0.0.1/src/main/python/vantiqservicesdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-07 16:46:14.000000 vantiqservicesdk-0.0.1/src/main/python/vantiqservicesdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2638 2023-07-06 01:13:00.000000 vantiqservicesdk-0.0.1/src/main/python/vantiqservicesdk.py
+drwxrwxrwx   0        0        0        0 2023-07-09 16:16:40.382606 vantiqservicesdk-0.0.2/
+-rw-rw-rw-   0        0        0     1098 2023-07-08 17:40:47.000000 vantiqservicesdk-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2637 2023-07-09 16:16:40.381606 vantiqservicesdk-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      885 2023-07-08 17:40:47.000000 vantiqservicesdk-0.0.2/README.md
+-rw-rw-rw-   0        0        0     1072 2023-07-09 16:16:25.000000 vantiqservicesdk-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-09 16:16:40.382606 vantiqservicesdk-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-09 16:16:40.366616 vantiqservicesdk-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-09 16:16:40.366616 vantiqservicesdk-0.0.2/src/main/
+drwxrwxrwx   0        0        0        0 2023-07-09 16:16:40.379606 vantiqservicesdk-0.0.2/src/main/python/
+drwxrwxrwx   0        0        0        0 2023-07-09 16:16:40.377614 vantiqservicesdk-0.0.2/src/main/python/vantiqservicesdk.egg-info/
+-rw-rw-rw-   0        0        0     2637 2023-07-09 16:16:40.000000 vantiqservicesdk-0.0.2/src/main/python/vantiqservicesdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      626 2023-07-09 16:16:40.000000 vantiqservicesdk-0.0.2/src/main/python/vantiqservicesdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 16:16:40.000000 vantiqservicesdk-0.0.2/src/main/python/vantiqservicesdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-07-09 16:16:40.000000 vantiqservicesdk-0.0.2/src/main/python/vantiqservicesdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-09 16:16:40.000000 vantiqservicesdk-0.0.2/src/main/python/vantiqservicesdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2638 2023-07-08 17:40:47.000000 vantiqservicesdk-0.0.2/src/main/python/vantiqservicesdk.py
```

### Comparing `vantiqservicesdk-0.0.1/LICENSE` & `vantiqservicesdk-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vantiqservicesdk-0.0.1/PKG-INFO` & `vantiqservicesdk-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: vantiqservicesdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: SDK for building Vantiq service connectors in Python
-Home-page: https://github.com/Vantiq/vantiq-service-connectors
-Author: Vantiq, Inc
-Author-email: sfitts@vantiq.com
+Author-email: Vantiq <sfitts@vantiq.com>
 License: MIT
+Project-URL: Homepage, https://github.com/Vantiq/vantiq-service-connectors
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `vantiqservicesdk-0.0.1/README.md` & `vantiqservicesdk-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `vantiqservicesdk-0.0.1/src/main/python/vantiqservicesdk.egg-info/PKG-INFO` & `vantiqservicesdk-0.0.2/src/main/python/vantiqservicesdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: vantiqservicesdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: SDK for building Vantiq service connectors in Python
-Home-page: https://github.com/Vantiq/vantiq-service-connectors
-Author: Vantiq, Inc
-Author-email: sfitts@vantiq.com
+Author-email: Vantiq <sfitts@vantiq.com>
 License: MIT
+Project-URL: Homepage, https://github.com/Vantiq/vantiq-service-connectors
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `vantiqservicesdk-0.0.1/src/main/python/vantiqservicesdk.egg-info/SOURCES.txt` & `vantiqservicesdk-0.0.2/src/main/python/vantiqservicesdk.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 README.md
 pyproject.toml
-setup.cfg
 src/main/python/vantiqservicesdk.egg-info/PKG-INFO
 src/main/python/vantiqservicesdk.egg-info/SOURCES.txt
 src/main/python/vantiqservicesdk.egg-info/dependency_links.txt
 src/main/python/vantiqservicesdk.egg-info/requires.txt
 src/main/python/vantiqservicesdk.egg-info/top_level.txt
 src/main/python/vantiqservicesdk.py
 src/main/python/vantiqservicesdk.egg-info/PKG-INFO
```

### Comparing `vantiqservicesdk-0.0.1/src/main/python/vantiqservicesdk.py` & `vantiqservicesdk-0.0.2/src/main/python/vantiqservicesdk.py`

 * *Files identical despite different names*

