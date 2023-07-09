# Comparing `tmp/parametricGarch-0.0.1.tar.gz` & `tmp/parametricGarch-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parametricGarch-0.0.1.tar", last modified: Tue Jul  4 18:04:18 2023, max compression
+gzip compressed data, was "parametricGarch-0.0.2.tar", last modified: Sun Jul  9 20:41:17 2023, max compression
```

## Comparing `parametricGarch-0.0.1.tar` & `parametricGarch-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 playerone   (501) staff       (20)        0 2023-07-04 18:04:18.569480 parametricGarch-0.0.1/
--rw-r--r--   0 playerone   (501) staff       (20)    35148 2023-07-04 17:25:08.000000 parametricGarch-0.0.1/LICENSE
--rw-r--r--   0 playerone   (501) staff       (20)     1158 2023-07-04 18:04:18.569210 parametricGarch-0.0.1/PKG-INFO
--rw-r--r--   0 playerone   (501) staff       (20)      213 2023-07-04 14:11:34.000000 parametricGarch-0.0.1/README.md
-drwxr-xr-x   0 playerone   (501) staff       (20)        0 2023-07-04 18:04:18.565802 parametricGarch-0.0.1/parametricGarch/
--rw-r--r--   0 playerone   (501) staff       (20)       45 2023-07-04 17:29:41.000000 parametricGarch-0.0.1/parametricGarch/__init__.py
--rw-r--r--   0 playerone   (501) staff       (20)     8840 2023-07-04 13:57:11.000000 parametricGarch-0.0.1/parametricGarch/parametric.py
-drwxr-xr-x   0 playerone   (501) staff       (20)        0 2023-07-04 18:04:18.568742 parametricGarch-0.0.1/parametricGarch.egg-info/
--rw-r--r--   0 playerone   (501) staff       (20)     1158 2023-07-04 18:04:17.000000 parametricGarch-0.0.1/parametricGarch.egg-info/PKG-INFO
--rw-r--r--   0 playerone   (501) staff       (20)      278 2023-07-04 18:04:18.000000 parametricGarch-0.0.1/parametricGarch.egg-info/SOURCES.txt
--rw-r--r--   0 playerone   (501) staff       (20)        1 2023-07-04 18:04:17.000000 parametricGarch-0.0.1/parametricGarch.egg-info/dependency_links.txt
--rw-r--r--   0 playerone   (501) staff       (20)       11 2023-07-04 18:04:18.000000 parametricGarch-0.0.1/parametricGarch.egg-info/requires.txt
--rw-r--r--   0 playerone   (501) staff       (20)       16 2023-07-04 18:04:18.000000 parametricGarch-0.0.1/parametricGarch.egg-info/top_level.txt
--rw-r--r--   0 playerone   (501) staff       (20)       38 2023-07-04 18:04:18.569575 parametricGarch-0.0.1/setup.cfg
--rw-r--r--   0 playerone   (501) staff       (20)     1787 2023-07-04 18:04:14.000000 parametricGarch-0.0.1/setup.py
+drwxr-xr-x   0 playerone   (501) staff       (20)        0 2023-07-09 20:41:17.912311 parametricGarch-0.0.2/
+-rw-r--r--   0 playerone   (501) staff       (20)    35148 2023-07-04 17:25:08.000000 parametricGarch-0.0.2/LICENSE
+-rw-r--r--   0 playerone   (501) staff       (20)     1167 2023-07-09 20:41:17.911929 parametricGarch-0.0.2/PKG-INFO
+-rw-r--r--   0 playerone   (501) staff       (20)     2190 2023-07-09 20:31:59.000000 parametricGarch-0.0.2/README.md
+drwxr-xr-x   0 playerone   (501) staff       (20)        0 2023-07-09 20:41:17.907796 parametricGarch-0.0.2/parametricGarch/
+-rw-r--r--   0 playerone   (501) staff       (20)       45 2023-07-04 17:29:41.000000 parametricGarch-0.0.2/parametricGarch/__init__.py
+-rw-r--r--   0 playerone   (501) staff       (20)    11642 2023-07-06 15:32:05.000000 parametricGarch-0.0.2/parametricGarch/parametric.py
+drwxr-xr-x   0 playerone   (501) staff       (20)        0 2023-07-09 20:41:17.911442 parametricGarch-0.0.2/parametricGarch.egg-info/
+-rw-r--r--   0 playerone   (501) staff       (20)     1167 2023-07-09 20:41:17.000000 parametricGarch-0.0.2/parametricGarch.egg-info/PKG-INFO
+-rw-r--r--   0 playerone   (501) staff       (20)      278 2023-07-09 20:41:17.000000 parametricGarch-0.0.2/parametricGarch.egg-info/SOURCES.txt
+-rw-r--r--   0 playerone   (501) staff       (20)        1 2023-07-09 20:41:17.000000 parametricGarch-0.0.2/parametricGarch.egg-info/dependency_links.txt
+-rw-r--r--   0 playerone   (501) staff       (20)       24 2023-07-09 20:41:17.000000 parametricGarch-0.0.2/parametricGarch.egg-info/requires.txt
+-rw-r--r--   0 playerone   (501) staff       (20)       16 2023-07-09 20:41:17.000000 parametricGarch-0.0.2/parametricGarch.egg-info/top_level.txt
+-rw-r--r--   0 playerone   (501) staff       (20)       38 2023-07-09 20:41:17.912413 parametricGarch-0.0.2/setup.cfg
+-rw-r--r--   0 playerone   (501) staff       (20)     1815 2023-07-09 20:34:25.000000 parametricGarch-0.0.2/setup.py
```

### Comparing `parametricGarch-0.0.1/LICENSE` & `parametricGarch-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `parametricGarch-0.0.1/PKG-INFO` & `parametricGarch-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: parametricGarch
-Version: 0.0.1
+Version: 0.0.2
 Summary: Parametric Bootstrapping via the GARCH model
 Home-page: https://github.com/chideraani/ParametricGarch
 Author: Chidera
 Author-email: chideraani27@gmail.com
 License: GNU
 Keywords: python,bootstrapping,garch,volatility,VaR,risk management,parametric bootstrapping
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
```

### Comparing `parametricGarch-0.0.1/parametricGarch.egg-info/PKG-INFO` & `parametricGarch-0.0.2/parametricGarch.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: parametricGarch
-Version: 0.0.1
+Version: 0.0.2
 Summary: Parametric Bootstrapping via the GARCH model
 Home-page: https://github.com/chideraani/ParametricGarch
 Author: Chidera
 Author-email: chideraani27@gmail.com
 License: GNU
 Keywords: python,bootstrapping,garch,volatility,VaR,risk management,parametric bootstrapping
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
```

### Comparing `parametricGarch-0.0.1/setup.py` & `parametricGarch-0.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,34 +13,34 @@
     long_description = f.read()
 
 LONG_DESCRIPTION = 'A package that estimates the Volatility and Value-at-Risk (VaR) of financial assets using parametric bootstrapping via the GARCH model'
 
 # This call to setup() does all the work
 setup(
     name="parametricGarch",
-    version="0.0.1",
+    version="0.0.2",
     description="Parametric Bootstrapping via the GARCH model",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/chideraani/ParametricGarch",
     author="Chidera",
     author_email="chideraani27@gmail.com",
     license="GNU",
     keywords=['python', 'bootstrapping', 'garch', 'volatility', 'VaR', 'risk management', 'parametric bootstrapping'],
     classifiers=[
         "Intended Audience :: Developers",
         "Intended Audience :: Financial and Insurance Industry",
         "Natural Language :: English",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-        "Development Status :: 1 - Planning",
+        "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent"
     ],
     packages=["parametricGarch"],
     include_package_data=True,
-    install_requires=["numpy", "arch"]
+    install_requires=["numpy", "arch", "pandas", "scipy"]
 )
```

