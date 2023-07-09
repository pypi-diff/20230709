# Comparing `tmp/pocket-to-sqlite-0.2.2.tar.gz` & `tmp/pocket-to-sqlite-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pocket-to-sqlite-0.2.2.tar", last modified: Mon Aug 22 16:22:39 2022, max compression
+gzip compressed data, was "pocket-to-sqlite-0.2.3.tar", last modified: Sun Jul  9 01:15:58 2023, max compression
```

## Comparing `pocket-to-sqlite-0.2.2.tar` & `pocket-to-sqlite-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 16:22:39.593724 pocket-to-sqlite-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-08-22 16:22:22.000000 pocket-to-sqlite-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2440 2022-08-22 16:22:39.593724 pocket-to-sqlite-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1821 2022-08-22 16:22:22.000000 pocket-to-sqlite-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 16:22:39.589724 pocket-to-sqlite-0.2.2/pocket_to_sqlite/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 16:22:22.000000 pocket-to-sqlite-0.2.2/pocket_to_sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3296 2022-08-22 16:22:22.000000 pocket-to-sqlite-0.2.2/pocket_to_sqlite/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     3913 2022-08-22 16:22:22.000000 pocket-to-sqlite-0.2.2/pocket_to_sqlite/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 16:22:39.593724 pocket-to-sqlite-0.2.2/pocket_to_sqlite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2440 2022-08-22 16:22:39.000000 pocket-to-sqlite-0.2.2/pocket_to_sqlite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      347 2022-08-22 16:22:39.000000 pocket-to-sqlite-0.2.2/pocket_to_sqlite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 16:22:39.000000 pocket-to-sqlite-0.2.2/pocket_to_sqlite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-08-22 16:22:39.000000 pocket-to-sqlite-0.2.2/pocket_to_sqlite.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-08-22 16:22:39.000000 pocket-to-sqlite-0.2.2/pocket_to_sqlite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-22 16:22:39.000000 pocket-to-sqlite-0.2.2/pocket_to_sqlite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-22 16:22:39.593724 pocket-to-sqlite-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1244 2022-08-22 16:22:22.000000 pocket-to-sqlite-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:15:58.403875 pocket-to-sqlite-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-09 01:15:41.000000 pocket-to-sqlite-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-09 01:15:58.403875 pocket-to-sqlite-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-09 01:15:41.000000 pocket-to-sqlite-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:15:58.399875 pocket-to-sqlite-0.2.3/pocket_to_sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 01:15:41.000000 pocket-to-sqlite-0.2.3/pocket_to_sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-09 01:15:41.000000 pocket-to-sqlite-0.2.3/pocket_to_sqlite/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-07-09 01:15:41.000000 pocket-to-sqlite-0.2.3/pocket_to_sqlite/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:15:58.399875 pocket-to-sqlite-0.2.3/pocket_to_sqlite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-09 01:15:58.000000 pocket-to-sqlite-0.2.3/pocket_to_sqlite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-09 01:15:58.000000 pocket-to-sqlite-0.2.3/pocket_to_sqlite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 01:15:58.000000 pocket-to-sqlite-0.2.3/pocket_to_sqlite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-09 01:15:58.000000 pocket-to-sqlite-0.2.3/pocket_to_sqlite.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-09 01:15:58.000000 pocket-to-sqlite-0.2.3/pocket_to_sqlite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-09 01:15:58.000000 pocket-to-sqlite-0.2.3/pocket_to_sqlite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-09 01:15:41.000000 pocket-to-sqlite-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 01:15:58.403875 pocket-to-sqlite-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:15:58.399875 pocket-to-sqlite-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-09 01:15:41.000000 pocket-to-sqlite-0.2.3/tests/test_save_pocket.py
```

### Comparing `pocket-to-sqlite-0.2.2/LICENSE` & `pocket-to-sqlite-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pocket-to-sqlite-0.2.2/PKG-INFO` & `pocket-to-sqlite-0.2.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,50 +1,57 @@
 Metadata-Version: 2.1
 Name: pocket-to-sqlite
-Version: 0.2.2
+Version: 0.2.3
 Summary: Create a SQLite database containing data from your Pocket account
-Home-page: https://github.com/dogsheep/pocket-to-sqlite
 Author: Simon Willison
-License: Apache License, Version 2.0
+License: Apache-2.0
+Project-URL: homepage, https://github.com/dogsheep/pocket-to-sqlite
+Project-URL: Changelog, https://github.com/dogsheep/pocket-to-sqlite/releases
 Project-URL: Issues, https://github.com/dogsheep/pocket-to-sqlite/issues
 Project-URL: CI, https://github.com/dogsheep/pocket-to-sqlite/actions
-Project-URL: Changelog, https://github.com/dogsheep/pocket-to-sqlite/releases
 Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # pocket-to-sqlite
 
 [![PyPI](https://img.shields.io/pypi/v/pocket-to-sqlite.svg)](https://pypi.org/project/pocket-to-sqlite/)
 [![Changelog](https://img.shields.io/github/v/release/dogsheep/pocket-to-sqlite?include_prereleases&label=changelog)](https://github.com/dogsheep/pocket-to-sqlite/releases)
 [![Tests](https://github.com/dogsheep/pocket-to-sqlite/workflows/Test/badge.svg)](https://github.com/dogsheep/pocket-to-sqlite/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/dogsheep/pocket-to-sqlite/blob/main/LICENSE)
 
 Create a SQLite database containing data from your [Pocket](https://getpocket.com/) account.
 
 ## How to install
-
-    $ pip install pocket-to-sqlite
-
+```bash
+pip install pocket-to-sqlite
+```
 ## Usage
 
 You will need to first obtain a valid OAuth token for your Pocket account. You can do this by running the `auth` command and following the prompts:
-
-    $ pocket-to-sqlite auth
-    Visit this page and sign in with your Pocket account:
-
-    https://getpocket.com/auth/author...
-
-    Once you have signed in there, hit <enter> to continue
-    Authentication tokens written to auth.json
+```bash
+pocket-to-sqlite auth
+```
+Which looks like this:
+```
+Visit this page and sign in with your Pocket account:
+
+https://getpocket.com/auth/author...
+
+Once you have signed in there, hit <enter> to continue
+Authentication tokens written to auth.json
+```
 
 Now you can fetch all of your items from Pocket like this:
 
-    $ pocket-to-sqlite fetch pocket.db
+```bash
+pocket-to-sqlite fetch pocket.db
+```
 
 The first time you run this command it will fetch all of your items, and display a progress bar while it does it.
 
 On subsequent runs it will only fetch new items.
 
 You can force it to fetch everything from the beginning again using `--all`. Use `--silent` to disable the progress bar.
```

### Comparing `pocket-to-sqlite-0.2.2/README.md` & `pocket-to-sqlite-0.2.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -4,32 +4,38 @@
 [![Changelog](https://img.shields.io/github/v/release/dogsheep/pocket-to-sqlite?include_prereleases&label=changelog)](https://github.com/dogsheep/pocket-to-sqlite/releases)
 [![Tests](https://github.com/dogsheep/pocket-to-sqlite/workflows/Test/badge.svg)](https://github.com/dogsheep/pocket-to-sqlite/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/dogsheep/pocket-to-sqlite/blob/main/LICENSE)
 
 Create a SQLite database containing data from your [Pocket](https://getpocket.com/) account.
 
 ## How to install
-
-    $ pip install pocket-to-sqlite
-
+```bash
+pip install pocket-to-sqlite
+```
 ## Usage
 
 You will need to first obtain a valid OAuth token for your Pocket account. You can do this by running the `auth` command and following the prompts:
-
-    $ pocket-to-sqlite auth
-    Visit this page and sign in with your Pocket account:
-
-    https://getpocket.com/auth/author...
-
-    Once you have signed in there, hit <enter> to continue
-    Authentication tokens written to auth.json
+```bash
+pocket-to-sqlite auth
+```
+Which looks like this:
+```
+Visit this page and sign in with your Pocket account:
+
+https://getpocket.com/auth/author...
+
+Once you have signed in there, hit <enter> to continue
+Authentication tokens written to auth.json
+```
 
 Now you can fetch all of your items from Pocket like this:
 
-    $ pocket-to-sqlite fetch pocket.db
+```bash
+pocket-to-sqlite fetch pocket.db
+```
 
 The first time you run this command it will fetch all of your items, and display a progress bar while it does it.
 
 On subsequent runs it will only fetch new items.
 
 You can force it to fetch everything from the beginning again using `--all`. Use `--silent` to disable the progress bar.
```

### Comparing `pocket-to-sqlite-0.2.2/pocket_to_sqlite/cli.py` & `pocket-to-sqlite-0.2.3/pocket_to_sqlite/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,14 +93,14 @@
         since=last_since,
         record_since=lambda since: db["since"].insert(
             {"id": 1, "since": since}, replace=True, pk="id"
         ),
     )
     if (all or last_since is None) and not silent:
         total_items = utils.fetch_stats(auth)["count_list"]
-        with click.progressbar(fetch, length=total_items) as bar:
+        with click.progressbar(fetch, length=total_items, show_pos=True) as bar:
             utils.save_items(bar, db)
     else:
         # No progress bar
         print("Fetching items since {}".format(last_since))
         utils.save_items(fetch, db)
     utils.ensure_fts(db)
```

### Comparing `pocket-to-sqlite-0.2.2/pocket_to_sqlite/utils.py` & `pocket-to-sqlite-0.2.3/pocket_to_sqlite/utils.py`

 * *Files identical despite different names*

### Comparing `pocket-to-sqlite-0.2.2/pocket_to_sqlite.egg-info/PKG-INFO` & `pocket-to-sqlite-0.2.3/pocket_to_sqlite.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,50 +1,57 @@
 Metadata-Version: 2.1
 Name: pocket-to-sqlite
-Version: 0.2.2
+Version: 0.2.3
 Summary: Create a SQLite database containing data from your Pocket account
-Home-page: https://github.com/dogsheep/pocket-to-sqlite
 Author: Simon Willison
-License: Apache License, Version 2.0
+License: Apache-2.0
+Project-URL: homepage, https://github.com/dogsheep/pocket-to-sqlite
+Project-URL: Changelog, https://github.com/dogsheep/pocket-to-sqlite/releases
 Project-URL: Issues, https://github.com/dogsheep/pocket-to-sqlite/issues
 Project-URL: CI, https://github.com/dogsheep/pocket-to-sqlite/actions
-Project-URL: Changelog, https://github.com/dogsheep/pocket-to-sqlite/releases
 Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # pocket-to-sqlite
 
 [![PyPI](https://img.shields.io/pypi/v/pocket-to-sqlite.svg)](https://pypi.org/project/pocket-to-sqlite/)
 [![Changelog](https://img.shields.io/github/v/release/dogsheep/pocket-to-sqlite?include_prereleases&label=changelog)](https://github.com/dogsheep/pocket-to-sqlite/releases)
 [![Tests](https://github.com/dogsheep/pocket-to-sqlite/workflows/Test/badge.svg)](https://github.com/dogsheep/pocket-to-sqlite/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/dogsheep/pocket-to-sqlite/blob/main/LICENSE)
 
 Create a SQLite database containing data from your [Pocket](https://getpocket.com/) account.
 
 ## How to install
-
-    $ pip install pocket-to-sqlite
-
+```bash
+pip install pocket-to-sqlite
+```
 ## Usage
 
 You will need to first obtain a valid OAuth token for your Pocket account. You can do this by running the `auth` command and following the prompts:
-
-    $ pocket-to-sqlite auth
-    Visit this page and sign in with your Pocket account:
-
-    https://getpocket.com/auth/author...
-
-    Once you have signed in there, hit <enter> to continue
-    Authentication tokens written to auth.json
+```bash
+pocket-to-sqlite auth
+```
+Which looks like this:
+```
+Visit this page and sign in with your Pocket account:
+
+https://getpocket.com/auth/author...
+
+Once you have signed in there, hit <enter> to continue
+Authentication tokens written to auth.json
+```
 
 Now you can fetch all of your items from Pocket like this:
 
-    $ pocket-to-sqlite fetch pocket.db
+```bash
+pocket-to-sqlite fetch pocket.db
+```
 
 The first time you run this command it will fetch all of your items, and display a progress bar while it does it.
 
 On subsequent runs it will only fetch new items.
 
 You can force it to fetch everything from the beginning again using `--all`. Use `--silent` to disable the progress bar.
```

