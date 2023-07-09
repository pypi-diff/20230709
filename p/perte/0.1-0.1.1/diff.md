# Comparing `tmp/perte-0.1.tar.gz` & `tmp/perte-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\perte-0.1.tar", last modified: Sun Jul  2 13:32:31 2023, max compression
+gzip compressed data, was "dist\perte-0.1.1.tar", last modified: Sun Jul  2 13:46:57 2023, max compression
```

## Comparing `perte-0.1.tar` & `perte-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 13:32:31.000000 perte-0.1/
--rw-rw-rw-   0        0        0     1079 2023-07-02 13:23:25.000000 perte-0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      939 2023-07-02 13:32:31.000000 perte-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      425 2023-07-02 13:31:44.000000 perte-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-02 13:32:31.000000 perte-0.1/perte/
--rw-rw-rw-   0        0        0       28 2023-07-02 13:13:56.000000 perte-0.1/perte/__init__.py
--rw-rw-rw-   0        0        0     9297 2023-07-02 13:14:29.000000 perte-0.1/perte/triplet_losses.py
-drwxrwxrwx   0        0        0        0 2023-07-02 13:32:31.000000 perte-0.1/perte.egg-info/
--rw-rw-rw-   0        0        0      939 2023-07-02 13:32:31.000000 perte-0.1/perte.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-07-02 13:32:31.000000 perte-0.1/perte.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 13:32:31.000000 perte-0.1/perte.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-07-02 13:32:31.000000 perte-0.1/perte.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-02 13:32:31.000000 perte-0.1/perte.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-02 13:32:31.000000 perte-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1388 2023-07-02 13:21:58.000000 perte-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 13:46:57.000000 perte-0.1.1/
+-rw-rw-rw-   0        0        0     1079 2023-07-02 13:23:25.000000 perte-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      943 2023-07-02 13:46:57.000000 perte-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      425 2023-07-02 13:31:44.000000 perte-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-02 13:46:56.000000 perte-0.1.1/perte/
+-rw-rw-rw-   0        0        0       29 2023-07-02 13:37:55.000000 perte-0.1.1/perte/__init__.py
+-rw-rw-rw-   0        0        0     9297 2023-07-02 13:14:29.000000 perte-0.1.1/perte/triplet_losses.py
+drwxrwxrwx   0        0        0        0 2023-07-02 13:46:56.000000 perte-0.1.1/perte.egg-info/
+-rw-rw-rw-   0        0        0      943 2023-07-02 13:46:56.000000 perte-0.1.1/perte.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-07-02 13:46:56.000000 perte-0.1.1/perte.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 13:46:56.000000 perte-0.1.1/perte.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-07-02 13:46:56.000000 perte-0.1.1/perte.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-02 13:46:56.000000 perte-0.1.1/perte.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-02 13:46:57.000000 perte-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1392 2023-07-02 13:46:53.000000 perte-0.1.1/setup.py
```

### Comparing `perte-0.1/LICENSE.txt` & `perte-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `perte-0.1/PKG-INFO` & `perte-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: perte
-Version: 0.1
+Version: 0.1.1
 Summary: A fast way to use the diverse loss functions in deep learning
 Home-page: https://github.com/taindp98/perte
-Download-URL: https://github.com/taindp98/perte/archive/refs/tags/v0.1.tar.gz
+Download-URL: https://github.com/taindp98/perte/archive/refs/tags/v0.1.1.tar.gz
 Author: Rémi NGUYEN
 Author-email: taindp98@gmail.com
 License: MIT
 Keywords: loss-function,discrimination
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `perte-0.1/perte/triplet_losses.py` & `perte-0.1.1/perte/triplet_losses.py`

 * *Files identical despite different names*

### Comparing `perte-0.1/perte.egg-info/PKG-INFO` & `perte-0.1.1/perte.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: perte
-Version: 0.1
+Version: 0.1.1
 Summary: A fast way to use the diverse loss functions in deep learning
 Home-page: https://github.com/taindp98/perte
-Download-URL: https://github.com/taindp98/perte/archive/refs/tags/v0.1.tar.gz
+Download-URL: https://github.com/taindp98/perte/archive/refs/tags/v0.1.1.tar.gz
 Author: Rémi NGUYEN
 Author-email: taindp98@gmail.com
 License: MIT
 Keywords: loss-function,discrimination
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `perte-0.1/setup.py` & `perte-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import setuptools,re,sys
 
 setuptools.setup(
     name = 'perte',         
     packages = ['perte'],
-    version = '0.1',     
+    version = '0.1.1',     
     license='MIT', 
     description = 'A fast way to use the diverse loss functions in deep learning', 
     author = 'Rémi NGUYEN',                   
     author_email = 'taindp98@gmail.com',      
     url = 'https://github.com/taindp98/perte',   
-    download_url = 'https://github.com/taindp98/perte/archive/refs/tags/v0.1.tar.gz',   
+    download_url = 'https://github.com/taindp98/perte/archive/refs/tags/v0.1.1.tar.gz',   
     keywords = ['loss-function', 'discrimination'],  
     install_requires=[
         'pip', 'packaging',
         'torch', 'numpy'
     ],
     classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
```

