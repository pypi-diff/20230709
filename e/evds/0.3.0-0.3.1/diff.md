# Comparing `tmp/evds-0.3.0.tar.gz` & `tmp/evds-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evds-0.3.0.tar", last modified: Sun Jul  9 13:09:06 2023, max compression
+gzip compressed data, was "evds-0.3.1.tar", last modified: Sun Jul  9 14:00:50 2023, max compression
```

## Comparing `evds-0.3.0.tar` & `evds-0.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ege       (1000) ege       (1000)        0 2023-07-09 13:09:06.640123 evds-0.3.0/
--rw-r--r--   0 ege       (1000) ege       (1000)     1071 2023-07-09 11:31:39.000000 evds-0.3.0/LICENCE
--rw-r--r--   0 ege       (1000) ege       (1000)    10762 2023-07-09 13:09:06.640123 evds-0.3.0/PKG-INFO
--rw-r--r--   0 ege       (1000) ege       (1000)    10356 2023-07-09 13:02:24.000000 evds-0.3.0/README.md
-drwxr-xr-x   0 ege       (1000) ege       (1000)        0 2023-07-09 13:09:06.640123 evds-0.3.0/evds/
--rw-r--r--   0 ege       (1000) ege       (1000)    10195 2023-07-09 13:02:24.000000 evds-0.3.0/evds/__init__.py
-drwxr-xr-x   0 ege       (1000) ege       (1000)        0 2023-07-09 13:09:06.640123 evds-0.3.0/evds.egg-info/
--rw-r--r--   0 ege       (1000) ege       (1000)    10762 2023-07-09 13:09:06.000000 evds-0.3.0/evds.egg-info/PKG-INFO
--rw-r--r--   0 ege       (1000) ege       (1000)      182 2023-07-09 13:09:06.000000 evds-0.3.0/evds.egg-info/SOURCES.txt
--rw-r--r--   0 ege       (1000) ege       (1000)        1 2023-07-09 13:09:06.000000 evds-0.3.0/evds.egg-info/dependency_links.txt
--rw-r--r--   0 ege       (1000) ege       (1000)       24 2023-07-09 13:09:06.000000 evds-0.3.0/evds.egg-info/requires.txt
--rw-r--r--   0 ege       (1000) ege       (1000)        5 2023-07-09 13:09:06.000000 evds-0.3.0/evds.egg-info/top_level.txt
--rw-r--r--   0 ege       (1000) ege       (1000)       38 2023-07-09 13:09:06.640123 evds-0.3.0/setup.cfg
--rw-r--r--   0 ege       (1000) ege       (1000)      709 2023-07-09 13:02:24.000000 evds-0.3.0/setup.py
+drwxr-xr-x   0 ege       (1000) ege       (1000)        0 2023-07-09 14:00:50.711154 evds-0.3.1/
+-rw-r--r--   0 ege       (1000) ege       (1000)     1071 2023-07-09 13:53:18.000000 evds-0.3.1/LICENCE
+-rw-r--r--   0 ege       (1000) ege       (1000)    10762 2023-07-09 14:00:50.711154 evds-0.3.1/PKG-INFO
+-rw-r--r--   0 ege       (1000) ege       (1000)    10356 2023-07-09 13:53:18.000000 evds-0.3.1/README.md
+drwxr-xr-x   0 ege       (1000) ege       (1000)        0 2023-07-09 14:00:50.711154 evds-0.3.1/evds/
+-rw-r--r--   0 ege       (1000) ege       (1000)    10194 2023-07-09 13:59:50.000000 evds-0.3.1/evds/__init__.py
+drwxr-xr-x   0 ege       (1000) ege       (1000)        0 2023-07-09 14:00:50.711154 evds-0.3.1/evds.egg-info/
+-rw-r--r--   0 ege       (1000) ege       (1000)    10762 2023-07-09 14:00:50.000000 evds-0.3.1/evds.egg-info/PKG-INFO
+-rw-r--r--   0 ege       (1000) ege       (1000)      182 2023-07-09 14:00:50.000000 evds-0.3.1/evds.egg-info/SOURCES.txt
+-rw-r--r--   0 ege       (1000) ege       (1000)        1 2023-07-09 14:00:50.000000 evds-0.3.1/evds.egg-info/dependency_links.txt
+-rw-r--r--   0 ege       (1000) ege       (1000)       24 2023-07-09 14:00:50.000000 evds-0.3.1/evds.egg-info/requires.txt
+-rw-r--r--   0 ege       (1000) ege       (1000)        5 2023-07-09 14:00:50.000000 evds-0.3.1/evds.egg-info/top_level.txt
+-rw-r--r--   0 ege       (1000) ege       (1000)       38 2023-07-09 14:00:50.711154 evds-0.3.1/setup.cfg
+-rw-r--r--   0 ege       (1000) ege       (1000)      709 2023-07-09 13:59:50.000000 evds-0.3.1/setup.py
```

### Comparing `evds-0.3.0/LICENCE` & `evds-0.3.1/LICENCE`

 * *Files identical despite different names*

### Comparing `evds-0.3.0/PKG-INFO` & `evds-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evds
-Version: 0.3.0
+Version: 0.3.1
 Summary: EVDS python wrapper
 Home-page: https://github.com/fatihmete/evds
 Author: Fatih Mete
 Author-email: fatihmete@live.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `evds-0.3.0/README.md` & `evds-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `evds-0.3.0/evds/__init__.py` & `evds-0.3.1/evds/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     for more detail https://github.com/fatihmete/evds
     Example usage:
     from evds import evdsAPI
     evds = evdsAPI('EVDS_API_KEY')
     evds.get_data(['TP.DK.USD.A.YTL','TP.DK.EUR.A.YTL'], startdate="01-01-2019", enddate="01-01-2020")
     """
 
-    def __init__(self, key, lang="TR", DEBUG=False, proxies="", httpsVerify=True, legacySSL=False):
+    def __init__(self, key, lang="TR", DEBUG=False, proxies="", httpsVerify=True, legacySSL=True):
         self.key = key
         self.DEBUG = DEBUG
         self.proxies = proxies
         self.httpsVerify = httpsVerify
         self.legacySSL = legacySSL
 
         self.__create_session()
```

### Comparing `evds-0.3.0/evds.egg-info/PKG-INFO` & `evds-0.3.1/evds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evds
-Version: 0.3.0
+Version: 0.3.1
 Summary: EVDS python wrapper
 Home-page: https://github.com/fatihmete/evds
 Author: Fatih Mete
 Author-email: fatihmete@live.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `evds-0.3.0/setup.py` & `evds-0.3.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="evds",
-    version="0.3.0",
+    version="0.3.1",
     author="Fatih Mete",
     author_email="fatihmete@live.com",
     description="EVDS python wrapper",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/fatihmete/evds",
     packages=setuptools.find_packages(),
```

