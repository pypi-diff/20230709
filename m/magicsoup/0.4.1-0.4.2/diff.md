# Comparing `tmp/magicsoup-0.4.1.tar.gz` & `tmp/magicsoup-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magicsoup-0.4.1.tar", last modified: Sun Jul  9 20:47:25 2023, max compression
+gzip compressed data, was "magicsoup-0.4.2.tar", last modified: Sun Jul  9 21:35:45 2023, max compression
```

## Comparing `magicsoup-0.4.1.tar` & `magicsoup-0.4.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-07-09 20:47:25.434118 magicsoup-0.4.1/
--rw-rw-r--   0 marc      (1000) marc      (1003)    34888 2023-01-23 15:27:37.000000 magicsoup-0.4.1/LICENSE
--rw-rw-r--   0 marc      (1000) marc      (1003)     5298 2023-07-09 20:47:25.434118 magicsoup-0.4.1/PKG-INFO
--rw-rw-r--   0 marc      (1000) marc      (1003)     4361 2023-05-29 15:40:09.000000 magicsoup-0.4.1/README.md
--rw-rw-r--   0 marc      (1000) marc      (1003)     1092 2023-01-26 15:22:43.000000 magicsoup-0.4.1/pyproject.toml
--rw-rw-r--   0 marc      (1000) marc      (1003)       38 2023-07-09 20:47:25.434118 magicsoup-0.4.1/setup.cfg
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-07-09 20:47:25.430118 magicsoup-0.4.1/src/
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-07-09 20:47:25.430118 magicsoup-0.4.1/src/magicsoup/
--rw-rw-r--   0 marc      (1000) marc      (1003)      119 2023-07-09 20:47:10.000000 magicsoup-0.4.1/src/magicsoup/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1109 2023-04-27 20:14:44.000000 magicsoup-0.4.1/src/magicsoup/constants.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    25390 2023-06-19 19:49:05.000000 magicsoup-0.4.1/src/magicsoup/containers.py
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-07-09 20:47:25.434118 magicsoup-0.4.1/src/magicsoup/examples/
--rw-rw-r--   0 marc      (1000) marc      (1003)        0 2023-01-23 15:27:37.000000 magicsoup-0.4.1/src/magicsoup/examples/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    13915 2023-07-09 10:27:32.000000 magicsoup-0.4.1/src/magicsoup/examples/co2_fixing.py
--rw-rw-r--   0 marc      (1000) marc      (1003)      833 2023-01-23 15:27:37.000000 magicsoup-0.4.1/src/magicsoup/examples/n2_fixing.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1473 2023-01-23 15:27:37.000000 magicsoup-0.4.1/src/magicsoup/examples/reverse_krebs.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1978 2023-07-09 15:18:23.000000 magicsoup-0.4.1/src/magicsoup/examples/wood_ljungdahl.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    12180 2023-04-27 20:14:54.000000 magicsoup-0.4.1/src/magicsoup/genetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    40215 2023-07-09 19:39:35.000000 magicsoup-0.4.1/src/magicsoup/kinetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     4143 2023-05-01 20:15:52.000000 magicsoup-0.4.1/src/magicsoup/mutations.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     5288 2023-04-07 13:25:00.000000 magicsoup-0.4.1/src/magicsoup/util.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    45270 2023-06-19 19:47:46.000000 magicsoup-0.4.1/src/magicsoup/world.py
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-07-09 20:47:25.434118 magicsoup-0.4.1/src/magicsoup.egg-info/
--rw-rw-r--   0 marc      (1000) marc      (1003)     5298 2023-07-09 20:47:25.000000 magicsoup-0.4.1/src/magicsoup.egg-info/PKG-INFO
--rw-rw-r--   0 marc      (1000) marc      (1003)      775 2023-07-09 20:47:25.000000 magicsoup-0.4.1/src/magicsoup.egg-info/SOURCES.txt
--rw-rw-r--   0 marc      (1000) marc      (1003)        1 2023-07-09 20:47:25.000000 magicsoup-0.4.1/src/magicsoup.egg-info/dependency_links.txt
--rw-rw-r--   0 marc      (1000) marc      (1003)       10 2023-07-09 20:47:25.000000 magicsoup-0.4.1/src/magicsoup.egg-info/top_level.txt
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-07-09 20:47:25.434118 magicsoup-0.4.1/tests/
--rw-rw-r--   0 marc      (1000) marc      (1003)      960 2023-07-09 20:44:20.000000 magicsoup-0.4.1/tests/test_containers.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     5984 2023-07-09 20:43:48.000000 magicsoup-0.4.1/tests/test_genetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    45367 2023-07-09 20:43:00.000000 magicsoup-0.4.1/tests/test_kinetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     5142 2023-07-09 20:37:44.000000 magicsoup-0.4.1/tests/test_kinetics_integration.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1041 2023-05-01 20:29:24.000000 magicsoup-0.4.1/tests/test_mutations.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1433 2023-07-09 20:28:00.000000 magicsoup-0.4.1/tests/test_util.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    22786 2023-07-09 10:21:14.000000 magicsoup-0.4.1/tests/test_world.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     2971 2023-07-09 20:31:45.000000 magicsoup-0.4.1/tests/test_world_integration.py
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-07-09 21:35:45.300153 magicsoup-0.4.2/
+-rw-rw-r--   0 marc      (1000) marc      (1003)    34888 2023-01-23 15:27:37.000000 magicsoup-0.4.2/LICENSE
+-rw-rw-r--   0 marc      (1000) marc      (1003)     5298 2023-07-09 21:35:45.300153 magicsoup-0.4.2/PKG-INFO
+-rw-rw-r--   0 marc      (1000) marc      (1003)     4361 2023-05-29 15:40:09.000000 magicsoup-0.4.2/README.md
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1092 2023-01-26 15:22:43.000000 magicsoup-0.4.2/pyproject.toml
+-rw-rw-r--   0 marc      (1000) marc      (1003)       38 2023-07-09 21:35:45.300153 magicsoup-0.4.2/setup.cfg
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-07-09 21:35:45.296153 magicsoup-0.4.2/src/
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-07-09 21:35:45.296153 magicsoup-0.4.2/src/magicsoup/
+-rw-rw-r--   0 marc      (1000) marc      (1003)      119 2023-07-09 21:35:34.000000 magicsoup-0.4.2/src/magicsoup/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1109 2023-04-27 20:14:44.000000 magicsoup-0.4.2/src/magicsoup/constants.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    25390 2023-06-19 19:49:05.000000 magicsoup-0.4.2/src/magicsoup/containers.py
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-07-09 21:35:45.300153 magicsoup-0.4.2/src/magicsoup/examples/
+-rw-rw-r--   0 marc      (1000) marc      (1003)        0 2023-01-23 15:27:37.000000 magicsoup-0.4.2/src/magicsoup/examples/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    13915 2023-07-09 10:27:32.000000 magicsoup-0.4.2/src/magicsoup/examples/co2_fixing.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)      833 2023-01-23 15:27:37.000000 magicsoup-0.4.2/src/magicsoup/examples/n2_fixing.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1473 2023-01-23 15:27:37.000000 magicsoup-0.4.2/src/magicsoup/examples/reverse_krebs.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1978 2023-07-09 15:18:23.000000 magicsoup-0.4.2/src/magicsoup/examples/wood_ljungdahl.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    12180 2023-04-27 20:14:54.000000 magicsoup-0.4.2/src/magicsoup/genetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    40933 2023-07-09 21:34:46.000000 magicsoup-0.4.2/src/magicsoup/kinetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     4143 2023-05-01 20:15:52.000000 magicsoup-0.4.2/src/magicsoup/mutations.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     5288 2023-04-07 13:25:00.000000 magicsoup-0.4.2/src/magicsoup/util.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    45270 2023-06-19 19:47:46.000000 magicsoup-0.4.2/src/magicsoup/world.py
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-07-09 21:35:45.296153 magicsoup-0.4.2/src/magicsoup.egg-info/
+-rw-rw-r--   0 marc      (1000) marc      (1003)     5298 2023-07-09 21:35:45.000000 magicsoup-0.4.2/src/magicsoup.egg-info/PKG-INFO
+-rw-rw-r--   0 marc      (1000) marc      (1003)      775 2023-07-09 21:35:45.000000 magicsoup-0.4.2/src/magicsoup.egg-info/SOURCES.txt
+-rw-rw-r--   0 marc      (1000) marc      (1003)        1 2023-07-09 21:35:45.000000 magicsoup-0.4.2/src/magicsoup.egg-info/dependency_links.txt
+-rw-rw-r--   0 marc      (1000) marc      (1003)       10 2023-07-09 21:35:45.000000 magicsoup-0.4.2/src/magicsoup.egg-info/top_level.txt
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-07-09 21:35:45.300153 magicsoup-0.4.2/tests/
+-rw-rw-r--   0 marc      (1000) marc      (1003)      960 2023-07-09 20:44:20.000000 magicsoup-0.4.2/tests/test_containers.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     5984 2023-07-09 20:43:48.000000 magicsoup-0.4.2/tests/test_genetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    45367 2023-07-09 20:43:00.000000 magicsoup-0.4.2/tests/test_kinetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     4961 2023-07-09 21:24:24.000000 magicsoup-0.4.2/tests/test_kinetics_integration.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1041 2023-05-01 20:29:24.000000 magicsoup-0.4.2/tests/test_mutations.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1433 2023-07-09 20:28:00.000000 magicsoup-0.4.2/tests/test_util.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    22786 2023-07-09 10:21:14.000000 magicsoup-0.4.2/tests/test_world.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     2971 2023-07-09 21:29:47.000000 magicsoup-0.4.2/tests/test_world_integration.py
```

### Comparing `magicsoup-0.4.1/LICENSE` & `magicsoup-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.1/PKG-INFO` & `magicsoup-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magicsoup
-Version: 0.4.1
+Version: 0.4.2
 Summary: Simulation for cell metabolic and transduction pathway evolution
 Author-email: Marc <schweringmarc01@gmail.com>
 Project-URL: Documentation, https://magic-soup.readthedocs.io/
 Project-URL: Homepage, https://github.com/mRcSchwering/magic-soup
 Project-URL: Bug Tracker, https://github.com/mRcSchwering/magic-soup/issues
 Classifier: Environment :: Console
 Classifier: Environment :: GPU
```

### Comparing `magicsoup-0.4.1/README.md` & `magicsoup-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.1/pyproject.toml` & `magicsoup-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.1/src/magicsoup/constants.py` & `magicsoup-0.4.2/src/magicsoup/constants.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.1/src/magicsoup/containers.py` & `magicsoup-0.4.2/src/magicsoup/containers.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.1/src/magicsoup/examples/co2_fixing.py` & `magicsoup-0.4.2/src/magicsoup/examples/co2_fixing.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.1/src/magicsoup/examples/n2_fixing.py` & `magicsoup-0.4.2/src/magicsoup/examples/n2_fixing.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.1/src/magicsoup/examples/reverse_krebs.py` & `magicsoup-0.4.2/src/magicsoup/examples/reverse_krebs.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.1/src/magicsoup/examples/wood_ljungdahl.py` & `magicsoup-0.4.2/src/magicsoup/examples/wood_ljungdahl.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.1/src/magicsoup/genetics.py` & `magicsoup-0.4.2/src/magicsoup/genetics.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.1/src/magicsoup/kinetics.py` & `magicsoup-0.4.2/src/magicsoup/kinetics.py`

 * *Files 0% similar despite different names*

```diff
@@ -702,14 +702,25 @@
             mb = X + Xd < 0.0
             trim_to_zero = torch.where(ma & mb, X / -Xd - _EPS, 1.0).amin(1)  # (c,)
             Xd = torch.einsum("cs,c->cs", Xd, trim_to_zero)
 
             # update signals, this time no negative X
             X = X + Xd
 
+            # The above should make it impossible to create negative X
+            # However in some simulations I see negative values, they usually
+            # create extremely high values within 1 or 2 steps (cell molecule concentrations)
+            # I was not able to reproduce this in any of the tests
+            # TODO: luca/e1_co2_fixing has this problem but it can be avoided
+            #       by clamping after every computation
+            # it seems that clamping here does not create molecules from nothing
+            # my hypothesis is that the negative value was a floating point error
+            # and so clamping does not necessarily create molecules from nothing
+            X = X.clamp(0.0)
+
         # NaNs can be created when overflow creates Infs (most likely in aggregate_signals)
         # with kinetics default values I have not been able to achieve this (>100 testruns)
         # however non-default values (e.g. large Vmax) might achieve that
         # once a 1 NaN is generated, it will spread over the whole simulation
         # this is a last effort in avoiding that
         X[X.isnan()] = 0.0
```

### Comparing `magicsoup-0.4.1/src/magicsoup/mutations.py` & `magicsoup-0.4.2/src/magicsoup/mutations.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.1/src/magicsoup/util.py` & `magicsoup-0.4.2/src/magicsoup/util.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.1/src/magicsoup/world.py` & `magicsoup-0.4.2/src/magicsoup/world.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.1/src/magicsoup.egg-info/PKG-INFO` & `magicsoup-0.4.2/src/magicsoup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magicsoup
-Version: 0.4.1
+Version: 0.4.2
 Summary: Simulation for cell metabolic and transduction pathway evolution
 Author-email: Marc <schweringmarc01@gmail.com>
 Project-URL: Documentation, https://magic-soup.readthedocs.io/
 Project-URL: Homepage, https://github.com/mRcSchwering/magic-soup
 Project-URL: Bug Tracker, https://github.com/mRcSchwering/magic-soup/issues
 Classifier: Environment :: Console
 Classifier: Environment :: GPU
```

### Comparing `magicsoup-0.4.1/src/magicsoup.egg-info/SOURCES.txt` & `magicsoup-0.4.2/src/magicsoup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.1/tests/test_containers.py` & `magicsoup-0.4.2/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.1/tests/test_genetics.py` & `magicsoup-0.4.2/tests/test_genetics.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.1/tests/test_kinetics.py` & `magicsoup-0.4.2/tests/test_kinetics.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.1/tests/test_kinetics_integration.py` & `magicsoup-0.4.2/tests/test_kinetics_integration.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,25 @@
 import pytest
 import torch
-from magicsoup.containers import Molecule
-from magicsoup.kinetics import Kinetics
+import magicsoup as ms
+from magicsoup.examples.wood_ljungdahl import MOLECULES, REACTIONS
 
 # mark all tests in this module as slow
 pytestmark = pytest.mark.slow
 
 
-_ma = Molecule("a", energy=15 * 1e3)
-_mb = Molecule("b", energy=10 * 1e3)
-_mc = Molecule("c", energy=10 * 1e3)
-_md = Molecule("d", energy=5 * 1e3)
-_MOLECULES = [_ma, _mb, _mc, _md]
-
-_r_a_b = ([_ma], [_mb])
-_r_b_c = ([_mb], [_mc])
-_r_bc_d = ([_mb, _mc], [_md])
-_r_d_bb = ([_md], [_mb, _mb])
-_REACTIONS = [_r_a_b, _r_b_c, _r_bc_d, _r_d_bb]
-
-
-def _get_kinetics(n_computations=1) -> Kinetics:
-    kinetics = Kinetics(
-        molecules=_MOLECULES,
-        reactions=_REACTIONS,
+def _get_kinetics(n_computations=1) -> ms.Kinetics:
+    chemistry = ms.Chemistry(molecules=MOLECULES, reactions=REACTIONS)
+    kinetics = ms.Kinetics(
+        molecules=chemistry.molecules,
+        reactions=chemistry.reactions,
         n_computations=n_computations,
         abs_temp=310,
+        scalar_enc_size=61,
+        vector_enc_size=3904,
     )
     return kinetics
 
 
 def test_equilibrium_is_reached():
     # molecules should reach equilibrium after a few steps
     # with Vmax > 1.0 higher order reactions cant reach equilibrium
@@ -107,21 +97,21 @@
     # 1. when using exp(ln(x)) 1s can accidentally be created
     # 2. when doing a^b 1s can be created (0^1=0 but 0^0=1)
     n_cells = 100
     n_prots = 100
     n_steps = 1000
 
     kinetics = _get_kinetics()
-    n_mols = len(_MOLECULES) * 2
+    n_mols = len(MOLECULES) * 2
 
     # concentrations (c, s)
     X = torch.zeros(n_cells, n_mols).abs()
 
     # reactions (c, p, s)
-    kinetics.N = torch.randint(low=-5, high=6, size=(n_cells, n_prots, n_mols)).float()
+    kinetics.N = torch.randint(low=-8, high=9, size=(n_cells, n_prots, n_mols)).float()
     kinetics.Nf = torch.where(kinetics.N < 0.0, -kinetics.N, 0.0)
     kinetics.Nb = torch.where(kinetics.N > 0.0, kinetics.N, 0.0)
 
     # max velocities (c, p)
     kinetics.Vmax = torch.randn(n_cells, n_prots).abs() * 100
 
     # allosterics (c, p, s)
@@ -145,21 +135,21 @@
     # i.g. exponents too high and many substrates
     # this will create infinites which will eventually become NaN
     n_cells = 100
     n_prots = 100
     n_steps = 1000
 
     kinetics = _get_kinetics()
-    n_mols = len(_MOLECULES) * 2
+    n_mols = len(MOLECULES) * 2
 
     # concentrations (c, s)
     X = torch.randn(n_cells, n_mols).abs().clamp(max=1.0) * 100
 
     # reactions (c, p, s)
-    kinetics.N = torch.randint(low=-5, high=6, size=(n_cells, n_prots, n_mols)).float()
+    kinetics.N = torch.randint(low=-8, high=9, size=(n_cells, n_prots, n_mols)).float()
     kinetics.Nf = torch.where(kinetics.N < 0.0, -kinetics.N, 0.0)
     kinetics.Nb = torch.where(kinetics.N > 0.0, kinetics.N, 0.0)
 
     # max velocities (c, p)
     kinetics.Vmax = torch.randn(n_cells, n_prots).abs().clamp(max=1.0) * 100
 
     # allosterics (c, p, s)
```

### Comparing `magicsoup-0.4.1/tests/test_mutations.py` & `magicsoup-0.4.2/tests/test_mutations.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.1/tests/test_util.py` & `magicsoup-0.4.2/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.1/tests/test_world.py` & `magicsoup-0.4.2/tests/test_world.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.1/tests/test_world_integration.py` & `magicsoup-0.4.2/tests/test_world_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,13 +72,13 @@
         world.diffuse_molecules()
         world.enzymatic_activity()
 
         molmap = world.molecule_map
         cellmols = world.cell_molecules
 
         assert molmap.min() >= 0.0, i
-        assert 0.0 < molmap.mean() < 30.0, i
+        assert 0.0 < molmap.mean() < 50.0, i
         assert molmap.max() < 500.0, i
 
         assert cellmols.min() >= 0.0, i
-        assert 0.0 < cellmols.mean() < 30.0, i
+        assert 0.0 < cellmols.mean() < 50.0, i
         assert cellmols.max() < 500.0, i
```

