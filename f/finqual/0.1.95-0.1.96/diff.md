# Comparing `tmp/finqual-0.1.95.tar.gz` & `tmp/finqual-0.1.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finqual-0.1.95.tar", last modified: Sun Jul  9 20:23:42 2023, max compression
+gzip compressed data, was "finqual-0.1.96.tar", last modified: Sun Jul  9 21:10:50 2023, max compression
```

## Comparing `finqual-0.1.95.tar` & `finqual-0.1.96.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 20:23:42.704474 finqual-0.1.95/
--rw-rw-rw-   0        0        0     1091 2023-05-30 17:24:17.000000 finqual-0.1.95/LICENSE.txt
--rw-rw-rw-   0        0        0     2491 2023-07-09 20:23:42.704474 finqual-0.1.95/PKG-INFO
--rw-rw-rw-   0        0        0     1968 2023-07-09 19:52:56.000000 finqual-0.1.95/README.md
-drwxrwxrwx   0        0        0        0 2023-07-09 20:23:42.698689 finqual-0.1.95/finqual/
--rw-rw-rw-   0        0        0        0 2023-05-17 21:28:31.000000 finqual-0.1.95/finqual/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 20:23:42.703204 finqual-0.1.95/finqual/data/
--rw-rw-rw-   0        0        0   434839 2023-06-14 22:18:44.000000 finqual-0.1.95/finqual/data/sec_sic.csv
--rw-rw-rw-   0        0        0   120333 2023-07-09 19:51:21.000000 finqual-0.1.95/finqual/finqual.py
-drwxrwxrwx   0        0        0        0 2023-07-09 20:23:42.702194 finqual-0.1.95/finqual.egg-info/
--rw-rw-rw-   0        0        0     2491 2023-07-09 20:23:42.000000 finqual-0.1.95/finqual.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-07-09 20:23:42.000000 finqual-0.1.95/finqual.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 20:23:42.000000 finqual-0.1.95/finqual.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-09 20:23:42.000000 finqual-0.1.95/finqual.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-09 20:23:42.704474 finqual-0.1.95/setup.cfg
--rw-rw-rw-   0        0        0      833 2023-07-09 19:51:25.000000 finqual-0.1.95/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 21:10:50.236621 finqual-0.1.96/
+-rw-rw-rw-   0        0        0     1091 2023-05-30 17:24:17.000000 finqual-0.1.96/LICENSE.txt
+-rw-rw-rw-   0        0        0     2491 2023-07-09 21:10:50.235621 finqual-0.1.96/PKG-INFO
+-rw-rw-rw-   0        0        0     1968 2023-07-09 19:52:56.000000 finqual-0.1.96/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 21:10:50.225102 finqual-0.1.96/finqual/
+-rw-rw-rw-   0        0        0        0 2023-05-17 21:28:31.000000 finqual-0.1.96/finqual/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 21:10:50.234619 finqual-0.1.96/finqual/data/
+-rw-rw-rw-   0        0        0   434839 2023-06-14 22:18:44.000000 finqual-0.1.96/finqual/data/sec_sic.csv
+-rw-rw-rw-   0        0        0   120333 2023-07-09 21:10:07.000000 finqual-0.1.96/finqual/finqual.py
+drwxrwxrwx   0        0        0        0 2023-07-09 21:10:50.234619 finqual-0.1.96/finqual.egg-info/
+-rw-rw-rw-   0        0        0     2491 2023-07-09 21:10:50.000000 finqual-0.1.96/finqual.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-07-09 21:10:50.000000 finqual-0.1.96/finqual.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 21:10:50.000000 finqual-0.1.96/finqual.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-09 21:10:50.000000 finqual-0.1.96/finqual.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-09 21:10:50.236621 finqual-0.1.96/setup.cfg
+-rw-rw-rw-   0        0        0      833 2023-07-09 21:10:12.000000 finqual-0.1.96/setup.py
```

### Comparing `finqual-0.1.95/LICENSE.txt` & `finqual-0.1.96/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `finqual-0.1.95/PKG-INFO` & `finqual-0.1.96/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finqual
-Version: 0.1.95
+Version: 0.1.96
 Summary: A package to retrieve historical fundamental financial data such as income statement, balance sheet, and cash flow statement directly from the SEC with no request caps and fast request rate limits.
 Author: Myztika
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `finqual-0.1.95/README.md` & `finqual-0.1.96/README.md`

 * *Files identical despite different names*

### Comparing `finqual-0.1.95/finqual/data/sec_sic.csv` & `finqual-0.1.96/finqual/data/sec_sic.csv`

 * *Files identical despite different names*

### Comparing `finqual-0.1.95/finqual/finqual.py` & `finqual-0.1.96/finqual/finqual.py`

 * *Files 0% similar despite different names*

```diff
@@ -552,15 +552,15 @@
 
         this_dir, this_filename = os.path.split(__file__)
         sic_path = os.path.join(this_dir, "data", "sec_sic.csv")
 
         if level == None:
             level = 4
 
-        sic = pd.read_csv(sec_path, index_col=0)
+        sic = pd.read_csv(sic_path, index_col=0)
         sic = sic.dropna()
 
         sic["SIC"] = sic["SIC"].astype(int)
         sic["SIC"] = sic["SIC"].astype(str)
         sic['SIC'] = sic['SIC'].apply(lambda x: x[:level])
         sic["SIC"] = sic["SIC"].astype(int)
```

### Comparing `finqual-0.1.95/finqual.egg-info/PKG-INFO` & `finqual-0.1.96/finqual.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finqual
-Version: 0.1.95
+Version: 0.1.96
 Summary: A package to retrieve historical fundamental financial data such as income statement, balance sheet, and cash flow statement directly from the SEC with no request caps and fast request rate limits.
 Author: Myztika
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `finqual-0.1.95/setup.py` & `finqual-0.1.96/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 
 with open('README.md', 'r') as readme_file:
     long_description = readme_file.read()
 
 setup(
     name='finqual',
-    version='0.1.95',
+    version='0.1.96',
     description='A package to retrieve historical fundamental financial data such as income statement, balance sheet, and cash flow statement directly from the SEC with no request caps and fast request rate limits.',
     author='Myztika',
     packages=['finqual'],
     package_dir = {'finqual':"finqual"},
     package_data={'finqual': ['data/*.csv']},
     long_description=long_description,
     long_description_content_type='text/markdown',
```

