# Comparing `tmp/frontmatter-cli-2023.7.1.tar.gz` & `tmp/frontmatter-cli-2023.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frontmatter-cli-2023.7.1.tar", last modified: Sun Jul  9 13:41:08 2023, max compression
+gzip compressed data, was "frontmatter-cli-2023.7.2.tar", last modified: Sun Jul  9 13:51:21 2023, max compression
```

## Comparing `frontmatter-cli-2023.7.1.tar` & `frontmatter-cli-2023.7.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 jefftriplett   (501) staff       (20)        0 2023-07-09 13:41:08.830857 frontmatter-cli-2023.7.1/
--rw-r--r--   0 jefftriplett   (501) staff       (20)       11 2023-06-09 02:13:44.000000 frontmatter-cli-2023.7.1/HISTORY.md
--rw-r--r--   0 jefftriplett   (501) staff       (20)     1513 2023-06-09 02:13:44.000000 frontmatter-cli-2023.7.1/LICENSE
--rw-r--r--   0 jefftriplett   (501) staff       (20)      134 2023-06-09 02:13:44.000000 frontmatter-cli-2023.7.1/MANIFEST.in
--rw-r--r--   0 jefftriplett   (501) staff       (20)     1950 2023-07-09 13:41:08.830753 frontmatter-cli-2023.7.1/PKG-INFO
--rw-r--r--   0 jefftriplett   (501) staff       (20)     1683 2023-06-09 02:23:17.000000 frontmatter-cli-2023.7.1/README.md
-drwxr-xr-x   0 jefftriplett   (501) staff       (20)        0 2023-07-09 13:41:08.829852 frontmatter-cli-2023.7.1/frontmatter_cli/
--rw-r--r--   0 jefftriplett   (501) staff       (20)       67 2023-07-09 13:35:20.000000 frontmatter-cli-2023.7.1/frontmatter_cli/__init__.py
--rw-r--r--   0 jefftriplett   (501) staff       (20)       74 2023-06-09 02:13:44.000000 frontmatter-cli-2023.7.1/frontmatter_cli/__main__.py
--rw-r--r--   0 jefftriplett   (501) staff       (20)     1325 2023-07-09 13:41:01.000000 frontmatter-cli-2023.7.1/frontmatter_cli/cli.py
-drwxr-xr-x   0 jefftriplett   (501) staff       (20)        0 2023-07-09 13:41:08.830611 frontmatter-cli-2023.7.1/frontmatter_cli.egg-info/
--rw-r--r--   0 jefftriplett   (501) staff       (20)     1950 2023-07-09 13:41:08.000000 frontmatter-cli-2023.7.1/frontmatter_cli.egg-info/PKG-INFO
--rw-r--r--   0 jefftriplett   (501) staff       (20)      370 2023-07-09 13:41:08.000000 frontmatter-cli-2023.7.1/frontmatter_cli.egg-info/SOURCES.txt
--rw-r--r--   0 jefftriplett   (501) staff       (20)        1 2023-07-09 13:41:08.000000 frontmatter-cli-2023.7.1/frontmatter_cli.egg-info/dependency_links.txt
--rw-r--r--   0 jefftriplett   (501) staff       (20)       90 2023-07-09 13:41:08.000000 frontmatter-cli-2023.7.1/frontmatter_cli.egg-info/entry_points.txt
--rw-r--r--   0 jefftriplett   (501) staff       (20)        1 2023-06-09 02:14:15.000000 frontmatter-cli-2023.7.1/frontmatter_cli.egg-info/not-zip-safe
--rw-r--r--   0 jefftriplett   (501) staff       (20)       16 2023-07-09 13:41:08.000000 frontmatter-cli-2023.7.1/frontmatter_cli.egg-info/top_level.txt
--rw-r--r--   0 jefftriplett   (501) staff       (20)     2557 2023-07-09 13:41:01.000000 frontmatter-cli-2023.7.1/pyproject.toml
--rw-r--r--   0 jefftriplett   (501) staff       (20)       38 2023-07-09 13:41:08.830889 frontmatter-cli-2023.7.1/setup.cfg
+drwxr-xr-x   0 jefftriplett   (501) staff       (20)        0 2023-07-09 13:51:21.917930 frontmatter-cli-2023.7.2/
+-rw-r--r--   0 jefftriplett   (501) staff       (20)       11 2023-06-09 02:13:44.000000 frontmatter-cli-2023.7.2/HISTORY.md
+-rw-r--r--   0 jefftriplett   (501) staff       (20)     1513 2023-06-09 02:13:44.000000 frontmatter-cli-2023.7.2/LICENSE
+-rw-r--r--   0 jefftriplett   (501) staff       (20)      134 2023-06-09 02:13:44.000000 frontmatter-cli-2023.7.2/MANIFEST.in
+-rw-r--r--   0 jefftriplett   (501) staff       (20)     2764 2023-07-09 13:51:21.917811 frontmatter-cli-2023.7.2/PKG-INFO
+-rw-r--r--   0 jefftriplett   (501) staff       (20)     1683 2023-06-09 02:23:17.000000 frontmatter-cli-2023.7.2/README.md
+drwxr-xr-x   0 jefftriplett   (501) staff       (20)        0 2023-07-09 13:51:21.916652 frontmatter-cli-2023.7.2/frontmatter_cli/
+-rw-r--r--   0 jefftriplett   (501) staff       (20)       67 2023-07-09 13:35:20.000000 frontmatter-cli-2023.7.2/frontmatter_cli/__init__.py
+-rw-r--r--   0 jefftriplett   (501) staff       (20)       74 2023-06-09 02:13:44.000000 frontmatter-cli-2023.7.2/frontmatter_cli/__main__.py
+-rw-r--r--   0 jefftriplett   (501) staff       (20)     1325 2023-07-09 13:51:14.000000 frontmatter-cli-2023.7.2/frontmatter_cli/cli.py
+drwxr-xr-x   0 jefftriplett   (501) staff       (20)        0 2023-07-09 13:51:21.917644 frontmatter-cli-2023.7.2/frontmatter_cli.egg-info/
+-rw-r--r--   0 jefftriplett   (501) staff       (20)     2764 2023-07-09 13:51:21.000000 frontmatter-cli-2023.7.2/frontmatter_cli.egg-info/PKG-INFO
+-rw-r--r--   0 jefftriplett   (501) staff       (20)      408 2023-07-09 13:51:21.000000 frontmatter-cli-2023.7.2/frontmatter_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 jefftriplett   (501) staff       (20)        1 2023-07-09 13:51:21.000000 frontmatter-cli-2023.7.2/frontmatter_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 jefftriplett   (501) staff       (20)       90 2023-07-09 13:51:21.000000 frontmatter-cli-2023.7.2/frontmatter_cli.egg-info/entry_points.txt
+-rw-r--r--   0 jefftriplett   (501) staff       (20)        1 2023-06-09 02:14:15.000000 frontmatter-cli-2023.7.2/frontmatter_cli.egg-info/not-zip-safe
+-rw-r--r--   0 jefftriplett   (501) staff       (20)       52 2023-07-09 13:51:21.000000 frontmatter-cli-2023.7.2/frontmatter_cli.egg-info/requires.txt
+-rw-r--r--   0 jefftriplett   (501) staff       (20)       16 2023-07-09 13:51:21.000000 frontmatter-cli-2023.7.2/frontmatter_cli.egg-info/top_level.txt
+-rw-r--r--   0 jefftriplett   (501) staff       (20)     2694 2023-07-09 13:51:14.000000 frontmatter-cli-2023.7.2/pyproject.toml
+-rw-r--r--   0 jefftriplett   (501) staff       (20)       38 2023-07-09 13:51:21.917979 frontmatter-cli-2023.7.2/setup.cfg
```

### Comparing `frontmatter-cli-2023.7.1/LICENSE` & `frontmatter-cli-2023.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `frontmatter-cli-2023.7.1/PKG-INFO` & `frontmatter-cli-2023.7.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: frontmatter-cli
-Version: 2023.7.1
-Summary: Frontmatter CLI tool to make working with frontmatter easier.
-Project-URL: Homepage, https://github.com/jefftriplett/frontmatter-cli
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # frontmatter-cli
 
 This is a very early WIP project. My goal is to make working with Frontmatter a little nicer from the command line. The API is going to change, and I plan on adding some other features to make editing Frontmatter easier too.
 
 ## Install
 
 ```shell
```

### Comparing `frontmatter-cli-2023.7.1/README.md` & `frontmatter-cli-2023.7.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: frontmatter-cli
+Version: 2023.7.2
+Summary: Frontmatter CLI tool to make working with frontmatter easier.
+Author-email: Jeff Triplett <jeff.triplett@gmail.com>
+License: BSD-3-Clause
+Project-URL: Bug Tracker, https://github.com/jefftriplett/frontmatter-cli/issues
+Project-URL: Homepage, https://github.com/jefftriplett/frontmatter-cli
+Project-URL: Source Code, https://github.com/jefftriplett/frontmatter-cli
+Keywords: frontmatter,frontmatter-cli
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Framework :: Django
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # frontmatter-cli
 
 This is a very early WIP project. My goal is to make working with Frontmatter a little nicer from the command line. The API is going to change, and I plan on adding some other features to make editing Frontmatter easier too.
 
 ## Install
 
 ```shell
```

### Comparing `frontmatter-cli-2023.7.1/frontmatter_cli/cli.py` & `frontmatter-cli-2023.7.2/frontmatter_cli/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import frontmatter
 
 from click_default_group import DefaultGroup
 from pydash import set_
 
 __author__ = "Jeff Triplett"
 __email__ = "jeff.triplett@gmail.com"
-__version__ = "2023.7.1"
+__version__ = "2023.7.2"
 
 
 def validate_extra_context(ctx, param, value):
     """Validate extra context."""
     for key in value:
         if "=" not in key:
             raise click.BadParameter(
```

### Comparing `frontmatter-cli-2023.7.1/frontmatter_cli.egg-info/PKG-INFO` & `frontmatter-cli-2023.7.2/frontmatter_cli.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,29 @@
 Metadata-Version: 2.1
 Name: frontmatter-cli
-Version: 2023.7.1
+Version: 2023.7.2
 Summary: Frontmatter CLI tool to make working with frontmatter easier.
+Author-email: Jeff Triplett <jeff.triplett@gmail.com>
+License: BSD-3-Clause
+Project-URL: Bug Tracker, https://github.com/jefftriplett/frontmatter-cli/issues
 Project-URL: Homepage, https://github.com/jefftriplett/frontmatter-cli
+Project-URL: Source Code, https://github.com/jefftriplett/frontmatter-cli
+Keywords: frontmatter,frontmatter-cli
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Framework :: Django
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # frontmatter-cli
 
 This is a very early WIP project. My goal is to make working with Frontmatter a little nicer from the command line. The API is going to change, and I plan on adding some other features to make editing Frontmatter easier too.
```

### Comparing `frontmatter-cli-2023.7.1/pyproject.toml` & `frontmatter-cli-2023.7.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -2,27 +2,23 @@
 build-backend = "setuptools.build_meta"
 requires = [
   "setuptools>=61.2",
 ]
 
 [project]
 name = "frontmatter-cli"
-version = "2023.7.1"
+version = "2023.7.2"
 description = "Frontmatter CLI tool to make working with frontmatter easier."
-[project.readme]
-file = "README.md"
-content-type = "text/markdown"
-
 keywords = [
   "frontmatter",
   "frontmatter-cli",
 ]
 license = {text = "BSD-3-Clause"}
 authors = [{name = "Jeff Triplett", email = "jeff.triplett@gmail.com"}]
-requires-python = ">=3.7"
+requires-python = ">3.7"
 classifiers = [
   "Development Status :: 2 - Pre-Alpha",
   "Framework :: Django",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: BSD License",
   "Natural Language :: English",
   "Programming Language :: Python :: 3 :: Only",
@@ -34,16 +30,21 @@
 ]
 dependencies = [
   "click",
   "click-default-group",
   "pydash",
   "python-frontmatter",
 ]
+[project.readme]
+file = "README.md"
+content-type = "text/markdown"
 [project.urls]
+"Bug Tracker" = "https://github.com/jefftriplett/frontmatter-cli/issues"
 Homepage = "https://github.com/jefftriplett/frontmatter-cli"
+"Source Code" = "https://github.com/jefftriplett/frontmatter-cli"
 [project.scripts]
 frontmatter = "frontmatter_cli:cli"
 frontmatter-cli = "frontmatter_cli:cli"
 
 [tool.setuptools]
 packages = ["frontmatter_cli"]
 zip-safe = false
@@ -92,15 +93,15 @@
 target-version = "py311"
 
 [tool.ruff.mccabe]
 # Unlike Flake8, default to a complexity level of 10.
 max-complexity = 10
 
 [tool.bumpver]
-current_version = "2023.7.1"
+current_version = "2023.7.2"
 version_pattern = "YYYY.MM.INC1"
 commit_message = ":bookmark: Bump version {old_version} -> {new_version}"
 commit = true
 push = true  # disable for GitHub Actions
 tag = true
 
 [tool.bumpver.file_patterns]
```

