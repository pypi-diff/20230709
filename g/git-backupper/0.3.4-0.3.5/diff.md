# Comparing `tmp/git-backupper-0.3.4.tar.gz` & `tmp/git-backupper-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-backupper-0.3.4.tar", last modified: Fri May  5 16:10:29 2023, max compression
+gzip compressed data, was "git-backupper-0.3.5.tar", last modified: Sun Jul  9 12:48:44 2023, max compression
```

## Comparing `git-backupper-0.3.4.tar` & `git-backupper-0.3.5.tar`

### file list

```diff
@@ -1,49 +1,51 @@
-drwxr-xr-x   0 pika      (1000) pika      (1000)        0 2023-05-05 16:10:29.565394 git-backupper-0.3.4/
--rw-r--r--   0 pika      (1000) pika      (1000)       12 2023-05-05 16:01:30.000000 git-backupper-0.3.4/.gitattributes
--rw-r--r--   0 pika      (1000) pika      (1000)      815 2023-05-05 16:01:30.000000 git-backupper-0.3.4/.githooks.yml
-drwxr-xr-x   0 pika      (1000) pika      (1000)        0 2023-05-05 16:10:29.561394 git-backupper-0.3.4/.github/
-drwxr-xr-x   0 pika      (1000) pika      (1000)        0 2023-05-05 16:10:29.563394 git-backupper-0.3.4/.github/workflows/
--rw-r--r--   0 pika      (1000) pika      (1000)      540 2023-05-05 16:01:30.000000 git-backupper-0.3.4/.github/workflows/tests.yml
--rw-r--r--   0 pika      (1000) pika      (1000)       86 2023-05-05 16:01:30.000000 git-backupper-0.3.4/.gitignore
--rw-r--r--   0 pika      (1000) pika      (1000)       43 2023-05-05 16:01:30.000000 git-backupper-0.3.4/.mailmap
--rw-r--r--   0 pika      (1000) pika      (1000)       28 2023-05-05 16:01:30.000000 git-backupper-0.3.4/.mypy.ini
--rw-r--r--   0 pika      (1000) pika      (1000)      263 2023-05-05 16:01:30.000000 git-backupper-0.3.4/HOWTOPUBLISH
--rw-r--r--   0 pika      (1000) pika      (1000)     1072 2023-05-05 16:01:30.000000 git-backupper-0.3.4/LICENSE
--rw-r--r--   0 pika      (1000) pika      (1000)       26 2023-05-05 16:01:30.000000 git-backupper-0.3.4/MANIFEST.in
--rw-r--r--   0 pika      (1000) pika      (1000)     3438 2023-05-05 16:10:29.565394 git-backupper-0.3.4/PKG-INFO
--rw-r--r--   0 pika      (1000) pika      (1000)     2325 2023-05-05 16:01:30.000000 git-backupper-0.3.4/README.md
--rw-r--r--   0 pika      (1000) pika      (1000)   463052 2023-05-05 16:01:30.000000 git-backupper-0.3.4/git-backupper.gif
-drwxr-xr-x   0 pika      (1000) pika      (1000)        0 2023-05-05 16:10:29.564394 git-backupper-0.3.4/git_backupper/
--rw-r--r--   0 pika      (1000) pika      (1000)        0 2023-05-05 16:01:30.000000 git-backupper-0.3.4/git_backupper/__init__.py
--rw-r--r--   0 pika      (1000) pika      (1000)     1971 2023-05-05 16:01:30.000000 git-backupper-0.3.4/git_backupper/__main__.py
--rw-r--r--   0 pika      (1000) pika      (1000)     2224 2023-05-05 16:01:30.000000 git-backupper-0.3.4/git_backupper/api.py
--rw-r--r--   0 pika      (1000) pika      (1000)     1961 2023-05-05 16:01:30.000000 git-backupper-0.3.4/git_backupper/cache.py
--rw-r--r--   0 pika      (1000) pika      (1000)      451 2023-05-05 16:01:30.000000 git-backupper-0.3.4/git_backupper/defaults.py
--rw-r--r--   0 pika      (1000) pika      (1000)     1262 2023-05-05 16:01:30.000000 git-backupper-0.3.4/git_backupper/exceptions.py
--rw-r--r--   0 pika      (1000) pika      (1000)     2548 2023-05-05 16:01:30.000000 git-backupper-0.3.4/git_backupper/fs.py
--rw-r--r--   0 pika      (1000) pika      (1000)     1228 2023-05-05 16:01:30.000000 git-backupper-0.3.4/git_backupper/logger_wrapper.py
--rw-r--r--   0 pika      (1000) pika      (1000)        0 2023-05-05 16:01:30.000000 git-backupper-0.3.4/git_backupper/py.typed
--rw-r--r--   0 pika      (1000) pika      (1000)     3341 2023-05-05 16:01:30.000000 git-backupper-0.3.4/git_backupper/repository.py
-drwxr-xr-x   0 pika      (1000) pika      (1000)        0 2023-05-05 16:10:29.565394 git-backupper-0.3.4/git_backupper/settings/
--rw-r--r--   0 pika      (1000) pika      (1000)      142 2023-05-05 16:01:30.000000 git-backupper-0.3.4/git_backupper/settings/__init__.py
--rw-r--r--   0 pika      (1000) pika      (1000)     2014 2023-05-05 16:01:30.000000 git-backupper-0.3.4/git_backupper/settings/fields.py
--rw-r--r--   0 pika      (1000) pika      (1000)     2262 2023-05-05 16:01:30.000000 git-backupper-0.3.4/git_backupper/settings/settings.py
-drwxr-xr-x   0 pika      (1000) pika      (1000)        0 2023-05-05 16:10:29.564394 git-backupper-0.3.4/git_backupper.egg-info/
--rw-r--r--   0 pika      (1000) pika      (1000)     3438 2023-05-05 16:10:29.000000 git-backupper-0.3.4/git_backupper.egg-info/PKG-INFO
--rw-r--r--   0 pika      (1000) pika      (1000)      910 2023-05-05 16:10:29.000000 git-backupper-0.3.4/git_backupper.egg-info/SOURCES.txt
--rw-r--r--   0 pika      (1000) pika      (1000)        1 2023-05-05 16:10:29.000000 git-backupper-0.3.4/git_backupper.egg-info/dependency_links.txt
--rw-r--r--   0 pika      (1000) pika      (1000)       62 2023-05-05 16:10:29.000000 git-backupper-0.3.4/git_backupper.egg-info/entry_points.txt
--rw-r--r--   0 pika      (1000) pika      (1000)       85 2023-05-05 16:10:29.000000 git-backupper-0.3.4/git_backupper.egg-info/requires.txt
--rw-r--r--   0 pika      (1000) pika      (1000)       14 2023-05-05 16:10:29.000000 git-backupper-0.3.4/git_backupper.egg-info/top_level.txt
--rw-r--r--   0 pika      (1000) pika      (1000)     1745 2023-05-05 16:08:59.000000 git-backupper-0.3.4/pyproject.toml
--rw-r--r--   0 pika      (1000) pika      (1000)       38 2023-05-05 16:10:29.565394 git-backupper-0.3.4/setup.cfg
-drwxr-xr-x   0 pika      (1000) pika      (1000)        0 2023-05-05 16:10:29.565394 git-backupper-0.3.4/tests/
--rw-r--r--   0 pika      (1000) pika      (1000)      793 2023-05-05 16:01:30.000000 git-backupper-0.3.4/tests/conftest.py
-drwxr-xr-x   0 pika      (1000) pika      (1000)        0 2023-05-05 16:10:29.565394 git-backupper-0.3.4/tests/settings/
--rw-r--r--   0 pika      (1000) pika      (1000)     1225 2023-05-05 16:01:30.000000 git-backupper-0.3.4/tests/settings/test_fields.py
--rw-r--r--   0 pika      (1000) pika      (1000)     3057 2023-05-05 16:01:30.000000 git-backupper-0.3.4/tests/settings/test_settings.py
--rw-r--r--   0 pika      (1000) pika      (1000)     2220 2023-05-05 16:01:30.000000 git-backupper-0.3.4/tests/test_api.py
--rw-r--r--   0 pika      (1000) pika      (1000)     2185 2023-05-05 16:01:30.000000 git-backupper-0.3.4/tests/test_cache.py
--rw-r--r--   0 pika      (1000) pika      (1000)     2460 2023-05-05 16:01:30.000000 git-backupper-0.3.4/tests/test_fs.py
--rw-r--r--   0 pika      (1000) pika      (1000)     4201 2023-05-05 16:01:30.000000 git-backupper-0.3.4/tests/test_repository.py
--rw-r--r--   0 pika      (1000) pika      (1000)      384 2023-05-05 16:01:30.000000 git-backupper-0.3.4/tox.ini
+drwxr-xr-x   0 pika      (1000) pika      (1000)        0 2023-07-09 12:48:44.203355 git-backupper-0.3.5/
+-rw-r--r--   0 pika      (1000) pika      (1000)       12 2023-07-09 12:34:05.000000 git-backupper-0.3.5/.gitattributes
+-rw-r--r--   0 pika      (1000) pika      (1000)     1125 2023-07-09 12:39:43.000000 git-backupper-0.3.5/.githooks.yml
+drwxr-xr-x   0 pika      (1000) pika      (1000)        0 2023-07-09 12:48:44.201355 git-backupper-0.3.5/.github/
+-rw-r--r--   0 pika      (1000) pika      (1000)        0 2023-07-09 12:40:43.000000 git-backupper-0.3.5/.github/.gitkeep
+drwxr-xr-x   0 pika      (1000) pika      (1000)        0 2023-07-09 12:48:44.201355 git-backupper-0.3.5/.github/workflows/
+-rw-r--r--   0 pika      (1000) pika      (1000)      569 2023-07-09 12:41:12.000000 git-backupper-0.3.5/.github/workflows/tests.yml
+-rw-r--r--   0 pika      (1000) pika      (1000)      146 2023-07-09 12:37:42.000000 git-backupper-0.3.5/.gitignore
+-rw-r--r--   0 pika      (1000) pika      (1000)        0 2023-07-09 12:41:25.000000 git-backupper-0.3.5/.gitkeep
+-rw-r--r--   0 pika      (1000) pika      (1000)       43 2023-07-09 12:34:05.000000 git-backupper-0.3.5/.mailmap
+-rw-r--r--   0 pika      (1000) pika      (1000)       28 2023-07-09 12:34:05.000000 git-backupper-0.3.5/.mypy.ini
+-rw-r--r--   0 pika      (1000) pika      (1000)      263 2023-07-09 12:34:05.000000 git-backupper-0.3.5/HOWTOPUBLISH
+-rw-r--r--   0 pika      (1000) pika      (1000)     1072 2023-07-09 12:34:05.000000 git-backupper-0.3.5/LICENSE
+-rw-r--r--   0 pika      (1000) pika      (1000)       26 2023-07-09 12:34:05.000000 git-backupper-0.3.5/MANIFEST.in
+-rw-r--r--   0 pika      (1000) pika      (1000)     3436 2023-07-09 12:48:44.203355 git-backupper-0.3.5/PKG-INFO
+-rw-r--r--   0 pika      (1000) pika      (1000)     2323 2023-07-09 12:43:29.000000 git-backupper-0.3.5/README.md
+-rw-r--r--   0 pika      (1000) pika      (1000)   463052 2023-07-09 12:34:05.000000 git-backupper-0.3.5/git-backupper.gif
+drwxr-xr-x   0 pika      (1000) pika      (1000)        0 2023-07-09 12:48:44.202355 git-backupper-0.3.5/git_backupper/
+-rw-r--r--   0 pika      (1000) pika      (1000)        0 2023-07-09 12:34:05.000000 git-backupper-0.3.5/git_backupper/__init__.py
+-rw-r--r--   0 pika      (1000) pika      (1000)     1971 2023-07-09 12:34:05.000000 git-backupper-0.3.5/git_backupper/__main__.py
+-rw-r--r--   0 pika      (1000) pika      (1000)     2224 2023-07-09 12:34:05.000000 git-backupper-0.3.5/git_backupper/api.py
+-rw-r--r--   0 pika      (1000) pika      (1000)     1961 2023-07-09 12:34:05.000000 git-backupper-0.3.5/git_backupper/cache.py
+-rw-r--r--   0 pika      (1000) pika      (1000)      451 2023-07-09 12:34:05.000000 git-backupper-0.3.5/git_backupper/defaults.py
+-rw-r--r--   0 pika      (1000) pika      (1000)     1262 2023-07-09 12:34:05.000000 git-backupper-0.3.5/git_backupper/exceptions.py
+-rw-r--r--   0 pika      (1000) pika      (1000)     2548 2023-07-09 12:34:05.000000 git-backupper-0.3.5/git_backupper/fs.py
+-rw-r--r--   0 pika      (1000) pika      (1000)     1228 2023-07-09 12:34:05.000000 git-backupper-0.3.5/git_backupper/logger_wrapper.py
+-rw-r--r--   0 pika      (1000) pika      (1000)        0 2023-07-09 12:34:05.000000 git-backupper-0.3.5/git_backupper/py.typed
+-rw-r--r--   0 pika      (1000) pika      (1000)     3341 2023-07-09 12:34:05.000000 git-backupper-0.3.5/git_backupper/repository.py
+drwxr-xr-x   0 pika      (1000) pika      (1000)        0 2023-07-09 12:48:44.203355 git-backupper-0.3.5/git_backupper/settings/
+-rw-r--r--   0 pika      (1000) pika      (1000)      142 2023-07-09 12:34:05.000000 git-backupper-0.3.5/git_backupper/settings/__init__.py
+-rw-r--r--   0 pika      (1000) pika      (1000)     2014 2023-07-09 12:34:05.000000 git-backupper-0.3.5/git_backupper/settings/fields.py
+-rw-r--r--   0 pika      (1000) pika      (1000)     2262 2023-07-09 12:34:05.000000 git-backupper-0.3.5/git_backupper/settings/settings.py
+drwxr-xr-x   0 pika      (1000) pika      (1000)        0 2023-07-09 12:48:44.202355 git-backupper-0.3.5/git_backupper.egg-info/
+-rw-r--r--   0 pika      (1000) pika      (1000)     3436 2023-07-09 12:48:44.000000 git-backupper-0.3.5/git_backupper.egg-info/PKG-INFO
+-rw-r--r--   0 pika      (1000) pika      (1000)      936 2023-07-09 12:48:44.000000 git-backupper-0.3.5/git_backupper.egg-info/SOURCES.txt
+-rw-r--r--   0 pika      (1000) pika      (1000)        1 2023-07-09 12:48:44.000000 git-backupper-0.3.5/git_backupper.egg-info/dependency_links.txt
+-rw-r--r--   0 pika      (1000) pika      (1000)       62 2023-07-09 12:48:44.000000 git-backupper-0.3.5/git_backupper.egg-info/entry_points.txt
+-rw-r--r--   0 pika      (1000) pika      (1000)       71 2023-07-09 12:48:44.000000 git-backupper-0.3.5/git_backupper.egg-info/requires.txt
+-rw-r--r--   0 pika      (1000) pika      (1000)       14 2023-07-09 12:48:44.000000 git-backupper-0.3.5/git_backupper.egg-info/top_level.txt
+-rw-r--r--   0 pika      (1000) pika      (1000)     1689 2023-07-09 12:39:03.000000 git-backupper-0.3.5/pyproject.toml
+-rw-r--r--   0 pika      (1000) pika      (1000)       38 2023-07-09 12:48:44.204355 git-backupper-0.3.5/setup.cfg
+drwxr-xr-x   0 pika      (1000) pika      (1000)        0 2023-07-09 12:48:44.203355 git-backupper-0.3.5/tests/
+-rw-r--r--   0 pika      (1000) pika      (1000)      793 2023-07-09 12:34:05.000000 git-backupper-0.3.5/tests/conftest.py
+drwxr-xr-x   0 pika      (1000) pika      (1000)        0 2023-07-09 12:48:44.203355 git-backupper-0.3.5/tests/settings/
+-rw-r--r--   0 pika      (1000) pika      (1000)     1225 2023-07-09 12:34:05.000000 git-backupper-0.3.5/tests/settings/test_fields.py
+-rw-r--r--   0 pika      (1000) pika      (1000)     3057 2023-07-09 12:34:05.000000 git-backupper-0.3.5/tests/settings/test_settings.py
+-rw-r--r--   0 pika      (1000) pika      (1000)     2220 2023-07-09 12:34:05.000000 git-backupper-0.3.5/tests/test_api.py
+-rw-r--r--   0 pika      (1000) pika      (1000)     2185 2023-07-09 12:34:05.000000 git-backupper-0.3.5/tests/test_cache.py
+-rw-r--r--   0 pika      (1000) pika      (1000)     2460 2023-07-09 12:34:05.000000 git-backupper-0.3.5/tests/test_fs.py
+-rw-r--r--   0 pika      (1000) pika      (1000)     4201 2023-07-09 12:34:05.000000 git-backupper-0.3.5/tests/test_repository.py
+-rw-r--r--   0 pika      (1000) pika      (1000)      446 2023-07-09 12:39:59.000000 git-backupper-0.3.5/tox.ini
```

### Comparing `git-backupper-0.3.4/.github/workflows/tests.yml` & `git-backupper-0.3.5/.github/workflows/tests.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: python tests
+name: python testing and linting
 
 on:
   push:
     branches:
       - "master"
 
 jobs:
@@ -22,8 +22,8 @@
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Step -- 3.
         run: pip3 install --upgrade pip && pip3 install --no-cache-dir --upgrade tox
 
       - name: Step -- 4.
-        run: tox
+        run: tox && tox -e lint
```

### Comparing `git-backupper-0.3.4/LICENSE` & `git-backupper-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `git-backupper-0.3.4/PKG-INFO` & `git-backupper-0.3.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-backupper
-Version: 0.3.4
+Version: 0.3.5
 Summary: Simplest way to backup and restore git repositories
 Author-email: Vladislav Punko <iam.vlad.punko@gmail.com>
 License: MIT
 Project-URL: Issue tracker, https://github.com/vladpunko/git-backupper/issues
 Project-URL: Source code, https://github.com/vladpunko/git-backupper
 Keywords: automation,git
 Classifier: Intended Audience :: Developers
@@ -74,15 +74,15 @@
 # Step -- 1.
 git-backupper  # back up all repositories from the configuration file
 
 # Step -- 2.
 cd /tmp/backup_repositories/git-backupper.git
 
 # Step -- 3.
-git push --mirror 'https://github.com/vladpunko/git-backupper.git'
+git push --mirror https://github.com/vladpunko/git-backupper.git
 ```
 
 ## Contributing
 
 Pull requests are welcome.
 Please open an issue first to discuss what should be changed.
```

### Comparing `git-backupper-0.3.4/README.md` & `git-backupper-0.3.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 # Step -- 1.
 git-backupper  # back up all repositories from the configuration file
 
 # Step -- 2.
 cd /tmp/backup_repositories/git-backupper.git
 
 # Step -- 3.
-git push --mirror 'https://github.com/vladpunko/git-backupper.git'
+git push --mirror https://github.com/vladpunko/git-backupper.git
 ```
 
 ## Contributing
 
 Pull requests are welcome.
 Please open an issue first to discuss what should be changed.
```

### Comparing `git-backupper-0.3.4/git-backupper.gif` & `git-backupper-0.3.5/git-backupper.gif`

 * *Files identical despite different names*

### Comparing `git-backupper-0.3.4/git_backupper/__main__.py` & `git-backupper-0.3.5/git_backupper/__main__.py`

 * *Files identical despite different names*

### Comparing `git-backupper-0.3.4/git_backupper/api.py` & `git-backupper-0.3.5/git_backupper/api.py`

 * *Files identical despite different names*

### Comparing `git-backupper-0.3.4/git_backupper/cache.py` & `git-backupper-0.3.5/git_backupper/cache.py`

 * *Files identical despite different names*

### Comparing `git-backupper-0.3.4/git_backupper/exceptions.py` & `git-backupper-0.3.5/git_backupper/exceptions.py`

 * *Files identical despite different names*

### Comparing `git-backupper-0.3.4/git_backupper/fs.py` & `git-backupper-0.3.5/git_backupper/fs.py`

 * *Files identical despite different names*

### Comparing `git-backupper-0.3.4/git_backupper/logger_wrapper.py` & `git-backupper-0.3.5/git_backupper/logger_wrapper.py`

 * *Files identical despite different names*

### Comparing `git-backupper-0.3.4/git_backupper/repository.py` & `git-backupper-0.3.5/git_backupper/repository.py`

 * *Files identical despite different names*

### Comparing `git-backupper-0.3.4/git_backupper/settings/fields.py` & `git-backupper-0.3.5/git_backupper/settings/fields.py`

 * *Files identical despite different names*

### Comparing `git-backupper-0.3.4/git_backupper/settings/settings.py` & `git-backupper-0.3.5/git_backupper/settings/settings.py`

 * *Files identical despite different names*

### Comparing `git-backupper-0.3.4/git_backupper.egg-info/PKG-INFO` & `git-backupper-0.3.5/git_backupper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-backupper
-Version: 0.3.4
+Version: 0.3.5
 Summary: Simplest way to backup and restore git repositories
 Author-email: Vladislav Punko <iam.vlad.punko@gmail.com>
 License: MIT
 Project-URL: Issue tracker, https://github.com/vladpunko/git-backupper/issues
 Project-URL: Source code, https://github.com/vladpunko/git-backupper
 Keywords: automation,git
 Classifier: Intended Audience :: Developers
@@ -74,15 +74,15 @@
 # Step -- 1.
 git-backupper  # back up all repositories from the configuration file
 
 # Step -- 2.
 cd /tmp/backup_repositories/git-backupper.git
 
 # Step -- 3.
-git push --mirror 'https://github.com/vladpunko/git-backupper.git'
+git push --mirror https://github.com/vladpunko/git-backupper.git
 ```
 
 ## Contributing
 
 Pull requests are welcome.
 Please open an issue first to discuss what should be changed.
```

### Comparing `git-backupper-0.3.4/git_backupper.egg-info/SOURCES.txt` & `git-backupper-0.3.5/git_backupper.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 .gitattributes
 .githooks.yml
 .gitignore
+.gitkeep
 .mailmap
 .mypy.ini
 HOWTOPUBLISH
 LICENSE
 MANIFEST.in
 README.md
 git-backupper.gif
 pyproject.toml
 tox.ini
+.github/.gitkeep
 .github/workflows/tests.yml
 git_backupper/__init__.py
 git_backupper/__main__.py
 git_backupper/api.py
 git_backupper/cache.py
 git_backupper/defaults.py
 git_backupper/exceptions.py
```

### Comparing `git-backupper-0.3.4/pyproject.toml` & `git-backupper-0.3.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 dynamic = ["version"]
 
 [project.urls]
 "Issue tracker" = "https://github.com/vladpunko/git-backupper/issues"
 "Source code" = "https://github.com/vladpunko/git-backupper"
 
 [project.optional-dependencies]
-dev = ["black>=22.0.0", "ruff>=0.0.250", "mypy>=v0.950", "pre-commit>=3.0.0"]
+dev = ["black>=23.0.0", "isort>=5.0.0", "pre-commit>=3.0.0"]
 test = ["tox>=4.0.0"]
 
 [project.scripts]
 git-backupper = "git_backupper.__main__:main"
 
 [tool.setuptools_scm]
 version_scheme = "post-release"
@@ -51,10 +51,9 @@
 parallel = true
 source = ["git_backupper"]
 
 [tool.black]
 line-length = 100
 target-version = ["py39", "py310", "py311"]
 
-[tool.ruff]
-line-length = 100
-select = ["B", "C", "E", "F", "I", "W"]
+[tool.isort]
+profile = "black"
```

### Comparing `git-backupper-0.3.4/tests/conftest.py` & `git-backupper-0.3.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `git-backupper-0.3.4/tests/settings/test_fields.py` & `git-backupper-0.3.5/tests/settings/test_fields.py`

 * *Files identical despite different names*

### Comparing `git-backupper-0.3.4/tests/settings/test_settings.py` & `git-backupper-0.3.5/tests/settings/test_settings.py`

 * *Files identical despite different names*

### Comparing `git-backupper-0.3.4/tests/test_api.py` & `git-backupper-0.3.5/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `git-backupper-0.3.4/tests/test_cache.py` & `git-backupper-0.3.5/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `git-backupper-0.3.4/tests/test_fs.py` & `git-backupper-0.3.5/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `git-backupper-0.3.4/tests/test_repository.py` & `git-backupper-0.3.5/tests/test_repository.py`

 * *Files identical despite different names*

