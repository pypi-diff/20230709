# Comparing `tmp/pdir2-0.3.6.tar.gz` & `tmp/pdir2-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdir2-0.3.6.tar", last modified: Sun Jul  3 05:16:00 2022, max compression
+gzip compressed data, was "pdir2-1.0.0.tar", last modified: Sun Jul  9 21:57:17 2023, max compression
```

## Comparing `pdir2-0.3.6.tar` & `pdir2-1.0.0.tar`

### file list

```diff
@@ -1,39 +1,31 @@
--rw-r--r--   0 laike9m    (501) staff       (20)     1064 2017-03-08 15:53:25.000000 pdir2-0.3.6/LICENSE
--rw-r--r--   0 laike9m    (501) staff       (20)     3069 2022-04-21 06:47:40.255532 pdir2-0.3.6/README.md
--rw-r--r--   0 laike9m    (501) staff       (20)      159 2018-02-08 14:24:11.785120 pdir2-0.3.6/pdir/.idea/encodings.xml
--rw-r--r--   0 laike9m    (501) staff       (20)     1567 2018-02-08 14:24:11.579171 pdir2-0.3.6/pdir/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 laike9m    (501) staff       (20)      228 2018-02-08 14:24:11.791144 pdir2-0.3.6/pdir/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 laike9m    (501) staff       (20)      909 2018-11-13 14:37:04.598287 pdir2-0.3.6/pdir/.idea/misc.xml
--rw-r--r--   0 laike9m    (501) staff       (20)      411 2018-11-13 14:35:13.509435 pdir2-0.3.6/pdir/.idea/modules.xml
--rw-r--r--   0 laike9m    (501) staff       (20)      557 2018-11-13 14:35:13.494672 pdir2-0.3.6/pdir/.idea/pdir.iml
--rw-r--r--   0 laike9m    (501) staff       (20)      322 2018-11-13 14:35:13.506561 pdir2-0.3.6/pdir/.idea/vcs.xml
--rw-r--r--   0 laike9m    (501) staff       (20)    22629 2018-11-13 15:29:51.389770 pdir2-0.3.6/pdir/.idea/workspace.xml
--rw-r--r--   0 laike9m    (501) staff       (20)      133 2018-11-18 13:04:53.285294 pdir2-0.3.6/pdir/__init__.py
--rw-r--r--   0 laike9m    (501) staff       (20)     2353 2022-04-21 06:40:02.258267 pdir2-0.3.6/pdir/_internal_utils.py
--rw-r--r--   0 laike9m    (501) staff       (20)     6711 2022-07-03 05:10:51.279309 pdir2-0.3.6/pdir/api.py
--rw-r--r--   0 laike9m    (501) staff       (20)    14341 2022-03-12 20:04:59.048600 pdir2-0.3.6/pdir/attr_category.py
--rw-r--r--   0 laike9m    (501) staff       (20)     1991 2022-07-03 05:10:51.280705 pdir2-0.3.6/pdir/color.py
--rw-r--r--   0 laike9m    (501) staff       (20)     3948 2022-07-03 05:10:51.281716 pdir2-0.3.6/pdir/configuration.py
--rw-r--r--   0 laike9m    (501) staff       (20)      341 2018-11-18 13:05:32.321846 pdir2-0.3.6/pdir/constants.py
--rw-r--r--   0 laike9m    (501) staff       (20)     3473 2022-03-12 20:04:54.587736 pdir2-0.3.6/pdir/format.py
--rw-r--r--   0 laike9m    (501) staff       (20)     1644 2022-07-03 05:14:39.941367 pdir2-0.3.6/pyproject.toml
--rw-r--r--   0 laike9m    (501) staff       (20)     1577 2022-07-03 05:10:51.285528 pdir2-0.3.6/tests/conftest.py
--rw-r--r--   0 laike9m    (501) staff       (20)       85 2017-04-04 08:35:45.000000 pdir2-0.3.6/tests/data/config_1.ini
--rw-r--r--   0 laike9m    (501) staff       (20)       71 2017-04-04 08:34:07.000000 pdir2-0.3.6/tests/data/config_2.ini
--rw-r--r--   0 laike9m    (501) staff       (20)       39 2022-07-03 05:10:51.285844 pdir2-0.3.6/tests/data/config_auto_color.ini
--rw-r--r--   0 laike9m    (501) staff       (20)       40 2022-07-03 05:10:51.286103 pdir2-0.3.6/tests/data/config_disable_color.ini
--rw-r--r--   0 laike9m    (501) staff       (20)       39 2022-07-03 05:10:51.286427 pdir2-0.3.6/tests/data/config_enable_color.ini
--rw-r--r--   0 laike9m    (501) staff       (20)        0 2017-04-04 08:34:07.000000 pdir2-0.3.6/tests/data/empty_config.ini
--rw-r--r--   0 laike9m    (501) staff       (20)       49 2017-04-04 08:34:07.000000 pdir2-0.3.6/tests/data/error_config_1.ini
--rw-r--r--   0 laike9m    (501) staff       (20)       47 2017-04-04 08:34:07.000000 pdir2-0.3.6/tests/data/error_config_2.ini
--rw-r--r--   0 laike9m    (501) staff       (20)     1123 2022-07-03 05:10:51.287246 pdir2-0.3.6/tests/interactive_test.py
--rw-r--r--   0 laike9m    (501) staff       (20)      108 2018-11-08 13:53:46.451887 pdir2-0.3.6/tests/m.py
--rw-r--r--   0 laike9m    (501) staff       (20)     3581 2022-07-03 05:10:51.288257 pdir2-0.3.6/tests/test_buggy_attrs.py
--rw-r--r--   0 laike9m    (501) staff       (20)      609 2022-07-03 05:10:51.289806 pdir2-0.3.6/tests/test_container.py
--rw-r--r--   0 laike9m    (501) staff       (20)      204 2022-07-03 05:10:51.290042 pdir2-0.3.6/tests/test_disbale_color.py
--rw-r--r--   0 laike9m    (501) staff       (20)     4455 2022-07-03 05:10:51.291279 pdir2-0.3.6/tests/test_filters.py
--rw-r--r--   0 laike9m    (501) staff       (20)    14321 2022-07-03 05:10:51.291996 pdir2-0.3.6/tests/test_pdir_format.py
--rw-r--r--   0 laike9m    (501) staff       (20)     1368 2022-07-03 05:10:51.292842 pdir2-0.3.6/tests/test_search.py
--rw-r--r--   0 laike9m    (501) staff       (20)     2600 2022-07-03 05:10:51.293167 pdir2-0.3.6/tests/test_slots.py
--rw-r--r--   0 laike9m    (501) staff       (20)     4331 2022-07-03 05:10:51.294777 pdir2-0.3.6/tests/test_user_config.py
--rw-------   0 laike9m    (501) staff       (20)     4810 2022-07-03 05:16:01.010373 pdir2-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-06 01:11:13.424107 pdir2-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3536 2023-07-08 20:26:53.812929 pdir2-1.0.0/README.md
+-rw-r--r--   0        0        0      133 2023-07-06 01:11:13.427960 pdir2-1.0.0/pdir/__init__.py
+-rw-r--r--   0        0        0     2353 2023-07-06 01:11:13.428048 pdir2-1.0.0/pdir/_internal_utils.py
+-rw-r--r--   0        0        0     6711 2023-07-06 01:11:13.428162 pdir2-1.0.0/pdir/api.py
+-rw-r--r--   0        0        0    14495 2023-07-09 20:47:03.895414 pdir2-1.0.0/pdir/attr_category.py
+-rw-r--r--   0        0        0     1991 2023-07-06 01:11:13.428338 pdir2-1.0.0/pdir/color.py
+-rw-r--r--   0        0        0     3947 2023-07-08 06:01:19.918879 pdir2-1.0.0/pdir/configuration.py
+-rw-r--r--   0        0        0      341 2023-07-06 01:11:13.428483 pdir2-1.0.0/pdir/constants.py
+-rw-r--r--   0        0        0     3515 2023-07-09 20:54:24.984865 pdir2-1.0.0/pdir/format.py
+-rw-r--r--   0        0        0     1628 2023-07-09 21:55:12.456385 pdir2-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1577 2023-07-09 21:20:19.298532 pdir2-1.0.0/tests/conftest.py
+-rw-r--r--   0        0        0       85 2023-07-06 01:11:13.429205 pdir2-1.0.0/tests/data/config_1.ini
+-rw-r--r--   0        0        0       71 2023-07-06 01:11:13.429268 pdir2-1.0.0/tests/data/config_2.ini
+-rw-r--r--   0        0        0       39 2023-07-06 01:11:13.429326 pdir2-1.0.0/tests/data/config_auto_color.ini
+-rw-r--r--   0        0        0       40 2023-07-06 01:11:13.429384 pdir2-1.0.0/tests/data/config_disable_color.ini
+-rw-r--r--   0        0        0       39 2023-07-06 01:11:13.429448 pdir2-1.0.0/tests/data/config_enable_color.ini
+-rw-r--r--   0        0        0        0 2023-07-06 01:11:13.429473 pdir2-1.0.0/tests/data/empty_config.ini
+-rw-r--r--   0        0        0       49 2023-07-06 01:11:13.429546 pdir2-1.0.0/tests/data/error_config_1.ini
+-rw-r--r--   0        0        0       47 2023-07-06 01:11:13.429599 pdir2-1.0.0/tests/data/error_config_2.ini
+-rw-r--r--   0        0        0     1123 2023-07-06 01:11:13.429668 pdir2-1.0.0/tests/interactive_test.py
+-rw-r--r--   0        0        0      108 2023-07-06 01:11:13.429741 pdir2-1.0.0/tests/m.py
+-rw-r--r--   0        0        0     3580 2023-07-08 06:00:02.676001 pdir2-1.0.0/tests/test_buggy_attrs.py
+-rw-r--r--   0        0        0      606 2023-07-08 06:00:02.661487 pdir2-1.0.0/tests/test_container.py
+-rw-r--r--   0        0        0      203 2023-07-08 06:00:02.659623 pdir2-1.0.0/tests/test_disbale_color.py
+-rw-r--r--   0        0        0     4580 2023-07-08 07:03:54.085461 pdir2-1.0.0/tests/test_filters.py
+-rw-r--r--   0        0        0    14682 2023-07-08 07:03:54.085905 pdir2-1.0.0/tests/test_pdir_format.py
+-rw-r--r--   0        0        0     1368 2023-07-06 01:11:13.430190 pdir2-1.0.0/tests/test_search.py
+-rw-r--r--   0        0        0     2597 2023-07-08 06:00:02.681110 pdir2-1.0.0/tests/test_slots.py
+-rw-r--r--   0        0        0     4331 2023-07-06 01:11:13.430342 pdir2-1.0.0/tests/test_user_config.py
+-rw-r--r--   0        0        0     4569 1970-01-01 00:00:00.000000 pdir2-1.0.0/PKG-INFO
```

### Comparing `pdir2-0.3.6/LICENSE` & `pdir2-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdir2-0.3.6/README.md` & `pdir2-1.0.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # pdir2: Pretty dir() printing with joy
 
-[![Build Status](https://travis-ci.org/laike9m/pdir2.svg)](https://travis-ci.org/laike9m/pdir2)
+![Build status](https://github.com/laike9m/pdir2/actions/workflows/ci.yml/badge.svg)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/pdir2.svg)](https://pypi.python.org/pypi/pdir2/)
 ![PyPI Version](https://img.shields.io/pypi/v/pdir2.svg)
 <a href="https://github.com/ambv/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 
 Have you ever dreamed of a better output of `dir()`? I do. So I created this.
 
 ![](https://github.com/laike9m/pdir2/raw/master/images/presentation_v2.gif)
@@ -19,19 +19,19 @@
 
 -   Support [ipython](https://github.com/ipython/ipython), [ptpython](https://github.com/jonathanslenders/ptpython), [bpython](https://www.bpython-interpreter.org/) and [Jupyter Notebook](http://jupyter.org/)! See [wiki](https://github.com/laike9m/pdir2/wiki/REPL-Support) for details.
 
 -   The return value of `pdir()` can still be used as a list of names.
 
 -   ✨ Attribute searching
 
-    You can search for certain names with `.s()` or `.search()`:  
+    You can search for certain names with `.s()` or `.search()`:
 
     ![](https://github.com/laike9m/pdir2/raw/master/images/search.gif)
 
-    Search is case-insensitive by default.  
+    Search is case-insensitive by default.
      `search(name, case_sensitive=True)` does case-sensitive searching.
 
 -   :star2: Attribute filtering
 
     `properties`: Find properties/variables defined in the inspected object.
 
     `methods`: Find methods/functions defined in the inspected object.
@@ -72,16 +72,26 @@
 
 Then, create `.pythonstartup` in your home folder. Add one line:
 
     import pdir
 
 Next time you launch REPL, `pdir()` is already there, Hooray!
 
-## Testing
+## Development
 
-Simply run `pytest`, or use `tox` if you like.
+1. Set up development environment
 
-## Development
+   - **PDM**: pdir2 uses [PDM](https://pdm.fming.dev/latest/) to manage dependencies, so you want to make sure it's installed.
+   - **pyenv**: Since you need to test pdir2 on multiple Python versions, [pyenv](https://github.com/pyenv/pyenv) is highly recommended. Make sure you have Python 3.8, 3.9, 3.10 and 3.11 installed.
+
+2. Install dev dependencies
+
+   Simply run `pdm install`.
+
+   If you want to work on a specific Python version, run `pdm use [PYTHON_VERSION]` first to switch PDM to that version (e.g. `pdm use 3.9` if you want to debug a Python 3.9 specific issue).
+
+
+3. Run tests
+
+   Run `pdm run tox`
 
-Clone the source, run `make install_dev_packages`.   
-Don't forget to add proper type annotations,
-if you're not sure what to do, check out the `gen_type_info` section in `tox.ini`.
+The guide may be incomplete. Please file bugs if you encounter any issues.
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-# pdir2: Pretty dir() printing with joy [![Build Status](https://travis-ci.org/
-laike9m/pdir2.svg)](https://travis-ci.org/laike9m/pdir2) [![Supported Python
-versions](https://img.shields.io/pypi/pyversions/pdir2.svg)](https://
-pypi.python.org/pypi/pdir2/) ![PyPI Version](https://img.shields.io/pypi/v/
-pdir2.svg) [Code_style:_black] Have you ever dreamed of a better output of `dir
-()`? I do. So I created this. ![](https://github.com/laike9m/pdir2/raw/master/
-images/presentation_v2.gif) ## Features - Attributes are grouped by types/
+# pdir2: Pretty dir() printing with joy ![Build status](https://github.com/
+laike9m/pdir2/actions/workflows/ci.yml/badge.svg) [![Supported Python versions]
+(https://img.shields.io/pypi/pyversions/pdir2.svg)](https://pypi.python.org/
+pypi/pdir2/) ![PyPI Version](https://img.shields.io/pypi/v/pdir2.svg) [Code
+style:_black] Have you ever dreamed of a better output of `dir()`? I do. So I
+created this. ![](https://github.com/laike9m/pdir2/raw/master/images/
+presentation_v2.gif) ## Features - Attributes are grouped by types/
 functionalities, with beautiful colors. - Support color customization, [here's
 how](https://github.com/laike9m/pdir2/wiki/User-Configuration). - Support all
 platforms including Windows(Thanks to [colorama](https://github.com/tartley/
 colorama)). - Support [ipython](https://github.com/ipython/ipython), [ptpython]
 (https://github.com/jonathanslenders/ptpython), [bpython](https://www.bpython-
 interpreter.org/) and [Jupyter Notebook](http://jupyter.org/)! See [wiki]
 (https://github.com/laike9m/pdir2/wiki/REPL-Support) for details. - The return
@@ -27,11 +27,17 @@
 pdir2 About the name. I wanted to call it "pdir", but there's already one with
 this name on pypi. Mine is better, of course. ### Fedora dnf install python3-
 pdir2 --or-- dnf install python2-pdir2 ## Automatic Import As a better
 alternative of `dir()`, it's more convenient to automatically import pdir2 when
 launching REPL. Luckily, Python provides a way to do this. In you `.bashrc`(or
 `.zshrc`), add this line: export PYTHONSTARTUP=$HOME/.pythonstartup Then,
 create `.pythonstartup` in your home folder. Add one line: import pdir Next
-time you launch REPL, `pdir()` is already there, Hooray! ## Testing Simply run
-`pytest`, or use `tox` if you like. ## Development Clone the source, run `make
-install_dev_packages`. Don't forget to add proper type annotations, if you're
-not sure what to do, check out the `gen_type_info` section in `tox.ini`.
+time you launch REPL, `pdir()` is already there, Hooray! ## Development 1. Set
+up development environment - **PDM**: pdir2 uses [PDM](https://pdm.fming.dev/
+latest/) to manage dependencies, so you want to make sure it's installed. -
+**pyenv**: Since you need to test pdir2 on multiple Python versions, [pyenv]
+(https://github.com/pyenv/pyenv) is highly recommended. Make sure you have
+Python 3.8, 3.9, 3.10 and 3.11 installed. 2. Install dev dependencies Simply
+run `pdm install`. If you want to work on a specific Python version, run `pdm
+use [PYTHON_VERSION]` first to switch PDM to that version (e.g. `pdm use 3.9`
+if you want to debug a Python 3.9 specific issue). 3. Run tests Run `pdm run
+tox` The guide may be incomplete. Please file bugs if you encounter any issues.
```

### Comparing `pdir2-0.3.6/pdir/_internal_utils.py` & `pdir2-1.0.0/pdir/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `pdir2-0.3.6/pdir/api.py` & `pdir2-1.0.0/pdir/api.py`

 * *Files identical despite different names*

### Comparing `pdir2-0.3.6/pdir/attr_category.py` & `pdir2-1.0.0/pdir/attr_category.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     CLASS_CUSTOMIZATION = auto()
     CONTAINER = auto()
     COROUTINE = auto()
     COPY = auto()
     PICKLE = auto()
     PATTERN_MATCHING = auto()
     TYPING = auto()
+    DECORATOR = auto()
 
     def __str__(self) -> str:
         """
         e.g. RICH_COMPARISON -> rich comparison
         """
         return ' '.join(self.name.split('_')).lower()
 
@@ -214,14 +215,16 @@
     '__reduce__': (AttrCategory.PICKLE, AttrCategory.FUNCTION),
     '__reduce_ex__': (AttrCategory.PICKLE, AttrCategory.FUNCTION),
     '__match_args__': (AttrCategory.PATTERN_MATCHING, AttrCategory.PROPERTY),
     '__origin__': (AttrCategory.TYPING, AttrCategory.PROPERTY),
     '__args__': (AttrCategory.TYPING, AttrCategory.PROPERTY),
     '__parameters__': (AttrCategory.TYPING, AttrCategory.PROPERTY),
     '__class_getitem__': (AttrCategory.TYPING, AttrCategory.FUNCTION),
+    '__final__': (AttrCategory.TYPING, AttrCategory.PROPERTY),
+    '__wrapped__': (AttrCategory.DECORATOR, AttrCategory.PROPERTY),
 }
 
 
 def attr_category_postprocess(get_attr_category_func):
     """Unifies attr_category to a tuple, add AttrCategory.SLOT if needed."""
 
     @functools.wraps(get_attr_category_func)
```

### Comparing `pdir2-0.3.6/pdir/color.py` & `pdir2-1.0.0/pdir/color.py`

 * *Files identical despite different names*

### Comparing `pdir2-0.3.6/pdir/configuration.py` & `pdir2-1.0.0/pdir/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
         'doc-color',
         'slot-color',
     }
 )
 
 
 class Configuration:
-
     _uniform_color = None
     _enable_colorful_output = None
     _category_color = COLORS['yellow']
     _attribute_color = COLORS['cyan']
     _comma_color = COLORS['grey']
     _doc_color = COLORS['grey']
     _slot_color = COLORS['magenta']
```

### Comparing `pdir2-0.3.6/pdir/format.py` & `pdir2-1.0.0/pdir/format.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,8 +88,9 @@
     AttrCategory.CONTAINER: _single_line,
     AttrCategory.COROUTINE: _single_line,
     AttrCategory.COPY: _single_line,
     AttrCategory.PICKLE: _single_line,
     AttrCategory.ABSTRACT_CLASS: _single_line,
     AttrCategory.PATTERN_MATCHING: _single_line,
     AttrCategory.TYPING: _single_line,
+    AttrCategory.DECORATOR: _single_line,
 }
```

### Comparing `pdir2-0.3.6/pyproject.toml` & `pdir2-1.0.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [project]
 name = "pdir2"
-version = "0.3.6"
+version = "1.0.0"
 authors = [
     { name = "laike9m", email = "laike9m@gmail.com" },
 ]
 dependencies = [
     "colorama;platform_system==\"Windows\"",
-    "typing-extensions==4.2.*",
+    "typing-extensions==4.*",
 ]
-requires-python = ">=3.7.1,<3.11"
+requires-python = ">=3.8"
 description = "Pretty dir printing with joy"
 readme = "README.md"
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows",
@@ -30,29 +30,29 @@
 
 [project.urls]
 Funding = "https://github.com/sponsors/laike9m"
 "Bug Tracker" = "https://github.com/laike9m/pdir2/issues"
 homepage = "https://github.com/laike9m/pdir2"
 repository = "https://github.com/laike9m/pdir2"
 
-[project.optional-dependencies]
-
 [tool.pdm.dev-dependencies]
 dev = [
-    "pytest==6.2.*",
-    "tox==3.24.*",
+    "pytest==7.*",
+    "tox==4.*",
     "tox-pdm==0.5.*",
     "ptpython==3.0.*",
-    "bpython==0.21.*",
+    "bpython>=0.24",
     "ipython==7.16.*",
     "flake8==3.9.*",
-    "pytest-mypy==0.8.*",
-    "pandas==1.3.5",
+    "pytest-mypy==0.10.*",
+    "pandas==2.*",
     "hypothesis==6.21.*",
-    "tox-gh-actions==2.8.*",
+    "tox-gh-actions==3.*",
+    "mypy>=1.4",
+    "twine>=4.0.2",
 ]
 
 [tool.black]
 skip-string-normalization = true
 
 [[tool.mypy.overrides]]
 module = [
```

### Comparing `pdir2-0.3.6/tests/conftest.py` & `pdir2-1.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pdir2-0.3.6/tests/interactive_test.py` & `pdir2-1.0.0/tests/interactive_test.py`

 * *Files identical despite different names*

### Comparing `pdir2-0.3.6/tests/test_buggy_attrs.py` & `pdir2-1.0.0/tests/test_buggy_attrs.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,14 @@
             )
         if pattr.name == 'p':
             assert category_match(pattr.category, AttrCategory.DESCRIPTOR)
             assert pattr.doc == ('@property with getter, setter, ' 'deleter, this is p')
 
 
 def test_override_dir():
-
     # In the class attrs in `__dir__()` can not be found in `__dict__`
     class ClassWithUserDefinedDir:
         def __dir__(self):
             return ['foo']
 
     inst = ClassWithUserDefinedDir()
     pattrs = pdir(inst).pattrs
```

### Comparing `pdir2-0.3.6/tests/test_container.py` & `pdir2-1.0.0/tests/test_container.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 import pdir
 
 
 def test_acting_like_a_list():
-
     dadada = 1
     cadada = 1
     vadada = 1
     apple1 = 1
     xapple2 = 1
     result, correct = pdir(), dir()
     assert len(correct) == len(result)
 
     for x, y in zip(correct, result):
         assert x == y
 
 
 def test_acting_like_a_list_when_search():
-
     dadada = 1
     cadada = 1
     vadada = 1
     apple1 = 1
     xapple2 = 1
     result = pdir().s('apple')
     assert len(result) == 2
     assert list(result) == ['apple1', 'xapple2']
 
 
 def test_attr_order():
-
     dir_attrs = dir(None)
     pdir_attrs = list(pdir(None))
     assert dir_attrs == pdir_attrs
```

### Comparing `pdir2-0.3.6/tests/test_filters.py` & `pdir2-1.0.0/tests/test_filters.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 import collections
 import sys
 import pdir
 
 
 # https://github.com/python/cpython/blob/da2bf9f66d0c95b988c5d87646d168f65499b316/Lib/unittest/case.py#L1164-L1195
-def items_equal(first, second):
+def check_items_equality(first, second):
     """A simplified version of the unittest.assertEqual method."""
     first_seq, second_seq = list(first), list(second)
     first = collections.Counter(first_seq)
     second = collections.Counter(second_seq)
-    return first == second
+    assert first == second
 
 
 class Base:
     base_class_variable = 1
 
     def __init__(self):
         self.base_instance_variable = 2
@@ -37,16 +37,15 @@
         pass
 
 
 inst = DerivedClass()
 
 
 def test_properties():
-
-    assert items_equal(
+    check_items_equality(
         [p.name for p in pdir(inst).properties.pattrs],
         [
             'base_class_variable',
             'base_instance_variable',
             'derived_class_variable',
             'derived_instance_variable',
             '__class__',
@@ -55,17 +54,16 @@
             '__module__',
             '__weakref__',
         ],
     )
 
 
 def test_methods():
-
     if sys.version[0] == '2':
-        assert items_equal(
+        check_items_equality(
             [p.name for p in pdir(inst).methods.pattrs],
             [
                 '__subclasshook__',
                 '__delattr__',
                 '__getattribute__',
                 '__setattr__',
                 'base_method',
@@ -78,15 +76,16 @@
                 '__sizeof__',
                 '__str__',
                 '__reduce__',
                 '__reduce_ex__',
             ],
         )
     else:
-        assert items_equal(
+        extra_items = ['__getstate__'] if sys.version_info >= (3, 11) else []
+        check_items_equality(
             [p.name for p in pdir(inst).methods.pattrs],
             [
                 '__subclasshook__',
                 '__delattr__',
                 '__dir__',
                 '__getattribute__',
                 '__setattr__',
@@ -104,83 +103,80 @@
                 '__reduce_ex__',
                 '__eq__',
                 '__ge__',
                 '__gt__',
                 '__le__',
                 '__lt__',
                 '__ne__',
-            ],
+            ]
+            + extra_items,
         )
 
 
 def test_public():
-
-    assert items_equal(
+    check_items_equality(
         [p.name for p in pdir(inst).public.pattrs],
         [
             'base_method',
             'derived_method',
             'base_class_variable',
             'base_instance_variable',
             'derived_class_variable',
             'derived_instance_variable',
         ],
     )
 
 
 def test_own():
-
-    assert items_equal(
+    check_items_equality(
         [p.name for p in pdir(inst).own.pattrs],
         [
             'derived_method',
             '__init__',
             'base_instance_variable',
             'derived_class_variable',
             'derived_instance_variable',
             '__doc__',
             '__module__',
         ],
     )
 
 
 def test_chained_filters():
-
-    assert items_equal(
+    check_items_equality(
         [p.name for p in pdir(inst).public.own.properties.pattrs],
         [
             'base_instance_variable',
             'derived_class_variable',
             'derived_instance_variable',
         ],
     )
 
 
 def test_order_of_chained_filters():
-
-    assert items_equal(
+    check_items_equality(
         [p.name for p in pdir(inst).own.properties.public.pattrs],
         [
             'base_instance_variable',
             'derived_class_variable',
             'derived_instance_variable',
         ],
     )
-    assert items_equal(
+    check_items_equality(
         [p.name for p in pdir(inst).properties.public.own.pattrs],
         [
             'base_instance_variable',
             'derived_class_variable',
             'derived_instance_variable',
         ],
     )
 
 
 def test_filters_with_search():
     def test_chained_filters():
-        assert items_equal(
+        check_items_equality(
             [
                 p.name
                 for p in pdir(inst).public.own.properties.search('derived_in').pattrs
             ],
             ['derived_instance_variable'],
         )
```

### Comparing `pdir2-0.3.6/tests/test_pdir_format.py` & `pdir2-1.0.0/tests/test_pdir_format.py`

 * *Files 2% similar despite different names*

```diff
@@ -324,16 +324,24 @@
                     '\x1b[0m\x1b[0;36m__getattribute__\x1b[0m\x1b[1;30m, '
                     '\x1b[0m\x1b[0;36m__setattr__\x1b[0m'
                 ),
                 '\x1b[0;33mclass customization:\x1b[0m',
                 '    \x1b[0;36m__init_subclass__\x1b[0m',
                 '\x1b[0;33mpickle:\x1b[0m',
                 (
-                    '    \x1b[0;36m__reduce__\x1b[0m\x1b[1;30m, '
-                    '\x1b[0m\x1b[0;36m__reduce_ex__\x1b[0m'
+                    (
+                        '    \x1b[0;36m__getstate__\x1b[0m\x1b[1;30m, '
+                        '\x1b[0m\x1b[0;36m__reduce__\x1b[0m\x1b[1;30m, '
+                        '\x1b[0m\x1b[0;36m__reduce_ex__\x1b[0m'
+                    )
+                    if sys.version_info >= (3, 11)
+                    else (
+                        '    \x1b[0;36m__reduce__\x1b[0m\x1b[1;30m, '
+                        '\x1b[0m\x1b[0;36m__reduce_ex__\x1b[0m'
+                    )
                 ),
                 '\x1b[0;33mdescriptor:\x1b[0m',
                 (
                     '    \x1b[0;36ma\x1b[0m'
                     '\x1b[0;35m(slotted)\x1b[0m\x1b[0;36m: '
                     '\x1b[0m\x1b[1;30mclass member_descriptor with '
                     'getter, setter, deleter\x1b[0m'
```

### Comparing `pdir2-0.3.6/tests/test_search.py` & `pdir2-1.0.0/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `pdir2-0.3.6/tests/test_slots.py` & `pdir2-1.0.0/tests/test_slots.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,14 @@
 
 
 class DeriveSlotBaseSlot(BaseSlot):
     __slots__ = [DERIVE]
 
 
 def test_not_set():
-
     expected_res = [  # class type    empty slot attr num
         (DeriveNoSlotBaseEmpty, 0),
         (DeriveNoSlotBaseSlot, 1),
         (DeriveEmptySlotBaseNo, 0),
         (DeriveEmptySlotBaseEmpty, 0),
         (DeriveEmptySlotBaseSlot, 1),
         (DeriveSlotBaseNo, 1),
@@ -74,15 +73,14 @@
                 attr_count += 1
                 assert category_match(attr.category, AttrCategory.DESCRIPTOR)
                 assert category_match(attr.category, AttrCategory.SLOT)
         assert attr_count == attr_num
 
 
 def test_set_derive():
-
     c_types = [DeriveSlotBaseNo, DeriveSlotBaseEmpty, DeriveSlotBaseSlot]
     for c_type in c_types:
         instance = c_type()
         instance.derive = 'foo'
         for attr in pdir(instance).pattrs:
             if attr.name == DERIVE:
                 assert category_match(attr.category, AttrCategory.DESCRIPTOR)
@@ -90,15 +88,14 @@
                 break
         else:
             # No derive attribute found
             assert False
 
 
 def test_set_base():
-
     c_types = [DeriveNoSlotBaseSlot, DeriveEmptySlotBaseSlot, DeriveSlotBaseSlot]
     for c_type in c_types:
         instance = c_type()
         instance.base = 'foo'
         for attr in pdir(instance).pattrs:
             if attr.name == BASE:
                 assert category_match(attr.category, AttrCategory.DESCRIPTOR)
```

### Comparing `pdir2-0.3.6/tests/test_user_config.py` & `pdir2-1.0.0/tests/test_user_config.py`

 * *Files identical despite different names*

### Comparing `pdir2-0.3.6/PKG-INFO` & `pdir2-1.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pdir2
-Version: 0.3.6
+Version: 1.0.0
 Summary: Pretty dir printing with joy
 License: MIT
 Author-email: laike9m <laike9m@gmail.com>
-Requires-Python: >=3.7.1,<3.11
+Requires-Python: >=3.8
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
@@ -17,95 +17,106 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Project-URL: Bug Tracker, https://github.com/laike9m/pdir2/issues
 Project-URL: Funding, https://github.com/sponsors/laike9m
 Project-URL: homepage, https://github.com/laike9m/pdir2
 Project-URL: repository, https://github.com/laike9m/pdir2
 Description-Content-Type: text/markdown
-Description: # pdir2: Pretty dir() printing with joy
-        
-        [![Build Status](https://travis-ci.org/laike9m/pdir2.svg)](https://travis-ci.org/laike9m/pdir2)
-        [![Supported Python versions](https://img.shields.io/pypi/pyversions/pdir2.svg)](https://pypi.python.org/pypi/pdir2/)
-        ![PyPI Version](https://img.shields.io/pypi/v/pdir2.svg)
-        <a href="https://github.com/ambv/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
-        
-        Have you ever dreamed of a better output of `dir()`? I do. So I created this.
-        
-        ![](https://github.com/laike9m/pdir2/raw/master/images/presentation_v2.gif)
-        
-        ## Features
-        
-        -   Attributes are grouped by types/functionalities, with beautiful colors.
-        
-        -   Support color customization, [here's how](https://github.com/laike9m/pdir2/wiki/User-Configuration).
-        
-        -   Support all platforms including Windows(Thanks to [colorama](https://github.com/tartley/colorama)).
-        
-        -   Support [ipython](https://github.com/ipython/ipython), [ptpython](https://github.com/jonathanslenders/ptpython), [bpython](https://www.bpython-interpreter.org/) and [Jupyter Notebook](http://jupyter.org/)! See [wiki](https://github.com/laike9m/pdir2/wiki/REPL-Support) for details.
-        
-        -   The return value of `pdir()` can still be used as a list of names.
-        
-        -   ✨ Attribute searching
-        
-            You can search for certain names with `.s()` or `.search()`:  
-        
-            ![](https://github.com/laike9m/pdir2/raw/master/images/search.gif)
-        
-            Search is case-insensitive by default.  
-             `search(name, case_sensitive=True)` does case-sensitive searching.
-        
-        -   :star2: Attribute filtering
-        
-            `properties`: Find properties/variables defined in the inspected object.
-        
-            `methods`: Find methods/functions defined in the inspected object.
-        
-            `public`: Find public attributes.
-        
-            `own`: Find attributes that are not inherited from parent classes.
-        
-            These filters **can be chained!** Order does **NOT** matter.
-        
-            For example, use `pdir(obj).public.own.methods` to find all public own methods.
-        
-            You can also call `search` on the returned results.
-        
-            See a [complete example](https://github.com/laike9m/pdir2/wiki/Attribute-Filtering).
-        
-        ## Install
-        
-        ### Generic
-        
-            pip install pdir2
-        
-        About the name. I wanted to call it "pdir", but there's already one with this
-        name on pypi. Mine is better, of course.
-        
-        ### Fedora
-        
-            dnf install python3-pdir2
-            --or--
-            dnf install python2-pdir2
-        
-        ## Automatic Import
-        
-        As a better alternative of `dir()`, it's more convenient to automatically import
-        pdir2 when launching REPL. Luckily, Python provides a way to do this. In you `.bashrc`(or `.zshrc`), add this line:
-        
-            export PYTHONSTARTUP=$HOME/.pythonstartup
-        
-        Then, create `.pythonstartup` in your home folder. Add one line:
-        
-            import pdir
-        
-        Next time you launch REPL, `pdir()` is already there, Hooray!
-        
-        ## Testing
-        
-        Simply run `pytest`, or use `tox` if you like.
-        
-        ## Development
-        
-        Clone the source, run `make install_dev_packages`.   
-        Don't forget to add proper type annotations,
-        if you're not sure what to do, check out the `gen_type_info` section in `tox.ini`.
+
+# pdir2: Pretty dir() printing with joy
+
+![Build status](https://github.com/laike9m/pdir2/actions/workflows/ci.yml/badge.svg)
+[![Supported Python versions](https://img.shields.io/pypi/pyversions/pdir2.svg)](https://pypi.python.org/pypi/pdir2/)
+![PyPI Version](https://img.shields.io/pypi/v/pdir2.svg)
+<a href="https://github.com/ambv/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
+
+Have you ever dreamed of a better output of `dir()`? I do. So I created this.
+
+![](https://github.com/laike9m/pdir2/raw/master/images/presentation_v2.gif)
+
+## Features
+
+-   Attributes are grouped by types/functionalities, with beautiful colors.
+
+-   Support color customization, [here's how](https://github.com/laike9m/pdir2/wiki/User-Configuration).
+
+-   Support all platforms including Windows(Thanks to [colorama](https://github.com/tartley/colorama)).
+
+-   Support [ipython](https://github.com/ipython/ipython), [ptpython](https://github.com/jonathanslenders/ptpython), [bpython](https://www.bpython-interpreter.org/) and [Jupyter Notebook](http://jupyter.org/)! See [wiki](https://github.com/laike9m/pdir2/wiki/REPL-Support) for details.
+
+-   The return value of `pdir()` can still be used as a list of names.
+
+-   ✨ Attribute searching
+
+    You can search for certain names with `.s()` or `.search()`:
+
+    ![](https://github.com/laike9m/pdir2/raw/master/images/search.gif)
+
+    Search is case-insensitive by default.
+     `search(name, case_sensitive=True)` does case-sensitive searching.
+
+-   :star2: Attribute filtering
+
+    `properties`: Find properties/variables defined in the inspected object.
+
+    `methods`: Find methods/functions defined in the inspected object.
+
+    `public`: Find public attributes.
+
+    `own`: Find attributes that are not inherited from parent classes.
+
+    These filters **can be chained!** Order does **NOT** matter.
+
+    For example, use `pdir(obj).public.own.methods` to find all public own methods.
+
+    You can also call `search` on the returned results.
+
+    See a [complete example](https://github.com/laike9m/pdir2/wiki/Attribute-Filtering).
+
+## Install
+
+### Generic
+
+    pip install pdir2
+
+About the name. I wanted to call it "pdir", but there's already one with this
+name on pypi. Mine is better, of course.
+
+### Fedora
+
+    dnf install python3-pdir2
+    --or--
+    dnf install python2-pdir2
+
+## Automatic Import
+
+As a better alternative of `dir()`, it's more convenient to automatically import
+pdir2 when launching REPL. Luckily, Python provides a way to do this. In you `.bashrc`(or `.zshrc`), add this line:
+
+    export PYTHONSTARTUP=$HOME/.pythonstartup
+
+Then, create `.pythonstartup` in your home folder. Add one line:
+
+    import pdir
+
+Next time you launch REPL, `pdir()` is already there, Hooray!
+
+## Development
+
+1. Set up development environment
+
+   - **PDM**: pdir2 uses [PDM](https://pdm.fming.dev/latest/) to manage dependencies, so you want to make sure it's installed.
+   - **pyenv**: Since you need to test pdir2 on multiple Python versions, [pyenv](https://github.com/pyenv/pyenv) is highly recommended. Make sure you have Python 3.8, 3.9, 3.10 and 3.11 installed.
+
+2. Install dev dependencies
+
+   Simply run `pdm install`.
+
+   If you want to work on a specific Python version, run `pdm use [PYTHON_VERSION]` first to switch PDM to that version (e.g. `pdm use 3.9` if you want to debug a Python 3.9 specific issue).
+
+
+3. Run tests
+
+   Run `pdm run tox`
+
+The guide may be incomplete. Please file bugs if you encounter any issues.
```

#### html2text {}

```diff
@@ -1,51 +1,57 @@
-Metadata-Version: 2.1 Name: pdir2 Version: 0.3.6 Summary: Pretty dir printing
+Metadata-Version: 2.1 Name: pdir2 Version: 1.0.0 Summary: Pretty dir printing
 with joy License: MIT Author-email: laike9m
-gmail.com> Requires-Python: >=3.7.1,<3.11 Classifier: Intended Audience ::
-Developers Classifier: License :: OSI Approved :: MIT License Classifier:
-Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
-:: Windows Classifier: Operating System :: POSIX Classifier: Programming
-Language :: Python Classifier: Programming Language :: Python :: 2 Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: Implementation :: CPython Classifier: Programming Language :: Python ::
+gmail.com> Requires-Python: >=3.8 Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: MacOS :: MacOS X Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX Classifier: Programming Language ::
+Python Classifier: Programming Language :: Python :: 2 Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python ::
+Implementation :: CPython Classifier: Programming Language :: Python ::
 Implementation :: PyPy Classifier: Topic :: Software Development :: Libraries
 :: Python Modules Project-URL: Bug Tracker, https://github.com/laike9m/pdir2/
 issues Project-URL: Funding, https://github.com/sponsors/laike9m Project-URL:
 homepage, https://github.com/laike9m/pdir2 Project-URL: repository, https://
-github.com/laike9m/pdir2 Description-Content-Type: text/markdown Description: #
-pdir2: Pretty dir() printing with joy [![Build Status](https://travis-ci.org/
-laike9m/pdir2.svg)](https://travis-ci.org/laike9m/pdir2) [![Supported Python
-versions](https://img.shields.io/pypi/pyversions/pdir2.svg)](https://
-pypi.python.org/pypi/pdir2/) ![PyPI Version](https://img.shields.io/pypi/v/
-pdir2.svg) [Code_style:_black] Have you ever dreamed of a better output of `dir
-()`? I do. So I created this. ![](https://github.com/laike9m/pdir2/raw/master/
-images/presentation_v2.gif) ## Features - Attributes are grouped by types/
-functionalities, with beautiful colors. - Support color customization, [here's
-how](https://github.com/laike9m/pdir2/wiki/User-Configuration). - Support all
-platforms including Windows(Thanks to [colorama](https://github.com/tartley/
-colorama)). - Support [ipython](https://github.com/ipython/ipython), [ptpython]
-(https://github.com/jonathanslenders/ptpython), [bpython](https://www.bpython-
-interpreter.org/) and [Jupyter Notebook](http://jupyter.org/)! See [wiki]
-(https://github.com/laike9m/pdir2/wiki/REPL-Support) for details. - The return
-value of `pdir()` can still be used as a list of names. - â¨ Attribute
-searching You can search for certain names with `.s()` or `.search()`: ![]
-(https://github.com/laike9m/pdir2/raw/master/images/search.gif) Search is case-
-insensitive by default. `search(name, case_sensitive=True)` does case-sensitive
-searching. - :star2: Attribute filtering `properties`: Find properties/
-variables defined in the inspected object. `methods`: Find methods/functions
-defined in the inspected object. `public`: Find public attributes. `own`: Find
-attributes that are not inherited from parent classes. These filters **can be
-chained!** Order does **NOT** matter. For example, use `pdir
-(obj).public.own.methods` to find all public own methods. You can also call
-`search` on the returned results. See a [complete example](https://github.com/
-laike9m/pdir2/wiki/Attribute-Filtering). ## Install ### Generic pip install
-pdir2 About the name. I wanted to call it "pdir", but there's already one with
-this name on pypi. Mine is better, of course. ### Fedora dnf install python3-
-pdir2 --or-- dnf install python2-pdir2 ## Automatic Import As a better
-alternative of `dir()`, it's more convenient to automatically import pdir2 when
-launching REPL. Luckily, Python provides a way to do this. In you `.bashrc`(or
-`.zshrc`), add this line: export PYTHONSTARTUP=$HOME/.pythonstartup Then,
-create `.pythonstartup` in your home folder. Add one line: import pdir Next
-time you launch REPL, `pdir()` is already there, Hooray! ## Testing Simply run
-`pytest`, or use `tox` if you like. ## Development Clone the source, run `make
-install_dev_packages`. Don't forget to add proper type annotations, if you're
-not sure what to do, check out the `gen_type_info` section in `tox.ini`.
+github.com/laike9m/pdir2 Description-Content-Type: text/markdown # pdir2:
+Pretty dir() printing with joy ![Build status](https://github.com/laike9m/
+pdir2/actions/workflows/ci.yml/badge.svg) [![Supported Python versions](https:/
+/img.shields.io/pypi/pyversions/pdir2.svg)](https://pypi.python.org/pypi/pdir2/
+) ![PyPI Version](https://img.shields.io/pypi/v/pdir2.svg) [Code_style:_black]
+Have you ever dreamed of a better output of `dir()`? I do. So I created this. !
+[](https://github.com/laike9m/pdir2/raw/master/images/presentation_v2.gif) ##
+Features - Attributes are grouped by types/functionalities, with beautiful
+colors. - Support color customization, [here's how](https://github.com/laike9m/
+pdir2/wiki/User-Configuration). - Support all platforms including Windows
+(Thanks to [colorama](https://github.com/tartley/colorama)). - Support
+[ipython](https://github.com/ipython/ipython), [ptpython](https://github.com/
+jonathanslenders/ptpython), [bpython](https://www.bpython-interpreter.org/) and
+[Jupyter Notebook](http://jupyter.org/)! See [wiki](https://github.com/laike9m/
+pdir2/wiki/REPL-Support) for details. - The return value of `pdir()` can still
+be used as a list of names. - â¨ Attribute searching You can search for
+certain names with `.s()` or `.search()`: ![](https://github.com/laike9m/pdir2/
+raw/master/images/search.gif) Search is case-insensitive by default. `search
+(name, case_sensitive=True)` does case-sensitive searching. - :star2: Attribute
+filtering `properties`: Find properties/variables defined in the inspected
+object. `methods`: Find methods/functions defined in the inspected object.
+`public`: Find public attributes. `own`: Find attributes that are not inherited
+from parent classes. These filters **can be chained!** Order does **NOT**
+matter. For example, use `pdir(obj).public.own.methods` to find all public own
+methods. You can also call `search` on the returned results. See a [complete
+example](https://github.com/laike9m/pdir2/wiki/Attribute-Filtering). ## Install
+### Generic pip install pdir2 About the name. I wanted to call it "pdir", but
+there's already one with this name on pypi. Mine is better, of course. ###
+Fedora dnf install python3-pdir2 --or-- dnf install python2-pdir2 ## Automatic
+Import As a better alternative of `dir()`, it's more convenient to
+automatically import pdir2 when launching REPL. Luckily, Python provides a way
+to do this. In you `.bashrc`(or `.zshrc`), add this line: export
+PYTHONSTARTUP=$HOME/.pythonstartup Then, create `.pythonstartup` in your home
+folder. Add one line: import pdir Next time you launch REPL, `pdir()` is
+already there, Hooray! ## Development 1. Set up development environment -
+**PDM**: pdir2 uses [PDM](https://pdm.fming.dev/latest/) to manage
+dependencies, so you want to make sure it's installed. - **pyenv**: Since you
+need to test pdir2 on multiple Python versions, [pyenv](https://github.com/
+pyenv/pyenv) is highly recommended. Make sure you have Python 3.8, 3.9, 3.10
+and 3.11 installed. 2. Install dev dependencies Simply run `pdm install`. If
+you want to work on a specific Python version, run `pdm use [PYTHON_VERSION]`
+first to switch PDM to that version (e.g. `pdm use 3.9` if you want to debug a
+Python 3.9 specific issue). 3. Run tests Run `pdm run tox` The guide may be
+incomplete. Please file bugs if you encounter any issues.
```

