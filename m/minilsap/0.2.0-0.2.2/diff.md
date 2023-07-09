# Comparing `tmp/minilsap-0.2.0.tar.gz` & `tmp/minilsap-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minilsap-0.2.0.tar", last modified: Mon Feb  7 21:30:58 2022, max compression
+gzip compressed data, was "minilsap-0.2.2.tar", last modified: Sun Jul  9 13:17:03 2023, max compression
```

## Comparing `minilsap-0.2.0.tar` & `minilsap-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 21:30:58.236726 minilsap-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1443 2022-02-07 21:30:42.000000 minilsap-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-02-07 21:30:42.000000 minilsap-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1283 2022-02-07 21:30:58.236726 minilsap-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      693 2022-02-07 21:30:42.000000 minilsap-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-02-07 21:30:42.000000 minilsap-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      797 2022-02-07 21:30:58.240727 minilsap-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1154 2022-02-07 21:30:42.000000 minilsap-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 21:30:58.236726 minilsap-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 21:30:58.236726 minilsap-0.2.0/src/_lsap/
--rw-r--r--   0 runner    (1001) docker     (121)     4623 2022-02-07 21:30:42.000000 minilsap-0.2.0/src/_lsap/_lsap_module.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     7683 2022-02-07 21:30:42.000000 minilsap-0.2.0/src/_lsap/rectangular_lsap.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1920 2022-02-07 21:30:42.000000 minilsap-0.2.0/src/_lsap/rectangular_lsap.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 21:30:58.236726 minilsap-0.2.0/src/minilsap/
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-02-07 21:30:42.000000 minilsap-0.2.0/src/minilsap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-02-07 21:30:42.000000 minilsap-0.2.0/src/minilsap/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1027 2022-02-07 21:30:42.000000 minilsap-0.2.0/src/minilsap/solver.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 21:30:58.236726 minilsap-0.2.0/src/minilsap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1283 2022-02-07 21:30:58.000000 minilsap-0.2.0/src/minilsap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      402 2022-02-07 21:30:58.000000 minilsap-0.2.0/src/minilsap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-07 21:30:58.000000 minilsap-0.2.0/src/minilsap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-02-07 21:30:58.000000 minilsap-0.2.0/src/minilsap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-02-07 21:30:58.000000 minilsap-0.2.0/src/minilsap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:17:03.374289 minilsap-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-09 13:16:51.000000 minilsap-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-09 13:16:51.000000 minilsap-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-09 13:17:03.374289 minilsap-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-09 13:16:51.000000 minilsap-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-09 13:16:51.000000 minilsap-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-09 13:17:03.374289 minilsap-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-09 13:16:51.000000 minilsap-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:17:03.374289 minilsap-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:17:03.374289 minilsap-0.2.2/src/_lsap/
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-07-09 13:16:51.000000 minilsap-0.2.2/src/_lsap/_lsap_module.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7683 2023-07-09 13:16:51.000000 minilsap-0.2.2/src/_lsap/rectangular_lsap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-09 13:16:51.000000 minilsap-0.2.2/src/_lsap/rectangular_lsap.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:17:03.374289 minilsap-0.2.2/src/minilsap/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-09 13:16:51.000000 minilsap-0.2.2/src/minilsap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-09 13:16:51.000000 minilsap-0.2.2/src/minilsap/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-09 13:16:51.000000 minilsap-0.2.2/src/minilsap/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:17:03.374289 minilsap-0.2.2/src/minilsap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-09 13:17:03.000000 minilsap-0.2.2/src/minilsap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-09 13:17:03.000000 minilsap-0.2.2/src/minilsap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 13:17:03.000000 minilsap-0.2.2/src/minilsap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-09 13:17:03.000000 minilsap-0.2.2/src/minilsap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-09 13:17:03.000000 minilsap-0.2.2/src/minilsap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:17:03.374289 minilsap-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-09 13:16:51.000000 minilsap-0.2.2/tests/test_solve.py
```

### Comparing `minilsap-0.2.0/LICENSE` & `minilsap-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `minilsap-0.2.0/PKG-INFO` & `minilsap-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: minilsap
-Version: 0.2.0
+Version: 0.2.2
 Summary: Python module to solve the linear sum assignment problem (LSAP) efficiently
 Home-page: https://github.com/ntamas/lsap
 Maintainer: Tamas Nepusz
 Maintainer-email: ntamas@gmail.com
 License: BSD 3-Clause License
 Keywords: lsap,munkres,kuhn-munkres,linear sum assignment problem
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -32,9 +31,7 @@
 -------
 
 The code in this repository is licensed under the 3-clause BSD license, except
 for files including a different license header.
 
 The LSAP solver copied from SciPy is also licensed under the 3-clause BSD
 license.
-
-
```

### Comparing `minilsap-0.2.0/README.md` & `minilsap-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `minilsap-0.2.0/setup.cfg` & `minilsap-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `minilsap-0.2.0/setup.py` & `minilsap-0.2.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,21 +20,21 @@
                     f"cp{PY_LIMITED_API_VERSION[0]}{PY_LIMITED_API_VERSION[1]}"
                 )
                 super().finalize_options()
 
         cmdclass = {"bdist_wheel": bdist_wheel}
 else:
     cmdclass = {}
-setup_args = dict(
-    ext_modules=[
+setup_args = {
+    "ext_modules": [
         Extension(
             "minilsap._lsap",
             ["src/_lsap/rectangular_lsap.cpp", "src/_lsap/_lsap_module.cpp"],
             py_limited_api=True,
             include_dirs=[numpy.get_include()],
             extra_compile_args=["-std=c++11", "-Wall"],
             define_macros=[("Py_LIMITED_API", PY_LIMITED_API), ("PY_SSIZE_T_CLEAN", 1)],
         )
     ],
-    cmdclass=cmdclass,
-)
+    "cmdclass": cmdclass,
+}
 setup(**setup_args)
```

### Comparing `minilsap-0.2.0/src/_lsap/_lsap_module.cpp` & `minilsap-0.2.2/src/_lsap/_lsap_module.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     PyObject* a = NULL;
     PyObject* b = NULL;
     PyObject* result = NULL;
     PyObject* obj_cost = NULL;
     int maximize = 0;
     int ret;
     npy_intp num_rows, num_cols, dim;
+    int64_t *pa, *pb;
     double* cost_matrix;
 
     if (!PyArg_ParseTuple(args, "Op", &obj_cost, &maximize))
         return NULL;
 
     PyArrayObject* obj_cont = (PyArrayObject*)PyArray_ContiguousFromAny(obj_cost, NPY_DOUBLE, 0, 0);
     if (!obj_cont) {
@@ -93,18 +94,24 @@
     if (!a)
         goto cleanup;
 
     b = PyArray_SimpleNew(1, &dim, NPY_INT64);
     if (!b)
         goto cleanup;
 
+    pa = (int64_t*)PyArray_DATA((PyArrayObject*)a);
+    pb = (int64_t*)PyArray_DATA((PyArrayObject*)b);
+
+    Py_BEGIN_ALLOW_THREADS;
+
     ret = solve_rectangular_linear_sum_assignment(
-        num_rows, num_cols, cost_matrix, maximize,
-        (int64_t*)PyArray_DATA((PyArrayObject*)a),
-        (int64_t*)PyArray_DATA((PyArrayObject*)b));
+        num_rows, num_cols, cost_matrix, maximize, pa, pb);
+
+    Py_END_ALLOW_THREADS;
+
     if (ret == RECTANGULAR_LSAP_INFEASIBLE) {
         PyErr_SetString(PyExc_ValueError, "cost matrix is infeasible");
         goto cleanup;
     } else if (ret == RECTANGULAR_LSAP_INVALID) {
         PyErr_SetString(PyExc_ValueError,
             "matrix contains invalid numeric entries");
         goto cleanup;
```

### Comparing `minilsap-0.2.0/src/_lsap/rectangular_lsap.cpp` & `minilsap-0.2.2/src/_lsap/rectangular_lsap.cpp`

 * *Files identical despite different names*

### Comparing `minilsap-0.2.0/src/_lsap/rectangular_lsap.h` & `minilsap-0.2.2/src/_lsap/rectangular_lsap.h`

 * *Files identical despite different names*

### Comparing `minilsap-0.2.0/src/minilsap/solver.py` & `minilsap-0.2.2/src/minilsap/solver.py`

 * *Files identical despite different names*

### Comparing `minilsap-0.2.0/src/minilsap.egg-info/PKG-INFO` & `minilsap-0.2.2/src/minilsap.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: minilsap
-Version: 0.2.0
+Version: 0.2.2
 Summary: Python module to solve the linear sum assignment problem (LSAP) efficiently
 Home-page: https://github.com/ntamas/lsap
 Maintainer: Tamas Nepusz
 Maintainer-email: ntamas@gmail.com
 License: BSD 3-Clause License
 Keywords: lsap,munkres,kuhn-munkres,linear sum assignment problem
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -32,9 +31,7 @@
 -------
 
 The code in this repository is licensed under the 3-clause BSD license, except
 for files including a different license header.
 
 The LSAP solver copied from SciPy is also licensed under the 3-clause BSD
 license.
-
-
```

