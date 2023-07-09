# Comparing `tmp/searchenginepy-0.1.0.tar.gz` & `tmp/searchenginepy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchenginepy-0.1.0.tar", last modified: Sun Jul  9 15:47:08 2023, max compression
+gzip compressed data, was "searchenginepy-0.1.1.tar", last modified: Sun Jul  9 19:01:53 2023, max compression
```

## Comparing `searchenginepy-0.1.0.tar` & `searchenginepy-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 15:47:08.145646 searchenginepy-0.1.0/
--rw-rw-rw-   0        0        0     1069 2023-07-09 15:32:43.000000 searchenginepy-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      246 2023-07-09 15:47:08.145646 searchenginepy-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       74 2023-07-09 15:32:43.000000 searchenginepy-0.1.0/README.md
--rw-rw-rw-   0        0        0      111 2023-07-09 15:47:08.149173 searchenginepy-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      421 2023-07-09 15:46:36.000000 searchenginepy-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-09 15:47:08.105779 searchenginepy-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-09 15:47:08.118729 searchenginepy-0.1.0/src/searchenginepy/
--rw-rw-rw-   0        0        0        0 2023-07-09 15:37:25.000000 searchenginepy-0.1.0/src/searchenginepy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 15:47:08.142638 searchenginepy-0.1.0/src/searchenginepy.egg-info/
--rw-rw-rw-   0        0        0      246 2023-07-09 15:47:07.000000 searchenginepy-0.1.0/src/searchenginepy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-07-09 15:47:07.000000 searchenginepy-0.1.0/src/searchenginepy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 15:47:07.000000 searchenginepy-0.1.0/src/searchenginepy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-09 15:47:07.000000 searchenginepy-0.1.0/src/searchenginepy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-09 15:47:07.000000 searchenginepy-0.1.0/src/searchenginepy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-09 19:01:53.266897 searchenginepy-0.1.1/
+-rw-rw-rw-   0        0        0     1069 2023-07-09 15:32:43.000000 searchenginepy-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      791 2023-07-09 19:01:53.266897 searchenginepy-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      528 2023-07-09 18:56:35.000000 searchenginepy-0.1.1/README.md
+-rw-rw-rw-   0        0        0      111 2023-07-09 19:01:53.266897 searchenginepy-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1699 2023-07-09 18:59:06.000000 searchenginepy-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 19:01:53.227026 searchenginepy-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-09 19:01:53.241817 searchenginepy-0.1.1/src/searchenginepy/
+drwxrwxrwx   0        0        0        0 2023-07-09 19:01:53.264322 searchenginepy-0.1.1/src/searchenginepy/Brave/
+-rw-rw-rw-   0        0        0        0 2023-07-09 16:19:13.000000 searchenginepy-0.1.1/src/searchenginepy/Brave/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 19:01:53.264322 searchenginepy-0.1.1/src/searchenginepy/DuckDuckGo/
+-rw-rw-rw-   0        0        0        0 2023-07-09 16:19:24.000000 searchenginepy-0.1.1/src/searchenginepy/DuckDuckGo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 19:01:53.266897 searchenginepy-0.1.1/src/searchenginepy/Google/
+-rw-rw-rw-   0        0        0     1017 2023-07-09 18:48:11.000000 searchenginepy-0.1.1/src/searchenginepy/Google/__init__.py
+-rw-rw-rw-   0        0        0      583 2023-07-09 18:19:37.000000 searchenginepy-0.1.1/src/searchenginepy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 19:01:53.261820 searchenginepy-0.1.1/src/searchenginepy.egg-info/
+-rw-rw-rw-   0        0        0      791 2023-07-09 19:01:52.000000 searchenginepy-0.1.1/src/searchenginepy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2023-07-09 19:01:52.000000 searchenginepy-0.1.1/src/searchenginepy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 19:01:52.000000 searchenginepy-0.1.1/src/searchenginepy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-09 19:01:52.000000 searchenginepy-0.1.1/src/searchenginepy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-09 19:01:52.000000 searchenginepy-0.1.1/src/searchenginepy.egg-info/top_level.txt
```

### Comparing `searchenginepy-0.1.0/LICENSE` & `searchenginepy-0.1.1/LICENSE`

 * *Files identical despite different names*

