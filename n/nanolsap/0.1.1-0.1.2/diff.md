# Comparing `tmp/nanolsap-0.1.1.tar.gz` & `tmp/nanolsap-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanolsap-0.1.1.tar", last modified: Sat Jun 24 15:23:07 2023, max compression
+gzip compressed data, was "nanolsap-0.1.2.tar", last modified: Sun Jul  9 13:50:49 2023, max compression
```

## Comparing `nanolsap-0.1.1.tar` & `nanolsap-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:23:07.947695 nanolsap-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:23:07.939695 nanolsap-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:23:07.943694 nanolsap-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-24 15:22:54.000000 nanolsap-0.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-24 15:22:54.000000 nanolsap-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-24 15:22:54.000000 nanolsap-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-06-24 15:23:07.947695 nanolsap-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-06-24 15:22:54.000000 nanolsap-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-24 15:22:54.000000 nanolsap-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-24 15:23:07.947695 nanolsap-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-24 15:22:54.000000 nanolsap-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:23:07.939695 nanolsap-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:23:07.943694 nanolsap-0.1.1/src/nanolsap/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-24 15:22:54.000000 nanolsap-0.1.1/src/nanolsap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-06-24 15:22:54.000000 nanolsap-0.1.1/src/nanolsap/_lsap.c
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-24 15:22:54.000000 nanolsap-0.1.1/src/nanolsap/_lsap.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 15:22:54.000000 nanolsap-0.1.1/src/nanolsap/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:23:07.947695 nanolsap-0.1.1/src/nanolsap/rectangular_lsap/
--rw-r--r--   0 runner    (1001) docker     (123)    12229 2023-06-24 15:22:54.000000 nanolsap-0.1.1/src/nanolsap/rectangular_lsap/rectangular_lsap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-06-24 15:22:54.000000 nanolsap-0.1.1/src/nanolsap/rectangular_lsap/rectangular_lsap.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:23:07.943694 nanolsap-0.1.1/src/nanolsap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-06-24 15:23:07.000000 nanolsap-0.1.1/src/nanolsap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-24 15:23:07.000000 nanolsap-0.1.1/src/nanolsap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 15:23:07.000000 nanolsap-0.1.1/src/nanolsap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-24 15:23:07.000000 nanolsap-0.1.1/src/nanolsap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-24 15:23:07.000000 nanolsap-0.1.1/src/nanolsap.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:23:07.947695 nanolsap-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-06-24 15:22:54.000000 nanolsap-0.1.1/tests/test_linear_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-24 15:22:54.000000 nanolsap-0.1.1/tests/test_solve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-24 15:22:54.000000 nanolsap-0.1.1/tests/test_subrowcol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:50:49.289047 nanolsap-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:50:49.281047 nanolsap-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:50:49.285047 nanolsap-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-09 13:50:36.000000 nanolsap-0.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-09 13:50:36.000000 nanolsap-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-09 13:50:36.000000 nanolsap-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-09 13:50:49.289047 nanolsap-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-07-09 13:50:36.000000 nanolsap-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-09 13:50:36.000000 nanolsap-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 13:50:49.289047 nanolsap-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-09 13:50:36.000000 nanolsap-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:50:49.281047 nanolsap-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:50:49.285047 nanolsap-0.1.2/src/nanolsap/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-09 13:50:36.000000 nanolsap-0.1.2/src/nanolsap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-07-09 13:50:36.000000 nanolsap-0.1.2/src/nanolsap/_lsap.c
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-09 13:50:36.000000 nanolsap-0.1.2/src/nanolsap/_lsap.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 13:50:36.000000 nanolsap-0.1.2/src/nanolsap/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:50:49.285047 nanolsap-0.1.2/src/nanolsap/rectangular_lsap/
+-rw-r--r--   0 runner    (1001) docker     (123)    12229 2023-07-09 13:50:36.000000 nanolsap-0.1.2/src/nanolsap/rectangular_lsap/rectangular_lsap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-07-09 13:50:36.000000 nanolsap-0.1.2/src/nanolsap/rectangular_lsap/rectangular_lsap.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:50:49.285047 nanolsap-0.1.2/src/nanolsap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-09 13:50:49.000000 nanolsap-0.1.2/src/nanolsap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-09 13:50:49.000000 nanolsap-0.1.2/src/nanolsap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 13:50:49.000000 nanolsap-0.1.2/src/nanolsap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-09 13:50:49.000000 nanolsap-0.1.2/src/nanolsap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-09 13:50:49.000000 nanolsap-0.1.2/src/nanolsap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:50:49.289047 nanolsap-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-07-09 13:50:36.000000 nanolsap-0.1.2/tests/test_linear_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-09 13:50:36.000000 nanolsap-0.1.2/tests/test_solve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-09 13:50:36.000000 nanolsap-0.1.2/tests/test_subrowcol.py
```

### Comparing `nanolsap-0.1.1/.github/workflows/python-publish.yml` & `nanolsap-0.1.2/.github/workflows/python-publish.yml`

 * *Files 18% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 
 jobs:
   build_wheels:
     name: Build wheels on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        # os: [ubuntu-22.04, windows-2019, macos-11]
-        os: [ubuntu-22.04, windows-2019]
+        os: [ubuntu-22.04, windows-2019, macos-11]
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Build wheels
         uses: pypa/cibuildwheel@v2.13.1
 
@@ -58,7 +57,29 @@
           path: dist
 
       - uses: pypa/gh-action-pypi-publish@v1.5.0
         with:
           user: __token__
           password: ${{ secrets.pypi_password }}
           # To test: repository_url: https://test.pypi.org/legacy/
+
+  upload_assets:
+    needs: [build_wheels, build_sdist]
+    runs-on: ubuntu-latest
+    permissions:
+      contents: write
+    # upload on every tag starting with 'v'
+    # if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags/v')
+    # alternatively, to publish when a GitHub Release is created, use the following rule:
+    if: github.event_name == 'release' && github.event.action == 'published'
+    steps:
+      - uses: actions/download-artifact@v3
+        with:
+          # unpacks default artifact into dist/
+          # if `name: artifact` is omitted, the action will create extra parent dir
+          name: artifact
+          path: dist
+
+      - uses: softprops/action-gh-release@v1
+        with:
+          tag_name: ${{ github.event.release.tag_name }}
+          files: dist/*
```

### Comparing `nanolsap-0.1.1/.gitignore` & `nanolsap-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `nanolsap-0.1.1/LICENSE` & `nanolsap-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nanolsap-0.1.1/PKG-INFO` & `nanolsap-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanolsap
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python module to solve the linear sum assignment problem (LSAP) low memory friendly
 Author-email: hzqmwne <huangzhengqmwne@sina.cn>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/hzqmwne/nanolsap
 Keywords: lsap,munkres,kuhn-munkres,linear sum assignment problem
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nanolsap-0.1.1/README.md` & `nanolsap-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nanolsap-0.1.1/pyproject.toml` & `nanolsap-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nanolsap-0.1.1/src/nanolsap/_lsap.c` & `nanolsap-0.1.2/src/nanolsap/_lsap.c`

 * *Files identical despite different names*

### Comparing `nanolsap-0.1.1/src/nanolsap/rectangular_lsap/rectangular_lsap.cpp` & `nanolsap-0.1.2/src/nanolsap/rectangular_lsap/rectangular_lsap.cpp`

 * *Files identical despite different names*

### Comparing `nanolsap-0.1.1/src/nanolsap/rectangular_lsap/rectangular_lsap.h` & `nanolsap-0.1.2/src/nanolsap/rectangular_lsap/rectangular_lsap.h`

 * *Files identical despite different names*

### Comparing `nanolsap-0.1.1/src/nanolsap.egg-info/PKG-INFO` & `nanolsap-0.1.2/src/nanolsap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanolsap
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python module to solve the linear sum assignment problem (LSAP) low memory friendly
 Author-email: hzqmwne <huangzhengqmwne@sina.cn>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/hzqmwne/nanolsap
 Keywords: lsap,munkres,kuhn-munkres,linear sum assignment problem
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nanolsap-0.1.1/src/nanolsap.egg-info/SOURCES.txt` & `nanolsap-0.1.2/src/nanolsap.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 .gitignore
 LICENSE
 README.md
 pyproject.toml
-setup.cfg
 setup.py
 .github/workflows/python-publish.yml
 src/nanolsap/__init__.py
 src/nanolsap/_lsap.c
 src/nanolsap/_lsap.pyi
 src/nanolsap/py.typed
 src/nanolsap.egg-info/PKG-INFO
```

### Comparing `nanolsap-0.1.1/tests/test_linear_assignment.py` & `nanolsap-0.1.2/tests/test_linear_assignment.py`

 * *Files identical despite different names*

### Comparing `nanolsap-0.1.1/tests/test_solve.py` & `nanolsap-0.1.2/tests/test_solve.py`

 * *Files identical despite different names*

### Comparing `nanolsap-0.1.1/tests/test_subrowcol.py` & `nanolsap-0.1.2/tests/test_subrowcol.py`

 * *Files identical despite different names*

