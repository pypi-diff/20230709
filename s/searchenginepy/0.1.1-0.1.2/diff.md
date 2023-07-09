# Comparing `tmp/searchenginepy-0.1.1.tar.gz` & `tmp/searchenginepy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchenginepy-0.1.1.tar", last modified: Sun Jul  9 19:01:53 2023, max compression
+gzip compressed data, was "searchenginepy-0.1.2.tar", last modified: Sun Jul  9 19:08:36 2023, max compression
```

## Comparing `searchenginepy-0.1.1.tar` & `searchenginepy-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 19:01:53.266897 searchenginepy-0.1.1/
--rw-rw-rw-   0        0        0     1069 2023-07-09 15:32:43.000000 searchenginepy-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      791 2023-07-09 19:01:53.266897 searchenginepy-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      528 2023-07-09 18:56:35.000000 searchenginepy-0.1.1/README.md
--rw-rw-rw-   0        0        0      111 2023-07-09 19:01:53.266897 searchenginepy-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1699 2023-07-09 18:59:06.000000 searchenginepy-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-09 19:01:53.227026 searchenginepy-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-09 19:01:53.241817 searchenginepy-0.1.1/src/searchenginepy/
-drwxrwxrwx   0        0        0        0 2023-07-09 19:01:53.264322 searchenginepy-0.1.1/src/searchenginepy/Brave/
--rw-rw-rw-   0        0        0        0 2023-07-09 16:19:13.000000 searchenginepy-0.1.1/src/searchenginepy/Brave/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 19:01:53.264322 searchenginepy-0.1.1/src/searchenginepy/DuckDuckGo/
--rw-rw-rw-   0        0        0        0 2023-07-09 16:19:24.000000 searchenginepy-0.1.1/src/searchenginepy/DuckDuckGo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 19:01:53.266897 searchenginepy-0.1.1/src/searchenginepy/Google/
--rw-rw-rw-   0        0        0     1017 2023-07-09 18:48:11.000000 searchenginepy-0.1.1/src/searchenginepy/Google/__init__.py
--rw-rw-rw-   0        0        0      583 2023-07-09 18:19:37.000000 searchenginepy-0.1.1/src/searchenginepy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 19:01:53.261820 searchenginepy-0.1.1/src/searchenginepy.egg-info/
--rw-rw-rw-   0        0        0      791 2023-07-09 19:01:52.000000 searchenginepy-0.1.1/src/searchenginepy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2023-07-09 19:01:52.000000 searchenginepy-0.1.1/src/searchenginepy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 19:01:52.000000 searchenginepy-0.1.1/src/searchenginepy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-09 19:01:52.000000 searchenginepy-0.1.1/src/searchenginepy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-09 19:01:52.000000 searchenginepy-0.1.1/src/searchenginepy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-09 19:08:36.139877 searchenginepy-0.1.2/
+-rw-rw-rw-   0        0        0     1069 2023-07-09 15:32:43.000000 searchenginepy-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      791 2023-07-09 19:08:36.139877 searchenginepy-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      528 2023-07-09 18:56:35.000000 searchenginepy-0.1.2/README.md
+-rw-rw-rw-   0        0        0      111 2023-07-09 19:08:36.139877 searchenginepy-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1836 2023-07-09 19:08:24.000000 searchenginepy-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 19:08:36.089365 searchenginepy-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-09 19:08:36.114104 searchenginepy-0.1.2/src/searchenginepy/
+drwxrwxrwx   0        0        0        0 2023-07-09 19:08:36.138322 searchenginepy-0.1.2/src/searchenginepy/Brave/
+-rw-rw-rw-   0        0        0        0 2023-07-09 16:19:13.000000 searchenginepy-0.1.2/src/searchenginepy/Brave/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 19:08:36.139877 searchenginepy-0.1.2/src/searchenginepy/DuckDuckGo/
+-rw-rw-rw-   0        0        0        0 2023-07-09 16:19:24.000000 searchenginepy-0.1.2/src/searchenginepy/DuckDuckGo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 19:08:36.139877 searchenginepy-0.1.2/src/searchenginepy/Google/
+-rw-rw-rw-   0        0        0     1017 2023-07-09 18:48:11.000000 searchenginepy-0.1.2/src/searchenginepy/Google/__init__.py
+-rw-rw-rw-   0        0        0      583 2023-07-09 18:19:37.000000 searchenginepy-0.1.2/src/searchenginepy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 19:08:36.136046 searchenginepy-0.1.2/src/searchenginepy.egg-info/
+-rw-rw-rw-   0        0        0      791 2023-07-09 19:08:35.000000 searchenginepy-0.1.2/src/searchenginepy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2023-07-09 19:08:35.000000 searchenginepy-0.1.2/src/searchenginepy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 19:08:35.000000 searchenginepy-0.1.2/src/searchenginepy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-09 19:08:35.000000 searchenginepy-0.1.2/src/searchenginepy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-09 19:08:35.000000 searchenginepy-0.1.2/src/searchenginepy.egg-info/top_level.txt
```

### Comparing `searchenginepy-0.1.1/LICENSE` & `searchenginepy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `searchenginepy-0.1.1/PKG-INFO` & `searchenginepy-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchenginepy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Query popular search engines and get results easily
 Home-page: https://github.com/codewithnick/searchengine
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: codewithnick
 Author-email: nikhilsingh52645@gmail.com
 License: MIT
 Keywords: google,search engine,crawler
```

### Comparing `searchenginepy-0.1.1/README.md` & `searchenginepy-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `searchenginepy-0.1.1/setup.py` & `searchenginepy-0.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 from distutils.core import setup
+
+# read the contents of your README file
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
+
 setup(
   name = 'searchenginepy',         # How you named your package folder (MyLib)
-  version = '0.1.1',      # Start with a small number and increase it with every change you make
+  version = '0.1.2',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Query popular search engines and get results easily',   # Give a short description about your library
-  description_file = ['README.md'],
   author = 'codewithnick',                   # Type in your name
   author_email = 'nikhilsingh52645@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/codewithnick/searchengine',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',    # I explain this later on
   keywords = ['google', 'search engine', 'crawler'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'requests',
```

### Comparing `searchenginepy-0.1.1/src/searchenginepy/Google/__init__.py` & `searchenginepy-0.1.2/src/searchenginepy/Google/__init__.py`

 * *Files identical despite different names*

### Comparing `searchenginepy-0.1.1/src/searchenginepy/__init__.py` & `searchenginepy-0.1.2/src/searchenginepy/__init__.py`

 * *Files identical despite different names*

### Comparing `searchenginepy-0.1.1/src/searchenginepy.egg-info/PKG-INFO` & `searchenginepy-0.1.2/src/searchenginepy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchenginepy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Query popular search engines and get results easily
 Home-page: https://github.com/codewithnick/searchengine
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: codewithnick
 Author-email: nikhilsingh52645@gmail.com
 License: MIT
 Keywords: google,search engine,crawler
```

