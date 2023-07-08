# Comparing `tmp/lrc_adjuster-0.1.1.tar.gz` & `tmp/lrc_adjuster-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lrc_adjuster-0.1.1.tar", max compression
+gzip compressed data, was "lrc_adjuster-0.1.2.tar", max compression
```

## Comparing `lrc_adjuster-0.1.1.tar` & `lrc_adjuster-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     1069 2023-07-08 20:16:13.033847 lrc_adjuster-0.1.1/LICENSE
--rw-r--r--   0        0        0        0 2023-07-08 21:21:47.997303 lrc_adjuster-0.1.1/lrc_adjuster/__init__.py
--rw-r--r--   0        0        0     1494 2023-07-08 20:30:47.847202 lrc_adjuster-0.1.1/lrc_adjuster/adjuster.py
--rw-r--r--   0        0        0      370 2023-07-08 21:37:00.271977 lrc_adjuster-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 lrc_adjuster-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-08 22:00:49.344916 lrc_adjuster-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1710 2023-07-08 22:00:49.348916 lrc_adjuster-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-08 22:00:49.348916 lrc_adjuster-0.1.2/lrc_adjuster/__init__.py
+-rw-r--r--   0        0        0     1494 2023-07-08 22:00:49.348916 lrc_adjuster-0.1.2/lrc_adjuster/adjuster.py
+-rw-r--r--   0        0        0      407 2023-07-08 22:00:49.348916 lrc_adjuster-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2369 1970-01-01 00:00:00.000000 lrc_adjuster-0.1.2/PKG-INFO
```

### Comparing `lrc_adjuster-0.1.1/LICENSE` & `lrc_adjuster-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lrc_adjuster-0.1.1/lrc_adjuster/adjuster.py` & `lrc_adjuster-0.1.2/lrc_adjuster/adjuster.py`

 * *Files identical despite different names*

