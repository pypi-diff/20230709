# Comparing `tmp/libsvm-official-3.31.0.tar.gz` & `tmp/libsvm-official-3.32.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libsvm-official-3.31.0.tar", last modified: Sat Mar  4 06:11:09 2023, max compression
+gzip compressed data, was "libsvm-official-3.32.0.tar", last modified: Sat Jul  8 14:40:03 2023, max compression
```

## Comparing `libsvm-official-3.31.0.tar` & `libsvm-official-3.32.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-03-04 06:11:09.398995 libsvm-official-3.31.0/
--rw-rw-rw-   0        0        0     1528 2023-03-04 06:11:07.000000 libsvm-official-3.31.0/LICENSE
--rw-rw-rw-   0        0        0       48 2023-02-27 12:14:41.000000 libsvm-official-3.31.0/MANIFEST.in
--rw-rw-rw-   0        0        0    18055 2023-03-04 06:11:09.397999 libsvm-official-3.31.0/PKG-INFO
--rw-rw-rw-   0        0        0    17733 2023-02-27 12:14:41.000000 libsvm-official-3.31.0/README
-drwxrwxrwx   0        0        0        0 2023-03-04 06:11:09.329654 libsvm-official-3.31.0/cpp-source/
--rw-rw-rw-   0        0        0    72157 2023-03-04 06:11:07.000000 libsvm-official-3.31.0/cpp-source/svm.cpp
--rw-rw-rw-   0        0        0      498 2023-03-04 06:11:07.000000 libsvm-official-3.31.0/cpp-source/svm.def
--rw-rw-rw-   0        0        0     3559 2023-03-04 06:11:07.000000 libsvm-official-3.31.0/cpp-source/svm.h
-drwxrwxrwx   0        0        0        0 2023-03-04 06:11:09.344144 libsvm-official-3.31.0/libsvm/
--rw-rw-rw-   0        0        0        0 2023-02-27 12:14:41.000000 libsvm-official-3.31.0/libsvm/__init__.py
--rw-rw-rw-   0        0        0     6384 2023-02-27 12:14:41.000000 libsvm-official-3.31.0/libsvm/commonutil.py
--rw-rw-rw-   0        0        0    16504 2023-02-27 12:14:41.000000 libsvm-official-3.31.0/libsvm/svm.py
--rw-rw-rw-   0        0        0    10805 2023-02-27 12:14:41.000000 libsvm-official-3.31.0/libsvm/svmutil.py
-drwxrwxrwx   0        0        0        0 2023-03-04 06:11:09.395007 libsvm-official-3.31.0/libsvm_official.egg-info/
--rw-rw-rw-   0        0        0    18055 2023-03-04 06:11:08.000000 libsvm-official-3.31.0/libsvm_official.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2023-03-04 06:11:09.000000 libsvm-official-3.31.0/libsvm_official.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-04 06:11:08.000000 libsvm-official-3.31.0/libsvm_official.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-03-04 06:11:08.000000 libsvm-official-3.31.0/libsvm_official.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-04 06:11:08.000000 libsvm-official-3.31.0/libsvm_official.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-04 06:11:09.399993 libsvm-official-3.31.0/setup.cfg
--rw-rw-rw-   0        0        0     3561 2023-02-27 12:14:41.000000 libsvm-official-3.31.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 14:40:03.504759 libsvm-official-3.32.0/
+-rw-rw-rw-   0        0        0     1528 2023-07-08 14:40:03.000000 libsvm-official-3.32.0/LICENSE
+-rw-rw-rw-   0        0        0       48 2023-07-08 13:41:26.000000 libsvm-official-3.32.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    18055 2023-07-08 14:40:03.503755 libsvm-official-3.32.0/PKG-INFO
+-rw-rw-rw-   0        0        0    17733 2023-07-08 13:41:26.000000 libsvm-official-3.32.0/README
+drwxrwxrwx   0        0        0        0 2023-07-08 14:40:03.465926 libsvm-official-3.32.0/cpp-source/
+-rw-rw-rw-   0        0        0    72157 2023-07-08 14:40:03.000000 libsvm-official-3.32.0/cpp-source/svm.cpp
+-rw-rw-rw-   0        0        0      498 2023-07-08 14:40:03.000000 libsvm-official-3.32.0/cpp-source/svm.def
+-rw-rw-rw-   0        0        0     3559 2023-07-08 14:40:03.000000 libsvm-official-3.32.0/cpp-source/svm.h
+drwxrwxrwx   0        0        0        0 2023-07-08 14:40:03.471919 libsvm-official-3.32.0/libsvm/
+-rw-rw-rw-   0        0        0        0 2023-07-08 13:41:26.000000 libsvm-official-3.32.0/libsvm/__init__.py
+-rw-rw-rw-   0        0        0     6384 2023-07-08 13:41:26.000000 libsvm-official-3.32.0/libsvm/commonutil.py
+-rw-rw-rw-   0        0        0    16712 2023-07-08 13:41:26.000000 libsvm-official-3.32.0/libsvm/svm.py
+-rw-rw-rw-   0        0        0    10805 2023-07-08 13:41:26.000000 libsvm-official-3.32.0/libsvm/svmutil.py
+drwxrwxrwx   0        0        0        0 2023-07-08 14:40:03.501178 libsvm-official-3.32.0/libsvm_official.egg-info/
+-rw-rw-rw-   0        0        0    18055 2023-07-08 14:40:03.000000 libsvm-official-3.32.0/libsvm_official.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-07-08 14:40:03.000000 libsvm-official-3.32.0/libsvm_official.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 14:40:03.000000 libsvm-official-3.32.0/libsvm_official.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-08 14:40:03.000000 libsvm-official-3.32.0/libsvm_official.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-08 14:40:03.000000 libsvm-official-3.32.0/libsvm_official.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 14:40:03.504759 libsvm-official-3.32.0/setup.cfg
+-rw-rw-rw-   0        0        0     3561 2023-07-08 13:41:26.000000 libsvm-official-3.32.0/setup.py
```

### Comparing `libsvm-official-3.31.0/LICENSE` & `libsvm-official-3.32.0/LICENSE`

 * *Files identical despite different names*

### Comparing `libsvm-official-3.31.0/PKG-INFO` & `libsvm-official-3.32.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libsvm-official
-Version: 3.31.0
+Version: 3.32.0
 Summary: Python binding of LIBSVM
 Home-page: https://www.csie.ntu.edu.tw/~cjlin/libsvm
 Author: ML group @ National Taiwan University
 Author-email: cjlin@csie.ntu.edu.tw
 License: BSD-3-Clause
 Description-Content-Type: text/plain
 License-File: LICENSE
```

### Comparing `libsvm-official-3.31.0/README` & `libsvm-official-3.32.0/README`

 * *Files identical despite different names*

### Comparing `libsvm-official-3.31.0/cpp-source/svm.cpp` & `libsvm-official-3.32.0/cpp-source/svm.cpp`

 * *Files identical despite different names*

### Comparing `libsvm-official-3.31.0/cpp-source/svm.h` & `libsvm-official-3.32.0/cpp-source/svm.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #ifndef _LIBSVM_H
 #define _LIBSVM_H
 
-#define LIBSVM_VERSION 331
+#define LIBSVM_VERSION 332
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 extern int libsvm_version;
```

### Comparing `libsvm-official-3.31.0/libsvm/commonutil.py` & `libsvm-official-3.32.0/libsvm/commonutil.py`

 * *Files identical despite different names*

### Comparing `libsvm-official-3.31.0/libsvm/svm.py` & `libsvm-official-3.32.0/libsvm/svm.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,15 +160,17 @@
 
 def csr_to_problem(x, prob, isKernel):
     if not x.has_sorted_indices:
         x.sort_indices()
 
     # Extra space for termination node and (possibly) bias term
     x_space = prob.x_space = np.empty((x.nnz+x.shape[0]), dtype=svm_node)
-    prob.rowptr = x.indptr.copy()
+    # rowptr has to be a 64bit integer because it will later be used for pointer arithmetic,
+    # which overflows when the added pointer points to an address that is numerically high.
+    prob.rowptr = x.indptr.astype(np.int64, copy=True)
     prob.rowptr[1:] += np.arange(1,x.shape[0]+1)
     prob_ind = x_space["index"]
     prob_val = x_space["value"]
     prob_ind[:] = -1
     if not isKernel:
         indx_start = 1 # index starts from 1
     else:
```

### Comparing `libsvm-official-3.31.0/libsvm/svmutil.py` & `libsvm-official-3.32.0/libsvm/svmutil.py`

 * *Files identical despite different names*

### Comparing `libsvm-official-3.31.0/libsvm_official.egg-info/PKG-INFO` & `libsvm-official-3.32.0/libsvm_official.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libsvm-official
-Version: 3.31.0
+Version: 3.32.0
 Summary: Python binding of LIBSVM
 Home-page: https://www.csie.ntu.edu.tw/~cjlin/libsvm
 Author: ML group @ National Taiwan University
 Author-email: cjlin@csie.ntu.edu.tw
 License: BSD-3-Clause
 Description-Content-Type: text/plain
 License-File: LICENSE
```

### Comparing `libsvm-official-3.31.0/setup.py` & `libsvm-official-3.32.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from distutils.command.build_ext import build_ext
 
 build_ext.get_export_symbols = lambda x, y: []
 
 
 PACKAGE_DIR = "libsvm"
 PACKAGE_NAME = "libsvm-official"
-VERSION = "3.31.0"
+VERSION = "3.32.0"
 cpp_dir = "cpp-source"
 # should be consistent with dynamic_lib_name in libsvm/svm.py
 dynamic_lib_name = "clib"
 
 # sources to be included to build the shared library
 source_codes = [
     "svm.cpp",
```

