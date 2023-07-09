# Comparing `tmp/autokattis-1.4.4.tar.gz` & `tmp/autokattis-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autokattis-1.4.4.tar", last modified: Tue Jun 20 09:10:38 2023, max compression
+gzip compressed data, was "autokattis-1.4.5.tar", last modified: Sun Jul  9 08:57:56 2023, max compression
```

## Comparing `autokattis-1.4.4.tar` & `autokattis-1.4.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-06-20 09:10:38.300587 autokattis-1.4.4/
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)    35148 2023-05-04 07:45:56.000000 autokattis-1.4.4/LICENSE
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)     2639 2023-06-20 09:10:38.299526 autokattis-1.4.4/PKG-INFO
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)     2285 2023-06-20 09:03:54.000000 autokattis-1.4.4/README.md
-drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-06-20 09:10:38.274178 autokattis-1.4.4/autokattis/
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       24 2023-05-11 09:21:05.000000 autokattis-1.4.4/autokattis/__init__.py
-drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-06-20 09:10:38.288192 autokattis-1.4.4/autokattis/api/
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)    22404 2023-06-20 08:58:31.000000 autokattis-1.4.4/autokattis/api/__init__.py
-drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-06-20 09:10:38.290491 autokattis-1.4.4/autokattis/database/
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)   133880 2023-05-08 08:31:18.000000 autokattis-1.4.4/autokattis/database/__init__.py
-drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-06-20 09:10:38.295490 autokattis-1.4.4/autokattis/scraper/
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       37 2023-05-11 07:47:42.000000 autokattis-1.4.4/autokattis/scraper/__init__.py
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)     3031 2023-05-11 07:45:04.000000 autokattis-1.4.4/autokattis/scraper/country.py
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)      977 2023-05-11 07:45:16.000000 autokattis-1.4.4/autokattis/scraper/university.py
-drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-06-20 09:10:38.298490 autokattis-1.4.4/autokattis/utils/
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)      518 2023-05-11 07:23:19.000000 autokattis-1.4.4/autokattis/utils/__init__.py
-drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-06-20 09:10:38.287178 autokattis-1.4.4/autokattis.egg-info/
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)     2639 2023-06-20 09:10:38.000000 autokattis-1.4.4/autokattis.egg-info/PKG-INFO
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)      400 2023-06-20 09:10:38.000000 autokattis-1.4.4/autokattis.egg-info/SOURCES.txt
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)        1 2023-06-20 09:10:38.000000 autokattis-1.4.4/autokattis.egg-info/dependency_links.txt
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       80 2023-06-20 09:10:38.000000 autokattis-1.4.4/autokattis.egg-info/requires.txt
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       11 2023-06-20 09:10:38.000000 autokattis-1.4.4/autokattis.egg-info/top_level.txt
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       38 2023-06-20 09:10:38.301490 autokattis-1.4.4/setup.cfg
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)      878 2023-06-20 08:56:45.000000 autokattis-1.4.4/setup.py
+drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-07-09 08:57:56.573488 autokattis-1.4.5/
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)    35148 2023-05-04 07:45:56.000000 autokattis-1.4.5/LICENSE
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)     2639 2023-07-09 08:57:56.572488 autokattis-1.4.5/PKG-INFO
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)     2285 2023-06-20 09:03:54.000000 autokattis-1.4.5/README.md
+drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-07-09 08:57:56.547473 autokattis-1.4.5/autokattis/
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       24 2023-05-11 09:21:05.000000 autokattis-1.4.5/autokattis/__init__.py
+drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-07-09 08:57:56.560763 autokattis-1.4.5/autokattis/api/
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)    22404 2023-07-09 08:54:22.000000 autokattis-1.4.5/autokattis/api/__init__.py
+drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-07-09 08:57:56.561762 autokattis-1.4.5/autokattis/database/
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)   133880 2023-05-08 08:31:18.000000 autokattis-1.4.5/autokattis/database/__init__.py
+drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-07-09 08:57:56.569491 autokattis-1.4.5/autokattis/scraper/
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       37 2023-05-11 07:47:42.000000 autokattis-1.4.5/autokattis/scraper/__init__.py
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)     3031 2023-05-11 07:45:04.000000 autokattis-1.4.5/autokattis/scraper/country.py
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)      977 2023-05-11 07:45:16.000000 autokattis-1.4.5/autokattis/scraper/university.py
+drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-07-09 08:57:56.571489 autokattis-1.4.5/autokattis/utils/
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)      518 2023-05-11 07:23:19.000000 autokattis-1.4.5/autokattis/utils/__init__.py
+drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-07-09 08:57:56.558747 autokattis-1.4.5/autokattis.egg-info/
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)     2639 2023-07-09 08:57:56.000000 autokattis-1.4.5/autokattis.egg-info/PKG-INFO
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)      400 2023-07-09 08:57:56.000000 autokattis-1.4.5/autokattis.egg-info/SOURCES.txt
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)        1 2023-07-09 08:57:56.000000 autokattis-1.4.5/autokattis.egg-info/dependency_links.txt
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       80 2023-07-09 08:57:56.000000 autokattis-1.4.5/autokattis.egg-info/requires.txt
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       11 2023-07-09 08:57:56.000000 autokattis-1.4.5/autokattis.egg-info/top_level.txt
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       38 2023-07-09 08:57:56.574489 autokattis-1.4.5/setup.cfg
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)      878 2023-07-09 08:54:41.000000 autokattis-1.4.5/setup.py
```

### Comparing `autokattis-1.4.4/LICENSE` & `autokattis-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `autokattis-1.4.4/PKG-INFO` & `autokattis-1.4.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autokattis
-Version: 1.4.4
+Version: 1.4.5
 Summary: Updated Kattis API wrapper
 Home-page: https://github.com/RussellDash332/autokattis
 Download-URL: https://pypi.org/project/autokattis/
 Author: Russell Saerang
 Author-email: russellsaerang@gmail.com
 License: MIT
 Keywords: Kattis
```

### Comparing `autokattis-1.4.4/README.md` & `autokattis-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `autokattis-1.4.4/autokattis/api/__init__.py` & `autokattis-1.4.5/autokattis/api/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -126,18 +126,18 @@
         Default: plots all solved and partially solved problems without saving it to any file.
         '''
 
         df = pd.DataFrame(self.problems(show_solved, show_partial, show_tried, show_untried))
         hist = sns.histplot(data=df, x='difficulty', hue='category', multiple='stack', binwidth=0.1)
         hist.set(title=f'Solved Kattis Problems ({df.shape[0]})', xlabel='Difficulty')
         plt.xticks([*range(math.floor(min(df.difficulty)), math.ceil(max(df.difficulty))+1)])
-        plt.show()
         if filepath != None:
             plt.savefig(filepath)
             print(f'Saved to {filepath}')
+        plt.show()
 
     def list_unsolved(self, show_partial=True):
         '''
         Quick shortcut for all Kattis grinders to list all unsolved questions.
 
         Default: includes partially solved questions.
         '''
```

### Comparing `autokattis-1.4.4/autokattis/database/__init__.py` & `autokattis-1.4.5/autokattis/database/__init__.py`

 * *Files identical despite different names*

### Comparing `autokattis-1.4.4/autokattis/scraper/country.py` & `autokattis-1.4.5/autokattis/scraper/country.py`

 * *Files identical despite different names*

### Comparing `autokattis-1.4.4/autokattis/scraper/university.py` & `autokattis-1.4.5/autokattis/scraper/university.py`

 * *Files identical despite different names*

### Comparing `autokattis-1.4.4/autokattis/utils/__init__.py` & `autokattis-1.4.5/autokattis/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `autokattis-1.4.4/autokattis.egg-info/PKG-INFO` & `autokattis-1.4.5/autokattis.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autokattis
-Version: 1.4.4
+Version: 1.4.5
 Summary: Updated Kattis API wrapper
 Home-page: https://github.com/RussellDash332/autokattis
 Download-URL: https://pypi.org/project/autokattis/
 Author: Russell Saerang
 Author-email: russellsaerang@gmail.com
 License: MIT
 Keywords: Kattis
```

### Comparing `autokattis-1.4.4/setup.py` & `autokattis-1.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name='autokattis',
-    version='1.4.4',
+    version='1.4.5',
     description='Updated Kattis API wrapper',
     long_description_content_type="text/markdown",
     long_description=README,
     license='MIT',
     packages=find_packages(),
     author='Russell Saerang',
     author_email='russellsaerang@gmail.com',
```

