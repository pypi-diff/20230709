# Comparing `tmp/hs_api-0.1.4.tar.gz` & `tmp/hs_api-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hs_api-0.1.4.tar", max compression
+gzip compressed data, was "hs_api-0.1.5.tar", max compression
```

## Comparing `hs_api-0.1.4.tar` & `hs_api-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       80 2023-07-06 05:05:08.874856 hs_api-0.1.4/hs_api/__init__.py
--rw-r--r--   0        0        0     8498 2023-06-25 19:30:59.213648 hs_api-0.1.4/hs_api/_intermediate_format.py
--rw-r--r--   0        0        0    18569 2023-07-08 18:14:10.137693 hs_api-0.1.4/hs_api/_simple_sim.py
--rw-r--r--   0        0        0    20965 2023-07-08 17:51:02.744663 hs_api-0.1.4/hs_api/api.py
--rw-r--r--   0        0        0    44903 2023-07-08 17:51:02.752663 hs_api-0.1.4/hs_api/converter.py
--rwxr-xr-x   0        0        0      655 2023-07-08 19:26:26.050352 hs_api-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      788 1970-01-01 00:00:00.000000 hs_api-0.1.4/setup.py
--rw-r--r--   0        0        0      559 1970-01-01 00:00:00.000000 hs_api-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       80 2023-07-06 05:05:08.874856 hs_api-0.1.5/hs_api/__init__.py
+-rw-r--r--   0        0        0     8498 2023-06-25 19:30:59.213648 hs_api-0.1.5/hs_api/_intermediate_format.py
+-rw-r--r--   0        0        0    18646 2023-07-08 22:11:33.538265 hs_api-0.1.5/hs_api/_simple_sim.py
+-rw-r--r--   0        0        0    21274 2023-07-08 22:16:06.588449 hs_api-0.1.5/hs_api/api.py
+-rw-r--r--   0        0        0    44903 2023-07-08 17:51:02.752663 hs_api-0.1.5/hs_api/converter.py
+-rwxr-xr-x   0        0        0      655 2023-07-08 22:13:16.961553 hs_api-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      788 1970-01-01 00:00:00.000000 hs_api-0.1.5/setup.py
+-rw-r--r--   0        0        0      559 1970-01-01 00:00:00.000000 hs_api-0.1.5/PKG-INFO
```

### Comparing `hs_api-0.1.4/hs_api/_intermediate_format.py` & `hs_api-0.1.5/hs_api/_intermediate_format.py`

 * *Files identical despite different names*

### Comparing `hs_api-0.1.4/hs_api/_simple_sim.py` & `hs_api-0.1.5/hs_api/_simple_sim.py`

 * *Files 1% similar despite different names*

```diff
@@ -354,14 +354,20 @@
             self.membranePotentials = phase_two(self.firedNeurons, currentInputs, self.membranePotentials, self.axons, self.connections)#update the membrane potentials
 
             #print(time, 'Vmem', self.membranePotentials)
 
             self.firedNeurons = [] #np.array([])
             #
     """
+
+    def set_perturbMag(perturbMag):
+        self.perturbMag = perturbMag
+
+
+
     def gen_weights(self):
         nNeurons = len(self.connections)
         nAxons = len(self.axons)
         S = Fxp(np.zeros((nNeurons,nNeurons)),dtype=self.formatDict['synapse_weights'])
         for key, value in self.connections.items():
             for synapse in value:
                 presynapticIdx = key
```

### Comparing `hs_api-0.1.4/hs_api/api.py` & `hs_api-0.1.5/hs_api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,14 +158,23 @@
                 self.connections,
                 outputs=formatedOutputs,
                 perturbMag=self.perturbMag,
                 leak=self.leak,
             )
         # breakpoint()
         # print("initialized")
+        #
+    def set_perturbMag(perturbMag):
+        if self.target == "simpleSim":
+            self.simpleSim.set_perturbMag(perturbMag)
+        elif self.target == "CRI":
+            logging.error('dynamic change in perturbMag not supported yet')
+        else:
+            logging.error('invalid target')
+
 
     def checkHw(self):
         """
         Checks if the magic file exists to demark that we're running on a system with CRI hardware accessible.
 
         Returns
         -------
```

### Comparing `hs_api-0.1.4/hs_api/converter.py` & `hs_api-0.1.5/hs_api/converter.py`

 * *Files identical despite different names*

### Comparing `hs_api-0.1.4/pyproject.toml` & `hs_api-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hs_api"
-version = "0.1.4"
+version = "0.1.5"
 description = "CRI User Software"
 authors = ["Justin Frank & Abhinav Uppal"]
 
 [tool.poetry.dependencies]
 
 python = ">=3.10,<3.11"
 numba = "^0.55.1"
```

### Comparing `hs_api-0.1.4/setup.py` & `hs_api-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'matplotlib>=3.5.1,<4.0.0',
  'numba>=0.55.1,<0.56.0',
  'numpy>=1.18',
  'tqdm>=4.64.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'hs-api',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': 'CRI User Software',
     'long_description': 'None',
     'author': 'Justin Frank & Abhinav Uppal',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `hs_api-0.1.4/PKG-INFO` & `hs_api-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hs-api
-Version: 0.1.4
+Version: 0.1.5
 Summary: CRI User Software
 Author: Justin Frank & Abhinav Uppal
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: bidict (>=0.22.0,<0.23.0)
```

