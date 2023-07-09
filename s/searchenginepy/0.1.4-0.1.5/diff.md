# Comparing `tmp/searchenginepy-0.1.4.tar.gz` & `tmp/searchenginepy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchenginepy-0.1.4.tar", last modified: Sun Jul  9 19:36:30 2023, max compression
+gzip compressed data, was "searchenginepy-0.1.5.tar", last modified: Sun Jul  9 19:48:59 2023, max compression
```

## Comparing `searchenginepy-0.1.4.tar` & `searchenginepy-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 19:36:30.484935 searchenginepy-0.1.4/
--rw-rw-rw-   0        0        0     1069 2023-07-09 15:32:43.000000 searchenginepy-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     1807 2023-07-09 19:36:30.484935 searchenginepy-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      886 2023-07-09 19:35:32.000000 searchenginepy-0.1.4/README.md
--rw-rw-rw-   0        0        0      111 2023-07-09 19:36:30.487752 searchenginepy-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1952 2023-07-09 19:36:11.000000 searchenginepy-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-09 19:36:30.428374 searchenginepy-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-09 19:36:30.433179 searchenginepy-0.1.4/src/searchenginepy/
-drwxrwxrwx   0        0        0        0 2023-07-09 19:36:30.474146 searchenginepy-0.1.4/src/searchenginepy/Bing/
--rw-rw-rw-   0        0        0     1007 2023-07-09 19:27:30.000000 searchenginepy-0.1.4/src/searchenginepy/Bing/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 19:36:30.479165 searchenginepy-0.1.4/src/searchenginepy/Brave/
--rw-rw-rw-   0        0        0     1015 2023-07-09 19:24:03.000000 searchenginepy-0.1.4/src/searchenginepy/Brave/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 19:36:30.481300 searchenginepy-0.1.4/src/searchenginepy/DuckDuckGo/
--rw-rw-rw-   0        0        0     1021 2023-07-09 19:26:04.000000 searchenginepy-0.1.4/src/searchenginepy/DuckDuckGo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 19:36:30.482995 searchenginepy-0.1.4/src/searchenginepy/Google/
--rw-rw-rw-   0        0        0     1017 2023-07-09 18:48:11.000000 searchenginepy-0.1.4/src/searchenginepy/Google/__init__.py
--rw-rw-rw-   0        0        0      581 2023-07-09 19:17:05.000000 searchenginepy-0.1.4/src/searchenginepy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 19:36:30.474146 searchenginepy-0.1.4/src/searchenginepy.egg-info/
--rw-rw-rw-   0        0        0     1807 2023-07-09 19:36:29.000000 searchenginepy-0.1.4/src/searchenginepy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-07-09 19:36:30.000000 searchenginepy-0.1.4/src/searchenginepy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 19:36:29.000000 searchenginepy-0.1.4/src/searchenginepy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-09 19:36:29.000000 searchenginepy-0.1.4/src/searchenginepy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-09 19:36:29.000000 searchenginepy-0.1.4/src/searchenginepy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-09 19:48:59.206829 searchenginepy-0.1.5/
+-rw-rw-rw-   0        0        0     1069 2023-07-09 15:32:43.000000 searchenginepy-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     1758 2023-07-09 19:48:59.206829 searchenginepy-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      837 2023-07-09 19:37:18.000000 searchenginepy-0.1.5/README.md
+-rw-rw-rw-   0        0        0      111 2023-07-09 19:48:59.209163 searchenginepy-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1952 2023-07-09 19:48:50.000000 searchenginepy-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 19:48:59.155114 searchenginepy-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-09 19:48:59.173090 searchenginepy-0.1.5/src/searchenginepy/
+drwxrwxrwx   0        0        0        0 2023-07-09 19:48:59.199706 searchenginepy-0.1.5/src/searchenginepy/Bing/
+-rw-rw-rw-   0        0        0     1007 2023-07-09 19:27:30.000000 searchenginepy-0.1.5/src/searchenginepy/Bing/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 19:48:59.200678 searchenginepy-0.1.5/src/searchenginepy/Brave/
+-rw-rw-rw-   0        0        0     1015 2023-07-09 19:24:03.000000 searchenginepy-0.1.5/src/searchenginepy/Brave/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 19:48:59.202791 searchenginepy-0.1.5/src/searchenginepy/DuckDuckGo/
+-rw-rw-rw-   0        0        0     1021 2023-07-09 19:26:04.000000 searchenginepy-0.1.5/src/searchenginepy/DuckDuckGo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 19:48:59.203801 searchenginepy-0.1.5/src/searchenginepy/Google/
+-rw-rw-rw-   0        0        0     1017 2023-07-09 18:48:11.000000 searchenginepy-0.1.5/src/searchenginepy/Google/__init__.py
+-rw-rw-rw-   0        0        0      667 2023-07-09 19:47:55.000000 searchenginepy-0.1.5/src/searchenginepy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 19:48:59.197510 searchenginepy-0.1.5/src/searchenginepy.egg-info/
+-rw-rw-rw-   0        0        0     1758 2023-07-09 19:48:58.000000 searchenginepy-0.1.5/src/searchenginepy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-07-09 19:48:58.000000 searchenginepy-0.1.5/src/searchenginepy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 19:48:58.000000 searchenginepy-0.1.5/src/searchenginepy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-09 19:48:58.000000 searchenginepy-0.1.5/src/searchenginepy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-09 19:48:58.000000 searchenginepy-0.1.5/src/searchenginepy.egg-info/top_level.txt
```

### Comparing `searchenginepy-0.1.4/LICENSE` & `searchenginepy-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `searchenginepy-0.1.4/PKG-INFO` & `searchenginepy-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchenginepy
-Version: 0.1.4
+Version: 0.1.5
 Summary: Query popular search engines and get results easily
 Home-page: https://github.com/codewithnick/searchengine
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: codewithnick
 Author-email: nikhilsingh52645@gmail.com
 License: MIT
 Keywords: google,bing,brave,duckduckgo,search engine,crawler
@@ -79,8 +79,8 @@
 ```
 
 ## Supported search engines
 
 - Google
 - Bing
 - DuckDuckGo
-- Bravehttps://search.brave.com/search?q=test&source=web
+- Brave
```

### Comparing `searchenginepy-0.1.4/README.md` & `searchenginepy-0.1.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -58,8 +58,8 @@
 ```
 
 ## Supported search engines
 
 - Google
 - Bing
 - DuckDuckGo
-- Bravehttps://search.brave.com/search?q=test&source=web
+- Brave
```

### Comparing `searchenginepy-0.1.4/setup.py` & `searchenginepy-0.1.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'searchenginepy',         # How you named your package folder (MyLib)
-  version = '0.1.4',      # Start with a small number and increase it with every change you make
+  version = '0.1.5',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Query popular search engines and get results easily',   # Give a short description about your library
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'codewithnick',                   # Type in your name
   author_email = 'nikhilsingh52645@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/codewithnick/searchengine',   # Provide either the link to your github or to your website
```

### Comparing `searchenginepy-0.1.4/src/searchenginepy/Bing/__init__.py` & `searchenginepy-0.1.5/src/searchenginepy/Bing/__init__.py`

 * *Files identical despite different names*

### Comparing `searchenginepy-0.1.4/src/searchenginepy/Brave/__init__.py` & `searchenginepy-0.1.5/src/searchenginepy/Brave/__init__.py`

 * *Files identical despite different names*

### Comparing `searchenginepy-0.1.4/src/searchenginepy/DuckDuckGo/__init__.py` & `searchenginepy-0.1.5/src/searchenginepy/DuckDuckGo/__init__.py`

 * *Files identical despite different names*

### Comparing `searchenginepy-0.1.4/src/searchenginepy/Google/__init__.py` & `searchenginepy-0.1.5/src/searchenginepy/Google/__init__.py`

 * *Files identical despite different names*

### Comparing `searchenginepy-0.1.4/src/searchenginepy/__init__.py` & `searchenginepy-0.1.5/src/searchenginepy/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # __init__.py
 # #importing google class
 from .Google import Google
+from .Bing import Bing
+from .DuckDuckGo import DuckDuckGo
+from .Brave import Brave
 import logging
 __pkgname='searchenginepy'
 logging.basicConfig(level=logging.INFO)
 log = logging.getLogger(__name__)
 
 log.info('Initializing '+__pkgname+' package')
```

### Comparing `searchenginepy-0.1.4/src/searchenginepy.egg-info/PKG-INFO` & `searchenginepy-0.1.5/src/searchenginepy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchenginepy
-Version: 0.1.4
+Version: 0.1.5
 Summary: Query popular search engines and get results easily
 Home-page: https://github.com/codewithnick/searchengine
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: codewithnick
 Author-email: nikhilsingh52645@gmail.com
 License: MIT
 Keywords: google,bing,brave,duckduckgo,search engine,crawler
@@ -79,8 +79,8 @@
 ```
 
 ## Supported search engines
 
 - Google
 - Bing
 - DuckDuckGo
-- Bravehttps://search.brave.com/search?q=test&source=web
+- Brave
```

