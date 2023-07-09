# Comparing `tmp/finqual-0.1.91.tar.gz` & `tmp/finqual-0.1.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finqual-0.1.91.tar", last modified: Sun Jul  9 18:25:16 2023, max compression
+gzip compressed data, was "finqual-0.1.92.tar", last modified: Sun Jul  9 18:26:48 2023, max compression
```

## Comparing `finqual-0.1.91.tar` & `finqual-0.1.92.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 18:25:16.085923 finqual-0.1.91/
--rw-rw-rw-   0        0        0     1091 2023-05-30 17:24:17.000000 finqual-0.1.91/LICENSE.txt
--rw-rw-rw-   0        0        0     2464 2023-07-09 18:25:16.084922 finqual-0.1.91/PKG-INFO
--rw-rw-rw-   0        0        0     1941 2023-07-09 17:41:58.000000 finqual-0.1.91/README.md
-drwxrwxrwx   0        0        0        0 2023-07-09 18:25:16.074933 finqual-0.1.91/finqual/
--rw-rw-rw-   0        0        0        0 2023-05-17 21:28:31.000000 finqual-0.1.91/finqual/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 18:25:16.083920 finqual-0.1.91/finqual/data/
--rw-rw-rw-   0        0        0   434839 2023-06-14 22:18:44.000000 finqual-0.1.91/finqual/data/sec_sic.csv
--rw-rw-rw-   0        0        0   120213 2023-07-09 18:20:53.000000 finqual-0.1.91/finqual/finqual.py
-drwxrwxrwx   0        0        0        0 2023-07-09 18:25:16.083920 finqual-0.1.91/finqual.egg-info/
--rw-rw-rw-   0        0        0     2464 2023-07-09 18:25:16.000000 finqual-0.1.91/finqual.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-07-09 18:25:16.000000 finqual-0.1.91/finqual.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 18:25:16.000000 finqual-0.1.91/finqual.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-09 18:25:16.000000 finqual-0.1.91/finqual.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-09 18:25:16.085923 finqual-0.1.91/setup.cfg
--rw-rw-rw-   0        0        0      791 2023-07-09 18:24:49.000000 finqual-0.1.91/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:26:48.435324 finqual-0.1.92/
+-rw-rw-rw-   0        0        0     1091 2023-05-30 17:24:17.000000 finqual-0.1.92/LICENSE.txt
+-rw-rw-rw-   0        0        0     2464 2023-07-09 18:26:48.435324 finqual-0.1.92/PKG-INFO
+-rw-rw-rw-   0        0        0     1941 2023-07-09 17:41:58.000000 finqual-0.1.92/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 18:26:48.426316 finqual-0.1.92/finqual/
+-rw-rw-rw-   0        0        0        0 2023-05-17 21:28:31.000000 finqual-0.1.92/finqual/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:26:48.434324 finqual-0.1.92/finqual/data/
+-rw-rw-rw-   0        0        0   434839 2023-06-14 22:18:44.000000 finqual-0.1.92/finqual/data/sec_sic.csv
+-rw-rw-rw-   0        0        0   120228 2023-07-09 18:26:25.000000 finqual-0.1.92/finqual/finqual.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:26:48.433323 finqual-0.1.92/finqual.egg-info/
+-rw-rw-rw-   0        0        0     2464 2023-07-09 18:26:48.000000 finqual-0.1.92/finqual.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-07-09 18:26:48.000000 finqual-0.1.92/finqual.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 18:26:48.000000 finqual-0.1.92/finqual.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-09 18:26:48.000000 finqual-0.1.92/finqual.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-09 18:26:48.435324 finqual-0.1.92/setup.cfg
+-rw-rw-rw-   0        0        0      791 2023-07-09 18:26:40.000000 finqual-0.1.92/setup.py
```

### Comparing `finqual-0.1.91/LICENSE.txt` & `finqual-0.1.92/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `finqual-0.1.91/PKG-INFO` & `finqual-0.1.92/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finqual
-Version: 0.1.91
+Version: 0.1.92
 Summary: A package to retrieve historical fundamental financial data such as income statement, balance sheet, and cash flow statement directly from the SEC with no request caps and fast request rate limits.
 Author: Myztika
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `finqual-0.1.91/README.md` & `finqual-0.1.92/README.md`

 * *Files identical despite different names*

### Comparing `finqual-0.1.91/finqual/data/sec_sic.csv` & `finqual-0.1.92/finqual/data/sec_sic.csv`

 * *Files identical despite different names*

### Comparing `finqual-0.1.91/finqual/finqual.py` & `finqual-0.1.92/finqual/finqual.py`

 * *Files 0% similar despite different names*

```diff
@@ -549,14 +549,15 @@
 
     def comparables(self, n, level = None):
 
         if level == None:
             level = 4
 
         sic = pd.read_csv('finqual/data/sec_sic.csv', index_col=0)
+        #test
         sic = sic.dropna()
 
         sic["SIC"] = sic["SIC"].astype(int)
         sic["SIC"] = sic["SIC"].astype(str)
         sic['SIC'] = sic['SIC'].apply(lambda x: x[:level])
         sic["SIC"] = sic["SIC"].astype(int)
```

### Comparing `finqual-0.1.91/finqual.egg-info/PKG-INFO` & `finqual-0.1.92/finqual.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finqual
-Version: 0.1.91
+Version: 0.1.92
 Summary: A package to retrieve historical fundamental financial data such as income statement, balance sheet, and cash flow statement directly from the SEC with no request caps and fast request rate limits.
 Author: Myztika
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `finqual-0.1.91/setup.py` & `finqual-0.1.92/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 
 with open('README.md', 'r') as readme_file:
     long_description = readme_file.read()
 
 setup(
     name='finqual',
-    version='0.1.91',
+    version='0.1.92',
     description='A package to retrieve historical fundamental financial data such as income statement, balance sheet, and cash flow statement directly from the SEC with no request caps and fast request rate limits.',
     author='Myztika',
     packages=['finqual'],
     package_data={'finqual': ['data/*.csv']},
     long_description=long_description,
     long_description_content_type='text/markdown',
     python_requires='>=3.7',
```

