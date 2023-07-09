# Comparing `tmp/finqual-0.1.93.tar.gz` & `tmp/finqual-0.1.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finqual-0.1.93.tar", last modified: Sun Jul  9 18:35:01 2023, max compression
+gzip compressed data, was "finqual-0.1.94.tar", last modified: Sun Jul  9 18:37:24 2023, max compression
```

## Comparing `finqual-0.1.93.tar` & `finqual-0.1.94.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 18:35:01.254800 finqual-0.1.93/
--rw-rw-rw-   0        0        0     1091 2023-05-30 17:24:17.000000 finqual-0.1.93/LICENSE.txt
--rw-rw-rw-   0        0        0     2464 2023-07-09 18:35:01.253799 finqual-0.1.93/PKG-INFO
--rw-rw-rw-   0        0        0     1941 2023-07-09 17:41:58.000000 finqual-0.1.93/README.md
-drwxrwxrwx   0        0        0        0 2023-07-09 18:35:01.244270 finqual-0.1.93/finqual/
--rw-rw-rw-   0        0        0        0 2023-05-17 21:28:31.000000 finqual-0.1.93/finqual/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 18:35:01.252797 finqual-0.1.93/finqual/data/
--rw-rw-rw-   0        0        0   434839 2023-06-14 22:18:44.000000 finqual-0.1.93/finqual/data/sec_sic.csv
--rw-rw-rw-   0        0        0   120213 2023-07-09 18:34:46.000000 finqual-0.1.93/finqual/finqual.py
-drwxrwxrwx   0        0        0        0 2023-07-09 18:35:01.252797 finqual-0.1.93/finqual.egg-info/
--rw-rw-rw-   0        0        0     2464 2023-07-09 18:35:01.000000 finqual-0.1.93/finqual.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-07-09 18:35:01.000000 finqual-0.1.93/finqual.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 18:35:01.000000 finqual-0.1.93/finqual.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-09 18:35:01.000000 finqual-0.1.93/finqual.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-09 18:35:01.254800 finqual-0.1.93/setup.cfg
--rw-rw-rw-   0        0        0      833 2023-07-09 18:34:38.000000 finqual-0.1.93/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:37:24.003379 finqual-0.1.94/
+-rw-rw-rw-   0        0        0     1091 2023-05-30 17:24:17.000000 finqual-0.1.94/LICENSE.txt
+-rw-rw-rw-   0        0        0     2464 2023-07-09 18:37:24.003379 finqual-0.1.94/PKG-INFO
+-rw-rw-rw-   0        0        0     1941 2023-07-09 17:41:58.000000 finqual-0.1.94/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 18:37:23.994370 finqual-0.1.94/finqual/
+-rw-rw-rw-   0        0        0        0 2023-05-17 21:28:31.000000 finqual-0.1.94/finqual/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:37:24.002378 finqual-0.1.94/finqual/data/
+-rw-rw-rw-   0        0        0   434839 2023-06-14 22:18:44.000000 finqual-0.1.94/finqual/data/sec_sic.csv
+-rw-rw-rw-   0        0        0   120205 2023-07-09 18:36:59.000000 finqual-0.1.94/finqual/finqual.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:37:24.002378 finqual-0.1.94/finqual.egg-info/
+-rw-rw-rw-   0        0        0     2464 2023-07-09 18:37:23.000000 finqual-0.1.94/finqual.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-07-09 18:37:23.000000 finqual-0.1.94/finqual.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 18:37:23.000000 finqual-0.1.94/finqual.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-09 18:37:23.000000 finqual-0.1.94/finqual.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-09 18:37:24.004625 finqual-0.1.94/setup.cfg
+-rw-rw-rw-   0        0        0      833 2023-07-09 18:37:08.000000 finqual-0.1.94/setup.py
```

### Comparing `finqual-0.1.93/LICENSE.txt` & `finqual-0.1.94/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `finqual-0.1.93/PKG-INFO` & `finqual-0.1.94/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finqual
-Version: 0.1.93
+Version: 0.1.94
 Summary: A package to retrieve historical fundamental financial data such as income statement, balance sheet, and cash flow statement directly from the SEC with no request caps and fast request rate limits.
 Author: Myztika
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `finqual-0.1.93/README.md` & `finqual-0.1.94/README.md`

 * *Files identical despite different names*

### Comparing `finqual-0.1.93/finqual/data/sec_sic.csv` & `finqual-0.1.94/finqual/data/sec_sic.csv`

 * *Files identical despite different names*

### Comparing `finqual-0.1.93/finqual/finqual.py` & `finqual-0.1.94/finqual/finqual.py`

 * *Files 0% similar despite different names*

```diff
@@ -548,15 +548,15 @@
             return df
 
     def comparables(self, n, level = None):
 
         if level == None:
             level = 4
 
-        sic = pd.read_csv('finqual/data/sec_sic.csv', index_col=0)
+        sic = pd.read_csv('data/sec_sic.csv', index_col=0)
         sic = sic.dropna()
 
         sic["SIC"] = sic["SIC"].astype(int)
         sic["SIC"] = sic["SIC"].astype(str)
         sic['SIC'] = sic['SIC'].apply(lambda x: x[:level])
         sic["SIC"] = sic["SIC"].astype(int)
```

### Comparing `finqual-0.1.93/finqual.egg-info/PKG-INFO` & `finqual-0.1.94/finqual.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finqual
-Version: 0.1.93
+Version: 0.1.94
 Summary: A package to retrieve historical fundamental financial data such as income statement, balance sheet, and cash flow statement directly from the SEC with no request caps and fast request rate limits.
 Author: Myztika
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `finqual-0.1.93/setup.py` & `finqual-0.1.94/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 
 with open('README.md', 'r') as readme_file:
     long_description = readme_file.read()
 
 setup(
     name='finqual',
-    version='0.1.93',
+    version='0.1.94',
     description='A package to retrieve historical fundamental financial data such as income statement, balance sheet, and cash flow statement directly from the SEC with no request caps and fast request rate limits.',
     author='Myztika',
     packages=['finqual'],
     package_dir = {'finqual':"finqual"},
     package_data={'finqual': ['data/*.csv']},
     long_description=long_description,
     long_description_content_type='text/markdown',
```

