# Comparing `tmp/searchenginepy-0.1.3.tar.gz` & `tmp/searchenginepy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchenginepy-0.1.3.tar", last modified: Sun Jul  9 19:12:10 2023, max compression
+gzip compressed data, was "searchenginepy-0.1.4.tar", last modified: Sun Jul  9 19:36:30 2023, max compression
```

## Comparing `searchenginepy-0.1.3.tar` & `searchenginepy-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 19:12:10.000454 searchenginepy-0.1.3/
--rw-rw-rw-   0        0        0     1069 2023-07-09 15:32:43.000000 searchenginepy-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     1396 2023-07-09 19:12:10.000454 searchenginepy-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      528 2023-07-09 18:56:35.000000 searchenginepy-0.1.3/README.md
--rw-rw-rw-   0        0        0      111 2023-07-09 19:12:10.004987 searchenginepy-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1924 2023-07-09 19:12:03.000000 searchenginepy-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-09 19:12:09.957810 searchenginepy-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-09 19:12:09.966163 searchenginepy-0.1.3/src/searchenginepy/
-drwxrwxrwx   0        0        0        0 2023-07-09 19:12:09.991528 searchenginepy-0.1.3/src/searchenginepy/Brave/
--rw-rw-rw-   0        0        0        0 2023-07-09 16:19:13.000000 searchenginepy-0.1.3/src/searchenginepy/Brave/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 19:12:09.991528 searchenginepy-0.1.3/src/searchenginepy/DuckDuckGo/
--rw-rw-rw-   0        0        0        0 2023-07-09 16:19:24.000000 searchenginepy-0.1.3/src/searchenginepy/DuckDuckGo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 19:12:09.991528 searchenginepy-0.1.3/src/searchenginepy/Google/
--rw-rw-rw-   0        0        0     1017 2023-07-09 18:48:11.000000 searchenginepy-0.1.3/src/searchenginepy/Google/__init__.py
--rw-rw-rw-   0        0        0      583 2023-07-09 18:19:37.000000 searchenginepy-0.1.3/src/searchenginepy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 19:12:09.991528 searchenginepy-0.1.3/src/searchenginepy.egg-info/
--rw-rw-rw-   0        0        0     1396 2023-07-09 19:12:09.000000 searchenginepy-0.1.3/src/searchenginepy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2023-07-09 19:12:09.000000 searchenginepy-0.1.3/src/searchenginepy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 19:12:09.000000 searchenginepy-0.1.3/src/searchenginepy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-09 19:12:09.000000 searchenginepy-0.1.3/src/searchenginepy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-09 19:12:09.000000 searchenginepy-0.1.3/src/searchenginepy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-09 19:36:30.484935 searchenginepy-0.1.4/
+-rw-rw-rw-   0        0        0     1069 2023-07-09 15:32:43.000000 searchenginepy-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     1807 2023-07-09 19:36:30.484935 searchenginepy-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      886 2023-07-09 19:35:32.000000 searchenginepy-0.1.4/README.md
+-rw-rw-rw-   0        0        0      111 2023-07-09 19:36:30.487752 searchenginepy-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1952 2023-07-09 19:36:11.000000 searchenginepy-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 19:36:30.428374 searchenginepy-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-09 19:36:30.433179 searchenginepy-0.1.4/src/searchenginepy/
+drwxrwxrwx   0        0        0        0 2023-07-09 19:36:30.474146 searchenginepy-0.1.4/src/searchenginepy/Bing/
+-rw-rw-rw-   0        0        0     1007 2023-07-09 19:27:30.000000 searchenginepy-0.1.4/src/searchenginepy/Bing/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 19:36:30.479165 searchenginepy-0.1.4/src/searchenginepy/Brave/
+-rw-rw-rw-   0        0        0     1015 2023-07-09 19:24:03.000000 searchenginepy-0.1.4/src/searchenginepy/Brave/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 19:36:30.481300 searchenginepy-0.1.4/src/searchenginepy/DuckDuckGo/
+-rw-rw-rw-   0        0        0     1021 2023-07-09 19:26:04.000000 searchenginepy-0.1.4/src/searchenginepy/DuckDuckGo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 19:36:30.482995 searchenginepy-0.1.4/src/searchenginepy/Google/
+-rw-rw-rw-   0        0        0     1017 2023-07-09 18:48:11.000000 searchenginepy-0.1.4/src/searchenginepy/Google/__init__.py
+-rw-rw-rw-   0        0        0      581 2023-07-09 19:17:05.000000 searchenginepy-0.1.4/src/searchenginepy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 19:36:30.474146 searchenginepy-0.1.4/src/searchenginepy.egg-info/
+-rw-rw-rw-   0        0        0     1807 2023-07-09 19:36:29.000000 searchenginepy-0.1.4/src/searchenginepy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-07-09 19:36:30.000000 searchenginepy-0.1.4/src/searchenginepy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 19:36:29.000000 searchenginepy-0.1.4/src/searchenginepy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-09 19:36:29.000000 searchenginepy-0.1.4/src/searchenginepy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-09 19:36:29.000000 searchenginepy-0.1.4/src/searchenginepy.egg-info/top_level.txt
```

### Comparing `searchenginepy-0.1.3/LICENSE` & `searchenginepy-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `searchenginepy-0.1.3/README.md` & `searchenginepy-0.1.4/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,65 @@
 # searchenginepy
+
 search engine for python (Query and scrape search engines)
 
 # How to use?
 
-##### Installation
+## Installation
+
 `pip install searchenginepy`
-##### Importing
-``` 
-import searchenginepy 
-``` 
-
-##### Usage
-``` 
-list=searchenginepy.search("search query")
-``` 
-
-##### Example
-``` 
-list=searchenginepy.google("search query")
-``` 
+
+## Importing
+
+```
+import SearchEngine from searchenginepy
+engine=SearchEngine()
+```
+
+## Usage
+
+```
+list=engine.search("search query")
+```
+
+## Example
+
+```
+list=engine.google("search query")
+```
 
 using google to search a query
+
 ## Using a specific search engine
+
+### google
+
 ```
 from searchenginepy import Google
 list=Google().search("search query")
 ```
 
-##### Supported search engines
+### Bing
+
+```
+from searchenginepy import Bing
+list=Bing().search("search query")
+```
+### Brave
+```
+from searchenginepy import Brave
+list=Brave().search("search query")
+```
+
+### DuckDuckGo
+
+```
+from searchenginepy import DuckDuckGo
+list=DuckDuckGo().search("search query")
+```
+
+## Supported search engines
+
 - Google
 - Bing
-- DuckDuckGo
+- DuckDuckGo
+- Bravehttps://search.brave.com/search?q=test&source=web
```

### Comparing `searchenginepy-0.1.3/setup.py` & `searchenginepy-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'searchenginepy',         # How you named your package folder (MyLib)
-  version = '0.1.3',      # Start with a small number and increase it with every change you make
+  version = '0.1.4',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Query popular search engines and get results easily',   # Give a short description about your library
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'codewithnick',                   # Type in your name
   author_email = 'nikhilsingh52645@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/codewithnick/searchengine',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',    # I explain this later on
-  keywords = ['google', 'search engine', 'crawler'],   # Keywords that define your package best
+  keywords = ['google','bing','brave','duckduckgo', 'search engine', 'crawler'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'requests',
           'beautifulsoup4',
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
```

### Comparing `searchenginepy-0.1.3/src/searchenginepy/Google/__init__.py` & `searchenginepy-0.1.4/src/searchenginepy/Google/__init__.py`

 * *Files identical despite different names*

### Comparing `searchenginepy-0.1.3/src/searchenginepy/__init__.py` & `searchenginepy-0.1.4/src/searchenginepy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 log.info('Initializing '+__pkgname+' package')
 
 class SearchEngine:
     def __init__(self, query):
         self.query = query
         self.results = []
-
     def google(self):
         googleobj=Google()
         result=googleobj.search(self.query)
         return result
     def get_results(self):
         return self.results
```

