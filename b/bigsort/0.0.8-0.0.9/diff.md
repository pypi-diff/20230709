# Comparing `tmp/bigsort-0.0.8.tar.gz` & `tmp/bigsort-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigsort-0.0.8.tar", last modified: Wed May 24 14:00:55 2023, max compression
+gzip compressed data, was "bigsort-0.0.9.tar", last modified: Sun Jul  9 16:52:02 2023, max compression
```

## Comparing `bigsort-0.0.8.tar` & `bigsort-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 14:00:55.095916 bigsort-0.0.8/
--rw-rw-rw-   0        0        0     1359 2023-05-24 14:00:55.094916 bigsort-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-24 14:00:55.093917 bigsort-0.0.8/bigsort.egg-info/
--rw-rw-rw-   0        0        0     1359 2023-05-24 14:00:54.000000 bigsort-0.0.8/bigsort.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-05-24 14:00:54.000000 bigsort-0.0.8/bigsort.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 14:00:54.000000 bigsort-0.0.8/bigsort.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-05-24 14:00:54.000000 bigsort-0.0.8/bigsort.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-05-24 14:00:54.000000 bigsort-0.0.8/bigsort.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-24 14:00:54.000000 bigsort-0.0.8/bigsort.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10658 2023-05-24 13:37:18.000000 bigsort-0.0.8/bigsort.py
--rw-rw-rw-   0        0        0       42 2023-05-24 14:00:55.095916 bigsort-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      993 2023-05-24 13:46:49.000000 bigsort-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 16:52:02.044140 bigsort-0.0.9/
+-rw-rw-rw-   0        0        0     1359 2023-07-09 16:52:02.043137 bigsort-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-09 16:52:02.041137 bigsort-0.0.9/bigsort.egg-info/
+-rw-rw-rw-   0        0        0     1359 2023-07-09 16:52:01.000000 bigsort-0.0.9/bigsort.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2023-07-09 16:52:01.000000 bigsort-0.0.9/bigsort.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 16:52:01.000000 bigsort-0.0.9/bigsort.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-09 16:52:01.000000 bigsort-0.0.9/bigsort.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-07-09 16:52:01.000000 bigsort-0.0.9/bigsort.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-09 16:52:01.000000 bigsort-0.0.9/bigsort.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10658 2023-07-09 16:50:40.000000 bigsort-0.0.9/bigsort.py
+-rw-rw-rw-   0        0        0       42 2023-07-09 16:52:02.044140 bigsort-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      993 2023-07-09 16:51:26.000000 bigsort-0.0.9/setup.py
```

### Comparing `bigsort-0.0.8/PKG-INFO` & `bigsort-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigsort
-Version: 0.0.8
+Version: 0.0.9
 Summary: sort big file or streams
 Home-page: https://github.com/laohur/bigsort
 Author: laohur
 Author-email: laohur@gmail.com
 License: [Anti-996 License](https: // github.com/996icu/996.ICU/blob/master/LICENSE)
 Keywords: bigsort,sort,external sort,big file sort
 Requires-Python: >=3.0
```

### Comparing `bigsort-0.0.8/bigsort.egg-info/PKG-INFO` & `bigsort-0.0.9/bigsort.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigsort
-Version: 0.0.8
+Version: 0.0.9
 Summary: sort big file or streams
 Home-page: https://github.com/laohur/bigsort
 Author: laohur
 Author-email: laohur@gmail.com
 License: [Anti-996 License](https: // github.com/996icu/996.ICU/blob/master/LICENSE)
 Keywords: bigsort,sort,external sort,big file sort
 Requires-Python: >=3.0
```

### Comparing `bigsort-0.0.8/bigsort.py` & `bigsort-0.0.9/bigsort.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,16 +235,16 @@
     return True
 
 
 def main():
     parser = argparse.ArgumentParser()
     # parser.add_argument("src") # sys.stdin
     # parser.add_argument("tgt") # sys.stdout
-    parser.add_argument("-i", "--input", default="readme.md")
-    # parser.add_argument("-i", "--input", default=None)
+    # parser.add_argument("-i", "--input", default="readme.md")
+    parser.add_argument("-i", "--input", default=None)
     parser.add_argument("-o", "--output", default=None)
     parser.add_argument("--buffering", type=int, default=1024*1024)
     parser.add_argument("--nSplit", type=int, default=10)  # bigger if skew or shuffle
     parser.add_argument("--nLine", type=int, default=100000)
     parser.add_argument("-M", "--budget", type=float, default=0.4)  # 0.8 memary budget in ratio if single pipe
     parser.add_argument("-u", "--unique", default=False)  # remove repeat neighbor; only when sort
     parser.add_argument("-s", "--sortType", default="i")  # one of  'i/d/R': increase descend random
```

### Comparing `bigsort-0.0.8/setup.py` & `bigsort-0.0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     long_description = f.read()
 
 
 setup(
     name="bigsort",
     # packages=find_packages(),
     py_modules=['bigsort'],
-    version='0.0.8',
+    version='0.0.9',
     description='sort big file or streams',
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires='>=3.0',
     install_requires=[
         "psutil",
         "logzero"
```

