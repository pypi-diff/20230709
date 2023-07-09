# Comparing `tmp/frontmatter-cli-2023.7.2.tar.gz` & `tmp/frontmatter-cli-2023.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frontmatter-cli-2023.7.2.tar", last modified: Sun Jul  9 13:51:21 2023, max compression
+gzip compressed data, was "frontmatter-cli-2023.7.3.tar", last modified: Sun Jul  9 13:54:46 2023, max compression
```

## Comparing `frontmatter-cli-2023.7.2.tar` & `frontmatter-cli-2023.7.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jefftriplett   (501) staff       (20)        0 2023-07-09 13:51:21.917930 frontmatter-cli-2023.7.2/
--rw-r--r--   0 jefftriplett   (501) staff       (20)       11 2023-06-09 02:13:44.000000 frontmatter-cli-2023.7.2/HISTORY.md
--rw-r--r--   0 jefftriplett   (501) staff       (20)     1513 2023-06-09 02:13:44.000000 frontmatter-cli-2023.7.2/LICENSE
--rw-r--r--   0 jefftriplett   (501) staff       (20)      134 2023-06-09 02:13:44.000000 frontmatter-cli-2023.7.2/MANIFEST.in
--rw-r--r--   0 jefftriplett   (501) staff       (20)     2764 2023-07-09 13:51:21.917811 frontmatter-cli-2023.7.2/PKG-INFO
--rw-r--r--   0 jefftriplett   (501) staff       (20)     1683 2023-06-09 02:23:17.000000 frontmatter-cli-2023.7.2/README.md
-drwxr-xr-x   0 jefftriplett   (501) staff       (20)        0 2023-07-09 13:51:21.916652 frontmatter-cli-2023.7.2/frontmatter_cli/
--rw-r--r--   0 jefftriplett   (501) staff       (20)       67 2023-07-09 13:35:20.000000 frontmatter-cli-2023.7.2/frontmatter_cli/__init__.py
--rw-r--r--   0 jefftriplett   (501) staff       (20)       74 2023-06-09 02:13:44.000000 frontmatter-cli-2023.7.2/frontmatter_cli/__main__.py
--rw-r--r--   0 jefftriplett   (501) staff       (20)     1325 2023-07-09 13:51:14.000000 frontmatter-cli-2023.7.2/frontmatter_cli/cli.py
-drwxr-xr-x   0 jefftriplett   (501) staff       (20)        0 2023-07-09 13:51:21.917644 frontmatter-cli-2023.7.2/frontmatter_cli.egg-info/
--rw-r--r--   0 jefftriplett   (501) staff       (20)     2764 2023-07-09 13:51:21.000000 frontmatter-cli-2023.7.2/frontmatter_cli.egg-info/PKG-INFO
--rw-r--r--   0 jefftriplett   (501) staff       (20)      408 2023-07-09 13:51:21.000000 frontmatter-cli-2023.7.2/frontmatter_cli.egg-info/SOURCES.txt
--rw-r--r--   0 jefftriplett   (501) staff       (20)        1 2023-07-09 13:51:21.000000 frontmatter-cli-2023.7.2/frontmatter_cli.egg-info/dependency_links.txt
--rw-r--r--   0 jefftriplett   (501) staff       (20)       90 2023-07-09 13:51:21.000000 frontmatter-cli-2023.7.2/frontmatter_cli.egg-info/entry_points.txt
--rw-r--r--   0 jefftriplett   (501) staff       (20)        1 2023-06-09 02:14:15.000000 frontmatter-cli-2023.7.2/frontmatter_cli.egg-info/not-zip-safe
--rw-r--r--   0 jefftriplett   (501) staff       (20)       52 2023-07-09 13:51:21.000000 frontmatter-cli-2023.7.2/frontmatter_cli.egg-info/requires.txt
--rw-r--r--   0 jefftriplett   (501) staff       (20)       16 2023-07-09 13:51:21.000000 frontmatter-cli-2023.7.2/frontmatter_cli.egg-info/top_level.txt
--rw-r--r--   0 jefftriplett   (501) staff       (20)     2694 2023-07-09 13:51:14.000000 frontmatter-cli-2023.7.2/pyproject.toml
--rw-r--r--   0 jefftriplett   (501) staff       (20)       38 2023-07-09 13:51:21.917979 frontmatter-cli-2023.7.2/setup.cfg
+drwxr-xr-x   0 jefftriplett   (501) staff       (20)        0 2023-07-09 13:54:46.012319 frontmatter-cli-2023.7.3/
+-rw-r--r--   0 jefftriplett   (501) staff       (20)       11 2023-06-09 02:13:44.000000 frontmatter-cli-2023.7.3/HISTORY.md
+-rw-r--r--   0 jefftriplett   (501) staff       (20)     1513 2023-06-09 02:13:44.000000 frontmatter-cli-2023.7.3/LICENSE
+-rw-r--r--   0 jefftriplett   (501) staff       (20)      134 2023-06-09 02:13:44.000000 frontmatter-cli-2023.7.3/MANIFEST.in
+-rw-r--r--   0 jefftriplett   (501) staff       (20)     2764 2023-07-09 13:54:46.012212 frontmatter-cli-2023.7.3/PKG-INFO
+-rw-r--r--   0 jefftriplett   (501) staff       (20)     1683 2023-06-09 02:23:17.000000 frontmatter-cli-2023.7.3/README.md
+drwxr-xr-x   0 jefftriplett   (501) staff       (20)        0 2023-07-09 13:54:46.011186 frontmatter-cli-2023.7.3/frontmatter_cli/
+-rw-r--r--   0 jefftriplett   (501) staff       (20)       67 2023-07-09 13:35:20.000000 frontmatter-cli-2023.7.3/frontmatter_cli/__init__.py
+-rw-r--r--   0 jefftriplett   (501) staff       (20)       74 2023-06-09 02:13:44.000000 frontmatter-cli-2023.7.3/frontmatter_cli/__main__.py
+-rw-r--r--   0 jefftriplett   (501) staff       (20)     1325 2023-07-09 13:54:35.000000 frontmatter-cli-2023.7.3/frontmatter_cli/cli.py
+drwxr-xr-x   0 jefftriplett   (501) staff       (20)        0 2023-07-09 13:54:46.012056 frontmatter-cli-2023.7.3/frontmatter_cli.egg-info/
+-rw-r--r--   0 jefftriplett   (501) staff       (20)     2764 2023-07-09 13:54:46.000000 frontmatter-cli-2023.7.3/frontmatter_cli.egg-info/PKG-INFO
+-rw-r--r--   0 jefftriplett   (501) staff       (20)      408 2023-07-09 13:54:46.000000 frontmatter-cli-2023.7.3/frontmatter_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 jefftriplett   (501) staff       (20)        1 2023-07-09 13:54:46.000000 frontmatter-cli-2023.7.3/frontmatter_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 jefftriplett   (501) staff       (20)       90 2023-07-09 13:54:46.000000 frontmatter-cli-2023.7.3/frontmatter_cli.egg-info/entry_points.txt
+-rw-r--r--   0 jefftriplett   (501) staff       (20)        1 2023-06-09 02:14:15.000000 frontmatter-cli-2023.7.3/frontmatter_cli.egg-info/not-zip-safe
+-rw-r--r--   0 jefftriplett   (501) staff       (20)       52 2023-07-09 13:54:46.000000 frontmatter-cli-2023.7.3/frontmatter_cli.egg-info/requires.txt
+-rw-r--r--   0 jefftriplett   (501) staff       (20)       16 2023-07-09 13:54:46.000000 frontmatter-cli-2023.7.3/frontmatter_cli.egg-info/top_level.txt
+-rw-r--r--   0 jefftriplett   (501) staff       (20)     2648 2023-07-09 13:54:35.000000 frontmatter-cli-2023.7.3/pyproject.toml
+-rw-r--r--   0 jefftriplett   (501) staff       (20)       38 2023-07-09 13:54:46.012353 frontmatter-cli-2023.7.3/setup.cfg
```

### Comparing `frontmatter-cli-2023.7.2/LICENSE` & `frontmatter-cli-2023.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `frontmatter-cli-2023.7.2/PKG-INFO` & `frontmatter-cli-2023.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frontmatter-cli
-Version: 2023.7.2
+Version: 2023.7.3
 Summary: Frontmatter CLI tool to make working with frontmatter easier.
 Author-email: Jeff Triplett <jeff.triplett@gmail.com>
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/jefftriplett/frontmatter-cli/issues
 Project-URL: Homepage, https://github.com/jefftriplett/frontmatter-cli
 Project-URL: Source Code, https://github.com/jefftriplett/frontmatter-cli
 Keywords: frontmatter,frontmatter-cli
```

### Comparing `frontmatter-cli-2023.7.2/README.md` & `frontmatter-cli-2023.7.3/README.md`

 * *Files identical despite different names*

### Comparing `frontmatter-cli-2023.7.2/frontmatter_cli/cli.py` & `frontmatter-cli-2023.7.3/frontmatter_cli/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import frontmatter
 
 from click_default_group import DefaultGroup
 from pydash import set_
 
 __author__ = "Jeff Triplett"
 __email__ = "jeff.triplett@gmail.com"
-__version__ = "2023.7.2"
+__version__ = "2023.7.3"
 
 
 def validate_extra_context(ctx, param, value):
     """Validate extra context."""
     for key in value:
         if "=" not in key:
             raise click.BadParameter(
```

### Comparing `frontmatter-cli-2023.7.2/frontmatter_cli.egg-info/PKG-INFO` & `frontmatter-cli-2023.7.3/frontmatter_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frontmatter-cli
-Version: 2023.7.2
+Version: 2023.7.3
 Summary: Frontmatter CLI tool to make working with frontmatter easier.
 Author-email: Jeff Triplett <jeff.triplett@gmail.com>
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/jefftriplett/frontmatter-cli/issues
 Project-URL: Homepage, https://github.com/jefftriplett/frontmatter-cli
 Project-URL: Source Code, https://github.com/jefftriplett/frontmatter-cli
 Keywords: frontmatter,frontmatter-cli
```

### Comparing `frontmatter-cli-2023.7.2/pyproject.toml` & `frontmatter-cli-2023.7.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 build-backend = "setuptools.build_meta"
 requires = [
   "setuptools>=61.2",
 ]
 
 [project]
 name = "frontmatter-cli"
-version = "2023.7.2"
+version = "2023.7.3"
 description = "Frontmatter CLI tool to make working with frontmatter easier."
+readme = "README.md"
 keywords = [
   "frontmatter",
   "frontmatter-cli",
 ]
 license = {text = "BSD-3-Clause"}
 authors = [{name = "Jeff Triplett", email = "jeff.triplett@gmail.com"}]
 requires-python = ">3.7"
@@ -30,17 +31,14 @@
 ]
 dependencies = [
   "click",
   "click-default-group",
   "pydash",
   "python-frontmatter",
 ]
-[project.readme]
-file = "README.md"
-content-type = "text/markdown"
 [project.urls]
 "Bug Tracker" = "https://github.com/jefftriplett/frontmatter-cli/issues"
 Homepage = "https://github.com/jefftriplett/frontmatter-cli"
 "Source Code" = "https://github.com/jefftriplett/frontmatter-cli"
 [project.scripts]
 frontmatter = "frontmatter_cli:cli"
 frontmatter-cli = "frontmatter_cli:cli"
@@ -93,15 +91,15 @@
 target-version = "py311"
 
 [tool.ruff.mccabe]
 # Unlike Flake8, default to a complexity level of 10.
 max-complexity = 10
 
 [tool.bumpver]
-current_version = "2023.7.2"
+current_version = "2023.7.3"
 version_pattern = "YYYY.MM.INC1"
 commit_message = ":bookmark: Bump version {old_version} -> {new_version}"
 commit = true
 push = true  # disable for GitHub Actions
 tag = true
 
 [tool.bumpver.file_patterns]
```

