# Comparing `tmp/searchenginepy-0.1.5.tar.gz` & `tmp/searchenginepy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchenginepy-0.1.5.tar", last modified: Sun Jul  9 19:48:59 2023, max compression
+gzip compressed data, was "searchenginepy-0.1.6.tar", last modified: Sun Jul  9 20:05:45 2023, max compression
```

## Comparing `searchenginepy-0.1.5.tar` & `searchenginepy-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 19:48:59.206829 searchenginepy-0.1.5/
--rw-rw-rw-   0        0        0     1069 2023-07-09 15:32:43.000000 searchenginepy-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     1758 2023-07-09 19:48:59.206829 searchenginepy-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      837 2023-07-09 19:37:18.000000 searchenginepy-0.1.5/README.md
--rw-rw-rw-   0        0        0      111 2023-07-09 19:48:59.209163 searchenginepy-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1952 2023-07-09 19:48:50.000000 searchenginepy-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-09 19:48:59.155114 searchenginepy-0.1.5/src/
-drwxrwxrwx   0        0        0        0 2023-07-09 19:48:59.173090 searchenginepy-0.1.5/src/searchenginepy/
-drwxrwxrwx   0        0        0        0 2023-07-09 19:48:59.199706 searchenginepy-0.1.5/src/searchenginepy/Bing/
--rw-rw-rw-   0        0        0     1007 2023-07-09 19:27:30.000000 searchenginepy-0.1.5/src/searchenginepy/Bing/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 19:48:59.200678 searchenginepy-0.1.5/src/searchenginepy/Brave/
--rw-rw-rw-   0        0        0     1015 2023-07-09 19:24:03.000000 searchenginepy-0.1.5/src/searchenginepy/Brave/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 19:48:59.202791 searchenginepy-0.1.5/src/searchenginepy/DuckDuckGo/
--rw-rw-rw-   0        0        0     1021 2023-07-09 19:26:04.000000 searchenginepy-0.1.5/src/searchenginepy/DuckDuckGo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 19:48:59.203801 searchenginepy-0.1.5/src/searchenginepy/Google/
--rw-rw-rw-   0        0        0     1017 2023-07-09 18:48:11.000000 searchenginepy-0.1.5/src/searchenginepy/Google/__init__.py
--rw-rw-rw-   0        0        0      667 2023-07-09 19:47:55.000000 searchenginepy-0.1.5/src/searchenginepy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 19:48:59.197510 searchenginepy-0.1.5/src/searchenginepy.egg-info/
--rw-rw-rw-   0        0        0     1758 2023-07-09 19:48:58.000000 searchenginepy-0.1.5/src/searchenginepy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-07-09 19:48:58.000000 searchenginepy-0.1.5/src/searchenginepy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 19:48:58.000000 searchenginepy-0.1.5/src/searchenginepy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-09 19:48:58.000000 searchenginepy-0.1.5/src/searchenginepy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-09 19:48:58.000000 searchenginepy-0.1.5/src/searchenginepy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-09 20:05:45.716262 searchenginepy-0.1.6/
+-rw-rw-rw-   0        0        0     1069 2023-07-09 15:32:43.000000 searchenginepy-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     1787 2023-07-09 20:05:45.716262 searchenginepy-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      866 2023-07-09 19:53:29.000000 searchenginepy-0.1.6/README.md
+-rw-rw-rw-   0        0        0      111 2023-07-09 20:05:45.719255 searchenginepy-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1952 2023-07-09 20:05:25.000000 searchenginepy-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 20:05:45.667076 searchenginepy-0.1.6/src/
+drwxrwxrwx   0        0        0        0 2023-07-09 20:05:45.686360 searchenginepy-0.1.6/src/searchenginepy/
+drwxrwxrwx   0        0        0        0 2023-07-09 20:05:45.708256 searchenginepy-0.1.6/src/searchenginepy/Bing/
+-rw-rw-rw-   0        0        0     1007 2023-07-09 19:27:30.000000 searchenginepy-0.1.6/src/searchenginepy/Bing/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 20:05:45.710259 searchenginepy-0.1.6/src/searchenginepy/Brave/
+-rw-rw-rw-   0        0        0     1015 2023-07-09 19:24:03.000000 searchenginepy-0.1.6/src/searchenginepy/Brave/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 20:05:45.711257 searchenginepy-0.1.6/src/searchenginepy/DuckDuckGo/
+-rw-rw-rw-   0        0        0     1021 2023-07-09 19:26:04.000000 searchenginepy-0.1.6/src/searchenginepy/DuckDuckGo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 20:05:45.713257 searchenginepy-0.1.6/src/searchenginepy/Google/
+-rw-rw-rw-   0        0        0     1017 2023-07-09 18:48:11.000000 searchenginepy-0.1.6/src/searchenginepy/Google/__init__.py
+-rw-rw-rw-   0        0        0     1028 2023-07-09 20:00:06.000000 searchenginepy-0.1.6/src/searchenginepy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 20:05:45.707254 searchenginepy-0.1.6/src/searchenginepy.egg-info/
+-rw-rw-rw-   0        0        0     1787 2023-07-09 20:05:44.000000 searchenginepy-0.1.6/src/searchenginepy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-07-09 20:05:45.000000 searchenginepy-0.1.6/src/searchenginepy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 20:05:44.000000 searchenginepy-0.1.6/src/searchenginepy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-09 20:05:44.000000 searchenginepy-0.1.6/src/searchenginepy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-09 20:05:44.000000 searchenginepy-0.1.6/src/searchenginepy.egg-info/top_level.txt
```

### Comparing `searchenginepy-0.1.5/LICENSE` & `searchenginepy-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `searchenginepy-0.1.5/PKG-INFO` & `searchenginepy-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchenginepy
-Version: 0.1.5
+Version: 0.1.6
 Summary: Query popular search engines and get results easily
 Home-page: https://github.com/codewithnick/searchengine
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: codewithnick
 Author-email: nikhilsingh52645@gmail.com
 License: MIT
 Keywords: google,bing,brave,duckduckgo,search engine,crawler
@@ -51,34 +51,34 @@
 using google to search a query
 
 ## Using a specific search engine
 
 ### google
 
 ```
-from searchenginepy import Google
+from searchenginepy.Google import Google
 list=Google().search("search query")
 ```
 
 ### Bing
 
 ```
-from searchenginepy import Bing
+from searchenginepy.Bing import Bing
 list=Bing().search("search query")
 ```
 ### Brave
 ```
-from searchenginepy import Brave
+from searchenginepy.Brave import Brave
 list=Brave().search("search query")
 ```
 
 ### DuckDuckGo
 
 ```
-from searchenginepy import DuckDuckGo
+from searchenginepy.DuckDuckGo import DuckDuckGo
 list=DuckDuckGo().search("search query")
 ```
 
 ## Supported search engines
 
 - Google
 - Bing
```

### Comparing `searchenginepy-0.1.5/README.md` & `searchenginepy-0.1.6/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -30,34 +30,34 @@
 using google to search a query
 
 ## Using a specific search engine
 
 ### google
 
 ```
-from searchenginepy import Google
+from searchenginepy.Google import Google
 list=Google().search("search query")
 ```
 
 ### Bing
 
 ```
-from searchenginepy import Bing
+from searchenginepy.Bing import Bing
 list=Bing().search("search query")
 ```
 ### Brave
 ```
-from searchenginepy import Brave
+from searchenginepy.Brave import Brave
 list=Brave().search("search query")
 ```
 
 ### DuckDuckGo
 
 ```
-from searchenginepy import DuckDuckGo
+from searchenginepy.DuckDuckGo import DuckDuckGo
 list=DuckDuckGo().search("search query")
 ```
 
 ## Supported search engines
 
 - Google
 - Bing
```

### Comparing `searchenginepy-0.1.5/setup.py` & `searchenginepy-0.1.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'searchenginepy',         # How you named your package folder (MyLib)
-  version = '0.1.5',      # Start with a small number and increase it with every change you make
+  version = '0.1.6',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Query popular search engines and get results easily',   # Give a short description about your library
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'codewithnick',                   # Type in your name
   author_email = 'nikhilsingh52645@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/codewithnick/searchengine',   # Provide either the link to your github or to your website
```

### Comparing `searchenginepy-0.1.5/src/searchenginepy/Bing/__init__.py` & `searchenginepy-0.1.6/src/searchenginepy/Bing/__init__.py`

 * *Files identical despite different names*

### Comparing `searchenginepy-0.1.5/src/searchenginepy/Brave/__init__.py` & `searchenginepy-0.1.6/src/searchenginepy/Brave/__init__.py`

 * *Files identical despite different names*

### Comparing `searchenginepy-0.1.5/src/searchenginepy/DuckDuckGo/__init__.py` & `searchenginepy-0.1.6/src/searchenginepy/DuckDuckGo/__init__.py`

 * *Files identical despite different names*

### Comparing `searchenginepy-0.1.5/src/searchenginepy/Google/__init__.py` & `searchenginepy-0.1.6/src/searchenginepy/Google/__init__.py`

 * *Files identical despite different names*

### Comparing `searchenginepy-0.1.5/src/searchenginepy/__init__.py` & `searchenginepy-0.1.6/src/searchenginepy/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # __init__.py
 # #importing google class
 from .Google import Google
 from .Bing import Bing
-from .DuckDuckGo import DuckDuckGo
+from .DuckDuckGo import Duckduckgo
 from .Brave import Brave
 import logging
 __pkgname='searchenginepy'
 logging.basicConfig(level=logging.INFO)
 log = logging.getLogger(__name__)
 
 log.info('Initializing '+__pkgname+' package')
@@ -15,12 +15,24 @@
     def __init__(self, query):
         self.query = query
         self.results = []
     def google(self):
         googleobj=Google()
         result=googleobj.search(self.query)
         return result
+    def bing(self):
+        bingobj=Bing()
+        result=bingobj.search(self.query)
+        return result
+    def duckduckgo(self):
+        duckduckgoobj=Duckduckgo()
+        result=duckduckgoobj.search(self.query)
+        return result
+    def brave(self):
+        braveobj=Brave()
+        result=braveobj.search(self.query)
+        return result
     def get_results(self):
         return self.results
 
     def get_query(self):
         return self.query
```

### Comparing `searchenginepy-0.1.5/src/searchenginepy.egg-info/PKG-INFO` & `searchenginepy-0.1.6/src/searchenginepy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchenginepy
-Version: 0.1.5
+Version: 0.1.6
 Summary: Query popular search engines and get results easily
 Home-page: https://github.com/codewithnick/searchengine
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: codewithnick
 Author-email: nikhilsingh52645@gmail.com
 License: MIT
 Keywords: google,bing,brave,duckduckgo,search engine,crawler
@@ -51,34 +51,34 @@
 using google to search a query
 
 ## Using a specific search engine
 
 ### google
 
 ```
-from searchenginepy import Google
+from searchenginepy.Google import Google
 list=Google().search("search query")
 ```
 
 ### Bing
 
 ```
-from searchenginepy import Bing
+from searchenginepy.Bing import Bing
 list=Bing().search("search query")
 ```
 ### Brave
 ```
-from searchenginepy import Brave
+from searchenginepy.Brave import Brave
 list=Brave().search("search query")
 ```
 
 ### DuckDuckGo
 
 ```
-from searchenginepy import DuckDuckGo
+from searchenginepy.DuckDuckGo import DuckDuckGo
 list=DuckDuckGo().search("search query")
 ```
 
 ## Supported search engines
 
 - Google
 - Bing
```

