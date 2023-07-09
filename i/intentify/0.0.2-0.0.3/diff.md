# Comparing `tmp/intentify-0.0.2.tar.gz` & `tmp/intentify-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intentify-0.0.2.tar", last modified: Sun Jul  9 18:33:45 2023, max compression
+gzip compressed data, was "intentify-0.0.3.tar", last modified: Sun Jul  9 18:41:45 2023, max compression
```

## Comparing `intentify-0.0.2.tar` & `intentify-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 18:33:45.370852 intentify-0.0.2/
--rw-rw-rw-   0        0        0     2753 2023-07-09 18:33:45.369852 intentify-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2183 2023-07-09 18:18:34.000000 intentify-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-09 18:33:45.359771 intentify-0.0.2/intentify/
--rw-rw-rw-   0        0        0       36 2023-07-07 19:32:27.000000 intentify-0.0.2/intentify/__init__.py
--rw-rw-rw-   0        0        0     6570 2023-07-07 20:09:00.000000 intentify-0.0.2/intentify/main.py
-drwxrwxrwx   0        0        0        0 2023-07-09 18:33:45.369852 intentify-0.0.2/intentify.egg-info/
--rw-rw-rw-   0        0        0     2753 2023-07-09 18:33:45.000000 intentify-0.0.2/intentify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-07-09 18:33:45.000000 intentify-0.0.2/intentify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 18:33:45.000000 intentify-0.0.2/intentify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-07-09 18:33:45.000000 intentify-0.0.2/intentify.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-09 18:33:45.000000 intentify-0.0.2/intentify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-09 18:33:45.370852 intentify-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1022 2023-07-09 18:32:36.000000 intentify-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:41:45.530049 intentify-0.0.3/
+-rw-rw-rw-   0        0        0     2753 2023-07-09 18:41:45.530049 intentify-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2183 2023-07-09 18:18:34.000000 intentify-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 18:41:45.517084 intentify-0.0.3/intentify/
+-rw-rw-rw-   0        0        0       36 2023-07-07 19:32:27.000000 intentify-0.0.3/intentify/__init__.py
+-rw-rw-rw-   0        0        0     6570 2023-07-07 20:09:00.000000 intentify-0.0.3/intentify/main.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:41:45.529051 intentify-0.0.3/intentify.egg-info/
+-rw-rw-rw-   0        0        0     2753 2023-07-09 18:41:45.000000 intentify-0.0.3/intentify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-07-09 18:41:45.000000 intentify-0.0.3/intentify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 18:41:45.000000 intentify-0.0.3/intentify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-07-09 18:41:45.000000 intentify-0.0.3/intentify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-09 18:41:45.000000 intentify-0.0.3/intentify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-09 18:41:45.531047 intentify-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1012 2023-07-09 18:41:39.000000 intentify-0.0.3/setup.py
```

### Comparing `intentify-0.0.2/PKG-INFO` & `intentify-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intentify
-Version: 0.0.2
+Version: 0.0.3
 Summary: An intent classification library for AI Models.
 Author: Ice (Rishan Pancham)
 Author-email: <rishanpan@hotmail.com>
 Keywords: python,intent,intents,ai,intent classification
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `intentify-0.0.2/README.md` & `intentify-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `intentify-0.0.2/intentify/main.py` & `intentify-0.0.3/intentify/main.py`

 * *Files identical despite different names*

### Comparing `intentify-0.0.2/intentify.egg-info/PKG-INFO` & `intentify-0.0.3/intentify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intentify
-Version: 0.0.2
+Version: 0.0.3
 Summary: An intent classification library for AI Models.
 Author: Ice (Rishan Pancham)
 Author-email: <rishanpan@hotmail.com>
 Keywords: python,intent,intents,ai,intent classification
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `intentify-0.0.2/setup.py` & `intentify-0.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'An intent classification library for AI Models.'
 
 # Setting up
 setup(
     name="intentify",
     version=VERSION,
     author="Ice (Rishan Pancham)",
     author_email="<rishanpan@hotmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
-    install_requires=['pickle', 'numpy', 'tensorflow', 'nltk', 'keras'],
+    install_requires=['numpy', 'tensorflow', 'nltk', 'keras'],
     keywords=['python', 'intent', 'intents', 'ai', 'intent classification'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

