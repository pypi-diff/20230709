# Comparing `tmp/magicsoup-0.4.0.tar.gz` & `tmp/magicsoup-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magicsoup-0.4.0.tar", last modified: Thu Jun  8 20:20:10 2023, max compression
+gzip compressed data, was "magicsoup-0.4.1.tar", last modified: Sun Jul  9 20:47:25 2023, max compression
```

## Comparing `magicsoup-0.4.0.tar` & `magicsoup-0.4.1.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-06-08 20:20:10.332495 magicsoup-0.4.0/
--rw-rw-r--   0 marc      (1000) marc      (1003)    34888 2023-01-23 15:27:37.000000 magicsoup-0.4.0/LICENSE
--rw-rw-r--   0 marc      (1000) marc      (1003)     5298 2023-06-08 20:20:10.332495 magicsoup-0.4.0/PKG-INFO
--rw-rw-r--   0 marc      (1000) marc      (1003)     4361 2023-05-29 15:40:09.000000 magicsoup-0.4.0/README.md
--rw-rw-r--   0 marc      (1000) marc      (1003)     1092 2023-01-26 15:22:43.000000 magicsoup-0.4.0/pyproject.toml
--rw-rw-r--   0 marc      (1000) marc      (1003)       38 2023-06-08 20:20:10.332495 magicsoup-0.4.0/setup.cfg
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-06-08 20:20:10.332495 magicsoup-0.4.0/src/
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-06-08 20:20:10.332495 magicsoup-0.4.0/src/magicsoup/
--rw-rw-r--   0 marc      (1000) marc      (1003)      119 2023-06-08 20:19:57.000000 magicsoup-0.4.0/src/magicsoup/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1109 2023-04-27 20:14:44.000000 magicsoup-0.4.0/src/magicsoup/constants.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    25381 2023-06-08 20:05:48.000000 magicsoup-0.4.0/src/magicsoup/containers.py
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-06-08 20:20:10.332495 magicsoup-0.4.0/src/magicsoup/examples/
--rw-rw-r--   0 marc      (1000) marc      (1003)        0 2023-01-23 15:27:37.000000 magicsoup-0.4.0/src/magicsoup/examples/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1003)      833 2023-01-23 15:27:37.000000 magicsoup-0.4.0/src/magicsoup/examples/n2_fixing.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1473 2023-01-23 15:27:37.000000 magicsoup-0.4.0/src/magicsoup/examples/reverse_krebs.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1930 2023-02-16 21:19:27.000000 magicsoup-0.4.0/src/magicsoup/examples/wood_ljungdahl.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    12180 2023-04-27 20:14:54.000000 magicsoup-0.4.0/src/magicsoup/genetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    40436 2023-06-08 19:43:19.000000 magicsoup-0.4.0/src/magicsoup/kinetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     4143 2023-05-01 20:15:52.000000 magicsoup-0.4.0/src/magicsoup/mutations.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     5288 2023-04-07 13:25:00.000000 magicsoup-0.4.0/src/magicsoup/util.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    45267 2023-05-29 15:43:01.000000 magicsoup-0.4.0/src/magicsoup/world.py
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-06-08 20:20:10.332495 magicsoup-0.4.0/src/magicsoup.egg-info/
--rw-rw-r--   0 marc      (1000) marc      (1003)     5298 2023-06-08 20:20:10.000000 magicsoup-0.4.0/src/magicsoup.egg-info/PKG-INFO
--rw-rw-r--   0 marc      (1000) marc      (1003)      671 2023-06-08 20:20:10.000000 magicsoup-0.4.0/src/magicsoup.egg-info/SOURCES.txt
--rw-rw-r--   0 marc      (1000) marc      (1003)        1 2023-06-08 20:20:10.000000 magicsoup-0.4.0/src/magicsoup.egg-info/dependency_links.txt
--rw-rw-r--   0 marc      (1000) marc      (1003)       10 2023-06-08 20:20:10.000000 magicsoup-0.4.0/src/magicsoup.egg-info/top_level.txt
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-06-08 20:20:10.332495 magicsoup-0.4.0/tests/
--rw-rw-r--   0 marc      (1000) marc      (1003)      950 2023-05-29 15:58:52.000000 magicsoup-0.4.0/tests/test_containers.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     6012 2023-04-06 09:44:07.000000 magicsoup-0.4.0/tests/test_genetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    49435 2023-06-06 21:41:32.000000 magicsoup-0.4.0/tests/test_kinetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1041 2023-05-01 20:29:24.000000 magicsoup-0.4.0/tests/test_mutations.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1433 2023-04-03 15:10:20.000000 magicsoup-0.4.0/tests/test_util.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    24597 2023-06-08 18:10:34.000000 magicsoup-0.4.0/tests/test_world.py
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-07-09 20:47:25.434118 magicsoup-0.4.1/
+-rw-rw-r--   0 marc      (1000) marc      (1003)    34888 2023-01-23 15:27:37.000000 magicsoup-0.4.1/LICENSE
+-rw-rw-r--   0 marc      (1000) marc      (1003)     5298 2023-07-09 20:47:25.434118 magicsoup-0.4.1/PKG-INFO
+-rw-rw-r--   0 marc      (1000) marc      (1003)     4361 2023-05-29 15:40:09.000000 magicsoup-0.4.1/README.md
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1092 2023-01-26 15:22:43.000000 magicsoup-0.4.1/pyproject.toml
+-rw-rw-r--   0 marc      (1000) marc      (1003)       38 2023-07-09 20:47:25.434118 magicsoup-0.4.1/setup.cfg
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-07-09 20:47:25.430118 magicsoup-0.4.1/src/
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-07-09 20:47:25.430118 magicsoup-0.4.1/src/magicsoup/
+-rw-rw-r--   0 marc      (1000) marc      (1003)      119 2023-07-09 20:47:10.000000 magicsoup-0.4.1/src/magicsoup/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1109 2023-04-27 20:14:44.000000 magicsoup-0.4.1/src/magicsoup/constants.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    25390 2023-06-19 19:49:05.000000 magicsoup-0.4.1/src/magicsoup/containers.py
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-07-09 20:47:25.434118 magicsoup-0.4.1/src/magicsoup/examples/
+-rw-rw-r--   0 marc      (1000) marc      (1003)        0 2023-01-23 15:27:37.000000 magicsoup-0.4.1/src/magicsoup/examples/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    13915 2023-07-09 10:27:32.000000 magicsoup-0.4.1/src/magicsoup/examples/co2_fixing.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)      833 2023-01-23 15:27:37.000000 magicsoup-0.4.1/src/magicsoup/examples/n2_fixing.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1473 2023-01-23 15:27:37.000000 magicsoup-0.4.1/src/magicsoup/examples/reverse_krebs.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1978 2023-07-09 15:18:23.000000 magicsoup-0.4.1/src/magicsoup/examples/wood_ljungdahl.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    12180 2023-04-27 20:14:54.000000 magicsoup-0.4.1/src/magicsoup/genetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    40215 2023-07-09 19:39:35.000000 magicsoup-0.4.1/src/magicsoup/kinetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     4143 2023-05-01 20:15:52.000000 magicsoup-0.4.1/src/magicsoup/mutations.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     5288 2023-04-07 13:25:00.000000 magicsoup-0.4.1/src/magicsoup/util.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    45270 2023-06-19 19:47:46.000000 magicsoup-0.4.1/src/magicsoup/world.py
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-07-09 20:47:25.434118 magicsoup-0.4.1/src/magicsoup.egg-info/
+-rw-rw-r--   0 marc      (1000) marc      (1003)     5298 2023-07-09 20:47:25.000000 magicsoup-0.4.1/src/magicsoup.egg-info/PKG-INFO
+-rw-rw-r--   0 marc      (1000) marc      (1003)      775 2023-07-09 20:47:25.000000 magicsoup-0.4.1/src/magicsoup.egg-info/SOURCES.txt
+-rw-rw-r--   0 marc      (1000) marc      (1003)        1 2023-07-09 20:47:25.000000 magicsoup-0.4.1/src/magicsoup.egg-info/dependency_links.txt
+-rw-rw-r--   0 marc      (1000) marc      (1003)       10 2023-07-09 20:47:25.000000 magicsoup-0.4.1/src/magicsoup.egg-info/top_level.txt
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-07-09 20:47:25.434118 magicsoup-0.4.1/tests/
+-rw-rw-r--   0 marc      (1000) marc      (1003)      960 2023-07-09 20:44:20.000000 magicsoup-0.4.1/tests/test_containers.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     5984 2023-07-09 20:43:48.000000 magicsoup-0.4.1/tests/test_genetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    45367 2023-07-09 20:43:00.000000 magicsoup-0.4.1/tests/test_kinetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     5142 2023-07-09 20:37:44.000000 magicsoup-0.4.1/tests/test_kinetics_integration.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1041 2023-05-01 20:29:24.000000 magicsoup-0.4.1/tests/test_mutations.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1433 2023-07-09 20:28:00.000000 magicsoup-0.4.1/tests/test_util.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    22786 2023-07-09 10:21:14.000000 magicsoup-0.4.1/tests/test_world.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     2971 2023-07-09 20:31:45.000000 magicsoup-0.4.1/tests/test_world_integration.py
```

### Comparing `magicsoup-0.4.0/LICENSE` & `magicsoup-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.0/PKG-INFO` & `magicsoup-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magicsoup
-Version: 0.4.0
+Version: 0.4.1
 Summary: Simulation for cell metabolic and transduction pathway evolution
 Author-email: Marc <schweringmarc01@gmail.com>
 Project-URL: Documentation, https://magic-soup.readthedocs.io/
 Project-URL: Homepage, https://github.com/mRcSchwering/magic-soup
 Project-URL: Bug Tracker, https://github.com/mRcSchwering/magic-soup/issues
 Classifier: Environment :: Console
 Classifier: Environment :: GPU
```

### Comparing `magicsoup-0.4.0/README.md` & `magicsoup-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.0/pyproject.toml` & `magicsoup-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.0/src/magicsoup/constants.py` & `magicsoup-0.4.1/src/magicsoup/constants.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.0/src/magicsoup/containers.py` & `magicsoup-0.4.1/src/magicsoup/containers.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     ```
         atp = Molecule("ATP", 10)
         atp2 = Molecule("ATP", 10)
         assert atp is atp2
     ```
 
     This is used later on in the simulation to make efficient comparisons.
-    It also allows you to define overlapping chemistries without creating multiple molecule instances of the same molecule species.
+    Additionally, it allows you to define overlapping chemistries without creating multiple molecule instances of the same molecule species.
 
     However, this also means that if 2 molecules have the same name, other attributes like e.g. energy must also match:
 
     ```
         atp = Molecule("ATP", 10)
         Molecule("ATP", 20)  # raises error
     ```
```

### Comparing `magicsoup-0.4.0/src/magicsoup/examples/n2_fixing.py` & `magicsoup-0.4.1/src/magicsoup/examples/n2_fixing.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.0/src/magicsoup/examples/reverse_krebs.py` & `magicsoup-0.4.1/src/magicsoup/examples/reverse_krebs.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.0/src/magicsoup/examples/wood_ljungdahl.py` & `magicsoup-0.4.1/src/magicsoup/examples/wood_ljungdahl.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,16 +46,16 @@
     NiACS,
     methylNiACS,
     HSCoA,
     acetylCoA,
 ]
 
 REACTIONS = [
-    ([co2, NADPH], [formiat, NADP]),
-    ([formiat, FH4, ATP], [formylFH4, ADP]),
-    ([formylFH4, NADPH], [methylenFH4, NADP]),
-    ([methylenFH4, NADPH], [methylFH4, NADP]),
-    ([methylFH4, NiACS], [FH4, methylNiACS]),
-    ([methylNiACS, co2, HSCoA], [NiACS, acetylCoA]),
+    ([co2, NADPH], [formiat, NADP]),  # -90k
+    ([formiat, FH4, ATP], [formylFH4, ADP]),  # -10k
+    ([formylFH4, NADPH], [methylenFH4, NADP]),  # -40k
+    ([methylenFH4, NADPH], [methylFH4, NADP]),  # -40k
+    ([methylFH4, NiACS], [FH4, methylNiACS]),  # -60k
+    ([methylNiACS, co2, HSCoA], [NiACS, acetylCoA]),  # -50k
 ]
 
 CHEMISTRY = Chemistry(molecules=MOLECULES, reactions=REACTIONS)
```

### Comparing `magicsoup-0.4.0/src/magicsoup/genetics.py` & `magicsoup-0.4.1/src/magicsoup/genetics.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.0/src/magicsoup/kinetics.py` & `magicsoup-0.4.1/src/magicsoup/kinetics.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Protein,
     CatalyticDomain,
     TransporterDomain,
     RegulatoryDomain,
     DomainType,
 )
 
-_EPS = 1e-8
+_EPS = 1e-7
 _MIN = 1e-45
 _MAX = 1e38
 
 
 class _LogNormWeightMapFact:
     """
     Creates an object that maps tokens to a float
@@ -655,18 +655,15 @@
             kf = xxf / self.Kmf
             kf[~f_prots] = 0.0  # rm artifacts created by ln
 
             xxb, b_prots = self._aggregate_signals(X=X, mask=is_bwd, N=self.Nb)
             kb = xxb / self.Kmb
             kb[~b_prots] = 0.0  # rm artifacts created by ln
 
-            # the correct formula yields 2 * (ks - kp) / (1 + ks + kp)
-            # but then there can be a maximum activity of 200%
-            # while regulatory regions can only go up to 100%
-            # thus (ks - kp) / (1 + ks + kp)
+            # custom reversible MM equation
             a_cat = (kf - kb) / (1 + kf + kb)  # (c, p)
 
             # NaNs could have been propagated so far by stray NaN Kms
             # they should represent 0 velocity
             a_cat = a_cat.nan_to_num(0.0)
 
             # inhibitor activity
@@ -683,34 +680,35 @@
             # as well as trimming factor of n_computations
             V = Vmax_adj * a_cat * (1 - a_inh) * a_act * self.alpha**i  # (c, p)
 
             # Kms can be close to Inf, they can create Infs
             # thus result velocity should be clamped again
             V = V.clamp(max=_MAX)
 
-            # naive Xd
+            # naive Xd, might produce negative X
             Xd = torch.einsum("cps,cp->cs", self.N, V)  # (c, s)
 
             # proteins can deconstruct more of a molecule than available in a cell
             # but I can't just clip X at 0 because then reactions would not adhere
             # to their stoichiometry anymore
             # instead I need to reduce protein velocity
             # However, a cell's Xd is the sum of all its protein's activities
             # if I reduce the velocity of 1 protein, it could create a new
             # below-zero situation for another one
             # One would have to repeat this action until all conflicts are satisfied
             # Here, I am instead reducing all the cell's proteins by the same factor
             # that way these secondary below-zero situations cannot appear
-            trim_to_zero = torch.where(X + Xd < 0.0, (X - _EPS) / -Xd, 1.0)  # (c, s)
-            Xd = torch.einsum("cs,c->cs", Xd, trim_to_zero.amin(1))
+            # due to floating point precision I need to lift the cutoff from 0 to EPS
+            ma = Xd < 0.0
+            mb = X + Xd < 0.0
+            trim_to_zero = torch.where(ma & mb, X / -Xd - _EPS, 1.0).amin(1)  # (c,)
+            Xd = torch.einsum("cs,c->cs", Xd, trim_to_zero)
 
-            # should not be necessary but floating point precision
-            # can still create very small negative values (<1e-7)
-            # these are so small that they should not matter in the overall simulation
-            X = (X + Xd).clamp(min=0.0)
+            # update signals, this time no negative X
+            X = X + Xd
 
         # NaNs can be created when overflow creates Infs (most likely in aggregate_signals)
         # with kinetics default values I have not been able to achieve this (>100 testruns)
         # however non-default values (e.g. large Vmax) might achieve that
         # once a 1 NaN is generated, it will spread over the whole simulation
         # this is a last effort in avoiding that
         X[X.isnan()] = 0.0
```

### Comparing `magicsoup-0.4.0/src/magicsoup/mutations.py` & `magicsoup-0.4.1/src/magicsoup/mutations.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.0/src/magicsoup/util.py` & `magicsoup-0.4.1/src/magicsoup/util.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.0/src/magicsoup/world.py` & `magicsoup-0.4.1/src/magicsoup/world.py`

 * *Files identical despite different names*

```diff
@@ -69,22 +69,22 @@
         genomes: A list of cell genomes. Each cell's index in this list is what is referred to as the cell index.
             The cell index is used for the same cell in other orderings of cells (_e.g._ `labels`, `cell_divisions`, `cell_molecules`).
         labels: List of cell labels. Cells are ordered as in `world.genomes`. Labels are strings that can be used to
             track cell origins. When adding new cells (`world.add_cells()`) a random label is assigned to each cell.
             If a cell divides, its descendants will have the same label.
         cell_map: Boolean 2D tensor referencing which pixels are occupied by a cell.
             Dimension 0 represents the x, dimension 1 y.
-        molecule_map: Float 3D tensor describing how many molecules (in mol) of each molecule species exist on every pixel in this world.
+        molecule_map: Float 3D tensor describing how many molecules (in mmol) of each molecule species exist on every pixel in this world.
             Dimension 0 describes the molecule species. They are in the same order as `chemistry.molecules`.
             Dimension 1 represents x, dimension 2 y.
             So, `world.molecule_map[0, 1, 2]` is number of molecules of the 0th molecule species on pixel 1, 2.
-        cell_molecules: Float 2D tensor describing the number of molecules (in mol) for each molecule species in each cell.
+        cell_molecules: Float 2D tensor describing the number of molecules (in mmol) for each molecule species in each cell.
             Dimension 0 is the cell index. It is the same as in `world.genomes` and the same as on a cell object (`cell.idx`).
             Dimension 1 describes the molecule species. They are in the same order as `chemistry.molecules`.
-            So, `world.cell_molecules[0, 1]` represents how many mol of the 1st molecule species the 0th cell contains.
+            So, `world.cell_molecules[0, 1]` represents how many mmol of the 1st molecule species the 0th cell contains.
         cell_lifetimes: Integer 1D tensor describing how many time steps each cell survived since the last division.
             This tensor is for monitoring and doesn't have any other effect.
             Cells are in the same as in `world.genomes` and the same as on a cell object (`cell.idx`).
         cell_divisions: Integer 1D tensor describing how many times each cell's ancestors divided.
             This tensor is for monitoring and doesn't have any other effect.
             Cells are in the same order as in `world.genomes` and the same as on a cell object (`cell.idx`).
```

### Comparing `magicsoup-0.4.0/src/magicsoup.egg-info/PKG-INFO` & `magicsoup-0.4.1/src/magicsoup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magicsoup
-Version: 0.4.0
+Version: 0.4.1
 Summary: Simulation for cell metabolic and transduction pathway evolution
 Author-email: Marc <schweringmarc01@gmail.com>
 Project-URL: Documentation, https://magic-soup.readthedocs.io/
 Project-URL: Homepage, https://github.com/mRcSchwering/magic-soup
 Project-URL: Bug Tracker, https://github.com/mRcSchwering/magic-soup/issues
 Classifier: Environment :: Console
 Classifier: Environment :: GPU
```

### Comparing `magicsoup-0.4.0/src/magicsoup.egg-info/SOURCES.txt` & `magicsoup-0.4.1/src/magicsoup.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,19 @@
 src/magicsoup/util.py
 src/magicsoup/world.py
 src/magicsoup.egg-info/PKG-INFO
 src/magicsoup.egg-info/SOURCES.txt
 src/magicsoup.egg-info/dependency_links.txt
 src/magicsoup.egg-info/top_level.txt
 src/magicsoup/examples/__init__.py
+src/magicsoup/examples/co2_fixing.py
 src/magicsoup/examples/n2_fixing.py
 src/magicsoup/examples/reverse_krebs.py
 src/magicsoup/examples/wood_ljungdahl.py
 tests/test_containers.py
 tests/test_genetics.py
 tests/test_kinetics.py
+tests/test_kinetics_integration.py
 tests/test_mutations.py
 tests/test_util.py
-tests/test_world.py
+tests/test_world.py
+tests/test_world_integration.py
```

### Comparing `magicsoup-0.4.0/tests/test_containers.py` & `magicsoup-0.4.1/tests/test_containers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import warnings
 import pytest
 import magicsoup.containers as cntnrs
 
-X = cntnrs.Molecule(name="X", energy=10)
-Y = cntnrs.Molecule(name="Y", energy=100)
+_X = cntnrs.Molecule(name="X", energy=10)
+_Y = cntnrs.Molecule(name="Y", energy=100)
 
 
 def test_same_molecules_get_same_instance():
     X2 = cntnrs.Molecule(name="X", energy=10)
     Y2 = cntnrs.Molecule(name="Y", energy=100)
-    assert X is X2
-    assert Y is Y2
-    assert Y is not X
+    assert _X is X2
+    assert _Y is Y2
+    assert _Y is not _X
 
 
 def test_raise_if_same_molecule_with_different_energy():
     with pytest.raises(ValueError):
         cntnrs.Molecule(name="X", energy=20)
 
 
@@ -23,12 +23,12 @@
     with warnings.catch_warnings(record=True) as warn:
         cntnrs.Molecule(name="x", energy=10)
     assert len(warn) > 0
     assert issubclass(warn[-1].category, UserWarning)
 
 
 def test_molecule_mappings():
-    chem = cntnrs.Chemistry(molecules=[X, Y], reactions=[])
-    assert chem.mol_2_idx[X] == 0
-    assert chem.mol_2_idx[Y] == 1
+    chem = cntnrs.Chemistry(molecules=[_X, _Y], reactions=[])
+    assert chem.mol_2_idx[_X] == 0
+    assert chem.mol_2_idx[_Y] == 1
     assert chem.molname_2_idx["X"] == 0
     assert chem.molname_2_idx["Y"] == 1
```

### Comparing `magicsoup-0.4.0/tests/test_genetics.py` & `magicsoup-0.4.1/tests/test_genetics.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from magicsoup.constants import CODON_SIZE
 
 
 # (genome, cds)
 # starts: "TTG", "GTG", "ATG"
 # stops: "TGA", "TAG", "TAA"
 # forward only
-DATA = [
+_DATA = [
     (
         """
         TACCGGATA GCAGCTTTT CTTGGAATA GCCAAGGGT
         CGCCTTTAT ACCTATCTA CAACTACTA CTCGGTTGG
         TAACAAAGG TTAAAACGC CAAACGAGT ATCGGCCAA
         TCCTGTCAC TGTGAGAAG TTTCAATTA TAGATTCCT
         GGGGCGATT GGCGATGGT
@@ -42,15 +42,15 @@
             "TTGTGCGGCGCTATACACCCCTGCAGTTATTTAAGGGCTTAG",
             "GTGCGGCGCTATACACCCCTGCAGTTATTTAAGGGCTTAGGCGAGAAGTTCCGCCTGCTAAGGAGTCCCTGTTGGGTGAAGTAA",
         ],
     ),
 ]
 
 
-@pytest.mark.parametrize("seq, exp", DATA)
+@pytest.mark.parametrize("seq, exp", _DATA)
 def test_get_coding_regions(seq: str, exp: list[str]):
     # 1 codon is too small to express p=0.01 domain types
     with pytest.warns(UserWarning):
         genetics = ms.Genetics(n_dom_type_codons=1)
 
     kwargs = {
         "start_codons": genetics.start_codons,
@@ -102,53 +102,50 @@
     assert res[0][0] == (1, 2, 5, 1, 3)
     assert res[1][0] == (2, 3, 4, 2, 3)
     assert res[2][0] == (1, 3, 4, 5, 2)
     assert res[3][0] == (3, 3, 4, 2, 3)
     assert res[3][1] == (2, 1, 2, 3, 4)
 
 
-
 def test_genetics():
     # 1=catalytic, 2=transporter, 3=regulatory
     # regulatory-only proteins get sorted out, so there is a bias towards
     # fewer regulatory domains
 
     # all same likelihood (while considering reg bias)
     kwargs = {"p_catal_dom": 0.1, "p_transp_dom": 0.1, "p_reg_dom": 0.1}
     genetics = ms.Genetics(**kwargs)
     genomes = [ms.random_genome(s=500) for _ in range(1000)]
     proteomes = genetics.translate_genomes(genomes=genomes)
-    
+
     n_catal = sum(ddd[0] == 1 for d in proteomes for dd in d for ddd in dd)
     n_trnsp = sum(ddd[0] == 2 for d in proteomes for dd in d for ddd in dd)
     n_reg = sum(ddd[0] == 3 for d in proteomes for dd in d for ddd in dd)
     n = n_catal + n_trnsp + n_reg
     assert abs(n_catal - n_trnsp) < 0.1 * n
     assert abs(n_trnsp - n_reg) < 0.2 * n
 
     # fewer catalytics (while considering reg bias)
     kwargs["p_catal_dom"] = 0.01
     genetics = ms.Genetics(**kwargs)
     genomes = [ms.random_genome(s=500) for _ in range(1000)]
     proteomes = genetics.translate_genomes(genomes=genomes)
-    
+
     n_catal = sum(ddd[0] == 1 for d in proteomes for dd in d for ddd in dd)
     n_trnsp = sum(ddd[0] == 2 for d in proteomes for dd in d for ddd in dd)
     n_reg = sum(ddd[0] == 3 for d in proteomes for dd in d for ddd in dd)
     n = n_catal + n_trnsp + n_reg
     assert n_trnsp - n_catal > 0.9 * n / 3
     assert n_reg - n_catal > 0.6 * n / 3
 
     # also fewer transporters (while considering reg bias)
     kwargs["p_transp_dom"] = 0.01
     genetics = ms.Genetics(**kwargs)
     genomes = [ms.random_genome(s=500) for _ in range(1000)]
     proteomes = genetics.translate_genomes(genomes=genomes)
-    
+
     n_catal = sum(ddd[0] == 1 for d in proteomes for dd in d for ddd in dd)
     n_trnsp = sum(ddd[0] == 2 for d in proteomes for dd in d for ddd in dd)
     n_reg = sum(ddd[0] == 3 for d in proteomes for dd in d for ddd in dd)
     n = n_catal + n_trnsp + n_reg
     assert n_reg - n_catal > 0.6 * n / 3
     assert n_reg - n_trnsp > 0.6 * n / 3
-
-
```

### Comparing `magicsoup-0.4.0/tests/test_kinetics.py` & `magicsoup-0.4.1/tests/test_kinetics.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,105 +6,105 @@
     CatalyticDomain,
     RegulatoryDomain,
     TransporterDomain,
 )
 from magicsoup.constants import GAS_CONSTANT
 from magicsoup.kinetics import Kinetics
 
-TOLERANCE = 1e-4
-EPS = 1e-8
+_TOLERANCE = 1e-4
+_EPS = 1e-8
 
 
-ma = Molecule("a", energy=15 * 1e3)
-mb = Molecule("b", energy=10 * 1e3)
-mc = Molecule("c", energy=10 * 1e3)
-md = Molecule("d", energy=5 * 1e3)
-MOLECULES = [ma, mb, mc, md]
-
-r_a_b = ([ma], [mb])
-r_b_c = ([mb], [mc])
-r_bc_d = ([mb, mc], [md])
-r_d_bb = ([md], [mb, mb])
-REACTIONS = [r_a_b, r_b_c, r_bc_d, r_d_bb]
+_ma = Molecule("a", energy=15 * 1e3)
+_mb = Molecule("b", energy=10 * 1e3)
+_mc = Molecule("c", energy=10 * 1e3)
+_md = Molecule("d", energy=5 * 1e3)
+_MOLECULES = [_ma, _mb, _mc, _md]
+
+_r_a_b = ([_ma], [_mb])
+_r_b_c = ([_mb], [_mc])
+_r_bc_d = ([_mb, _mc], [_md])
+_r_d_bb = ([_md], [_mb, _mb])
+_REACTIONS = [_r_a_b, _r_b_c, _r_bc_d, _r_d_bb]
 
 # fmt: off
-KM_WEIGHTS = torch.tensor([
+_KM_WEIGHTS = torch.tensor([
     torch.nan, 0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9,  # idxs 0-9
     1.0, 1.1, 1.2, 1.3, 1.4, 1.5, 1.6, 1.7, 1.8, 1.9,  # idxs 10-19
     2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, 2.9  # idxs 20-29
 ])
 
-VMAX_WEIGHTS = torch.tensor([
+_VMAX_WEIGHTS = torch.tensor([
     torch.nan, 1.1, 1.2, 1.3, 1.4, 1.5, 1.6, 1.7, 1.8, 1.9,  # idxs 0-9
     2.0, 2.1, 2.2, 2.3, 2.4, 2.5, 2.6, 2.7, 2.8, 2.9,  # idxs 10-19
 ])
 
-SIGNS = torch.tensor([0.0, 1.0, -1.0])  # idxs 0-2
+_SIGNS = torch.tensor([0.0, 1.0, -1.0])  # idxs 0-2
 
-TRANSPORT_M = torch.tensor([
+_TRANSPORT_M = torch.tensor([
     [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],  # idx 0: none
     [-1.0, 0.0, 0.0, 0.0, 1.0, 0.0, 0.0, 0.0], # idx 1: a in->out
     [0.0, -1.0, 0.0, 0.0, 0.0, 1.0, 0.0, 0.0], # idx 2: b in->out
     [0.0, 0.0, -1.0, 0.0, 0.0, 0.0, 1.0, 0.0], # idx 3: c in->out
     [0.0, 0.0, 0.0, -1.0, 0.0, 0.0, 0.0, 1.0], # idx 4: d in->out
     [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
     [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
     [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
     [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
 ])
 
-EFFECTOR_M = torch.tensor([
+_EFFECTOR_M = torch.tensor([
     [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0], # idx 0: none
     [1.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0], # idx 1: a in
     [0.0, 1.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0], # idx 2: b in
     [0.0, 0.0, 1.0, 0.0, 0.0, 0.0, 0.0, 0.0], # idx 3: c in
     [0.0, 0.0, 0.0, 1.0, 0.0, 0.0, 0.0, 0.0], # idx 4: d in
     [0.0, 0.0, 0.0, 0.0, 1.0, 0.0, 0.0, 0.0], # idx 5: a out
     [0.0, 0.0, 0.0, 0.0, 0.0, 1.0, 0.0, 0.0], # idx 6: b out
     [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 1.0, 0.0], # idx 7: c out
     [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 1.0], # idx 8: d out
 ])
 
-REACTION_M = torch.tensor([
+_REACTION_M = torch.tensor([
     [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],   # idx 0: none
     [-1.0, 1.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],  # idx 1: a -> b
     [0.0, -1.0, 1.0, 0.0, 0.0, 0.0, 0.0, 0.0],  # idx 2: b -> c
     [0.0, -1.0, -1.0, 1.0, 0.0, 0.0, 0.0, 0.0], # idx 3: b,c -> d
     [0.0, 2.0, 0.0, -1.0, 0.0, 0.0, 0.0, 0.0],  # idx 4: d -> 2b
     [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
     [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
     [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
     [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
 ])
 
 # fmt: on
 
 
-def get_kinetics(n_computations=1) -> Kinetics:
+def _get_kinetics(n_computations=1) -> Kinetics:
     kinetics = Kinetics(
-        molecules=MOLECULES,
-        reactions=REACTIONS,
+        molecules=_MOLECULES,
+        reactions=_REACTIONS,
         n_computations=n_computations,
         abs_temp=310,
     )
-    kinetics.km_map.weights = KM_WEIGHTS.clone()
-    kinetics.vmax_map.weights = VMAX_WEIGHTS.clone()
-    kinetics.sign_map.signs = SIGNS.clone()
-    kinetics.transport_map.M = TRANSPORT_M.clone()
-    kinetics.effector_map.M = EFFECTOR_M.clone()
-    kinetics.reaction_map.M = REACTION_M.clone()
+    kinetics.km_map.weights = _KM_WEIGHTS.clone()
+    kinetics.vmax_map.weights = _VMAX_WEIGHTS.clone()
+    kinetics.sign_map.signs = _SIGNS.clone()
+    kinetics.transport_map.M = _TRANSPORT_M.clone()
+    kinetics.effector_map.M = _EFFECTOR_M.clone()
+    kinetics.reaction_map.M = _REACTION_M.clone()
     return kinetics
 
 
-def ke(subs: list[Molecule], prods: list[Molecule]):
+def _ke(subs: list[Molecule], prods: list[Molecule]):
     e = sum(d.energy for d in prods) - sum(d.energy for d in subs)
     return math.exp(-e / 310 / GAS_CONSTANT)
 
 
-def avg(*x):
+def _avg(*x):
     return sum(x) / len(x)
 
 
 def test_cell_params_with_transporter_domains():
     # Domain spec indexes: (dom_types, reacts_trnspts_effctrs, Vmaxs, Kms, signs)
     # fmt: off
     c0 = [
@@ -136,48 +136,48 @@
     Vmax = torch.zeros(2, 3)
     N = torch.zeros(2, 3, 8)
     Nf = torch.zeros(2, 3, 8)
     Nb = torch.zeros(2, 3, 8)
     A = torch.zeros(2, 3, 8)
 
     # test
-    kinetics = get_kinetics()
+    kinetics = _get_kinetics()
     kinetics.Kmf = Kmf
     kinetics.Kmb = Kmb
     kinetics.Kmr = Kmr
     kinetics.Vmax = Vmax
     kinetics.N = N
     kinetics.Nf = Nf
     kinetics.Nb = Nb
     kinetics.A = A
     kinetics.set_cell_params(cell_idxs=[0, 1], proteomes=[c0, c1])
 
-    assert Kmf[0, 0] == pytest.approx(0.5, abs=TOLERANCE)
-    assert Kmb[0, 0] == pytest.approx(0.5, abs=TOLERANCE)
-    assert Kmf[0, 1] == pytest.approx(avg(0.5, 0.2), abs=TOLERANCE)
-    assert Kmb[0, 1] == pytest.approx(avg(0.5, 0.2), abs=TOLERANCE)
-    assert Kmf[0, 2] == pytest.approx(0.0, TOLERANCE)
-    assert Kmb[0, 2] == pytest.approx(0.0, TOLERANCE)
-
-    ke_c1_1 = ke([ma], [mb])
-    assert Kmf[1, 0] == pytest.approx(avg(0.4, 0.5, 0.6, 0.7), abs=TOLERANCE)
-    assert Kmb[1, 0] == pytest.approx(avg(0.4, 0.5, 0.6, 0.7), abs=TOLERANCE)
-    assert Kmf[1, 1] == pytest.approx(avg(0.5, 0.5), abs=TOLERANCE)
-    assert Kmb[1, 1] == pytest.approx(avg(0.5, 0.5) * ke_c1_1, abs=TOLERANCE)
-    assert Kmf[1, 2] == pytest.approx(0.0, TOLERANCE)
-    assert Kmb[1, 2] == pytest.approx(0.0, TOLERANCE)
+    assert Kmf[0, 0] == pytest.approx(0.5, abs=_TOLERANCE)
+    assert Kmb[0, 0] == pytest.approx(0.5, abs=_TOLERANCE)
+    assert Kmf[0, 1] == pytest.approx(_avg(0.5, 0.2), abs=_TOLERANCE)
+    assert Kmb[0, 1] == pytest.approx(_avg(0.5, 0.2), abs=_TOLERANCE)
+    assert Kmf[0, 2] == pytest.approx(0.0, _TOLERANCE)
+    assert Kmb[0, 2] == pytest.approx(0.0, _TOLERANCE)
+
+    ke_c1_1 = _ke([_ma], [_mb])
+    assert Kmf[1, 0] == pytest.approx(_avg(0.4, 0.5, 0.6, 0.7), abs=_TOLERANCE)
+    assert Kmb[1, 0] == pytest.approx(_avg(0.4, 0.5, 0.6, 0.7), abs=_TOLERANCE)
+    assert Kmf[1, 1] == pytest.approx(_avg(0.5, 0.5), abs=_TOLERANCE)
+    assert Kmb[1, 1] == pytest.approx(_avg(0.5, 0.5) * ke_c1_1, abs=_TOLERANCE)
+    assert Kmf[1, 2] == pytest.approx(0.0, _TOLERANCE)
+    assert Kmb[1, 2] == pytest.approx(0.0, _TOLERANCE)
 
-    assert (Kmr < TOLERANCE).all()
+    assert (Kmr < _TOLERANCE).all()
 
-    assert Vmax[0, 0] == pytest.approx(1.5, abs=TOLERANCE)
-    assert Vmax[0, 1] == pytest.approx(avg(1.5, 1.1), abs=TOLERANCE)
+    assert Vmax[0, 0] == pytest.approx(1.5, abs=_TOLERANCE)
+    assert Vmax[0, 1] == pytest.approx(_avg(1.5, 1.1), abs=_TOLERANCE)
     assert Vmax[0, 2] == 0.0
 
-    assert Vmax[1, 0] == pytest.approx(avg(1.5, 1.4, 1.3, 1.2), abs=TOLERANCE)
-    assert Vmax[1, 1] == pytest.approx(avg(2.0, 1.5), abs=TOLERANCE)
+    assert Vmax[1, 0] == pytest.approx(_avg(1.5, 1.4, 1.3, 1.2), abs=_TOLERANCE)
+    assert Vmax[1, 1] == pytest.approx(_avg(2.0, 1.5), abs=_TOLERANCE)
     assert Vmax[1, 2] == 0.0
 
     assert N[0, 0, 0] == -1
     assert N[0, 0, 4] == 1
     assert (N[0, 0, [1, 2, 3, 5, 6, 7]] == 0).all()
     assert Nf[0, 0, 0] == 1
     assert (Nf[0, 0, [1, 2, 3, 4, 5, 6, 7]] == 0).all()
@@ -213,58 +213,58 @@
 
     # test proteome representation
 
     proteins = kinetics.get_proteome(proteome=c0)
 
     p0 = proteins[0]
     assert isinstance(p0.domains[0], TransporterDomain)
-    assert p0.domains[0].molecule is ma
-    assert p0.domains[0].vmax == pytest.approx(1.5, abs=TOLERANCE)
-    assert p0.domains[0].km == pytest.approx(0.5, abs=TOLERANCE)
+    assert p0.domains[0].molecule is _ma
+    assert p0.domains[0].vmax == pytest.approx(1.5, abs=_TOLERANCE)
+    assert p0.domains[0].km == pytest.approx(0.5, abs=_TOLERANCE)
 
     p1 = proteins[1]
     assert isinstance(p1.domains[0], TransporterDomain)
-    assert p1.domains[0].molecule is ma
-    assert p1.domains[0].vmax == pytest.approx(1.5, abs=TOLERANCE)
-    assert p1.domains[0].km == pytest.approx(0.5, abs=TOLERANCE)
+    assert p1.domains[0].molecule is _ma
+    assert p1.domains[0].vmax == pytest.approx(1.5, abs=_TOLERANCE)
+    assert p1.domains[0].km == pytest.approx(0.5, abs=_TOLERANCE)
     assert isinstance(p1.domains[1], TransporterDomain)
-    assert p1.domains[1].molecule is ma
-    assert p1.domains[1].vmax == pytest.approx(1.1, abs=TOLERANCE)
-    assert p1.domains[1].km == pytest.approx(0.2, abs=TOLERANCE)
+    assert p1.domains[1].molecule is _ma
+    assert p1.domains[1].vmax == pytest.approx(1.1, abs=_TOLERANCE)
+    assert p1.domains[1].km == pytest.approx(0.2, abs=_TOLERANCE)
 
     proteins = kinetics.get_proteome(proteome=c1)
 
     p0 = proteins[0]
     assert isinstance(p0.domains[0], TransporterDomain)
-    assert p0.domains[0].molecule is ma
-    assert p0.domains[0].vmax == pytest.approx(1.5, abs=TOLERANCE)
-    assert p0.domains[0].km == pytest.approx(0.4, abs=TOLERANCE)
+    assert p0.domains[0].molecule is _ma
+    assert p0.domains[0].vmax == pytest.approx(1.5, abs=_TOLERANCE)
+    assert p0.domains[0].km == pytest.approx(0.4, abs=_TOLERANCE)
     assert isinstance(p0.domains[1], TransporterDomain)
-    assert p0.domains[1].molecule is ma
-    assert p0.domains[1].vmax == pytest.approx(1.4, abs=TOLERANCE)
-    assert p0.domains[1].km == pytest.approx(0.5, abs=TOLERANCE)
+    assert p0.domains[1].molecule is _ma
+    assert p0.domains[1].vmax == pytest.approx(1.4, abs=_TOLERANCE)
+    assert p0.domains[1].km == pytest.approx(0.5, abs=_TOLERANCE)
     assert isinstance(p0.domains[2], TransporterDomain)
-    assert p0.domains[2].molecule is mb
-    assert p0.domains[2].vmax == pytest.approx(1.3, abs=TOLERANCE)
-    assert p0.domains[2].km == pytest.approx(0.6, abs=TOLERANCE)
+    assert p0.domains[2].molecule is _mb
+    assert p0.domains[2].vmax == pytest.approx(1.3, abs=_TOLERANCE)
+    assert p0.domains[2].km == pytest.approx(0.6, abs=_TOLERANCE)
     assert isinstance(p0.domains[3], TransporterDomain)
-    assert p0.domains[3].molecule is mc
-    assert p0.domains[3].vmax == pytest.approx(1.2, abs=TOLERANCE)
-    assert p0.domains[3].km == pytest.approx(0.7, abs=TOLERANCE)
+    assert p0.domains[3].molecule is _mc
+    assert p0.domains[3].vmax == pytest.approx(1.2, abs=_TOLERANCE)
+    assert p0.domains[3].km == pytest.approx(0.7, abs=_TOLERANCE)
 
     p1 = proteins[1]
     assert isinstance(p1.domains[0], CatalyticDomain)
-    assert p1.domains[0].substrates == [ma]
-    assert p1.domains[0].products == [mb]
-    assert p1.domains[0].vmax == pytest.approx(2.0, abs=TOLERANCE)
-    assert p1.domains[0].km == pytest.approx(0.5, abs=TOLERANCE)
+    assert p1.domains[0].substrates == [_ma]
+    assert p1.domains[0].products == [_mb]
+    assert p1.domains[0].vmax == pytest.approx(2.0, abs=_TOLERANCE)
+    assert p1.domains[0].km == pytest.approx(0.5, abs=_TOLERANCE)
     assert isinstance(p1.domains[1], TransporterDomain)
-    assert p1.domains[1].molecule is ma
-    assert p1.domains[1].vmax == pytest.approx(1.5, abs=TOLERANCE)
-    assert p1.domains[1].km == pytest.approx(0.5, abs=TOLERANCE)
+    assert p1.domains[1].molecule is _ma
+    assert p1.domains[1].vmax == pytest.approx(1.5, abs=_TOLERANCE)
+    assert p1.domains[1].km == pytest.approx(0.5, abs=_TOLERANCE)
 
 
 def test_cell_params_with_regulatory_domains():
     # Domain spec indexes: (dom_types, reacts_trnspts_effctrs, Vmaxs, Kms, signs)
     # fmt: off
     c0 = [
         [
@@ -299,50 +299,50 @@
     Vmax = torch.zeros(2, 3)
     N = torch.zeros(2, 3, 8)
     Nf = torch.zeros(2, 3, 8)
     Nb = torch.zeros(2, 3, 8)
     A = torch.zeros(2, 3, 8)
 
     # test
-    kinetics = get_kinetics()
+    kinetics = _get_kinetics()
     kinetics.Kmf = Kmf
     kinetics.Kmb = Kmb
     kinetics.Kmr = Kmr
     kinetics.Vmax = Vmax
     kinetics.N = N
     kinetics.Nf = Nf
     kinetics.Nb = Nb
     kinetics.A = A
     kinetics.set_cell_params(cell_idxs=[0, 1], proteomes=[c0, c1])
 
-    ke_c0_0 = ke([ma], [mb])
-    ke_c0_1 = ke([ma], [mb])
-    assert Kmf[0, 0] == pytest.approx(0.5, abs=TOLERANCE)
-    assert Kmb[0, 0] == pytest.approx(0.5 * ke_c0_0, abs=TOLERANCE)
-    assert Kmr[0, 0] == pytest.approx(avg(1.0, 2.0), abs=TOLERANCE)
-    assert Kmf[0, 1] == pytest.approx(0.5, abs=TOLERANCE)
-    assert Kmb[0, 1] == pytest.approx(0.5 * ke_c0_1, abs=TOLERANCE)
-    assert Kmr[0, 1] == pytest.approx(avg(1.0, 1.5), abs=TOLERANCE)
-    assert Kmf[0, 2] == pytest.approx(0.0, TOLERANCE)
-    assert Kmb[0, 2] == pytest.approx(0.0, TOLERANCE)
-    assert Kmr[0, 2] == pytest.approx(0.0, TOLERANCE)
-
-    assert Kmf[1, 0] == pytest.approx(0.5, abs=TOLERANCE)
-    assert Kmb[1, 0] == pytest.approx(0.5 * ke_c0_0, abs=TOLERANCE)
-    assert Kmf[1, 1] == pytest.approx(0.5, abs=TOLERANCE)
-    assert Kmb[1, 1] == pytest.approx(0.5 * ke_c0_1, abs=TOLERANCE)
-    assert Kmf[1, 2] == pytest.approx(0.0, TOLERANCE)
-    assert Kmb[1, 2] == pytest.approx(0.0, TOLERANCE)
+    ke_c0_0 = _ke([_ma], [_mb])
+    ke_c0_1 = _ke([_ma], [_mb])
+    assert Kmf[0, 0] == pytest.approx(0.5, abs=_TOLERANCE)
+    assert Kmb[0, 0] == pytest.approx(0.5 * ke_c0_0, abs=_TOLERANCE)
+    assert Kmr[0, 0] == pytest.approx(_avg(1.0, 2.0), abs=_TOLERANCE)
+    assert Kmf[0, 1] == pytest.approx(0.5, abs=_TOLERANCE)
+    assert Kmb[0, 1] == pytest.approx(0.5 * ke_c0_1, abs=_TOLERANCE)
+    assert Kmr[0, 1] == pytest.approx(_avg(1.0, 1.5), abs=_TOLERANCE)
+    assert Kmf[0, 2] == pytest.approx(0.0, _TOLERANCE)
+    assert Kmb[0, 2] == pytest.approx(0.0, _TOLERANCE)
+    assert Kmr[0, 2] == pytest.approx(0.0, _TOLERANCE)
+
+    assert Kmf[1, 0] == pytest.approx(0.5, abs=_TOLERANCE)
+    assert Kmb[1, 0] == pytest.approx(0.5 * ke_c0_0, abs=_TOLERANCE)
+    assert Kmf[1, 1] == pytest.approx(0.5, abs=_TOLERANCE)
+    assert Kmb[1, 1] == pytest.approx(0.5 * ke_c0_1, abs=_TOLERANCE)
+    assert Kmf[1, 2] == pytest.approx(0.0, _TOLERANCE)
+    assert Kmb[1, 2] == pytest.approx(0.0, _TOLERANCE)
 
-    assert Vmax[0, 0] == pytest.approx(2.0, abs=TOLERANCE)
-    assert Vmax[0, 1] == pytest.approx(2.0, abs=TOLERANCE)
+    assert Vmax[0, 0] == pytest.approx(2.0, abs=_TOLERANCE)
+    assert Vmax[0, 1] == pytest.approx(2.0, abs=_TOLERANCE)
     assert Vmax[0, 2] == 0.0
 
-    assert Vmax[1, 0] == pytest.approx(2.0, abs=TOLERANCE)
-    assert Vmax[1, 1] == pytest.approx(2.0, abs=TOLERANCE)
+    assert Vmax[1, 0] == pytest.approx(2.0, abs=_TOLERANCE)
+    assert Vmax[1, 1] == pytest.approx(2.0, abs=_TOLERANCE)
     assert Vmax[1, 2] == 0.0
 
     assert N[0, 0, 0] == -1
     assert N[0, 0, 1] == 1
     assert (N[0, 0, [2, 3, 4, 5, 6]] == 0).all()
     assert Nf[0, 0, 0] == 1
     assert (Nf[0, 0, [1, 2, 3, 4, 5, 6]] == 0).all()
@@ -395,81 +395,81 @@
 
     # test protein representation
 
     proteins = kinetics.get_proteome(proteome=c0)
 
     p0 = proteins[0]
     assert isinstance(p0.domains[0], CatalyticDomain)
-    assert p0.domains[0].substrates == [ma]
-    assert p0.domains[0].products == [mb]
-    assert p0.domains[0].vmax == pytest.approx(2.0, abs=TOLERANCE)
-    assert p0.domains[0].km == pytest.approx(0.5, abs=TOLERANCE)
+    assert p0.domains[0].substrates == [_ma]
+    assert p0.domains[0].products == [_mb]
+    assert p0.domains[0].vmax == pytest.approx(2.0, abs=_TOLERANCE)
+    assert p0.domains[0].km == pytest.approx(0.5, abs=_TOLERANCE)
     assert isinstance(p0.domains[1], RegulatoryDomain)
-    assert p0.domains[1].effector is mc
+    assert p0.domains[1].effector is _mc
     assert not p0.domains[1].is_inhibiting
     assert not p0.domains[1].is_transmembrane
-    assert p0.domains[1].km == pytest.approx(1.0, abs=TOLERANCE)
+    assert p0.domains[1].km == pytest.approx(1.0, abs=_TOLERANCE)
     assert isinstance(p0.domains[2], RegulatoryDomain)
-    assert p0.domains[2].effector is md
+    assert p0.domains[2].effector is _md
     assert p0.domains[2].is_inhibiting
     assert not p0.domains[2].is_transmembrane
-    assert p0.domains[2].km == pytest.approx(2.0, abs=TOLERANCE)
+    assert p0.domains[2].km == pytest.approx(2.0, abs=_TOLERANCE)
 
     p1 = proteins[1]
     assert isinstance(p1.domains[0], CatalyticDomain)
-    assert p1.domains[0].substrates == [ma]
-    assert p1.domains[0].products == [mb]
-    assert p1.domains[0].vmax == pytest.approx(2.0, abs=TOLERANCE)
-    assert p1.domains[0].km == pytest.approx(0.5, abs=TOLERANCE)
+    assert p1.domains[0].substrates == [_ma]
+    assert p1.domains[0].products == [_mb]
+    assert p1.domains[0].vmax == pytest.approx(2.0, abs=_TOLERANCE)
+    assert p1.domains[0].km == pytest.approx(0.5, abs=_TOLERANCE)
     assert isinstance(p1.domains[1], RegulatoryDomain)
-    assert p1.domains[1].effector is ma
+    assert p1.domains[1].effector is _ma
     assert not p1.domains[1].is_inhibiting
     assert not p1.domains[1].is_transmembrane
-    assert p1.domains[1].km == pytest.approx(1.0, abs=TOLERANCE)
+    assert p1.domains[1].km == pytest.approx(1.0, abs=_TOLERANCE)
     assert isinstance(p1.domains[2], RegulatoryDomain)
-    assert p1.domains[2].effector is ma
+    assert p1.domains[2].effector is _ma
     assert not p1.domains[2].is_inhibiting
     assert p1.domains[2].is_transmembrane
-    assert p1.domains[2].km == pytest.approx(1.5, abs=TOLERANCE)
+    assert p1.domains[2].km == pytest.approx(1.5, abs=_TOLERANCE)
 
     proteins = kinetics.get_proteome(proteome=c1)
 
     p0 = proteins[0]
     assert isinstance(p0.domains[0], CatalyticDomain)
-    assert p0.domains[0].substrates == [ma]
-    assert p0.domains[0].products == [mb]
-    assert p0.domains[0].vmax == pytest.approx(2.0, abs=TOLERANCE)
-    assert p0.domains[0].km == pytest.approx(0.5, abs=TOLERANCE)
+    assert p0.domains[0].substrates == [_ma]
+    assert p0.domains[0].products == [_mb]
+    assert p0.domains[0].vmax == pytest.approx(2.0, abs=_TOLERANCE)
+    assert p0.domains[0].km == pytest.approx(0.5, abs=_TOLERANCE)
     assert isinstance(p0.domains[1], RegulatoryDomain)
-    assert p0.domains[1].effector is mb
+    assert p0.domains[1].effector is _mb
     assert p0.domains[1].is_inhibiting
     assert not p0.domains[1].is_transmembrane
-    assert p0.domains[1].km == pytest.approx(1.0, abs=TOLERANCE)
+    assert p0.domains[1].km == pytest.approx(1.0, abs=_TOLERANCE)
     assert isinstance(p0.domains[2], RegulatoryDomain)
-    assert p0.domains[2].effector is mb
+    assert p0.domains[2].effector is _mb
     assert p0.domains[2].is_inhibiting
     assert p0.domains[2].is_transmembrane
-    assert p0.domains[2].km == pytest.approx(1.5, abs=TOLERANCE)
+    assert p0.domains[2].km == pytest.approx(1.5, abs=_TOLERANCE)
 
     p1 = proteins[1]
     assert isinstance(p1.domains[0], CatalyticDomain)
-    assert p1.domains[0].substrates == [ma]
-    assert p1.domains[0].products == [mb]
-    assert p1.domains[0].vmax == pytest.approx(2.0, abs=TOLERANCE)
-    assert p1.domains[0].km == pytest.approx(0.5, abs=TOLERANCE)
+    assert p1.domains[0].substrates == [_ma]
+    assert p1.domains[0].products == [_mb]
+    assert p1.domains[0].vmax == pytest.approx(2.0, abs=_TOLERANCE)
+    assert p1.domains[0].km == pytest.approx(0.5, abs=_TOLERANCE)
     assert isinstance(p1.domains[1], RegulatoryDomain)
-    assert p1.domains[1].effector is md
+    assert p1.domains[1].effector is _md
     assert not p1.domains[1].is_inhibiting
     assert not p1.domains[1].is_transmembrane
-    assert p1.domains[1].km == pytest.approx(1.0, abs=TOLERANCE)
+    assert p1.domains[1].km == pytest.approx(1.0, abs=_TOLERANCE)
     assert isinstance(p1.domains[2], RegulatoryDomain)
-    assert p1.domains[2].effector is md
+    assert p1.domains[2].effector is _md
     assert not p1.domains[2].is_inhibiting
     assert not p1.domains[2].is_transmembrane
-    assert p1.domains[2].km == pytest.approx(1.5, abs=TOLERANCE)
+    assert p1.domains[2].km == pytest.approx(1.5, abs=_TOLERANCE)
 
 
 def test_cell_params_with_catalytic_domains():
     # Domain spec indexes: (dom_types, reacts_trnspts_effctrs, Vmaxs, Kms, signs)
     # fmt: off
     c0 = [
         [
@@ -503,52 +503,52 @@
     Vmax = torch.zeros(2, 3)
     N = torch.zeros(2, 3, 8)
     Nf = torch.zeros(2, 3, 8)
     Nb = torch.zeros(2, 3, 8)
     A = torch.zeros(2, 3, 8)
 
     # test
-    kinetics = get_kinetics()
+    kinetics = _get_kinetics()
     kinetics.Kmf = Kmf
     kinetics.Kmb = Kmb
     kinetics.Kmr = Kmr
     kinetics.Vmax = Vmax
     kinetics.N = N
     kinetics.Nf = Nf
     kinetics.Nb = Nb
     kinetics.A = A
     kinetics.set_cell_params(cell_idxs=[0, 1], proteomes=[c0, c1])
 
-    ke_c0_0 = ke([ma, md], [mb, mb, mc])
-    ke_c0_1 = ke([mb, md], [mc, mb, mc])
-    ke_c0_2 = ke([md], [mb, mb])
-    assert Kmf[0, 0] == pytest.approx(avg(0.5, 1.5) / ke_c0_0, abs=TOLERANCE)
-    assert Kmb[0, 0] == pytest.approx(avg(0.5, 1.5), abs=TOLERANCE)
-    assert Kmf[0, 1] == pytest.approx(avg(0.9, 1.2) / ke_c0_1, abs=TOLERANCE)
-    assert Kmb[0, 1] == pytest.approx(avg(0.9, 1.2), abs=TOLERANCE)
-    assert Kmf[0, 2] == pytest.approx(2.9 / ke_c0_2, abs=TOLERANCE)
-    assert Kmb[0, 2] == pytest.approx(2.9, abs=TOLERANCE)
-
-    ke_c1_0 = ke([mb, md], [ma, mb, mc])
-    ke_c1_1 = ke([mb, mb, mc], [mc, md])
-    assert Kmf[1, 0] == pytest.approx(avg(0.3, 1.4) / ke_c1_0, TOLERANCE)
-    assert Kmb[1, 0] == pytest.approx(avg(0.3, 1.4), TOLERANCE)
-    assert Kmf[1, 1] == pytest.approx(avg(0.3, 1.7), TOLERANCE)
-    assert Kmb[1, 1] == pytest.approx(avg(0.3, 1.7) * ke_c1_1, TOLERANCE)
-    assert Kmf[1, 2] == pytest.approx(0.0, TOLERANCE)
-    assert Kmb[1, 2] == pytest.approx(0.0, TOLERANCE)
-
-    assert (Kmr < TOLERANCE).all()
-
-    assert Vmax[0, 0] == pytest.approx(avg(1.1, 1.2), abs=TOLERANCE)
-    assert Vmax[0, 1] == pytest.approx(avg(2.0, 1.3), abs=TOLERANCE)
-    assert Vmax[0, 2] == pytest.approx(2.9, abs=TOLERANCE)
+    ke_c0_0 = _ke([_ma, _md], [_mb, _mb, _mc])
+    ke_c0_1 = _ke([_mb, _md], [_mc, _mb, _mc])
+    ke_c0_2 = _ke([_md], [_mb, _mb])
+    assert Kmf[0, 0] == pytest.approx(_avg(0.5, 1.5) / ke_c0_0, abs=_TOLERANCE)
+    assert Kmb[0, 0] == pytest.approx(_avg(0.5, 1.5), abs=_TOLERANCE)
+    assert Kmf[0, 1] == pytest.approx(_avg(0.9, 1.2) / ke_c0_1, abs=_TOLERANCE)
+    assert Kmb[0, 1] == pytest.approx(_avg(0.9, 1.2), abs=_TOLERANCE)
+    assert Kmf[0, 2] == pytest.approx(2.9 / ke_c0_2, abs=_TOLERANCE)
+    assert Kmb[0, 2] == pytest.approx(2.9, abs=_TOLERANCE)
+
+    ke_c1_0 = _ke([_mb, _md], [_ma, _mb, _mc])
+    ke_c1_1 = _ke([_mb, _mb, _mc], [_mc, _md])
+    assert Kmf[1, 0] == pytest.approx(_avg(0.3, 1.4) / ke_c1_0, _TOLERANCE)
+    assert Kmb[1, 0] == pytest.approx(_avg(0.3, 1.4), _TOLERANCE)
+    assert Kmf[1, 1] == pytest.approx(_avg(0.3, 1.7), _TOLERANCE)
+    assert Kmb[1, 1] == pytest.approx(_avg(0.3, 1.7) * ke_c1_1, _TOLERANCE)
+    assert Kmf[1, 2] == pytest.approx(0.0, _TOLERANCE)
+    assert Kmb[1, 2] == pytest.approx(0.0, _TOLERANCE)
+
+    assert (Kmr < _TOLERANCE).all()
+
+    assert Vmax[0, 0] == pytest.approx(_avg(1.1, 1.2), abs=_TOLERANCE)
+    assert Vmax[0, 1] == pytest.approx(_avg(2.0, 1.3), abs=_TOLERANCE)
+    assert Vmax[0, 2] == pytest.approx(2.9, abs=_TOLERANCE)
 
-    assert Vmax[1, 0] == pytest.approx(avg(1.1, 2.1), abs=TOLERANCE)
-    assert Vmax[1, 1] == pytest.approx(avg(1.9, 2.3), abs=TOLERANCE)
+    assert Vmax[1, 0] == pytest.approx(_avg(1.1, 2.1), abs=_TOLERANCE)
+    assert Vmax[1, 1] == pytest.approx(_avg(1.9, 2.3), abs=_TOLERANCE)
     assert Vmax[1, 2] == 0.0
 
     assert N[0, 0, 0] == -1
     assert N[0, 0, 1] == 2
     assert N[0, 0, 2] == 1
     assert N[0, 0, 3] == -1
     assert (N[0, 0, [4, 5, 6, 7]] == 0).all()
@@ -608,68 +608,68 @@
 
     # test protein representation
 
     proteins = kinetics.get_proteome(proteome=c0)
 
     p0 = proteins[0]
     assert isinstance(p0.domains[0], CatalyticDomain)
-    assert p0.domains[0].substrates == [ma]
-    assert p0.domains[0].products == [mb]
-    assert p0.domains[0].vmax == pytest.approx(1.1, abs=TOLERANCE)
-    assert p0.domains[0].km == pytest.approx(0.5, abs=TOLERANCE)
+    assert p0.domains[0].substrates == [_ma]
+    assert p0.domains[0].products == [_mb]
+    assert p0.domains[0].vmax == pytest.approx(1.1, abs=_TOLERANCE)
+    assert p0.domains[0].km == pytest.approx(0.5, abs=_TOLERANCE)
     assert isinstance(p0.domains[1], CatalyticDomain)
-    assert p0.domains[1].substrates == [md]
-    assert p0.domains[1].products == [mb, mc]
-    assert p0.domains[1].vmax == pytest.approx(1.2, abs=TOLERANCE)
-    assert p0.domains[1].km == pytest.approx(1.5, abs=TOLERANCE)
+    assert p0.domains[1].substrates == [_md]
+    assert p0.domains[1].products == [_mb, _mc]
+    assert p0.domains[1].vmax == pytest.approx(1.2, abs=_TOLERANCE)
+    assert p0.domains[1].km == pytest.approx(1.5, abs=_TOLERANCE)
 
     p1 = proteins[1]
     assert isinstance(p1.domains[0], CatalyticDomain)
-    assert p1.domains[0].substrates == [mb]
-    assert p1.domains[0].products == [mc]
-    assert p1.domains[0].vmax == pytest.approx(2.0, abs=TOLERANCE)
-    assert p1.domains[0].km == pytest.approx(0.9, abs=TOLERANCE)
+    assert p1.domains[0].substrates == [_mb]
+    assert p1.domains[0].products == [_mc]
+    assert p1.domains[0].vmax == pytest.approx(2.0, abs=_TOLERANCE)
+    assert p1.domains[0].km == pytest.approx(0.9, abs=_TOLERANCE)
     assert isinstance(p1.domains[1], CatalyticDomain)
-    assert p1.domains[1].substrates == [md]
-    assert p1.domains[1].products == [mb, mc]
-    assert p1.domains[1].vmax == pytest.approx(1.3, abs=TOLERANCE)
-    assert p1.domains[1].km == pytest.approx(1.2, abs=TOLERANCE)
+    assert p1.domains[1].substrates == [_md]
+    assert p1.domains[1].products == [_mb, _mc]
+    assert p1.domains[1].vmax == pytest.approx(1.3, abs=_TOLERANCE)
+    assert p1.domains[1].km == pytest.approx(1.2, abs=_TOLERANCE)
 
     p2 = proteins[2]
     assert isinstance(p2.domains[0], CatalyticDomain)
-    assert p2.domains[0].substrates == [md]
-    assert p2.domains[0].products == [mb, mb]
-    assert p2.domains[0].vmax == pytest.approx(2.9, abs=TOLERANCE)
-    assert p2.domains[0].km == pytest.approx(2.9, abs=TOLERANCE)
+    assert p2.domains[0].substrates == [_md]
+    assert p2.domains[0].products == [_mb, _mb]
+    assert p2.domains[0].vmax == pytest.approx(2.9, abs=_TOLERANCE)
+    assert p2.domains[0].km == pytest.approx(2.9, abs=_TOLERANCE)
 
     proteins = kinetics.get_proteome(proteome=c1)
 
     p0 = proteins[0]
     assert isinstance(p0.domains[0], CatalyticDomain)
-    assert p0.domains[0].substrates == [mb]
-    assert p0.domains[0].products == [ma]
-    assert p0.domains[0].vmax == pytest.approx(1.1, abs=TOLERANCE)
-    assert p0.domains[0].km == pytest.approx(0.3, abs=TOLERANCE)
+    assert p0.domains[0].substrates == [_mb]
+    assert p0.domains[0].products == [_ma]
+    assert p0.domains[0].vmax == pytest.approx(1.1, abs=_TOLERANCE)
+    assert p0.domains[0].km == pytest.approx(0.3, abs=_TOLERANCE)
     assert isinstance(p0.domains[1], CatalyticDomain)
-    assert p0.domains[1].substrates == [md]
-    assert p0.domains[1].products == [mb, mc]
-    assert p0.domains[1].vmax == pytest.approx(2.1, abs=TOLERANCE)
-    assert p0.domains[1].km == pytest.approx(1.4, abs=TOLERANCE)
+    assert p0.domains[1].substrates == [_md]
+    assert p0.domains[1].products == [_mb, _mc]
+    assert p0.domains[1].vmax == pytest.approx(2.1, abs=_TOLERANCE)
+    assert p0.domains[1].km == pytest.approx(1.4, abs=_TOLERANCE)
 
     p1 = proteins[1]
     assert isinstance(p1.domains[0], CatalyticDomain)
-    assert p1.domains[0].substrates == [mb]
-    assert p1.domains[0].products == [mc]
-    assert p1.domains[0].vmax == pytest.approx(1.9, abs=TOLERANCE)
-    assert p1.domains[0].km == pytest.approx(0.3, abs=TOLERANCE)
+    assert p1.domains[0].substrates == [_mb]
+    assert p1.domains[0].products == [_mc]
+    assert p1.domains[0].vmax == pytest.approx(1.9, abs=_TOLERANCE)
+    assert p1.domains[0].km == pytest.approx(0.3, abs=_TOLERANCE)
     assert isinstance(p1.domains[1], CatalyticDomain)
-    assert p1.domains[1].substrates == [mb, mc]
-    assert p1.domains[1].products == [md]
-    assert p1.domains[1].vmax == pytest.approx(2.3, abs=TOLERANCE)
-    assert p1.domains[1].km == pytest.approx(1.7, abs=TOLERANCE)
+    assert p1.domains[1].substrates == [_mb, _mc]
+    assert p1.domains[1].products == [_md]
+    assert p1.domains[1].vmax == pytest.approx(2.3, abs=_TOLERANCE)
+    assert p1.domains[1].km == pytest.approx(1.7, abs=_TOLERANCE)
 
 
 def test_simple_mm_kinetic():
     # 2 cell, 3 max proteins, 4 molecules (a, b, c, d)
     # cell 0: P0: a -> b, P1: b -> d
     # cell 1: P0: c -> d, P1: a -> d
 
@@ -732,34 +732,34 @@
     v_c1_1 = mm(X0[1, 0], X0[1, 3], Kmf[1, 1], Kmb[1, 1], Vmax[1, 1])
     dx_c1_a = -v_c1_1
     dx_c1_b = 0.0
     dx_c1_c = -v_c1_0
     dx_c1_d = v_c1_0 + v_c1_1
 
     # test
-    kinetics = get_kinetics()
+    kinetics = _get_kinetics()
     kinetics.N = N
     kinetics.Nf = Nf
     kinetics.Nb = Nb
     kinetics.Kmf = Kmf
     kinetics.Kmb = Kmb
     kinetics.Kmr = Kmr
     kinetics.Vmax = Vmax
     kinetics.A = A
     Xd = kinetics.integrate_signals(X=X0) - X0
 
-    assert (Xd[0, 0] - dx_c0_a).abs() < TOLERANCE
-    assert (Xd[0, 1] - dx_c0_b).abs() < TOLERANCE
-    assert (Xd[0, 2] - dx_c0_c).abs() < TOLERANCE
-    assert (Xd[0, 3] - dx_c0_d).abs() < TOLERANCE
-
-    assert (Xd[1, 0] - dx_c1_a).abs() < TOLERANCE
-    assert (Xd[1, 1] - dx_c1_b).abs() < TOLERANCE
-    assert (Xd[1, 2] - dx_c1_c).abs() < TOLERANCE
-    assert (Xd[1, 3] - dx_c1_d).abs() < TOLERANCE
+    assert (Xd[0, 0] - dx_c0_a).abs() < _TOLERANCE
+    assert (Xd[0, 1] - dx_c0_b).abs() < _TOLERANCE
+    assert (Xd[0, 2] - dx_c0_c).abs() < _TOLERANCE
+    assert (Xd[0, 3] - dx_c0_d).abs() < _TOLERANCE
+
+    assert (Xd[1, 0] - dx_c1_a).abs() < _TOLERANCE
+    assert (Xd[1, 1] - dx_c1_b).abs() < _TOLERANCE
+    assert (Xd[1, 2] - dx_c1_c).abs() < _TOLERANCE
+    assert (Xd[1, 3] - dx_c1_d).abs() < _TOLERANCE
 
 
 def test_mm_kinetic_with_proportions():
     # 2 cell, 3 max proteins, 4 molecules (a, b, c, d)
     # cell 0: P0: a -> 2b, P1: 2c -> d
     # cell 1: P0: 3b -> 2c
 
@@ -831,34 +831,34 @@
     v_c1_0 = mm32(X0[1, 1], X0[1, 2], Kmf[1, 0], Kmb[1, 0], Vmax[1, 0])
     dx_c1_a = 0.0
     dx_c1_b = -3 * v_c1_0
     dx_c1_c = 2 * v_c1_0
     dx_c1_d = 0.0
 
     # test
-    kinetics = get_kinetics()
+    kinetics = _get_kinetics()
     kinetics.N = N
     kinetics.Nf = Nf
     kinetics.Nb = Nb
     kinetics.Kmf = Kmf
     kinetics.Kmb = Kmb
     kinetics.Kmr = Kmr
     kinetics.Vmax = Vmax
     kinetics.A = A
     Xd = kinetics.integrate_signals(X=X0) - X0
 
-    assert (Xd[0, 0] - dx_c0_a).abs() < TOLERANCE
-    assert (Xd[0, 1] - dx_c0_b).abs() < TOLERANCE
-    assert (Xd[0, 2] - dx_c0_c).abs() < TOLERANCE
-    assert (Xd[0, 3] - dx_c0_d).abs() < TOLERANCE
-
-    assert (Xd[1, 0] - dx_c1_a).abs() < TOLERANCE
-    assert (Xd[1, 1] - dx_c1_b).abs() < TOLERANCE
-    assert (Xd[1, 2] - dx_c1_c).abs() < TOLERANCE
-    assert (Xd[1, 3] - dx_c1_d).abs() < TOLERANCE
+    assert (Xd[0, 0] - dx_c0_a).abs() < _TOLERANCE
+    assert (Xd[0, 1] - dx_c0_b).abs() < _TOLERANCE
+    assert (Xd[0, 2] - dx_c0_c).abs() < _TOLERANCE
+    assert (Xd[0, 3] - dx_c0_d).abs() < _TOLERANCE
+
+    assert (Xd[1, 0] - dx_c1_a).abs() < _TOLERANCE
+    assert (Xd[1, 1] - dx_c1_b).abs() < _TOLERANCE
+    assert (Xd[1, 2] - dx_c1_c).abs() < _TOLERANCE
+    assert (Xd[1, 3] - dx_c1_d).abs() < _TOLERANCE
 
 
 def test_mm_kinetic_with_multiple_substrates():
     # 2 cell, 3 max proteins, 4 molecules (a, b, c, d)
     # cell 0: P0: a,b -> c, P1: b,d -> 2a,c
     # cell 1: P0: a,d -> b
 
@@ -928,34 +928,34 @@
     v_c1_0 = mm111(X0[1, 0], X0[1, 3], X0[1, 1], Kmf[1, 0], Kmb[1, 0], Vmax[1, 0])
     dx_c1_a = -v_c1_0
     dx_c1_b = v_c1_0
     dx_c1_c = 0.0
     dx_c1_d = -v_c1_0
 
     # test
-    kinetics = get_kinetics()
+    kinetics = _get_kinetics()
     kinetics.N = N
     kinetics.Nf = Nf
     kinetics.Nb = Nb
     kinetics.Kmf = Kmf
     kinetics.Kmb = Kmb
     kinetics.Kmr = Kmr
     kinetics.Vmax = Vmax
     kinetics.A = A
     Xd = kinetics.integrate_signals(X=X0) - X0
 
-    assert (Xd[0, 0] - dx_c0_a).abs() < TOLERANCE
-    assert (Xd[0, 1] - dx_c0_b).abs() < TOLERANCE
-    assert (Xd[0, 2] - dx_c0_c).abs() < TOLERANCE
-    assert (Xd[0, 3] - dx_c0_d).abs() < TOLERANCE
-
-    assert (Xd[1, 0] - dx_c1_a).abs() < TOLERANCE
-    assert (Xd[1, 1] - dx_c1_b).abs() < TOLERANCE
-    assert (Xd[1, 2] - dx_c1_c).abs() < TOLERANCE
-    assert (Xd[1, 3] - dx_c1_d).abs() < TOLERANCE
+    assert (Xd[0, 0] - dx_c0_a).abs() < _TOLERANCE
+    assert (Xd[0, 1] - dx_c0_b).abs() < _TOLERANCE
+    assert (Xd[0, 2] - dx_c0_c).abs() < _TOLERANCE
+    assert (Xd[0, 3] - dx_c0_d).abs() < _TOLERANCE
+
+    assert (Xd[1, 0] - dx_c1_a).abs() < _TOLERANCE
+    assert (Xd[1, 1] - dx_c1_b).abs() < _TOLERANCE
+    assert (Xd[1, 2] - dx_c1_c).abs() < _TOLERANCE
+    assert (Xd[1, 3] - dx_c1_d).abs() < _TOLERANCE
 
 
 def test_mm_kinetic_with_cofactors():
     # 2 cell, 3 max proteins, 4 molecules (a, b, c, d)
     # N for a molecule might be 0 but it's still required
     # cell 0: P0: a -> b | b -> c
     # cell 0: P1: a + c -> b + c
@@ -1035,34 +1035,34 @@
     )
     dx_c1_a = -v_c1_0
     dx_c1_b = v_c1_0
     dx_c1_c = 0.0
     dx_c1_d = 0.0
 
     # test
-    kinetics = get_kinetics()
+    kinetics = _get_kinetics()
     kinetics.N = N
     kinetics.Nf = Nf
     kinetics.Nb = Nb
     kinetics.Kmf = Kmf
     kinetics.Kmb = Kmb
     kinetics.Kmr = Kmr
     kinetics.Vmax = Vmax
     kinetics.A = A
     Xd = kinetics.integrate_signals(X=X0) - X0
 
-    assert (Xd[0, 0] - dx_c0_a).abs() < TOLERANCE
-    assert (Xd[0, 1] - dx_c0_b).abs() < TOLERANCE
-    assert (Xd[0, 2] - dx_c0_c).abs() < TOLERANCE
-    assert (Xd[0, 3] - dx_c0_d).abs() < TOLERANCE
-
-    assert (Xd[1, 0] - dx_c1_a).abs() < TOLERANCE
-    assert (Xd[1, 1] - dx_c1_b).abs() < TOLERANCE
-    assert (Xd[1, 2] - dx_c1_c).abs() < TOLERANCE
-    assert (Xd[1, 3] - dx_c1_d).abs() < TOLERANCE
+    assert (Xd[0, 0] - dx_c0_a).abs() < _TOLERANCE
+    assert (Xd[0, 1] - dx_c0_b).abs() < _TOLERANCE
+    assert (Xd[0, 2] - dx_c0_c).abs() < _TOLERANCE
+    assert (Xd[0, 3] - dx_c0_d).abs() < _TOLERANCE
+
+    assert (Xd[1, 0] - dx_c1_a).abs() < _TOLERANCE
+    assert (Xd[1, 1] - dx_c1_b).abs() < _TOLERANCE
+    assert (Xd[1, 2] - dx_c1_c).abs() < _TOLERANCE
+    assert (Xd[1, 3] - dx_c1_d).abs() < _TOLERANCE
 
 
 def test_mm_kinetic_with_allosteric_action():
     # 2 cell, 3 max proteins, 4 molecules (a, b, c, d)
     # cell 0: P0: a -> b, inhibitor=c, P1: c -> d, activator=a, P2: a -> b, inh=c, act=d
     # cell 1: P0: a -> b, inhibitor=c,d, P1: c -> d, activator=a,b
 
@@ -1159,34 +1159,34 @@
     )
     dx_c1_a = -v_c1_0
     dx_c1_b = v_c1_0
     dx_c1_c = -v_c1_1
     dx_c1_d = v_c1_1
 
     # test
-    kinetics = get_kinetics()
+    kinetics = _get_kinetics()
     kinetics.N = N
     kinetics.Nf = Nf
     kinetics.Nb = Nb
     kinetics.Kmf = Kmf
     kinetics.Kmb = Kmb
     kinetics.Kmr = Kmr
     kinetics.Vmax = Vmax
     kinetics.A = A
     Xd = kinetics.integrate_signals(X=X0) - X0
 
-    assert (Xd[0, 0] - dx_c0_a).abs() < TOLERANCE
-    assert (Xd[0, 1] - dx_c0_b).abs() < TOLERANCE
-    assert (Xd[0, 2] - dx_c0_c).abs() < TOLERANCE
-    assert (Xd[0, 3] - dx_c0_d).abs() < TOLERANCE
-
-    assert (Xd[1, 0] - dx_c1_a).abs() < TOLERANCE
-    assert (Xd[1, 1] - dx_c1_b).abs() < TOLERANCE
-    assert (Xd[1, 2] - dx_c1_c).abs() < TOLERANCE
-    assert (Xd[1, 3] - dx_c1_d).abs() < TOLERANCE
+    assert (Xd[0, 0] - dx_c0_a).abs() < _TOLERANCE
+    assert (Xd[0, 1] - dx_c0_b).abs() < _TOLERANCE
+    assert (Xd[0, 2] - dx_c0_c).abs() < _TOLERANCE
+    assert (Xd[0, 3] - dx_c0_d).abs() < _TOLERANCE
+
+    assert (Xd[1, 0] - dx_c1_a).abs() < _TOLERANCE
+    assert (Xd[1, 1] - dx_c1_b).abs() < _TOLERANCE
+    assert (Xd[1, 2] - dx_c1_c).abs() < _TOLERANCE
+    assert (Xd[1, 3] - dx_c1_d).abs() < _TOLERANCE
 
 
 def test_reduce_velocity_to_avoid_negative_concentrations():
     # 2 cell, 3 max proteins, 4 molecules (a, b, c, d)
     # cell 0: P0: a -> b, P1: b -> d
     # cell 1: P0: 2c -> d
 
@@ -1246,53 +1246,53 @@
     v_c0_0 = mm(X0[0, 0], X0[0, 1], Kmf[0, 0], Kmb[0, 0], Vmax[0, 0])
     v_c0_1 = mm(X0[0, 1], X0[0, 3], Kmf[0, 1], Kmb[0, 1], Vmax[0, 1])
     # but this would lead to Xd + X0 = -0.0615 (for a)
     assert X0[0, 0] - v_c0_0 < 0.0
     # so velocity should be reduced by a factor depending on current a
     # all other proteins in this cell are reduce by the same factor
     # to avoid follow up problems with other molecules being destroyed by other proteins
-    f = (X0[0, 0] - EPS) / v_c0_0
+    f = (X0[0, 0] - _EPS) / v_c0_0
     v_c0_0 = f * v_c0_0
     v_c0_1 = f * v_c0_1
     dx_c0_a = -v_c0_0
     dx_c0_b = v_c0_0 - v_c0_1
     dx_c0_c = 0.0
     dx_c0_d = v_c0_1
 
     v_c1_0 = mm21(X0[1, 2], X0[1, 3], Kmf[1, 0], Kmb[1, 0], Vmax[1, 0])
     # but this would lead to Xd + X0 = -0.0722 (for c)
     assert X0[1, 2] - 2 * v_c1_0 < 0.0
     # as above, velocities are reduced. here its only this protein
-    v_c1_0 = (X0[1, 2] - EPS) / 2
+    v_c1_0 = (X0[1, 2] - _EPS) / 2
     dx_c1_a = 0.0
     dx_c1_b = 0.0
     dx_c1_c = -2 * v_c1_0
     dx_c1_d = v_c1_0
 
     # test
-    kinetics = get_kinetics()
+    kinetics = _get_kinetics()
     kinetics.N = N
     kinetics.Nf = Nf
     kinetics.Nb = Nb
     kinetics.Kmf = Kmf
     kinetics.Kmb = Kmb
     kinetics.Kmr = Kmr
     kinetics.Vmax = Vmax
     kinetics.A = A
     Xd = kinetics.integrate_signals(X=X0) - X0
 
-    assert (Xd[0, 0] - dx_c0_a).abs() < TOLERANCE
-    assert (Xd[0, 1] - dx_c0_b).abs() < TOLERANCE
-    assert (Xd[0, 2] - dx_c0_c).abs() < TOLERANCE
-    assert (Xd[0, 3] - dx_c0_d).abs() < TOLERANCE
-
-    assert (Xd[1, 0] - dx_c1_a).abs() < TOLERANCE
-    assert (Xd[1, 1] - dx_c1_b).abs() < TOLERANCE
-    assert (Xd[1, 2] - dx_c1_c).abs() < TOLERANCE
-    assert (Xd[1, 3] - dx_c1_d).abs() < TOLERANCE
+    assert (Xd[0, 0] - dx_c0_a).abs() < _TOLERANCE
+    assert (Xd[0, 1] - dx_c0_b).abs() < _TOLERANCE
+    assert (Xd[0, 2] - dx_c0_c).abs() < _TOLERANCE
+    assert (Xd[0, 3] - dx_c0_d).abs() < _TOLERANCE
+
+    assert (Xd[1, 0] - dx_c1_a).abs() < _TOLERANCE
+    assert (Xd[1, 1] - dx_c1_b).abs() < _TOLERANCE
+    assert (Xd[1, 2] - dx_c1_c).abs() < _TOLERANCE
+    assert (Xd[1, 3] - dx_c1_d).abs() < _TOLERANCE
 
     X1 = X0 + Xd
     assert not torch.any(X1 < 0.0)
 
 
 def test_reduce_velocity_in_multiple_proteins():
     # 2 cell, 3 max proteins, 4 molecules (a, b, c, d)
@@ -1358,15 +1358,15 @@
     v_c0_0 = mm(X0[0, 0], X0[0, 1], Kmf[0, 0], Kmb[0, 0], Vmax[0, 0])
     v_c0_1 = mm21(X0[0, 0], X0[0, 3], Kmf[0, 1], Kmb[0, 1], Vmax[0, 1])
     # but this would lead to a < 0.0
     naive_dx_c0_a = -v_c0_0 - 2 * v_c0_1
     assert X0[0, 0] + naive_dx_c0_a < 0.0
     # so velocity should be reduced to by a factor to not deconstruct too much a
     # all other proteins have to be reduced by the same factor to not cause downstream problems
-    f = (X0[0, 0] - EPS) / -naive_dx_c0_a
+    f = (X0[0, 0] - _EPS) / -naive_dx_c0_a
     v_c0_0 = v_c0_0 * f
     v_c0_1 = v_c0_1 * f
     dx_c0_a = -v_c0_0 - v_c0_1 * 2
     dx_c0_b = v_c0_0
     dx_c0_c = 0.0
     dx_c0_d = v_c0_1
 
@@ -1374,180 +1374,30 @@
     v_c1_0 = mm(X0[1, 0], X0[1, 1], Kmf[1, 0], Kmb[1, 0], Vmax[1, 0])
     dx_c1_a = -v_c1_0
     dx_c1_b = v_c1_0
     dx_c1_c = 0.0
     dx_c1_d = 0.0
 
     # test
-    kinetics = get_kinetics()
+    kinetics = _get_kinetics()
     kinetics.N = N
     kinetics.Nf = Nf
     kinetics.Nb = Nb
     kinetics.Kmf = Kmf
     kinetics.Kmb = Kmb
     kinetics.Kmr = Kmr
     kinetics.Vmax = Vmax
     kinetics.A = A
     Xd = kinetics.integrate_signals(X=X0) - X0
 
-    assert (Xd[0, 0] - dx_c0_a).abs() < TOLERANCE
-    assert (Xd[0, 1] - dx_c0_b).abs() < TOLERANCE
-    assert (Xd[0, 2] - dx_c0_c).abs() < TOLERANCE
-    assert (Xd[0, 3] - dx_c0_d).abs() < TOLERANCE
-
-    assert (Xd[1, 0] - dx_c1_a).abs() < TOLERANCE
-    assert (Xd[1, 1] - dx_c1_b).abs() < TOLERANCE
-    assert (Xd[1, 2] - dx_c1_c).abs() < TOLERANCE
-    assert (Xd[1, 3] - dx_c1_d).abs() < TOLERANCE
+    assert (Xd[0, 0] - dx_c0_a).abs() < _TOLERANCE
+    assert (Xd[0, 1] - dx_c0_b).abs() < _TOLERANCE
+    assert (Xd[0, 2] - dx_c0_c).abs() < _TOLERANCE
+    assert (Xd[0, 3] - dx_c0_d).abs() < _TOLERANCE
+
+    assert (Xd[1, 0] - dx_c1_a).abs() < _TOLERANCE
+    assert (Xd[1, 1] - dx_c1_b).abs() < _TOLERANCE
+    assert (Xd[1, 2] - dx_c1_c).abs() < _TOLERANCE
+    assert (Xd[1, 3] - dx_c1_d).abs() < _TOLERANCE
 
     X1 = X0 + Xd
     assert not torch.any(X1 < 0.0)
-
-
-def test_equilibrium_is_reached():
-    # molecules should reach equilibrium after a few steps
-    # with Vmax > 1.0 higher order reactions cant reach equilibrium
-    # because they overshoot
-
-    # 2 cell, 3 max proteins, 4 molecules (a, b, c, d)
-    # cell 0: P0: a -> b (Ke=1.0), P1: c -> d (Ke=20.0)
-    # cell 1: P0: a,2b -> c (Ke=10.0)
-
-    # fmt: off
-
-    # concentrations (c, s)
-    X0 = torch.tensor([
-        [2.0, 20.0, 5.0, 5.0],
-        [2.0, 3.1, 1.3, 2.9],
-    ])
-
-    # reactions (c, p, s)
-    N = torch.tensor([
-        [   [-1.0, 1.0, 0.0, 0.0],
-            [0.0, 0.0, -1.0, 1.0],
-            [0.0, 0.0, 0.0, 0.0]    ],
-        [   [-1.0, -2.0, 1.0, 0.0],
-            [0.0, 0.0, 0.0, 0.0],
-            [0.0, 0.0, 0.0, 0.0]    ],
-    ])
-    Nf = torch.where(N < 0.0, -N, 0.0)
-    Nb = torch.where(N > 0.0, N, 0.0)
-
-    # affinities (c, p)
-    Kmf = torch.tensor([
-        [1.0, 1.0, 0.0],
-        [1.0, 0.0, 0.0],
-    ])
-    Kmb = torch.tensor([
-        [1.0, 20.0, 0.0],
-        [10.0, 0.0, 0.0],
-    ])
-    Kmr = torch.zeros(2, 3)
-
-    # max velocities (c, p)
-    Vmax = torch.tensor([
-        [100.0, 100.0, 0.0],
-        [100.0, 0.0, 0.0],
-    ])
-
-    # allosterics (c, p, s)
-    A = torch.zeros(2, 3, 4)
-
-    # test
-    kinetics = get_kinetics(n_computations=11)
-    kinetics.N = N
-    kinetics.Nf = Nf
-    kinetics.Nb = Nb
-    kinetics.Kmf = Kmf
-    kinetics.Kmb = Kmb
-    kinetics.Kmr = Kmr
-    kinetics.Vmax = Vmax
-    kinetics.A = A
-
-    for _ in range(10):
-        X0 = kinetics.integrate_signals(X=X0)
-
-    q_c0_0 = X0[0, 1] / X0[0, 0]
-    q_c0_1 = X0[0, 3] / X0[0, 2]
-    q_c1_0 = X0[1, 2] / (X0[1, 0] * X0[1, 1] * X0[1, 1])
-
-    assert (q_c0_0 - 1.0).abs() < 0.1
-    assert (q_c0_1 - 20.0).abs() < 2.0
-    assert (q_c1_0 - 10.0).abs() < 1.0
-
-
-def test_zero_substrates_stay_zero():
-    # Typical reasons for cells creating signals from 0:
-    # 1. when using exp(ln(x)) 1s can accidentally be created
-    # 2. when doing a^b 1s can be created (0^1=0 but 0^0=1)
-
-    n_cells = 100
-    n_prots = 100
-    n_steps = 100
-
-    kinetics = get_kinetics()
-    n_mols = len(MOLECULES) * 2
-
-    # concentrations (c, s)
-    X = torch.zeros(n_cells, n_mols).abs()
-
-    # reactions (c, p, s)
-    kinetics.N = torch.randint(low=-3, high=4, size=(n_cells, n_prots, n_mols)).float()
-    kinetics.Nf = torch.where(kinetics.N < 0.0, -kinetics.N, 0.0)
-    kinetics.Nb = torch.where(kinetics.N > 0.0, kinetics.N, 0.0)
-
-    # max velocities (c, p)
-    kinetics.Vmax = torch.randn(n_cells, n_prots).abs() * 100
-
-    # allosterics (c, p, s)
-    kinetics.A = torch.randint(low=-2, high=3, size=(n_cells, n_prots, n_mols))
-
-    # affinities (c, p)
-    Ke = torch.randn(n_cells, n_prots)
-    kinetics.Kmf = torch.randn(n_cells, n_prots).abs()
-    kinetics.Kmb = kinetics.Kmf * Ke
-    kinetics.Kmr = torch.randn(n_cells, n_prots).abs()
-
-    # test
-    for _ in range(n_steps):
-        X = kinetics.integrate_signals(X=X)
-        assert X.min() == 0.0
-        assert X.max() == 0.0
-
-
-def test_substrate_concentrations_are_always_finite_and_positive():
-    # interaction terms can overflow float32 when they become too big
-    # i.g. exponents too high and many substrates
-    # this will create infinites which will eventually become NaN
-    n_cells = 100
-    n_prots = 100
-    n_steps = 100
-
-    kinetics = get_kinetics()
-    n_mols = len(MOLECULES) * 2
-
-    # concentrations (c, s)
-    X = torch.randn(n_cells, n_mols).abs()
-
-    # reactions (c, p, s)
-    kinetics.N = torch.randint(low=-3, high=4, size=(n_cells, n_prots, n_mols)).float()
-    kinetics.Nf = torch.where(kinetics.N < 0.0, -kinetics.N, 0.0)
-    kinetics.Nb = torch.where(kinetics.N > 0.0, kinetics.N, 0.0)
-
-    # max velocities (c, p)
-    kinetics.Vmax = torch.randn(n_cells, n_prots).abs().clamp(max=1.0) * 100
-
-    # allosterics (c, p, s)
-    kinetics.A = torch.randint(low=-2, high=3, size=(n_cells, n_prots, n_mols))
-
-    # affinities (c, p)
-    Ke = torch.randn(n_cells, n_prots)
-    kinetics.Kmf = torch.randn(n_cells, n_prots).abs().clamp(0.001)
-    kinetics.Kmb = (kinetics.Kmf * Ke).clamp(0.001)
-    kinetics.Kmr = torch.randn(n_cells, n_prots).abs().clamp(0.001)
-
-    # test
-    for _ in range(n_steps):
-        X = kinetics.integrate_signals(X=X)
-        assert not torch.any(X < 0.0), X[X < 0.0].min()
-        assert not torch.any(X.isnan()), X.isnan().sum()
-        assert torch.all(X.isfinite()), ~X.isfinite().sum()
```

### Comparing `magicsoup-0.4.0/tests/test_mutations.py` & `magicsoup-0.4.1/tests/test_mutations.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.0/tests/test_util.py` & `magicsoup-0.4.1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.4.0/tests/test_world.py` & `magicsoup-0.4.1/tests/test_world.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,65 +188,14 @@
 
     world.kill_cells(cell_idxs=list(range(n2)))
     n3 = world.n_cells
     assert n3 == 0
     assert world.cell_map.sum().item() == n3
 
 
-def test_molecule_amount_integrity_during_diffusion():
-    chemistry = ms.Chemistry(molecules=MOLECULES, reactions=[])
-    world = ms.World(chemistry=chemistry, map_size=128)
-
-    exp = world.molecule_map.sum(dim=[1, 2])
-    for step_i in range(100):
-        world.diffuse_molecules()
-        res = world.molecule_map.sum(dim=[1, 2])
-        assert (res.sum() - exp.sum()).abs() < 10.0, step_i
-        assert torch.all(torch.abs(res - exp) < 1.0), step_i
-
-
-def test_molecule_amount_integrity_during_reactions():
-    # X and Y can react back and forth but X + Y <-> Z
-    # so if Z is counted as 2, n should stay equal
-    mi = ms.Molecule("i", 10 * 1e3)
-    mj = ms.Molecule("j", 20 * 1e3)
-    mk = ms.Molecule("k", 30 * 1e3)
-    molecules = [mi, mj, mk]
-    reactions = [([mi], [mj]), ([mi, mj], [mk])]
-
-    chemistry = ms.Chemistry(molecules=molecules, reactions=reactions)
-    world = ms.World(chemistry=chemistry, map_size=128)
-    genomes = [ms.random_genome(s=500) for _ in range(1000)]
-    world.add_cells(genomes=genomes)
-
-    def count(world: ms.World) -> float:
-        mij = world.molecule_map[[0, 1]].sum().item()
-        mk = world.molecule_map[2].sum().item() * 2
-        cij = world.cell_molecules[:, [0, 1]].sum().item()
-        ck = world.cell_molecules[:, 2].sum().item() * 2
-        return mij + mk + cij + ck
-
-    n0 = count(world)
-    for step_i in range(100):
-        world.enzymatic_activity()
-        n = count(world)
-        assert n == pytest.approx(n0, abs=1.0), step_i
-
-
-def test_run_world_without_reactions():
-    chemistry = ms.Chemistry(molecules=MOLECULES[:2], reactions=[])
-    world = ms.World(chemistry=chemistry)
-
-    genomes = [ms.random_genome(s=500) for _ in range(1000)]
-    world.add_cells(genomes=genomes)
-
-    for _ in range(100):
-        world.enzymatic_activity()
-
-
 def test_cells_unable_to_divide():
     chemistry = ms.Chemistry(molecules=MOLECULES[:2], reactions=[])
     world = ms.World(chemistry=chemistry, map_size=3)
 
     genomes = [ms.random_genome(s=500) for _ in range(9)]
     world.add_cells(genomes=genomes)
```

