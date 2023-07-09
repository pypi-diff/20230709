# Comparing `tmp/clown_sort-1.9.1.tar.gz` & `tmp/clown_sort-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clown_sort-1.9.1.tar", max compression
+gzip compressed data, was "clown_sort-1.9.2.tar", max compression
```

## Comparing `clown_sort-1.9.1.tar` & `clown_sort-1.9.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     4098 2023-07-09 08:22:00.390857 clown_sort-1.9.1/CHANGELOG.md
--rw-r--r--   0        0        0     1078 2023-02-19 21:54:39.742371 clown_sort-1.9.1/LICENSE
--rw-r--r--   0        0        0     9287 2023-06-25 02:54:41.522424 clown_sort-1.9.1/README.md
--rw-r--r--   0        0        0     4502 2023-07-09 08:21:26.854406 clown_sort-1.9.1/clown_sort/__init__.py
--rw-r--r--   0        0        0     8167 2023-07-09 08:21:26.854847 clown_sort-1.9.1/clown_sort/config.py
--rw-r--r--   0        0        0     9021 2023-06-02 20:58:04.234216 clown_sort-1.9.1/clown_sort/filename_extractor.py
--rw-r--r--   0        0        0     4832 2023-06-25 02:54:41.523569 clown_sort-1.9.1/clown_sort/files/image_file.py
--rw-r--r--   0        0        0      392 2023-06-24 02:14:02.169664 clown_sort-1.9.1/clown_sort/files/import pdfplumber.py
--rw-r--r--   0        0        0     4914 2023-07-09 08:21:26.855255 clown_sort-1.9.1/clown_sort/files/pdf_file.py
--rw-r--r--   0        0        0    12130 2023-07-09 08:21:26.855827 clown_sort-1.9.1/clown_sort/files/sortable_file.py
--rwxr-xr-x   0        0        0     3456 2023-06-15 23:17:52.887054 clown_sort-1.9.1/clown_sort/sort_selector.py
--rw-r--r--   0        0        0    12478 2023-07-06 21:33:53.445844 clown_sort-1.9.1/clown_sort/sorting_rules/crypto.csv
--rw-r--r--   0        0        0     4416 2023-07-09 08:21:26.856147 clown_sort-1.9.1/clown_sort/util/argument_parser.py
--rw-r--r--   0        0        0     1559 2023-05-09 18:20:37.531689 clown_sort-1.9.1/clown_sort/util/constants.py
--rw-r--r--   0        0        0      196 2023-03-25 04:04:12.967064 clown_sort-1.9.1/clown_sort/util/dict_helper.py
--rw-r--r--   0        0        0     3705 2023-06-20 03:19:34.508422 clown_sort-1.9.1/clown_sort/util/filesystem_helper.py
--rw-r--r--   0        0        0      372 2023-04-14 22:24:41.414299 clown_sort-1.9.1/clown_sort/util/logging.py
--rw-r--r--   0        0        0     3527 2023-07-09 08:21:26.856578 clown_sort-1.9.1/clown_sort/util/rich_helper.py
--rw-r--r--   0        0        0      667 2023-05-27 16:06:01.554255 clown_sort-1.9.1/clown_sort/util/string_helper.py
--rw-r--r--   0        0        0     1713 2023-07-09 08:22:00.396643 clown_sort-1.9.1/pyproject.toml
--rw-r--r--   0        0        0    10710 1970-01-01 00:00:00.000000 clown_sort-1.9.1/PKG-INFO
+-rw-r--r--   0        0        0     4171 2023-07-09 10:49:12.556368 clown_sort-1.9.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1078 2023-02-19 21:54:39.742371 clown_sort-1.9.2/LICENSE
+-rw-r--r--   0        0        0     9287 2023-06-25 02:54:41.522424 clown_sort-1.9.2/README.md
+-rw-r--r--   0        0        0     4502 2023-07-09 08:21:26.854406 clown_sort-1.9.2/clown_sort/__init__.py
+-rw-r--r--   0        0        0     8167 2023-07-09 08:21:26.854847 clown_sort-1.9.2/clown_sort/config.py
+-rw-r--r--   0        0        0     9021 2023-06-02 20:58:04.234216 clown_sort-1.9.2/clown_sort/filename_extractor.py
+-rw-r--r--   0        0        0     4832 2023-06-25 02:54:41.523569 clown_sort-1.9.2/clown_sort/files/image_file.py
+-rw-r--r--   0        0        0      392 2023-06-24 02:14:02.169664 clown_sort-1.9.2/clown_sort/files/import pdfplumber.py
+-rw-r--r--   0        0        0     4914 2023-07-09 08:26:42.337760 clown_sort-1.9.2/clown_sort/files/pdf_file.py
+-rw-r--r--   0        0        0    12130 2023-07-09 08:21:26.855827 clown_sort-1.9.2/clown_sort/files/sortable_file.py
+-rwxr-xr-x   0        0        0     3456 2023-06-15 23:17:52.887054 clown_sort-1.9.2/clown_sort/sort_selector.py
+-rw-r--r--   0        0        0    12478 2023-07-06 21:33:53.445844 clown_sort-1.9.2/clown_sort/sorting_rules/crypto.csv
+-rw-r--r--   0        0        0     4416 2023-07-09 08:21:26.856147 clown_sort-1.9.2/clown_sort/util/argument_parser.py
+-rw-r--r--   0        0        0     1559 2023-05-09 18:20:37.531689 clown_sort-1.9.2/clown_sort/util/constants.py
+-rw-r--r--   0        0        0      196 2023-03-25 04:04:12.967064 clown_sort-1.9.2/clown_sort/util/dict_helper.py
+-rw-r--r--   0        0        0     3705 2023-06-20 03:19:34.508422 clown_sort-1.9.2/clown_sort/util/filesystem_helper.py
+-rw-r--r--   0        0        0      372 2023-04-14 22:24:41.414299 clown_sort-1.9.2/clown_sort/util/logging.py
+-rw-r--r--   0        0        0     3527 2023-07-09 08:21:26.856578 clown_sort-1.9.2/clown_sort/util/rich_helper.py
+-rw-r--r--   0        0        0      667 2023-05-27 16:06:01.554255 clown_sort-1.9.2/clown_sort/util/string_helper.py
+-rw-r--r--   0        0        0     1721 2023-07-09 10:49:12.563226 clown_sort-1.9.2/pyproject.toml
+-rw-r--r--   0        0        0    10809 1970-01-01 00:00:00.000000 clown_sort-1.9.2/PKG-INFO
```

### Comparing `clown_sort-1.9.1/CHANGELOG.md` & `clown_sort-1.9.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # NEXT RELEASE
 
+### 1.9.2
+* Allow `Pillow` 10.0.0
+* Reduce required python version to 3.8
+
 ### 1.9.1
 * Output progress notifications to STDERR when parsing text from very large PDFs
 * Fix issue that caused explosive memory growth when parsing large PDFs
 * `--print-when-parsed` command line option for `extract_text_from_files`
-* Upgrade `pypdf` to `3.12.0` to resolve various PDF parsing failures
+* Upgrade `pypdf` to 3.12.0 to resolve various PDF parsing failures
 * PDFs: Handle various exceptions when enumerating embedded images:
    * `OSError: cannot write mode CMYK as PNG`
    * `ValueError: not enough image data`
    * `TypeError: unhashable type: 'ArrayObject'`
    * `TypeError: unhashable type: 'IndirectObject'`
 
 # 1.9.0
```

### Comparing `clown_sort-1.9.1/LICENSE` & `clown_sort-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clown_sort-1.9.1/README.md` & `clown_sort-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `clown_sort-1.9.1/clown_sort/__init__.py` & `clown_sort-1.9.2/clown_sort/__init__.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.9.1/clown_sort/config.py` & `clown_sort-1.9.2/clown_sort/config.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.9.1/clown_sort/filename_extractor.py` & `clown_sort-1.9.2/clown_sort/filename_extractor.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.9.1/clown_sort/files/image_file.py` & `clown_sort-1.9.2/clown_sort/files/image_file.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.9.1/clown_sort/files/pdf_file.py` & `clown_sort-1.9.2/clown_sort/files/pdf_file.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.9.1/clown_sort/files/sortable_file.py` & `clown_sort-1.9.2/clown_sort/files/sortable_file.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.9.1/clown_sort/sort_selector.py` & `clown_sort-1.9.2/clown_sort/sort_selector.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.9.1/clown_sort/sorting_rules/crypto.csv` & `clown_sort-1.9.2/clown_sort/sorting_rules/crypto.csv`

 * *Files identical despite different names*

### Comparing `clown_sort-1.9.1/clown_sort/util/argument_parser.py` & `clown_sort-1.9.2/clown_sort/util/argument_parser.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.9.1/clown_sort/util/constants.py` & `clown_sort-1.9.2/clown_sort/util/constants.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.9.1/clown_sort/util/filesystem_helper.py` & `clown_sort-1.9.2/clown_sort/util/filesystem_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.9.1/clown_sort/util/rich_helper.py` & `clown_sort-1.9.2/clown_sort/util/rich_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.9.1/clown_sort/util/string_helper.py` & `clown_sort-1.9.2/clown_sort/util/string_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.9.1/pyproject.toml` & `clown_sort-1.9.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clown_sort"
-version = "1.9.1"
+version = "1.9.2"
 description = "Sort screenshots based on rules or through individual review."
 authors = ["Michel de Cryptadamus <michel@cryptadamus.com>"]
 readme = "README.md"
 packages = [{include = "clown_sort"}]
 homepage = "https://github.com/michelcrypt4d4mus/clown_sort"
 
 include = [
@@ -27,21 +27,21 @@
     "Topic :: Multimedia :: Graphics :: Capture :: Screen Capture",
     "Topic :: Multimedia :: Graphics :: Capture",
     "Topic :: Scientific/Engineering :: Image Processing",
 ]
 
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.8"
 exif = "^1.5.0"
 PySimpleGUI = {version = "^4.60.4", optional = true}
 pytesseract = "^0.3.10"
 rich = "^13.0.1"
 piexif = "^1.1.3"
-pillow = "^9.5.0"
+pillow = ">=9.5.0,<11.0.0"
 filedate = "^2.0"
 python-dotenv = "^0.21.1"
 rich-argparse-plus = "^0.3.1.4"
 pycryptodome = {version = "^3.17", optional = true}
 pyexiftool = "^0.5.5"
 PyMuPDF = {version = "^1.22.3", optional = true}
 pypdf = "^3.12.0"
```

### Comparing `clown_sort-1.9.1/PKG-INFO` & `clown_sort-1.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: clown-sort
-Version: 1.9.1
+Version: 1.9.2
 Summary: Sort screenshots based on rules or through individual review.
 Home-page: https://github.com/michelcrypt4d4mus/clown_sort
 Keywords: ocr,organization,organizer,screenshot,rename,sort
 Author: Michel de Cryptadamus
 Author-email: michel@cryptadamus.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Desktop Environment :: File Managers
 Classifier: Topic :: Multimedia :: Graphics :: Capture
 Classifier: Topic :: Multimedia :: Graphics :: Capture :: Screen Capture
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Provides-Extra: gui
 Provides-Extra: pdf
 Requires-Dist: PyMuPDF (>=1.22.3,<2.0.0) ; extra == "pdf"
 Requires-Dist: PySimpleGUI (>=4.60.4,<5.0.0) ; extra == "gui"
 Requires-Dist: exif (>=1.5.0,<2.0.0)
 Requires-Dist: filedate (>=2.0,<3.0)
 Requires-Dist: piexif (>=1.1.3,<2.0.0)
-Requires-Dist: pillow (>=9.5.0,<10.0.0)
+Requires-Dist: pillow (>=9.5.0,<11.0.0)
 Requires-Dist: pycryptodome (>=3.17,<4.0) ; extra == "pdf"
 Requires-Dist: pyexiftool (>=0.5.5,<0.6.0)
 Requires-Dist: pypdf (>=3.12.0,<4.0.0)
 Requires-Dist: pytesseract (>=0.3.10,<0.4.0)
 Requires-Dist: python-dotenv (>=0.21.1,<0.22.0)
 Requires-Dist: rich (>=13.0.1,<14.0.0)
 Requires-Dist: rich-argparse-plus (>=0.3.1.4,<0.4.0.0)
```

