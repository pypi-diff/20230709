# Comparing `tmp/perte-0.1.2.tar.gz` & `tmp/perte-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Admin\working\python\mine\perte\dist\.tmp-ld4va5q5\perte-0.1.2.tar", last modified: Sun Jul  9 03:43:28 2023, max compression
+gzip compressed data, was "C:\Users\Admin\working\python\mine\perte\dist\.tmp-nx18wf53\perte-0.1.3.tar", last modified: Sun Jul  9 03:47:13 2023, max compression
```

## Comparing `perte-0.1.2.tar` & `perte-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 03:43:28.000000 perte-0.1.2/
--rw-rw-rw-   0        0        0     1079 2023-07-02 13:23:25.000000 perte-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0      943 2023-07-09 03:43:28.000000 perte-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1771 2023-07-09 03:36:41.000000 perte-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-09 03:43:28.000000 perte-0.1.2/perte/
--rw-rw-rw-   0        0        0      171 2023-07-09 02:57:22.000000 perte-0.1.2/perte/__init__.py
--rw-rw-rw-   0        0        0     4442 2023-07-09 03:18:17.000000 perte-0.1.2/perte/angular_losses.py
--rw-rw-rw-   0        0        0     1801 2023-07-09 03:20:52.000000 perte-0.1.2/perte/focal_losses.py
--rw-rw-rw-   0        0        0     1139 2023-07-09 03:21:43.000000 perte-0.1.2/perte/ldam_loss.py
--rw-rw-rw-   0        0        0     4925 2023-07-09 03:29:20.000000 perte-0.1.2/perte/poly_loss.py
--rw-rw-rw-   0        0        0     2241 2023-07-09 03:34:22.000000 perte-0.1.2/perte/recall_loss.py
--rw-rw-rw-   0        0        0     9773 2023-07-09 03:10:49.000000 perte-0.1.2/perte/triplet_losses.py
-drwxrwxrwx   0        0        0        0 2023-07-09 03:43:28.000000 perte-0.1.2/perte.egg-info/
--rw-rw-rw-   0        0        0      943 2023-07-09 03:43:28.000000 perte-0.1.2/perte.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2023-07-09 03:43:28.000000 perte-0.1.2/perte.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 03:43:28.000000 perte-0.1.2/perte.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-07-09 03:43:28.000000 perte-0.1.2/perte.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-09 03:43:28.000000 perte-0.1.2/perte.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-09 03:43:28.000000 perte-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1392 2023-07-09 03:42:52.000000 perte-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 03:47:13.000000 perte-0.1.3/
+-rw-rw-rw-   0        0        0     1079 2023-07-02 13:23:25.000000 perte-0.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      944 2023-07-09 03:47:13.000000 perte-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1771 2023-07-09 03:36:41.000000 perte-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 03:47:13.000000 perte-0.1.3/perte/
+-rw-rw-rw-   0        0        0      171 2023-07-09 02:57:22.000000 perte-0.1.3/perte/__init__.py
+-rw-rw-rw-   0        0        0     4442 2023-07-09 03:18:17.000000 perte-0.1.3/perte/angular_losses.py
+-rw-rw-rw-   0        0        0     1801 2023-07-09 03:20:52.000000 perte-0.1.3/perte/focal_losses.py
+-rw-rw-rw-   0        0        0     1139 2023-07-09 03:21:43.000000 perte-0.1.3/perte/ldam_loss.py
+-rw-rw-rw-   0        0        0     4925 2023-07-09 03:29:20.000000 perte-0.1.3/perte/poly_loss.py
+-rw-rw-rw-   0        0        0     2241 2023-07-09 03:34:22.000000 perte-0.1.3/perte/recall_loss.py
+-rw-rw-rw-   0        0        0     9773 2023-07-09 03:10:49.000000 perte-0.1.3/perte/triplet_losses.py
+drwxrwxrwx   0        0        0        0 2023-07-09 03:47:13.000000 perte-0.1.3/perte.egg-info/
+-rw-rw-rw-   0        0        0      944 2023-07-09 03:47:13.000000 perte-0.1.3/perte.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2023-07-09 03:47:13.000000 perte-0.1.3/perte.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 03:47:13.000000 perte-0.1.3/perte.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-07-09 03:47:13.000000 perte-0.1.3/perte.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-09 03:47:13.000000 perte-0.1.3/perte.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-09 03:47:13.000000 perte-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1393 2023-07-09 03:46:24.000000 perte-0.1.3/setup.py
```

### Comparing `perte-0.1.2/LICENSE.txt` & `perte-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `perte-0.1.2/PKG-INFO` & `perte-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: perte
-Version: 0.1.2
+Version: 0.1.3
 Summary: A fast way to use the diverse loss functions in deep learning
 Home-page: https://github.com/taindp98/perte
-Download-URL: https://github.com/taindp98/perte/archive/refs/tags/v0.1.1.tar.gz
+Download-URL: https://github.com/taindp98/perte/archive/refs/tags/v.0.1.2.tar.gz
 Author: Rémi NGUYEN
 Author-email: taindp98@gmail.com
 License: MIT
 Keywords: loss-function,discrimination
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `perte-0.1.2/README.md` & `perte-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `perte-0.1.2/perte/angular_losses.py` & `perte-0.1.3/perte/angular_losses.py`

 * *Files identical despite different names*

### Comparing `perte-0.1.2/perte/focal_losses.py` & `perte-0.1.3/perte/focal_losses.py`

 * *Files identical despite different names*

### Comparing `perte-0.1.2/perte/ldam_loss.py` & `perte-0.1.3/perte/ldam_loss.py`

 * *Files identical despite different names*

### Comparing `perte-0.1.2/perte/poly_loss.py` & `perte-0.1.3/perte/poly_loss.py`

 * *Files identical despite different names*

### Comparing `perte-0.1.2/perte/recall_loss.py` & `perte-0.1.3/perte/recall_loss.py`

 * *Files identical despite different names*

### Comparing `perte-0.1.2/perte/triplet_losses.py` & `perte-0.1.3/perte/triplet_losses.py`

 * *Files identical despite different names*

### Comparing `perte-0.1.2/perte.egg-info/PKG-INFO` & `perte-0.1.3/perte.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: perte
-Version: 0.1.2
+Version: 0.1.3
 Summary: A fast way to use the diverse loss functions in deep learning
 Home-page: https://github.com/taindp98/perte
-Download-URL: https://github.com/taindp98/perte/archive/refs/tags/v0.1.1.tar.gz
+Download-URL: https://github.com/taindp98/perte/archive/refs/tags/v.0.1.2.tar.gz
 Author: Rémi NGUYEN
 Author-email: taindp98@gmail.com
 License: MIT
 Keywords: loss-function,discrimination
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `perte-0.1.2/setup.py` & `perte-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import setuptools,re,sys
 
 setuptools.setup(
     name = 'perte',         
     packages = ['perte'],
-    version = '0.1.2',     
+    version = '0.1.3',     
     license='MIT', 
     description = 'A fast way to use the diverse loss functions in deep learning', 
     author = 'Rémi NGUYEN',                   
     author_email = 'taindp98@gmail.com',      
     url = 'https://github.com/taindp98/perte',   
-    download_url = 'https://github.com/taindp98/perte/archive/refs/tags/v0.1.1.tar.gz',   
+    download_url = 'https://github.com/taindp98/perte/archive/refs/tags/v.0.1.2.tar.gz',   
     keywords = ['loss-function', 'discrimination'],  
     install_requires=[
         'pip', 'packaging',
         'torch', 'numpy'
     ],
     classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
```

