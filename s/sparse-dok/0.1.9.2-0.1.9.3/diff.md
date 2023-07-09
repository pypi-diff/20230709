# Comparing `tmp/sparse_dok-0.1.9.2.tar.gz` & `tmp/sparse_dok-0.1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparse_dok-0.1.9.2.tar", last modified: Sun Jul  9 03:15:49 2023, max compression
+gzip compressed data, was "sparse_dok-0.1.9.3.tar", last modified: Sun Jul  9 13:59:16 2023, max compression
```

## Comparing `sparse_dok-0.1.9.2.tar` & `sparse_dok-0.1.9.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 03:15:49.121091 sparse_dok-0.1.9.2/
--rw-rw-rw-   0        0        0     1088 2023-07-08 01:12:38.000000 sparse_dok-0.1.9.2/LICENCE
--rw-rw-rw-   0        0        0       39 2022-06-03 19:13:32.000000 sparse_dok-0.1.9.2/MANIFEST.in
--rw-rw-rw-   0        0        0      956 2023-07-09 03:15:49.121091 sparse_dok-0.1.9.2/PKG-INFO
--rw-rw-rw-   0        0        0     8731 2023-07-08 01:12:38.000000 sparse_dok-0.1.9.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-09 03:15:49.121091 sparse_dok-0.1.9.2/setup.cfg
--rw-rw-rw-   0        0        0     1303 2023-07-08 01:14:44.000000 sparse_dok-0.1.9.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-09 03:15:49.019967 sparse_dok-0.1.9.2/sparse_dok/
--rw-rw-rw-   0        0        0       95 2023-07-08 01:11:28.000000 sparse_dok-0.1.9.2/sparse_dok/__init__.py
--rw-rw-rw-   0        0        0       23 2023-07-09 03:15:12.000000 sparse_dok-0.1.9.2/sparse_dok/__version__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 03:15:49.043782 sparse_dok-0.1.9.2/sparse_dok/components/
--rw-rw-rw-   0        0        0       98 2022-06-03 18:42:54.000000 sparse_dok-0.1.9.2/sparse_dok/components/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 03:15:49.117581 sparse_dok-0.1.9.2/sparse_dok/components/cuda/
--rw-rw-rw-   0        0        0        0 2022-05-23 01:01:14.000000 sparse_dok-0.1.9.2/sparse_dok/components/cuda/__init__.py
--rw-rw-rw-   0        0        0     2878 2022-05-30 20:40:04.000000 sparse_dok-0.1.9.2/sparse_dok/components/cuda/binary_search.cu
--rw-rw-rw-   0        0        0    18343 2022-05-24 15:02:58.000000 sparse_dok-0.1.9.2/sparse_dok/components/cuda/bitonic.cu
--rw-rw-rw-   0        0        0    14628 2022-05-23 01:50:08.000000 sparse_dok-0.1.9.2/sparse_dok/components/cuda/bmm_helpers.cu
--rw-rw-rw-   0        0        0     6398 2022-11-15 22:41:58.000000 sparse_dok-0.1.9.2/sparse_dok/components/cuda/closed_hashmap_impl.cu
--rw-rw-rw-   0        0        0     9929 2023-07-09 03:12:32.000000 sparse_dok-0.1.9.2/sparse_dok/components/cuda/closed_hashmap_impl.py
--rw-rw-rw-   0        0        0    18328 2022-11-20 15:11:16.000000 sparse_dok-0.1.9.2/sparse_dok/components/cuda/closed_hashmap_impl_class.cu
--rw-rw-rw-   0        0        0    38155 2023-07-09 03:15:48.000000 sparse_dok-0.1.9.2/sparse_dok/components/cuda/closed_hashmap_impl_preview.cu
--rw-rw-rw-   0        0        0     6776 2022-11-19 20:13:52.000000 sparse_dok-0.1.9.2/sparse_dok/components/cuda/cuda_kernel.py
--rw-rw-rw-   0        0        0     1362 2022-11-11 22:10:53.000000 sparse_dok-0.1.9.2/sparse_dok/components/cuda/filtered_elementwise.py
--rw-rw-rw-   0        0        0     6711 2022-05-25 17:47:18.000000 sparse_dok-0.1.9.2/sparse_dok/components/cuda/hashmap.cu
--rw-rw-rw-   0        0        0     4028 2022-12-05 13:56:04.000000 sparse_dok-0.1.9.2/sparse_dok/components/cuda/head.cu
--rw-rw-rw-   0        0        0    35905 2022-11-17 22:43:16.000000 sparse_dok-0.1.9.2/sparse_dok/components/cuda/preview.cu
--rw-rw-rw-   0        0        0     3417 2022-11-15 23:20:13.000000 sparse_dok-0.1.9.2/sparse_dok/components/cuda/reduce.cu
--rw-rw-rw-   0        0        0    15548 2022-12-06 13:06:16.000000 sparse_dok-0.1.9.2/sparse_dok/components/cuda/safe_closed_hashmap_impl_class.cu
--rw-rw-rw-   0        0        0     7944 2022-05-31 14:14:10.000000 sparse_dok-0.1.9.2/sparse_dok/components/cuda/smem_hashmap.cu
--rw-rw-rw-   0        0        0     7903 2022-05-29 01:53:58.000000 sparse_dok-0.1.9.2/sparse_dok/components/cuda/smem_hashmap_simple.cu
--rw-rw-rw-   0        0        0     9395 2022-11-13 23:05:51.000000 sparse_dok-0.1.9.2/sparse_dok/components/cuda/smem_tensor.cu
--rw-rw-rw-   0        0        0    10707 2022-11-20 14:28:17.000000 sparse_dok-0.1.9.2/sparse_dok/components/cuda/sparse_dok_tensor_impl.cu
--rw-rw-rw-   0        0        0    25680 2023-07-09 03:15:06.000000 sparse_dok-0.1.9.2/sparse_dok/components/cuda/sparse_dok_tensor_impl.py
--rw-rw-rw-   0        0        0    52037 2023-07-09 03:15:48.000000 sparse_dok-0.1.9.2/sparse_dok/components/cuda/sparse_dok_tensor_impl_preview.cu
--rw-rw-rw-   0        0        0     1541 2022-05-24 20:22:36.000000 sparse_dok-0.1.9.2/sparse_dok/components/cuda/stack.cu
--rw-rw-rw-   0        0        0     6152 2022-11-20 23:38:59.000000 sparse_dok-0.1.9.2/sparse_dok/components/cuda/tensor_accessor.cu
--rw-rw-rw-   0        0        0    11198 2022-06-03 18:56:52.000000 sparse_dok-0.1.9.2/sparse_dok/components/cuda/topkspspcsim.cu
--rw-rw-rw-   0        0        0    10190 2022-11-11 21:44:22.000000 sparse_dok-0.1.9.2/sparse_dok/components/cuda/topkspspcsim.py
--rw-rw-rw-   0        0        0     1161 2022-11-17 22:40:56.000000 sparse_dok-0.1.9.2/sparse_dok/components/cuda_callable.py
--rw-rw-rw-   0        0        0    15308 2023-07-09 02:03:16.000000 sparse_dok-0.1.9.2/sparse_dok/components/cuda_closed_hashmap.py
--rw-rw-rw-   0        0        0    17858 2022-11-20 00:15:06.000000 sparse_dok-0.1.9.2/sparse_dok/components/sparse_dok_tensor.py
--rw-rw-rw-   0        0        0     6264 2022-11-11 21:43:04.000000 sparse_dok-0.1.9.2/sparse_dok/functions.py
--rw-rw-rw-   0        0        0    10849 2022-11-19 19:06:50.000000 sparse_dok-0.1.9.2/sparse_dok/util.py
-drwxrwxrwx   0        0        0        0 2023-07-09 03:15:49.039780 sparse_dok-0.1.9.2/sparse_dok.egg-info/
--rw-rw-rw-   0        0        0      956 2023-07-09 03:15:48.000000 sparse_dok-0.1.9.2/sparse_dok.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1705 2023-07-09 03:15:48.000000 sparse_dok-0.1.9.2/sparse_dok.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 03:15:48.000000 sparse_dok-0.1.9.2/sparse_dok.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-07-09 03:15:48.000000 sparse_dok-0.1.9.2/sparse_dok.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-09 03:15:48.000000 sparse_dok-0.1.9.2/sparse_dok.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-09 03:15:49.120092 sparse_dok-0.1.9.2/tests/
--rw-rw-rw-   0        0        0     2616 2022-11-13 00:44:01.000000 sparse_dok-0.1.9.2/tests/test_remove.py
--rw-rw-rw-   0        0        0     1587 2022-11-12 19:56:37.000000 sparse_dok-0.1.9.2/tests/test_reshape.py
--rw-rw-rw-   0        0        0     1490 2022-11-12 16:31:01.000000 sparse_dok-0.1.9.2/tests/test_sparse_dok_methods.py
--rw-rw-rw-   0        0        0     3121 2022-12-06 12:53:47.000000 sparse_dok-0.1.9.2/tests/test_spget.py
+drwxrwxrwx   0        0        0        0 2023-07-09 13:59:16.554011 sparse_dok-0.1.9.3/
+-rw-rw-rw-   0        0        0     1088 2023-07-08 01:12:38.000000 sparse_dok-0.1.9.3/LICENCE
+-rw-rw-rw-   0        0        0       39 2022-06-03 19:13:32.000000 sparse_dok-0.1.9.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      956 2023-07-09 13:59:16.554011 sparse_dok-0.1.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0     8731 2023-07-08 01:12:38.000000 sparse_dok-0.1.9.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-09 13:59:16.554011 sparse_dok-0.1.9.3/setup.cfg
+-rw-rw-rw-   0        0        0     1303 2023-07-08 01:14:44.000000 sparse_dok-0.1.9.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 13:59:16.463719 sparse_dok-0.1.9.3/sparse_dok/
+-rw-rw-rw-   0        0        0       95 2023-07-08 01:11:28.000000 sparse_dok-0.1.9.3/sparse_dok/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-07-09 13:50:07.000000 sparse_dok-0.1.9.3/sparse_dok/__version__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 13:59:16.480726 sparse_dok-0.1.9.3/sparse_dok/components/
+-rw-rw-rw-   0        0        0       98 2022-06-03 18:42:54.000000 sparse_dok-0.1.9.3/sparse_dok/components/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 13:59:16.550011 sparse_dok-0.1.9.3/sparse_dok/components/cuda/
+-rw-rw-rw-   0        0        0        0 2022-05-23 01:01:14.000000 sparse_dok-0.1.9.3/sparse_dok/components/cuda/__init__.py
+-rw-rw-rw-   0        0        0     2878 2022-05-30 20:40:04.000000 sparse_dok-0.1.9.3/sparse_dok/components/cuda/binary_search.cu
+-rw-rw-rw-   0        0        0    18343 2022-05-24 15:02:58.000000 sparse_dok-0.1.9.3/sparse_dok/components/cuda/bitonic.cu
+-rw-rw-rw-   0        0        0    14628 2022-05-23 01:50:08.000000 sparse_dok-0.1.9.3/sparse_dok/components/cuda/bmm_helpers.cu
+-rw-rw-rw-   0        0        0     6398 2022-11-15 22:41:58.000000 sparse_dok-0.1.9.3/sparse_dok/components/cuda/closed_hashmap_impl.cu
+-rw-rw-rw-   0        0        0     9929 2023-07-09 13:57:15.000000 sparse_dok-0.1.9.3/sparse_dok/components/cuda/closed_hashmap_impl.py
+-rw-rw-rw-   0        0        0    18328 2022-11-20 15:11:16.000000 sparse_dok-0.1.9.3/sparse_dok/components/cuda/closed_hashmap_impl_class.cu
+-rw-rw-rw-   0        0        0    38155 2023-07-09 13:59:15.000000 sparse_dok-0.1.9.3/sparse_dok/components/cuda/closed_hashmap_impl_preview.cu
+-rw-rw-rw-   0        0        0     6776 2022-11-19 20:13:52.000000 sparse_dok-0.1.9.3/sparse_dok/components/cuda/cuda_kernel.py
+-rw-rw-rw-   0        0        0     1362 2022-11-11 22:10:53.000000 sparse_dok-0.1.9.3/sparse_dok/components/cuda/filtered_elementwise.py
+-rw-rw-rw-   0        0        0     6711 2022-05-25 17:47:18.000000 sparse_dok-0.1.9.3/sparse_dok/components/cuda/hashmap.cu
+-rw-rw-rw-   0        0        0     4028 2022-12-05 13:56:04.000000 sparse_dok-0.1.9.3/sparse_dok/components/cuda/head.cu
+-rw-rw-rw-   0        0        0    35905 2022-11-17 22:43:16.000000 sparse_dok-0.1.9.3/sparse_dok/components/cuda/preview.cu
+-rw-rw-rw-   0        0        0     3417 2022-11-15 23:20:13.000000 sparse_dok-0.1.9.3/sparse_dok/components/cuda/reduce.cu
+-rw-rw-rw-   0        0        0    15548 2022-12-06 13:06:16.000000 sparse_dok-0.1.9.3/sparse_dok/components/cuda/safe_closed_hashmap_impl_class.cu
+-rw-rw-rw-   0        0        0     7944 2022-05-31 14:14:10.000000 sparse_dok-0.1.9.3/sparse_dok/components/cuda/smem_hashmap.cu
+-rw-rw-rw-   0        0        0     7903 2022-05-29 01:53:58.000000 sparse_dok-0.1.9.3/sparse_dok/components/cuda/smem_hashmap_simple.cu
+-rw-rw-rw-   0        0        0     9395 2022-11-13 23:05:51.000000 sparse_dok-0.1.9.3/sparse_dok/components/cuda/smem_tensor.cu
+-rw-rw-rw-   0        0        0    10707 2022-11-20 14:28:17.000000 sparse_dok-0.1.9.3/sparse_dok/components/cuda/sparse_dok_tensor_impl.cu
+-rw-rw-rw-   0        0        0    25686 2023-07-09 13:57:24.000000 sparse_dok-0.1.9.3/sparse_dok/components/cuda/sparse_dok_tensor_impl.py
+-rw-rw-rw-   0        0        0    52037 2023-07-09 13:59:16.000000 sparse_dok-0.1.9.3/sparse_dok/components/cuda/sparse_dok_tensor_impl_preview.cu
+-rw-rw-rw-   0        0        0     1541 2022-05-24 20:22:36.000000 sparse_dok-0.1.9.3/sparse_dok/components/cuda/stack.cu
+-rw-rw-rw-   0        0        0     6152 2022-11-20 23:38:59.000000 sparse_dok-0.1.9.3/sparse_dok/components/cuda/tensor_accessor.cu
+-rw-rw-rw-   0        0        0    11198 2022-06-03 18:56:52.000000 sparse_dok-0.1.9.3/sparse_dok/components/cuda/topkspspcsim.cu
+-rw-rw-rw-   0        0        0    10190 2022-11-11 21:44:22.000000 sparse_dok-0.1.9.3/sparse_dok/components/cuda/topkspspcsim.py
+-rw-rw-rw-   0        0        0     1161 2022-11-17 22:40:56.000000 sparse_dok-0.1.9.3/sparse_dok/components/cuda_callable.py
+-rw-rw-rw-   0        0        0    15308 2023-07-09 13:58:52.000000 sparse_dok-0.1.9.3/sparse_dok/components/cuda_closed_hashmap.py
+-rw-rw-rw-   0        0        0    17858 2022-11-20 00:15:06.000000 sparse_dok-0.1.9.3/sparse_dok/components/sparse_dok_tensor.py
+-rw-rw-rw-   0        0        0     6264 2022-11-11 21:43:04.000000 sparse_dok-0.1.9.3/sparse_dok/functions.py
+-rw-rw-rw-   0        0        0    10849 2022-11-19 19:06:50.000000 sparse_dok-0.1.9.3/sparse_dok/util.py
+drwxrwxrwx   0        0        0        0 2023-07-09 13:59:16.477719 sparse_dok-0.1.9.3/sparse_dok.egg-info/
+-rw-rw-rw-   0        0        0      956 2023-07-09 13:59:16.000000 sparse_dok-0.1.9.3/sparse_dok.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1705 2023-07-09 13:59:16.000000 sparse_dok-0.1.9.3/sparse_dok.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 13:59:16.000000 sparse_dok-0.1.9.3/sparse_dok.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-07-09 13:59:16.000000 sparse_dok-0.1.9.3/sparse_dok.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-09 13:59:16.000000 sparse_dok-0.1.9.3/sparse_dok.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-09 13:59:16.553011 sparse_dok-0.1.9.3/tests/
+-rw-rw-rw-   0        0        0     2616 2022-11-13 00:44:01.000000 sparse_dok-0.1.9.3/tests/test_remove.py
+-rw-rw-rw-   0        0        0     1587 2022-11-12 19:56:37.000000 sparse_dok-0.1.9.3/tests/test_reshape.py
+-rw-rw-rw-   0        0        0     1490 2022-11-12 16:31:01.000000 sparse_dok-0.1.9.3/tests/test_sparse_dok_methods.py
+-rw-rw-rw-   0        0        0     3121 2022-12-06 12:53:47.000000 sparse_dok-0.1.9.3/tests/test_spget.py
```

### Comparing `sparse_dok-0.1.9.2/LICENCE` & `sparse_dok-0.1.9.3/LICENCE`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9.2/PKG-INFO` & `sparse_dok-0.1.9.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sparse_dok
-Version: 0.1.9.2
+Version: 0.1.9.3
 Summary: sparse dok tensor implementation
 Home-page: https://github.com/DeMoriarty/SparseDOK
-Download-URL: https://github.com/DeMoriarty/SparseDOK/archive/v_0192.tar.gz
+Download-URL: https://github.com/DeMoriarty/SparseDOK/archive/v_0193.tar.gz
 Author: demoriarty
 Author-email: sahbanjan@gmail.com
 License: MIT
 Keywords: pytorch,sparse
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `sparse_dok-0.1.9.2/README.md` & `sparse_dok-0.1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9.2/setup.py` & `sparse_dok-0.1.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9.2/sparse_dok/components/cuda/binary_search.cu` & `sparse_dok-0.1.9.3/sparse_dok/components/cuda/binary_search.cu`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9.2/sparse_dok/components/cuda/bitonic.cu` & `sparse_dok-0.1.9.3/sparse_dok/components/cuda/bitonic.cu`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9.2/sparse_dok/components/cuda/bmm_helpers.cu` & `sparse_dok-0.1.9.3/sparse_dok/components/cuda/bmm_helpers.cu`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9.2/sparse_dok/components/cuda/closed_hashmap_impl.cu` & `sparse_dok-0.1.9.3/sparse_dok/components/cuda/closed_hashmap_impl.cu`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9.2/sparse_dok/components/cuda/closed_hashmap_impl.py` & `sparse_dok-0.1.9.3/sparse_dok/components/cuda/closed_hashmap_impl.py`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9.2/sparse_dok/components/cuda/closed_hashmap_impl_class.cu` & `sparse_dok-0.1.9.3/sparse_dok/components/cuda/closed_hashmap_impl_class.cu`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9.2/sparse_dok/components/cuda/closed_hashmap_impl_preview.cu` & `sparse_dok-0.1.9.3/sparse_dok/components/cuda/closed_hashmap_impl_preview.cu`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9.2/sparse_dok/components/cuda/cuda_kernel.py` & `sparse_dok-0.1.9.3/sparse_dok/components/cuda/cuda_kernel.py`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9.2/sparse_dok/components/cuda/filtered_elementwise.py` & `sparse_dok-0.1.9.3/sparse_dok/components/cuda/filtered_elementwise.py`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9.2/sparse_dok/components/cuda/hashmap.cu` & `sparse_dok-0.1.9.3/sparse_dok/components/cuda/hashmap.cu`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9.2/sparse_dok/components/cuda/head.cu` & `sparse_dok-0.1.9.3/sparse_dok/components/cuda/head.cu`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9.2/sparse_dok/components/cuda/preview.cu` & `sparse_dok-0.1.9.3/sparse_dok/components/cuda/preview.cu`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9.2/sparse_dok/components/cuda/reduce.cu` & `sparse_dok-0.1.9.3/sparse_dok/components/cuda/reduce.cu`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9.2/sparse_dok/components/cuda/safe_closed_hashmap_impl_class.cu` & `sparse_dok-0.1.9.3/sparse_dok/components/cuda/safe_closed_hashmap_impl_class.cu`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9.2/sparse_dok/components/cuda/smem_hashmap.cu` & `sparse_dok-0.1.9.3/sparse_dok/components/cuda/smem_hashmap.cu`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9.2/sparse_dok/components/cuda/smem_hashmap_simple.cu` & `sparse_dok-0.1.9.3/sparse_dok/components/cuda/smem_hashmap_simple.cu`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9.2/sparse_dok/components/cuda/smem_tensor.cu` & `sparse_dok-0.1.9.3/sparse_dok/components/cuda/smem_tensor.cu`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9.2/sparse_dok/components/cuda/sparse_dok_tensor_impl.cu` & `sparse_dok-0.1.9.3/sparse_dok/components/cuda/sparse_dok_tensor_impl.cu`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9.2/sparse_dok/components/cuda/sparse_dok_tensor_impl.py` & `sparse_dok-0.1.9.3/sparse_dok/components/cuda/sparse_dok_tensor_impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -408,15 +408,15 @@
             ]
         )
         # dest_hashmap._n_elements += n_src_elements
 
     def set_items_dense(self, dest_hashmap: CudaClosedHashmap, src: Tensor, selectors: list[Tensor]):
         if dest_hashmap._keys is None:
           first_key = torch.stack([s.data[0] for s in selectors], dim=0)[None] #[1, num_selectors]
-          first_value = src.data[0][None] #[1, 1]
+          first_value = src.data[0][None, None] #[1, 1]
           dest_hashmap.set(first_key, first_value)
           
         assert dest_hashmap.device == src.device
         assert all(isinstance(selector, Tensor) for selector in selectors), "all selectors must be Long Tensors"
         assert all(selector.dtype == torch.long for selector in selectors), "all selectors must be Long Tensors"
         assert all(selector.device == dest_hashmap.device for selector in selectors), "all selectors must be on the same cuda device as the SparseDOKTensor"
         assert all(selector.shape == selectors[0].shape for selector in selectors), "all selectors must be broadcasted to the same shape"
```

### Comparing `sparse_dok-0.1.9.2/sparse_dok/components/cuda/sparse_dok_tensor_impl_preview.cu` & `sparse_dok-0.1.9.3/sparse_dok/components/cuda/sparse_dok_tensor_impl_preview.cu`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9.2/sparse_dok/components/cuda/stack.cu` & `sparse_dok-0.1.9.3/sparse_dok/components/cuda/stack.cu`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9.2/sparse_dok/components/cuda/tensor_accessor.cu` & `sparse_dok-0.1.9.3/sparse_dok/components/cuda/tensor_accessor.cu`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9.2/sparse_dok/components/cuda/topkspspcsim.cu` & `sparse_dok-0.1.9.3/sparse_dok/components/cuda/topkspspcsim.cu`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9.2/sparse_dok/components/cuda/topkspspcsim.py` & `sparse_dok-0.1.9.3/sparse_dok/components/cuda/topkspspcsim.py`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9.2/sparse_dok/components/cuda_callable.py` & `sparse_dok-0.1.9.3/sparse_dok/components/cuda_callable.py`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9.2/sparse_dok/components/cuda_closed_hashmap.py` & `sparse_dok-0.1.9.3/sparse_dok/components/cuda_closed_hashmap.py`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9.2/sparse_dok/components/sparse_dok_tensor.py` & `sparse_dok-0.1.9.3/sparse_dok/components/sparse_dok_tensor.py`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9.2/sparse_dok/functions.py` & `sparse_dok-0.1.9.3/sparse_dok/functions.py`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9.2/sparse_dok/util.py` & `sparse_dok-0.1.9.3/sparse_dok/util.py`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9.2/sparse_dok.egg-info/PKG-INFO` & `sparse_dok-0.1.9.3/sparse_dok.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sparse-dok
-Version: 0.1.9.2
+Version: 0.1.9.3
 Summary: sparse dok tensor implementation
 Home-page: https://github.com/DeMoriarty/SparseDOK
-Download-URL: https://github.com/DeMoriarty/SparseDOK/archive/v_0192.tar.gz
+Download-URL: https://github.com/DeMoriarty/SparseDOK/archive/v_0193.tar.gz
 Author: demoriarty
 Author-email: sahbanjan@gmail.com
 License: MIT
 Keywords: pytorch,sparse
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `sparse_dok-0.1.9.2/sparse_dok.egg-info/SOURCES.txt` & `sparse_dok-0.1.9.3/sparse_dok.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9.2/tests/test_remove.py` & `sparse_dok-0.1.9.3/tests/test_remove.py`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9.2/tests/test_reshape.py` & `sparse_dok-0.1.9.3/tests/test_reshape.py`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9.2/tests/test_sparse_dok_methods.py` & `sparse_dok-0.1.9.3/tests/test_sparse_dok_methods.py`

 * *Files identical despite different names*

### Comparing `sparse_dok-0.1.9.2/tests/test_spget.py` & `sparse_dok-0.1.9.3/tests/test_spget.py`

 * *Files identical despite different names*

