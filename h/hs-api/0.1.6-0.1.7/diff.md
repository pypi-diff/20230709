# Comparing `tmp/hs_api-0.1.6.tar.gz` & `tmp/hs_api-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hs_api-0.1.6.tar", max compression
+gzip compressed data, was "hs_api-0.1.7.tar", max compression
```

## Comparing `hs_api-0.1.6.tar` & `hs_api-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       80 2023-07-06 05:05:08.874856 hs_api-0.1.6/hs_api/__init__.py
--rw-r--r--   0        0        0     8498 2023-06-25 19:30:59.213648 hs_api-0.1.6/hs_api/_intermediate_format.py
--rw-r--r--   0        0        0    18652 2023-07-08 22:23:06.393716 hs_api-0.1.6/hs_api/_simple_sim.py
--rw-r--r--   0        0        0    21280 2023-07-08 22:22:27.593969 hs_api-0.1.6/hs_api/api.py
--rw-r--r--   0        0        0    44903 2023-07-08 17:51:02.752663 hs_api-0.1.6/hs_api/converter.py
--rwxr-xr-x   0        0        0      655 2023-07-08 22:35:19.540696 hs_api-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      788 1970-01-01 00:00:00.000000 hs_api-0.1.6/setup.py
--rw-r--r--   0        0        0      559 1970-01-01 00:00:00.000000 hs_api-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       80 2023-07-06 05:05:08.874856 hs_api-0.1.7/hs_api/__init__.py
+-rw-r--r--   0        0        0     8498 2023-06-25 19:30:59.213648 hs_api-0.1.7/hs_api/_intermediate_format.py
+-rw-r--r--   0        0        0    18652 2023-07-08 22:23:06.393716 hs_api-0.1.7/hs_api/_simple_sim.py
+-rw-r--r--   0        0        0    21026 2023-07-08 22:52:25.377276 hs_api-0.1.7/hs_api/api.py
+-rw-r--r--   0        0        0    44903 2023-07-08 17:51:02.752663 hs_api-0.1.7/hs_api/converter.py
+-rwxr-xr-x   0        0        0      655 2023-07-08 22:53:50.828664 hs_api-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      788 1970-01-01 00:00:00.000000 hs_api-0.1.7/setup.py
+-rw-r--r--   0        0        0      559 1970-01-01 00:00:00.000000 hs_api-0.1.7/PKG-INFO
```

### Comparing `hs_api-0.1.6/hs_api/_intermediate_format.py` & `hs_api-0.1.7/hs_api/_intermediate_format.py`

 * *Files identical despite different names*

### Comparing `hs_api-0.1.6/hs_api/_simple_sim.py` & `hs_api-0.1.7/hs_api/_simple_sim.py`

 * *Files identical despite different names*

### Comparing `hs_api-0.1.6/hs_api/api.py` & `hs_api-0.1.7/hs_api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,20 +112,15 @@
                 logging.error(
                     "config does not contain neuron type or global neuron params"
                 )
         else:
             logging.error("config should be a dictionary")
 
         #self.perturb = perturb
-        if perturbMag > (6) or perturbMag < 0 or not isinstance(perturbMag, int):
-            raise perturbMagError('bad perturbMag')
         self.perturbMag = perturbMag
-        if perturbMag:
-            if perturbMag > 16:
-                logging.error("perturbMag must be less than 16")
         self.leak = leak
         if leak > 2**6:
             logging.error("Leak must be less than two to the sixth")
         self.simpleSim = None
         self.key2index = {}
         self.simDump = simDump
         self.connectome = None
```

### Comparing `hs_api-0.1.6/hs_api/converter.py` & `hs_api-0.1.7/hs_api/converter.py`

 * *Files identical despite different names*

### Comparing `hs_api-0.1.6/pyproject.toml` & `hs_api-0.1.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hs_api"
-version = "0.1.6"
+version = "0.1.7"
 description = "CRI User Software"
 authors = ["Justin Frank & Abhinav Uppal"]
 
 [tool.poetry.dependencies]
 
 python = ">=3.10,<3.11"
 numba = "^0.55.1"
```

### Comparing `hs_api-0.1.6/setup.py` & `hs_api-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'matplotlib>=3.5.1,<4.0.0',
  'numba>=0.55.1,<0.56.0',
  'numpy>=1.18',
  'tqdm>=4.64.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'hs-api',
-    'version': '0.1.6',
+    'version': '0.1.7',
     'description': 'CRI User Software',
     'long_description': 'None',
     'author': 'Justin Frank & Abhinav Uppal',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `hs_api-0.1.6/PKG-INFO` & `hs_api-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hs-api
-Version: 0.1.6
+Version: 0.1.7
 Summary: CRI User Software
 Author: Justin Frank & Abhinav Uppal
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: bidict (>=0.22.0,<0.23.0)
```

