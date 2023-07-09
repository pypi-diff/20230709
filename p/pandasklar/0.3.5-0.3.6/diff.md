# Comparing `tmp/pandasklar-0.3.5.tar.gz` & `tmp/pandasklar-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasklar-0.3.5.tar", last modified: Sat Jun 17 20:47:35 2023, max compression
+gzip compressed data, was "pandasklar-0.3.6.tar", last modified: Sun Jul  9 19:56:08 2023, max compression
```

## Comparing `pandasklar-0.3.5.tar` & `pandasklar-0.3.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-17 20:47:35.803096 pandasklar-0.3.5/
--rw-r--r--   0 me        (1000) me        (1000)     1063 2022-09-06 17:06:11.000000 pandasklar-0.3.5/LICENSE
--rw-rw-r--   0 me        (1000) me        (1000)     9805 2023-06-17 20:47:35.803096 pandasklar-0.3.5/PKG-INFO
--rw-r--r--   0 me        (1000) me        (1000)     9297 2023-06-17 20:46:52.000000 pandasklar-0.3.5/README.md
--rw-r--r--   0 me        (1000) me        (1000)     1301 2023-06-17 20:46:44.000000 pandasklar-0.3.5/pyproject.toml
--rw-rw-r--   0 me        (1000) me        (1000)       38 2023-06-17 20:47:35.803096 pandasklar-0.3.5/setup.cfg
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-17 20:47:35.407100 pandasklar-0.3.5/src/
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-17 20:47:35.783096 pandasklar-0.3.5/src/pandasklar/
--rw-r--r--   0 me        (1000) me        (1000)      537 2023-02-13 16:45:54.000000 pandasklar-0.3.5/src/pandasklar/__init__.py
--rw-r--r--   0 me        (1000) me        (1000)      214 2023-02-14 22:57:35.000000 pandasklar-0.3.5/src/pandasklar/__main__.py
--rw-r--r--   0 me        (1000) me        (1000)    19899 2023-05-12 20:23:55.000000 pandasklar-0.3.5/src/pandasklar/aggregate.py
--rw-r--r--   0 me        (1000) me        (1000)    28272 2023-06-16 15:41:42.000000 pandasklar-0.3.5/src/pandasklar/analyse.py
--rw-r--r--   0 me        (1000) me        (1000)    10330 2023-02-12 20:17:03.000000 pandasklar-0.3.5/src/pandasklar/compare.py
--rw-r--r--   0 me        (1000) me        (1000)     1092 2023-02-19 10:51:49.000000 pandasklar-0.3.5/src/pandasklar/config.py
--rw-r--r--   0 me        (1000) me        (1000)    27326 2023-06-16 08:25:57.000000 pandasklar-0.3.5/src/pandasklar/content.py
--rw-r--r--   0 me        (1000) me        (1000)     8710 2023-03-11 11:39:52.000000 pandasklar-0.3.5/src/pandasklar/develop.py
--rw-r--r--   0 me        (1000) me        (1000)    32239 2023-03-16 08:54:51.000000 pandasklar-0.3.5/src/pandasklar/pandas.py
--rw-rw-r--   0 me        (1000) me        (1000)     2613 2023-02-13 21:21:37.000000 pandasklar-0.3.5/src/pandasklar/plot.py
--rw-r--r--   0 me        (1000) me        (1000)     4827 2023-02-08 06:49:03.000000 pandasklar-0.3.5/src/pandasklar/rank.py
--rw-r--r--   0 me        (1000) me        (1000)     8464 2023-02-12 21:40:20.000000 pandasklar-0.3.5/src/pandasklar/scale.py
--rw-r--r--   0 me        (1000) me        (1000)     9244 2023-06-16 08:47:39.000000 pandasklar-0.3.5/src/pandasklar/string.py
--rw-r--r--   0 me        (1000) me        (1000)     8810 2022-11-12 13:55:33.000000 pandasklar-0.3.5/src/pandasklar/subsets.py
--rw-r--r--   0 me        (1000) me        (1000)     5665 2023-06-09 20:00:34.000000 pandasklar-0.3.5/src/pandasklar/type_info.py
--rw-r--r--   0 me        (1000) me        (1000)     7796 2023-06-16 19:15:33.000000 pandasklar-0.3.5/src/pandasklar/values_info.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-17 20:47:35.803096 pandasklar-0.3.5/src/pandasklar.egg-info/
--rw-r--r--   0 me        (1000) me        (1000)     9805 2023-06-17 20:47:35.000000 pandasklar-0.3.5/src/pandasklar.egg-info/PKG-INFO
--rw-r--r--   0 me        (1000) me        (1000)      677 2023-06-17 20:47:35.000000 pandasklar-0.3.5/src/pandasklar.egg-info/SOURCES.txt
--rw-r--r--   0 me        (1000) me        (1000)        1 2023-06-17 20:47:35.000000 pandasklar-0.3.5/src/pandasklar.egg-info/dependency_links.txt
--rw-r--r--   0 me        (1000) me        (1000)       56 2023-06-17 20:47:35.000000 pandasklar-0.3.5/src/pandasklar.egg-info/entry_points.txt
--rw-r--r--   0 me        (1000) me        (1000)       47 2023-06-17 20:47:35.000000 pandasklar-0.3.5/src/pandasklar.egg-info/requires.txt
--rw-r--r--   0 me        (1000) me        (1000)       11 2023-06-17 20:47:35.000000 pandasklar-0.3.5/src/pandasklar.egg-info/top_level.txt
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-07-09 19:56:08.550866 pandasklar-0.3.6/
+-rw-r--r--   0 me        (1000) me        (1000)     1063 2022-09-06 17:06:11.000000 pandasklar-0.3.6/LICENSE
+-rw-rw-r--   0 me        (1000) me        (1000)     9874 2023-07-09 19:56:08.550866 pandasklar-0.3.6/PKG-INFO
+-rw-r--r--   0 me        (1000) me        (1000)     9366 2023-07-09 19:55:13.000000 pandasklar-0.3.6/README.md
+-rw-r--r--   0 me        (1000) me        (1000)     1301 2023-07-09 19:54:56.000000 pandasklar-0.3.6/pyproject.toml
+-rw-rw-r--   0 me        (1000) me        (1000)       38 2023-07-09 19:56:08.550866 pandasklar-0.3.6/setup.cfg
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-07-09 19:56:08.178869 pandasklar-0.3.6/src/
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-07-09 19:56:08.538866 pandasklar-0.3.6/src/pandasklar/
+-rw-r--r--   0 me        (1000) me        (1000)      537 2023-02-13 16:45:54.000000 pandasklar-0.3.6/src/pandasklar/__init__.py
+-rw-r--r--   0 me        (1000) me        (1000)      214 2023-02-14 22:57:35.000000 pandasklar-0.3.6/src/pandasklar/__main__.py
+-rw-r--r--   0 me        (1000) me        (1000)    19899 2023-05-12 20:23:55.000000 pandasklar-0.3.6/src/pandasklar/aggregate.py
+-rw-r--r--   0 me        (1000) me        (1000)    28272 2023-06-16 15:41:42.000000 pandasklar-0.3.6/src/pandasklar/analyse.py
+-rw-r--r--   0 me        (1000) me        (1000)    10412 2023-07-04 19:08:15.000000 pandasklar-0.3.6/src/pandasklar/compare.py
+-rw-r--r--   0 me        (1000) me        (1000)     1092 2023-02-19 10:51:49.000000 pandasklar-0.3.6/src/pandasklar/config.py
+-rw-r--r--   0 me        (1000) me        (1000)    27326 2023-06-16 08:25:57.000000 pandasklar-0.3.6/src/pandasklar/content.py
+-rw-r--r--   0 me        (1000) me        (1000)     8710 2023-03-11 11:39:52.000000 pandasklar-0.3.6/src/pandasklar/develop.py
+-rw-r--r--   0 me        (1000) me        (1000)    32239 2023-03-16 08:54:51.000000 pandasklar-0.3.6/src/pandasklar/pandas.py
+-rw-rw-r--   0 me        (1000) me        (1000)     2613 2023-02-13 21:21:37.000000 pandasklar-0.3.6/src/pandasklar/plot.py
+-rw-r--r--   0 me        (1000) me        (1000)     4827 2023-02-08 06:49:03.000000 pandasklar-0.3.6/src/pandasklar/rank.py
+-rw-r--r--   0 me        (1000) me        (1000)     8464 2023-02-12 21:40:20.000000 pandasklar-0.3.6/src/pandasklar/scale.py
+-rw-r--r--   0 me        (1000) me        (1000)    12190 2023-07-07 14:05:16.000000 pandasklar-0.3.6/src/pandasklar/string.py
+-rw-r--r--   0 me        (1000) me        (1000)     8810 2022-11-12 13:55:33.000000 pandasklar-0.3.6/src/pandasklar/subsets.py
+-rw-r--r--   0 me        (1000) me        (1000)     5665 2023-06-09 20:00:34.000000 pandasklar-0.3.6/src/pandasklar/type_info.py
+-rw-r--r--   0 me        (1000) me        (1000)     7796 2023-06-16 19:15:33.000000 pandasklar-0.3.6/src/pandasklar/values_info.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-07-09 19:56:08.550866 pandasklar-0.3.6/src/pandasklar.egg-info/
+-rw-r--r--   0 me        (1000) me        (1000)     9874 2023-07-09 19:56:08.000000 pandasklar-0.3.6/src/pandasklar.egg-info/PKG-INFO
+-rw-r--r--   0 me        (1000) me        (1000)      677 2023-07-09 19:56:08.000000 pandasklar-0.3.6/src/pandasklar.egg-info/SOURCES.txt
+-rw-r--r--   0 me        (1000) me        (1000)        1 2023-07-09 19:56:08.000000 pandasklar-0.3.6/src/pandasklar.egg-info/dependency_links.txt
+-rw-r--r--   0 me        (1000) me        (1000)       56 2023-07-09 19:56:08.000000 pandasklar-0.3.6/src/pandasklar.egg-info/entry_points.txt
+-rw-r--r--   0 me        (1000) me        (1000)       47 2023-07-09 19:56:08.000000 pandasklar-0.3.6/src/pandasklar.egg-info/requires.txt
+-rw-r--r--   0 me        (1000) me        (1000)       11 2023-07-09 19:56:08.000000 pandasklar-0.3.6/src/pandasklar.egg-info/top_level.txt
```

### Comparing `pandasklar-0.3.5/LICENSE` & `pandasklar-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.5/PKG-INFO` & `pandasklar-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasklar
-Version: 0.3.5
+Version: 0.3.6
 Summary: Toolbox / Ecosystem for data science. Easier handling of pandas, especially when thinking in SQL.
 Author-email: djekra <hopsalla@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/djekra/pandasklar
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -124,14 +124,15 @@
    compare_median, rank and random.
 
 
 ## Cleanup Strings
 * `remove_str`: Removes a list of unwanted substrings from a Series of strings.
 * `remove_words`: Removes a list of unwanted words from a Series of strings.
 * `replace_str`: Replaces substrings from a Series of strings according to a dict.
+* `preprocess_str`: Multiple methods for simplification and cleaning
 
 
 ## Slice Strings Variably
 * `slice_string`: Slices a column of strings based on indexes in another columns.
 
 
 ## Search Strings Fast
```

### Comparing `pandasklar-0.3.5/README.md` & `pandasklar-0.3.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -110,14 +110,15 @@
    compare_median, rank and random.
 
 
 ## Cleanup Strings
 * `remove_str`: Removes a list of unwanted substrings from a Series of strings.
 * `remove_words`: Removes a list of unwanted words from a Series of strings.
 * `replace_str`: Replaces substrings from a Series of strings according to a dict.
+* `preprocess_str`: Multiple methods for simplification and cleaning
 
 
 ## Slice Strings Variably
 * `slice_string`: Slices a column of strings based on indexes in another columns.
 
 
 ## Search Strings Fast
```

### Comparing `pandasklar-0.3.5/pyproject.toml` & `pandasklar-0.3.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # pyproject.toml
 
 
 [project]
 name            = "pandasklar"
-version         = "0.3.5"    
+version         = "0.3.6"    
 
 requires-python = ">=3.8"
 dependencies    = ['pandas','numpy','perlin_noise','termcolor','bpyth','blab',]
 
 authors        = [{ name = "djekra", email = "hopsalla@gmail.com" }]
 description     = "Toolbox / Ecosystem for data science. Easier handling of pandas, especially when thinking in SQL."
 readme          = "README.md"
```

### Comparing `pandasklar-0.3.5/src/pandasklar/__init__.py` & `pandasklar-0.3.6/src/pandasklar/__init__.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.5/src/pandasklar/aggregate.py` & `pandasklar-0.3.6/src/pandasklar/aggregate.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.5/src/pandasklar/analyse.py` & `pandasklar-0.3.6/src/pandasklar/analyse.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.5/src/pandasklar/compare.py` & `pandasklar-0.3.6/src/pandasklar/compare.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,16 +78,19 @@
             try:
                 if list(s).sort() == list(t).sort():
                     result['content'] = True    
             except:
                 result['content'] = None               
 
             # sort
-            if list(s) == list(t):
-                result['sort'] = True    
+            try:
+                if list(s) == list(t):
+                    result['sort'] = True 
+            except:
+                result['sort'] = None  
 
             # eq
             if s.eq(t).all(skipna=False): 
                 result['eq']      = True
                 result['content'] = True    # falls es None war  
         
     # return result
```

### Comparing `pandasklar-0.3.5/src/pandasklar/config.py` & `pandasklar-0.3.6/src/pandasklar/config.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.5/src/pandasklar/content.py` & `pandasklar-0.3.6/src/pandasklar/content.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.5/src/pandasklar/develop.py` & `pandasklar-0.3.6/src/pandasklar/develop.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.5/src/pandasklar/pandas.py` & `pandasklar-0.3.6/src/pandasklar/pandas.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.5/src/pandasklar/plot.py` & `pandasklar-0.3.6/src/pandasklar/plot.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.5/src/pandasklar/rank.py` & `pandasklar-0.3.6/src/pandasklar/rank.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.5/src/pandasklar/scale.py` & `pandasklar-0.3.6/src/pandasklar/scale.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.5/src/pandasklar/subsets.py` & `pandasklar-0.3.6/src/pandasklar/subsets.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.5/src/pandasklar/type_info.py` & `pandasklar-0.3.6/src/pandasklar/type_info.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.5/src/pandasklar/values_info.py` & `pandasklar-0.3.6/src/pandasklar/values_info.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.5/src/pandasklar.egg-info/PKG-INFO` & `pandasklar-0.3.6/src/pandasklar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasklar
-Version: 0.3.5
+Version: 0.3.6
 Summary: Toolbox / Ecosystem for data science. Easier handling of pandas, especially when thinking in SQL.
 Author-email: djekra <hopsalla@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/djekra/pandasklar
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -124,14 +124,15 @@
    compare_median, rank and random.
 
 
 ## Cleanup Strings
 * `remove_str`: Removes a list of unwanted substrings from a Series of strings.
 * `remove_words`: Removes a list of unwanted words from a Series of strings.
 * `replace_str`: Replaces substrings from a Series of strings according to a dict.
+* `preprocess_str`: Multiple methods for simplification and cleaning
 
 
 ## Slice Strings Variably
 * `slice_string`: Slices a column of strings based on indexes in another columns.
 
 
 ## Search Strings Fast
```

### Comparing `pandasklar-0.3.5/src/pandasklar.egg-info/SOURCES.txt` & `pandasklar-0.3.6/src/pandasklar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

