# Comparing `tmp/ixbrlparse-0.5.4.tar.gz` & `tmp/ixbrlparse-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ixbrlparse-0.5.4.tar", last modified: Sun Jul  9 08:52:22 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `ixbrlparse-0.5.4.tar` & `ixbrlparse-0.6.0.tar`

### file list

```diff
@@ -1,27 +1,5 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 08:52:22.006368 ixbrlparse-0.5.4/
--rw-rw-rw-   0        0        0     1088 2020-02-25 22:10:31.000000 ixbrlparse-0.5.4/LICENSE
--rw-rw-rw-   0        0        0     7433 2023-07-09 08:52:22.004371 ixbrlparse-0.5.4/PKG-INFO
--rw-rw-rw-   0        0        0     6656 2023-07-09 08:45:00.000000 ixbrlparse-0.5.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-09 08:52:21.955374 ixbrlparse-0.5.4/ixbrlparse/
--rw-rw-rw-   0        0        0       97 2022-11-16 21:23:50.000000 ixbrlparse-0.5.4/ixbrlparse/__init__.py
--rw-rw-rw-   0        0        0     1907 2022-11-16 21:16:55.000000 ixbrlparse-0.5.4/ixbrlparse/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 08:52:21.994372 ixbrlparse-0.5.4/ixbrlparse/components/
--rw-rw-rw-   0        0        0      176 2022-12-20 14:20:48.000000 ixbrlparse-0.5.4/ixbrlparse/components/__init__.py
--rw-rw-rw-   0        0        0     1644 2022-12-20 14:20:48.000000 ixbrlparse-0.5.4/ixbrlparse/components/context.py
--rw-rw-rw-   0        0        0     1052 2023-07-09 08:39:20.000000 ixbrlparse-0.5.4/ixbrlparse/components/nonnumeric.py
--rw-rw-rw-   0        0        0     2403 2023-07-09 08:47:05.000000 ixbrlparse-0.5.4/ixbrlparse/components/numeric.py
--rw-rw-rw-   0        0        0     4066 2022-11-16 23:59:06.000000 ixbrlparse-0.5.4/ixbrlparse/components/transform.py
--rw-rw-rw-   0        0        0    14082 2023-07-09 08:39:20.000000 ixbrlparse-0.5.4/ixbrlparse/core.py
--rw-rw-rw-   0        0        0        0 2022-11-16 21:16:55.000000 ixbrlparse-0.5.4/ixbrlparse/utils.py
--rw-rw-rw-   0        0        0       23 2023-07-09 08:44:24.000000 ixbrlparse-0.5.4/ixbrlparse/version.py
-drwxrwxrwx   0        0        0        0 2023-07-09 08:52:21.980367 ixbrlparse-0.5.4/ixbrlparse.egg-info/
--rw-rw-rw-   0        0        0     7433 2023-07-09 08:52:21.000000 ixbrlparse-0.5.4/ixbrlparse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      515 2023-07-09 08:52:21.000000 ixbrlparse-0.5.4/ixbrlparse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 08:52:21.000000 ixbrlparse-0.5.4/ixbrlparse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-07-09 08:52:21.000000 ixbrlparse-0.5.4/ixbrlparse.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-09 08:52:21.000000 ixbrlparse-0.5.4/ixbrlparse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-09 08:52:22.006368 ixbrlparse-0.5.4/setup.cfg
--rw-rw-rw-   0        0        0     1149 2022-11-16 23:59:06.000000 ixbrlparse-0.5.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-09 08:52:22.000368 ixbrlparse-0.5.4/tests/
--rw-rw-rw-   0        0        0     9070 2022-12-20 20:32:07.000000 ixbrlparse-0.5.4/tests/test_classes.py
--rw-rw-rw-   0        0        0    14270 2023-07-09 08:42:01.000000 ixbrlparse-0.5.4/tests/test_parse.py
+-rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 ixbrlparse-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 ixbrlparse-0.6.0/LICENSE
+-rw-r--r--   0        0        0     6234 2020-02-02 00:00:00.000000 ixbrlparse-0.6.0/README.md
+-rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 ixbrlparse-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     7038 2020-02-02 00:00:00.000000 ixbrlparse-0.6.0/PKG-INFO
```

### Comparing `ixbrlparse-0.5.4/LICENSE` & `ixbrlparse-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ixbrlparse-0.5.4/PKG-INFO` & `ixbrlparse-0.6.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,242 +1,255 @@
-Metadata-Version: 2.1
-Name: ixbrlparse
-Version: 0.5.4
-Summary: A python module for getting useful data out of ixbrl files.
-Home-page: https://github.com/drkane/ixbrl-parse
-Author: David Kane
-Author-email: david@dkane.net
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# ixbrl-parse
-
-
-![Test status](https://github.com/drkane/ixbrl-parse/workflows/tests/badge.svg)
-[![PyPI version](https://img.shields.io/pypi/v/ixbrlparse)](https://pypi.org/project/ixbrlparse/)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ixbrlparse)
-![PyPI - License](https://img.shields.io/pypi/l/ixbrlparse)
-
-A python module for getting useful data out of ixbrl files. The library is at an early stage - feedback and improvements are very welcome.
-
-**New in version 0.5.4**: Added backreferences to BeautifulSoup objects - thanks to @avyfain for PR.
-
-**New in version 0.5.3**: Support for `exclude` and `continuation` elements within XBRL documents. Thanks to @wcollinscw for adding support for exclude elements.
-
-**New in version 0.5**: Support for Python 3.11 has been added. I've had some problems with Python 3.11 and Windows as lxml binaries aren't yet available. Also new in version 0.5 is type checking - the whole library now has types added. 
-
-**New in version 0.4**: I've added initial support for pure XBRL files as well as tagged HTML iXBRL files. Feedback on this feature is welcome - particularly around getting values out of numeric items.
-
-## Requirements
-
-The module requires [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/) and [lxml](https://lxml.de/) to parse the documents.
-
-[word2number](https://github.com/akshaynagpal/w2n) is used to process the
-numeric items with the `numsenwords` format.
-
-## How to install
-
-You can install from pypi using pip:
-
-```
-pip install ixbrlparse
-```
-
-## How to use
-
-### Run the python module
-
-You can run the module directly to extract data from an IXBRL file.
-
-```bash
-python -m ixbrlparse example_file.html
-```
-
-The various options for using this can be found through:
-
-```bash
-python -m ixbrlparse -h
-# optional arguments:
-#   -h, --help            show this help message and exit
-#   --outfile OUTFILE     Where to output the file
-#   --format {csv,json,jsonlines,jsonl}
-#                         format of the output
-#   --fields {numeric,nonnumeric,all}
-#                         Which fields to output
-```
-
-### Use as a python module
-
-An example of usage is shown in [`test.py`](test.py).
-
-#### Import the `IXBRL` class which parses the file.
-
-```python
-from ixbrlparse import IXBRL
-```
-
-#### Initialise an object and parse the file
-
-You need to pass a file handle or other object with a `.read()` method.
-
-```python
-with open('sample_ixbrl.html', encoding="utf8") as a:
-  x = IXBRL(a)
-```
-
-If your IXBRL data comes as a string then use a `io.StringIO` wrapper to
-pass it to the class:
-
-```python
-import io
-from ixbrlparse import IXBRL
-
-content = '''<some ixbrl content>'''
-x = IXBRL(io.StringIO(content))
-```
-
-
-#### Get the contexts and units used in the data
-
-These are held in the object. The contexts are stored as a dictionary with the context
-id as the key, and a `ixbrlContext` object as the value.
-
-```python
-print(x.contexts)
-# {
-#    "cfwd_2018_03_31": ixbrlContext(
-#       id="cfwd_2018_03_31",
-#       entity="0123456", # company number
-#       segments=[], # used for hypercubes
-#       instant="2018-03-31",
-#       startdate=None, # used for periods
-#       enddate=None, # used for periods
-#    ),
-#    ....
-# }
-```
-
-The units are stored as key:value dictionary entries
-```python
-print(x.units)
-# {
-#    "GBP": "ISO4107:GBP"
-#    "shares": "shares"
-# }
-```
-
-#### Get financial facts
-
-Numeric facts are stored in `x.numeric` as a list of `ixbrlNumeric` objects.
-The `ixbrlNumeric.value` object contains the value as a parsed python number
-(after the sign and scale formatting values have been applied).
-
-`ixbrlNumeric.context` holds the context object relating to this value.
-The `.name` and `.schema` values give the key of this value, according to
-the applied schema.
-
-Non-numeric facts are stored in `x.nonnumeric` as a list of `ixbrlNonnumeric`
-objects, with similar `.value`, `.context`, `.name` and `.schema` values. 
-The value of `.value` will be a string for non-numeric facts.
-
-#### Check for any parsing errors
-
-By default, the parser will throw an exception if it encounters an error
-when processing the document.
-
-You can parse `raise_on_error=False` to the initial object to suppress
-these exceptions. You can then access a list of the errors (and the element)
-that created them through the `.errors` attribute. For example:
-
-```python
-with open('sample_ixbrl.html', encoding="utf8") as a:
-  x = IXBRL(a, raise_on_error=False)
-  print(x.errors) # populated with any exceptions found
-  # [ eg...
-  #   {
-  #     "error": <NotImplementedError>,
-  #     "element": <BeautifulSoupElement>
-  #   }
-  # ]
-```
-
-Note that the error catching is only available for parsing of `.nonnumeric`
-and `numeric` items in the document. Any other errors with parsing will be
-thrown as normal no matter what `raise_on_error` is set to.
-
-## Code checks
-
-### Run tests
-
-Tests can be run with `pytest`:
-
-```bash
-pip install -e . # install the package
-pytest tests
-```
-
-### Test coverage
-
-```bash
-coverage run -m pytest tests
-coverage html
-python -m http.server -d htmlcov
-```
-
-### Run typing checks
-
-```bash
-mypy ixbrlparse tests
-```
-
-### Linting
-
-Black and isort should be run before committing any changes.
-
-```bash
-isort ixbrlparse tests
-black ixbrlparse tests
-```
-
-### Run all checks at once
-
-```sh
-black . && isort . && mypy ixbrlparse tests && coverage run -m pytest tests && coverage html --fail-under=100
-```
-
-## Publish to pypi
-
-```bash
-python -m build
-twine upload dist/*
-git tag v<VERSION_NUMBER>
-git push origin v<VERSION_NUMBER>
-```
-
-## Install development version
-
-The development requirements are installed using `pip install -r dev-requirements.txt`.
-
-Any additional requirements for the module itself must be added to
-`install_requires` in `setup.py`. You should then generate a new 
-`requirements.txt` using using [`pip-tools`](https://github.com/jazzband/pip-tools) (`pip-compile`). You can then run `pip-sync` to install the 
-requirement.
-
-Any additional development requirements must be added to `dev-requirements.in`
-and then the `dev-requirements.txt` should be generated using `pip-compile dev-requirements.in`. You can then install the development requirements using
-`pip-sync dev-requirements.txt`.
-
-## Acknowledgements
-
-Originally developed for a project with 
-[Power to Change](https://www.powertochange.org.uk/) looking at how to extract data from 
-financial documents of community businesses.
+Metadata-Version: 2.1
+Name: ixbrlparse
+Version: 0.6.0
+Summary: A python module for getting useful data out of ixbrl files.
+Project-URL: Homepage, https://github.com/drkane/ixbrl-parse
+Project-URL: Documentation, https://github.com/drkane/ixbrl-parse#readme
+Project-URL: Issues, https://github.com/drkane/ixbrl-parse/issues
+Project-URL: Source, https://github.com/drkane/ixbrl-parse
+Author-email: David Kane <david@dkane.net>
+License-Expression: MIT
+License-File: LICENSE
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Requires-Dist: beautifulsoup4
+Requires-Dist: click
+Requires-Dist: lxml
+Requires-Dist: word2number
+Description-Content-Type: text/markdown
+
+# ixbrl-parse
+
+
+![Test status](https://github.com/drkane/ixbrl-parse/workflows/tests/badge.svg)
+[![PyPI version](https://img.shields.io/pypi/v/ixbrlparse)](https://pypi.org/project/ixbrlparse/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ixbrlparse)
+![PyPI - License](https://img.shields.io/pypi/l/ixbrlparse)
+
+A python module for getting useful data out of ixbrl files. The library is at an early stage - feedback and improvements are very welcome.
+
+## Changelog
+
+**New in version 0.6.0**: Switch to use the [hatch](https://hatch.pypa.io/latest/) build and development system.
+
+**New in version 0.5.4**: Added backreferences to BeautifulSoup objects - thanks to @avyfain for PR.
+
+**New in version 0.5.3**: Support for `exclude` and `continuation` elements within XBRL documents. Thanks to @wcollinscw for adding support for exclude elements.
+
+**New in version 0.5**: Support for Python 3.11 has been added. I've had some problems with Python 3.11 and Windows as lxml binaries aren't yet available. Also new in version 0.5 is type checking - the whole library now has types added. 
+
+**New in version 0.4**: I've added initial support for pure XBRL files as well as tagged HTML iXBRL files. Feedback on this feature is welcome - particularly around getting values out of numeric items.
+
+## Requirements
+
+The module requires [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/) and [lxml](https://lxml.de/) to parse the documents.
+
+[word2number](https://github.com/akshaynagpal/w2n) is used to process the
+numeric items with the `numsenwords` format.
+
+## How to install
+
+You can install from pypi using pip:
+
+```
+pip install ixbrlparse
+```
+
+## How to use
+
+### Run the python module
+
+You can run the module directly to extract data from an IXBRL file.
+
+```bash
+ixbrlparse example_file.html
+# or
+python -m ixbrlparse example_file.html
+```
+
+The various options for using this can be found through:
+
+```bash
+python -m ixbrlparse -h
+# optional arguments:
+#   -h, --help            show this help message and exit
+#   --outfile OUTFILE     Where to output the file
+#   --format {csv,json,jsonlines,jsonl}
+#                         format of the output
+#   --fields {numeric,nonnumeric,all}
+#                         Which fields to output
+```
+
+### Use as a python module
+
+An example of usage is shown in [`test.py`](test.py).
+
+#### Import the `IXBRL` class which parses the file.
+
+```python
+from ixbrlparse import IXBRL
+```
+
+#### Initialise an object and parse the file
+
+You need to pass a file handle or other object with a `.read()` method.
+
+```python
+with open('sample_ixbrl.html', encoding="utf8") as a:
+  x = IXBRL(a)
+```
+
+If your IXBRL data comes as a string then use a `io.StringIO` wrapper to
+pass it to the class:
+
+```python
+import io
+from ixbrlparse import IXBRL
+
+content = '''<some ixbrl content>'''
+x = IXBRL(io.StringIO(content))
+```
+
+
+#### Get the contexts and units used in the data
+
+These are held in the object. The contexts are stored as a dictionary with the context
+id as the key, and a `ixbrlContext` object as the value.
+
+```python
+print(x.contexts)
+# {
+#    "cfwd_2018_03_31": ixbrlContext(
+#       id="cfwd_2018_03_31",
+#       entity="0123456", # company number
+#       segments=[], # used for hypercubes
+#       instant="2018-03-31",
+#       startdate=None, # used for periods
+#       enddate=None, # used for periods
+#    ),
+#    ....
+# }
+```
+
+The units are stored as key:value dictionary entries
+```python
+print(x.units)
+# {
+#    "GBP": "ISO4107:GBP"
+#    "shares": "shares"
+# }
+```
+
+#### Get financial facts
+
+Numeric facts are stored in `x.numeric` as a list of `ixbrlNumeric` objects.
+The `ixbrlNumeric.value` object contains the value as a parsed python number
+(after the sign and scale formatting values have been applied).
+
+`ixbrlNumeric.context` holds the context object relating to this value.
+The `.name` and `.schema` values give the key of this value, according to
+the applied schema.
+
+Non-numeric facts are stored in `x.nonnumeric` as a list of `ixbrlNonnumeric`
+objects, with similar `.value`, `.context`, `.name` and `.schema` values. 
+The value of `.value` will be a string for non-numeric facts.
+
+#### Check for any parsing errors
+
+By default, the parser will throw an exception if it encounters an error
+when processing the document.
+
+You can parse `raise_on_error=False` to the initial object to suppress
+these exceptions. You can then access a list of the errors (and the element)
+that created them through the `.errors` attribute. For example:
+
+```python
+with open('sample_ixbrl.html', encoding="utf8") as a:
+  x = IXBRL(a, raise_on_error=False)
+  print(x.errors) # populated with any exceptions found
+  # [ eg...
+  #   {
+  #     "error": <NotImplementedError>,
+  #     "element": <BeautifulSoupElement>
+  #   }
+  # ]
+```
+
+Note that the error catching is only available for parsing of `.nonnumeric`
+and `numeric` items in the document. Any other errors with parsing will be
+thrown as normal no matter what `raise_on_error` is set to.
+
+## Code checks
+
+The module is setup for development using [hatch](https://hatch.pypa.io/latest/).
+
+### Run tests
+
+Tests can be run with `pytest`:
+
+```bash
+hatch run test
+```
+
+### Test coverage
+
+Run tests then report on coverage
+
+```bash
+hatch run cov
+```
+
+Run tests then run a server showing where coverage is missing
+
+```bash
+hatch run cov-html
+```
+
+### Run typing checks
+
+```bash
+hatch run lint:typing
+```
+
+### Linting
+
+Black and ruff should be run before committing any changes.
+
+To check for any changes needed:
+
+```bash
+hatch run lint:style
+```
+
+To run any autoformatting possible:
+
+```sh
+hatch run lint:fmt
+```
+
+### Run all checks at once
+
+```sh
+hatch run lint:all
+```
+
+## Publish to pypi
+
+```bash
+hatch build
+hatch publish
+git tag v<VERSION_NUMBER>
+git push origin v<VERSION_NUMBER>
+```
+
+## Acknowledgements
+
+Originally developed for a project with 
+[Power to Change](https://www.powertochange.org.uk/) looking at how to extract data from 
+financial documents of community businesses.
```

### Comparing `ixbrlparse-0.5.4/README.md` & `ixbrlparse-0.6.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 ![Test status](https://github.com/drkane/ixbrl-parse/workflows/tests/badge.svg)
 [![PyPI version](https://img.shields.io/pypi/v/ixbrlparse)](https://pypi.org/project/ixbrlparse/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ixbrlparse)
 ![PyPI - License](https://img.shields.io/pypi/l/ixbrlparse)
 
 A python module for getting useful data out of ixbrl files. The library is at an early stage - feedback and improvements are very welcome.
 
+## Changelog
+
+**New in version 0.6.0**: Switch to use the [hatch](https://hatch.pypa.io/latest/) build and development system.
+
 **New in version 0.5.4**: Added backreferences to BeautifulSoup objects - thanks to @avyfain for PR.
 
 **New in version 0.5.3**: Support for `exclude` and `continuation` elements within XBRL documents. Thanks to @wcollinscw for adding support for exclude elements.
 
 **New in version 0.5**: Support for Python 3.11 has been added. I've had some problems with Python 3.11 and Windows as lxml binaries aren't yet available. Also new in version 0.5 is type checking - the whole library now has types added. 
 
 **New in version 0.4**: I've added initial support for pure XBRL files as well as tagged HTML iXBRL files. Feedback on this feature is welcome - particularly around getting values out of numeric items.
@@ -34,14 +38,16 @@
 ## How to use
 
 ### Run the python module
 
 You can run the module directly to extract data from an IXBRL file.
 
 ```bash
+ixbrlparse example_file.html
+# or
 python -m ixbrlparse example_file.html
 ```
 
 The various options for using this can be found through:
 
 ```bash
 python -m ixbrlparse -h
@@ -151,72 +157,73 @@
 
 Note that the error catching is only available for parsing of `.nonnumeric`
 and `numeric` items in the document. Any other errors with parsing will be
 thrown as normal no matter what `raise_on_error` is set to.
 
 ## Code checks
 
+The module is setup for development using [hatch](https://hatch.pypa.io/latest/).
+
 ### Run tests
 
 Tests can be run with `pytest`:
 
 ```bash
-pip install -e . # install the package
-pytest tests
+hatch run test
 ```
 
 ### Test coverage
 
+Run tests then report on coverage
+
+```bash
+hatch run cov
+```
+
+Run tests then run a server showing where coverage is missing
+
 ```bash
-coverage run -m pytest tests
-coverage html
-python -m http.server -d htmlcov
+hatch run cov-html
 ```
 
 ### Run typing checks
 
 ```bash
-mypy ixbrlparse tests
+hatch run lint:typing
 ```
 
 ### Linting
 
-Black and isort should be run before committing any changes.
+Black and ruff should be run before committing any changes.
+
+To check for any changes needed:
 
 ```bash
-isort ixbrlparse tests
-black ixbrlparse tests
+hatch run lint:style
+```
+
+To run any autoformatting possible:
+
+```sh
+hatch run lint:fmt
 ```
 
 ### Run all checks at once
 
 ```sh
-black . && isort . && mypy ixbrlparse tests && coverage run -m pytest tests && coverage html --fail-under=100
+hatch run lint:all
 ```
 
 ## Publish to pypi
 
 ```bash
-python -m build
-twine upload dist/*
+hatch build
+hatch publish
 git tag v<VERSION_NUMBER>
 git push origin v<VERSION_NUMBER>
 ```
 
-## Install development version
-
-The development requirements are installed using `pip install -r dev-requirements.txt`.
-
-Any additional requirements for the module itself must be added to
-`install_requires` in `setup.py`. You should then generate a new 
-`requirements.txt` using using [`pip-tools`](https://github.com/jazzband/pip-tools) (`pip-compile`). You can then run `pip-sync` to install the 
-requirement.
-
-Any additional development requirements must be added to `dev-requirements.in`
-and then the `dev-requirements.txt` should be generated using `pip-compile dev-requirements.in`. You can then install the development requirements using
-`pip-sync dev-requirements.txt`.
-
 ## Acknowledgements
 
 Originally developed for a project with 
 [Power to Change](https://www.powertochange.org.uk/) looking at how to extract data from 
 financial documents of community businesses.
```

