# Comparing `tmp/pytrials-0.2.0.tar.gz` & `tmp/pytrials-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytrials-0.2.0.tar", last modified: Fri Apr 30 14:35:19 2021, max compression
+gzip compressed data, was "pytrials-0.2.1.tar", last modified: Sun Jul  9 17:42:40 2023, max compression
```

## Comparing `pytrials-0.2.0.tar` & `pytrials-0.2.1.tar`

### file list

```diff
@@ -1,52 +1,38 @@
-drwxrwxr-x   0 jvfe      (1000) jvfe      (1000)        0 2021-04-30 14:35:19.296280 pytrials-0.2.0/
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)      174 2021-04-30 14:27:18.000000 pytrials-0.2.0/AUTHORS.rst
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)     3275 2021-04-30 14:27:18.000000 pytrials-0.2.0/CONTRIBUTING.rst
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)      238 2021-04-30 14:30:47.000000 pytrials-0.2.0/HISTORY.rst
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)     1519 2020-07-08 18:07:19.000000 pytrials-0.2.0/LICENSE
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)      262 2020-07-08 18:07:19.000000 pytrials-0.2.0/MANIFEST.in
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)     3833 2021-04-30 14:35:19.296280 pytrials-0.2.0/PKG-INFO
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)     2088 2021-04-30 14:27:18.000000 pytrials-0.2.0/README.rst
-drwxrwxr-x   0 jvfe      (1000) jvfe      (1000)        0 2021-04-30 14:35:19.292280 pytrials-0.2.0/docs/
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)      609 2020-07-08 18:07:19.000000 pytrials-0.2.0/docs/Makefile
-drwxrwxr-x   0 jvfe      (1000) jvfe      (1000)        0 2021-04-30 14:35:19.292280 pytrials-0.2.0/docs/_build/
-drwxrwxr-x   0 jvfe      (1000) jvfe      (1000)        0 2021-04-30 14:35:19.292280 pytrials-0.2.0/docs/_build/html/
-drwxrwxr-x   0 jvfe      (1000) jvfe      (1000)        0 2021-04-30 14:35:19.296280 pytrials-0.2.0/docs/_build/html/_static/
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)      673 2021-04-29 10:21:12.000000 pytrials-0.2.0/docs/_build/html/_static/ajax-loader.gif
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)      756 2021-04-29 10:21:12.000000 pytrials-0.2.0/docs/_build/html/_static/comment-bright.png
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)      829 2021-04-29 10:21:12.000000 pytrials-0.2.0/docs/_build/html/_static/comment-close.png
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)      641 2021-04-29 10:21:12.000000 pytrials-0.2.0/docs/_build/html/_static/comment.png
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)      222 2021-04-29 10:21:12.000000 pytrials-0.2.0/docs/_build/html/_static/down-pressed.png
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)      202 2021-04-29 10:21:12.000000 pytrials-0.2.0/docs/_build/html/_static/down.png
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)      286 2021-04-29 10:21:12.000000 pytrials-0.2.0/docs/_build/html/_static/file.png
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)       90 2021-04-29 10:21:12.000000 pytrials-0.2.0/docs/_build/html/_static/minus.png
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)       90 2021-04-29 10:21:12.000000 pytrials-0.2.0/docs/_build/html/_static/plus.png
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)      214 2021-04-29 10:21:12.000000 pytrials-0.2.0/docs/_build/html/_static/up-pressed.png
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)      203 2021-04-29 10:21:12.000000 pytrials-0.2.0/docs/_build/html/_static/up.png
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)       28 2020-07-08 18:07:19.000000 pytrials-0.2.0/docs/authors.rst
--rwxrwxr-x   0 jvfe      (1000) jvfe      (1000)     4911 2020-07-08 18:07:19.000000 pytrials-0.2.0/docs/conf.py
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)       33 2020-07-08 18:07:19.000000 pytrials-0.2.0/docs/contributing.rst
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)       28 2020-07-08 18:07:19.000000 pytrials-0.2.0/docs/history.rst
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)      305 2020-07-08 18:07:19.000000 pytrials-0.2.0/docs/index.rst
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)     1106 2020-07-08 18:07:19.000000 pytrials-0.2.0/docs/installation.rst
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)      770 2020-07-08 18:07:19.000000 pytrials-0.2.0/docs/make.bat
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)       61 2021-04-29 11:40:27.000000 pytrials-0.2.0/docs/modules.rst
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)      445 2021-04-29 11:40:27.000000 pytrials-0.2.0/docs/pytrials.rst
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)       27 2020-07-08 18:07:19.000000 pytrials-0.2.0/docs/readme.rst
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)       71 2020-07-08 18:07:19.000000 pytrials-0.2.0/docs/usage.rst
-drwxrwxr-x   0 jvfe      (1000) jvfe      (1000)        0 2021-04-30 14:35:19.296280 pytrials-0.2.0/pytrials/
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)      137 2021-04-30 14:32:24.000000 pytrials-0.2.0/pytrials/__init__.py
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)     5817 2021-04-30 14:27:18.000000 pytrials-0.2.0/pytrials/client.py
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)      873 2021-04-30 14:27:18.000000 pytrials-0.2.0/pytrials/utils.py
-drwxrwxr-x   0 jvfe      (1000) jvfe      (1000)        0 2021-04-30 14:35:19.296280 pytrials-0.2.0/pytrials.egg-info/
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)     3833 2021-04-30 14:35:18.000000 pytrials-0.2.0/pytrials.egg-info/PKG-INFO
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)     1013 2021-04-30 14:35:19.000000 pytrials-0.2.0/pytrials.egg-info/SOURCES.txt
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)        1 2021-04-30 14:35:18.000000 pytrials-0.2.0/pytrials.egg-info/dependency_links.txt
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)        1 2021-04-30 14:35:18.000000 pytrials-0.2.0/pytrials.egg-info/not-zip-safe
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)        9 2021-04-30 14:35:18.000000 pytrials-0.2.0/pytrials.egg-info/requires.txt
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)        9 2021-04-30 14:35:18.000000 pytrials-0.2.0/pytrials.egg-info/top_level.txt
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)      425 2021-04-30 14:35:19.296280 pytrials-0.2.0/setup.cfg
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)     1467 2021-04-30 14:31:51.000000 pytrials-0.2.0/setup.py
-drwxrwxr-x   0 jvfe      (1000) jvfe      (1000)        0 2021-04-30 14:35:19.296280 pytrials-0.2.0/tests/
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)       38 2020-07-08 18:07:19.000000 pytrials-0.2.0/tests/__init__.py
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)     2941 2021-04-30 14:27:19.000000 pytrials-0.2.0/tests/test_client.py
--rw-rw-r--   0 jvfe      (1000) jvfe      (1000)      151 2021-04-30 14:27:19.000000 pytrials-0.2.0/tests/test_utils.py
+drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2023-07-09 17:42:40.420018 pytrials-0.2.1/
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      174 2023-07-09 17:21:39.000000 pytrials-0.2.1/AUTHORS.rst
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)     3275 2023-07-09 17:21:39.000000 pytrials-0.2.1/CONTRIBUTING.rst
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      356 2023-07-09 17:37:49.000000 pytrials-0.2.1/HISTORY.rst
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)     1519 2023-07-09 17:21:39.000000 pytrials-0.2.1/LICENSE
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      262 2023-07-09 17:21:39.000000 pytrials-0.2.1/MANIFEST.in
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)     3224 2023-07-09 17:42:40.420018 pytrials-0.2.1/PKG-INFO
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)     2088 2023-07-09 17:21:39.000000 pytrials-0.2.1/README.rst
+drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2023-07-09 17:42:40.420018 pytrials-0.2.1/docs/
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      609 2023-07-09 17:21:39.000000 pytrials-0.2.1/docs/Makefile
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)       28 2023-07-09 17:21:39.000000 pytrials-0.2.1/docs/authors.rst
+-rwxr-xr-x   0 jvfe      (1000) jvfe      (1000)     4911 2023-07-09 17:21:39.000000 pytrials-0.2.1/docs/conf.py
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)       33 2023-07-09 17:21:39.000000 pytrials-0.2.1/docs/contributing.rst
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)       28 2023-07-09 17:21:39.000000 pytrials-0.2.1/docs/history.rst
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      305 2023-07-09 17:21:39.000000 pytrials-0.2.1/docs/index.rst
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)     1106 2023-07-09 17:21:39.000000 pytrials-0.2.1/docs/installation.rst
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      770 2023-07-09 17:21:39.000000 pytrials-0.2.1/docs/make.bat
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)       61 2023-07-09 17:21:39.000000 pytrials-0.2.1/docs/modules.rst
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      445 2023-07-09 17:21:39.000000 pytrials-0.2.1/docs/pytrials.rst
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)       27 2023-07-09 17:21:39.000000 pytrials-0.2.1/docs/readme.rst
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)       71 2023-07-09 17:21:39.000000 pytrials-0.2.1/docs/usage.rst
+drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2023-07-09 17:42:40.420018 pytrials-0.2.1/pytrials/
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      137 2023-07-09 17:42:11.000000 pytrials-0.2.1/pytrials/__init__.py
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)     5825 2023-07-09 17:31:27.000000 pytrials-0.2.1/pytrials/client.py
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      963 2023-07-09 17:36:25.000000 pytrials-0.2.1/pytrials/utils.py
+drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2023-07-09 17:42:40.420018 pytrials-0.2.1/pytrials.egg-info/
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)     3224 2023-07-09 17:42:40.000000 pytrials-0.2.1/pytrials.egg-info/PKG-INFO
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      597 2023-07-09 17:42:40.000000 pytrials-0.2.1/pytrials.egg-info/SOURCES.txt
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)        1 2023-07-09 17:42:40.000000 pytrials-0.2.1/pytrials.egg-info/dependency_links.txt
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)        1 2023-07-09 17:42:40.000000 pytrials-0.2.1/pytrials.egg-info/not-zip-safe
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)        9 2023-07-09 17:42:40.000000 pytrials-0.2.1/pytrials.egg-info/requires.txt
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)        9 2023-07-09 17:42:40.000000 pytrials-0.2.1/pytrials.egg-info/top_level.txt
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      542 2023-07-09 17:42:40.420018 pytrials-0.2.1/setup.cfg
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)     1467 2023-07-09 17:42:11.000000 pytrials-0.2.1/setup.py
+drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2023-07-09 17:42:40.420018 pytrials-0.2.1/tests/
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)       38 2023-07-09 17:21:39.000000 pytrials-0.2.1/tests/__init__.py
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)     2941 2023-07-09 17:21:39.000000 pytrials-0.2.1/tests/test_client.py
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      151 2023-07-09 17:21:39.000000 pytrials-0.2.1/tests/test_utils.py
```

### Comparing `pytrials-0.2.0/CONTRIBUTING.rst` & `pytrials-0.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pytrials-0.2.0/LICENSE` & `pytrials-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytrials-0.2.0/README.rst` & `pytrials-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `pytrials-0.2.0/docs/Makefile` & `pytrials-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pytrials-0.2.0/docs/conf.py` & `pytrials-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytrials-0.2.0/docs/installation.rst` & `pytrials-0.2.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pytrials-0.2.0/docs/make.bat` & `pytrials-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pytrials-0.2.0/pytrials/client.py` & `pytrials-0.2.1/pytrials/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     Attributes:
         study_fields: List of all study fields you can use in your query.
         api_info: Tuple containing the API version number and the last
         time the database was updated.
     """
 
-    _BASE_URL = "https://clinicaltrials.gov/api/"
+    _BASE_URL = "https://classic.clinicaltrials.gov/api/"
     _INFO = "info/"
     _QUERY = "query/"
     _JSON = "fmt=json"
     _CSV = "fmt=csv"
 
     def __init__(self):
         self.api_info = self.__api_info()
```

### Comparing `pytrials-0.2.0/pytrials/utils.py` & `pytrials-0.2.1/pytrials/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 import re
 
 
 def request_ct(url):
     """Performs a get request that provides a (somewhat) useful error message."""
     try:
         response = requests.get(url)
+        response.raise_for_status()
+    except requests.HTTPError as ex:
+        raise ex
     except ImportError:
         raise ImportError(
             "Couldn't retrieve the data, check your search expression or try again later."
         )
     else:
         return response
```

### Comparing `pytrials-0.2.0/setup.py` & `pytrials-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,10 +44,10 @@
     keywords="pytrials clinical-trials clinical trials tabular text-mining text opendata",
     name="pytrials",
     packages=find_packages(include=["pytrials", "pytrials.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/jvfe/pytrials",
-    version="0.2.0",
+    version="0.2.1",
     zip_safe=False,
 )
```

### Comparing `pytrials-0.2.0/tests/test_client.py` & `pytrials-0.2.1/tests/test_client.py`

 * *Files identical despite different names*

