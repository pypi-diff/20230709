# Comparing `tmp/pytrials-0.2.1.tar.gz` & `tmp/pytrials-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytrials-0.2.1.tar", last modified: Sun Jul  9 17:42:40 2023, max compression
+gzip compressed data, was "pytrials-0.3.0.tar", last modified: Sun Jul  9 18:09:49 2023, max compression
```

## Comparing `pytrials-0.2.1.tar` & `pytrials-0.3.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2023-07-09 17:42:40.420018 pytrials-0.2.1/
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)      174 2023-07-09 17:21:39.000000 pytrials-0.2.1/AUTHORS.rst
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)     3275 2023-07-09 17:21:39.000000 pytrials-0.2.1/CONTRIBUTING.rst
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)      356 2023-07-09 17:37:49.000000 pytrials-0.2.1/HISTORY.rst
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)     1519 2023-07-09 17:21:39.000000 pytrials-0.2.1/LICENSE
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)      262 2023-07-09 17:21:39.000000 pytrials-0.2.1/MANIFEST.in
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)     3224 2023-07-09 17:42:40.420018 pytrials-0.2.1/PKG-INFO
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)     2088 2023-07-09 17:21:39.000000 pytrials-0.2.1/README.rst
-drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2023-07-09 17:42:40.420018 pytrials-0.2.1/docs/
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)      609 2023-07-09 17:21:39.000000 pytrials-0.2.1/docs/Makefile
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)       28 2023-07-09 17:21:39.000000 pytrials-0.2.1/docs/authors.rst
--rwxr-xr-x   0 jvfe      (1000) jvfe      (1000)     4911 2023-07-09 17:21:39.000000 pytrials-0.2.1/docs/conf.py
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)       33 2023-07-09 17:21:39.000000 pytrials-0.2.1/docs/contributing.rst
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)       28 2023-07-09 17:21:39.000000 pytrials-0.2.1/docs/history.rst
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)      305 2023-07-09 17:21:39.000000 pytrials-0.2.1/docs/index.rst
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)     1106 2023-07-09 17:21:39.000000 pytrials-0.2.1/docs/installation.rst
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)      770 2023-07-09 17:21:39.000000 pytrials-0.2.1/docs/make.bat
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)       61 2023-07-09 17:21:39.000000 pytrials-0.2.1/docs/modules.rst
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)      445 2023-07-09 17:21:39.000000 pytrials-0.2.1/docs/pytrials.rst
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)       27 2023-07-09 17:21:39.000000 pytrials-0.2.1/docs/readme.rst
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)       71 2023-07-09 17:21:39.000000 pytrials-0.2.1/docs/usage.rst
-drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2023-07-09 17:42:40.420018 pytrials-0.2.1/pytrials/
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)      137 2023-07-09 17:42:11.000000 pytrials-0.2.1/pytrials/__init__.py
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)     5825 2023-07-09 17:31:27.000000 pytrials-0.2.1/pytrials/client.py
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)      963 2023-07-09 17:36:25.000000 pytrials-0.2.1/pytrials/utils.py
-drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2023-07-09 17:42:40.420018 pytrials-0.2.1/pytrials.egg-info/
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)     3224 2023-07-09 17:42:40.000000 pytrials-0.2.1/pytrials.egg-info/PKG-INFO
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)      597 2023-07-09 17:42:40.000000 pytrials-0.2.1/pytrials.egg-info/SOURCES.txt
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)        1 2023-07-09 17:42:40.000000 pytrials-0.2.1/pytrials.egg-info/dependency_links.txt
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)        1 2023-07-09 17:42:40.000000 pytrials-0.2.1/pytrials.egg-info/not-zip-safe
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)        9 2023-07-09 17:42:40.000000 pytrials-0.2.1/pytrials.egg-info/requires.txt
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)        9 2023-07-09 17:42:40.000000 pytrials-0.2.1/pytrials.egg-info/top_level.txt
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)      542 2023-07-09 17:42:40.420018 pytrials-0.2.1/setup.cfg
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)     1467 2023-07-09 17:42:11.000000 pytrials-0.2.1/setup.py
-drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2023-07-09 17:42:40.420018 pytrials-0.2.1/tests/
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)       38 2023-07-09 17:21:39.000000 pytrials-0.2.1/tests/__init__.py
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)     2941 2023-07-09 17:21:39.000000 pytrials-0.2.1/tests/test_client.py
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)      151 2023-07-09 17:21:39.000000 pytrials-0.2.1/tests/test_utils.py
+drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2023-07-09 18:09:49.270042 pytrials-0.3.0/
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      235 2023-07-09 18:08:52.000000 pytrials-0.3.0/AUTHORS.rst
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)     3275 2023-07-09 17:21:39.000000 pytrials-0.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      443 2023-07-09 18:08:10.000000 pytrials-0.3.0/HISTORY.rst
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)     1519 2023-07-09 17:21:39.000000 pytrials-0.3.0/LICENSE
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      262 2023-07-09 17:21:39.000000 pytrials-0.3.0/MANIFEST.in
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)     3311 2023-07-09 18:09:49.270042 pytrials-0.3.0/PKG-INFO
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)     2088 2023-07-09 17:21:39.000000 pytrials-0.3.0/README.rst
+drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2023-07-09 18:09:49.270042 pytrials-0.3.0/docs/
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      609 2023-07-09 17:21:39.000000 pytrials-0.3.0/docs/Makefile
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)       28 2023-07-09 17:21:39.000000 pytrials-0.3.0/docs/authors.rst
+-rwxr-xr-x   0 jvfe      (1000) jvfe      (1000)     4911 2023-07-09 17:21:39.000000 pytrials-0.3.0/docs/conf.py
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)       33 2023-07-09 17:21:39.000000 pytrials-0.3.0/docs/contributing.rst
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)       28 2023-07-09 17:21:39.000000 pytrials-0.3.0/docs/history.rst
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      305 2023-07-09 17:21:39.000000 pytrials-0.3.0/docs/index.rst
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)     1106 2023-07-09 17:21:39.000000 pytrials-0.3.0/docs/installation.rst
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      770 2023-07-09 17:21:39.000000 pytrials-0.3.0/docs/make.bat
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)       61 2023-07-09 17:21:39.000000 pytrials-0.3.0/docs/modules.rst
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      445 2023-07-09 17:21:39.000000 pytrials-0.3.0/docs/pytrials.rst
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)       27 2023-07-09 17:21:39.000000 pytrials-0.3.0/docs/readme.rst
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)       71 2023-07-09 17:21:39.000000 pytrials-0.3.0/docs/usage.rst
+drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2023-07-09 18:09:49.270042 pytrials-0.3.0/pytrials/
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      137 2023-07-09 18:09:34.000000 pytrials-0.3.0/pytrials/__init__.py
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)     6029 2023-07-09 18:07:29.000000 pytrials-0.3.0/pytrials/client.py
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      963 2023-07-09 17:58:10.000000 pytrials-0.3.0/pytrials/utils.py
+drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2023-07-09 18:09:49.270042 pytrials-0.3.0/pytrials.egg-info/
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)     3311 2023-07-09 18:09:49.000000 pytrials-0.3.0/pytrials.egg-info/PKG-INFO
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      597 2023-07-09 18:09:49.000000 pytrials-0.3.0/pytrials.egg-info/SOURCES.txt
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)        1 2023-07-09 18:09:49.000000 pytrials-0.3.0/pytrials.egg-info/dependency_links.txt
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)        1 2023-07-09 18:09:49.000000 pytrials-0.3.0/pytrials.egg-info/not-zip-safe
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)        9 2023-07-09 18:09:49.000000 pytrials-0.3.0/pytrials.egg-info/requires.txt
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)        9 2023-07-09 18:09:49.000000 pytrials-0.3.0/pytrials.egg-info/top_level.txt
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      542 2023-07-09 18:09:49.270042 pytrials-0.3.0/setup.cfg
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)     1467 2023-07-09 18:09:34.000000 pytrials-0.3.0/setup.py
+drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2023-07-09 18:09:49.270042 pytrials-0.3.0/tests/
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)       38 2023-07-09 17:21:39.000000 pytrials-0.3.0/tests/__init__.py
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)     2941 2023-07-09 17:21:39.000000 pytrials-0.3.0/tests/test_client.py
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      151 2023-07-09 17:21:39.000000 pytrials-0.3.0/tests/test_utils.py
```

### Comparing `pytrials-0.2.1/CONTRIBUTING.rst` & `pytrials-0.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pytrials-0.2.1/LICENSE` & `pytrials-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytrials-0.2.1/PKG-INFO` & `pytrials-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrials
-Version: 0.2.1
+Version: 0.3.0
 Summary: Python wrapper around the clinicaltrials.gov API
 Home-page: https://github.com/jvfe/pytrials
 Author: João Vitor F. Cavalcante
 Author-email: jvfe@ufrn.edu.br
 License: BSD license
 Keywords: pytrials clinical-trials clinical trials tabular text-mining text opendata
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -114,7 +114,12 @@
 * Added get_study_count function
 
 0.2.1 (2023-07-09)
 ------------------
 
 * Add classic prefix to url - #10
 * Raise error if API status is not ok - #11
+
+0.3.0 (2023-07-09)
+------------------
+
+* Add min_rnk option to get_study_fields - #12
```

### Comparing `pytrials-0.2.1/README.rst` & `pytrials-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `pytrials-0.2.1/docs/Makefile` & `pytrials-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pytrials-0.2.1/docs/conf.py` & `pytrials-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytrials-0.2.1/docs/installation.rst` & `pytrials-0.3.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pytrials-0.2.1/docs/make.bat` & `pytrials-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pytrials-0.2.1/pytrials/client.py` & `pytrials-0.3.0/pytrials/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pytrials.utils import json_handler, csv_handler
 
 
 class ClinicalTrials:
     """ClinicalTrials API client
 
     Provides functions to easily access the ClinicalTrials.gov API
-    (https://clinicaltrials.gov/api/)
+    (https://classic.clinicaltrials.gov/api/)
     in Python.
 
     Attributes:
         study_fields: List of all study fields you can use in your query.
         api_info: Tuple containing the API version number and the last
         time the database was updated.
     """
@@ -65,27 +65,29 @@
 
         req = f"full_studies?expr={search_expr}&max_rnk={max_studies}&{self._JSON}"
 
         full_studies = json_handler(f"{self._BASE_URL}{self._QUERY}{req}")
 
         return full_studies
 
-    def get_study_fields(self, search_expr, fields, max_studies=50, fmt="csv"):
+    def get_study_fields(self, search_expr, fields, max_studies=50, min_rnk=1, fmt="csv"):
         """Returns study content for specified fields
 
         Retrieves information from the study fields endpoint, which acquires specified information
         from a large (max 1000) studies. To see a list of all possible fields, check the class'
         study_fields attribute.
 
         Args:
             search_expr (str): A string containing a search expression as specified by
                 `their documentation <https://clinicaltrials.gov/api/gui/ref/syntax#searchExpr>`_.
             fields (list(str)): A list containing the desired information fields.
             max_studies (int): An integer indicating the maximum number of studies to return.
                 Defaults to 50.
+            min_rnk (int): Minimum Rank sets the lower limit on the range of study records used to return results.
+                If absent, defaults to 1.
             fmt (str): A string indicating the output format, csv or json. Defaults to csv.
 
         Returns:
             Either a dict, if fmt='json', or a list of records (e.g. a list of lists), if fmt='csv.
             Both containing the maximum number of study fields queried using the specified search expression.
 
         Raises:
@@ -98,15 +100,15 @@
             raise ValueError("The number of studies can only be between 1 and 1000")
         elif not set(fields).issubset(self.study_fields):
             raise ValueError(
                 "One of the fields is not valid! Check the study_fields attribute for a list of valid ones."
             )
         else:
             concat_fields = ",".join(fields)
-            req = f"study_fields?expr={search_expr}&max_rnk={max_studies}&fields={concat_fields}"
+            req = f"study_fields?expr={search_expr}&min_rnk={min_rnk}&max_rnk={max_studies+min_rnk-1}&fields={concat_fields}"
             if fmt == "csv":
                 url = f"{self._BASE_URL}{self._QUERY}{req}&{self._CSV}"
                 return csv_handler(url)
 
             elif fmt == "json":
                 url = f"{self._BASE_URL}{self._QUERY}{req}&{self._JSON}"
                 return json_handler(url)
```

### Comparing `pytrials-0.2.1/pytrials/utils.py` & `pytrials-0.3.0/pytrials/utils.py`

 * *Files identical despite different names*

### Comparing `pytrials-0.2.1/pytrials.egg-info/PKG-INFO` & `pytrials-0.3.0/pytrials.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrials
-Version: 0.2.1
+Version: 0.3.0
 Summary: Python wrapper around the clinicaltrials.gov API
 Home-page: https://github.com/jvfe/pytrials
 Author: João Vitor F. Cavalcante
 Author-email: jvfe@ufrn.edu.br
 License: BSD license
 Keywords: pytrials clinical-trials clinical trials tabular text-mining text opendata
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -114,7 +114,12 @@
 * Added get_study_count function
 
 0.2.1 (2023-07-09)
 ------------------
 
 * Add classic prefix to url - #10
 * Raise error if API status is not ok - #11
+
+0.3.0 (2023-07-09)
+------------------
+
+* Add min_rnk option to get_study_fields - #12
```

### Comparing `pytrials-0.2.1/pytrials.egg-info/SOURCES.txt` & `pytrials-0.3.0/pytrials.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytrials-0.2.1/setup.cfg` & `pytrials-0.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.1
+current_version = 0.3.0
 commit = True
 tag = True
 
 [bumpversion:file:pytrials/__init__.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
```

### Comparing `pytrials-0.2.1/setup.py` & `pytrials-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,10 +44,10 @@
     keywords="pytrials clinical-trials clinical trials tabular text-mining text opendata",
     name="pytrials",
     packages=find_packages(include=["pytrials", "pytrials.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/jvfe/pytrials",
-    version="0.2.1",
+    version="0.3.0",
     zip_safe=False,
 )
```

### Comparing `pytrials-0.2.1/tests/test_client.py` & `pytrials-0.3.0/tests/test_client.py`

 * *Files identical despite different names*

