# Comparing `tmp/smartscoutscrape-0.2.0.tar.gz` & `tmp/smartscoutscrape-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartscoutscrape-0.2.0.tar", max compression
+gzip compressed data, was "smartscoutscrape-0.2.1.tar", max compression
```

## Comparing `smartscoutscrape-0.2.0.tar` & `smartscoutscrape-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    10912 2023-06-21 00:43:17.419814 smartscoutscrape-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0    15504 2023-07-09 03:55:21.817334 smartscoutscrape-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4173 2023-07-01 17:10:53.999740 smartscoutscrape-0.2.0/README.md
--rw-r--r--   0        0        0     2331 2023-07-09 03:29:25.504056 smartscoutscrape-0.2.0/smartscoutscrape/__init__.py
--rw-r--r--   0        0        0     7509 2023-07-08 23:43:27.927487 smartscoutscrape-0.2.0/smartscoutscrape/amazon.py
--rw-r--r--   0        0        0     6318 2023-07-09 02:15:49.073930 smartscoutscrape-0.2.0/smartscoutscrape/cli.py
--rw-r--r--   0        0        0     6638 2023-07-09 03:51:24.420503 smartscoutscrape-0.2.0/smartscoutscrape/pandas.py
--rw-r--r--   0        0        0    14978 2023-07-09 02:49:29.826968 smartscoutscrape-0.2.0/smartscoutscrape/smartscout.py
--rw-r--r--   0        0        0    28096 2023-07-09 03:26:04.334379 smartscoutscrape-0.2.0/smartscoutscrape/sqlite.py
--rw-r--r--   0        0        0     1892 2023-07-01 16:44:40.327989 smartscoutscrape-0.2.0/smartscoutscrape/utils.py
--rw-r--r--   0        0        0     5914 1970-01-01 00:00:00.000000 smartscoutscrape-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    10912 2023-06-21 00:43:17.419814 smartscoutscrape-0.2.1/LICENSE.txt
+-rw-r--r--   0        0        0    15504 2023-07-09 04:19:19.557822 smartscoutscrape-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4173 2023-07-01 17:10:53.999740 smartscoutscrape-0.2.1/README.md
+-rw-r--r--   0        0        0     2331 2023-07-09 04:19:56.453799 smartscoutscrape-0.2.1/smartscoutscrape/__init__.py
+-rw-r--r--   0        0        0     7509 2023-07-08 23:43:27.927487 smartscoutscrape-0.2.1/smartscoutscrape/amazon.py
+-rw-r--r--   0        0        0     6422 2023-07-09 04:02:30.777241 smartscoutscrape-0.2.1/smartscoutscrape/cli.py
+-rw-r--r--   0        0        0     6638 2023-07-09 03:51:24.420503 smartscoutscrape-0.2.1/smartscoutscrape/pandas.py
+-rw-r--r--   0        0        0    14978 2023-07-09 02:49:29.826968 smartscoutscrape-0.2.1/smartscoutscrape/smartscout.py
+-rw-r--r--   0        0        0    28077 2023-07-09 04:00:55.354207 smartscoutscrape-0.2.1/smartscoutscrape/sqlite.py
+-rw-r--r--   0        0        0     1892 2023-07-01 16:44:40.327989 smartscoutscrape-0.2.1/smartscoutscrape/utils.py
+-rw-r--r--   0        0        0     5914 1970-01-01 00:00:00.000000 smartscoutscrape-0.2.1/PKG-INFO
```

### Comparing `smartscoutscrape-0.2.0/LICENSE.txt` & `smartscoutscrape-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smartscoutscrape-0.2.0/pyproject.toml` & `smartscoutscrape-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 # This is the version of your project. Keep it up-to-date and follow semantic versioning.
 # It's used in the PyPi, wheels, Docker, and GitHub packages.
 # Also make sure to use exactly this version when creating a GitHub release,
 # but prefix a "v" to the GitHub release.
 # E.g. This might be "1.2.13", and the GitHub release will be "v1.2.13".
 # Although semantic versioning allows for build tags (metadata),
 # not all tools are compatible with it, so avoid it if you can.
-version = "0.2.0"
+version = "0.2.1"
 
 # TODO: Set the description and keywords here
 description = "Lightweight data-extraction & general use library for smartscout.com"
 keywords = ["scraper", "data science", "requests", "python", "data"]
 authors = ["Parker Wahle <regulad@regulad.xyz>"]
 maintainers = ["Parker Wahle <regulad@regulad.xyz>"]
 # This must be an identifier listed in https://spdx.org/licenses/
```

### Comparing `smartscoutscrape-0.2.0/README.md` & `smartscoutscrape-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `smartscoutscrape-0.2.0/smartscoutscrape/__init__.py` & `smartscoutscrape-0.2.1/smartscoutscrape/__init__.py`

 * *Files identical despite different names*

### Comparing `smartscoutscrape-0.2.0/smartscoutscrape/amazon.py` & `smartscoutscrape-0.2.1/smartscoutscrape/amazon.py`

 * *Files identical despite different names*

### Comparing `smartscoutscrape-0.2.0/smartscoutscrape/cli.py` & `smartscoutscrape-0.2.1/smartscoutscrape/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,15 +156,17 @@
             smartscout_session=smartscout_session
         ) as helper:
             progress.remove_task(setup_task)
             # Download all products
             download_task = progress.add_task("Downloading products...", total=None, start=False)
             progress.update(download_task, total=smartscout_session.get_total_number_of_products())
             try:
-                for _ in helper.dump_all(yield_rows=True, dump_default=dump, dump_html=dump_html, extend=extend, images=images):
+                for i, _ in enumerate(helper.dump_all(yield_rows=True, dump_default=dump, dump_html=dump_html, extend=extend, images=images)):
+                    if i == 0:
+                        progress.start_task(download_task)
                     progress.advance(download_task)
             finally:
                 if log_level_debug_or_higher:
                     pr.create_stats()
                     stats = pstats.Stats(pr)
                     stats.sort_stats(pstats.SortKey.CUMULATIVE)
                     stats.print_stats(.05)
```

### Comparing `smartscoutscrape-0.2.0/smartscoutscrape/pandas.py` & `smartscoutscrape-0.2.1/smartscoutscrape/pandas.py`

 * *Files identical despite different names*

### Comparing `smartscoutscrape-0.2.0/smartscoutscrape/smartscout.py` & `smartscoutscrape-0.2.1/smartscoutscrape/smartscout.py`

 * *Files identical despite different names*

### Comparing `smartscoutscrape-0.2.0/smartscoutscrape/sqlite.py` & `smartscoutscrape-0.2.1/smartscoutscrape/sqlite.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import warnings
 import zlib
 from concurrent.futures import CancelledError, ThreadPoolExecutor, as_completed
 from queue import Empty, Queue
 from sqlite3 import Connection
 from threading import Event, Lock, Thread
-from typing import Generator, Literal, Self, overload
+from typing import Generator, Self
 
 import minify_html
 from requests import HTTPError
 
 from .amazon import AmazonBaseSession
 from .smartscout import SmartScoutSession
 from .utils import top_level_dict
```

### Comparing `smartscoutscrape-0.2.0/smartscoutscrape/utils.py` & `smartscoutscrape-0.2.1/smartscoutscrape/utils.py`

 * *Files identical despite different names*

### Comparing `smartscoutscrape-0.2.0/PKG-INFO` & `smartscoutscrape-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartscoutscrape
-Version: 0.2.0
+Version: 0.2.1
 Summary: Lightweight data-extraction & general use library for smartscout.com
 Home-page: https://github.com/regulad/smartscout-scrape
 License: Apache-2.0
 Keywords: scraper,data science,requests,python,data
 Author: Parker Wahle
 Author-email: regulad@regulad.xyz
 Maintainer: Parker Wahle
```

