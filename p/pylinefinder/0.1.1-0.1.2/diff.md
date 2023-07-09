# Comparing `tmp/pylinefinder-0.1.1.tar.gz` & `tmp/pylinefinder-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylinefinder-0.1.1.tar", max compression
+gzip compressed data, was "pylinefinder-0.1.2.tar", max compression
```

## Comparing `pylinefinder-0.1.1.tar` & `pylinefinder-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-07-09 18:25:21.168640 pylinefinder-0.1.1/README.md
--rw-r--r--   0        0        0      559 2023-07-09 18:43:55.301359 pylinefinder-0.1.1/pylinefinder/__main__.py
--rw-r--r--   0        0        0      294 2023-07-09 18:57:54.868362 pylinefinder-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      385 1970-01-01 00:00:00.000000 pylinefinder-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-09 18:25:21.168640 pylinefinder-0.1.2/README.md
+-rw-r--r--   0        0        0      851 2023-07-09 19:14:26.710181 pylinefinder-0.1.2/pylinefinder/__main__.py
+-rw-r--r--   0        0        0      294 2023-07-09 19:14:42.946611 pylinefinder-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      385 1970-01-01 00:00:00.000000 pylinefinder-0.1.2/PKG-INFO
```

