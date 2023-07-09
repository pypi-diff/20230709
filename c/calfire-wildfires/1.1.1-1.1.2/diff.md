# Comparing `tmp/calfire-wildfires-1.1.1.tar.gz` & `tmp/calfire-wildfires-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calfire-wildfires-1.1.1.tar", last modified: Fri Apr 28 19:56:14 2023, max compression
+gzip compressed data, was "calfire-wildfires-1.1.2.tar", last modified: Sun Jul  9 19:50:03 2023, max compression
```

## Comparing `calfire-wildfires-1.1.1.tar` & `calfire-wildfires-1.1.2.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:56:14.221748 calfire-wildfires-1.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:56:14.213748 calfire-wildfires-1.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:56:14.217748 calfire-wildfires-1.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/.github/workflows/continuous-deployment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/.github/workflows/scrape.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-28 19:56:14.221748 calfire-wildfires-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    37856 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:56:14.217748 calfire-wildfires-1.1.1/calfire_wildfires/
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/calfire_wildfires/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/calfire_wildfires/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:56:14.217748 calfire-wildfires-1.1.1/calfire_wildfires.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-28 19:56:14.000000 calfire-wildfires-1.1.1/calfire_wildfires.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-28 19:56:14.000000 calfire-wildfires-1.1.1/calfire_wildfires.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 19:56:14.000000 calfire-wildfires-1.1.1/calfire_wildfires.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-28 19:56:14.000000 calfire-wildfires-1.1.1/calfire_wildfires.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 19:56:14.000000 calfire-wildfires-1.1.1/calfire_wildfires.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-28 19:56:14.000000 calfire-wildfires-1.1.1/calfire_wildfires.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:56:14.217748 calfire-wildfires-1.1.1/data/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/data/active.json
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/data/all.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:56:14.217748 calfire-wildfires-1.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:56:14.213748 calfire-wildfires-1.1.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:56:14.217748 calfire-wildfires-1.1.1/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:56:14.217748 calfire-wildfires-1.1.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/docs/_templates/nav.html
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-28 19:56:14.221748 calfire-wildfires-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-28 19:56:05.000000 calfire-wildfires-1.1.1/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 19:50:03.391757 calfire-wildfires-1.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 19:50:03.387756 calfire-wildfires-1.1.2/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-09 19:49:53.000000 calfire-wildfires-1.1.2/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 19:50:03.387756 calfire-wildfires-1.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 19:50:03.391757 calfire-wildfires-1.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-09 19:49:53.000000 calfire-wildfires-1.1.2/.github/workflows/continuous-deployment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-09 19:49:53.000000 calfire-wildfires-1.1.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-09 19:49:53.000000 calfire-wildfires-1.1.2/.github/workflows/scrape.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-09 19:49:53.000000 calfire-wildfires-1.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-09 19:49:53.000000 calfire-wildfires-1.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-09 19:49:53.000000 calfire-wildfires-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-09 19:49:53.000000 calfire-wildfires-1.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-07-09 19:50:03.391757 calfire-wildfires-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-09 19:49:53.000000 calfire-wildfires-1.1.2/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    50570 2023-07-09 19:49:53.000000 calfire-wildfires-1.1.2/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-09 19:49:53.000000 calfire-wildfires-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 19:50:03.391757 calfire-wildfires-1.1.2/calfire_wildfires/
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-09 19:49:53.000000 calfire-wildfires-1.1.2/calfire_wildfires/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-09 19:49:53.000000 calfire-wildfires-1.1.2/calfire_wildfires/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 19:50:03.391757 calfire-wildfires-1.1.2/calfire_wildfires.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-07-09 19:50:03.000000 calfire-wildfires-1.1.2/calfire_wildfires.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-09 19:50:03.000000 calfire-wildfires-1.1.2/calfire_wildfires.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 19:50:03.000000 calfire-wildfires-1.1.2/calfire_wildfires.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-09 19:50:03.000000 calfire-wildfires-1.1.2/calfire_wildfires.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-09 19:50:03.000000 calfire-wildfires-1.1.2/calfire_wildfires.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-09 19:50:03.000000 calfire-wildfires-1.1.2/calfire_wildfires.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 19:50:03.391757 calfire-wildfires-1.1.2/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-09 19:49:53.000000 calfire-wildfires-1.1.2/data/active.json
+-rw-r--r--   0 runner    (1001) docker     (123)    34300 2023-07-09 19:49:53.000000 calfire-wildfires-1.1.2/data/all.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 19:50:03.391757 calfire-wildfires-1.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-09 19:49:53.000000 calfire-wildfires-1.1.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 19:50:03.387756 calfire-wildfires-1.1.2/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 19:50:03.391757 calfire-wildfires-1.1.2/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-09 19:49:53.000000 calfire-wildfires-1.1.2/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 19:50:03.391757 calfire-wildfires-1.1.2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-09 19:49:53.000000 calfire-wildfires-1.1.2/docs/_templates/nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-09 19:49:53.000000 calfire-wildfires-1.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-09 19:49:53.000000 calfire-wildfires-1.1.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-09 19:49:53.000000 calfire-wildfires-1.1.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-09 19:49:53.000000 calfire-wildfires-1.1.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-09 19:50:03.391757 calfire-wildfires-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-09 19:49:53.000000 calfire-wildfires-1.1.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-09 19:49:53.000000 calfire-wildfires-1.1.2/test.py
```

### Comparing `calfire-wildfires-1.1.1/.github/workflows/continuous-deployment.yml` & `calfire-wildfires-1.1.2/.github/workflows/continuous-deployment.yml`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
       - id: run
         name: Run
         run: pipenv run flake8 calfire_wildfires
 
   test-python:
     strategy:
       matrix:
-        python: ['3.7', '3.8', '3.9', '3.10']
+        python: ['3.8', '3.9', '3.10', '3.11']
     name: Test
     runs-on: ubuntu-latest
     steps:
       - name: Checkout
         uses: actions/checkout@v3
 
       - name: Install pipenv
```

### Comparing `calfire-wildfires-1.1.1/.github/workflows/docs.yml` & `calfire-wildfires-1.1.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `calfire-wildfires-1.1.1/.github/workflows/scrape.yml` & `calfire-wildfires-1.1.2/.github/workflows/scrape.yml`

 * *Files identical despite different names*

### Comparing `calfire-wildfires-1.1.1/.gitignore` & `calfire-wildfires-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `calfire-wildfires-1.1.1/.pre-commit-config.yaml` & `calfire-wildfires-1.1.2/.pre-commit-config.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
 repos:
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.1.0
+    rev: v4.4.0
     hooks:
     -   id: trailing-whitespace
     -   id: end-of-file-fixer
     -   id: check-yaml
     -   id: check-added-large-files
         args: ['--maxkb=10000']
     -   id: check-case-conflict
     -   id: mixed-line-ending
 
 -   repo: https://github.com/psf/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
     -   id: black
 
 -   repo: https://github.com/asottile/blacken-docs
-    rev: v1.12.1
+    rev: 1.15.0
     hooks:
     -   id: blacken-docs
         additional_dependencies: [black]
 
 -   repo: https://github.com/timothycrosley/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
     -   id: isort
         args: ["--profile", "black", "--filter-files"]
 
--   repo: https://gitlab.com/pycqa/flake8
-    rev: 3.9.2
+-   repo: https://github.com/pycqa/flake8
+    rev: 6.0.0
     hooks:
     - id: flake8
 
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v2.31.0
+    rev: v3.9.0
     hooks:
     -   id: pyupgrade
         args: [--py37-plus]
```

### Comparing `calfire-wildfires-1.1.1/LICENSE` & `calfire-wildfires-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `calfire-wildfires-1.1.1/PKG-INFO` & `calfire-wildfires-1.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: calfire-wildfires
-Version: 1.1.1
+Version: 1.1.2
 Summary: Download wildfires data from CalFire
 Home-page: https://palewi.re/docs/calfire-wildfires/
 Author: Ben Welsh
 Author-email: b@palewi.re
 License: MIT
 Project-URL: Maintainer, https://github.com/datadesk
 Project-URL: Source, https://github.com/datadesk/calfire-wildfires
 Project-URL: Tracker, https://github.com/datadesk/calfire-wildfires/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Califire Wildfires
 Download wildfires data from Calfire
```

### Comparing `calfire-wildfires-1.1.1/Pipfile.lock` & `calfire-wildfires-1.1.2/Pipfile.lock`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9246527777777778%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'711a5e611d1159bf86ad7fdca432d78a636e8b6ec8df8f860602539faafd376d'}, 'requires': "*

 * *            "{'python_version': '3.10'}}",*

 * * "'default'": "{'certifi': {'hashes': "*

 * *              "['sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7', "*

 * *              "'sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716'], "*

 * *              "'version': '==2023.5.7'}, 'charset-normalizer': {'hashes': "*

 * *              "['sha256:04e57ab9fbf9 […]*

```diff
@@ -1,72 +1,145 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "d7a48589ea82f0f169eb8a249455ed3e9c054839268b873813f04b76fbc3aaed"
+            "sha256": "711a5e611d1159bf86ad7fdca432d78a636e8b6ec8df8f860602539faafd376d"
         },
         "pipfile-spec": 6,
         "requires": {
-            "python_version": "3.9"
+            "python_version": "3.10"
         },
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.org/simple",
                 "verify_ssl": true
             }
         ]
     },
     "default": {
         "certifi": {
             "hashes": [
-                "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
-                "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
+                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
+                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2022.12.7"
+            "version": "==2023.5.7"
         },
         "charset-normalizer": {
             "hashes": [
-                "sha256:2857e29ff0d34db842cd7ca3230549d1a697f96ee6d3fb071cfa6c7393832597",
-                "sha256:6881edbebdb17b39b4eaaa821b438bf6eddffb4468cf344f09f89def34a8b1df"
+                "sha256:04e57ab9fbf9607b77f7d057974694b4f6b142da9ed4a199859d9d4d5c63fe96",
+                "sha256:09393e1b2a9461950b1c9a45d5fd251dc7c6f228acab64da1c9c0165d9c7765c",
+                "sha256:0b87549028f680ca955556e3bd57013ab47474c3124dc069faa0b6545b6c9710",
+                "sha256:1000fba1057b92a65daec275aec30586c3de2401ccdcd41f8a5c1e2c87078706",
+                "sha256:1249cbbf3d3b04902ff081ffbb33ce3377fa6e4c7356f759f3cd076cc138d020",
+                "sha256:1920d4ff15ce893210c1f0c0e9d19bfbecb7983c76b33f046c13a8ffbd570252",
+                "sha256:193cbc708ea3aca45e7221ae58f0fd63f933753a9bfb498a3b474878f12caaad",
+                "sha256:1a100c6d595a7f316f1b6f01d20815d916e75ff98c27a01ae817439ea7726329",
+                "sha256:1f30b48dd7fa1474554b0b0f3fdfdd4c13b5c737a3c6284d3cdc424ec0ffff3a",
+                "sha256:203f0c8871d5a7987be20c72442488a0b8cfd0f43b7973771640fc593f56321f",
+                "sha256:246de67b99b6851627d945db38147d1b209a899311b1305dd84916f2b88526c6",
+                "sha256:2dee8e57f052ef5353cf608e0b4c871aee320dd1b87d351c28764fc0ca55f9f4",
+                "sha256:2efb1bd13885392adfda4614c33d3b68dee4921fd0ac1d3988f8cbb7d589e72a",
+                "sha256:2f4ac36d8e2b4cc1aa71df3dd84ff8efbe3bfb97ac41242fbcfc053c67434f46",
+                "sha256:3170c9399da12c9dc66366e9d14da8bf7147e1e9d9ea566067bbce7bb74bd9c2",
+                "sha256:3b1613dd5aee995ec6d4c69f00378bbd07614702a315a2cf6c1d21461fe17c23",
+                "sha256:3bb3d25a8e6c0aedd251753a79ae98a093c7e7b471faa3aa9a93a81431987ace",
+                "sha256:3bb7fda7260735efe66d5107fb7e6af6a7c04c7fce9b2514e04b7a74b06bf5dd",
+                "sha256:41b25eaa7d15909cf3ac4c96088c1f266a9a93ec44f87f1d13d4a0e86c81b982",
+                "sha256:45de3f87179c1823e6d9e32156fb14c1927fcc9aba21433f088fdfb555b77c10",
+                "sha256:46fb8c61d794b78ec7134a715a3e564aafc8f6b5e338417cb19fe9f57a5a9bf2",
+                "sha256:48021783bdf96e3d6de03a6e39a1171ed5bd7e8bb93fc84cc649d11490f87cea",
+                "sha256:4957669ef390f0e6719db3613ab3a7631e68424604a7b448f079bee145da6e09",
+                "sha256:5e86d77b090dbddbe78867a0275cb4df08ea195e660f1f7f13435a4649e954e5",
+                "sha256:6339d047dab2780cc6220f46306628e04d9750f02f983ddb37439ca47ced7149",
+                "sha256:681eb3d7e02e3c3655d1b16059fbfb605ac464c834a0c629048a30fad2b27489",
+                "sha256:6c409c0deba34f147f77efaa67b8e4bb83d2f11c8806405f76397ae5b8c0d1c9",
+                "sha256:7095f6fbfaa55defb6b733cfeb14efaae7a29f0b59d8cf213be4e7ca0b857b80",
+                "sha256:70c610f6cbe4b9fce272c407dd9d07e33e6bf7b4aa1b7ffb6f6ded8e634e3592",
+                "sha256:72814c01533f51d68702802d74f77ea026b5ec52793c791e2da806a3844a46c3",
+                "sha256:7a4826ad2bd6b07ca615c74ab91f32f6c96d08f6fcc3902ceeedaec8cdc3bcd6",
+                "sha256:7c70087bfee18a42b4040bb9ec1ca15a08242cf5867c58726530bdf3945672ed",
+                "sha256:855eafa5d5a2034b4621c74925d89c5efef61418570e5ef9b37717d9c796419c",
+                "sha256:8700f06d0ce6f128de3ccdbc1acaea1ee264d2caa9ca05daaf492fde7c2a7200",
+                "sha256:89f1b185a01fe560bc8ae5f619e924407efca2191b56ce749ec84982fc59a32a",
+                "sha256:8b2c760cfc7042b27ebdb4a43a4453bd829a5742503599144d54a032c5dc7e9e",
+                "sha256:8c2f5e83493748286002f9369f3e6607c565a6a90425a3a1fef5ae32a36d749d",
+                "sha256:8e098148dd37b4ce3baca71fb394c81dc5d9c7728c95df695d2dca218edf40e6",
+                "sha256:94aea8eff76ee6d1cdacb07dd2123a68283cb5569e0250feab1240058f53b623",
+                "sha256:95eb302ff792e12aba9a8b8f8474ab229a83c103d74a750ec0bd1c1eea32e669",
+                "sha256:9bd9b3b31adcb054116447ea22caa61a285d92e94d710aa5ec97992ff5eb7cf3",
+                "sha256:9e608aafdb55eb9f255034709e20d5a83b6d60c054df0802fa9c9883d0a937aa",
+                "sha256:a103b3a7069b62f5d4890ae1b8f0597618f628b286b03d4bc9195230b154bfa9",
+                "sha256:a386ebe437176aab38c041de1260cd3ea459c6ce5263594399880bbc398225b2",
+                "sha256:a38856a971c602f98472050165cea2cdc97709240373041b69030be15047691f",
+                "sha256:a401b4598e5d3f4a9a811f3daf42ee2291790c7f9d74b18d75d6e21dda98a1a1",
+                "sha256:a7647ebdfb9682b7bb97e2a5e7cb6ae735b1c25008a70b906aecca294ee96cf4",
+                "sha256:aaf63899c94de41fe3cf934601b0f7ccb6b428c6e4eeb80da72c58eab077b19a",
+                "sha256:b0dac0ff919ba34d4df1b6131f59ce95b08b9065233446be7e459f95554c0dc8",
+                "sha256:baacc6aee0b2ef6f3d308e197b5d7a81c0e70b06beae1f1fcacffdbd124fe0e3",
+                "sha256:bf420121d4c8dce6b889f0e8e4ec0ca34b7f40186203f06a946fa0276ba54029",
+                "sha256:c04a46716adde8d927adb9457bbe39cf473e1e2c2f5d0a16ceb837e5d841ad4f",
+                "sha256:c0b21078a4b56965e2b12f247467b234734491897e99c1d51cee628da9786959",
+                "sha256:c1c76a1743432b4b60ab3358c937a3fe1341c828ae6194108a94c69028247f22",
+                "sha256:c4983bf937209c57240cff65906b18bb35e64ae872da6a0db937d7b4af845dd7",
+                "sha256:c4fb39a81950ec280984b3a44f5bd12819953dc5fa3a7e6fa7a80db5ee853952",
+                "sha256:c57921cda3a80d0f2b8aec7e25c8aa14479ea92b5b51b6876d975d925a2ea346",
+                "sha256:c8063cf17b19661471ecbdb3df1c84f24ad2e389e326ccaf89e3fb2484d8dd7e",
+                "sha256:ccd16eb18a849fd8dcb23e23380e2f0a354e8daa0c984b8a732d9cfaba3a776d",
+                "sha256:cd6dbe0238f7743d0efe563ab46294f54f9bc8f4b9bcf57c3c666cc5bc9d1299",
+                "sha256:d62e51710986674142526ab9f78663ca2b0726066ae26b78b22e0f5e571238dd",
+                "sha256:db901e2ac34c931d73054d9797383d0f8009991e723dab15109740a63e7f902a",
+                "sha256:e03b8895a6990c9ab2cdcd0f2fe44088ca1c65ae592b8f795c3294af00a461c3",
+                "sha256:e1c8a2f4c69e08e89632defbfabec2feb8a8d99edc9f89ce33c4b9e36ab63037",
+                "sha256:e4b749b9cc6ee664a3300bb3a273c1ca8068c46be705b6c31cf5d276f8628a94",
+                "sha256:e6a5bf2cba5ae1bb80b154ed68a3cfa2fa00fde979a7f50d6598d3e17d9ac20c",
+                "sha256:e857a2232ba53ae940d3456f7533ce6ca98b81917d47adc3c7fd55dad8fab858",
+                "sha256:ee4006268ed33370957f55bf2e6f4d263eaf4dc3cfc473d1d90baff6ed36ce4a",
+                "sha256:eef9df1eefada2c09a5e7a40991b9fc6ac6ef20b1372abd48d2794a316dc0449",
+                "sha256:f058f6963fd82eb143c692cecdc89e075fa0828db2e5b291070485390b2f1c9c",
+                "sha256:f25c229a6ba38a35ae6e25ca1264621cc25d4d38dca2942a7fce0b67a4efe918",
+                "sha256:f2a1d0fd4242bd8643ce6f98927cf9c04540af6efa92323e9d3124f57727bfc1",
+                "sha256:f7560358a6811e52e9c4d142d497f1a6e10103d3a6881f18d04dbce3729c0e2c",
+                "sha256:f779d3ad205f108d14e99bb3859aa7dd8e9c68874617c72354d7ecaec2a054ac",
+                "sha256:f87f746ee241d30d6ed93969de31e5ffd09a2961a051e60ae6bddde9ec3583aa"
             ],
-            "markers": "python_version >= '3'",
-            "version": "==2.0.12"
+            "markers": "python_full_version >= '3.7.0'",
+            "version": "==3.2.0"
         },
         "click": {
             "hashes": [
-                "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e",
-                "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"
+                "sha256:2739815aaa5d2c986a88f1e9230c55e17f0caad3d958a5e13ad0797c166db9e3",
+                "sha256:b97d0c74955da062a7d4ef92fadb583806a585b2ea81958a81bd72726cbb8e37"
             ],
             "index": "pypi",
-            "version": "==8.1.3"
+            "version": "==8.1.4"
         },
         "idna": {
             "hashes": [
                 "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
-            "markers": "python_version >= '3'",
+            "markers": "python_version >= '3.5'",
             "version": "==3.4"
         },
         "requests": {
             "hashes": [
-                "sha256:68d7c56fd5a8999887728ef304a6d12edc7be74f1cfa47714fc8b414525c9a61",
-                "sha256:f22fa1e554c9ddfd16e6e41ac79759e17be9e492b3587efa038054674760e72d"
+                "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f",
+                "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"
             ],
             "index": "pypi",
-            "version": "==2.27.1"
+            "version": "==2.31.0"
         },
         "urllib3": {
             "hashes": [
-                "sha256:076907bf8fd355cde77728471316625a4d2f7e713c125f51953bb5b3eecf4f72",
-                "sha256:75edcdc2f7d85b137124a6c3c9fc3933cdeaa12ecb9a6a959f22797a0feca7e1"
+                "sha256:48e7fafa40319d358848e1bc6809b208340fafe2096f1725d05d67443d0483d1",
+                "sha256:bee28b5e56addb8226c96f7f13ac28cb4c301dd5ea8a6ca179c0b9835e032825"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==1.26.14"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.0.3"
         }
     },
     "develop": {
         "alabaster": {
             "hashes": [
                 "sha256:1ee19aca801bbabb5ba3f5f258e4422dfa86f82f3e9cefb0859b283cdd7f62a3",
                 "sha256:a27a4a084d5e690e16e01e03ad2b2e552c61a65469419b907243193de1a84ae2"
@@ -88,19 +161,19 @@
                 "sha256:33c16e3353dbd13028ab4799a0f89a83f113405c766e9c122df8a06f5b85b3f4"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==6.0.0"
         },
         "certifi": {
             "hashes": [
-                "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
-                "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
+                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
+                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2022.12.7"
+            "version": "==2023.5.7"
         },
         "cffi": {
             "hashes": [
                 "sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5",
                 "sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef",
                 "sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104",
                 "sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426",
@@ -173,119 +246,188 @@
                 "sha256:f5a830efb9ce7a445376bb66ec94c638a9787422f96264c98edc6bdeed8ab736"
             ],
             "markers": "python_full_version >= '3.6.1'",
             "version": "==3.3.1"
         },
         "charset-normalizer": {
             "hashes": [
-                "sha256:2857e29ff0d34db842cd7ca3230549d1a697f96ee6d3fb071cfa6c7393832597",
-                "sha256:6881edbebdb17b39b4eaaa821b438bf6eddffb4468cf344f09f89def34a8b1df"
+                "sha256:04e57ab9fbf9607b77f7d057974694b4f6b142da9ed4a199859d9d4d5c63fe96",
+                "sha256:09393e1b2a9461950b1c9a45d5fd251dc7c6f228acab64da1c9c0165d9c7765c",
+                "sha256:0b87549028f680ca955556e3bd57013ab47474c3124dc069faa0b6545b6c9710",
+                "sha256:1000fba1057b92a65daec275aec30586c3de2401ccdcd41f8a5c1e2c87078706",
+                "sha256:1249cbbf3d3b04902ff081ffbb33ce3377fa6e4c7356f759f3cd076cc138d020",
+                "sha256:1920d4ff15ce893210c1f0c0e9d19bfbecb7983c76b33f046c13a8ffbd570252",
+                "sha256:193cbc708ea3aca45e7221ae58f0fd63f933753a9bfb498a3b474878f12caaad",
+                "sha256:1a100c6d595a7f316f1b6f01d20815d916e75ff98c27a01ae817439ea7726329",
+                "sha256:1f30b48dd7fa1474554b0b0f3fdfdd4c13b5c737a3c6284d3cdc424ec0ffff3a",
+                "sha256:203f0c8871d5a7987be20c72442488a0b8cfd0f43b7973771640fc593f56321f",
+                "sha256:246de67b99b6851627d945db38147d1b209a899311b1305dd84916f2b88526c6",
+                "sha256:2dee8e57f052ef5353cf608e0b4c871aee320dd1b87d351c28764fc0ca55f9f4",
+                "sha256:2efb1bd13885392adfda4614c33d3b68dee4921fd0ac1d3988f8cbb7d589e72a",
+                "sha256:2f4ac36d8e2b4cc1aa71df3dd84ff8efbe3bfb97ac41242fbcfc053c67434f46",
+                "sha256:3170c9399da12c9dc66366e9d14da8bf7147e1e9d9ea566067bbce7bb74bd9c2",
+                "sha256:3b1613dd5aee995ec6d4c69f00378bbd07614702a315a2cf6c1d21461fe17c23",
+                "sha256:3bb3d25a8e6c0aedd251753a79ae98a093c7e7b471faa3aa9a93a81431987ace",
+                "sha256:3bb7fda7260735efe66d5107fb7e6af6a7c04c7fce9b2514e04b7a74b06bf5dd",
+                "sha256:41b25eaa7d15909cf3ac4c96088c1f266a9a93ec44f87f1d13d4a0e86c81b982",
+                "sha256:45de3f87179c1823e6d9e32156fb14c1927fcc9aba21433f088fdfb555b77c10",
+                "sha256:46fb8c61d794b78ec7134a715a3e564aafc8f6b5e338417cb19fe9f57a5a9bf2",
+                "sha256:48021783bdf96e3d6de03a6e39a1171ed5bd7e8bb93fc84cc649d11490f87cea",
+                "sha256:4957669ef390f0e6719db3613ab3a7631e68424604a7b448f079bee145da6e09",
+                "sha256:5e86d77b090dbddbe78867a0275cb4df08ea195e660f1f7f13435a4649e954e5",
+                "sha256:6339d047dab2780cc6220f46306628e04d9750f02f983ddb37439ca47ced7149",
+                "sha256:681eb3d7e02e3c3655d1b16059fbfb605ac464c834a0c629048a30fad2b27489",
+                "sha256:6c409c0deba34f147f77efaa67b8e4bb83d2f11c8806405f76397ae5b8c0d1c9",
+                "sha256:7095f6fbfaa55defb6b733cfeb14efaae7a29f0b59d8cf213be4e7ca0b857b80",
+                "sha256:70c610f6cbe4b9fce272c407dd9d07e33e6bf7b4aa1b7ffb6f6ded8e634e3592",
+                "sha256:72814c01533f51d68702802d74f77ea026b5ec52793c791e2da806a3844a46c3",
+                "sha256:7a4826ad2bd6b07ca615c74ab91f32f6c96d08f6fcc3902ceeedaec8cdc3bcd6",
+                "sha256:7c70087bfee18a42b4040bb9ec1ca15a08242cf5867c58726530bdf3945672ed",
+                "sha256:855eafa5d5a2034b4621c74925d89c5efef61418570e5ef9b37717d9c796419c",
+                "sha256:8700f06d0ce6f128de3ccdbc1acaea1ee264d2caa9ca05daaf492fde7c2a7200",
+                "sha256:89f1b185a01fe560bc8ae5f619e924407efca2191b56ce749ec84982fc59a32a",
+                "sha256:8b2c760cfc7042b27ebdb4a43a4453bd829a5742503599144d54a032c5dc7e9e",
+                "sha256:8c2f5e83493748286002f9369f3e6607c565a6a90425a3a1fef5ae32a36d749d",
+                "sha256:8e098148dd37b4ce3baca71fb394c81dc5d9c7728c95df695d2dca218edf40e6",
+                "sha256:94aea8eff76ee6d1cdacb07dd2123a68283cb5569e0250feab1240058f53b623",
+                "sha256:95eb302ff792e12aba9a8b8f8474ab229a83c103d74a750ec0bd1c1eea32e669",
+                "sha256:9bd9b3b31adcb054116447ea22caa61a285d92e94d710aa5ec97992ff5eb7cf3",
+                "sha256:9e608aafdb55eb9f255034709e20d5a83b6d60c054df0802fa9c9883d0a937aa",
+                "sha256:a103b3a7069b62f5d4890ae1b8f0597618f628b286b03d4bc9195230b154bfa9",
+                "sha256:a386ebe437176aab38c041de1260cd3ea459c6ce5263594399880bbc398225b2",
+                "sha256:a38856a971c602f98472050165cea2cdc97709240373041b69030be15047691f",
+                "sha256:a401b4598e5d3f4a9a811f3daf42ee2291790c7f9d74b18d75d6e21dda98a1a1",
+                "sha256:a7647ebdfb9682b7bb97e2a5e7cb6ae735b1c25008a70b906aecca294ee96cf4",
+                "sha256:aaf63899c94de41fe3cf934601b0f7ccb6b428c6e4eeb80da72c58eab077b19a",
+                "sha256:b0dac0ff919ba34d4df1b6131f59ce95b08b9065233446be7e459f95554c0dc8",
+                "sha256:baacc6aee0b2ef6f3d308e197b5d7a81c0e70b06beae1f1fcacffdbd124fe0e3",
+                "sha256:bf420121d4c8dce6b889f0e8e4ec0ca34b7f40186203f06a946fa0276ba54029",
+                "sha256:c04a46716adde8d927adb9457bbe39cf473e1e2c2f5d0a16ceb837e5d841ad4f",
+                "sha256:c0b21078a4b56965e2b12f247467b234734491897e99c1d51cee628da9786959",
+                "sha256:c1c76a1743432b4b60ab3358c937a3fe1341c828ae6194108a94c69028247f22",
+                "sha256:c4983bf937209c57240cff65906b18bb35e64ae872da6a0db937d7b4af845dd7",
+                "sha256:c4fb39a81950ec280984b3a44f5bd12819953dc5fa3a7e6fa7a80db5ee853952",
+                "sha256:c57921cda3a80d0f2b8aec7e25c8aa14479ea92b5b51b6876d975d925a2ea346",
+                "sha256:c8063cf17b19661471ecbdb3df1c84f24ad2e389e326ccaf89e3fb2484d8dd7e",
+                "sha256:ccd16eb18a849fd8dcb23e23380e2f0a354e8daa0c984b8a732d9cfaba3a776d",
+                "sha256:cd6dbe0238f7743d0efe563ab46294f54f9bc8f4b9bcf57c3c666cc5bc9d1299",
+                "sha256:d62e51710986674142526ab9f78663ca2b0726066ae26b78b22e0f5e571238dd",
+                "sha256:db901e2ac34c931d73054d9797383d0f8009991e723dab15109740a63e7f902a",
+                "sha256:e03b8895a6990c9ab2cdcd0f2fe44088ca1c65ae592b8f795c3294af00a461c3",
+                "sha256:e1c8a2f4c69e08e89632defbfabec2feb8a8d99edc9f89ce33c4b9e36ab63037",
+                "sha256:e4b749b9cc6ee664a3300bb3a273c1ca8068c46be705b6c31cf5d276f8628a94",
+                "sha256:e6a5bf2cba5ae1bb80b154ed68a3cfa2fa00fde979a7f50d6598d3e17d9ac20c",
+                "sha256:e857a2232ba53ae940d3456f7533ce6ca98b81917d47adc3c7fd55dad8fab858",
+                "sha256:ee4006268ed33370957f55bf2e6f4d263eaf4dc3cfc473d1d90baff6ed36ce4a",
+                "sha256:eef9df1eefada2c09a5e7a40991b9fc6ac6ef20b1372abd48d2794a316dc0449",
+                "sha256:f058f6963fd82eb143c692cecdc89e075fa0828db2e5b291070485390b2f1c9c",
+                "sha256:f25c229a6ba38a35ae6e25ca1264621cc25d4d38dca2942a7fce0b67a4efe918",
+                "sha256:f2a1d0fd4242bd8643ce6f98927cf9c04540af6efa92323e9d3124f57727bfc1",
+                "sha256:f7560358a6811e52e9c4d142d497f1a6e10103d3a6881f18d04dbce3729c0e2c",
+                "sha256:f779d3ad205f108d14e99bb3859aa7dd8e9c68874617c72354d7ecaec2a054ac",
+                "sha256:f87f746ee241d30d6ed93969de31e5ffd09a2961a051e60ae6bddde9ec3583aa"
             ],
-            "markers": "python_version >= '3'",
-            "version": "==2.0.12"
+            "markers": "python_full_version >= '3.7.0'",
+            "version": "==3.2.0"
         },
         "cryptography": {
             "hashes": [
-                "sha256:0f8da300b5c8af9f98111ffd512910bc792b4c77392a9523624680f7956a99d4",
-                "sha256:35f7c7d015d474f4011e859e93e789c87d21f6f4880ebdc29896a60403328f1f",
-                "sha256:4789d1e3e257965e960232345002262ede4d094d1a19f4d3b52e48d4d8f3b885",
-                "sha256:5aa67414fcdfa22cf052e640cb5ddc461924a045cacf325cd164e65312d99502",
-                "sha256:5d2d8b87a490bfcd407ed9d49093793d0f75198a35e6eb1a923ce1ee86c62b41",
-                "sha256:6687ef6d0a6497e2b58e7c5b852b53f62142cfa7cd1555795758934da363a965",
-                "sha256:6f8ba7f0328b79f08bdacc3e4e66fb4d7aab0c3584e0bd41328dce5262e26b2e",
-                "sha256:706843b48f9a3f9b9911979761c91541e3d90db1ca905fd63fee540a217698bc",
-                "sha256:807ce09d4434881ca3a7594733669bd834f5b2c6d5c7e36f8c00f691887042ad",
-                "sha256:83e17b26de248c33f3acffb922748151d71827d6021d98c70e6c1a25ddd78505",
-                "sha256:96f1157a7c08b5b189b16b47bc9db2332269d6680a196341bf30046330d15388",
-                "sha256:aec5a6c9864be7df2240c382740fcf3b96928c46604eaa7f3091f58b878c0bb6",
-                "sha256:b0afd054cd42f3d213bf82c629efb1ee5f22eba35bf0eec88ea9ea7304f511a2",
-                "sha256:c5caeb8188c24888c90b5108a441c106f7faa4c4c075a2bcae438c6e8ca73cef",
-                "sha256:ced4e447ae29ca194449a3f1ce132ded8fcab06971ef5f618605aacaa612beac",
-                "sha256:d1f6198ee6d9148405e49887803907fe8962a23e6c6f83ea7d98f1c0de375695",
-                "sha256:e124352fd3db36a9d4a21c1aa27fd5d051e621845cb87fb851c08f4f75ce8be6",
-                "sha256:e422abdec8b5fa8462aa016786680720d78bdce7a30c652b7fadf83a4ba35336",
-                "sha256:ef8b72fa70b348724ff1218267e7f7375b8de4e8194d1636ee60510aae104cd0",
-                "sha256:f0c64d1bd842ca2633e74a1a28033d139368ad959872533b1bab8c80e8240a0c",
-                "sha256:f24077a3b5298a5a06a8e0536e3ea9ec60e4c7ac486755e5fb6e6ea9b3500106",
-                "sha256:fdd188c8a6ef8769f148f88f859884507b954cc64db6b52f66ef199bb9ad660a",
-                "sha256:fe913f20024eb2cb2f323e42a64bdf2911bb9738a15dba7d3cce48151034e3a8"
+                "sha256:059e348f9a3c1950937e1b5d7ba1f8e968508ab181e75fc32b879452f08356db",
+                "sha256:1a5472d40c8f8e91ff7a3d8ac6dfa363d8e3138b961529c996f3e2df0c7a411a",
+                "sha256:1a8e6c2de6fbbcc5e14fd27fb24414507cb3333198ea9ab1258d916f00bc3039",
+                "sha256:1fee5aacc7367487b4e22484d3c7e547992ed726d14864ee33c0176ae43b0d7c",
+                "sha256:5d092fdfedaec4cbbffbf98cddc915ba145313a6fdaab83c6e67f4e6c218e6f3",
+                "sha256:5f0ff6e18d13a3de56f609dd1fd11470918f770c6bd5d00d632076c727d35485",
+                "sha256:7bfc55a5eae8b86a287747053140ba221afc65eb06207bedf6e019b8934b477c",
+                "sha256:7fa01527046ca5facdf973eef2535a27fec4cb651e4daec4d043ef63f6ecd4ca",
+                "sha256:8dde71c4169ec5ccc1087bb7521d54251c016f126f922ab2dfe6649170a3b8c5",
+                "sha256:8f4ab7021127a9b4323537300a2acfb450124b2def3756f64dc3a3d2160ee4b5",
+                "sha256:948224d76c4b6457349d47c0c98657557f429b4e93057cf5a2f71d603e2fc3a3",
+                "sha256:9a6c7a3c87d595608a39980ebaa04d5a37f94024c9f24eb7d10262b92f739ddb",
+                "sha256:b46e37db3cc267b4dea1f56da7346c9727e1209aa98487179ee8ebed09d21e43",
+                "sha256:b4ceb5324b998ce2003bc17d519080b4ec8d5b7b70794cbd2836101406a9be31",
+                "sha256:cb33ccf15e89f7ed89b235cff9d49e2e62c6c981a6061c9c8bb47ed7951190bc",
+                "sha256:d198820aba55660b4d74f7b5fd1f17db3aa5eb3e6893b0a41b75e84e4f9e0e4b",
+                "sha256:d34579085401d3f49762d2f7d6634d6b6c2ae1242202e860f4d26b046e3a1006",
+                "sha256:eb8163f5e549a22888c18b0d53d6bb62a20510060a22fd5a995ec8a05268df8a",
+                "sha256:f73bff05db2a3e5974a6fd248af2566134d8981fd7ab012e5dd4ddb1d9a70699"
             ],
-            "index": "pypi",
-            "version": "==39.0.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==41.0.1"
         },
         "distlib": {
             "hashes": [
                 "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
                 "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
             ],
             "version": "==0.3.6"
         },
         "docutils": {
             "hashes": [
-                "sha256:23010f129180089fbcd3bc08cfefccb3b890b0050e1ca00c867036e9d161b98c",
-                "sha256:679987caf361a7539d76e584cbeddc311e3aee937877c87346f31debc63e9d06"
+                "sha256:96f387a2c5562db4476f09f13bbab2192e764cac08ebbf3a34a95d9b1e4a59d6",
+                "sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-            "version": "==0.18.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==0.20.1"
         },
         "filelock": {
             "hashes": [
-                "sha256:7b319f24340b51f55a2bf7a12ac0755a9b03e718311dac567a0f4f7fabd2f5de",
-                "sha256:f58d535af89bb9ad5cd4df046f741f8553a418c01a7856bf0d173bbc9f6bd16d"
+                "sha256:002740518d8aa59a26b0c76e10fb8c6e15eae825d34b6fdf670333fd7b938d81",
+                "sha256:cbb791cdea2a72f23da6ac5b5269ab0a0d161e9ef0100e653b69049a7706d1ec"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.9.0"
+            "version": "==3.12.2"
         },
         "flake8": {
             "hashes": [
-                "sha256:479b1304f72536a55948cb40a32dce8bb0ffe3501e26eaf292c7e60eb5e0428d",
-                "sha256:806e034dda44114815e23c16ef92f95c91e4c71100ff52813adf7132a6ad870d"
+                "sha256:3833794e27ff64ea4e9cf5d410082a8b97ff1a06c16aa3d2027339cd0f1195c7",
+                "sha256:c61007e76655af75e6785a931f452915b371dc48f56efd765247c8fe68f2b181"
             ],
             "index": "pypi",
-            "version": "==4.0.1"
+            "version": "==6.0.0"
         },
         "identify": {
             "hashes": [
-                "sha256:89e144fa560cc4cffb6ef2ab5e9fb18ed9f9b3cb054384bab4b95c12f6c309fe",
-                "sha256:93aac7ecf2f6abf879b8f29a8002d3c6de7086b8c28d88e1ad15045a15ab63f9"
+                "sha256:0aac67d5b4812498056d28a9a512a483f5085cc28640b02b258a59dac34301d4",
+                "sha256:986dbfb38b1140e763e413e6feb44cd731faf72d1909543178aa79b0e258265d"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.5.18"
+            "version": "==2.5.24"
         },
         "idna": {
             "hashes": [
                 "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
-            "markers": "python_version >= '3'",
+            "markers": "python_version >= '3.5'",
             "version": "==3.4"
         },
         "imagesize": {
             "hashes": [
                 "sha256:0d8d18d08f840c19d0ee7ca1fd82490fdc3729b7ac93f49870406ddde8ef8d8b",
                 "sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.4.1"
         },
         "importlib-metadata": {
             "hashes": [
-                "sha256:7efb448ec9a5e313a57655d35aa54cd3e01b7e1fbcf72dce1bf06119420f5bad",
-                "sha256:e354bedeb60efa6affdcc8ae121b73544a7aa74156d047311948f6d711cd378d"
+                "sha256:3ebb78df84a805d7698245025b975d9d67053cd94c79245ba4b3eb694abe68bb",
+                "sha256:dbace7892d8c0c4ac1ad096662232f831d4e64f4c4545bd53016a3e9d4654743"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==6.0.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==6.8.0"
         },
         "jaraco.classes": {
             "hashes": [
-                "sha256:2353de3288bc6b82120752201c6b1c1a14b058267fa424ed5ce5984e3b922158",
-                "sha256:89559fa5c1d3c34eff6f631ad80bb21f378dbcbb35dd161fd2c6b93f5be2f98a"
+                "sha256:10afa92b6743f25c0cf5f37c6bb6e18e2c5bb84a16527ccfc0040ea377e7aaeb",
+                "sha256:c063dd08e89217cee02c8d5e5ec560f2c8ce6cdc2fcdc2e68f7b2e5547ed3621"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==3.2.3"
+            "markers": "python_version >= '3.8'",
+            "version": "==3.3.0"
         },
         "jeepney": {
             "hashes": [
                 "sha256:5efe48d255973902f6badc3ce55e2aa6c5c3b3bc642059ef3a91247bcfcc5806",
                 "sha256:c0a454ad016ca575060802ee4d590dd912e35c122fa04e70306de3d076cce755"
             ],
             "markers": "sys_platform == 'linux'",
@@ -297,90 +439,91 @@
                 "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==3.1.2"
         },
         "keyring": {
             "hashes": [
-                "sha256:771ed2a91909389ed6148631de678f82ddc73737d85a927f382a8a1b157898cd",
-                "sha256:ba2e15a9b35e21908d0aaf4e0a47acc52d6ae33444df0da2b49d41a46ef6d678"
+                "sha256:4901caaf597bfd3bbd78c9a0c7c4c29fcd8310dab2cffefe749e916b6527acd6",
+                "sha256:ca0746a19ec421219f4d713f848fa297a661a8a8c1504867e55bfb5e09091509"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==23.13.1"
+            "markers": "python_version >= '3.8'",
+            "version": "==24.2.0"
         },
         "markdown-it-py": {
             "hashes": [
-                "sha256:5a35f8d1870171d9acc47b99612dc146129b631baf04970128b568f190d0cc30",
-                "sha256:7c9a5e412688bc771c67432cbfebcdd686c93ce6484913dccf06cb5a0bea35a1"
+                "sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1",
+                "sha256:e3f60a94fa066dc52ec76661e37c851cb232d92f9886b15cb560aaada2df8feb"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==2.2.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==3.0.0"
         },
         "markupsafe": {
             "hashes": [
-                "sha256:0576fe974b40a400449768941d5d0858cc624e3249dfd1e0c33674e5c7ca7aed",
-                "sha256:085fd3201e7b12809f9e6e9bc1e5c96a368c8523fad5afb02afe3c051ae4afcc",
-                "sha256:090376d812fb6ac5f171e5938e82e7f2d7adc2b629101cec0db8b267815c85e2",
-                "sha256:0b462104ba25f1ac006fdab8b6a01ebbfbce9ed37fd37fd4acd70c67c973e460",
-                "sha256:137678c63c977754abe9086a3ec011e8fd985ab90631145dfb9294ad09c102a7",
-                "sha256:1bea30e9bf331f3fef67e0a3877b2288593c98a21ccb2cf29b74c581a4eb3af0",
-                "sha256:22152d00bf4a9c7c83960521fc558f55a1adbc0631fbb00a9471e097b19d72e1",
-                "sha256:22731d79ed2eb25059ae3df1dfc9cb1546691cc41f4e3130fe6bfbc3ecbbecfa",
-                "sha256:2298c859cfc5463f1b64bd55cb3e602528db6fa0f3cfd568d3605c50678f8f03",
-                "sha256:28057e985dace2f478e042eaa15606c7efccb700797660629da387eb289b9323",
-                "sha256:2e7821bffe00aa6bd07a23913b7f4e01328c3d5cc0b40b36c0bd81d362faeb65",
-                "sha256:2ec4f2d48ae59bbb9d1f9d7efb9236ab81429a764dedca114f5fdabbc3788013",
-                "sha256:340bea174e9761308703ae988e982005aedf427de816d1afe98147668cc03036",
-                "sha256:40627dcf047dadb22cd25ea7ecfe9cbf3bbbad0482ee5920b582f3809c97654f",
-                "sha256:40dfd3fefbef579ee058f139733ac336312663c6706d1163b82b3003fb1925c4",
-                "sha256:4cf06cdc1dda95223e9d2d3c58d3b178aa5dacb35ee7e3bbac10e4e1faacb419",
-                "sha256:50c42830a633fa0cf9e7d27664637532791bfc31c731a87b202d2d8ac40c3ea2",
-                "sha256:55f44b440d491028addb3b88f72207d71eeebfb7b5dbf0643f7c023ae1fba619",
-                "sha256:608e7073dfa9e38a85d38474c082d4281f4ce276ac0010224eaba11e929dd53a",
-                "sha256:63ba06c9941e46fa389d389644e2d8225e0e3e5ebcc4ff1ea8506dce646f8c8a",
-                "sha256:65608c35bfb8a76763f37036547f7adfd09270fbdbf96608be2bead319728fcd",
-                "sha256:665a36ae6f8f20a4676b53224e33d456a6f5a72657d9c83c2aa00765072f31f7",
-                "sha256:6d6607f98fcf17e534162f0709aaad3ab7a96032723d8ac8750ffe17ae5a0666",
-                "sha256:7313ce6a199651c4ed9d7e4cfb4aa56fe923b1adf9af3b420ee14e6d9a73df65",
-                "sha256:7668b52e102d0ed87cb082380a7e2e1e78737ddecdde129acadb0eccc5423859",
-                "sha256:7df70907e00c970c60b9ef2938d894a9381f38e6b9db73c5be35e59d92e06625",
-                "sha256:7e007132af78ea9df29495dbf7b5824cb71648d7133cf7848a2a5dd00d36f9ff",
-                "sha256:835fb5e38fd89328e9c81067fd642b3593c33e1e17e2fdbf77f5676abb14a156",
-                "sha256:8bca7e26c1dd751236cfb0c6c72d4ad61d986e9a41bbf76cb445f69488b2a2bd",
-                "sha256:8db032bf0ce9022a8e41a22598eefc802314e81b879ae093f36ce9ddf39ab1ba",
-                "sha256:99625a92da8229df6d44335e6fcc558a5037dd0a760e11d84be2260e6f37002f",
-                "sha256:9cad97ab29dfc3f0249b483412c85c8ef4766d96cdf9dcf5a1e3caa3f3661cf1",
-                "sha256:a4abaec6ca3ad8660690236d11bfe28dfd707778e2442b45addd2f086d6ef094",
-                "sha256:a6e40afa7f45939ca356f348c8e23048e02cb109ced1eb8420961b2f40fb373a",
-                "sha256:a6f2fcca746e8d5910e18782f976489939d54a91f9411c32051b4aab2bd7c513",
-                "sha256:a806db027852538d2ad7555b203300173dd1b77ba116de92da9afbc3a3be3eed",
-                "sha256:abcabc8c2b26036d62d4c746381a6f7cf60aafcc653198ad678306986b09450d",
-                "sha256:b8526c6d437855442cdd3d87eede9c425c4445ea011ca38d937db299382e6fa3",
-                "sha256:bb06feb762bade6bf3c8b844462274db0c76acc95c52abe8dbed28ae3d44a147",
-                "sha256:c0a33bc9f02c2b17c3ea382f91b4db0e6cde90b63b296422a939886a7a80de1c",
-                "sha256:c4a549890a45f57f1ebf99c067a4ad0cb423a05544accaf2b065246827ed9603",
-                "sha256:ca244fa73f50a800cf8c3ebf7fd93149ec37f5cb9596aa8873ae2c1d23498601",
-                "sha256:cf877ab4ed6e302ec1d04952ca358b381a882fbd9d1b07cccbfd61783561f98a",
-                "sha256:d9d971ec1e79906046aa3ca266de79eac42f1dbf3612a05dc9368125952bd1a1",
-                "sha256:da25303d91526aac3672ee6d49a2f3db2d9502a4a60b55519feb1a4c7714e07d",
-                "sha256:e55e40ff0cc8cc5c07996915ad367fa47da6b3fc091fdadca7f5403239c5fec3",
-                "sha256:f03a532d7dee1bed20bc4884194a16160a2de9ffc6354b3878ec9682bb623c54",
-                "sha256:f1cd098434e83e656abf198f103a8207a8187c0fc110306691a2e94a78d0abb2",
-                "sha256:f2bfb563d0211ce16b63c7cb9395d2c682a23187f54c3d79bfec33e6705473c6",
-                "sha256:f8ffb705ffcf5ddd0e80b65ddf7bed7ee4f5a441ea7d3419e861a12eaf41af58"
+                "sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e",
+                "sha256:0a4e4a1aff6c7ac4cd55792abf96c915634c2b97e3cc1c7129578aa68ebd754e",
+                "sha256:10bbfe99883db80bdbaff2dcf681dfc6533a614f700da1287707e8a5d78a8431",
+                "sha256:134da1eca9ec0ae528110ccc9e48041e0828d79f24121a1a146161103c76e686",
+                "sha256:1577735524cdad32f9f694208aa75e422adba74f1baee7551620e43a3141f559",
+                "sha256:1b40069d487e7edb2676d3fbdb2b0829ffa2cd63a2ec26c4938b2d34391b4ecc",
+                "sha256:282c2cb35b5b673bbcadb33a585408104df04f14b2d9b01d4c345a3b92861c2c",
+                "sha256:2c1b19b3aaacc6e57b7e25710ff571c24d6c3613a45e905b1fde04d691b98ee0",
+                "sha256:2ef12179d3a291be237280175b542c07a36e7f60718296278d8593d21ca937d4",
+                "sha256:338ae27d6b8745585f87218a3f23f1512dbf52c26c28e322dbe54bcede54ccb9",
+                "sha256:3c0fae6c3be832a0a0473ac912810b2877c8cb9d76ca48de1ed31e1c68386575",
+                "sha256:3fd4abcb888d15a94f32b75d8fd18ee162ca0c064f35b11134be77050296d6ba",
+                "sha256:42de32b22b6b804f42c5d98be4f7e5e977ecdd9ee9b660fda1a3edf03b11792d",
+                "sha256:504b320cd4b7eff6f968eddf81127112db685e81f7e36e75f9f84f0df46041c3",
+                "sha256:525808b8019e36eb524b8c68acdd63a37e75714eac50e988180b169d64480a00",
+                "sha256:56d9f2ecac662ca1611d183feb03a3fa4406469dafe241673d521dd5ae92a155",
+                "sha256:5bbe06f8eeafd38e5d0a4894ffec89378b6c6a625ff57e3028921f8ff59318ac",
+                "sha256:65c1a9bcdadc6c28eecee2c119465aebff8f7a584dd719facdd9e825ec61ab52",
+                "sha256:68e78619a61ecf91e76aa3e6e8e33fc4894a2bebe93410754bd28fce0a8a4f9f",
+                "sha256:69c0f17e9f5a7afdf2cc9fb2d1ce6aabdb3bafb7f38017c0b77862bcec2bbad8",
+                "sha256:6b2b56950d93e41f33b4223ead100ea0fe11f8e6ee5f641eb753ce4b77a7042b",
+                "sha256:787003c0ddb00500e49a10f2844fac87aa6ce977b90b0feaaf9de23c22508b24",
+                "sha256:7ef3cb2ebbf91e330e3bb937efada0edd9003683db6b57bb108c4001f37a02ea",
+                "sha256:8023faf4e01efadfa183e863fefde0046de576c6f14659e8782065bcece22198",
+                "sha256:8758846a7e80910096950b67071243da3e5a20ed2546e6392603c096778d48e0",
+                "sha256:8afafd99945ead6e075b973fefa56379c5b5c53fd8937dad92c662da5d8fd5ee",
+                "sha256:8c41976a29d078bb235fea9b2ecd3da465df42a562910f9022f1a03107bd02be",
+                "sha256:8e254ae696c88d98da6555f5ace2279cf7cd5b3f52be2b5cf97feafe883b58d2",
+                "sha256:9402b03f1a1b4dc4c19845e5c749e3ab82d5078d16a2a4c2cd2df62d57bb0707",
+                "sha256:962f82a3086483f5e5f64dbad880d31038b698494799b097bc59c2edf392fce6",
+                "sha256:9dcdfd0eaf283af041973bff14a2e143b8bd64e069f4c383416ecd79a81aab58",
+                "sha256:aa7bd130efab1c280bed0f45501b7c8795f9fdbeb02e965371bbef3523627779",
+                "sha256:ab4a0df41e7c16a1392727727e7998a467472d0ad65f3ad5e6e765015df08636",
+                "sha256:ad9e82fb8f09ade1c3e1b996a6337afac2b8b9e365f926f5a61aacc71adc5b3c",
+                "sha256:af598ed32d6ae86f1b747b82783958b1a4ab8f617b06fe68795c7f026abbdcad",
+                "sha256:b076b6226fb84157e3f7c971a47ff3a679d837cf338547532ab866c57930dbee",
+                "sha256:b7ff0f54cb4ff66dd38bebd335a38e2c22c41a8ee45aa608efc890ac3e3931bc",
+                "sha256:bfce63a9e7834b12b87c64d6b155fdd9b3b96191b6bd334bf37db7ff1fe457f2",
+                "sha256:c011a4149cfbcf9f03994ec2edffcb8b1dc2d2aede7ca243746df97a5d41ce48",
+                "sha256:c9c804664ebe8f83a211cace637506669e7890fec1b4195b505c214e50dd4eb7",
+                "sha256:ca379055a47383d02a5400cb0d110cef0a776fc644cda797db0c5696cfd7e18e",
+                "sha256:cb0932dc158471523c9637e807d9bfb93e06a95cbf010f1a38b98623b929ef2b",
+                "sha256:cd0f502fe016460680cd20aaa5a76d241d6f35a1c3350c474bac1273803893fa",
+                "sha256:ceb01949af7121f9fc39f7d27f91be8546f3fb112c608bc4029aef0bab86a2a5",
+                "sha256:d080e0a5eb2529460b30190fcfcc4199bd7f827663f858a226a81bc27beaa97e",
+                "sha256:dd15ff04ffd7e05ffcb7fe79f1b98041b8ea30ae9234aed2a9168b5797c3effb",
+                "sha256:df0be2b576a7abbf737b1575f048c23fb1d769f267ec4358296f31c2479db8f9",
+                "sha256:e09031c87a1e51556fdcb46e5bd4f59dfb743061cf93c4d6831bf894f125eb57",
+                "sha256:e4dd52d80b8c83fdce44e12478ad2e85c64ea965e75d66dbeafb0a3e77308fcc",
+                "sha256:fec21693218efe39aa7f8599346e90c705afa52c5b31ae019b2e57e8f6542bb2"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.1.2"
+            "version": "==2.1.3"
         },
         "mccabe": {
             "hashes": [
-                "sha256:ab8a6258860da4b6677da4bd2fe5dc2c659cff31b3ee4f7f5d64e79735b80d42",
-                "sha256:dd8d182285a0fe56bace7f45b5e7d1a6ebcbf524e8f3bd87eb0f125271b8831f"
+                "sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325",
+                "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"
             ],
-            "version": "==0.6.1"
+            "markers": "python_version >= '3.6'",
+            "version": "==0.7.0"
         },
         "mdurl": {
             "hashes": [
                 "sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8",
                 "sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba"
             ],
             "markers": "python_version >= '3.7'",
@@ -392,82 +535,82 @@
                 "sha256:d2bc7f02446e86a68911e58ded76d6561eea00cddfb2a91e7019bbb586c799f3"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==9.1.0"
         },
         "nodeenv": {
             "hashes": [
-                "sha256:27083a7b96a25f2f5e1d8cb4b6317ee8aeda3bdd121394e5ac54e498028a042e",
-                "sha256:e0e7f7dfb85fc5394c6fe1e8fa98131a2473e04311a45afb6508f7cf1836fa2b"
+                "sha256:d51e0c37e64fbf47d017feac3145cdbb58836d7eee8c6f6d3b6880c5456227d2",
+                "sha256:df865724bb3c3adc86b3876fa209771517b0cfe596beff01a92700e0e8be4cec"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'",
-            "version": "==1.7.0"
+            "version": "==1.8.0"
         },
         "packaging": {
             "hashes": [
-                "sha256:714ac14496c3e68c99c29b00845f7a2b85f3bb6f1078fd9f72fd20f0570002b2",
-                "sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97"
+                "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
+                "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==23.0"
+            "version": "==23.1"
         },
         "pkginfo": {
             "hashes": [
                 "sha256:4b7a555a6d5a22169fcc9cf7bfd78d296b0361adad412a346c1226849af5e546",
                 "sha256:8fd5896e8718a4372f0ea9cc9d96f6417c9b986e23a4d116dda26b62cc29d046"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.9.6"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:13b08a53ed71021350c9e300d4ea8668438fb0046ab3937ac9a29913a1a1350a",
-                "sha256:accc3665857288317f32c7bebb5a8e482ba717b474f3fc1d18ca7f9214be0cef"
+                "sha256:cec7b889196b9144d088e4c57d9ceef7374f6c39694ad1577a0aab50d27ea28c",
+                "sha256:f87ca4fcff7d2b0f81c6a748a77973d7af0f4d526f98f308477c3c436c74d528"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.1.0"
+            "version": "==3.8.1"
         },
         "pre-commit": {
             "hashes": [
-                "sha256:10c62741aa5704faea2ad69cb550ca78082efe5697d6f04e5710c3c229afdd10",
-                "sha256:4233a1e38621c87d9dda9808c6606d7e7ba0e087cd56d3fe03202a01d2919615"
+                "sha256:10badb65d6a38caff29703362271d7dca483d01da88f9d7e05d0b97171c136cb",
+                "sha256:a2256f489cd913d575c145132ae196fe335da32d91a8294b7afe6622335dd023"
             ],
             "index": "pypi",
-            "version": "==2.19.0"
+            "version": "==3.3.3"
         },
         "pycodestyle": {
             "hashes": [
-                "sha256:720f8b39dde8b293825e7ff02c475f3077124006db4f440dcbc9a20b76548a20",
-                "sha256:eddd5847ef438ea1c7870ca7eb78a9d47ce0cdb4851a5523949f2601d0cbbe7f"
+                "sha256:347187bdb476329d98f695c213d7295a846d1152ff4fe9bacb8a9590b8ee7053",
+                "sha256:8a4eaf0d0495c7395bdab3589ac2db602797d76207242c17d470186815706610"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-            "version": "==2.8.0"
+            "markers": "python_version >= '3.6'",
+            "version": "==2.10.0"
         },
         "pycparser": {
             "hashes": [
                 "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9",
                 "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"
             ],
             "version": "==2.21"
         },
         "pyflakes": {
             "hashes": [
-                "sha256:05a85c2872edf37a4ed30b0cce2f6093e1d0581f8c19d7393122da7e25b2b24c",
-                "sha256:3bb3a3f256f4b7968c9c788781e4ff07dce46bdf12339dcda61053375426ee2e"
+                "sha256:ec55bf7fe21fff7f1ad2f7da62363d749e2a470500eab1b555334b67aa1ef8cf",
+                "sha256:ec8b276a6b60bd80defed25add7e439881c19e64850afd9b346283d4165fd0fd"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==2.4.0"
+            "markers": "python_version >= '3.6'",
+            "version": "==3.0.1"
         },
         "pygments": {
             "hashes": [
-                "sha256:b3ed06a9e8ac9a9aae5a6f5dbe78a8a58655d17b43b93c078f094ddc476ae297",
-                "sha256:fa7bd7bd2771287c0de303af8bfdfc731f51bd2c6a47ab69d117138893b82717"
+                "sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c",
+                "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.14.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.15.1"
         },
         "pyyaml": {
             "hashes": [
                 "sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf",
                 "sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293",
                 "sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b",
                 "sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57",
@@ -509,75 +652,75 @@
                 "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==6.0"
         },
         "readme-renderer": {
             "hashes": [
-                "sha256:cd653186dfc73055656f090f227f5cb22a046d7f71a841dfa305f55c9a513273",
-                "sha256:f67a16caedfa71eef48a31b39708637a6f4664c4394801a7b0d6432d13907343"
+                "sha256:9f77b519d96d03d7d7dce44977ba543090a14397c4f60de5b6eb5b8048110aa4",
+                "sha256:e18feb2a1e7706f2865b81ebb460056d93fb29d69daa10b223c00faa7bd9a00a"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==37.3"
+            "markers": "python_version >= '3.8'",
+            "version": "==40.0"
         },
         "requests": {
             "hashes": [
-                "sha256:68d7c56fd5a8999887728ef304a6d12edc7be74f1cfa47714fc8b414525c9a61",
-                "sha256:f22fa1e554c9ddfd16e6e41ac79759e17be9e492b3587efa038054674760e72d"
+                "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f",
+                "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"
             ],
             "index": "pypi",
-            "version": "==2.27.1"
+            "version": "==2.31.0"
         },
         "requests-toolbelt": {
             "hashes": [
-                "sha256:18565aa58116d9951ac39baa288d3adb5b3ff975c4f25eee78555d89e8f247f7",
-                "sha256:62e09f7ff5ccbda92772a29f394a49c3ad6cb181d568b1337626b2abb628a63d"
+                "sha256:7681a0a3d047012b5bdc0ee37d7f8f07ebe76ab08caeccfc3921ce23c88d5bc6",
+                "sha256:cccfdd665f0a24fcf4726e690f65639d272bb0637b9b92dfd91a5568ccf6bd06"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==0.10.1"
+            "version": "==1.0.0"
         },
         "rfc3986": {
             "hashes": [
                 "sha256:50b1502b60e289cb37883f3dfd34532b8873c7de9f49bb546641ce9cbd256ebd",
                 "sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
         },
         "rich": {
             "hashes": [
-                "sha256:91954fe80cfb7985727a467ca98a7618e5dd15178cc2da10f553b36a93859001",
-                "sha256:a104f37270bf677148d8acb07d33be1569eeee87e2d1beb286a4e9113caf6f2f"
+                "sha256:8f87bc7ee54675732fa66a05ebfe489e27264caeeff3728c945d25971b6485ec",
+                "sha256:d653d6bccede5844304c605d5aac802c7cf9621efd700b46c7ec2b51ea914898"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==13.3.2"
+            "markers": "python_full_version >= '3.7.0'",
+            "version": "==13.4.2"
         },
         "secretstorage": {
             "hashes": [
                 "sha256:2403533ef369eca6d2ba81718576c5e0f564d5cca1b58f73a8b23e7d4eeebd77",
                 "sha256:f356e6628222568e3af06f2eba8df495efa13b3b63081dafd4f7d9a7b7bc9f99"
             ],
             "markers": "sys_platform == 'linux'",
             "version": "==3.3.3"
         },
         "setuptools": {
             "hashes": [
-                "sha256:2ee892cd5f29f3373097f5a814697e397cf3ce313616df0af11231e2ad118077",
-                "sha256:b78aaa36f6b90a074c1fa651168723acbf45d14cb1196b6f02c0fd07f17623b2"
+                "sha256:11e52c67415a381d10d6b462ced9cfb97066179f0e871399e006c4ab101fc85f",
+                "sha256:baf1fdb41c6da4cd2eae722e135500da913332ab3f2f5c7d33af9b492acb5235"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==67.6.0"
+            "version": "==68.0.0"
         },
         "setuptools-scm": {
             "hashes": [
-                "sha256:6833ac65c6ed9711a4d5d2266f8024cfa07c533a0e55f4c12f6eff280a5a9e30",
-                "sha256:acea13255093849de7ccb11af9e1fb8bde7067783450cee9ef7a93139bddf6d4"
+                "sha256:6c508345a771aad7d56ebff0e70628bf2b0ec7573762be9960214730de278f27",
+                "sha256:73988b6d848709e2af142aa48c986ea29592bbcfca5375678064708205253d8e"
             ],
             "index": "pypi",
-            "version": "==6.4.2"
+            "version": "==7.1.0"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
@@ -588,19 +731,19 @@
                 "sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1",
                 "sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a"
             ],
             "version": "==2.2.0"
         },
         "sphinx": {
             "hashes": [
-                "sha256:464d9c1bd5613bcebe76b46658763f3f3dbb184da7406e632a84596d3cd8ee90",
-                "sha256:af248b21e3282f847ff20feebe7a1985fb34773cbe3fc75bf206897f1a2199c4"
+                "sha256:60c5e04756c1709a98845ed27a2eed7a556af3993afb66e77fec48189f742616",
+                "sha256:61e025f788c5977d9412587e733733a289e2b9fdc2fef8868ddfbfc4ccfe881d"
             ],
             "index": "pypi",
-            "version": "==5.0.0"
+            "version": "==7.0.1"
         },
         "sphinxcontrib-applehelp": {
             "hashes": [
                 "sha256:29d341f67fb0f6f586b23ad80e072c8e6ad0b48417db2bde114a4c9746feb228",
                 "sha256:828f867945bbe39817c210a1abfd1bc4895c8b73fcaade56d45357a348a07d7e"
             ],
             "markers": "python_version >= '3.8'",
@@ -642,64 +785,64 @@
             "hashes": [
                 "sha256:352a9a00ae864471d3a7ead8d7d79f5fc0b57e8b3f95e9867eb9eb28999b92fd",
                 "sha256:aa5f6de5dfdf809ef505c4895e51ef5c9eac17d0f287933eb49ec495280b6952"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==1.1.5"
         },
-        "toml": {
-            "hashes": [
-                "sha256:806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b",
-                "sha256:b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f"
-            ],
-            "markers": "python_version >= '2.6' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==0.10.2"
-        },
         "tomli": {
             "hashes": [
                 "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc",
                 "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
             ],
-            "markers": "python_version >= '3.7'",
+            "markers": "python_version < '3.11'",
             "version": "==2.0.1"
         },
         "twine": {
             "hashes": [
-                "sha256:6f7496cf14a3a8903474552d5271c79c71916519edb42554f23f42a8563498a9",
-                "sha256:817aa0c0bdc02a5ebe32051e168e23c71a0608334e624c793011f120dbbc05b7"
+                "sha256:929bc3c280033347a00f847236564d1c52a3e61b1ac2516c97c48f3ceab756d8",
+                "sha256:9e102ef5fdd5a20661eb88fad46338806c3bd32cf1db729603fe3697b1bc83c8"
             ],
             "index": "pypi",
-            "version": "==4.0.0"
+            "version": "==4.0.2"
+        },
+        "typing-extensions": {
+            "hashes": [
+                "sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36",
+                "sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==4.7.1"
         },
         "urllib3": {
             "hashes": [
-                "sha256:076907bf8fd355cde77728471316625a4d2f7e713c125f51953bb5b3eecf4f72",
-                "sha256:75edcdc2f7d85b137124a6c3c9fc3933cdeaa12ecb9a6a959f22797a0feca7e1"
+                "sha256:48e7fafa40319d358848e1bc6809b208340fafe2096f1725d05d67443d0483d1",
+                "sha256:bee28b5e56addb8226c96f7f13ac28cb4c301dd5ea8a6ca179c0b9835e032825"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==1.26.14"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.0.3"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:3c22fa5a7c7aa106ced59934d2c20a2ecb7f49b4130b8bf444178a16b880fa45",
-                "sha256:a8a4b8ca1e28f864b7514a253f98c1d62b64e31e77325ba279248c65fb4fcef4"
+                "sha256:34da10f14fea9be20e0fd7f04aba9732f84e593dac291b757ce42e3368a39419",
+                "sha256:8ff19a38c1021c742148edc4f81cb43d7f8c6816d2ede2ab72af5b84c749ade1"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==20.20.0"
+            "version": "==20.23.1"
         },
         "webencodings": {
             "hashes": [
                 "sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78",
                 "sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923"
             ],
             "version": "==0.5.1"
         },
         "zipp": {
             "hashes": [
-                "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b",
-                "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"
+                "sha256:1876cb065531855bbe83b6c489dcf69ecc28f1068d8e95959fe8bbc77774c941",
+                "sha256:5dadc3ad0a1f825fe42ce1bce0f2fc5a13af2e6b2d386af5b0ff295bc0a287d3"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==3.15.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==3.16.0"
         }
     }
 }
```

### Comparing `calfire-wildfires-1.1.1/README.md` & `calfire-wildfires-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `calfire-wildfires-1.1.1/calfire_wildfires.egg-info/PKG-INFO` & `calfire-wildfires-1.1.2/calfire_wildfires.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: calfire-wildfires
-Version: 1.1.1
+Version: 1.1.2
 Summary: Download wildfires data from CalFire
 Home-page: https://palewi.re/docs/calfire-wildfires/
 Author: Ben Welsh
 Author-email: b@palewi.re
 License: MIT
 Project-URL: Maintainer, https://github.com/datadesk
 Project-URL: Source, https://github.com/datadesk/calfire-wildfires
 Project-URL: Tracker, https://github.com/datadesk/calfire-wildfires/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Califire Wildfires
 Download wildfires data from Calfire
```

### Comparing `calfire-wildfires-1.1.1/docs/Makefile` & `calfire-wildfires-1.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `calfire-wildfires-1.1.1/docs/_static/css/custom.css` & `calfire-wildfires-1.1.2/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `calfire-wildfires-1.1.1/docs/_templates/nav.html` & `calfire-wildfires-1.1.2/docs/_templates/nav.html`

 * *Files identical despite different names*

### Comparing `calfire-wildfires-1.1.1/docs/conf.py` & `calfire-wildfires-1.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `calfire-wildfires-1.1.1/docs/index.md` & `calfire-wildfires-1.1.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `calfire-wildfires-1.1.1/docs/make.bat` & `calfire-wildfires-1.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `calfire-wildfires-1.1.1/setup.py` & `calfire-wildfires-1.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,18 +54,19 @@
         [console_scripts]
         calfirewildfires=calfire_wildfires.cli:cmd
     """,
     use_scm_version={"version_scheme": version_scheme, "local_scheme": local_version},
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
     ],
     project_urls={
         "Maintainer": "https://github.com/datadesk",
         "Source": "https://github.com/datadesk/calfire-wildfires",
         "Tracker": "https://github.com/datadesk/calfire-wildfires/issues",
     },
```

