# Comparing `tmp/thiggle-0.0.1.tar.gz` & `tmp/thiggle-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thiggle-0.0.1.tar", last modified: Fri Jul  7 18:22:24 2023, max compression
+gzip compressed data, was "thiggle-0.0.2.tar", max compression
```

## Comparing `thiggle-0.0.1.tar` & `thiggle-0.0.2.tar`

### file list

```diff
@@ -1,49 +1,5 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 18:22:24.384685 thiggle-0.0.1/
--rw-r--r--   0 root         (0) root         (0)      327 2023-07-07 18:22:24.384685 thiggle-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9650 2023-07-07 18:22:22.000000 thiggle-0.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)       69 2023-07-07 18:22:24.384685 thiggle-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1091 2023-07-07 18:22:22.000000 thiggle-0.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 18:22:24.380685 thiggle-0.0.1/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 18:22:24.381685 thiggle-0.0.1/test/test_models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 18:22:22.000000 thiggle-0.0.1/test/test_models/__init__.py
--rw-r--r--   0 root         (0) root         (0)      517 2023-07-07 18:22:22.000000 thiggle-0.0.1/test/test_models/test_categorize_request.py
--rw-r--r--   0 root         (0) root         (0)      521 2023-07-07 18:22:22.000000 thiggle-0.0.1/test/test_models/test_categorize_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 18:22:24.381685 thiggle-0.0.1/test/test_paths/
--rw-r--r--   0 root         (0) root         (0)     1995 2023-07-07 18:22:22.000000 thiggle-0.0.1/test/test_paths/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 18:22:24.382685 thiggle-0.0.1/test/test_paths/test_v1_categorize/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 18:22:22.000000 thiggle-0.0.1/test/test_paths/test_v1_categorize/__init__.py
--rw-r--r--   0 root         (0) root         (0)      847 2023-07-07 18:22:22.000000 thiggle-0.0.1/test/test_paths/test_v1_categorize/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 18:22:24.382685 thiggle-0.0.1/thiggle/
--rw-r--r--   0 root         (0) root         (0)      659 2023-07-07 18:22:22.000000 thiggle-0.0.1/thiggle/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58436 2023-07-07 18:22:22.000000 thiggle-0.0.1/thiggle/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 18:22:24.383685 thiggle-0.0.1/thiggle/apis/
--rw-r--r--   0 root         (0) root         (0)      214 2023-07-07 18:22:22.000000 thiggle-0.0.1/thiggle/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)      330 2023-07-07 18:22:22.000000 thiggle-0.0.1/thiggle/apis/path_to_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 18:22:24.383685 thiggle-0.0.1/thiggle/apis/paths/
--rw-r--r--   0 root         (0) root         (0)      234 2023-07-07 18:22:22.000000 thiggle-0.0.1/thiggle/apis/paths/__init__.py
--rw-r--r--   0 root         (0) root         (0)      106 2023-07-07 18:22:22.000000 thiggle-0.0.1/thiggle/apis/paths/v1_categorize.py
--rw-r--r--   0 root         (0) root         (0)      306 2023-07-07 18:22:22.000000 thiggle-0.0.1/thiggle/apis/tag_to_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 18:22:24.383685 thiggle-0.0.1/thiggle/apis/tags/
--rw-r--r--   0 root         (0) root         (0)      304 2023-07-07 18:22:22.000000 thiggle-0.0.1/thiggle/apis/tags/__init__.py
--rw-r--r--   0 root         (0) root         (0)      458 2023-07-07 18:22:22.000000 thiggle-0.0.1/thiggle/apis/tags/thiggle_api.py
--rw-r--r--   0 root         (0) root         (0)    15450 2023-07-07 18:22:22.000000 thiggle-0.0.1/thiggle/configuration.py
--rw-r--r--   0 root         (0) root         (0)     4478 2023-07-07 18:22:22.000000 thiggle-0.0.1/thiggle/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 18:22:24.383685 thiggle-0.0.1/thiggle/model/
--rw-r--r--   0 root         (0) root         (0)      341 2023-07-07 18:22:22.000000 thiggle-0.0.1/thiggle/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5184 2023-07-07 18:22:21.000000 thiggle-0.0.1/thiggle/model/categorize_request.py
--rw-r--r--   0 root         (0) root         (0)     3194 2023-07-07 18:22:22.000000 thiggle-0.0.1/thiggle/model/categorize_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 18:22:24.383685 thiggle-0.0.1/thiggle/models/
--rw-r--r--   0 root         (0) root         (0)      509 2023-07-07 18:22:22.000000 thiggle-0.0.1/thiggle/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 18:22:24.383685 thiggle-0.0.1/thiggle/paths/
--rw-r--r--   0 root         (0) root         (0)      320 2023-07-07 18:22:22.000000 thiggle-0.0.1/thiggle/paths/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 18:22:24.383685 thiggle-0.0.1/thiggle/paths/v1_categorize/
--rw-r--r--   0 root         (0) root         (0)      299 2023-07-07 18:22:22.000000 thiggle-0.0.1/thiggle/paths/v1_categorize/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12229 2023-07-07 18:22:22.000000 thiggle-0.0.1/thiggle/paths/v1_categorize/post.py
--rw-r--r--   0 root         (0) root         (0)    10499 2023-07-07 18:22:22.000000 thiggle-0.0.1/thiggle/rest.py
--rw-r--r--   0 root         (0) root         (0)    97600 2023-07-07 18:22:22.000000 thiggle-0.0.1/thiggle/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 18:22:24.382685 thiggle-0.0.1/thiggle.egg-info/
--rw-r--r--   0 root         (0) root         (0)      327 2023-07-07 18:22:24.000000 thiggle-0.0.1/thiggle.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      985 2023-07-07 18:22:24.000000 thiggle-0.0.1/thiggle.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 18:22:24.000000 thiggle-0.0.1/thiggle.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      118 2023-07-07 18:22:24.000000 thiggle-0.0.1/thiggle.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-07 18:22:24.000000 thiggle-0.0.1/thiggle.egg-info/top_level.txt
+-rw-r--r--   0        0        0       17 2023-07-09 01:40:24.165796 thiggle-0.0.2/README.md
+-rw-r--r--   0        0        0     1171 2023-07-09 00:57:51.910260 thiggle-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       31 2023-07-09 01:09:38.996070 thiggle-0.0.2/thiggle/__init__.py
+-rw-r--r--   0        0        0      980 2023-07-09 02:03:04.498507 thiggle-0.0.2/thiggle/thiggle.py
+-rw-r--r--   0        0        0     1298 1970-01-01 00:00:00.000000 thiggle-0.0.2/PKG-INFO
```

