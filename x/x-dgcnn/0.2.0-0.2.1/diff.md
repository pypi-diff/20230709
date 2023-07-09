# Comparing `tmp/x-dgcnn-0.2.0.tar.gz` & `tmp/x-dgcnn-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "x-dgcnn-0.2.0.tar", last modified: Fri Jul  7 06:02:15 2023, max compression
+gzip compressed data, was "x-dgcnn-0.2.1.tar", last modified: Sun Jul  9 18:48:27 2023, max compression
```

## Comparing `x-dgcnn-0.2.0.tar` & `x-dgcnn-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:02:15.470608 x-dgcnn-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-07 06:02:05.000000 x-dgcnn-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-07 06:02:15.470608 x-dgcnn-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-07-07 06:02:05.000000 x-dgcnn-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 06:02:15.470608 x-dgcnn-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-07 06:02:05.000000 x-dgcnn-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:02:15.470608 x-dgcnn-0.2.0/x_dgcnn/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-07 06:02:05.000000 x-dgcnn-0.2.0/x_dgcnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9230 2023-07-07 06:02:05.000000 x-dgcnn-0.2.0/x_dgcnn/dgcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-07 06:02:05.000000 x-dgcnn-0.2.0/x_dgcnn/route.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:02:15.470608 x-dgcnn-0.2.0/x_dgcnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-07 06:02:15.000000 x-dgcnn-0.2.0/x_dgcnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-07 06:02:15.000000 x-dgcnn-0.2.0/x_dgcnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 06:02:15.000000 x-dgcnn-0.2.0/x_dgcnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-07 06:02:15.000000 x-dgcnn-0.2.0/x_dgcnn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 06:02:15.000000 x-dgcnn-0.2.0/x_dgcnn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:48:27.875172 x-dgcnn-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-09 18:48:17.000000 x-dgcnn-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-09 18:48:27.875172 x-dgcnn-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-07-09 18:48:17.000000 x-dgcnn-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 18:48:27.875172 x-dgcnn-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-09 18:48:17.000000 x-dgcnn-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:48:27.875172 x-dgcnn-0.2.1/x_dgcnn/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-09 18:48:17.000000 x-dgcnn-0.2.1/x_dgcnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-07-09 18:48:17.000000 x-dgcnn-0.2.1/x_dgcnn/dgcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-09 18:48:17.000000 x-dgcnn-0.2.1/x_dgcnn/route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10048 2023-07-09 18:48:17.000000 x-dgcnn-0.2.1/x_dgcnn/x_dgcnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:48:27.875172 x-dgcnn-0.2.1/x_dgcnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-09 18:48:27.000000 x-dgcnn-0.2.1/x_dgcnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-09 18:48:27.000000 x-dgcnn-0.2.1/x_dgcnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 18:48:27.000000 x-dgcnn-0.2.1/x_dgcnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-09 18:48:27.000000 x-dgcnn-0.2.1/x_dgcnn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-09 18:48:27.000000 x-dgcnn-0.2.1/x_dgcnn.egg-info/top_level.txt
```

### Comparing `x-dgcnn-0.2.0/LICENSE` & `x-dgcnn-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `x-dgcnn-0.2.0/PKG-INFO` & `x-dgcnn-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x-dgcnn
-Version: 0.2.0
+Version: 0.2.1
 Summary: X-DGCNN - Pytorch
 Home-page: https://github.com/kentechx/x-dgcnn
 Author: Kaidi Shen
 License: MIT
 Keywords: 3D segmentation,3D classification,point cloud understanding
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `x-dgcnn-0.2.0/README.md` & `x-dgcnn-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `x-dgcnn-0.2.0/setup.py` & `x-dgcnn-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='x-dgcnn',
     packages=find_packages(),
-    version='0.2.0',
+    version='0.2.1',
     license='MIT',
     description='X-DGCNN - Pytorch',
     author='Kaidi Shen',
     url='https://github.com/kentechx/x-dgcnn',
     long_description_content_type='text/markdown',
     keywords=[
         '3D segmentation',
```

### Comparing `x-dgcnn-0.2.0/x_dgcnn/dgcnn.py` & `x-dgcnn-0.2.1/x_dgcnn/dgcnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,14 +204,15 @@
             k,
             in_dim,
             out_dim,
             emb_dim=1024,
             n_category=0,
             depth=3,
             stn: SpatialTransformNet = None,
+            head_norm=True,
             dynamic=True,
             dropout=0,
     ):
         super().__init__()
         self.k = k
         self.dynamic = dynamic
 
@@ -225,15 +226,15 @@
         )
         for _ in range(depth - 2):
             self.blocks.append(EdgeConv(k=k, dims=(64, 64, 64)))
         self.blocks.append(EdgeConv(k=k, dims=(64, 64)))
 
         # global linear
         self.lin = nn.Conv1d(depth * 64, emb_dim, 1, bias=False)
-        self.norm = nn.BatchNorm1d(emb_dim)
+        self.norm = nn.BatchNorm1d(emb_dim) if head_norm else nn.Identity()
         self.act = nn.GELU()
         self.dropout = nn.Dropout(dropout) if dropout > 0 else nn.Identity()
 
         # head
         dim = emb_dim + depth * 64
         self.mlp = nn.Sequential(
             nn.Conv1d(dim, 512, 1, bias=False),
```

### Comparing `x-dgcnn-0.2.0/x_dgcnn/route.py` & `x-dgcnn-0.2.1/x_dgcnn/route.py`

 * *Files identical despite different names*

### Comparing `x-dgcnn-0.2.0/x_dgcnn.egg-info/PKG-INFO` & `x-dgcnn-0.2.1/x_dgcnn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x-dgcnn
-Version: 0.2.0
+Version: 0.2.1
 Summary: X-DGCNN - Pytorch
 Home-page: https://github.com/kentechx/x-dgcnn
 Author: Kaidi Shen
 License: MIT
 Keywords: 3D segmentation,3D classification,point cloud understanding
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

