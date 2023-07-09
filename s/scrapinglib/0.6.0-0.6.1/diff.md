# Comparing `tmp/scrapinglib-0.6.0.tar.gz` & `tmp/scrapinglib-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scrapinglib-0.6.0.tar", last modified: Mon May 22 02:56:36 2023, max compression
+gzip compressed data, was "dist/scrapinglib-0.6.1.tar", last modified: Sun Jul  9 10:29:11 2023, max compression
```

## Comparing `scrapinglib-0.6.0.tar` & `scrapinglib-0.6.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:56:36.000000 scrapinglib-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:56:36.000000 scrapinglib-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:56:36.000000 scrapinglib-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-22 02:56:36.000000 scrapinglib-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:56:36.000000 scrapinglib-0.6.0/scrapinglib/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/airav.py
--rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/avsox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/carib.py
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/dlsite.py
--rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/fanza.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/fc2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/gcolle.py
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/getchu.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/httprequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/imdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/jav321.py
--rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/javbus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/javday.py
--rw-r--r--   0 runner    (1001) docker     (123)    10679 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/javdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/javlibrary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/madou.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/mgstage.py
--rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/storyline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/tmdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/xcity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:56:36.000000 scrapinglib-0.6.0/scrapinglib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-22 02:56:36.000000 scrapinglib-0.6.0/scrapinglib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-22 02:56:36.000000 scrapinglib-0.6.0/scrapinglib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 02:56:36.000000 scrapinglib-0.6.0/scrapinglib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-22 02:56:36.000000 scrapinglib-0.6.0/scrapinglib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 02:56:36.000000 scrapinglib-0.6.0/scrapinglib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 02:56:36.000000 scrapinglib-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:56:36.000000 scrapinglib-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9449 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:29:11.000000 scrapinglib-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-09 10:28:59.000000 scrapinglib-0.6.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:29:11.000000 scrapinglib-0.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:29:11.000000 scrapinglib-0.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-09 10:28:59.000000 scrapinglib-0.6.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-09 10:28:59.000000 scrapinglib-0.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-09 10:29:11.000000 scrapinglib-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-09 10:28:59.000000 scrapinglib-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:29:11.000000 scrapinglib-0.6.1/scrapinglib/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-09 10:28:59.000000 scrapinglib-0.6.1/scrapinglib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-07-09 10:28:59.000000 scrapinglib-0.6.1/scrapinglib/airav.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-07-09 10:28:59.000000 scrapinglib-0.6.1/scrapinglib/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-07-09 10:28:59.000000 scrapinglib-0.6.1/scrapinglib/avsox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-07-09 10:28:59.000000 scrapinglib-0.6.1/scrapinglib/carib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-07-09 10:28:59.000000 scrapinglib-0.6.1/scrapinglib/dlsite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-07-09 10:28:59.000000 scrapinglib-0.6.1/scrapinglib/fanza.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-09 10:28:59.000000 scrapinglib-0.6.1/scrapinglib/fc2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-09 10:28:59.000000 scrapinglib-0.6.1/scrapinglib/gcolle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-07-09 10:28:59.000000 scrapinglib-0.6.1/scrapinglib/getchu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-07-09 10:28:59.000000 scrapinglib-0.6.1/scrapinglib/httprequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-09 10:28:59.000000 scrapinglib-0.6.1/scrapinglib/imdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-09 10:28:59.000000 scrapinglib-0.6.1/scrapinglib/jav321.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-07-09 10:28:59.000000 scrapinglib-0.6.1/scrapinglib/javbus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-09 10:28:59.000000 scrapinglib-0.6.1/scrapinglib/javday.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10679 2023-07-09 10:28:59.000000 scrapinglib-0.6.1/scrapinglib/javdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-09 10:28:59.000000 scrapinglib-0.6.1/scrapinglib/javlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-07-09 10:28:59.000000 scrapinglib-0.6.1/scrapinglib/madou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-07-09 10:28:59.000000 scrapinglib-0.6.1/scrapinglib/mgstage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-07-09 10:28:59.000000 scrapinglib-0.6.1/scrapinglib/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-07-09 10:28:59.000000 scrapinglib-0.6.1/scrapinglib/storyline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-09 10:28:59.000000 scrapinglib-0.6.1/scrapinglib/tmdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-09 10:28:59.000000 scrapinglib-0.6.1/scrapinglib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-07-09 10:28:59.000000 scrapinglib-0.6.1/scrapinglib/xcity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:29:11.000000 scrapinglib-0.6.1/scrapinglib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-09 10:29:11.000000 scrapinglib-0.6.1/scrapinglib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-09 10:29:11.000000 scrapinglib-0.6.1/scrapinglib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 10:29:11.000000 scrapinglib-0.6.1/scrapinglib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-09 10:29:11.000000 scrapinglib-0.6.1/scrapinglib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-09 10:29:11.000000 scrapinglib-0.6.1/scrapinglib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 10:29:11.000000 scrapinglib-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-09 10:28:59.000000 scrapinglib-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:29:11.000000 scrapinglib-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9459 2023-07-09 10:28:59.000000 scrapinglib-0.6.1/tests/test.py
```

### Comparing `scrapinglib-0.6.0/.github/workflows/release.yml` & `scrapinglib-0.6.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.6.0/.gitignore` & `scrapinglib-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.6.0/PKG-INFO` & `scrapinglib-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapinglib
-Version: 0.6.0
+Version: 0.6.1
 Summary: UNKNOWN
 Home-page: https://github.com/Suwmlee/scrapinglib
 Author: suwmlee
 Author-email: suwmlee@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Suwmlee/scrapinglib/issues
 Project-URL: Source, https://github.com/Suwmlee/scrapinglib
```

### Comparing `scrapinglib-0.6.0/scrapinglib/airav.py` & `scrapinglib-0.6.1/scrapinglib/airav.py`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.6.0/scrapinglib/api.py` & `scrapinglib-0.6.1/scrapinglib/api.py`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.6.0/scrapinglib/avsox.py` & `scrapinglib-0.6.1/scrapinglib/avsox.py`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.6.0/scrapinglib/carib.py` & `scrapinglib-0.6.1/scrapinglib/carib.py`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.6.0/scrapinglib/dlsite.py` & `scrapinglib-0.6.1/scrapinglib/dlsite.py`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.6.0/scrapinglib/fanza.py` & `scrapinglib-0.6.1/scrapinglib/fanza.py`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.6.0/scrapinglib/fc2.py` & `scrapinglib-0.6.1/scrapinglib/fc2.py`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.6.0/scrapinglib/gcolle.py` & `scrapinglib-0.6.1/scrapinglib/gcolle.py`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.6.0/scrapinglib/getchu.py` & `scrapinglib-0.6.1/scrapinglib/getchu.py`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.6.0/scrapinglib/httprequest.py` & `scrapinglib-0.6.1/scrapinglib/httprequest.py`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.6.0/scrapinglib/imdb.py` & `scrapinglib-0.6.1/scrapinglib/imdb.py`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.6.0/scrapinglib/jav321.py` & `scrapinglib-0.6.1/scrapinglib/jav321.py`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.6.0/scrapinglib/javbus.py` & `scrapinglib-0.6.1/scrapinglib/javbus.py`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.6.0/scrapinglib/javday.py` & `scrapinglib-0.6.1/scrapinglib/javday.py`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.6.0/scrapinglib/javdb.py` & `scrapinglib-0.6.1/scrapinglib/javdb.py`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.6.0/scrapinglib/javlibrary.py` & `scrapinglib-0.6.1/scrapinglib/javlibrary.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,16 +58,20 @@
             return queryResult.url
         else:
             queryTree = etree.fromstring(queryResult.text, etree.HTMLParser())
             numbers = queryTree.xpath('//div[@class="id"]/text()')
             if number in numbers:
                 urls = queryTree.xpath('//div[@class="id"]/../@href')
                 if len(numbers) == 2 and numbers[0] == numbers[1]:
-                    # 两个相同番号，第一个结果海报被拉伸，第二个正常
-                    detailurl = urls[1]
+                    # 相同番号, 剔除标题含 ブルーレイディスク 字段
+                    titles = queryTree.xpath('//div[@class="title"]/text()')
+                    if titles and "ブルーレイディスク" in titles[0]:
+                        detailurl = urls[1]
+                    else:
+                        detailurl = urls[0]
                 else:
                     detailurl = urls[numbers.index(number)]
                 return "http://www.javlibrary.com/cn" + detailurl.strip('.')
         return None
 
     def getTitle(self, htmltree):
         title = super().getTitle(htmltree)
```

### Comparing `scrapinglib-0.6.0/scrapinglib/madou.py` & `scrapinglib-0.6.1/scrapinglib/madou.py`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.6.0/scrapinglib/mgstage.py` & `scrapinglib-0.6.1/scrapinglib/mgstage.py`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.6.0/scrapinglib/parser.py` & `scrapinglib-0.6.1/scrapinglib/parser.py`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.6.0/scrapinglib/storyline.py` & `scrapinglib-0.6.1/scrapinglib/storyline.py`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.6.0/scrapinglib/tmdb.py` & `scrapinglib-0.6.1/scrapinglib/tmdb.py`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.6.0/scrapinglib/utils.py` & `scrapinglib-0.6.1/scrapinglib/utils.py`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.6.0/scrapinglib/xcity.py` & `scrapinglib-0.6.1/scrapinglib/xcity.py`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.6.0/scrapinglib.egg-info/PKG-INFO` & `scrapinglib-0.6.1/scrapinglib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapinglib
-Version: 0.6.0
+Version: 0.6.1
 Summary: UNKNOWN
 Home-page: https://github.com/Suwmlee/scrapinglib
 Author: suwmlee
 Author-email: suwmlee@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Suwmlee/scrapinglib/issues
 Project-URL: Source, https://github.com/Suwmlee/scrapinglib
```

### Comparing `scrapinglib-0.6.0/scrapinglib.egg-info/SOURCES.txt` & `scrapinglib-0.6.1/scrapinglib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.6.0/setup.py` & `scrapinglib-0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ]
 
 with open("README.md", "r", "utf-8") as f:
     readme = f.read()
 
 setup(
     name='scrapinglib',
-    version='0.6.0',
+    version='0.6.1',
     author="suwmlee",
     author_email='suwmlee@gmail.com',
     url='https://github.com/Suwmlee/scrapinglib',
     long_description=readme,
     long_description_content_type="text/markdown",
     packages=["scrapinglib"],
     package_dir={'scrapinglib': 'scrapinglib'},
```

### Comparing `scrapinglib-0.6.0/tests/test.py` & `scrapinglib-0.6.1/tests/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 # print(search('GETCHU-1139198', 'getchu', proxies=proxydict))
 # print(search('GETCHU-1139198', specifiedSource='getchu', specifiedUrl='http://www.getchu.com/soft.phtml?id=1139198', proxies=proxydict))
 
 # print(search('IPX-292', 'javlibrary', proxies=proxydict))
 # print(search('STAR-438', 'javlibrary', proxies=proxydict, morestoryline=True))
 # print(search('SNIS-003', 'javlibrary', proxies=proxydict, morestoryline=True))
 # print(search('n1403', 'javlibrary', proxies=proxydict))   # not found
-# print(search('SSNI-468', 'javlibrary', proxies=proxydict))
+# print(search('SSIS-698', 'javlibrary', proxies=proxydict))  # bluray
 # print(search('SSNI-468', specifiedSource='javlibrary', specifiedUrl='https://www.javlibrary.com/cn/?v=javli7zkyu', proxies=proxydict))
 
 # print(search('EBOD-646', proxies=proxydict))
 
 # print(search('14534', 'tmdb', type='general'))
 # print(search('526896', 'tmdb', type='general'))
 # print(search('the dark knight', 'tmdb', type='general'))
```

