# Comparing `tmp/tgeraser-1.1.1.tar.gz` & `tmp/tgeraser-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tgeraser-1.1.1.tar", last modified: Tue Sep  7 14:09:45 2021, max compression
+gzip compressed data, was "tgeraser-1.1.2.tar", last modified: Sun Jul  9 21:58:08 2023, max compression
```

## Comparing `tgeraser-1.1.1.tar` & `tgeraser-1.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-07 14:09:45.000000 tgeraser-1.1.1/
--rw-r--r--   0 root         (0) root         (0)     1074 2021-09-07 14:09:42.000000 tgeraser-1.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2900 2021-09-07 14:09:45.000000 tgeraser-1.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2248 2021-09-07 14:09:42.000000 tgeraser-1.1.1/README.md
--rw-r--r--   0 root         (0) root         (0)       89 2021-09-07 14:09:42.000000 tgeraser-1.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1006 2021-09-07 14:09:45.000000 tgeraser-1.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       72 2021-09-07 14:09:42.000000 tgeraser-1.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-07 14:09:45.000000 tgeraser-1.1.1/tgeraser/
--rw-r--r--   0 root         (0) root         (0)       73 2021-09-07 14:09:42.000000 tgeraser-1.1.1/tgeraser/__init__.py
--rw-r--r--   0 root         (0) root         (0)      105 2021-09-07 14:09:42.000000 tgeraser-1.1.1/tgeraser/__main__.py
--rw-r--r--   0 root         (0) root         (0)       40 2021-09-07 14:09:43.000000 tgeraser-1.1.1/tgeraser/__version__.py
--rw-r--r--   0 root         (0) root         (0)     4118 2021-09-07 14:09:42.000000 tgeraser-1.1.1/tgeraser/core.py
--rw-r--r--   0 root         (0) root         (0)     8196 2021-09-07 14:09:42.000000 tgeraser-1.1.1/tgeraser/eraser.py
--rw-r--r--   0 root         (0) root         (0)       73 2021-09-07 14:09:42.000000 tgeraser-1.1.1/tgeraser/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     8464 2021-09-07 14:09:42.000000 tgeraser-1.1.1/tgeraser/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-07 14:09:45.000000 tgeraser-1.1.1/tgeraser.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2900 2021-09-07 14:09:45.000000 tgeraser-1.1.1/tgeraser.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      419 2021-09-07 14:09:45.000000 tgeraser-1.1.1/tgeraser.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-09-07 14:09:45.000000 tgeraser-1.1.1/tgeraser.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2021-09-07 14:09:45.000000 tgeraser-1.1.1/tgeraser.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-09-07 14:09:45.000000 tgeraser-1.1.1/tgeraser.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       48 2021-09-07 14:09:45.000000 tgeraser-1.1.1/tgeraser.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2021-09-07 14:09:45.000000 tgeraser-1.1.1/tgeraser.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 21:58:08.005864 tgeraser-1.1.2/
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-07-09 21:58:05.000000 tgeraser-1.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2880 2023-07-09 21:58:08.005864 tgeraser-1.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2248 2023-07-09 21:58:05.000000 tgeraser-1.1.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       89 2023-07-09 21:58:05.000000 tgeraser-1.1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-09 21:58:08.005864 tgeraser-1.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       72 2023-07-09 21:58:05.000000 tgeraser-1.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 21:58:08.001864 tgeraser-1.1.2/tgeraser/
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-09 21:58:05.000000 tgeraser-1.1.2/tgeraser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      105 2023-07-09 21:58:05.000000 tgeraser-1.1.2/tgeraser/__main__.py
+-rw-r--r--   0 root         (0) root         (0)       40 2023-07-09 21:58:05.000000 tgeraser-1.1.2/tgeraser/__version__.py
+-rw-r--r--   0 root         (0) root         (0)     4118 2023-07-09 21:58:05.000000 tgeraser-1.1.2/tgeraser/core.py
+-rw-r--r--   0 root         (0) root         (0)     8196 2023-07-09 21:58:05.000000 tgeraser-1.1.2/tgeraser/eraser.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-09 21:58:05.000000 tgeraser-1.1.2/tgeraser/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     8464 2023-07-09 21:58:05.000000 tgeraser-1.1.2/tgeraser/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 21:58:08.005864 tgeraser-1.1.2/tgeraser.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2880 2023-07-09 21:58:07.000000 tgeraser-1.1.2/tgeraser.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      419 2023-07-09 21:58:07.000000 tgeraser-1.1.2/tgeraser.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 21:58:07.000000 tgeraser-1.1.2/tgeraser.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-07-09 21:58:07.000000 tgeraser-1.1.2/tgeraser.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 21:58:07.000000 tgeraser-1.1.2/tgeraser.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       48 2023-07-09 21:58:07.000000 tgeraser-1.1.2/tgeraser.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-09 21:58:07.000000 tgeraser-1.1.2/tgeraser.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tgeraser-1.1.1/LICENSE` & `tgeraser-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tgeraser-1.1.1/PKG-INFO` & `tgeraser-1.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: tgeraser
-Version: 1.1.1
+Version: 1.1.2
 Summary: Tool deletes all your messages from chat/channel/dialog on Telegram
 Home-page: https://github.com/en9inerd/tgeraser
 Author: Vladimir Loskutov
 Author-email: vladimir@enginerd.io
 License: MIT License
 Keywords: telegram,api,delete messages
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
@@ -57,9 +56,7 @@
     -l --limit NUM              Show specified number of recent chats.
     -t --time-period STRING     Specify period for infinite loop to run messages deletion every X seconds/minutes/hours/days/weeks.
                                 Example: --time-period "3*days" OR --time-period "5*seconds"
     -k --kill                   Kill existing background tgeraser processes (only for Unix-like OS).
     -h --help                   Show this screen.
     --version                   Show version.
 ```
-
-
```

### Comparing `tgeraser-1.1.1/README.md` & `tgeraser-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `tgeraser-1.1.1/setup.cfg` & `tgeraser-1.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `tgeraser-1.1.1/tgeraser/core.py` & `tgeraser-1.1.2/tgeraser/core.py`

 * *Files identical despite different names*

### Comparing `tgeraser-1.1.1/tgeraser/eraser.py` & `tgeraser-1.1.2/tgeraser/eraser.py`

 * *Files identical despite different names*

### Comparing `tgeraser-1.1.1/tgeraser/utils.py` & `tgeraser-1.1.2/tgeraser/utils.py`

 * *Files identical despite different names*

### Comparing `tgeraser-1.1.1/tgeraser.egg-info/PKG-INFO` & `tgeraser-1.1.2/tgeraser.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: tgeraser
-Version: 1.1.1
+Version: 1.1.2
 Summary: Tool deletes all your messages from chat/channel/dialog on Telegram
 Home-page: https://github.com/en9inerd/tgeraser
 Author: Vladimir Loskutov
 Author-email: vladimir@enginerd.io
 License: MIT License
 Keywords: telegram,api,delete messages
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
@@ -57,9 +56,7 @@
     -l --limit NUM              Show specified number of recent chats.
     -t --time-period STRING     Specify period for infinite loop to run messages deletion every X seconds/minutes/hours/days/weeks.
                                 Example: --time-period "3*days" OR --time-period "5*seconds"
     -k --kill                   Kill existing background tgeraser processes (only for Unix-like OS).
     -h --help                   Show this screen.
     --version                   Show version.
 ```
-
-
```

