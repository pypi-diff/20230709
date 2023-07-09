# Comparing `tmp/finqual-0.1.8.tar.gz` & `tmp/finqual-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finqual-0.1.8.tar", last modified: Sun Jul  9 17:38:33 2023, max compression
+gzip compressed data, was "finqual-0.1.9.tar", last modified: Sun Jul  9 18:21:29 2023, max compression
```

## Comparing `finqual-0.1.8.tar` & `finqual-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 17:38:33.263412 finqual-0.1.8/
--rw-rw-rw-   0        0        0     1091 2023-05-30 17:24:17.000000 finqual-0.1.8/LICENSE.txt
--rw-rw-rw-   0        0        0     2483 2023-07-09 17:38:33.263412 finqual-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1945 2023-06-08 21:03:22.000000 finqual-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-09 17:38:33.257397 finqual-0.1.8/finqual/
--rw-rw-rw-   0        0        0        0 2023-05-17 21:28:31.000000 finqual-0.1.8/finqual/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 17:38:33.261910 finqual-0.1.8/finqual/data/
--rw-rw-rw-   0        0        0   434839 2023-06-14 22:18:44.000000 finqual-0.1.8/finqual/data/sec_sic.csv
--rw-rw-rw-   0        0        0   120205 2023-07-09 17:37:48.000000 finqual-0.1.8/finqual/finqual.py
-drwxrwxrwx   0        0        0        0 2023-07-09 17:38:33.260909 finqual-0.1.8/finqual.egg-info/
--rw-rw-rw-   0        0        0     2483 2023-07-09 17:38:33.000000 finqual-0.1.8/finqual.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-07-09 17:38:33.000000 finqual-0.1.8/finqual.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 17:38:33.000000 finqual-0.1.8/finqual.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-09 17:38:33.000000 finqual-0.1.8/finqual.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-09 17:38:33.263412 finqual-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      790 2023-07-09 17:12:09.000000 finqual-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:21:29.971056 finqual-0.1.9/
+-rw-rw-rw-   0        0        0     1091 2023-05-30 17:24:17.000000 finqual-0.1.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     2463 2023-07-09 18:21:29.970055 finqual-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1941 2023-07-09 17:41:58.000000 finqual-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 18:21:29.959054 finqual-0.1.9/finqual/
+-rw-rw-rw-   0        0        0        0 2023-05-17 21:28:31.000000 finqual-0.1.9/finqual/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:21:29.969052 finqual-0.1.9/finqual/data/
+-rw-rw-rw-   0        0        0   434839 2023-06-14 22:18:44.000000 finqual-0.1.9/finqual/data/sec_sic.csv
+-rw-rw-rw-   0        0        0   120213 2023-07-09 18:20:53.000000 finqual-0.1.9/finqual/finqual.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:21:29.969052 finqual-0.1.9/finqual.egg-info/
+-rw-rw-rw-   0        0        0     2463 2023-07-09 18:21:29.000000 finqual-0.1.9/finqual.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-07-09 18:21:29.000000 finqual-0.1.9/finqual.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 18:21:29.000000 finqual-0.1.9/finqual.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-09 18:21:29.000000 finqual-0.1.9/finqual.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-09 18:21:29.971056 finqual-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      790 2023-07-09 18:20:59.000000 finqual-0.1.9/setup.py
```

### Comparing `finqual-0.1.8/LICENSE.txt` & `finqual-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `finqual-0.1.8/PKG-INFO` & `finqual-0.1.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finqual
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package to retrieve historical fundamental financial data such as income statement, balance sheet, and cash flow statement directly from the SEC with no request caps and fast request rate limits.
 Author: Myztika
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -39,17 +39,17 @@
 
 ## Dependencies
 
 Only four packages are required, with the following versions confirmed to be working:
 
 | Package   | Version  |
 |-----------|----------|
-| pandas    | â‰¥ 2.0.2  |
-| numpy     | â‰¥ 1.24.3 |
-| requests  | â‰¥ 2.31.0 |
-| ratelimit | â‰¥ 2.2.1  |
+| pandas    | >= 2.0.2  |
+| numpy     | >= 1.24.3 |
+| requests  | >= 2.31.0 |
+| ratelimit | >= 2.2.1  |
 
 ## Limitations
 Currently, there are several known limitations that I am aware of from my own testing. These are still to be looked at:
 
 - Missing data values for companies, this is mostly due to companies using custom tags that are not accessible via the SEC database, and quite prevalent for quarterly reports as well
 - More comprehensive mappings from known tags
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `finqual-0.1.8/README.md` & `finqual-0.1.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 
 ## Dependencies
 
 Only four packages are required, with the following versions confirmed to be working:
 
 | Package   | Version  |
 |-----------|----------|
-| pandas    | ≥ 2.0.2  |
-| numpy     | ≥ 1.24.3 |
-| requests  | ≥ 2.31.0 |
-| ratelimit | ≥ 2.2.1  |
+| pandas    | >= 2.0.2  |
+| numpy     | >= 1.24.3 |
+| requests  | >= 2.31.0 |
+| ratelimit | >= 2.2.1  |
 
 ## Limitations
 Currently, there are several known limitations that I am aware of from my own testing. These are still to be looked at:
 
 - Missing data values for companies, this is mostly due to companies using custom tags that are not accessible via the SEC database, and quite prevalent for quarterly reports as well
 - More comprehensive mappings from known tags
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `finqual-0.1.8/finqual/data/sec_sic.csv` & `finqual-0.1.9/finqual/data/sec_sic.csv`

 * *Files identical despite different names*

### Comparing `finqual-0.1.8/finqual/finqual.py` & `finqual-0.1.9/finqual/finqual.py`

 * *Files 0% similar despite different names*

```diff
@@ -548,15 +548,15 @@
             return df
 
     def comparables(self, n, level = None):
 
         if level == None:
             level = 4
 
-        sic = pd.read_csv('data/sec_sic.csv', index_col=0)
+        sic = pd.read_csv('finqual/data/sec_sic.csv', index_col=0)
         sic = sic.dropna()
 
         sic["SIC"] = sic["SIC"].astype(int)
         sic["SIC"] = sic["SIC"].astype(str)
         sic['SIC'] = sic['SIC'].apply(lambda x: x[:level])
         sic["SIC"] = sic["SIC"].astype(int)
```

### Comparing `finqual-0.1.8/finqual.egg-info/PKG-INFO` & `finqual-0.1.9/finqual.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finqual
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package to retrieve historical fundamental financial data such as income statement, balance sheet, and cash flow statement directly from the SEC with no request caps and fast request rate limits.
 Author: Myztika
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -39,17 +39,17 @@
 
 ## Dependencies
 
 Only four packages are required, with the following versions confirmed to be working:
 
 | Package   | Version  |
 |-----------|----------|
-| pandas    | â‰¥ 2.0.2  |
-| numpy     | â‰¥ 1.24.3 |
-| requests  | â‰¥ 2.31.0 |
-| ratelimit | â‰¥ 2.2.1  |
+| pandas    | >= 2.0.2  |
+| numpy     | >= 1.24.3 |
+| requests  | >= 2.31.0 |
+| ratelimit | >= 2.2.1  |
 
 ## Limitations
 Currently, there are several known limitations that I am aware of from my own testing. These are still to be looked at:
 
 - Missing data values for companies, this is mostly due to companies using custom tags that are not accessible via the SEC database, and quite prevalent for quarterly reports as well
 - More comprehensive mappings from known tags
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `finqual-0.1.8/setup.py` & `finqual-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 
 with open('README.md', 'r') as readme_file:
     long_description = readme_file.read()
 
 setup(
     name='finqual',
-    version='0.1.8',
+    version='0.1.9',
     description='A package to retrieve historical fundamental financial data such as income statement, balance sheet, and cash flow statement directly from the SEC with no request caps and fast request rate limits.',
     author='Myztika',
     packages=['finqual'],
     package_data={'finqual': ['data/*.csv']},
     long_description=long_description,
     long_description_content_type='text/markdown',
     python_requires='>=3.7',
```

