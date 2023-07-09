# Comparing `tmp/nanolsap-0.1.0.tar.gz` & `tmp/nanolsap-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanolsap-0.1.0.tar", last modified: Tue Jun 20 12:41:32 2023, max compression
+gzip compressed data, was "nanolsap-0.1.1.tar", last modified: Sat Jun 24 15:23:07 2023, max compression
```

## Comparing `nanolsap-0.1.0.tar` & `nanolsap-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:41:32.255155 nanolsap-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:41:32.251155 nanolsap-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:41:32.255155 nanolsap-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-20 12:41:15.000000 nanolsap-0.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-20 12:41:15.000000 nanolsap-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-20 12:41:15.000000 nanolsap-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-06-20 12:41:32.255155 nanolsap-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-06-20 12:41:15.000000 nanolsap-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-20 12:41:15.000000 nanolsap-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-20 12:41:32.259155 nanolsap-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-20 12:41:15.000000 nanolsap-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:41:32.251155 nanolsap-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:41:32.255155 nanolsap-0.1.0/src/nanolsap/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-20 12:41:15.000000 nanolsap-0.1.0/src/nanolsap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10488 2023-06-20 12:41:15.000000 nanolsap-0.1.0/src/nanolsap/_lsap.c
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-20 12:41:15.000000 nanolsap-0.1.0/src/nanolsap/_lsap.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 12:41:15.000000 nanolsap-0.1.0/src/nanolsap/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:41:32.255155 nanolsap-0.1.0/src/nanolsap/rectangular_lsap/
--rw-r--r--   0 runner    (1001) docker     (123)    12229 2023-06-20 12:41:15.000000 nanolsap-0.1.0/src/nanolsap/rectangular_lsap/rectangular_lsap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-06-20 12:41:15.000000 nanolsap-0.1.0/src/nanolsap/rectangular_lsap/rectangular_lsap.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:41:32.255155 nanolsap-0.1.0/src/nanolsap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-06-20 12:41:32.000000 nanolsap-0.1.0/src/nanolsap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-20 12:41:32.000000 nanolsap-0.1.0/src/nanolsap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 12:41:32.000000 nanolsap-0.1.0/src/nanolsap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-20 12:41:32.000000 nanolsap-0.1.0/src/nanolsap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 12:41:32.000000 nanolsap-0.1.0/src/nanolsap.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:41:32.255155 nanolsap-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-06-20 12:41:15.000000 nanolsap-0.1.0/tests/test_linear_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-20 12:41:15.000000 nanolsap-0.1.0/tests/test_solve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-20 12:41:15.000000 nanolsap-0.1.0/tests/test_subrowcol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:23:07.947695 nanolsap-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:23:07.939695 nanolsap-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:23:07.943694 nanolsap-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-24 15:22:54.000000 nanolsap-0.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-24 15:22:54.000000 nanolsap-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-24 15:22:54.000000 nanolsap-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-06-24 15:23:07.947695 nanolsap-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-06-24 15:22:54.000000 nanolsap-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-24 15:22:54.000000 nanolsap-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-24 15:23:07.947695 nanolsap-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-24 15:22:54.000000 nanolsap-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:23:07.939695 nanolsap-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:23:07.943694 nanolsap-0.1.1/src/nanolsap/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-24 15:22:54.000000 nanolsap-0.1.1/src/nanolsap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-06-24 15:22:54.000000 nanolsap-0.1.1/src/nanolsap/_lsap.c
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-24 15:22:54.000000 nanolsap-0.1.1/src/nanolsap/_lsap.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 15:22:54.000000 nanolsap-0.1.1/src/nanolsap/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:23:07.947695 nanolsap-0.1.1/src/nanolsap/rectangular_lsap/
+-rw-r--r--   0 runner    (1001) docker     (123)    12229 2023-06-24 15:22:54.000000 nanolsap-0.1.1/src/nanolsap/rectangular_lsap/rectangular_lsap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-06-24 15:22:54.000000 nanolsap-0.1.1/src/nanolsap/rectangular_lsap/rectangular_lsap.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:23:07.943694 nanolsap-0.1.1/src/nanolsap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-06-24 15:23:07.000000 nanolsap-0.1.1/src/nanolsap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-24 15:23:07.000000 nanolsap-0.1.1/src/nanolsap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 15:23:07.000000 nanolsap-0.1.1/src/nanolsap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-24 15:23:07.000000 nanolsap-0.1.1/src/nanolsap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-24 15:23:07.000000 nanolsap-0.1.1/src/nanolsap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:23:07.947695 nanolsap-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-06-24 15:22:54.000000 nanolsap-0.1.1/tests/test_linear_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-24 15:22:54.000000 nanolsap-0.1.1/tests/test_solve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-24 15:22:54.000000 nanolsap-0.1.1/tests/test_subrowcol.py
```

### Comparing `nanolsap-0.1.0/.github/workflows/python-publish.yml` & `nanolsap-0.1.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `nanolsap-0.1.0/.gitignore` & `nanolsap-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `nanolsap-0.1.0/LICENSE` & `nanolsap-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nanolsap-0.1.0/PKG-INFO` & `nanolsap-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanolsap
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python module to solve the linear sum assignment problem (LSAP) low memory friendly
 Author-email: hzqmwne <huangzhengqmwne@sina.cn>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/hzqmwne/nanolsap
 Keywords: lsap,munkres,kuhn-munkres,linear sum assignment problem
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nanolsap-0.1.0/README.md` & `nanolsap-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nanolsap-0.1.0/pyproject.toml` & `nanolsap-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nanolsap-0.1.0/setup.py` & `nanolsap-0.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import numpy
 import platform
 
 from setuptools import setup, Extension
 
 PY_LIMITED_API = "0x03070000"
 PY_LIMITED_API_VERSION = (3, 7)
@@ -20,14 +21,17 @@
                     f"cp{PY_LIMITED_API_VERSION[0]}{PY_LIMITED_API_VERSION[1]}"
                 )
                 super().finalize_options()
 
         cmdclass = {"bdist_wheel": bdist_wheel}
 else:
     cmdclass = {}
+
+os.environ["CXXFLAGS"] = "-std=c++11"
+os.environ["LDFLAGS"] = "-s"
 setup_args = dict(
     ext_modules=[
         Extension(
             "nanolsap._lsap",
             ["src/nanolsap/_lsap.c", "src/nanolsap/rectangular_lsap/rectangular_lsap.cpp"],
             py_limited_api=True,
             include_dirs=[numpy.get_include()],
```

### Comparing `nanolsap-0.1.0/src/nanolsap/_lsap.c` & `nanolsap-0.1.1/src/nanolsap/_lsap.c`

 * *Files 3% similar despite different names*

```diff
@@ -74,16 +74,16 @@
 {
     PyObject* a = NULL;
     PyObject* b = NULL;
     PyObject* result = NULL;
     PyObject* obj_cost = NULL;
     PyArrayObject* obj_cont = NULL;
     int maximize = 0;
-    PyObject* obj_subrows = NULL;
-    PyObject* obj_subcols = NULL;
+    PyObject* obj_subrows = Py_None;
+    PyObject* obj_subcols = Py_None;
     PyArrayObject* array_subrows = NULL;
     PyArrayObject* array_subcols = NULL;
     intptr_t *subrows = NULL;
     intptr_t n_subrows = 0;
     intptr_t *subcols = NULL;
     intptr_t n_subcols = 0;
     static const char *kwlist[] = { (const char*)"cost_matrix",
@@ -121,15 +121,15 @@
 
     void* cost_matrix = PyArray_DATA(obj_cont);
     if (cost_matrix == NULL) {
         PyErr_SetString(PyExc_TypeError, "invalid cost matrix object");
         goto cleanup;
     }
 
-    if (obj_subrows != NULL && obj_subrows != Py_None) {
+    if (obj_subrows != Py_None) {
         array_subrows = (PyArrayObject*)PyArray_ContiguousFromAny(obj_subrows, NPY_INTP, 0, 0);
         if (!array_subrows) {
             return NULL;
         }
         if (PyArray_NDIM(array_subrows) != 1) {
             PyErr_Format(PyExc_ValueError,
                         "subrows expected a 1-D array, got a %d array",
@@ -139,15 +139,15 @@
         subrows = (intptr_t *)PyArray_DATA(array_subrows);
         if (subrows == NULL) {
             PyErr_SetString(PyExc_TypeError, "invalid subrows array object");
             goto cleanup;
         }
         n_subrows = PyArray_DIM(array_subrows, 0);
     }
-    if (obj_subcols != NULL && obj_subcols != Py_None) {
+    if (obj_subcols != Py_None) {
         array_subcols = (PyArrayObject*)PyArray_ContiguousFromAny(obj_subcols, NPY_INTP, 0, 0);
         if (!array_subcols) {
             return NULL;
         }
         if (PyArray_NDIM(array_subcols) != 1) {
             PyErr_Format(PyExc_ValueError,
                         "subcols expected a 1-D array, got a %d array",
@@ -171,33 +171,43 @@
     if (!a)
         goto cleanup;
 
     b = PyArray_SimpleNew(1, dim, NPY_INT64);
     if (!b)
         goto cleanup;
 
-    int ret = solve_rectangular_linear_sum_assignment_dtype(
+    int64_t* a_data = PyArray_DATA((PyArrayObject*)a);
+    int64_t* b_data = PyArray_DATA((PyArrayObject*)b);
+    int ret;
+    NPY_BEGIN_ALLOW_THREADS
+    ret = solve_rectangular_linear_sum_assignment_dtype(
       num_rows, num_cols, cost_matrix, dtype, maximize,
       subrows, n_subrows, subcols, n_subcols,
-      PyArray_DATA((PyArrayObject*)a),
-      PyArray_DATA((PyArrayObject*)b));
+      a_data, b_data);
+    NPY_END_ALLOW_THREADS
+
     if (ret == RECTANGULAR_LSAP_INFEASIBLE) {
         PyErr_SetString(PyExc_ValueError, "cost matrix is infeasible");
         goto cleanup;
     }
     else if (ret == RECTANGULAR_LSAP_INVALID) {
         PyErr_SetString(PyExc_ValueError,
                         "matrix contains invalid numeric entries");
         goto cleanup;
     }
     else if (ret == RECTANGULAR_LSAP_SUBSCRIPT_INVALID) {
         PyErr_SetString(PyExc_ValueError,
                         "subrows or subcols is invalid");
         goto cleanup;
     }
+    else if (ret == RECTANGULAR_LSAP_DTYPE_INVALID) {
+        PyErr_SetString(PyExc_ValueError,
+                        "dtype is invalid");
+        goto cleanup;
+    }
 
     result = Py_BuildValue("OO", a, b);
 
 cleanup:
     Py_XDECREF((PyObject*)array_subcols);
     Py_XDECREF((PyObject*)array_subrows);
     Py_XDECREF((PyObject*)obj_cont);
```

### Comparing `nanolsap-0.1.0/src/nanolsap/rectangular_lsap/rectangular_lsap.cpp` & `nanolsap-0.1.1/src/nanolsap/rectangular_lsap/rectangular_lsap.cpp`

 * *Files identical despite different names*

### Comparing `nanolsap-0.1.0/src/nanolsap/rectangular_lsap/rectangular_lsap.h` & `nanolsap-0.1.1/src/nanolsap/rectangular_lsap/rectangular_lsap.h`

 * *Files identical despite different names*

### Comparing `nanolsap-0.1.0/src/nanolsap.egg-info/PKG-INFO` & `nanolsap-0.1.1/src/nanolsap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanolsap
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python module to solve the linear sum assignment problem (LSAP) low memory friendly
 Author-email: hzqmwne <huangzhengqmwne@sina.cn>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/hzqmwne/nanolsap
 Keywords: lsap,munkres,kuhn-munkres,linear sum assignment problem
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nanolsap-0.1.0/src/nanolsap.egg-info/SOURCES.txt` & `nanolsap-0.1.1/src/nanolsap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nanolsap-0.1.0/tests/test_linear_assignment.py` & `nanolsap-0.1.1/tests/test_linear_assignment.py`

 * *Files identical despite different names*

### Comparing `nanolsap-0.1.0/tests/test_solve.py` & `nanolsap-0.1.1/tests/test_solve.py`

 * *Files identical despite different names*

### Comparing `nanolsap-0.1.0/tests/test_subrowcol.py` & `nanolsap-0.1.1/tests/test_subrowcol.py`

 * *Files identical despite different names*

