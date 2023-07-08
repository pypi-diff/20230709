# Comparing `tmp/hs_api-0.1.3.tar.gz` & `tmp/hs_api-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hs_api-0.1.3.tar", max compression
+gzip compressed data, was "hs_api-0.1.4.tar", max compression
```

## Comparing `hs_api-0.1.3.tar` & `hs_api-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       80 2023-06-29 04:10:27.993074 hs_api-0.1.3/hs_api/__init__.py
--rw-r--r--   0        0        0     8498 2023-06-20 17:13:45.081189 hs_api-0.1.3/hs_api/_intermediate_format.py
--rw-r--r--   0        0        0    18447 2023-06-28 06:32:25.512755 hs_api-0.1.3/hs_api/_simple_sim.py
--rw-r--r--   0        0        0    20819 2023-06-29 04:13:26.765143 hs_api-0.1.3/hs_api/api.py
--rw-r--r--   0        0        0    44903 2023-06-29 02:48:27.983459 hs_api-0.1.3/hs_api/converter.py
--rwxr-xr-x   0        0        0      616 2023-06-29 04:16:04.463323 hs_api-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      802 2023-06-29 04:17:32.992462 hs_api-0.1.3/setup.py
--rw-r--r--   0        0        0      597 2023-06-29 04:17:32.992675 hs_api-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       80 2023-07-06 05:05:08.874856 hs_api-0.1.4/hs_api/__init__.py
+-rw-r--r--   0        0        0     8498 2023-06-25 19:30:59.213648 hs_api-0.1.4/hs_api/_intermediate_format.py
+-rw-r--r--   0        0        0    18569 2023-07-08 18:14:10.137693 hs_api-0.1.4/hs_api/_simple_sim.py
+-rw-r--r--   0        0        0    20965 2023-07-08 17:51:02.744663 hs_api-0.1.4/hs_api/api.py
+-rw-r--r--   0        0        0    44903 2023-07-08 17:51:02.752663 hs_api-0.1.4/hs_api/converter.py
+-rwxr-xr-x   0        0        0      655 2023-07-08 19:26:26.050352 hs_api-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      788 1970-01-01 00:00:00.000000 hs_api-0.1.4/setup.py
+-rw-r--r--   0        0        0      559 1970-01-01 00:00:00.000000 hs_api-0.1.4/PKG-INFO
```

### Comparing `hs_api-0.1.3/hs_api/_intermediate_format.py` & `hs_api-0.1.4/hs_api/_intermediate_format.py`

 * *Files identical despite different names*

### Comparing `hs_api-0.1.3/hs_api/_simple_sim.py` & `hs_api-0.1.4/hs_api/_simple_sim.py`

 * *Files 1% similar despite different names*

```diff
@@ -430,22 +430,25 @@
             initialize_sim_vars()
             self.stepNum == 0
         else:
             #membranePotentials = copy.deepcopy(self.membranePotentials)
             nNeurons = len(self.connections)
             nAxons = len(self.axons)
 
-            if self.perturbMag is not None and self.perturbMag < 17:
+            if self.perturbMag != None:
                 perturbBits = 17
                 perturbation = Fxp(np.random.randint(-1*2**(perturbBits-1),2**(perturbBits-1),size=nNeurons),dtype=self.formatDict['membrane_potential']) #upper is exclusive so no need to subtract one
-                #if self.perturbMag > 0:
-                # breakpoint()
-                if self.perturbMag > 0:
-                    perturbation (perturbation >> self.perturbMag)
-                perturbation (perturbation | Fxp(1, signed=False, n_word=35, n_frac=0))
+                perturbation( perturbation | Fxp(1,dtype='fxp-u35/0') )#set LSB to 1
+                shift = self.perturbMag - (perturbBits - 1)
+                if shift > 0:
+                    perturbation(perturbation << abs(shift))
+                elif shift < 0:
+                    perturbation(perturbation >> abs(shift))
+                else:
+                    pass #do nothing since Fxp doesn't like shifts
                 self.membranePotentials(self.membranePotentials+perturbation)
 
             spiked_inds = np.nonzero(self.membranePotentials() > self.threshold())
             self.membranePotentials[spiked_inds] = 0
             #TODO: you may be able to avoid the transpose if you use fortran ordering flatten
             self.firedNeurons = np.transpose(spiked_inds).flatten().tolist()
```

### Comparing `hs_api-0.1.3/hs_api/api.py` & `hs_api-0.1.4/hs_api/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from hs_api._simple_sim import simple_sim, map_neuron_type_to_int
-
-# from cri_simulations import network
-# from cri_simulations.utils import *
+#from cri_simulations import network
+#from cri_simulations.utils import *
 from connectome_utils.connectome import *
 from bidict import bidict
 import os
 import copy
 import logging
 
 
+class perturbMagError(ValueError):
+    pass
+
+
 class CRI_network:
     """
     This class represents a CRI network which initializes the network, checks hardware, generates connectome,
     formats input, reads and writes synapse, and runs simulation steps.
 
     Attributes
     ----------
@@ -108,15 +111,17 @@
             else:
                 logging.error(
                     "config does not contain neuron type or global neuron params"
                 )
         else:
             logging.error("config should be a dictionary")
 
-        # self.perturb = perturb
+        #self.perturb = perturb
+        if perturbMag > (6) or perturbMag < 0 or not isinstance(perturbMag, int):
+            raise perturbMagError('bad perturbMag')
         self.perturbMag = perturbMag
         if perturbMag:
             if perturbMag > 16:
                 logging.error("perturbMag must be less than 16")
         self.leak = leak
         if leak > 2**6:
             logging.error("Leak must be less than two to the sixth")
@@ -131,22 +136,21 @@
 
         if self.target == "CRI":
             logging.info("Initilizing to run on hardware")
             ##neurons are default to core ID 0, need to be fixed in the connectome to assign correct coreIdx to neurons
             # formatedOutputs = self.connectome.get_core_outputs_idx(coreID)
             formatedOutputs = self.connectome.get_outputs_idx()
             print("formatedOutputs:", formatedOutputs)
-            #breakpoint()
             self.CRI = network(
                 self.connectome,
                 formatedOutputs,
                 self.config,
                 simDump=simDump,
                 leak=self.leak,
-                perturbMag=self.perturbMag,
+                shift=self.perturbMag,
                 coreOveride=coreID,
             )
             self.CRI.initalize_network()
         elif self.target == "simpleSim":
             formatedOutputs = self.connectome.get_outputs_idx()
             self.simpleSim = simple_sim(
                 self.config["global_neuron_params"]["v_thr"],
@@ -559,14 +563,14 @@
                     self.connectome.get_neuron_by_key(symbol).get_coreTypeIdx()
                     for symbol in curInputs
                 ]
             )  # convert symbols to internal indicies
 
         result = self.CRI.run_cont(formated_inputs)
         spikeList = result[0]
-        breakpoint()
+        #breakpoint()
         if self.simDump == False:
             spikeList = [
                 (spike[0], self.connectome.get_neuron_by_idx(spike[1]).get_user_key())
                 for spike in spikeList
             ]
             return (spikeList, result[1], result[2])
```

### Comparing `hs_api-0.1.3/hs_api/converter.py` & `hs_api-0.1.4/hs_api/converter.py`

 * *Files identical despite different names*

### Comparing `hs_api-0.1.3/pyproject.toml` & `hs_api-0.1.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hs_api"
-version = "0.1.3"
+version = "0.1.4"
 description = "CRI User Software"
 authors = ["Justin Frank & Abhinav Uppal"]
 
 [tool.poetry.dependencies]
 
 python = ">=3.10,<3.11"
 numba = "^0.55.1"
@@ -12,16 +12,18 @@
 PyYAML = "^6.0"
 matplotlib = "^3.5.1"
 bidict = "^0.22.0"
 tqdm = "^4.64.1"
 #connectome_utils = {path = "../connectome_utils", develop = true}
 fxpmath = "^0.4.8"
 connectome-utils = "^0.1.0"
-torch = "^2.0.1"
 
 [tool.poetry.dev-dependencies]
 jupyterlab = "^3.3.3"
 hs_bridge = {path = "../hs_bridge", develop = true}
 
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.4.0"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `hs_api-0.1.3/setup.py` & `hs_api-0.1.4/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,27 +11,26 @@
 ['PyYAML>=6.0,<7.0',
  'bidict>=0.22.0,<0.23.0',
  'connectome-utils>=0.1.0,<0.2.0',
  'fxpmath>=0.4.8,<0.5.0',
  'matplotlib>=3.5.1,<4.0.0',
  'numba>=0.55.1,<0.56.0',
  'numpy>=1.18',
- 'torch>=2.0.1,<3.0.0',
  'tqdm>=4.64.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'hs-api',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'CRI User Software',
-    'long_description': None,
+    'long_description': 'None',
     'author': 'Justin Frank & Abhinav Uppal',
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'author_email': 'None',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.10,<3.11',
 }
```

### Comparing `hs_api-0.1.3/PKG-INFO` & `hs_api-0.1.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: hs-api
-Version: 0.1.3
+Version: 0.1.4
 Summary: CRI User Software
 Author: Justin Frank & Abhinav Uppal
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: bidict (>=0.22.0,<0.23.0)
 Requires-Dist: connectome-utils (>=0.1.0,<0.2.0)
 Requires-Dist: fxpmath (>=0.4.8,<0.5.0)
 Requires-Dist: matplotlib (>=3.5.1,<4.0.0)
 Requires-Dist: numba (>=0.55.1,<0.56.0)
 Requires-Dist: numpy (>=1.18)
-Requires-Dist: torch (>=2.0.1,<3.0.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
```

