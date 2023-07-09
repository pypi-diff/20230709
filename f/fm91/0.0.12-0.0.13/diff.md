# Comparing `tmp/fm91-0.0.12.tar.gz` & `tmp/fm91-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fm91-0.0.12.tar", max compression
+gzip compressed data, was "fm91-0.0.13.tar", max compression
```

## Comparing `fm91-0.0.12.tar` & `fm91-0.0.13.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-07-09 06:14:10.961033 fm91-0.0.12/fm91/__init__.py
--rw-r--r--   0        0        0       48 2023-07-09 07:05:18.792985 fm91-0.0.12/fm91/__main__.py
--rw-r--r--   0        0        0    10582 2023-07-09 06:14:23.055772 fm91-0.0.12/fm91/main.py
--rw-r--r--   0        0        0      429 2023-07-09 07:05:08.504487 fm91-0.0.12/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-09 06:14:10.961033 fm91-0.0.12/README.md
--rw-r--r--   0        0        0      446 1970-01-01 00:00:00.000000 fm91-0.0.12/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-09 06:14:10.961033 fm91-0.0.13/fm91/__init__.py
+-rw-r--r--   0        0        0       48 2023-07-09 07:05:18.792985 fm91-0.0.13/fm91/__main__.py
+-rw-r--r--   0        0        0    10582 2023-07-09 06:14:23.055772 fm91-0.0.13/fm91/main.py
+-rw-r--r--   0        0        0      429 2023-07-09 07:15:56.033572 fm91-0.0.13/pyproject.toml
+-rw-r--r--   0        0        0     5312 2023-07-09 07:13:47.845484 fm91-0.0.13/README.md
+-rw-r--r--   0        0        0     5457 1970-01-01 00:00:00.000000 fm91-0.0.13/PKG-INFO
```

### Comparing `fm91-0.0.12/fm91/main.py` & `fm91-0.0.13/fm91/main.py`

 * *Files identical despite different names*

