# Comparing `tmp/jirawiki2docx-1.0.0.tar.gz` & `tmp/jirawiki2docx-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/ifeoluwa/Documents/JiraWiki2Docx Project/dist/.tmp-s9qgx0w1/jirawiki2docx-1.0.0.tar", last modified: Sun Jul  9 13:50:11 2023, max compression
+gzip compressed data, was "/Users/ifeoluwa/Documents/JiraWiki2Docx Project/dist/.tmp-ktz28zil/jirawiki2docx-1.0.1.tar", last modified: Sun Jul  9 14:08:37 2023, max compression
```

## Comparing `jirawiki2docx-1.0.0.tar` & `jirawiki2docx-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ifeoluwa   (503) staff       (20)        0 2023-07-09 13:50:11.000000 jirawiki2docx-1.0.0/
--rw-r--r--   0 ifeoluwa   (503) staff       (20)     1073 2023-06-30 14:40:10.000000 jirawiki2docx-1.0.0/LICENSE
--rw-r--r--   0 ifeoluwa   (503) staff       (20)     3589 2023-07-09 13:50:11.000000 jirawiki2docx-1.0.0/PKG-INFO
--rw-r--r--   0 ifeoluwa   (503) staff       (20)     2864 2023-07-05 09:11:54.000000 jirawiki2docx-1.0.0/README.md
-drwxr-xr-x   0 ifeoluwa   (503) staff       (20)        0 2023-07-09 13:50:11.000000 jirawiki2docx-1.0.0/jirawiki2docx/
--rw-r--r--   0 ifeoluwa   (503) staff       (20)       40 2023-07-01 20:05:54.000000 jirawiki2docx-1.0.0/jirawiki2docx/__init__.py
--rw-r--r--   0 ifeoluwa   (503) staff       (20)    12504 2023-07-04 15:55:53.000000 jirawiki2docx-1.0.0/jirawiki2docx/jirawiki2docx.py
-drwxr-xr-x   0 ifeoluwa   (503) staff       (20)        0 2023-07-09 13:50:11.000000 jirawiki2docx-1.0.0/jirawiki2docx.egg-info/
--rw-r--r--   0 ifeoluwa   (503) staff       (20)     3589 2023-07-09 13:50:11.000000 jirawiki2docx-1.0.0/jirawiki2docx.egg-info/PKG-INFO
--rw-r--r--   0 ifeoluwa   (503) staff       (20)      283 2023-07-09 13:50:11.000000 jirawiki2docx-1.0.0/jirawiki2docx.egg-info/SOURCES.txt
--rw-r--r--   0 ifeoluwa   (503) staff       (20)        1 2023-07-09 13:50:11.000000 jirawiki2docx-1.0.0/jirawiki2docx.egg-info/dependency_links.txt
--rw-r--r--   0 ifeoluwa   (503) staff       (20)       36 2023-07-09 13:50:11.000000 jirawiki2docx-1.0.0/jirawiki2docx.egg-info/requires.txt
--rw-r--r--   0 ifeoluwa   (503) staff       (20)       14 2023-07-09 13:50:11.000000 jirawiki2docx-1.0.0/jirawiki2docx.egg-info/top_level.txt
--rw-r--r--   0 ifeoluwa   (503) staff       (20)       86 2023-07-02 22:27:47.000000 jirawiki2docx-1.0.0/pyproject.toml
--rw-r--r--   0 ifeoluwa   (503) staff       (20)      804 2023-07-09 13:50:11.000000 jirawiki2docx-1.0.0/setup.cfg
+drwxr-xr-x   0 ifeoluwa   (503) staff       (20)        0 2023-07-09 14:08:37.000000 jirawiki2docx-1.0.1/
+-rw-r--r--   0 ifeoluwa   (503) staff       (20)     1073 2023-06-30 14:40:10.000000 jirawiki2docx-1.0.1/LICENSE
+-rw-r--r--   0 ifeoluwa   (503) staff       (20)     3601 2023-07-09 14:08:37.000000 jirawiki2docx-1.0.1/PKG-INFO
+-rw-r--r--   0 ifeoluwa   (503) staff       (20)     2864 2023-07-05 09:11:54.000000 jirawiki2docx-1.0.1/README.md
+drwxr-xr-x   0 ifeoluwa   (503) staff       (20)        0 2023-07-09 14:08:37.000000 jirawiki2docx-1.0.1/jirawiki2docx/
+-rw-r--r--   0 ifeoluwa   (503) staff       (20)       40 2023-07-01 20:05:54.000000 jirawiki2docx-1.0.1/jirawiki2docx/__init__.py
+-rw-r--r--   0 ifeoluwa   (503) staff       (20)    12504 2023-07-04 15:55:53.000000 jirawiki2docx-1.0.1/jirawiki2docx/jirawiki2docx.py
+drwxr-xr-x   0 ifeoluwa   (503) staff       (20)        0 2023-07-09 14:08:37.000000 jirawiki2docx-1.0.1/jirawiki2docx.egg-info/
+-rw-r--r--   0 ifeoluwa   (503) staff       (20)     3601 2023-07-09 14:08:37.000000 jirawiki2docx-1.0.1/jirawiki2docx.egg-info/PKG-INFO
+-rw-r--r--   0 ifeoluwa   (503) staff       (20)      283 2023-07-09 14:08:37.000000 jirawiki2docx-1.0.1/jirawiki2docx.egg-info/SOURCES.txt
+-rw-r--r--   0 ifeoluwa   (503) staff       (20)        1 2023-07-09 14:08:37.000000 jirawiki2docx-1.0.1/jirawiki2docx.egg-info/dependency_links.txt
+-rw-r--r--   0 ifeoluwa   (503) staff       (20)       36 2023-07-09 14:08:37.000000 jirawiki2docx-1.0.1/jirawiki2docx.egg-info/requires.txt
+-rw-r--r--   0 ifeoluwa   (503) staff       (20)       14 2023-07-09 14:08:37.000000 jirawiki2docx-1.0.1/jirawiki2docx.egg-info/top_level.txt
+-rw-r--r--   0 ifeoluwa   (503) staff       (20)       86 2023-07-02 22:27:47.000000 jirawiki2docx-1.0.1/pyproject.toml
+-rw-r--r--   0 ifeoluwa   (503) staff       (20)      816 2023-07-09 14:08:37.000000 jirawiki2docx-1.0.1/setup.cfg
```

### Comparing `jirawiki2docx-1.0.0/LICENSE` & `jirawiki2docx-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jirawiki2docx-1.0.0/PKG-INFO` & `jirawiki2docx-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: jirawiki2docx
-Version: 1.0.0
+Version: 1.0.1
 Summary: Convert Jira wiki to DOCX format effectively
 Home-page: https://github.com/deitar/jirawiki2docx
 Author: Ifeoluwa Akande
 Author-email: 
 Project-URL: Bug Tracker, https://github.com/deitar/jirawiki2docx/issues
 Project-URL: repository, https://github.com/deitar/jirawiki2docx
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Office/Business :: Office Suites
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `jirawiki2docx-1.0.0/README.md` & `jirawiki2docx-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `jirawiki2docx-1.0.0/jirawiki2docx/jirawiki2docx.py` & `jirawiki2docx-1.0.1/jirawiki2docx/jirawiki2docx.py`

 * *Files identical despite different names*

### Comparing `jirawiki2docx-1.0.0/jirawiki2docx.egg-info/PKG-INFO` & `jirawiki2docx-1.0.1/jirawiki2docx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: jirawiki2docx
-Version: 1.0.0
+Version: 1.0.1
 Summary: Convert Jira wiki to DOCX format effectively
 Home-page: https://github.com/deitar/jirawiki2docx
 Author: Ifeoluwa Akande
 Author-email: 
 Project-URL: Bug Tracker, https://github.com/deitar/jirawiki2docx/issues
 Project-URL: repository, https://github.com/deitar/jirawiki2docx
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Office/Business :: Office Suites
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `jirawiki2docx-1.0.0/setup.cfg` & `jirawiki2docx-1.0.1/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [metadata]
 name = jirawiki2docx
-version = 1.0.0
+version = 1.0.1
 author = Ifeoluwa Akande
 author_email = 
 description = Convert Jira wiki to DOCX format effectively
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/deitar/jirawiki2docx
 project_urls = 
 	Bug Tracker = https://github.com/deitar/jirawiki2docx/issues
 	repository = https://github.com/deitar/jirawiki2docx
 classifiers = 
-	Development Status :: 3 - Alpha
+	Development Status :: 5 - Production/Stable
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Topic :: Office/Business :: Office Suites
 	Topic :: Software Development :: Libraries
 
 [options]
```

