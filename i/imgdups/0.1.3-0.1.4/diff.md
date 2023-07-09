# Comparing `tmp/imgdups-0.1.3.tar.gz` & `tmp/imgdups-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imgdups-0.1.3.tar", last modified: Sun Jul  9 16:52:48 2023, max compression
+gzip compressed data, was "imgdups-0.1.4.tar", last modified: Sun Jul  9 21:13:43 2023, max compression
```

## Comparing `imgdups-0.1.3.tar` & `imgdups-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 nice      (1000) nice      (1000)        0 2023-07-09 16:52:48.893410 imgdups-0.1.3/
--rw-rw-r--   0 nice      (1000) nice      (1000)    35149 2023-07-03 20:54:00.000000 imgdups-0.1.3/LICENSE
--rw-rw-r--   0 nice      (1000) nice      (1000)     2484 2023-07-09 16:52:48.893410 imgdups-0.1.3/PKG-INFO
--rw-r--r--   0 nice      (1000) nice      (1000)     1508 2023-07-04 17:37:18.000000 imgdups-0.1.3/README.md
-drwxrwxr-x   0 nice      (1000) nice      (1000)        0 2023-07-09 16:52:48.889410 imgdups-0.1.3/imgdups/
--rw-rw-r--   0 nice      (1000) nice      (1000)      114 2023-07-04 16:54:42.000000 imgdups-0.1.3/imgdups/__init__.py
--rwxrwxr-x   0 nice      (1000) nice      (1000)    11242 2023-07-09 16:49:59.000000 imgdups-0.1.3/imgdups/imgdups.py
-drwxrwxr-x   0 nice      (1000) nice      (1000)        0 2023-07-09 16:52:48.893410 imgdups-0.1.3/imgdups.egg-info/
--rw-rw-r--   0 nice      (1000) nice      (1000)     2484 2023-07-09 16:52:48.000000 imgdups-0.1.3/imgdups.egg-info/PKG-INFO
--rw-rw-r--   0 nice      (1000) nice      (1000)      316 2023-07-09 16:52:48.000000 imgdups-0.1.3/imgdups.egg-info/SOURCES.txt
--rw-rw-r--   0 nice      (1000) nice      (1000)        1 2023-07-09 16:52:48.000000 imgdups-0.1.3/imgdups.egg-info/dependency_links.txt
--rw-rw-r--   0 nice      (1000) nice      (1000)       49 2023-07-09 16:52:48.000000 imgdups-0.1.3/imgdups.egg-info/entry_points.txt
--rw-rw-r--   0 nice      (1000) nice      (1000)       20 2023-07-09 16:52:48.000000 imgdups-0.1.3/imgdups.egg-info/requires.txt
--rw-rw-r--   0 nice      (1000) nice      (1000)        8 2023-07-09 16:52:48.000000 imgdups-0.1.3/imgdups.egg-info/top_level.txt
--rw-rw-r--   0 nice      (1000) nice      (1000)        1 2023-07-04 16:37:56.000000 imgdups-0.1.3/imgdups.egg-info/zip-safe
--rw-rw-r--   0 nice      (1000) nice      (1000)       82 2023-07-03 21:28:15.000000 imgdups-0.1.3/pyproject.toml
--rw-rw-r--   0 nice      (1000) nice      (1000)       38 2023-07-09 16:52:48.893410 imgdups-0.1.3/setup.cfg
--rw-rw-r--   0 nice      (1000) nice      (1000)     1613 2023-07-09 16:52:12.000000 imgdups-0.1.3/setup.py
-drwxrwxr-x   0 nice      (1000) nice      (1000)        0 2023-07-09 16:52:48.893410 imgdups-0.1.3/tests/
--rw-rw-r--   0 nice      (1000) nice      (1000)      166 2023-07-04 17:05:07.000000 imgdups-0.1.3/tests/test_imgdups.py
+drwxrwxr-x   0 nice      (1000) nice      (1000)        0 2023-07-09 21:13:43.044994 imgdups-0.1.4/
+-rw-rw-r--   0 nice      (1000) nice      (1000)    35149 2023-07-03 20:54:00.000000 imgdups-0.1.4/LICENSE
+-rw-rw-r--   0 nice      (1000) nice      (1000)     2484 2023-07-09 21:13:43.044994 imgdups-0.1.4/PKG-INFO
+-rw-r--r--   0 nice      (1000) nice      (1000)     1508 2023-07-04 17:37:18.000000 imgdups-0.1.4/README.md
+drwxrwxr-x   0 nice      (1000) nice      (1000)        0 2023-07-09 21:13:43.040994 imgdups-0.1.4/imgdups/
+-rw-rw-r--   0 nice      (1000) nice      (1000)      114 2023-07-04 16:54:42.000000 imgdups-0.1.4/imgdups/__init__.py
+-rwxrwxr-x   0 nice      (1000) nice      (1000)    11418 2023-07-09 20:37:54.000000 imgdups-0.1.4/imgdups/imgdups.py
+drwxrwxr-x   0 nice      (1000) nice      (1000)        0 2023-07-09 21:13:43.040994 imgdups-0.1.4/imgdups.egg-info/
+-rw-rw-r--   0 nice      (1000) nice      (1000)     2484 2023-07-09 21:13:43.000000 imgdups-0.1.4/imgdups.egg-info/PKG-INFO
+-rw-rw-r--   0 nice      (1000) nice      (1000)      316 2023-07-09 21:13:43.000000 imgdups-0.1.4/imgdups.egg-info/SOURCES.txt
+-rw-rw-r--   0 nice      (1000) nice      (1000)        1 2023-07-09 21:13:43.000000 imgdups-0.1.4/imgdups.egg-info/dependency_links.txt
+-rw-rw-r--   0 nice      (1000) nice      (1000)       49 2023-07-09 21:13:43.000000 imgdups-0.1.4/imgdups.egg-info/entry_points.txt
+-rw-rw-r--   0 nice      (1000) nice      (1000)       20 2023-07-09 21:13:43.000000 imgdups-0.1.4/imgdups.egg-info/requires.txt
+-rw-rw-r--   0 nice      (1000) nice      (1000)        8 2023-07-09 21:13:43.000000 imgdups-0.1.4/imgdups.egg-info/top_level.txt
+-rw-rw-r--   0 nice      (1000) nice      (1000)        1 2023-07-04 16:37:56.000000 imgdups-0.1.4/imgdups.egg-info/zip-safe
+-rw-rw-r--   0 nice      (1000) nice      (1000)       82 2023-07-03 21:28:15.000000 imgdups-0.1.4/pyproject.toml
+-rw-rw-r--   0 nice      (1000) nice      (1000)       38 2023-07-09 21:13:43.044994 imgdups-0.1.4/setup.cfg
+-rw-rw-r--   0 nice      (1000) nice      (1000)     1613 2023-07-09 20:21:25.000000 imgdups-0.1.4/setup.py
+drwxrwxr-x   0 nice      (1000) nice      (1000)        0 2023-07-09 21:13:43.044994 imgdups-0.1.4/tests/
+-rw-rw-r--   0 nice      (1000) nice      (1000)      166 2023-07-04 17:05:07.000000 imgdups-0.1.4/tests/test_imgdups.py
```

### Comparing `imgdups-0.1.3/LICENSE` & `imgdups-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `imgdups-0.1.3/PKG-INFO` & `imgdups-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imgdups
-Version: 0.1.3
+Version: 0.1.4
 Summary: Very fast two folder image duplicate finder programmed with pickle and cv2
 Home-page: https://github.com/ChuckNorrison/imgdups/
 Author: Chuck Norrison
 Author-email: itsmells@yourshorts.club
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `imgdups-0.1.3/README.md` & `imgdups-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `imgdups-0.1.3/imgdups/imgdups.py` & `imgdups-0.1.4/imgdups/imgdups.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,32 +99,33 @@
         check = True
 
     return check
 
 def main():
     """Start standalone with config file or arguments"""
     parser = ArgumentParser()
-    parser.add_argument("--search", dest="search_path", required=True,
+    parser.add_argument("-s", "--search", dest="search_path", required=True,
                         help="path to images folder for duplicate candidates", metavar="PATH")
-    parser.add_argument("--target", dest="target_path", required=True,
+    parser.add_argument("-t", "--target", dest="target_path", required=True,
                         help="path to images folder to check for duplicates", metavar="PATH")
-    parser.add_argument("--score", dest="match_score",
-                        help="score for matching images as duplicates", metavar="PATH")
+    parser.add_argument("-m", "--match", dest="match_score",
+                        help="min match result score to return image as duplicate", metavar="INT")
 
     # parse args and ignore unknown args
     args, _unknown = parser.parse_known_args()
 
+    # use argument -m or set default score
+    match = 320
     if args.match_score.isdigit():
-        score = args.match_score
-    else:
-        # default score
-        score = 320
+        # test for maximum possible match score
+        if int(args.match_score) <= 500:
+            match = int(args.match_score)
 
     img_dups = ImgDups(args.target_path, args.search_path)
-    img_dups.find_duplicates(score)
+    img_dups.find_duplicates(match)
 
 class ImgDups():
     """
     Class to find image duplicates
     in target path from a search path
     """
     def __init__(self, target, search):
@@ -239,15 +240,15 @@
             # clean up
             os.remove(file_path)
 
         with open(file_path, 'wb') as cache_file:
             # write duplicates checked to cache file for next run
             pickle.dump((self.search_processed, self.search_cache), cache_file)
 
-    def find_duplicates(self, score = 320):
+    def find_duplicates(self, match = 320):
         """ Start the script """
         logger.info("Start script")
 
         garbage = 0
 
         if not os.path.exists(self.target):
             logger.error("Target path does not exist (%s)", self.target)
@@ -281,17 +282,19 @@
                 target_filename = os.path.basename(target_filepath)
 
                 if check_garbage(target_filepath):
                     garbage += 1
                     continue
 
                 bf_match = cv2.BFMatcher(cv2.NORM_HAMMING, crossCheck=True)
+
+                # calculate match score
                 match_score = bf_match.match(search_descriptors, target_descriptors)
 
-                if len(match_score) > score:
+                if len(match_score) > match:
                     logger.info("%s == %s (score: %d)",
                             filename,
                             target_filename,
                             len(match_score))
 
                     self.duplicates.append({
                         "search": filename,
```

### Comparing `imgdups-0.1.3/imgdups.egg-info/PKG-INFO` & `imgdups-0.1.4/imgdups.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imgdups
-Version: 0.1.3
+Version: 0.1.4
 Summary: Very fast two folder image duplicate finder programmed with pickle and cv2
 Home-page: https://github.com/ChuckNorrison/imgdups/
 Author: Chuck Norrison
 Author-email: itsmells@yourshorts.club
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `imgdups-0.1.3/setup.py` & `imgdups-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 test_requirements = [
     'pylint',
     'pytest',
 ]
 
 setup(
     name='imgdups',
-    version='0.1.3',
+    version='0.1.4',
     description="Very fast two folder image duplicate finder programmed with pickle and cv2",
     long_description=readme,
     long_description_content_type = 'text/markdown',
     author="Chuck Norrison",
     author_email='itsmells@yourshorts.club',
     url='https://github.com/ChuckNorrison/imgdups/',
     packages=['imgdups'],
```

