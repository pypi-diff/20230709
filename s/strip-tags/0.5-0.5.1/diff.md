# Comparing `tmp/strip-tags-0.5.tar.gz` & `tmp/strip-tags-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strip-tags-0.5.tar", last modified: Tue Jun 27 20:28:52 2023, max compression
+gzip compressed data, was "strip-tags-0.5.1.tar", last modified: Sun Jul  9 21:53:02 2023, max compression
```

## Comparing `strip-tags-0.5.tar` & `strip-tags-0.5.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:28:52.656208 strip-tags-0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 20:28:35.000000 strip-tags-0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-06-27 20:28:52.656208 strip-tags-0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-06-27 20:28:35.000000 strip-tags-0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 20:28:52.656208 strip-tags-0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-27 20:28:35.000000 strip-tags-0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:28:52.656208 strip-tags-0.5/strip_tags/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-27 20:28:35.000000 strip-tags-0.5/strip_tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-27 20:28:35.000000 strip-tags-0.5/strip_tags/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-27 20:28:35.000000 strip-tags-0.5/strip_tags/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-06-27 20:28:35.000000 strip-tags-0.5/strip_tags/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:28:52.656208 strip-tags-0.5/strip_tags.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-06-27 20:28:52.000000 strip-tags-0.5/strip_tags.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-27 20:28:52.000000 strip-tags-0.5/strip_tags.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 20:28:52.000000 strip-tags-0.5/strip_tags.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-27 20:28:52.000000 strip-tags-0.5/strip_tags.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-27 20:28:52.000000 strip-tags-0.5/strip_tags.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-27 20:28:52.000000 strip-tags-0.5/strip_tags.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:28:52.656208 strip-tags-0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-27 20:28:35.000000 strip-tags-0.5/tests/test_strip_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:53:02.056289 strip-tags-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-09 21:52:47.000000 strip-tags-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-07-09 21:53:02.056289 strip-tags-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-07-09 21:52:47.000000 strip-tags-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 21:53:02.056289 strip-tags-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-09 21:52:47.000000 strip-tags-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:53:02.056289 strip-tags-0.5.1/strip_tags/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-09 21:52:47.000000 strip-tags-0.5.1/strip_tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-09 21:52:47.000000 strip-tags-0.5.1/strip_tags/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-09 21:52:47.000000 strip-tags-0.5.1/strip_tags/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-07-09 21:52:47.000000 strip-tags-0.5.1/strip_tags/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:53:02.056289 strip-tags-0.5.1/strip_tags.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-07-09 21:53:02.000000 strip-tags-0.5.1/strip_tags.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-09 21:53:02.000000 strip-tags-0.5.1/strip_tags.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 21:53:02.000000 strip-tags-0.5.1/strip_tags.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-09 21:53:02.000000 strip-tags-0.5.1/strip_tags.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-09 21:53:02.000000 strip-tags-0.5.1/strip_tags.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-09 21:53:02.000000 strip-tags-0.5.1/strip_tags.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:53:02.056289 strip-tags-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-09 21:52:47.000000 strip-tags-0.5.1/tests/test_strip_tags.py
```

### Comparing `strip-tags-0.5/LICENSE` & `strip-tags-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `strip-tags-0.5/PKG-INFO` & `strip-tags-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strip-tags
-Version: 0.5
+Version: 0.5.1
 Summary: Strip tags from HTML, optionally from areas identified by CSS selectors
 Home-page: https://github.com/simonw/strip-tags
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/strip-tags/issues
 Project-URL: CI, https://github.com/simonw/strip-tags/actions
 Project-URL: Changelog, https://github.com/simonw/strip-tags/releases
```

### Comparing `strip-tags-0.5/README.md` & `strip-tags-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `strip-tags-0.5/setup.py` & `strip-tags-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.5"
+VERSION = "0.5.1"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

### Comparing `strip-tags-0.5/strip_tags/cli.py` & `strip-tags-0.5.1/strip_tags/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 @click.option(
     "removes",
     "-r",
     "--remove",
     multiple=True,
     help="Remove content in these selectors",
 )
-@click.option("-i", "--input", type=click.File("r"), default="-", help="Input file")
+@click.option("-i", "--input", type=click.File("rb"), default="-", help="Input file")
 @click.option("-m", "--minify", is_flag=True, help="Minify whitespace")
 @click.option("keep_tags", "-t", "--keep-tag", multiple=True, help="Keep these <tags>")
 @click.option("--all-attrs", is_flag=True, help="Include all attributes on kept tags")
 @click.option("--first", is_flag=True, help="First element matching the selectors")
 def cli(selectors, removes, input, minify, keep_tags, all_attrs, first):
     """
     Strip tags from HTML, optionally from areas identified by CSS selectors
```

### Comparing `strip-tags-0.5/strip_tags/lib.py` & `strip-tags-0.5.1/strip_tags/lib.py`

 * *Files identical despite different names*

### Comparing `strip-tags-0.5/strip_tags.egg-info/PKG-INFO` & `strip-tags-0.5.1/strip_tags.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strip-tags
-Version: 0.5
+Version: 0.5.1
 Summary: Strip tags from HTML, optionally from areas identified by CSS selectors
 Home-page: https://github.com/simonw/strip-tags
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/strip-tags/issues
 Project-URL: CI, https://github.com/simonw/strip-tags/actions
 Project-URL: Changelog, https://github.com/simonw/strip-tags/releases
```

### Comparing `strip-tags-0.5/tests/test_strip_tags.py` & `strip-tags-0.5.1/tests/test_strip_tags.py`

 * *Files 7% similar despite different names*

```diff
@@ -75,7 +75,17 @@
         removes=removes,
         minify=minify,
         first=first,
         keep_tags=keep_tags,
         all_attrs=all_attrs,
     )
     assert result == expected
+
+
+def test_not_ut8_encoding():
+    runner = CliRunner()
+    with runner.isolated_filesystem():
+        with open("input.html", "wb") as fp:
+            fp.write("<h1>hello</h1>".encode("utf-16"))
+        result = runner.invoke(cli, ["-i", "input.html"])
+    assert result.exit_code == 0
+    assert result.output == "hello\n"
```

