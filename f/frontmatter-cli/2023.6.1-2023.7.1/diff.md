# Comparing `tmp/frontmatter_cli-2023.6.1.tar.gz` & `tmp/frontmatter-cli-2023.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frontmatter_cli-2023.6.1.tar", last modified: Fri Jun  9 02:31:19 2023, max compression
+gzip compressed data, was "frontmatter-cli-2023.7.1.tar", last modified: Sun Jul  9 13:41:08 2023, max compression
```

## Comparing `frontmatter_cli-2023.6.1.tar` & `frontmatter-cli-2023.7.1.tar`

### file list

```diff
@@ -1,21 +1,19 @@
-drwxr-xr-x   0 jefftriplett   (501) staff       (20)        0 2023-06-09 02:31:19.274107 frontmatter_cli-2023.6.1/
--rw-r--r--   0 jefftriplett   (501) staff       (20)       11 2023-06-09 02:13:44.000000 frontmatter_cli-2023.6.1/HISTORY.md
--rw-r--r--   0 jefftriplett   (501) staff       (20)     1513 2023-06-09 02:13:44.000000 frontmatter_cli-2023.6.1/LICENSE
--rw-r--r--   0 jefftriplett   (501) staff       (20)      134 2023-06-09 02:13:44.000000 frontmatter_cli-2023.6.1/MANIFEST.in
--rw-r--r--   0 jefftriplett   (501) staff       (20)     2652 2023-06-09 02:31:19.274159 frontmatter_cli-2023.6.1/PKG-INFO
--rw-r--r--   0 jefftriplett   (501) staff       (20)     1683 2023-06-09 02:23:17.000000 frontmatter_cli-2023.6.1/README.md
-drwxr-xr-x   0 jefftriplett   (501) staff       (20)        0 2023-06-09 02:31:19.272969 frontmatter_cli-2023.6.1/frontmatter_cli/
--rw-r--r--   0 jefftriplett   (501) staff       (20)      160 2023-06-09 02:26:44.000000 frontmatter_cli-2023.6.1/frontmatter_cli/__init__.py
--rw-r--r--   0 jefftriplett   (501) staff       (20)       74 2023-06-09 02:13:44.000000 frontmatter_cli-2023.6.1/frontmatter_cli/__main__.py
--rw-r--r--   0 jefftriplett   (501) staff       (20)     1364 2023-06-09 02:26:44.000000 frontmatter_cli-2023.6.1/frontmatter_cli/cli.py
-drwxr-xr-x   0 jefftriplett   (501) staff       (20)        0 2023-06-09 02:31:19.274006 frontmatter_cli-2023.6.1/frontmatter_cli.egg-info/
--rw-r--r--   0 jefftriplett   (501) staff       (20)     2652 2023-06-09 02:31:19.000000 frontmatter_cli-2023.6.1/frontmatter_cli.egg-info/PKG-INFO
--rw-r--r--   0 jefftriplett   (501) staff       (20)      427 2023-06-09 02:31:19.000000 frontmatter_cli-2023.6.1/frontmatter_cli.egg-info/SOURCES.txt
--rw-r--r--   0 jefftriplett   (501) staff       (20)        1 2023-06-09 02:31:19.000000 frontmatter_cli-2023.6.1/frontmatter_cli.egg-info/dependency_links.txt
--rw-r--r--   0 jefftriplett   (501) staff       (20)       90 2023-06-09 02:31:19.000000 frontmatter_cli-2023.6.1/frontmatter_cli.egg-info/entry_points.txt
--rw-r--r--   0 jefftriplett   (501) staff       (20)        1 2023-06-09 02:14:15.000000 frontmatter_cli-2023.6.1/frontmatter_cli.egg-info/not-zip-safe
--rw-r--r--   0 jefftriplett   (501) staff       (20)       52 2023-06-09 02:31:19.000000 frontmatter_cli-2023.6.1/frontmatter_cli.egg-info/requires.txt
--rw-r--r--   0 jefftriplett   (501) staff       (20)       16 2023-06-09 02:31:19.000000 frontmatter_cli-2023.6.1/frontmatter_cli.egg-info/top_level.txt
--rw-r--r--   0 jefftriplett   (501) staff       (20)     1291 2023-06-09 02:26:44.000000 frontmatter_cli-2023.6.1/pyproject.toml
--rw-r--r--   0 jefftriplett   (501) staff       (20)     1229 2023-06-09 02:31:19.274470 frontmatter_cli-2023.6.1/setup.cfg
--rw-r--r--   0 jefftriplett   (501) staff       (20)       38 2023-06-09 02:13:44.000000 frontmatter_cli-2023.6.1/setup.py
+drwxr-xr-x   0 jefftriplett   (501) staff       (20)        0 2023-07-09 13:41:08.830857 frontmatter-cli-2023.7.1/
+-rw-r--r--   0 jefftriplett   (501) staff       (20)       11 2023-06-09 02:13:44.000000 frontmatter-cli-2023.7.1/HISTORY.md
+-rw-r--r--   0 jefftriplett   (501) staff       (20)     1513 2023-06-09 02:13:44.000000 frontmatter-cli-2023.7.1/LICENSE
+-rw-r--r--   0 jefftriplett   (501) staff       (20)      134 2023-06-09 02:13:44.000000 frontmatter-cli-2023.7.1/MANIFEST.in
+-rw-r--r--   0 jefftriplett   (501) staff       (20)     1950 2023-07-09 13:41:08.830753 frontmatter-cli-2023.7.1/PKG-INFO
+-rw-r--r--   0 jefftriplett   (501) staff       (20)     1683 2023-06-09 02:23:17.000000 frontmatter-cli-2023.7.1/README.md
+drwxr-xr-x   0 jefftriplett   (501) staff       (20)        0 2023-07-09 13:41:08.829852 frontmatter-cli-2023.7.1/frontmatter_cli/
+-rw-r--r--   0 jefftriplett   (501) staff       (20)       67 2023-07-09 13:35:20.000000 frontmatter-cli-2023.7.1/frontmatter_cli/__init__.py
+-rw-r--r--   0 jefftriplett   (501) staff       (20)       74 2023-06-09 02:13:44.000000 frontmatter-cli-2023.7.1/frontmatter_cli/__main__.py
+-rw-r--r--   0 jefftriplett   (501) staff       (20)     1325 2023-07-09 13:41:01.000000 frontmatter-cli-2023.7.1/frontmatter_cli/cli.py
+drwxr-xr-x   0 jefftriplett   (501) staff       (20)        0 2023-07-09 13:41:08.830611 frontmatter-cli-2023.7.1/frontmatter_cli.egg-info/
+-rw-r--r--   0 jefftriplett   (501) staff       (20)     1950 2023-07-09 13:41:08.000000 frontmatter-cli-2023.7.1/frontmatter_cli.egg-info/PKG-INFO
+-rw-r--r--   0 jefftriplett   (501) staff       (20)      370 2023-07-09 13:41:08.000000 frontmatter-cli-2023.7.1/frontmatter_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 jefftriplett   (501) staff       (20)        1 2023-07-09 13:41:08.000000 frontmatter-cli-2023.7.1/frontmatter_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 jefftriplett   (501) staff       (20)       90 2023-07-09 13:41:08.000000 frontmatter-cli-2023.7.1/frontmatter_cli.egg-info/entry_points.txt
+-rw-r--r--   0 jefftriplett   (501) staff       (20)        1 2023-06-09 02:14:15.000000 frontmatter-cli-2023.7.1/frontmatter_cli.egg-info/not-zip-safe
+-rw-r--r--   0 jefftriplett   (501) staff       (20)       16 2023-07-09 13:41:08.000000 frontmatter-cli-2023.7.1/frontmatter_cli.egg-info/top_level.txt
+-rw-r--r--   0 jefftriplett   (501) staff       (20)     2557 2023-07-09 13:41:01.000000 frontmatter-cli-2023.7.1/pyproject.toml
+-rw-r--r--   0 jefftriplett   (501) staff       (20)       38 2023-07-09 13:41:08.830889 frontmatter-cli-2023.7.1/setup.cfg
```

### Comparing `frontmatter_cli-2023.6.1/LICENSE` & `frontmatter-cli-2023.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `frontmatter_cli-2023.6.1/PKG-INFO` & `frontmatter-cli-2023.7.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,12 @@
 Metadata-Version: 2.1
-Name: frontmatter_cli
-Version: 2023.6.1
+Name: frontmatter-cli
+Version: 2023.7.1
 Summary: Frontmatter CLI tool to make working with frontmatter easier.
-Home-page: https://github.com/jefftriplett/frontmatter-cli
-Author: Jeff Triplett
-Author-email: jeff.triplett@gmail.com
-License: BSD-3-Clause
-Keywords: frontmatter,frontmatter-cli
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Framework :: Django
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Project-URL: Homepage, https://github.com/jefftriplett/frontmatter-cli
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # frontmatter-cli
 
 This is a very early WIP project. My goal is to make working with Frontmatter a little nicer from the command line. The API is going to change, and I plan on adding some other features to make editing Frontmatter easier too.
```

### Comparing `frontmatter_cli-2023.6.1/README.md` & `frontmatter-cli-2023.7.1/README.md`

 * *Files identical despite different names*

### Comparing `frontmatter_cli-2023.6.1/frontmatter_cli/cli.py` & `frontmatter-cli-2023.7.1/frontmatter_cli/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import frontmatter
 
 from click_default_group import DefaultGroup
 from pydash import set_
 
 __author__ = "Jeff Triplett"
 __email__ = "jeff.triplett@gmail.com"
-__version__ = "2023.6.1"
+__version__ = "2023.7.1"
 
 
 def validate_extra_context(ctx, param, value):
     """Validate extra context."""
     for key in value:
         if "=" not in key:
             raise click.BadParameter(
@@ -39,11 +39,7 @@
     post = frontmatter.loads(chunk)
 
     if extra_context:
         for key, value in extra_context.items():
             set_(post.metadata, key, value)
 
     frontmatter.dump(post, output)
-
-
-if __name__ == "__main__":
-    cli()
```

### Comparing `frontmatter_cli-2023.6.1/frontmatter_cli.egg-info/PKG-INFO` & `frontmatter-cli-2023.7.1/frontmatter_cli.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,12 @@
 Metadata-Version: 2.1
 Name: frontmatter-cli
-Version: 2023.6.1
+Version: 2023.7.1
 Summary: Frontmatter CLI tool to make working with frontmatter easier.
-Home-page: https://github.com/jefftriplett/frontmatter-cli
-Author: Jeff Triplett
-Author-email: jeff.triplett@gmail.com
-License: BSD-3-Clause
-Keywords: frontmatter,frontmatter-cli
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Framework :: Django
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Project-URL: Homepage, https://github.com/jefftriplett/frontmatter-cli
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # frontmatter-cli
 
 This is a very early WIP project. My goal is to make working with Frontmatter a little nicer from the command line. The API is going to change, and I plan on adding some other features to make editing Frontmatter easier too.
```

