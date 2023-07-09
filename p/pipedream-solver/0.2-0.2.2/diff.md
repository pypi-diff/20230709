# Comparing `tmp/pipedream-solver-0.2.tar.gz` & `tmp/pipedream-solver-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pipedream-solver-0.2.tar", last modified: Sun Oct 24 16:59:21 2021, max compression
+gzip compressed data, was "pipedream-solver-0.2.2.tar", last modified: Sun Jul  9 17:32:19 2023, max compression
```

## Comparing `pipedream-solver-0.2.tar` & `pipedream-solver-0.2.2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 mdbartos   (501) staff       (20)        0 2021-10-24 16:59:21.000000 pipedream-solver-0.2/
--rw-r--r--   0 mdbartos   (501) staff       (20)      320 2021-10-24 16:59:21.000000 pipedream-solver-0.2/PKG-INFO
-drwxr-xr-x   0 mdbartos   (501) staff       (20)        0 2021-10-24 16:59:21.000000 pipedream-solver-0.2/test/
--rw-r--r--   0 mdbartos   (501) staff       (20)    15752 2021-10-24 16:56:13.000000 pipedream-solver-0.2/test/test_pipedream.py
-drwxr-xr-x   0 mdbartos   (501) staff       (20)        0 2021-10-24 16:59:21.000000 pipedream-solver-0.2/pipedream_solver.egg-info/
--rw-r--r--   0 mdbartos   (501) staff       (20)      320 2021-10-24 16:59:21.000000 pipedream-solver-0.2/pipedream_solver.egg-info/PKG-INFO
--rw-r--r--   0 mdbartos   (501) staff       (20)      693 2021-10-24 16:59:21.000000 pipedream-solver-0.2/pipedream_solver.egg-info/SOURCES.txt
--rw-r--r--   0 mdbartos   (501) staff       (20)       36 2021-10-24 16:59:21.000000 pipedream-solver-0.2/pipedream_solver.egg-info/requires.txt
--rw-r--r--   0 mdbartos   (501) staff       (20)       17 2021-10-24 16:59:21.000000 pipedream-solver-0.2/pipedream_solver.egg-info/top_level.txt
--rw-r--r--   0 mdbartos   (501) staff       (20)        1 2021-10-24 16:59:21.000000 pipedream-solver-0.2/pipedream_solver.egg-info/dependency_links.txt
--rw-r--r--   0 mdbartos   (501) staff       (20)     4274 2021-10-24 16:56:13.000000 pipedream-solver-0.2/README.md
--rw-r--r--   0 mdbartos   (501) staff       (20)      484 2021-10-24 16:56:13.000000 pipedream-solver-0.2/setup.py
--rw-r--r--   0 mdbartos   (501) staff       (20)       38 2021-10-24 16:59:21.000000 pipedream-solver-0.2/setup.cfg
-drwxr-xr-x   0 mdbartos   (501) staff       (20)        0 2021-10-24 16:59:21.000000 pipedream-solver-0.2/pipedream_solver/
--rw-r--r--   0 mdbartos   (501) staff       (20)    23271 2021-10-24 16:56:13.000000 pipedream-solver-0.2/pipedream_solver/simulation.py
--rw-r--r--   0 mdbartos   (501) staff       (20)   122329 2021-10-24 16:56:13.000000 pipedream-solver-0.2/pipedream_solver/nsuperlink.py
--rw-r--r--   0 mdbartos   (501) staff       (20)   184615 2021-10-24 16:56:13.000000 pipedream-solver-0.2/pipedream_solver/superlink.py
--rw-r--r--   0 mdbartos   (501) staff       (20)      236 2021-10-24 16:56:13.000000 pipedream-solver-0.2/pipedream_solver/hydrology.py
--rw-r--r--   0 mdbartos   (501) staff       (20)      204 2021-10-24 16:56:13.000000 pipedream-solver-0.2/pipedream_solver/transport.py
--rw-r--r--   0 mdbartos   (501) staff       (20)    11343 2021-10-24 16:56:13.000000 pipedream-solver-0.2/pipedream_solver/visualization.py
--rw-r--r--   0 mdbartos   (501) staff       (20)    11353 2021-10-24 16:56:13.000000 pipedream-solver-0.2/pipedream_solver/ninfiltration.py
--rw-r--r--   0 mdbartos   (501) staff       (20)    18404 2021-10-24 16:56:13.000000 pipedream-solver-0.2/pipedream_solver/ngeometry.py
--rw-r--r--   0 mdbartos   (501) staff       (20)     3742 2021-10-24 16:56:13.000000 pipedream-solver-0.2/pipedream_solver/utils.py
--rw-r--r--   0 mdbartos   (501) staff       (20)    26637 2021-10-24 16:56:13.000000 pipedream-solver-0.2/pipedream_solver/geometry.py
--rw-r--r--   0 mdbartos   (501) staff       (20)     2798 2021-10-24 16:56:13.000000 pipedream-solver-0.2/pipedream_solver/storage.py
--rw-r--r--   0 mdbartos   (501) staff       (20)    63936 2021-10-24 16:56:13.000000 pipedream-solver-0.2/pipedream_solver/nquality.py
--rw-r--r--   0 mdbartos   (501) staff       (20)     5181 2021-10-24 16:56:13.000000 pipedream-solver-0.2/pipedream_solver/nutils.py
--rw-r--r--   0 mdbartos   (501) staff       (20)      230 2021-10-24 16:56:13.000000 pipedream-solver-0.2/pipedream_solver/hydraulics.py
--rw-r--r--   0 mdbartos   (501) staff       (20)    14649 2021-10-24 16:56:13.000000 pipedream-solver-0.2/pipedream_solver/infiltration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:32:19.383782 pipedream-solver-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-09 17:32:07.000000 pipedream-solver-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-09 17:32:19.379782 pipedream-solver-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-07-09 17:32:07.000000 pipedream-solver-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:32:19.379782 pipedream-solver-0.2.2/pipedream_solver/
+-rw-r--r--   0 runner    (1001) docker     (123)    27177 2023-07-09 17:32:07.000000 pipedream-solver-0.2.2/pipedream_solver/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-09 17:32:07.000000 pipedream-solver-0.2.2/pipedream_solver/hydraulics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-09 17:32:07.000000 pipedream-solver-0.2.2/pipedream_solver/hydrology.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14649 2023-07-09 17:32:07.000000 pipedream-solver-0.2.2/pipedream_solver/infiltration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26352 2023-07-09 17:32:07.000000 pipedream-solver-0.2.2/pipedream_solver/ngeometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-07-09 17:32:07.000000 pipedream-solver-0.2.2/pipedream_solver/ninfiltration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66332 2023-07-09 17:32:07.000000 pipedream-solver-0.2.2/pipedream_solver/nquality.py
+-rw-r--r--   0 runner    (1001) docker     (123)   139034 2023-07-09 17:32:07.000000 pipedream-solver-0.2.2/pipedream_solver/nsuperlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-07-09 17:32:07.000000 pipedream-solver-0.2.2/pipedream_solver/nutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23271 2023-07-09 17:32:07.000000 pipedream-solver-0.2.2/pipedream_solver/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-09 17:32:07.000000 pipedream-solver-0.2.2/pipedream_solver/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)   191343 2023-07-09 17:32:07.000000 pipedream-solver-0.2.2/pipedream_solver/superlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-09 17:32:07.000000 pipedream-solver-0.2.2/pipedream_solver/transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-07-09 17:32:07.000000 pipedream-solver-0.2.2/pipedream_solver/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-09 17:32:07.000000 pipedream-solver-0.2.2/pipedream_solver/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:32:19.379782 pipedream-solver-0.2.2/pipedream_solver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-09 17:32:19.000000 pipedream-solver-0.2.2/pipedream_solver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-09 17:32:19.000000 pipedream-solver-0.2.2/pipedream_solver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 17:32:19.000000 pipedream-solver-0.2.2/pipedream_solver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-09 17:32:19.000000 pipedream-solver-0.2.2/pipedream_solver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-09 17:32:19.000000 pipedream-solver-0.2.2/pipedream_solver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 17:32:19.383782 pipedream-solver-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-09 17:32:07.000000 pipedream-solver-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:32:19.379782 pipedream-solver-0.2.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    15752 2023-07-09 17:32:07.000000 pipedream-solver-0.2.2/test/test_pipedream.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pipedream-solver-0.2/test/test_pipedream.py` & `pipedream-solver-0.2.2/test/test_pipedream.py`

 * *Files identical despite different names*

### Comparing `pipedream-solver-0.2/pipedream_solver.egg-info/SOURCES.txt` & `pipedream-solver-0.2.2/pipedream_solver.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 pipedream_solver/geometry.py
 pipedream_solver/hydraulics.py
 pipedream_solver/hydrology.py
 pipedream_solver/infiltration.py
 pipedream_solver/ngeometry.py
```

### Comparing `pipedream-solver-0.2/README.md` & `pipedream-solver-0.2.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # pipedream <sub>🚰</sub> <sup>💭</sup>
-[![Build Status](https://travis-ci.org/mdbartos/pipedream.svg?branch=master)](https://travis-ci.org/mdbartos/pipedream) [![Coverage Status](https://coveralls.io/repos/github/mdbartos/pipedream/badge.svg?branch=master)](https://coveralls.io/github/mdbartos/pipedream?branch=master) [![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370/) [![Docs](https://img.shields.io/badge/docs-read%20here-ff69b4)](https://mdbartos.github.io/pipedream/) [![Paper](https://img.shields.io/badge/EarthArXiv-10.31223/osf.io/d8ca6-orange)](https://eartharxiv.org/d8ca6)
+[![Build Status](https://travis-ci.org/mdbartos/pipedream.svg?branch=master)](https://travis-ci.org/mdbartos/pipedream) [![Coverage Status](https://coveralls.io/repos/github/mdbartos/pipedream/badge.svg?branch=master)](https://coveralls.io/github/mdbartos/pipedream?branch=master) [![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370/) [![Docs](https://img.shields.io/badge/docs-read%20here-ff69b4)](https://mdbartos.github.io/pipedream/) [![Paper](https://img.shields.io/badge/doi-10.1016%2Fj.envsoft.2021.105120-orange)](https://www.sciencedirect.com/science/article/pii/S1364815221001638)
 
 An interactive hydrodynamic solver for sewer/stormwater networks.
 
 ## About
 
 *Pipedream* is a physically-based sewer/stormwater model designed for real-time applications. The *pipedream* toolkit consists of four major components:
 
@@ -18,15 +18,15 @@
 - Stormwater asset management and detection of maintenance emergencies.
 - Data-driven water quality assessment.
 
 ## Documentation
 
 - Read the docs [here 📖](https://mdbartos.github.io/pipedream/).
 
-- Read the paper [here 📄](https://eartharxiv.org/d8ca6).
+- Read the paper [here 📄](https://www.sciencedirect.com/science/article/pii/S1364815221001638).
 
 ## Installation
 
 Use `pip` to install `pipedream-solver` via pypi:
 
 ```shell
 $ pip install pipedream-solver
@@ -82,15 +82,15 @@
 dt = 30
 
 # Create simulation context manager
 with Simulation(superlink, Q_in=Q_in, H_bc=H_bc) as simulation:
     # While simulation time has not expired...
     while simulation.t <= simulation.t_end:
         # Step model forward in time
-        simulation.step(dt=dt)
+        simulation.step(dt=dt, num_iter=1)
         # Record internal depth and flow states
         simulation.record_state()
         # Print progress bar
         simulation.print_progress()
 ```
 
 > `[==================================================] 100.0% [0.82 s]`
```

### Comparing `pipedream-solver-0.2/pipedream_solver/simulation.py` & `pipedream-solver-0.2.2/pipedream_solver/simulation.py`

 * *Files identical despite different names*

### Comparing `pipedream-solver-0.2/pipedream_solver/nsuperlink.py` & `pipedream-solver-0.2.2/pipedream_solver/nsuperlink.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import pandas as pd
 import scipy.linalg
 import scipy.optimize
 import scipy.integrate
 import scipy.sparse
 import scipy.sparse.linalg
 from numba import njit, prange
+from numba.types import float64, int64, uint32, uint16, uint8, boolean, UniTuple, Tuple, List, DictType, void
 import pipedream_solver.geometry
 import pipedream_solver.ngeometry
 import pipedream_solver.storage
 from pipedream_solver.superlink import SuperLink
 
 class nSuperLink(SuperLink):
     """
@@ -283,21 +284,21 @@
     def __init__(self, superlinks, superjunctions,
                  links=None, junctions=None,
                  transects={}, storages={},
                  orifices=None, weirs=None, pumps=None,
                  dt=60, sparse=False, min_depth=1e-5, method='b',
                  inertial_damping=False, bc_method='z',
                  exit_hydraulics=False, auto_permute=False,
-                 end_length=None, end_method='b', internal_links=4):
+                 end_length=None, end_method='b', internal_links=4, mobile_elements=False):
         super().__init__(superlinks, superjunctions,
                          links, junctions, transects, storages,
                          orifices, weirs, pumps, dt, sparse,
                          min_depth, method, inertial_damping,
                          bc_method, exit_hydraulics, auto_permute,
-                         end_length, end_method, internal_links)
+                         end_length, end_method, internal_links, mobile_elements)
 
     def configure_storages(self):
         """
         Prepare data structures for computation of superjunction storage.
         """
         # Import instance variables
         storages = self.storages                # Table of storages
@@ -377,26 +378,31 @@
         _Pe_ik = self._Pe_ik           # Hydraulic perimeter at link ik
         _R_ik = self._R_ik             # Hydraulic radius at link ik
         _B_ik = self._B_ik             # Top width at link ik
         _dx_ik = self._dx_ik           # Length of link ik
         _g1_ik = self._g1_ik           # Geometry 1 of link ik (vertical)
         _g2_ik = self._g2_ik           # Geometry 2 of link ik (horizontal)
         _g3_ik = self._g3_ik           # Geometry 3 of link ik (other)
+        _g4_ik = self._g4_ik           # Geometry 4 of link ik (other)
+        _g5_ik = self._g5_ik           # Geometry 5 of link ik (other)
+        _g6_ik = self._g6_ik           # Geometry 6 of link ik (other)
+        _g7_ik = self._g7_ik           # Geometry 7 of link ik (other)
         _geom_codes = self._geom_codes
         _ellipse_ix = self._ellipse_ix
         _transect_factory = self._transect_factory
         _transect_indices = self._transect_indices
         _has_irregular = self._has_irregular
         # Compute hydraulic geometry for regular geometries
         # NOTE: Handle case for elliptical perimeter first
         handle_elliptical_perimeter(_Pe_ik, _ellipse_ix, _Ik, _Ip1k, _h_Ik,
                                    _g1_ik, _g2_ik)
         # Compute hydraulic geometries for all other regular geometries
         numba_hydraulic_geometry(_A_ik, _Pe_ik, _R_ik, _B_ik, _h_Ik,
-                                 _g1_ik, _g2_ik, _g3_ik, _geom_codes, _Ik, _ik)
+                                 _g1_ik, _g2_ik, _g3_ik, _g4_ik, _g5_ik, _g6_ik, _g7_ik,
+                                 _geom_codes, _Ik, _ik)
         # Compute hydraulic geometry for irregular geometries
         if _has_irregular:
             for transect_name, generator in _transect_factory.items():
                 _ik_g = _transect_indices.loc[[transect_name]].values
                 _Ik_g = _Ik[_ik_g]
                 _Ip1k_g = _Ip1k[_ik_g]
                 _h_Ik_g = _h_Ik[_Ik_g]
@@ -418,31 +424,37 @@
         # Import instance variables
         _ik = self._ik                 # Link index
         _Ik = self._Ik                 # Junction index
         _ki = self._ki                 # Superlink index containing link ik
         _h_Ik = self._h_Ik             # Depth at junction Ik
         _A_uk = self._A_uk             # Flow area at upstream end of superlink k
         _B_uk = self._B_uk             # Top width at upstream end of superlink k
+        _Pe_uk = self._Pe_uk
+        _R_uk = self._R_uk
         _dx_ik = self._dx_ik           # Length of link ik
         _g1_ik = self._g1_ik           # Geometry 1 of link ik (vertical)
         _g2_ik = self._g2_ik           # Geometry 2 of link ik (horizontal)
         _g3_ik = self._g3_ik           # Geometry 3 of link ik (other)
+        _g4_ik = self._g4_ik           # Geometry 4 of link ik (other)
+        _g5_ik = self._g5_ik           # Geometry 5 of link ik (other)
+        _g6_ik = self._g6_ik           # Geometry 6 of link ik (other)
+        _g7_ik = self._g7_ik           # Geometry 7 of link ik (other)        
         _z_inv_uk = self._z_inv_uk     # Invert offset of upstream end of superlink k
         _J_uk = self._J_uk             # Index of junction upstream of superlink k
         H_j = self.H_j                 # Head at superjunction j
         _transect_factory = self._transect_factory
         _uk_transect_indices = self._uk_transect_indices
         _uk_has_irregular = self._uk_has_irregular
         _i_1k = self._i_1k
         _I_1k = self._I_1k
         _geom_codes = self._geom_codes
         # Compute hydraulic geometry for regular geometries
-        numba_boundary_geometry(_A_uk, _B_uk, _h_Ik, H_j, _z_inv_uk,
-                                _g1_ik, _g2_ik, _g2_ik, _geom_codes,
-                                _i_1k, _I_1k, _J_uk)
+        numba_boundary_geometry(_A_uk, _Pe_uk, _R_uk, _B_uk, _h_Ik, H_j, _z_inv_uk,
+                                _g1_ik, _g2_ik, _g3_ik, _g4_ik, _g5_ik, _g6_ik, _g7_ik,
+                                _geom_codes, _i_1k, _I_1k, _J_uk)
         # Compute hydraulic geometry for irregular geometries
         if _uk_has_irregular:
             for transect_name, generator in _transect_factory.items():
                 _ik_g = _uk_transect_indices.loc[[transect_name]].values
                 _ki_g = _ki[_ik_g]
                 _Ik_g = _Ik[_ik_g]
                 _h_Ik_g = _h_Ik[_Ik_g]
@@ -460,31 +472,37 @@
         # Import instance variables
         _ik = self._ik                 # Link index
         _Ip1k = self._Ip1k             # Next junction index
         _ki = self._ki                 # Superlink index containing link ik
         _h_Ik = self._h_Ik             # Depth at junction Ik
         _A_dk = self._A_dk             # Flow area at downstream end of superlink k
         _B_dk = self._B_dk             # Top width at downstream end of superlink k
+        _Pe_dk = self._Pe_dk
+        _R_dk = self._R_dk
         _dx_ik = self._dx_ik           # Length of link ik
         _g1_ik = self._g1_ik           # Geometry 1 of link ik (vertical)
         _g2_ik = self._g2_ik           # Geometry 2 of link ik (horizontal)
         _g3_ik = self._g3_ik           # Geometry 3 of link ik (other)
+        _g4_ik = self._g4_ik           # Geometry 4 of link ik (other)
+        _g5_ik = self._g5_ik           # Geometry 5 of link ik (other)
+        _g6_ik = self._g6_ik           # Geometry 6 of link ik (other)
+        _g7_ik = self._g7_ik           # Geometry 7 of link ik (other)        
         _z_inv_dk = self._z_inv_dk     # Invert offset of downstream end of superlink k
         _J_dk = self._J_dk             # Index of junction downstream of superlink k
         H_j = self.H_j                 # Head at superjunction j
         _transect_factory = self._transect_factory
         _dk_transect_indices = self._dk_transect_indices
         _dk_has_irregular = self._dk_has_irregular
         _i_nk = self._i_nk
         _I_Np1k = self._I_Np1k
         _geom_codes = self._geom_codes
         # Compute hydraulic geometry for regular geometries
-        numba_boundary_geometry(_A_dk, _B_dk, _h_Ik, H_j, _z_inv_dk,
-                                _g1_ik, _g2_ik, _g2_ik, _geom_codes,
-                                _i_nk, _I_Np1k, _J_dk)
+        numba_boundary_geometry(_A_dk, _Pe_dk, _R_dk, _B_dk, _h_Ik, H_j, _z_inv_dk,
+                                _g1_ik, _g2_ik, _g3_ik, _g4_ik, _g5_ik, _g6_ik, _g7_ik,
+                                _geom_codes, _i_nk, _I_Np1k, _J_dk)
         # Compute hydraulic geometry for irregular geometries
         if _dk_has_irregular:
             for transect_name, generator in _transect_factory.items():
                 _ik_g = _dk_transect_indices.loc[[transect_name]].values
                 _ki_g = _ki[_ik_g]
                 _Ip1k_g = _Ip1k[_ik_g]
                 _h_Ip1k_g = _h_Ik[_Ip1k_g]
@@ -514,15 +532,15 @@
         _z_inv_j = self._z_inv_j
         # Compute effective head
         H_uo = H_j[_J_uo]
         H_do = H_j[_J_do]
         _z_inv_uo = _z_inv_j[_J_uo]
         h_e = np.maximum(H_uo - _z_inv_uo - _z_o, H_do - _z_inv_uo - _z_o)
         if u is None:
-            u = np.zeros(n_o, dtype=float)
+            u = np.zeros(n_o, dtype=np.float64)
         # Compute orifice geometries
         numba_orifice_geometry(_Ao, h_e, u, _g1_o, _g2_o, _g3_o, _geom_codes_o, n_o)
         # Export to instance variables
         self._Ao = _Ao
 
     def compute_storage_areas(self):
         """
@@ -587,73 +605,73 @@
         """
         Compute link momentum coefficients: a_ik, b_ik, c_ik and P_ik.
         """
         # Import instance variables
         _u_Ik = self._u_Ik         # Flow velocity at junction Ik
         _u_Ip1k = self._u_Ip1k     # Flow velocity at junction I + 1k
         _dx_ik = self._dx_ik       # Length of link ik
+        _Sf_method_ik = self._Sf_method_ik
         _n_ik = self._n_ik         # Manning's roughness of link ik
-        _Q_ik = self._Q_ik         # Flow rate at link ik
+        _Q_ik_prev = np.copy(self.states['Q_ik'])
+        _Q_ik_next = self._Q_ik         # Flow rate at link ik
         _A_ik = self._A_ik         # Flow area at link ik
         _R_ik = self._R_ik         # Hydraulic radius at link ik
         _S_o_ik = self._S_o_ik     # Channel bottom slope at link ik
         _A_c_ik = self._A_c_ik     # Area of control structure at link ik
         _C_ik = self._C_ik         # Discharge coefficient of control structure at link ik
         _ctrl = self._ctrl         # Control structure exists at link ik (y/n)
         inertial_damping = self.inertial_damping    # Use inertial damping (y/n)
+        _sigma_ik = self._sigma_ik  # Inertial damping coefficient
         g = 9.81
-        # If using inertial damping, import coefficient
-        if inertial_damping:
-            _sigma_ik = self._sigma_ik
-        # Otherwise, set coefficient to unity
-        else:
-            _sigma_ik = 1
         # If time step not specified, use instance time
         if _dt is None:
             _dt = self._dt
         # Compute link coefficients
         _a_ik = numba_a_ik(_u_Ik, _sigma_ik)
         _c_ik = numba_c_ik(_u_Ip1k, _sigma_ik)
-        _b_ik = numba_b_ik(_dx_ik, _dt, _n_ik, _Q_ik, _A_ik, _R_ik,
-                           _A_c_ik, _C_ik, _a_ik, _c_ik, _ctrl, _sigma_ik)
-        if first_iter:
-            _P_ik = numba_P_ik(_Q_ik, _dx_ik, _dt, _A_ik, _S_o_ik,
-                            _sigma_ik)
+        _b_ik = numba_b_ik(_dx_ik, _dt, _n_ik, _Q_ik_next, _A_ik, _R_ik, _A_c_ik,
+                           _C_ik, _a_ik, _c_ik, _ctrl, _sigma_ik, _Sf_method_ik, g)
+        _P_ik = numba_P_ik(_Q_ik_prev, _dx_ik, _dt, _A_ik, _S_o_ik,
+                           _sigma_ik, g)
         # Export to instance variables
         self._a_ik = _a_ik
         self._b_ik = _b_ik
         self._c_ik = _c_ik
-        if first_iter:
-            self._P_ik = _P_ik
+        self._P_ik = _P_ik
 
     def node_coeffs(self, _Q_0Ik=None, _dt=None, first_iter=True):
         """
         Compute nodal continuity coefficients: D_Ik and E_Ik.
         """
         # Import instance variables
         forward_I_i = self.forward_I_i       # Index of link after junction Ik
         backward_I_i = self.backward_I_i     # Index of link before junction Ik
         _is_start = self._is_start
         _is_end = self._is_end
         _B_ik = self._B_ik                   # Top width of link ik
         _dx_ik = self._dx_ik                 # Length of link ik
         _A_SIk = self._A_SIk                 # Surface area of junction Ik
-        _h_Ik = self._h_Ik                   # Depth at junction Ik
+        _h_Ik_prev = np.copy(self.states['h_Ik'])         # Depth at junction Ik
         _E_Ik = self._E_Ik                   # Continuity coefficient E_Ik
         _D_Ik = self._D_Ik                   # Continuity coefficient D_Ik
+        _B_uk = self._B_uk
+        _B_dk = self._B_dk
+        _dx_uk = self._dx_uk
+        _dx_dk = self._dx_dk
+        _kI = self._kI
         # If no time step specified, use instance time step
         if _dt is None:
             _dt = self._dt
         # If no nodal input specified, use zero input
         if _Q_0Ik is None:
-            _Q_0Ik = np.zeros(_h_Ik.size)
+            _Q_0Ik = np.zeros(_h_Ik_prev.size)
         # Compute E_Ik and D_Ik
-        numba_node_coeffs(_D_Ik, _E_Ik, _Q_0Ik, _B_ik, _h_Ik, _dx_ik, _A_SIk,
-                          _dt, forward_I_i, backward_I_i, _is_start, _is_end,
-                          first_iter)
+        numba_node_coeffs(_D_Ik, _E_Ik, _Q_0Ik, _B_ik, _h_Ik_prev, _dx_ik, _A_SIk,
+                          _B_uk, _B_dk, _dx_uk, _dx_dk, _kI,
+                          _dt, forward_I_i, backward_I_i, _is_start, _is_end)
         # Export instance variables
         self._E_Ik = _E_Ik
         self._D_Ik = _D_Ik
 
     def forward_recurrence(self):
         """
         Compute forward recurrence coefficients: T_ik, U_Ik, V_Ik, and W_Ik.
@@ -705,15 +723,15 @@
                                     _P_ik, _A_ik, _E_Ik, _D_Ik, NK, nk, _I_Nk, _i_nk)
         # Export instance variables
         self._O_ik = _O_ik
         self._X_Ik = _X_Ik
         self._Y_Ik = _Y_Ik
         self._Z_Ik = _Z_Ik
 
-    def superlink_upstream_head_coefficients(self):
+    def superlink_upstream_head_coefficients(self, _dt=None):
         """
         Compute upstream head coefficients for superlinks: kappa_uk, lambda_uk, and mu_uk.
         """
         # Import instance variables
         _I_1k = self._I_1k             # Index of first junction in superlink k
         _i_1k = self._i_1k             # Index of first link in superlink k
         _h_Ik = self._h_Ik             # Depth at junction Ik
@@ -722,42 +740,53 @@
         _A_ik = self._A_ik             # Flow area of link ik
         _B_ik = self._B_ik             # Top width of link ik
         _Q_ik = self._Q_ik             # Flow rate of link ik
         _bc_method = self._bc_method   # Method for computing superlink boundary condition (j/z)
         H_j = self.H_j                 # Head at superjunction j
         _A_uk = self._A_uk             # Flow area at upstream end of superlink k
         _B_uk = self._B_uk             # Top width at upstream end of superlink k
+        _R_uk = self._R_uk
+        _dx_uk = self._dx_uk
+        _S_o_uk = self._S_o_uk
+        _theta_uk = self._theta_uk
         # Placeholder discharge coefficient
         _C_uk = self._C_uk
         # Current upstream flows
-        _Q_uk_t = self._Q_uk
+        _Q_uk_next = self._Q_uk
+        _Q_uk_prev = np.copy(self.states['Q_uk'])
+        # Friction parameters
+        _n_uk = self._n_uk
+        _Sf_method_uk = self._Sf_method_uk
+        g = 9.81
+        # If time step not specified, use instance time
+        if _dt is None:
+            _dt = self._dt
+        # Compute theta indicator variables
+        _H_juk = H_j[_J_uk]
+        upstream_depth_above_invert = _H_juk >= _z_inv_uk
+        _theta_uk.fill(0.)
+        _theta_uk[upstream_depth_above_invert] = 1.
         if _bc_method == 'z':
             # Compute superlink upstream coefficients (Zahner)
-            _gamma_uk = gamma_uk(_Q_uk_t, _C_uk, _A_uk)
+            _gamma_uk = gamma_uk(_Q_uk_next, _C_uk, _A_uk, g)
             self._kappa_uk = _gamma_uk
-            self._lambda_uk = 1
-            self._mu_uk = - _z_inv_uk
-        elif _bc_method == 'j':
-            # Current upstream depth
-            _h_uk = _h_Ik[_I_1k]
-            # Junction head
-            _H_juk = H_j[_J_uk]
-            # Head difference
-            _dH_uk = _H_juk - _h_uk - _z_inv_uk
-            # Compute superlink upstream coefficients (Ji)
-            _kappa_uk = self.kappa_uk(_A_uk, _dH_uk, _Q_uk_t, _B_uk)
-            _lambda_uk = self.lambda_uk(_A_uk, _dH_uk, _B_uk)
-            _mu_uk = self.mu_uk(_A_uk, _dH_uk, _B_uk, _z_inv_uk)
-            self._kappa_uk = _kappa_uk
-            self._lambda_uk = _lambda_uk
-            self._mu_uk = _mu_uk
+            self._lambda_uk = _theta_uk
+            self._mu_uk = - _theta_uk * _z_inv_uk
+        elif _bc_method == 'b':
+            # Compute superlink upstream coefficients (momentum)
+            self._kappa_uk = kappa_uk(_Q_uk_next, _dx_uk, _A_uk, _C_uk,
+                                      _R_uk, _n_uk, _Sf_method_uk, _dt, g)
+            self._lambda_uk = _theta_uk
+            self._mu_uk = mu_uk(_Q_uk_prev, _dx_uk, _A_uk, _theta_uk, _z_inv_uk,
+                                _S_o_uk, _dt, g)
         else:
             raise ValueError('Invalid BC method {}.'.format(_bc_method))
+        self._theta_uk = _theta_uk
 
-    def superlink_downstream_head_coefficients(self):
+    def superlink_downstream_head_coefficients(self, _dt=None):
         """
         Compute downstream head coefficients for superlinks: kappa_dk, lambda_dk, and mu_dk.
         """
         # Import instance variables
         _I_Np1k = self._I_Np1k         # Index of last junction in superlink k
         _i_nk = self._i_nk             # Index of last link in superlink k
         _h_Ik = self._h_Ik             # Depth at junction Ik
@@ -766,41 +795,49 @@
         _A_ik = self._A_ik             # Flow area of link ik
         _B_ik = self._B_ik             # Top width of link ik
         _Q_ik = self._Q_ik             # Flow rate of link ik
         _bc_method = self._bc_method   # Method for computing superlink boundary condition (j/z)
         H_j = self.H_j                 # Head at superjunction j
         _A_dk = self._A_dk             # Flow area at downstream end of superlink k
         _B_dk = self._B_dk             # Top width at downstream end of superlink k
+        _R_dk = self._R_dk
+        _dx_dk = self._dx_dk
+        _S_o_dk = self._S_o_dk
+        _theta_dk = self._theta_dk
         # Placeholder discharge coefficient
         _C_dk = self._C_dk
         # Current downstream flows
-        _Q_dk_t = self._Q_dk
+        _Q_dk_next = self._Q_dk
+        _Q_dk_prev = np.copy(self.states['Q_dk'])
+        # Friction parameters
+        _n_dk = self._n_dk
+        _Sf_method_dk = self._Sf_method_dk
+        g = 9.81
+        if _dt is None:
+            _dt = self._dt
+        # Compute theta indicator variables
+        _H_jdk = H_j[_J_dk]
+        downstream_depth_above_invert = _H_jdk >= _z_inv_dk
+        _theta_dk.fill(0.)
+        _theta_dk[downstream_depth_above_invert] = 1.
         if _bc_method == 'z':
             # Compute superlink downstream coefficients (Zahner)
-            _gamma_dk = gamma_dk(_Q_dk_t, _C_dk, _A_dk)
+            _gamma_dk = gamma_dk(_Q_dk_next, _C_dk, _A_dk, g)
             self._kappa_dk = _gamma_dk
-            self._lambda_dk = 1
-            self._mu_dk = - _z_inv_dk
-        elif _bc_method == 'j':
-            # Downstream top width
-            # Current downstream depth
-            _h_dk = _h_Ik[_I_Np1k]
-            # Junction head
-            _H_jdk = H_j[_J_dk]
-            # Head difference
-            _dH_dk = _h_dk + _z_inv_dk - _H_jdk
-            # Compute superlink upstream coefficients (Ji)
-            _kappa_dk = self.kappa_dk(_A_dk, _dH_dk, _Q_dk_t, _B_dk)
-            _lambda_dk = self.lambda_dk(_A_dk, _dH_dk, _B_dk)
-            _mu_dk = self.mu_dk(_A_dk, _dH_dk, _B_dk, _z_inv_dk)
-            self._kappa_dk = _kappa_dk
-            self._lambda_dk = _lambda_dk
-            self._mu_dk = _mu_dk
+            self._lambda_dk = _theta_dk
+            self._mu_dk = - _theta_dk * _z_inv_dk
+        elif _bc_method == 'b':
+            # Compute superlink upstream coefficients (momentum)
+            self._kappa_dk = kappa_dk(_Q_dk_next, _dx_dk, _A_dk, _C_dk,
+                                      _R_dk, _n_dk, _Sf_method_dk, _dt, g)
+            self._lambda_dk = _theta_dk
+            self._mu_dk = mu_dk(_Q_dk_prev, _dx_dk, _A_dk, _theta_dk, _z_inv_dk, _S_o_dk, _dt, g)
         else:
             raise ValueError('Invalid BC method {}.'.format(_bc_method))
+        self._theta_dk = _theta_dk
 
     def superlink_flow_coefficients(self):
         """
         Compute superlink flow coefficients: alpha_uk, beta_uk, chi_uk,
         alpha_dk, beta_dk, chi_dk.
         """
         # Import instance variables
@@ -840,54 +877,45 @@
         else:
             _X_1k = _X_Ik[_I_1k] + _E_Ik[_I_1k]
             _Y_1k = _Y_Ik[_I_1k] - _D_Ik[_I_1k]
             _Z_1k = _Z_Ik[_I_1k]
             _U_Nk = _U_Ik[_I_Nk] - _E_Ik[_I_Np1k]
             _V_Nk = _V_Ik[_I_Nk] + _D_Ik[_I_Np1k]
             _W_Nk = _W_Ik[_I_Nk]
-        # Compute theta indicator variables
-        _H_juk = H_j[_J_uk]
-        _H_jdk = H_j[_J_dk]
-        _theta_uk = np.where(_H_juk >= _z_inv_uk, 1.0, 0.0)
-        _theta_dk = np.where(_H_jdk >= _z_inv_dk, 1.0, 0.0)
-        # _theta_uk = 1.
-        # _theta_dk = 1.
         # Compute D_k_star
         _D_k_star = numba_D_k_star(_X_1k, _kappa_uk, _U_Nk,
                                    _kappa_dk, _Z_1k, _W_Nk)
         # Compute upstream superlink flow coefficients
         _alpha_uk = numba_alpha_uk(_U_Nk, _kappa_dk, _X_1k,
                                    _Z_1k, _W_Nk, _D_k_star,
-                                   _lambda_uk, _theta_uk)
+                                   _lambda_uk)
         _beta_uk = numba_beta_uk(_U_Nk, _kappa_dk, _Z_1k,
-                                 _W_Nk, _D_k_star, _lambda_dk, _theta_dk)
+                                 _W_Nk, _D_k_star, _lambda_dk)
         _chi_uk = numba_chi_uk(_U_Nk, _kappa_dk, _Y_1k,
                                _X_1k, _mu_uk, _Z_1k,
                                _mu_dk, _V_Nk, _W_Nk,
-                               _D_k_star, _theta_uk, _theta_dk)
+                               _D_k_star)
         # Compute downstream superlink flow coefficients
         _alpha_dk = numba_alpha_dk(_X_1k, _kappa_uk, _W_Nk,
-                                   _D_k_star, _lambda_uk, _theta_uk)
+                                   _D_k_star, _lambda_uk)
         _beta_dk = numba_beta_dk(_X_1k, _kappa_uk, _U_Nk,
                                  _W_Nk, _Z_1k, _D_k_star,
-                                 _lambda_dk, _theta_dk)
+                                 _lambda_dk)
         _chi_dk = numba_chi_dk(_X_1k, _kappa_uk, _V_Nk,
                                _W_Nk, _mu_uk, _U_Nk,
                                _mu_dk, _Y_1k, _Z_1k,
-                               _D_k_star, _theta_uk, _theta_dk)
+                               _D_k_star)
         # Export instance variables
         self._D_k_star = _D_k_star
         self._alpha_uk = _alpha_uk
         self._beta_uk = _beta_uk
         self._chi_uk = _chi_uk
         self._alpha_dk = _alpha_dk
         self._beta_dk = _beta_dk
         self._chi_dk = _chi_dk
-        self._theta_uk = _theta_uk
-        self._theta_dk = _theta_dk
 
     def orifice_flow_coefficients(self, u=None):
         """
         Compute orifice flow coefficients: alpha_uo, beta_uo, chi_uo,
         alpha_do, beta_do, chi_do.
         """
         # Import instance variables
@@ -902,15 +930,15 @@
         _Co = self._Co               # Discharge coefficient of orifice o
         _Ao = self._Ao               # Maximum flow area of orifice o
         _alpha_o = self._alpha_o     # Orifice flow coefficient alpha_o
         _beta_o = self._beta_o       # Orifice flow coefficient beta_o
         _chi_o = self._chi_o         # Orifice flow coefficient chi_o
         # If no input signal, assume orifice is closed
         if u is None:
-            u = np.zeros(self.n_o, dtype=float)
+            u = np.zeros(self.n_o, dtype=np.float64)
         # Specify orifice heads at previous timestep
         numba_orifice_flow_coefficients(_alpha_o, _beta_o, _chi_o, H_j, _Qo, u, _z_inv_j,
                                         _z_o, _tau_o, _Co, _Ao, _y_max_o, _J_uo, _J_do)
         # Export instance variables
         self._alpha_o = _alpha_o
         self._beta_o = _beta_o
         self._chi_o = _chi_o
@@ -934,15 +962,15 @@
         _L_w = self._L_w           # Transverse length of rectangular section
         _alpha_w = self._alpha_w   # Weir flow coefficient alpha_w
         _beta_w = self._beta_w     # Weir flow coefficient beta_w
         _chi_w = self._chi_w       # Weir flow coefficient chi_w
         _Hw = self._Hw             # Current effective head above weir w
         # If no input signal, assume weir is closed
         if u is None:
-            u = np.zeros(self.n_w, dtype=float)
+            u = np.zeros(self.n_w, dtype=np.float64)
         # Compute weir flow coefficients
         numba_weir_flow_coefficients(_Hw, _Qw, _alpha_w, _beta_w, _chi_w, H_j, _z_inv_j, _z_w,
                                      _y_max_w, u, _L_w, _s_w, _Cwr, _Cwt, _J_uw, _J_dw)
         # Export instance variables
         self._alpha_w = _alpha_w
         self._beta_w = _beta_w
         self._chi_w = _chi_w
@@ -956,28 +984,29 @@
         H_j = self.H_j              # Head at superjunction j
         _z_inv_j = self._z_inv_j    # Invert elevation at superjunction j
         _J_up = self._J_up          # Index of superjunction upstream of pump p
         _J_dp = self._J_dp          # Index of superjunction downstream of pump p
         _z_p = self._z_p            # Offset of pump inlet above upstream invert elevation
         _dHp_max = self._dHp_max    # Maximum pump head difference
         _dHp_min = self._dHp_min    # Minimum pump head difference
-        _ap_h = self._ap_h          # Horizontal axis length of elliptical pump curve
-        _ap_q = self._ap_q          # Vertical axis length of elliptical pump curve
+        _a_p = self._a_p            # Pump curve parameter `a`
+        _b_p = self._b_p            # Pump curve parameter `b`
+        _c_p = self._c_p            # Pump curve parameter `c`
         _Qp = self._Qp              # Current flow rate through pump p
         _alpha_p = self._alpha_p    # Pump flow coefficient alpha_p
         _beta_p = self._beta_p      # Pump flow coefficient beta_p
         _chi_p = self._chi_p        # Pump flow coefficient chi_p
         # If no input signal, assume pump is closed
         if u is None:
-            u = np.zeros(self.n_p, dtype=float)
+            u = np.zeros(self.n_p, dtype=np.float64)
         # Check max/min head differences
         assert (_dHp_min <= _dHp_max).all()
         # Compute pump flow coefficients
         numba_pump_flow_coefficients(_alpha_p, _beta_p, _chi_p, H_j, _z_inv_j, _Qp, u,
-                                     _z_p, _dHp_max, _dHp_min, _ap_q, _ap_h, _J_up, _J_dp)
+                                     _z_p, _dHp_max, _dHp_min, _a_p, _b_p, _c_p, _J_up, _J_dp)
         # Export instance variables
         self._alpha_p = _alpha_p
         self._beta_p = _beta_p
         self._chi_p = _chi_p
 
     def sparse_matrix_equations(self, H_bc=None, _Q_0j=None, u=None, _dt=None, implicit=True,
                                 first_time=False):
@@ -996,14 +1025,20 @@
         _chi_dk = self._chi_dk           # Superlink flow coefficient
         _alpha_ukm = self._alpha_ukm     # Summation of superlink flow coefficients
         _beta_dkl = self._beta_dkl       # Summation of superlink flow coefficients
         _chi_ukl = self._chi_ukl         # Summation of superlink flow coefficients
         _chi_dkm = self._chi_dkm         # Summation of superlink flow coefficients
         _F_jj = self._F_jj
         _A_sj = self._A_sj               # Surface area of superjunction j
+        _dx_uk = self._dx_uk
+        _dx_dk = self._dx_dk
+        _B_uk = self._B_uk
+        _B_dk = self._B_dk
+        _theta_uk = self._theta_uk
+        _theta_dk = self._theta_dk
         NK = self.NK
         n_o = self.n_o                   # Number of orifices in system
         n_w = self.n_w                   # Number of weirs in system
         n_p = self.n_p                   # Number of pumps in system
         A = self.A
         if n_o:
             O = self.O
@@ -1039,41 +1074,47 @@
             _alpha_upm = self._alpha_upm     # Summation of pump flow coefficients
             _beta_dpl = self._beta_dpl       # Summation of pump flow coefficients
             _chi_upl = self._chi_upl         # Summation of pump flow coefficients
             _chi_dpm = self._chi_dpm         # Summation of pump flow coefficients
             _P_diag = self._P_diag           # Diagonal elements of matrix P
         _sparse = self._sparse           # Use sparse matrix data structures (y/n)
         M = self.M                       # Number of superjunctions in system
-        H_j = self.H_j                   # Head at superjunction j
+        H_j_next = self.H_j                   # Head at superjunction j
+        H_j_prev = self.states['H_j']
         bc = self.bc                     # Superjunction j has a fixed boundary condition (y/n)
         D = self.D                       # Vector for storing chi coefficients
         b = self.b                       # Right-hand side vector
         # If no time step specified, use instance time step
         if _dt is None:
             _dt = self._dt
         # If no boundary head specified, use current superjunction head
         if H_bc is None:
-            H_bc = self.H_j
+            H_bc = H_j_next
         # If no flow input specified, assume zero external inflow
         if _Q_0j is None:
             _Q_0j = 0
         # If no control input signal specified assume zero input
         if u is None:
             u = 0
+        # Compute upstream/downstream link volume parameters
+        _xi_uk = xi_uk(_dx_uk, _B_uk, _theta_uk, _dt)
+        _xi_dk = xi_dk(_dx_dk, _B_dk, _theta_dk, _dt)
         # Clear old data
         _F_jj.fill(0)
         D.fill(0)
         numba_clear_off_diagonals(A, bc, _J_uk, _J_dk, NK)
         # Create A matrix
         numba_create_A_matrix(A, _F_jj, bc, _J_uk, _J_dk, _alpha_uk,
-                              _alpha_dk, _beta_uk, _beta_dk, _A_sj, _dt,
-                              M, NK)
+                              _alpha_dk, _beta_uk, _beta_dk, _xi_uk, _xi_dk,
+                              _A_sj, _dt, M, NK)
         # Create D vector
         numba_add_at(D, _J_uk, -_chi_uk)
         numba_add_at(D, _J_dk, _chi_dk)
+        numba_add_at(D, _J_uk, _xi_uk * H_j_prev[_J_uk])
+        numba_add_at(D, _J_dk, _xi_dk * H_j_prev[_J_dk])
         # Compute control matrix
         if n_o:
             _alpha_uo = _alpha_o
             _alpha_do = _alpha_o
             _beta_uo = _beta_o
             _beta_do = _beta_o
             _chi_uo = _chi_o
@@ -1113,15 +1154,16 @@
             # Set diagonal
             numba_create_OWP_matrix(P, _P_diag, bc, _J_up, _J_dp, _alpha_up,
                                     _alpha_dp, _beta_up, _beta_dp, M, n_p)
             # Set right-hand side
             numba_add_at(D, _J_up, -_chi_up)
             numba_add_at(D, _J_dp, _chi_dp)
         b.fill(0)
-        b = (_A_sj * H_j / _dt) + _Q_0j + D
+        # TODO: Which A_sj? Might need to apply product rule here.
+        b = (_A_sj * H_j_prev / _dt) + _Q_0j + D
         # Ensure boundary condition is specified
         b[bc] = H_bc[bc]
         # Export instance variables
         self.D = D
         self.b = b
         # self._beta_dkl = _beta_dkl
         # self._alpha_ukm = _alpha_ukm
@@ -1378,20 +1420,21 @@
         _J_do = self._J_do            # Index of superjunction downstream of orifice o
         _z_o = self._z_o              # Offset of orifice above upstream invert elevation
         _tau_o = self._tau_o          # Orientation of orifice o (bottom/side)
         _y_max_o = self._y_max_o      # Maximum height of orifice o
         _Co = self._Co                # Discharge coefficient of orifice o
         _Ao = self._Ao                # Maximum flow area of orifice o
         _V_sj = self._V_sj
+        g = 9.81
         # If no input signal, assume orifice is closed
         if u is None:
-            u = np.zeros(self.n_o, dtype=float)
+            u = np.zeros(self.n_o, dtype=np.float64)
         # Compute orifice flows
         _Qo_next = numba_solve_orifice_flows(H_j, u, _z_inv_j, _z_o, _tau_o, _y_max_o, _Co, _Ao,
-                                             _J_uo, _J_do)
+                                             _J_uo, _J_do, g)
         # TODO: Move this inside numba function
         upstream_ctrl = (H_j[_J_uo] > H_j[_J_do])
         _Qo_max = np.where(upstream_ctrl, _V_sj[_J_uo], _V_sj[_J_do]) / dt
         _Qo_next = np.sign(_Qo_next) * np.minimum(np.abs(_Qo_next), _Qo_max)
         # Export instance variables
         self._Qo = _Qo_next
 
@@ -1410,15 +1453,15 @@
         _Cwr = self._Cwr            # Discharge coefficient of rectangular portion of weir w
         _Cwt = self._Cwt            # Discharge coefficient of triangular portion of weir w
         _s_w = self._s_w            # Inverse side slope of triangular portion of weir w
         _L_w = self._L_w            # Transverse length of rectangular portion of weir w
         _Hw = self._Hw              # Current effective head on weir w
         # If no input signal, assume weir is closed
         if u is None:
-            u = np.zeros(self.n_w, dtype=float)
+            u = np.zeros(self.n_w, dtype=np.float64)
         # Solve for weir flows
         _Qw_next = numba_solve_weir_flows(_Hw, _Qw, H_j, _z_inv_j, _z_w,
                                           _y_max_w, u, _L_w, _s_w, _Cwr,
                                           _Cwt, _J_uw, _J_dw)
         # Export instance variables
         self._Qw = _Qw_next
 
@@ -1430,23 +1473,24 @@
         H_j = self.H_j              # Head at superjunction j
         _z_inv_j = self._z_inv_j    # Invert elevation of superjunction j
         _J_up = self._J_up          # Index of superjunction upstream of pump p
         _J_dp = self._J_dp          # Index of superjunction downstream of pump p
         _z_p = self._z_p            # Offset of pump inlet above upstream invert
         _dHp_max = self._dHp_max    # Maximum pump head difference
         _dHp_min = self._dHp_min    # Minimum pump head difference
-        _ap_h = self._ap_h          # Horizontal axis length of elliptical pump curve
-        _ap_q = self._ap_q          # Vertical axis length of elliptical pump curve
+        _a_p = self._a_p            # Pump curve parameter `a`
+        _b_p = self._b_p            # Pump curve parameter `b`
+        _c_p = self._c_p            # Pump curve parameter `c`
         _Qp = self._Qp              # Current flow rate through pump p
         # If no input signal, assume pump is closed
         if u is None:
-            u = np.zeros(self.n_p, dtype=float)
+            u = np.zeros(self.n_p, dtype=np.float64)
         # Compute pump flows
         _Qp_next = numba_solve_pump_flows(H_j, u, _z_inv_j, _z_p, _dHp_max,
-                                          _dHp_min, _ap_q, _ap_h, _J_up, _J_dp)
+                                          _dHp_min, _a_p, _b_p, _c_p, _J_up, _J_dp)
         self._Qp = _Qp_next
 
     def compute_storage_volumes(self):
         """
         Compute storage volume of superjunctions at current time step.
         """
         # Import instance variables
@@ -1485,75 +1529,85 @@
         """
         Reposition junctions inside superlinks to enable capture of backwater effects.
         """
         # Import instance variables
         _b0 = self._b0                # Vertical coordinate of upstream end of superlink k
         _b1 = self._b1                # Vertical coordinate of downstream end of superlink k
         _m = self._m                  # Slope of superlink k
-        _x0 = self._x0                # Horizontal coordinate of center of superlink k
-        _z0 = self._z0                # Invert elevation of center of superlink k
+        _xc = self._xc                # Horizontal coordinate of center of superlink k
+        _zc = self._zc                # Invert elevation of center of superlink k
         _h_Ik = self._h_Ik            # Depth at junction Ik
         _Q_ik = self._Q_ik            # Flow rate at link ik
         _J_dk = self._J_dk            # Index of superjunction downstream of superlink k
         _x_Ik = self._x_Ik            # Horizontal coordinate of junction Ik
         _dx_ik = self._dx_ik          # Length of link ik
         _z_inv_Ik = self._z_inv_Ik    # Invert elevation of junction Ik
         _S_o_ik = self._S_o_ik        # Channel bottom slope of link ik
         _I_1k = self._I_1k            # Index of first junction in superlink k
         _I_Np1k = self._I_Np1k        # Index of last junction in superlink k
         _i_1k = self._i_1k            # Index of first link in superlink k
         H_j = self.H_j                # Head at superjunction j
         _elem_pos = self._elem_pos
         nk = self.nk
         NK = self.NK
+        # Check if possible to move elements
+        if not self.mobile_elements:
+            raise ValueError('Model must be instantiated with `mobile_elements=True` to reposition junctions.')
         # Get downstream head
         _H_dk = H_j[_J_dk]
         # Handle which superlinks to reposition
         if reposition is None:
-            reposition = np.ones(NK, dtype=bool)
+            reposition = np.ones(NK, dtype=np.bool8)
         # Reposition junctions
         numba_reposition_junctions(_x_Ik, _z_inv_Ik, _h_Ik, _dx_ik, _Q_ik, _H_dk,
-                                    _b0, _z0, _x0, _m, _elem_pos, _i_1k, _I_1k,
+                                    _b0, _zc, _xc, _m, _elem_pos, _i_1k, _I_1k,
                                     _I_Np1k, nk, NK, reposition)
 
 def handle_elliptical_perimeter(_Pe_ik, _ellipse_ix, _Ik, _Ip1k, _h_Ik, _g1_ik, _g2_ik):
     if (_ellipse_ix.size > 0):
         _ik_g = _ellipse_ix
         _Ik_g = _Ik[_ik_g]
         _Ip1k_g = _Ip1k[_ik_g]
         _Pe_ik[_ik_g] = pipedream_solver.geometry.Elliptical.Pe_ik(_h_Ik[_Ik_g],
                                                             _h_Ik[_Ip1k_g],
                                                             _g1_ik[_ik_g],
                                                             _g2_ik[_ik_g])
 
-
-@njit
+@njit(int64(float64[:], float64[:], float64[:], float64[:], float64[:],
+            float64[:], float64[:], float64[:], float64[:], float64[:], float64[:], float64[:],
+            int64[:], int64[:], int64[:]),
+      cache=True)
 def numba_hydraulic_geometry(_A_ik, _Pe_ik, _R_ik, _B_ik, _h_Ik,
-                             _g1_ik, _g2_ik, _g3_ik, _geom_codes, _Ik, _ik):
+                             _g1_ik, _g2_ik, _g3_ik, _g4_ik, _g5_ik, _g6_ik, _g7_ik,
+                             _geom_codes, _Ik, _ik):
     n = len(_ik)
     for i in range(n):
         I = _Ik[i]
         Ip1 = I + 1
         geom_code = _geom_codes[i]
         h_I = _h_Ik[I]
         h_Ip1 = _h_Ik[Ip1]
         g1_i = _g1_ik[i]
         g2_i = _g2_ik[i]
         g3_i = _g3_ik[i]
+        g4_i = _g4_ik[i]
+        g5_i = _g5_ik[i]
+        g6_i = _g6_ik[i]
+        g7_i = _g7_ik[i]
         if geom_code:
             if geom_code == 1:
                 _A_ik[i] = pipedream_solver.ngeometry.Circular_A_ik(h_I, h_Ip1, g1_i)
                 _Pe_ik[i] = pipedream_solver.ngeometry.Circular_Pe_ik(h_I, h_Ip1, g1_i)
                 _R_ik[i] = pipedream_solver.ngeometry.Circular_R_ik(_A_ik[i], _Pe_ik[i])
-                _B_ik[i] = pipedream_solver.ngeometry.Circular_B_ik(h_I, h_Ip1, g1_i)
+                _B_ik[i] = pipedream_solver.ngeometry.Circular_B_ik(h_I, h_Ip1, g1_i, g2_i)
             elif geom_code == 2:
                 _A_ik[i] = pipedream_solver.ngeometry.Rect_Closed_A_ik(h_I, h_Ip1, g1_i, g2_i)
                 _Pe_ik[i] = pipedream_solver.ngeometry.Rect_Closed_Pe_ik(h_I, h_Ip1, g1_i, g2_i)
                 _R_ik[i] = pipedream_solver.ngeometry.Rect_Closed_R_ik(_A_ik[i], _Pe_ik[i])
-                _B_ik[i] = pipedream_solver.ngeometry.Rect_Closed_B_ik(h_I, h_Ip1, g1_i, g2_i)
+                _B_ik[i] = pipedream_solver.ngeometry.Rect_Closed_B_ik(h_I, h_Ip1, g1_i, g2_i, g3_i)
             elif geom_code == 3:
                 _A_ik[i] = pipedream_solver.ngeometry.Rect_Open_A_ik(h_I, h_Ip1, g1_i, g2_i)
                 _Pe_ik[i] = pipedream_solver.ngeometry.Rect_Open_Pe_ik(h_I, h_Ip1, g1_i, g2_i)
                 _R_ik[i] = pipedream_solver.ngeometry.Rect_Open_R_ik(_A_ik[i], _Pe_ik[i])
                 _B_ik[i] = pipedream_solver.ngeometry.Rect_Open_B_ik(h_I, h_Ip1, g1_i, g2_i)
             elif geom_code == 4:
                 _A_ik[i] = pipedream_solver.ngeometry.Triangular_A_ik(h_I, h_Ip1, g1_i, g2_i)
@@ -1581,63 +1635,99 @@
                 _R_ik[i] = pipedream_solver.ngeometry.Wide_R_ik(_A_ik[i], _Pe_ik[i])
                 _B_ik[i] = pipedream_solver.ngeometry.Wide_B_ik(h_I, h_Ip1, g1_i, g2_i)
             elif geom_code == 9:
                 _A_ik[i] = pipedream_solver.ngeometry.Force_Main_A_ik(h_I, h_Ip1, g1_i, g2_i)
                 _Pe_ik[i] = pipedream_solver.ngeometry.Force_Main_Pe_ik(h_I, h_Ip1, g1_i, g2_i)
                 _R_ik[i] = pipedream_solver.ngeometry.Force_Main_R_ik(_A_ik[i], _Pe_ik[i])
                 _B_ik[i] = pipedream_solver.ngeometry.Force_Main_B_ik(h_I, h_Ip1, g1_i, g2_i)
+            elif geom_code == 10:
+                _A_ik[i] = pipedream_solver.ngeometry.Floodplain_A_ik(h_I, h_Ip1, g1_i, g2_i, g3_i, g4_i, g5_i, g6_i, g7_i)
+                _Pe_ik[i] = pipedream_solver.ngeometry.Floodplain_Pe_ik(h_I, h_Ip1, g1_i, g2_i, g3_i, g4_i, g5_i, g6_i, g7_i)
+                _R_ik[i] = pipedream_solver.ngeometry.Floodplain_R_ik(_A_ik[i], _Pe_ik[i])
+                _B_ik[i] = pipedream_solver.ngeometry.Floodplain_B_ik(h_I, h_Ip1, g1_i, g2_i, g3_i, g4_i, g5_i, g6_i, g7_i)
     return 1
 
-@njit
-def numba_boundary_geometry(_A_bk, _B_bk, _h_Ik, _H_j, _z_inv_bk,
-                            _g1_ik, _g2_ik, _g3_ik, _geom_codes,
-                            _i_bk, _I_bk, _J_bk):
+@njit(int64(float64[:], float64[:], float64[:], float64[:], float64[:], float64[:], float64[:],
+            float64[:], float64[:], float64[:], float64[:], float64[:], float64[:], float64[:],
+            int64[:], int64[:], int64[:], int64[:]),
+      cache=True)
+def numba_boundary_geometry(_A_bk, _Pe_bk, _R_bk, _B_bk, _h_Ik, _H_j, _z_inv_bk,
+                            _g1_ik, _g2_ik, _g3_ik, _g4_ik, _g5_ik, _g6_ik, _g7_ik,
+                            _geom_codes, _i_bk, _I_bk, _J_bk):
     n = len(_i_bk)
     for k in range(n):
         i = _i_bk[k]
         I = _I_bk[k]
         j = _J_bk[k]
         # TODO: does not handle "max" mode
         h_I = _h_Ik[I]
         h_Ip1 = _H_j[j] - _z_inv_bk[k]
         geom_code = _geom_codes[i]
         g1_i = _g1_ik[i]
         g2_i = _g2_ik[i]
         g3_i = _g3_ik[i]
+        g4_i = _g4_ik[i]
+        g5_i = _g5_ik[i]
+        g6_i = _g6_ik[i]
+        g7_i = _g7_ik[i]
         if geom_code:
             if geom_code == 1:
                 _A_bk[k] = pipedream_solver.ngeometry.Circular_A_ik(h_I, h_Ip1, g1_i)
-                _B_bk[k] = pipedream_solver.ngeometry.Circular_B_ik(h_I, h_Ip1, g1_i)
+                _Pe_bk[k] = pipedream_solver.ngeometry.Circular_Pe_ik(h_I, h_Ip1, g1_i)
+                _R_bk[k] = pipedream_solver.ngeometry.Circular_R_ik(_A_bk[k], _Pe_bk[k])
+                _B_bk[k] = pipedream_solver.ngeometry.Circular_B_ik(h_I, h_Ip1, g1_i, g2_i)
             elif geom_code == 2:
                 _A_bk[k] = pipedream_solver.ngeometry.Rect_Closed_A_ik(h_I, h_Ip1, g1_i, g2_i)
-                _B_bk[k] = pipedream_solver.ngeometry.Rect_Closed_B_ik(h_I, h_Ip1, g1_i, g2_i)
+                _Pe_bk[k] = pipedream_solver.ngeometry.Rect_Closed_Pe_ik(h_I, h_Ip1, g1_i, g2_i)
+                _R_bk[k] = pipedream_solver.ngeometry.Rect_Closed_R_ik(_A_bk[k], _Pe_bk[k])
+                _B_bk[k] = pipedream_solver.ngeometry.Rect_Closed_B_ik(h_I, h_Ip1, g1_i, g2_i, g3_i)
             elif geom_code == 3:
                 _A_bk[k] = pipedream_solver.ngeometry.Rect_Open_A_ik(h_I, h_Ip1, g1_i, g2_i)
+                _Pe_bk[k] = pipedream_solver.ngeometry.Rect_Open_Pe_ik(h_I, h_Ip1, g1_i, g2_i)
+                _R_bk[k] = pipedream_solver.ngeometry.Rect_Open_R_ik(_A_bk[k], _Pe_bk[k])
                 _B_bk[k] = pipedream_solver.ngeometry.Rect_Open_B_ik(h_I, h_Ip1, g1_i, g2_i)
             elif geom_code == 4:
                 _A_bk[k] = pipedream_solver.ngeometry.Triangular_A_ik(h_I, h_Ip1, g1_i, g2_i)
+                _Pe_bk[k] = pipedream_solver.ngeometry.Triangular_Pe_ik(h_I, h_Ip1, g1_i, g2_i)
+                _R_bk[k] = pipedream_solver.ngeometry.Triangular_R_ik(_A_bk[k], _Pe_bk[k])
                 _B_bk[k] = pipedream_solver.ngeometry.Triangular_B_ik(h_I, h_Ip1, g1_i, g2_i)
             elif geom_code == 5:
                 _A_bk[k] = pipedream_solver.ngeometry.Trapezoidal_A_ik(h_I, h_Ip1, g1_i, g2_i, g3_i)
+                _Pe_bk[k] = pipedream_solver.ngeometry.Trapezoidal_Pe_ik(h_I, h_Ip1, g1_i, g2_i, g3_i)
+                _R_bk[k] = pipedream_solver.ngeometry.Trapezoidal_R_ik(_A_bk[k], _Pe_bk[k])
                 _B_bk[k] = pipedream_solver.ngeometry.Trapezoidal_B_ik(h_I, h_Ip1, g1_i, g2_i, g3_i)
             elif geom_code == 6:
                 _A_bk[k] = pipedream_solver.ngeometry.Parabolic_A_ik(h_I, h_Ip1, g1_i, g2_i)
+                _Pe_bk[k] = pipedream_solver.ngeometry.Parabolic_Pe_ik(h_I, h_Ip1, g1_i, g2_i)
+                _R_bk[k] = pipedream_solver.ngeometry.Parabolic_R_ik(_A_bk[k], _Pe_bk[k])
                 _B_bk[k] = pipedream_solver.ngeometry.Parabolic_B_ik(h_I, h_Ip1, g1_i, g2_i)
             elif geom_code == 7:
                 _A_bk[k] = pipedream_solver.ngeometry.Elliptical_A_ik(h_I, h_Ip1, g1_i, g2_i)
+                _R_bk[k] = pipedream_solver.ngeometry.Elliptical_R_ik(_A_bk[k], _Pe_bk[k])
                 _B_bk[k] = pipedream_solver.ngeometry.Elliptical_B_ik(h_I, h_Ip1, g1_i, g2_i)
             elif geom_code == 8:
                 _A_bk[k] = pipedream_solver.ngeometry.Wide_A_ik(h_I, h_Ip1, g1_i, g2_i)
+                _Pe_bk[k] = pipedream_solver.ngeometry.Wide_Pe_ik(h_I, h_Ip1, g1_i, g2_i)
+                _R_bk[k] = pipedream_solver.ngeometry.Wide_R_ik(_A_bk[k], _Pe_bk[k])
                 _B_bk[k] = pipedream_solver.ngeometry.Wide_B_ik(h_I, h_Ip1, g1_i, g2_i)
             elif geom_code == 9:
                 _A_bk[k] = pipedream_solver.ngeometry.Force_Main_A_ik(h_I, h_Ip1, g1_i, g2_i)
+                _Pe_bk[k] = pipedream_solver.ngeometry.Force_Main_Pe_ik(h_I, h_Ip1, g1_i, g2_i)
+                _R_bk[k] = pipedream_solver.ngeometry.Force_Main_R_ik(_A_bk[k], _Pe_bk[k])
                 _B_bk[k] = pipedream_solver.ngeometry.Force_Main_B_ik(h_I, h_Ip1, g1_i, g2_i)
+            elif geom_code == 10:
+                _A_bk[k] = pipedream_solver.ngeometry.Floodplain_A_ik(h_I, h_Ip1, g1_i, g2_i, g3_i, g4_i, g5_i, g6_i, g7_i)
+                _Pe_bk[k] = pipedream_solver.ngeometry.Floodplain_Pe_ik(h_I, h_Ip1, g1_i, g2_i, g3_i, g4_i, g5_i, g6_i, g7_i)
+                _R_bk[k] = pipedream_solver.ngeometry.Floodplain_R_ik(_A_bk[k], _Pe_bk[k])
+                _B_bk[k] = pipedream_solver.ngeometry.Floodplain_B_ik(h_I, h_Ip1, g1_i, g2_i, g3_i, g4_i, g5_i, g6_i, g7_i)
     return 1
 
-@njit
+@njit(int64(float64[:], float64[:], float64[:], float64[:], float64[:], float64[:],
+            int64[:], int64),
+      cache=True)
 def numba_orifice_geometry(_Ao, h_eo, u_o, _g1_o, _g2_o, _g3_o, _geom_codes_o, n_o):
     for i in range(n_o):
         geom_code = _geom_codes_o[i]
         g1 = _g1_o[i]
         g2 = _g2_o[i]
         g3 = _g3_o[i]
         u = u_o[i]
@@ -1659,26 +1749,28 @@
                 _Ao[i] = pipedream_solver.ngeometry.Elliptical_A_ik(h_e, h_e, g1 * u, g2)
             elif geom_code == 8:
                 _Ao[i] = pipedream_solver.ngeometry.Wide_A_ik(h_e, h_e, g1 * u, g2)
             elif geom_code == 9:
                 _Ao[i] = pipedream_solver.ngeometry.Force_Main_A_ik(h_e, h_e, g1 * u, g2)
     return 1
 
-@njit
+@njit(float64[:](float64[:], float64[:], float64[:], float64[:], float64[:], boolean[:]),
+      cache=True)
 def numba_compute_functional_storage_areas(h, A, a, b, c, _functional):
     M = h.size
     for j in range(M):
         if _functional[j]:
             if h[j] < 0:
                 A[j] = 0
             else:
                 A[j] = a[j] * (h[j]**b[j]) + c[j]
     return A
 
-@njit
+@njit(float64[:](float64[:], float64[:], float64[:], float64[:], float64[:], boolean[:]),
+      cache=True)
 def numba_compute_functional_storage_volumes(h, V, a, b, c, _functional):
     M = h.size
     for j in range(M):
         if _functional[j]:
             if h[j] < 0:
                 V[j] = 0
             else:
@@ -1740,108 +1832,186 @@
         else:
             dx_0 = h_search - h_range[ix - 1]
             dx_1 = h_range[ix] - h_search
             frac = dx_0 / (dx_0 + dx_1)
             V_sj[sj] = (1 - frac) * V_range[ix - 1] + (frac) * V_range[ix]
     return V_sj
 
-@njit
+@njit(float64(float64, float64, float64, float64, float64, float64, float64))
+def friction_slope(Q_ik_t, dx_ik, A_ik, R_ik, n_ik, Sf_method_ik, g=9.81):
+    if A_ik > 0:
+        # Chezy-Manning eq.
+        if Sf_method_ik == 0:
+            t_1 = (g * n_ik**2 * np.abs(Q_ik_t) * dx_ik
+                   / A_ik / R_ik**(4/3))
+        # Hazen-Williams eq.
+        elif Sf_method_ik == 1:
+            t_1 = (1.354 * g * np.abs(Q_ik_t)**0.85 * dx_ik
+                   / A_ik**0.85 / n_ik**1.85 / R_ik**1.1655)
+        # Darcy-Weisbach eq.
+        elif Sf_method_ik == 2:
+            # kinematic viscosity(meter^2/sec), we can consider this is constant.
+            nu = 0.0000010034
+            Re = (np.abs(Q_ik_t) / A_ik) * 4 * R_ik / nu
+            f = 0.25 / (np.log10(n_ik / (3.7 * 4 * R_ik) + 5.74 / (Re**0.9)))**2
+            t_1 = (0.01274 * g * f * np.abs(Q_ik_t) * dx_ik
+                   / (A_ik * R_ik))
+        else:
+            raise ValueError('Invalid friction method.')
+        return t_1
+    else:
+        return 0.
+
+@njit(float64[:](float64[:], float64[:]),
+      cache=True)
 def numba_a_ik(u_Ik, sigma_ik):
     """
     Compute link coefficient 'a' for link i, superlink k.
     """
     return -np.maximum(u_Ik, 0) * sigma_ik
 
-@njit
+@njit(float64[:](float64[:], float64[:]),
+      cache=True)
 def numba_c_ik(u_Ip1k, sigma_ik):
     """
     Compute link coefficient 'c' for link i, superlink k.
     """
     return -np.maximum(-u_Ip1k, 0) * sigma_ik
 
-@njit
+@njit(float64[:](float64[:], float64, float64[:], float64[:], float64[:], float64[:],
+                 float64[:], float64[:], float64[:], float64[:], boolean[:], float64[:], int64[:], float64),
+      cache=True)
 def numba_b_ik(dx_ik, dt, n_ik, Q_ik_t, A_ik, R_ik,
-               A_c_ik, C_ik, a_ik, c_ik, ctrl, sigma_ik, g=9.81):
+               A_c_ik, C_ik, a_ik, c_ik, ctrl, sigma_ik, Sf_method_ik, g=9.81):
     """
     Compute link coefficient 'b' for link i, superlink k.
     """
     # TODO: Clean up
-    cond = A_ik > 0
     t_0 = (dx_ik / dt) * sigma_ik
     t_1 = np.zeros(Q_ik_t.size)
-    t_1[cond] = (g * n_ik[cond]**2 * np.abs(Q_ik_t[cond]) * dx_ik[cond]
-                / A_ik[cond] / R_ik[cond]**(4/3))
+    k = len(Sf_method_ik)
+    for n in range(k):
+        t_1[n] = friction_slope(Q_ik_t[n], dx_ik[n], A_ik[n], R_ik[n],
+                                n_ik[n], Sf_method_ik[n], g)
     t_2 = np.zeros(ctrl.size)
     cond = ctrl
-    t_2[cond] = A_ik[cond] * np.abs(Q_ik_t[cond]) / A_c_ik[cond]**2 / C_ik[cond]**2
+    t_2[cond] = C_ik[cond] * A_ik[cond] * np.abs(Q_ik_t[cond]) / A_c_ik[cond]**2
     t_3 = a_ik
     t_4 = c_ik
     return t_0 + t_1 + t_2 - t_3 - t_4
 
-@njit
+@njit(float64[:](float64[:], float64[:], float64, float64[:], float64[:], float64[:], float64),
+      cache=True)
 def numba_P_ik(Q_ik_t, dx_ik, dt, A_ik, S_o_ik, sigma_ik, g=9.81):
     """
     Compute link coefficient 'P' for link i, superlink k.
     """
     t_0 = (Q_ik_t * dx_ik / dt) * sigma_ik
     t_1 = g * A_ik * S_o_ik * dx_ik
     return t_0 + t_1
 
-@njit
+@njit(float64(float64, float64, float64, float64, float64, float64),
+      cache=True)
 def E_Ik(B_ik, dx_ik, B_im1k, dx_im1k, A_SIk, dt):
     """
     Compute node coefficient 'E' for node I, superlink k.
     """
     t_0 = B_ik * dx_ik / 2
     t_1 = B_im1k * dx_im1k / 2
     t_2 = A_SIk
     t_3 = dt
     return (t_0 + t_1 + t_2) / t_3
 
-@njit
+@njit(float64(float64, float64, float64, float64, float64, float64, float64, float64),
+      cache=True)
 def D_Ik(Q_0IK, B_ik, dx_ik, B_im1k, dx_im1k, A_SIk, h_Ik_t, dt):
     """
     Compute node coefficient 'D' for node I, superlink k.
     """
     t_0 = Q_0IK
     t_1 = B_ik * dx_ik / 2
     t_2 = B_im1k * dx_im1k / 2
     t_3 = A_SIk
     t_4 = h_Ik_t / dt
     return t_0 + ((t_1 + t_2 + t_3) * t_4)
 
-@njit
-def numba_node_coeffs(_D_Ik, _E_Ik, _Q_0Ik, _B_ik, _h_Ik, _dx_ik, _A_SIk, _dt,
-                      _forward_I_i, _backward_I_i, _is_start, _is_end, first_iter):
+@njit(int64(float64[:], float64[:], float64[:], float64[:], float64[:], float64[:], float64[:],
+            float64[:], float64[:], float64[:], float64[:], int64[:], float64,
+            int64[:], int64[:], boolean[:], boolean[:]),
+      cache=True)
+def numba_node_coeffs(_D_Ik, _E_Ik, _Q_0Ik, _B_ik, _h_Ik, _dx_ik, _A_SIk,
+                      _B_uk, _B_dk, _dx_uk, _dx_dk, _kI, _dt,
+                      _forward_I_i, _backward_I_i, _is_start, _is_end):
     N = _h_Ik.size
     for I in range(N):
+        k = _kI[I]
         if _is_start[I]:
             i = _forward_I_i[I]
-            _E_Ik[I] = E_Ik(_B_ik[i], _dx_ik[i], 0.0, 0.0, _A_SIk[I], _dt)
-            if first_iter:
-                _D_Ik[I] = D_Ik(_Q_0Ik[I], _B_ik[i], _dx_ik[i], 0.0, 0.0, _A_SIk[I],
-                                _h_Ik[I], _dt)
+            _E_Ik[I] = E_Ik(_B_ik[i], _dx_ik[i], _B_uk[k], _dx_uk[k], _A_SIk[I], _dt)
+            _D_Ik[I] = D_Ik(_Q_0Ik[I], _B_ik[i], _dx_ik[i], _B_uk[k], _dx_uk[k], _A_SIk[I],
+                            _h_Ik[I], _dt)
         elif _is_end[I]:
             im1 = _backward_I_i[I]
-            _E_Ik[I] = E_Ik(0.0, 0.0, _B_ik[im1], _dx_ik[im1],
+            _E_Ik[I] = E_Ik(_B_dk[k], _dx_dk[k], _B_ik[im1], _dx_ik[im1],
                             _A_SIk[I], _dt)
-            if first_iter:
-                _D_Ik[I] = D_Ik(_Q_0Ik[I], 0.0, 0.0, _B_ik[im1],
-                                _dx_ik[im1], _A_SIk[I], _h_Ik[I], _dt)
+            _D_Ik[I] = D_Ik(_Q_0Ik[I], _B_dk[k], _dx_dk[k], _B_ik[im1],
+                            _dx_ik[im1], _A_SIk[I], _h_Ik[I], _dt)
         else:
             i = _forward_I_i[I]
             im1 = i - 1
             _E_Ik[I] = E_Ik(_B_ik[i], _dx_ik[i], _B_ik[im1], _dx_ik[im1],
                             _A_SIk[I], _dt)
-            if first_iter:
-                _D_Ik[I] = D_Ik(_Q_0Ik[I], _B_ik[i], _dx_ik[i], _B_ik[im1],
-                                _dx_ik[im1], _A_SIk[I], _h_Ik[I], _dt)
+            _D_Ik[I] = D_Ik(_Q_0Ik[I], _B_ik[i], _dx_ik[i], _B_ik[im1],
+                            _dx_ik[im1], _A_SIk[I], _h_Ik[I], _dt)
     return 1
 
-@njit
+@njit(float64(float64, float64),
+      cache=True)
+def safe_divide(num, den):
+    if (den == 0):
+        return 0
+    else:
+        return num / den
+
+@njit(float64[:](float64[:], float64[:]),
+      cache=True)
+def safe_divide_vec(num, den):
+    result = np.zeros_like(num)
+    cond = (den != 0)
+    result[cond] = num[cond] / den[cond]
+    return result
+
+@njit(float64(float64, float64, float64, float64, float64),
+      cache=True)
+def Q_i_f(h_Ip1k, h_1k, U_Ik, V_Ik, W_Ik):
+    t_0 = U_Ik * h_Ip1k
+    t_1 = V_Ik
+    t_2 = W_Ik * h_1k
+    return t_0 + t_1 + t_2
+
+@njit(float64(float64, float64, float64, float64, float64),
+      cache=True)
+def Q_i_b(h_Ik, h_Np1k, X_Ik, Y_Ik, Z_Ik):
+    t_0 = X_Ik * h_Ik
+    t_1 = Y_Ik
+    t_2 = Z_Ik * h_Np1k
+    return t_0 + t_1 + t_2
+
+@njit(float64(float64, float64, float64, float64, float64),
+      cache=True)
+def h_i_b(Q_ik, h_Np1k, X_Ik, Y_Ik, Z_Ik):
+    num = Q_ik - Y_Ik - Z_Ik * h_Np1k
+    den = X_Ik
+    result = safe_divide(num, den)
+    return result
+
+@njit(int64(float64[:], float64[:], float64[:], float64[:], float64[:], float64[:], float64[:],
+            float64[:], float64[:], float64[:], int64[:], int64[:], int64[:], int64,
+            float64, float64[:], boolean),
+      cache=True)
 def numba_solve_internals(_h_Ik, _Q_ik, _h_uk, _h_dk, _U_Ik, _V_Ik, _W_Ik,
                           _X_Ik, _Y_Ik, _Z_Ik, _i_1k, _I_1k, nk, NK,
                           min_depth, max_depth_k, first_link_backwards=True):
     for k in range(NK):
         n = nk[k]
         i_1 = _i_1k[k]
         I_1 = _I_1k[k]
@@ -1871,70 +2041,53 @@
                             _Z_Ik[I_1])
         else:
             # Not theoretically correct, but seems to be more stable sometimes
             _Q_ik[i_1] = Q_i_f(_h_Ik[I_1 + 1], _h_1k, _U_Ik[I_1], _V_Ik[I_1],
                             _W_Ik[I_1])
     return 1
 
-@njit
-def Q_i_f(h_Ip1k, h_1k, U_Ik, V_Ik, W_Ik):
-    t_0 = U_Ik * h_Ip1k
-    t_1 = V_Ik
-    t_2 = W_Ik * h_1k
-    return t_0 + t_1 + t_2
-
-@njit
-def Q_i_b(h_Ik, h_Np1k, X_Ik, Y_Ik, Z_Ik):
-    t_0 = X_Ik * h_Ik
-    t_1 = Y_Ik
-    t_2 = Z_Ik * h_Np1k
-    return t_0 + t_1 + t_2
-
-@njit
-def h_i_b(Q_ik, h_Np1k, X_Ik, Y_Ik, Z_Ik):
-    num = Q_ik - Y_Ik - Z_Ik * h_Np1k
-    den = X_Ik
-    result = safe_divide(num, den)
-    return result
-
-@njit
+@njit(float64[:](float64[:], int64, int64[:], int64[:], int64[:], int64[:], float64[:], float64[:], float64[:]),
+      cache=True)
 def numba_solve_internals_ls(_h_Ik, NK, nk, _k_1k, _i_1k, _I_1k, _U, _X, _b):
     for k in range(NK):
         nlinks = nk[k]
         lstart = _k_1k[k]
         rstart = _i_1k[k]
         jstart = _I_1k[k]
         _Ak = np.zeros((nlinks, nlinks - 1))
         for i in range(nlinks - 1):
             _Ak[i, i] = _U[lstart + i]
             _Ak[i + 1, i] = -_X[lstart + i]
-        _bk = _b[rstart:rstart+nlinks]
-        _AA = _Ak.T @ _Ak
-        _Ab = _Ak.T @ _bk
+        _AkT = _Ak.T.copy()
+        _bk = _b[rstart:rstart+nlinks].copy()
+        _AA = _AkT @ _Ak
+        _Ab = _AkT @ _bk
         # If want to prevent singular matrix, set ( diag == 0 ) = 1
         for i in range(nlinks - 1):
             if (_AA[i, i] == 0.0):
                 _AA[i, i] = 1.0
         _h_inner = np.linalg.solve(_AA, _Ab)
         _h_Ik[jstart+1:jstart+nlinks] = _h_inner
     return _h_Ik
 
-@njit
+@njit(float64[:](float64[:], float64[:], float64[:]),
+      cache=True)
 def numba_u_ik(_Q_ik, _A_ik, _u_ik):
     n = _u_ik.size
     for i in range(n):
         _Q_i = _Q_ik[i]
         _A_i = _A_ik[i]
         if _A_i:
             _u_ik[i] = _Q_i / _A_i
         else:
             _u_ik[i] = 0
     return _u_ik
 
-@njit
+@njit(float64[:](float64[:], float64[:], boolean[:], float64[:]),
+      cache=True)
 def numba_u_Ik(_dx_ik, _u_ik, _link_start, _u_Ik):
     n = _u_Ik.size
     for i in range(n):
         if _link_start[i]:
             _u_Ik[i] = _u_ik[i]
         else:
             im1 = i - 1
@@ -1942,15 +2095,16 @@
             den = _dx_ik[i] + _dx_ik[im1]
             if den:
                 _u_Ik[i] = num / den
             else:
                 _u_Ik[i] = 0
     return _u_Ik
 
-@njit
+@njit(float64[:](float64[:], float64[:], boolean[:], float64[:]),
+      cache=True)
 def numba_u_Ip1k(_dx_ik, _u_ik, _link_end, _u_Ip1k):
     n = _u_Ip1k.size
     for i in range(n):
         if _link_end[i]:
             _u_Ip1k[i] = _u_ik[i]
         else:
             ip1 = i + 1
@@ -1958,76 +2112,120 @@
             den = _dx_ik[i] + _dx_ik[ip1]
             if den:
                 _u_Ip1k[i] = num / den
             else:
                 _u_Ip1k[i] = 0
     return _u_Ip1k
 
-@njit
-def safe_divide(num, den):
-    if (den == 0):
-        return 0
-    else:
-        return num / den
+@njit(float64[:](float64[:], float64[:], float64[:], float64[:], float64[:], float64[:],
+                 int64[:], float64, float64), cache=True)
+def kappa_uk(Q_uk, dx_uk, A_uk, C_uk, R_uk, n_uk, Sf_method_uk, dt, g=9.81):
+    """
+    Compute boundary coefficient 'kappa' for upstream end of superlink k.
+    """
+    k = Q_uk.size
+    t_0 = - dx_uk / g / A_uk / dt
+    t_1 = np.zeros(k, dtype=np.float64)
+    for n in range(k):
+        t_1[n] = friction_slope(Q_uk[n], dx_uk[n], A_uk[n], R_uk[n],
+                                n_uk[n], Sf_method_uk[n], g)
+    t_2 = - C_uk * np.abs(Q_uk) / 2 / g / A_uk**2
+    return t_0 + t_1 + t_2
 
-@njit
-def safe_divide_vec(num, den):
-    result = np.zeros_like(num)
-    cond = (den != 0)
-    result[cond] = num[cond] / den[cond]
-    return result
+@njit(float64[:](float64[:], float64[:], float64[:], float64[:], float64[:], float64[:],
+                 int64[:], float64, float64), cache=True)
+def kappa_dk(Q_dk, dx_dk, A_dk, C_dk, R_dk, n_dk, Sf_method_dk, dt, g=9.81):
+    """
+    Compute boundary coefficient 'kappa' for downstream end of superlink k.
+    """
+    k = Q_dk.size
+    t_0 = dx_dk / g / A_dk / dt
+    t_1 = np.zeros(k, dtype=np.float64)
+    for n in range(k):
+        t_1[n] = friction_slope(Q_dk[n], dx_dk[n], A_dk[n], R_dk[n],
+                                n_dk[n], Sf_method_dk[n], g)
+    t_2 = C_dk * np.abs(Q_dk) / 2 / g / A_dk**2
+    return t_0 + t_1 + t_2
 
-@njit
+@njit(float64[:](float64[:], float64[:], float64[:], float64[:], float64[:],
+                 float64[:], float64, float64), cache=True)
+def mu_uk(Q_uk_t, dx_uk, A_uk, theta_uk, z_inv_uk, S_o_uk, dt, g=9.81):
+    """
+    Compute boundary coefficient 'mu' for upstream end of superlink k.
+    """
+    t_0 = Q_uk_t * dx_uk / g / A_uk / dt
+    t_1 = - theta_uk * z_inv_uk
+    t_2 = dx_uk * S_o_uk
+    return t_0 + t_1 + t_2
+
+@njit(float64[:](float64[:], float64[:], float64[:], float64[:], float64[:],
+                 float64[:], float64, float64), cache=True)
+def mu_dk(Q_dk_t, dx_dk, A_dk, theta_dk, z_inv_dk, S_o_dk, dt, g=9.81):
+    """
+    Compute boundary coefficient 'mu' for downstream end of superlink k.
+    """
+    t_0 = - Q_dk_t * dx_dk / g / A_dk / dt
+    t_1 = - theta_dk * z_inv_dk
+    t_2 = - dx_dk * S_o_dk
+    return t_0 + t_1 + t_2
+
+@njit(float64(float64, float64, float64, float64, float64),
+      cache=True)
 def U_1k(E_2k, c_1k, A_1k, T_1k, g=9.81):
     """
     Compute forward recurrence coefficient 'U' for node 1, superlink k.
     """
     num = E_2k * c_1k - g * A_1k
     den = T_1k
     result = safe_divide(num, den)
     return result
 
-@njit
+@njit(float64(float64, float64, float64, float64, float64, float64),
+      cache=True)
 def V_1k(P_1k, D_2k, c_1k, T_1k, a_1k=0.0, D_1k=0.0):
     """
     Compute forward recurrence coefficient 'V' for node 1, superlink k.
     """
     num = P_1k - D_2k * c_1k + D_1k * a_1k
     den = T_1k
     result = safe_divide(num, den)
     return result
 
-@njit
+@njit(float64(float64, float64, float64, float64, float64),
+      cache=True)
 def W_1k(A_1k, T_1k, a_1k=0.0, E_1k=0.0, g=9.81):
     """
     Compute forward recurrence coefficient 'W' for node 1, superlink k.
     """
     num = g * A_1k - E_1k * a_1k
     den = T_1k
     result = safe_divide(num, den)
     return result
 
-@njit
+@njit(float64(float64, float64, float64),
+      cache=True)
 def T_1k(a_1k, b_1k, c_1k):
     """
     Compute forward recurrence coefficient 'T' for link 1, superlink k.
     """
     return a_1k + b_1k + c_1k
 
-@njit
+@njit(float64(float64, float64, float64, float64, float64),
+      cache=True)
 def U_Ik(E_Ip1k, c_ik, A_ik, T_ik, g=9.81):
     """
     Compute forward recurrence coefficient 'U' for node I, superlink k.
     """
     num = E_Ip1k * c_ik - g * A_ik
     den = T_ik
     result = safe_divide(num, den)
     return result
 
-@njit
+@njit(float64(float64, float64, float64, float64, float64, float64, float64, float64, float64, float64, float64),
+      cache=True)
 def V_Ik(P_ik, a_ik, D_Ik, D_Ip1k, c_ik, A_ik, E_Ik, V_Im1k, U_Im1k, T_ik, g=9.81):
     """
     Compute forward recurrence coefficient 'V' for node I, superlink k.
     """
     t_0 = P_ik
     t_1 = a_ik * D_Ik
     t_2 = D_Ip1k * c_ik
@@ -2037,83 +2235,91 @@
     t_6 = T_ik
     # TODO: There is still a divide by zero here
     num = (t_0 + t_1 - t_2 - (t_3 * t_4 / t_5))
     den = t_6
     result = safe_divide(num, den)
     return  result
 
-@njit
+@njit(float64(float64, float64, float64, float64, float64, float64, float64),
+      cache=True)
 def W_Ik(A_ik, E_Ik, a_ik, W_Im1k, U_Im1k, T_ik, g=9.81):
     """
     Compute forward recurrence coefficient 'W' for node I, superlink k.
     """
     num = -(g * A_ik - E_Ik * a_ik) * W_Im1k
     den = (U_Im1k - E_Ik) * T_ik
     result = safe_divide(num, den)
     return result
 
-@njit
+@njit(float64(float64, float64, float64, float64, float64, float64, float64),
+      cache=True)
 def T_ik(a_ik, b_ik, c_ik, A_ik, E_Ik, U_Im1k, g=9.81):
     """
     Compute forward recurrence coefficient 'T' for link i, superlink k.
     """
     t_0 = a_ik + b_ik + c_ik
     t_1 = g * A_ik - E_Ik * a_ik
     t_2 = U_Im1k - E_Ik
     result = t_0 - safe_divide(t_1, t_2)
     return result
 
-@njit
+@njit(float64(float64, float64, float64, float64, float64),
+      cache=True)
 def X_Nk(A_nk, E_Nk, a_nk, O_nk, g=9.81):
     """
     Compute backward recurrence coefficient 'X' for node N, superlink k.
     """
     num = g * A_nk - E_Nk * a_nk
     den = O_nk
     result = safe_divide(num, den)
     return result
 
-@njit
+@njit(float64(float64, float64, float64, float64, float64, float64),
+      cache=True)
 def Y_Nk(P_nk, D_Nk, a_nk, O_nk, c_nk=0.0, D_Np1k=0.0):
     """
     Compute backward recurrence coefficient 'Y' for node N, superlink k.
     """
     num = P_nk + D_Nk * a_nk - D_Np1k * c_nk
     den = O_nk
     result = safe_divide(num, den)
     return result
 
-@njit
+@njit(float64(float64, float64, float64, float64, float64),
+      cache=True)
 def Z_Nk(A_nk, O_nk, c_nk=0.0, E_Np1k=0.0, g=9.81):
     """
     Compute backward recurrence coefficient 'Z' for node N, superlink k.
     """
     num = E_Np1k * c_nk - g * A_nk
     den = O_nk
     result = safe_divide(num, den)
     return result
 
-@njit
+@njit(float64(float64, float64, float64),
+      cache=True)
 def O_nk(a_nk, b_nk, c_nk):
     """
     Compute backward recurrence coefficient 'O' for link n, superlink k.
     """
     return a_nk + b_nk + c_nk
 
-@njit
+@njit(float64(float64, float64, float64, float64, float64),
+      cache=True)
 def X_Ik(A_ik, E_Ik, a_ik, O_ik, g=9.81):
     """
     Compute backward recurrence coefficient 'X' for node I, superlink k.
     """
     num = g * A_ik - E_Ik * a_ik
     den = O_ik
     result = safe_divide(num, den)
     return result
 
-@njit
+@njit(float64(float64, float64, float64, float64, float64, float64, float64, float64, float64, float64, float64),
+      cache=True)
 def Y_Ik(P_ik, a_ik, D_Ik, D_Ip1k, c_ik, A_ik, E_Ip1k, Y_Ip1k, X_Ip1k, O_ik, g=9.81):
     """
     Compute backward recurrence coefficient 'Y' for node I, superlink k.
     """
     t_0 = P_ik
     t_1 = a_ik * D_Ik
     t_2 = D_Ip1k * c_ik
@@ -2123,182 +2329,213 @@
     t_6 = O_ik
     # TODO: There is still a divide by zero here
     num = (t_0 + t_1 - t_2 - (t_3 * t_4 / t_5))
     den = t_6
     result = safe_divide(num, den)
     return result
 
-@njit
+@njit(float64(float64, float64, float64, float64, float64, float64, float64),
+      cache=True)
 def Z_Ik(A_ik, E_Ip1k, c_ik, Z_Ip1k, X_Ip1k, O_ik, g=9.81):
     """
     Compute backward recurrence coefficient 'Z' for node I, superlink k.
     """
     num = (g * A_ik - E_Ip1k * c_ik) * Z_Ip1k
     den = (X_Ip1k + E_Ip1k) * O_ik
     result = safe_divide(num, den)
     return result
 
-@njit
+@njit(float64(float64, float64, float64, float64, float64, float64, float64),
+      cache=True)
 def O_ik(a_ik, b_ik, c_ik, A_ik, E_Ip1k, X_Ip1k, g=9.81):
     """
     Compute backward recurrence coefficient 'O' for link i, superlink k.
     """
     t_0 = a_ik + b_ik + c_ik
     t_1 = g * A_ik - E_Ip1k * c_ik
     t_2 = X_Ip1k + E_Ip1k
     result = t_0 + safe_divide(t_1, t_2)
     return result
 
-@njit
+@njit(float64[:](float64[:], float64[:], float64[:], float64[:], float64[:], float64[:]),
+      cache=True)
 def numba_D_k_star(X_1k, kappa_uk, U_Nk, kappa_dk, Z_1k, W_Nk):
     """
     Compute superlink boundary condition coefficient 'D_k_star'.
     """
     t_0 = (X_1k * kappa_uk - 1) * (U_Nk * kappa_dk - 1)
     t_1 = (Z_1k * kappa_dk) * (W_Nk * kappa_uk)
     result = t_0 - t_1
     return result
 
-@njit
-def numba_alpha_uk(U_Nk, kappa_dk, X_1k, Z_1k, W_Nk, D_k_star, lambda_uk, theta_uk):
+@njit(float64[:](float64[:], float64[:], float64[:], float64[:], float64[:], float64[:], float64[:]),
+      cache=True)
+def numba_alpha_uk(U_Nk, kappa_dk, X_1k, Z_1k, W_Nk, D_k_star, lambda_uk):
     """
     Compute superlink boundary condition coefficient 'alpha' for upstream end
     of superlink k.
     """
-    num = theta_uk * ((1 - U_Nk * kappa_dk) * X_1k * lambda_uk
-                        + (Z_1k * kappa_dk * W_Nk * lambda_uk))
+    num = lambda_uk * ((1 - U_Nk * kappa_dk) * X_1k + (Z_1k * kappa_dk * W_Nk))
     den = D_k_star
     result = safe_divide_vec(num, den)
     return result
 
-@njit
-def numba_beta_uk(U_Nk, kappa_dk, Z_1k, W_Nk, D_k_star, lambda_dk, theta_dk):
+@njit(float64[:](float64[:], float64[:], float64[:], float64[:], float64[:], float64[:]),
+      cache=True)
+def numba_beta_uk(U_Nk, kappa_dk, Z_1k, W_Nk, D_k_star, lambda_dk):
     """
     Compute superlink boundary condition coefficient 'beta' for upstream end
     of superlink k.
     """
-    num = theta_dk * ((1 - U_Nk * kappa_dk) * Z_1k * lambda_dk
-            + (Z_1k * kappa_dk * U_Nk * lambda_dk))
+    num = lambda_dk * ((1 - U_Nk * kappa_dk) * Z_1k + (Z_1k * kappa_dk * U_Nk))
     den = D_k_star
     result = safe_divide_vec(num, den)
     return result
 
-@njit
+@njit(float64[:](float64[:], float64[:], float64[:], float64[:], float64[:], float64[:],
+                 float64[:], float64[:], float64[:], float64[:]),
+      cache=True)
 def numba_chi_uk(U_Nk, kappa_dk, Y_1k, X_1k, mu_uk, Z_1k,
-                    mu_dk, V_Nk, W_Nk, D_k_star, theta_uk, theta_dk):
+                 mu_dk, V_Nk, W_Nk, D_k_star):
     """
     Compute superlink boundary condition coefficient 'chi' for upstream end
     of superlink k.
     """
-    t_0 = (1 - U_Nk * kappa_dk) * (Y_1k + theta_uk * X_1k * mu_uk + theta_dk * Z_1k * mu_dk)
-    t_1 = (Z_1k * kappa_dk) * (V_Nk + theta_uk * W_Nk * mu_uk + theta_dk * U_Nk * mu_dk)
+    t_0 = (1 - U_Nk * kappa_dk) * (Y_1k + X_1k * mu_uk + Z_1k * mu_dk)
+    t_1 = (Z_1k * kappa_dk) * (V_Nk + W_Nk * mu_uk + U_Nk * mu_dk)
     num = t_0 + t_1
     den = D_k_star
     result = safe_divide_vec(num, den)
     return result
 
-@njit
-def numba_alpha_dk(X_1k, kappa_uk, W_Nk, D_k_star, lambda_uk, theta_uk):
+@njit(float64[:](float64[:], float64[:], float64[:], float64[:], float64[:]),
+      cache=True)
+def numba_alpha_dk(X_1k, kappa_uk, W_Nk, D_k_star, lambda_uk):
     """
     Compute superlink boundary condition coefficient 'alpha' for downstream end
     of superlink k.
     """
-    num = theta_uk * ((1 - X_1k * kappa_uk) * W_Nk * lambda_uk
-            + (W_Nk * kappa_uk * X_1k * lambda_uk))
+    num = lambda_uk * ((1 - X_1k * kappa_uk) * W_Nk + (W_Nk * kappa_uk * X_1k))
     den = D_k_star
     result = safe_divide_vec(num, den)
     return result
 
-@njit
-def numba_beta_dk(X_1k, kappa_uk, U_Nk, W_Nk, Z_1k, D_k_star, lambda_dk, theta_dk):
+@njit(float64[:](float64[:], float64[:], float64[:], float64[:], float64[:], float64[:], float64[:]),
+      cache=True)
+def numba_beta_dk(X_1k, kappa_uk, U_Nk, W_Nk, Z_1k, D_k_star, lambda_dk):
     """
     Compute superlink boundary condition coefficient 'beta' for downstream end
     of superlink k.
     """
-    num = theta_dk * ((1 - X_1k * kappa_uk) * U_Nk * lambda_dk
-            + (W_Nk * kappa_uk * Z_1k * lambda_dk))
+    num = lambda_dk * ((1 - X_1k * kappa_uk) * U_Nk + (W_Nk * kappa_uk * Z_1k))
     den = D_k_star
     result = safe_divide_vec(num, den)
     return result
 
-@njit
+@njit(float64[:](float64[:], float64[:], float64[:], float64[:], float64[:], float64[:],
+                 float64[:], float64[:], float64[:], float64[:]),
+      cache=True)
 def numba_chi_dk(X_1k, kappa_uk, V_Nk, W_Nk, mu_uk, U_Nk,
-                    mu_dk, Y_1k, Z_1k, D_k_star, theta_uk, theta_dk):
+                    mu_dk, Y_1k, Z_1k, D_k_star):
     """
     Compute superlink boundary condition coefficient 'chi' for downstream end
     of superlink k.
     """
-    t_0 = (1 - X_1k * kappa_uk) * (V_Nk + theta_uk * W_Nk * mu_uk + theta_dk * U_Nk * mu_dk)
-    t_1 = (W_Nk * kappa_uk) * (Y_1k + theta_uk * X_1k * mu_uk + theta_dk * Z_1k * mu_dk)
+    t_0 = (1 - X_1k * kappa_uk) * (V_Nk + W_Nk * mu_uk + U_Nk * mu_dk)
+    t_1 = (W_Nk * kappa_uk) * (Y_1k + X_1k * mu_uk + Z_1k * mu_dk)
     num = t_0 + t_1
     den = D_k_star
     result = safe_divide_vec(num, den)
     return result
 
-@njit
-def gamma_o(Q_o_t, Ao, Co=0.67, g=9.81):
+@njit(float64[:](float64[:], float64[:], float64[:], float64),
+      cache=True)
+def gamma_o(Q_o_t, Ao, Co, g=9.81):
     """
     Compute flow coefficient 'gamma' for orifice o.
     """
     num = 2 * g * Co**2 * Ao**2
     den = np.abs(Q_o_t)
     result = safe_divide_vec(num, den)
     return result
 
-@njit
-def gamma_w(Q_w_t, H_w_t, L_w, s_w, Cwr=1.838, Cwt=1.380):
+@njit(float64[:](float64[:], float64[:], float64[:], float64[:], float64[:], float64[:]),
+      cache=True)
+def gamma_w(Q_w_t, H_w_t, L_w, s_w, Cwr, Cwt):
     """
     Compute flow coefficient 'gamma' for weir w.
     """
     num = (Cwr * L_w * H_w_t + Cwt * s_w * H_w_t**2)**2
     den = np.abs(Q_w_t)
     result = safe_divide_vec(num, den)
     return result
 
-@njit
-def gamma_p(Q_p_t, dH_p_t, a_q=1.0, a_h=1.0):
+@njit(float64[:](float64[:], float64[:], float64[:], float64[:]),
+      cache=True)
+def gamma_p(Q_p_t, b_p, c_p, u):
     """
     Compute flow coefficient 'gamma' for pump p.
     """
-    num = a_q**2 * np.abs(dH_p_t)
-    den = a_h**2 * np.abs(Q_p_t)
+    num = u
+    den = b_p * np.abs(Q_p_t)**(c_p - 1)
     result = safe_divide_vec(num, den)
     return result
 
-@njit
+@njit(float64[:](float64[:], float64[:], float64[:], float64),
+      cache=True)
 def gamma_uk(Q_uk_t, C_uk, A_uk, g=9.81):
     """
     Compute flow coefficient 'gamma' for upstream end of superlink k
     """
-    num = -np.abs(Q_uk_t)
-    den = 2 * (C_uk**2) * (A_uk**2) * g
+    num = -np.abs(Q_uk_t) * C_uk
+    den = 2 * (A_uk**2) * g
     result = safe_divide_vec(num, den)
     return result
 
-@njit
+@njit(float64[:](float64[:], float64[:], float64[:], float64),
+      cache=True)
 def gamma_dk(Q_dk_t, C_dk, A_dk, g=9.81):
     """
     Compute flow coefficient 'gamma' for downstream end of superlink k
     """
-    num = np.abs(Q_dk_t)
-    den = 2 * (C_dk**2) * (A_dk**2) * g
+    num = np.abs(Q_dk_t) * C_dk
+    den = 2 * (A_dk**2) * g
     result = safe_divide_vec(num, den)
     return result
 
-@njit
+@njit(float64[:](float64[:], float64[:], float64[:], float64),
+      cache=True)
+def xi_uk(dx_uk, B_uk, theta_uk, dt):
+    num = dx_uk * B_uk * theta_uk
+    den = 2 * dt
+    result = num / den
+    return result
+
+@njit(float64[:](float64[:], float64[:], float64[:], float64),
+      cache=True)
+def xi_dk(dx_dk, B_dk, theta_dk, dt):
+    num = dx_dk * B_dk * theta_dk
+    den = 2 * dt
+    result = num / den
+    return result
+
+@njit(int64(float64[:], float64[:], float64[:], float64[:], float64[:], float64[:], float64[:],
+            float64[:], float64[:], float64[:], float64[:], float64[:], int64[:], int64[:]),
+      cache=True)
 def numba_orifice_flow_coefficients(_alpha_o, _beta_o, _chi_o, H_j, _Qo, u, _z_inv_j,
                                     _z_o, _tau_o, _Co, _Ao, _y_max_o, _J_uo, _J_do):
+    g = 9.81
     _H_uo = H_j[_J_uo]
     _H_do = H_j[_J_do]
     _z_inv_uo = _z_inv_j[_J_uo]
     # Create indicator functions
     _omega_o = np.zeros_like(_H_uo)
     _omega_o[_H_uo >= _H_do] = 1.0
     # Compute universal coefficients
-    _gamma_o = gamma_o(_Qo, _Ao, _Co)
+    _gamma_o = gamma_o(_Qo, _Ao, _Co, g)
     # Create conditionals
     cond_0 = (_omega_o * _H_uo + (1 - _omega_o) * _H_do >
                 _z_o + _z_inv_uo + (_tau_o * _y_max_o * u))
     cond_1 = ((1 - _omega_o) * _H_uo + _omega_o * _H_do >
                 _z_o + _z_inv_uo + (_tau_o * _y_max_o * u / 2))
     cond_2 = (_omega_o * _H_uo + (1 - _omega_o) * _H_do >
                 _z_o + _z_inv_uo)
@@ -2324,15 +2561,17 @@
     # No flow
     d = (~cond_0 & ~cond_2)
     _alpha_o[d] = 0.0
     _beta_o[d] = 0.0
     _chi_o[d] = 0.0
     return 1
 
-@njit
+@njit(float64[:](float64[:], float64[:], float64[:], float64[:],
+            float64[:], float64[:], float64[:], float64[:], int64[:], int64[:], float64),
+      cache=True)
 def numba_solve_orifice_flows(H_j, u, _z_inv_j, _z_o,
                               _tau_o, _y_max_o, _Co, _Ao, _J_uo, _J_do, g=9.81):
     # Specify orifice heads at previous timestep
     _H_uo = H_j[_J_uo]
     _H_do = H_j[_J_do]
     _z_inv_uo = _z_inv_j[_J_uo]
     # Create indicator functions
@@ -2377,15 +2616,17 @@
     _chi_o[d] = 0.0
     # Compute flow
     _Qo_next = (-1)**(1 - _omega_o) * np.sqrt(np.abs(
                _alpha_o * _H_uo + _beta_o * _H_do + _chi_o))
     # Export instance variables
     return _Qo_next
 
-@njit
+@njit(int64(float64[:], float64[:], float64[:], float64[:], float64[:], float64[:], float64[:], float64[:],
+            float64[:], float64[:], float64[:], float64[:], float64[:], float64[:], int64[:], int64[:]),
+      cache=True)
 def numba_weir_flow_coefficients(_Hw, _Qw, _alpha_w, _beta_w, _chi_w, H_j, _z_inv_j, _z_w,
                                  _y_max_w, u, _L_w, _s_w, _Cwr, _Cwt, _J_uw, _J_dw):
     # Specify weir heads at previous timestep
     _H_uw = H_j[_J_uw]
     _H_dw = H_j[_J_dw]
     _z_inv_uw = _z_inv_j[_J_uw]
     # Create indicator functions
@@ -2422,15 +2663,17 @@
     # No flow
     c = (~cond_0)
     _alpha_w[c] = 0.0
     _beta_w[c] = 0.0
     _chi_w[c] = 0.0
     return 1
 
-@njit
+@njit(float64[:](float64[:], float64[:], float64[:], float64[:], float64[:], float64[:], float64[:], float64[:],
+            float64[:], float64[:], float64[:], int64[:], int64[:]),
+      cache=True)
 def numba_solve_weir_flows(_Hw, _Qw, H_j, _z_inv_j, _z_w, _y_max_w, u, _L_w,
                            _s_w, _Cwr, _Cwt, _J_uw, _J_dw):
     _H_uw = H_j[_J_uw]
     _H_dw = H_j[_J_dw]
     _z_inv_uw = _z_inv_j[_J_uw]
     # Create indicator functions
     _omega_w = np.zeros(_H_uw.size)
@@ -2452,163 +2695,187 @@
     _Hw = np.abs(_Hw)
     # Compute universal coefficient
     _gamma_ww = (_Cwr * _L_w * _Hw + _Cwt * _s_w * _Hw**2)**2
     # Compute flow
     _Qw_next = (-1)**(1 - _omega_w) * np.sqrt(_gamma_ww * _Hw)
     return _Qw_next
 
-@njit
+@njit(int64(float64[:], float64[:], float64[:], float64[:], float64[:], float64[:], float64[:],
+            float64[:], float64[:], float64[:], float64[:], float64[:], float64[:],
+            int64[:], int64[:]),
+      cache=True)
 def numba_pump_flow_coefficients(_alpha_p, _beta_p, _chi_p, H_j, _z_inv_j, _Qp, u,
-                                 _z_p, _dHp_max, _dHp_min, _ap_q, _ap_h, _J_up, _J_dp):
+                                 _z_p, _dHp_max, _dHp_min, _a_p, _b_p, _c_p,
+                                 _J_up, _J_dp):
     # Get upstream and downstream heads and invert elevation
     _H_up = H_j[_J_up]
     _H_dp = H_j[_J_dp]
     _z_inv_up = _z_inv_j[_J_up]
     # Compute effective head
     _dHp = _H_dp - _H_up
+    # Condition 0: Upstream head is above inlet height
     cond_0 = _H_up > _z_inv_up + _z_p
+    # Condition 1: Head difference is within range of pump curve
     cond_1 = (_dHp > _dHp_min) & (_dHp < _dHp_max)
     _dHp[_dHp > _dHp_max] = _dHp_max
     _dHp[_dHp < _dHp_min] = _dHp_min
     # Compute universal coefficients
-    _gamma_p = gamma_p(_Qp, _dHp, _ap_q, _ap_h)
+    _gamma_p = gamma_p(_Qp, _b_p, _c_p, u)
     # Fill coefficient arrays
     # Head in pump curve range
     a = (cond_0 & cond_1)
-    _alpha_p[a] = _gamma_p[a] * u[a]**2
-    _beta_p[a] = -_gamma_p[a] * u[a]**2
-    _chi_p[a] = (_gamma_p[a] * _ap_h[a]**2 / np.abs(_dHp[a])) * u[a]**2
+    _alpha_p[a] = _gamma_p[a]
+    _beta_p[a] = -_gamma_p[a]
+    _chi_p[a] = _gamma_p[a] * _a_p[a]
     # Head outside of pump curve range
     b = (cond_0 & ~cond_1)
     _alpha_p[b] = 0.0
     _beta_p[b] = 0.0
-    _chi_p[b] = np.sqrt(np.maximum(_ap_q[b]**2 * (1 - _dHp[b]**2 / _ap_h[b]**2), 0.0)) * u[b]
+    _chi_p[b] = _gamma_p[b] * (_a_p[b] - _dHp[b])
     # Depth below inlet
     c = (~cond_0)
     _alpha_p[c] = 0.0
     _beta_p[c] = 0.0
     _chi_p[c] = 0.0
     return 1
 
-@njit
-def numba_solve_pump_flows(H_j, u, _z_inv_j, _z_p, _dHp_max, _dHp_min, _ap_q, _ap_h,
+@njit(float64[:](float64[:], float64[:], float64[:], float64[:], float64[:], float64[:],
+                 float64[:], float64[:], float64[:], int64[:], int64[:]),
+      cache=True)
+def numba_solve_pump_flows(H_j, u, _z_inv_j, _z_p, _dHp_max, _dHp_min, _a_p, _b_p, _c_p,
                            _J_up, _J_dp):
     _H_up = H_j[_J_up]
     _H_dp = H_j[_J_dp]
     _z_inv_up = _z_inv_j[_J_up]
     # Create conditionals
     _dHp = _H_dp - _H_up
     _dHp[_dHp > _dHp_max] = _dHp_max
     _dHp[_dHp < _dHp_min] = _dHp_min
     cond_0 = _H_up > _z_inv_up + _z_p
     # Compute universal coefficients
-    _Qp_next = u * np.sqrt(np.maximum(_ap_q**2 * (1 - (_dHp)**2 / _ap_h**2), 0.0))
+    _Qp_next = (u / _b_p * (_a_p - _dHp))**(1 / _c_p)
     _Qp_next[~cond_0] = 0.0
     return _Qp_next
 
-@njit
+@njit(int64(float64[:], float64[:], float64[:], float64[:], float64[:], float64[:], float64[:],
+            float64[:], float64[:], float64[:], float64[:], int64, int64[:], int64[:], int64[:]),
+      cache=True)
 def numba_forward_recurrence(_T_ik, _U_Ik, _V_Ik, _W_Ik, _a_ik, _b_ik, _c_ik,
                              _P_ik, _A_ik, _E_Ik, _D_Ik, NK, nk, _I_1k, _i_1k):
+    g = 9.81
     for k in range(NK):
         # Start at junction 1
         _I_1 = _I_1k[k]
         _i_1 = _i_1k[k]
         _I_2 = _I_1 + 1
         _i_2 = _i_1 + 1
         nlinks = nk[k]
         _T_ik[_i_1] = T_1k(_a_ik[_i_1], _b_ik[_i_1], _c_ik[_i_1])
-        _U_Ik[_I_1] = U_1k(_E_Ik[_I_2], _c_ik[_i_1], _A_ik[_i_1], _T_ik[_i_1])
+        _U_Ik[_I_1] = U_1k(_E_Ik[_I_2], _c_ik[_i_1], _A_ik[_i_1], _T_ik[_i_1], g)
         _V_Ik[_I_1] = V_1k(_P_ik[_i_1], _D_Ik[_I_2], _c_ik[_i_1], _T_ik[_i_1],
                             _a_ik[_i_1], _D_Ik[_I_1])
-        _W_Ik[_I_1] = W_1k(_A_ik[_i_1], _T_ik[_i_1], _a_ik[_i_1], _E_Ik[_I_1])
+        _W_Ik[_I_1] = W_1k(_A_ik[_i_1], _T_ik[_i_1], _a_ik[_i_1], _E_Ik[_I_1], g)
         # Loop from junction 2 -> Nk
         for i in range(nlinks - 1):
             _i_next = _i_2 + i
             _I_next = _I_2 + i
             _Im1_next = _I_next - 1
             _Ip1_next = _I_next + 1
             _T_ik[_i_next] = T_ik(_a_ik[_i_next], _b_ik[_i_next], _c_ik[_i_next],
-                                  _A_ik[_i_next], _E_Ik[_I_next], _U_Ik[_Im1_next])
+                                  _A_ik[_i_next], _E_Ik[_I_next], _U_Ik[_Im1_next], g)
             _U_Ik[_I_next] = U_Ik(_E_Ik[_Ip1_next], _c_ik[_i_next],
-                                  _A_ik[_i_next], _T_ik[_i_next])
+                                  _A_ik[_i_next], _T_ik[_i_next], g)
             _V_Ik[_I_next] = V_Ik(_P_ik[_i_next], _a_ik[_i_next], _D_Ik[_I_next],
                                   _D_Ik[_Ip1_next], _c_ik[_i_next], _A_ik[_i_next],
                                   _E_Ik[_I_next], _V_Ik[_Im1_next], _U_Ik[_Im1_next],
-                                  _T_ik[_i_next])
+                                  _T_ik[_i_next], g)
             _W_Ik[_I_next] = W_Ik(_A_ik[_i_next], _E_Ik[_I_next], _a_ik[_i_next],
-                                  _W_Ik[_Im1_next], _U_Ik[_Im1_next], _T_ik[_i_next])
+                                  _W_Ik[_Im1_next], _U_Ik[_Im1_next], _T_ik[_i_next], g)
     return 1
 
-@njit
+@njit(int64(float64[:], float64[:], float64[:], float64[:], float64[:], float64[:], float64[:],
+            float64[:], float64[:], float64[:], float64[:], int64, int64[:], int64[:], int64[:]),
+      cache=True)
 def numba_backward_recurrence(_O_ik, _X_Ik, _Y_Ik, _Z_Ik, _a_ik, _b_ik, _c_ik,
                               _P_ik, _A_ik, _E_Ik, _D_Ik, NK, nk, _I_Nk, _i_nk):
+    g = 9.81
     for k in range(NK):
         _I_N = _I_Nk[k]
         _i_n = _i_nk[k]
         _I_Nm1 = _I_N - 1
         _i_nm1 = _i_n - 1
         _I_Np1 = _I_N + 1
         nlinks = nk[k]
         _O_ik[_i_n] = O_nk(_a_ik[_i_n], _b_ik[_i_n], _c_ik[_i_n])
-        _X_Ik[_I_N] = X_Nk(_A_ik[_i_n], _E_Ik[_I_N], _a_ik[_i_n], _O_ik[_i_n])
+        _X_Ik[_I_N] = X_Nk(_A_ik[_i_n], _E_Ik[_I_N], _a_ik[_i_n], _O_ik[_i_n], g)
         _Y_Ik[_I_N] = Y_Nk(_P_ik[_i_n], _D_Ik[_I_N], _a_ik[_i_n], _O_ik[_i_n],
                             _c_ik[_i_n], _D_Ik[_I_Np1])
-        _Z_Ik[_I_N] = Z_Nk(_A_ik[_i_n], _O_ik[_i_n], _c_ik[_i_n], _E_Ik[_I_Np1])
+        _Z_Ik[_I_N] = Z_Nk(_A_ik[_i_n], _O_ik[_i_n], _c_ik[_i_n], _E_Ik[_I_Np1], g)
         for i in range(nlinks - 1):
             _i_next = _i_nm1 - i
             _I_next = _I_Nm1 - i
             _Ip1_next = _I_next + 1
             _O_ik[_i_next] = O_ik(_a_ik[_i_next], _b_ik[_i_next], _c_ik[_i_next],
-                                  _A_ik[_i_next], _E_Ik[_Ip1_next], _X_Ik[_Ip1_next])
+                                  _A_ik[_i_next], _E_Ik[_Ip1_next], _X_Ik[_Ip1_next], g)
             _X_Ik[_I_next] = X_Ik(_A_ik[_i_next], _E_Ik[_I_next], _a_ik[_i_next],
-                                  _O_ik[_i_next])
+                                  _O_ik[_i_next], g)
             _Y_Ik[_I_next] = Y_Ik(_P_ik[_i_next], _a_ik[_i_next], _D_Ik[_I_next],
                                   _D_Ik[_Ip1_next], _c_ik[_i_next], _A_ik[_i_next],
                                   _E_Ik[_Ip1_next], _Y_Ik[_Ip1_next], _X_Ik[_Ip1_next],
-                                  _O_ik[_i_next])
+                                  _O_ik[_i_next], g)
             _Z_Ik[_I_next] = Z_Ik(_A_ik[_i_next], _E_Ik[_Ip1_next], _c_ik[_i_next],
-                                  _Z_Ik[_Ip1_next], _X_Ik[_Ip1_next], _O_ik[_i_next])
+                                  _Z_Ik[_Ip1_next], _X_Ik[_Ip1_next], _O_ik[_i_next], g)
     return 1
 
-@njit
+@njit(float64[:,:](float64[:,:], int64, int64),
+      cache=True)
 def numba_create_banded(l, bandwidth, M):
     AB = np.zeros((2*bandwidth + 1, M))
     for i in range(M):
         AB[bandwidth, i] = l[i, i]
     for n in range(bandwidth):
         for j in range(M - n - 1):
             AB[bandwidth - n - 1, -j - 1] = l[-j - 2 - n, -j - 1]
             AB[bandwidth + n + 1, j] = l[j + n + 1, j]
     return AB
 
-@njit(fastmath=True)
+@njit(void(float64[:], int64[:], float64[:]),
+      cache=True,
+      fastmath=True)
 def numba_add_at(a, indices, b):
     n = len(indices)
     for k in range(n):
         i = indices[k]
         a[i] += b[k]
 
-@njit
+@njit(void(float64[:, :], boolean[:], int64[:], int64[:], int64),
+      cache=True)
 def numba_clear_off_diagonals(A, bc, _J_uk, _J_dk, NK):
     for k in range(NK):
         _J_u = _J_uk[k]
         _J_d = _J_dk[k]
         _bc_u = bc[_J_u]
         _bc_d = bc[_J_d]
         if not _bc_u:
             A[_J_u, _J_d] = 0.0
         if not _bc_d:
             A[_J_d, _J_u] = 0.0
 
-@njit(fastmath=True)
+@njit(void(float64[:, :], float64[:], boolean[:], int64[:], int64[:], float64[:],
+           float64[:], float64[:], float64[:], float64[:], float64[:], float64[:],
+           float64, int64, int64),
+      cache=True,
+      fastmath=True)
 def numba_create_A_matrix(A, _F_jj, bc, _J_uk, _J_dk, _alpha_uk,
-                          _alpha_dk, _beta_uk, _beta_dk, _A_sj, _dt,
-                          M, NK):
+                          _alpha_dk, _beta_uk, _beta_dk, _xi_uk, _xi_dk,
+                          _A_sj, _dt, M, NK):
     numba_add_at(_F_jj, _J_uk, _alpha_uk)
     numba_add_at(_F_jj, _J_dk, -_beta_dk)
+    numba_add_at(_F_jj, _J_uk, _xi_uk)
+    numba_add_at(_F_jj, _J_dk, _xi_dk)
     _F_jj += (_A_sj / _dt)
     # Set diagonal of A matrix
     for i in range(M):
         if bc[i]:
             A[i,i] = 1.0
         else:
             A[i,i] = _F_jj[i]
@@ -2618,15 +2885,18 @@
         _bc_u = bc[_J_u]
         _bc_d = bc[_J_d]
         if not _bc_u:
             A[_J_u, _J_d] += _beta_uk[k]
         if not _bc_d:
             A[_J_d, _J_u] -= _alpha_dk[k]
 
-@njit(fastmath=True)
+@njit(void(float64[:, :], float64[:], boolean[:], int64[:], int64[:], float64[:],
+           float64[:], float64[:], float64[:], int64, int64),
+      cache=True,
+      fastmath=True)
 def numba_create_OWP_matrix(X, diag, bc, _J_uc, _J_dc, _alpha_uc,
                             _alpha_dc, _beta_uc, _beta_dc, M, NC):
     # Set diagonal
     numba_add_at(diag, _J_uc, _alpha_uc)
     numba_add_at(diag, _J_dc, -_beta_dc)
     for i in range(M):
         if bc[i]:
@@ -2640,42 +2910,47 @@
         _bc_u = bc[_J_u]
         _bc_d = bc[_J_d]
         if not _bc_u:
             X[_J_u, _J_d] += _beta_uc[c]
         if not _bc_d:
             X[_J_d, _J_u] -= _alpha_dc[c]
 
-@njit
+@njit(float64[:](float64[:], float64[:], float64[:], float64[:], float64[:], int64[:], int64[:], int64),
+      cache=True)
 def numba_Q_i_next_b(X_Ik, h_Ik, Y_Ik, Z_Ik, h_Np1k, _Ik, _ki, n):
     _Q_i = np.zeros(n)
     for i in range(n):
         I = _Ik[i]
         k = _ki[i]
         t_0 = X_Ik[I] * h_Ik[I]
         t_1 = Y_Ik[I]
         t_2 = Z_Ik[I] * h_Np1k[k]
         _Q_i[i] = t_0 + t_1 + t_2
     return _Q_i
 
-@njit
+@njit(float64[:](float64[:], float64[:], float64[:], float64[:], float64[:], int64[:], int64[:], int64),
+      cache=True)
 def numba_Q_im1k_next_f(U_Ik, h_Ik, V_Ik, W_Ik, h_1k, _Ik, _ki, n):
     _Q_i = np.zeros(n)
     for i in range(n):
         I = _Ik[i]
         Ip1 = I + 1
         k = _ki[i]
         t_0 = U_Ik[I] * h_Ik[Ip1]
         t_1 = V_Ik[I]
         t_2 = W_Ik[I] * h_1k[k]
         _Q_i[i] = t_0 + t_1 + t_2
     return _Q_i
 
-@njit
+@njit(void(float64[:], float64[:], float64[:], float64[:], float64[:], float64[:],
+           float64[:], float64[:], float64[:], float64[:], int64[:], int64[:], int64[:],
+           int64[:], int64[:], int64, boolean[:]),
+      cache=True)
 def numba_reposition_junctions(_x_Ik, _z_inv_Ik, _h_Ik, _dx_ik, _Q_ik, _H_dk,
-                               _b0, _z0, _x0, _m, _elem_pos, _i_1k, _I_1k,
+                               _b0, _zc, _xc, _m, _elem_pos, _i_1k, _I_1k,
                                _I_Np1k, nk, NK, reposition):
     for k in range(NK):
         if reposition[k]:
             _i_1 = _i_1k[k]
             _I_1 = _I_1k[k]
             _I_Np1 = _I_Np1k[k]
             nlinks = nk[k]
@@ -2691,21 +2966,19 @@
             _z_inv_I = _z_inv_Ik[_I_1:_I_end]
             _h_I = _h_Ik[_I_1:_I_end]
             _dx_i = _dx_ik[_i_1:_i_end]
             # Move junction if downstream head is within range
             move_junction = (_H_d > _z_inv_Np1) & (_H_d < _z_inv_1)
             if move_junction:
                 z_m = _H_d
-                x_m = (_H_d - _b0[k]) / _m[k]
+                _x0 = _x_I[_I_1]
+                x_m = (_H_d - _b0[k]) / _m[k] + _x0
             else:
-                z_m = _z0[k]
-                x_m = _x0[k]
-                # NOTE: Changing this to not move instead
-                # z_m = _z_inv_I[pos_prev]
-                # x_m = _x_I[pos_prev]
+                z_m = _zc[k]
+                x_m = _xc[k]
             # Determine new x-position of junction
             c = np.searchsorted(_x_I, x_m)
             cm1 = c - 1
             # Compute fractional x-position along superlink k
             frac = (x_m - _x_I[cm1]) / (_x_I[c] - _x_I[cm1])
             # Interpolate depth at new position
             h_m = (1 - frac) * _h_I[cm1] + (frac) * _h_I[c]
@@ -2724,16 +2997,14 @@
             _dx_ik[_i_1:_i_end] = _dx_i
             # Set position to new position
             pos_change = np.argsort(Ix)
             pos_next = pos_change[pos_prev]
             _elem_pos[k] = pos_next
             shifted = (pos_prev != pos_next)
             # If position has shifted interpolate flow
-            # TODO: For testing only, remove this later
-            # r = 0.5
             if shifted:
                 ix = np.arange(nlinks)
                 ix[pos_prev] = pos_next
                 ix.sort()
                 _Q_i = _Q_ik[_i_1:_i_end]
                 _Q_i[pos_prev - 1] = (1 - r) * _Q_i[pos_prev - 1] + r * _Q_i[pos_prev]
                 _Q_ik[_i_1:_i_end] = _Q_i[ix]
```

### Comparing `pipedream-solver-0.2/pipedream_solver/superlink.py` & `pipedream-solver-0.2.2/pipedream_solver/superlink.py`

 * *Files 6% similar despite different names*

```diff
@@ -269,33 +269,35 @@
     Q_w      : Weir flows (m^3/s)
     Q_p      : Pump flows (m^3/s)
     A_ik     : Cross-sectional area of flow in links (m^2)
     Pe_ik    : Wetted perimeter in links (m)
     R_ik     : Hydraulic radius in links (m)
     B_ik     : Top width of flow in links (m)
     A_sj     : Superjunction surface areas (m^2)
-    V_sj     : Superjunction stored volumes (m^3)
+    V_j      : Superjunction stored volumes (m^3)
     z_inv_j  : Superjunction invert elevation (m)
     z_inv_uk : Offset of superlink upstream invert above superjunction (m)
     z_inv_dk : Offset of superlink downstream invert above superjunction (m)
     """
     def __init__(self, superlinks, superjunctions,
                  links=None, junctions=None,
                  transects={}, storages={},
                  orifices=None, weirs=None, pumps=None,
                  dt=60, sparse=False, min_depth=1e-5, method='b',
                  inertial_damping=False, bc_method='z',
                  exit_hydraulics=False, auto_permute=False,
-                 end_length=None, end_method='b', internal_links=4):
+                 end_length=None, end_method='b', internal_links=4,
+                 mobile_elements=False):
         # Copy input tables to prevent modification
         superjunctions = copy.deepcopy(superjunctions)
         superlinks = copy.deepcopy(superlinks)
         orifices = copy.deepcopy(orifices)
         weirs = copy.deepcopy(weirs)
         pumps = copy.deepcopy(pumps)
+        # TODO: Ensure index is int
         # TODO: This needs to be done for orifices/weirs/pumps as well
         # Ensure nominal direction of superlinks is correct
         if (superlinks is not None) and (superjunctions is not None):
             for k in superlinks.index.values:
                 sj_0 = superlinks.loc[k, 'sj_0']
                 sj_1 = superlinks.loc[k, 'sj_1']
                 z_inv_0 = superjunctions.loc[sj_0, 'z_inv']
@@ -332,57 +334,87 @@
             self.permutations = np.arange(len(superjunctions))
             self.banded = False
         # TODO: What about id?
         if not 'map_x' in self.superjunctions.columns:
             self.superjunctions['map_x'] = 0.
         if not 'map_y' in self.superjunctions.columns:
             self.superjunctions['map_y'] = 0.
-        self._map_x_j = self.superjunctions['map_x'].values.astype(float)
-        self._map_y_j = self.superjunctions['map_y'].values.astype(float)
+        self._map_x_j = self.superjunctions['map_x'].values.astype(np.float64)
+        self._map_y_j = self.superjunctions['map_y'].values.astype(np.float64)
         if 'name' in self.superjunctions.columns:
             self.superjunction_names = self.superjunctions['name'].values
         else:
             self.superjunction_names = self.superjunctions.index.values
         if 'name' in self.superlinks.columns:
             self.superlink_names = self.superlinks['name'].values
         else:
             self.superlink_names = self.superlinks.index.values
+        if not 'friction_method' in self.superlinks.columns:
+            self.superlinks['friction_method'] = 'cm'
+        if 'n' in self.superlinks.columns:
+            if not 'roughness' in self.superlinks.columns:
+                self.superlinks = self.superlinks.rename(columns={'n' : 'roughness'})
+        if 'dx_uk' in self.superlinks:
+            self._dx_uk = self.superlinks['dx_uk'].values.astype(np.float64)
+        else:
+            self._dx_uk = np.zeros(self.NK, dtype=np.float64)
+        if 'dx_dk' in self.superlinks:
+            self._dx_dk = self.superlinks['dx_dk'].values.astype(np.float64)
+        else:
+            self._dx_dk = np.zeros(self.NK, dtype=np.float64)
+        # Handle invert elevations
+        self.min_depth = min_depth
+        self._z_inv_j = self.superjunctions['z_inv'].values.astype(np.float64)
+        self.H_j = self.superjunctions['h_0'].values.astype(np.float64) + self._z_inv_j
+        # Enforce minimum depth
+        self.H_j = np.maximum(self.H_j, self._z_inv_j + self.min_depth)
+        # Coefficients for head at upstream ends of superlink k
+        self._J_uk = self.superlinks['sj_0'].values.astype(np.int64)
+        # Coefficients for head at downstream ends of superlink k
+        self._J_dk = self.superlinks['sj_1'].values.astype(np.int64)
+        in_offset = superlinks['in_offset'].values.astype(np.float64)
+        out_offset = superlinks['out_offset'].values.astype(np.float64)
+        self._z_inv_uk = self._z_inv_j[self._J_uk] + in_offset
+        self._z_inv_dk = self._z_inv_j[self._J_dk] + out_offset
         # If internal links and junctions are not provided, create them
+        self.mobile_elements = mobile_elements
         if (links is None) or (junctions is None):
             generate_elems = True
-            self._configure_internals_variable(njunctions_fixed=internal_links)
+            self._configure_internals_variable(internal_links=internal_links,
+                                               mobile_elements=mobile_elements)
             links = self.links
             junctions = self.junctions
         else:
+            if mobile_elements:
+                raise ValueError('Cannot use mobile elements if supplying link and junction tables.')
             generate_elems = False
             self.links = links
             self.junctions = junctions
         self.NIk = self.junctions.shape[0]
         self.Nik = self.links.shape[0]
         self.transects = transects
         self.storages = storages
         self._dt = dt
         self._sparse = sparse
         self._method = method
         self._bc_method = bc_method
         self._end_method = end_method
         self._exit_hydraulics = exit_hydraulics
         self.inertial_damping = inertial_damping
-        self.min_depth = min_depth
-        self._I = junctions.index.values
-        self._ik = links.index.values
+        self._I = junctions.index.values.astype(np.int64)
+        self._ik = links.index.values.astype(np.int64)
         self._i = self._ik
-        self._Ik = links['j_0'].values.astype(int)
-        self._Ip1k = links['j_1'].values.astype(int)
-        self._kI = junctions['k'].values.astype(int)
-        self._ki = links['k'].values.astype(int)
-        self.start_nodes = self.superlinks['j_0'].values.astype(int)
-        self.end_nodes = self.superlinks['j_1'].values.astype(int)
-        self._is_start = np.zeros(self._I.size, dtype=bool)
-        self._is_end = np.zeros(self._I.size, dtype=bool)
+        self._Ik = links['j_0'].values.astype(np.int64)
+        self._Ip1k = links['j_1'].values.astype(np.int64)
+        self._kI = junctions['k'].values.astype(np.int64)
+        self._ki = links['k'].values.astype(np.int64)
+        self.start_nodes = self.superlinks['j_0'].values.astype(np.int64)
+        self.end_nodes = self.superlinks['j_1'].values.astype(np.int64)
+        self._is_start = np.zeros(self._I.size, dtype=np.bool8)
+        self._is_end = np.zeros(self._I.size, dtype=np.bool8)
         self._is_start[self.start_nodes] = True
         self._is_end[self.end_nodes] = True
         self.middle_nodes = self._I[(~self._is_start) & (~self._is_end)]
         self._is_penult = np.roll(self._is_end, -1)
         # Dimensions
         self.nk = np.bincount(self._ki)
         # Create forward and backward indexers
@@ -398,259 +430,282 @@
         self.backward_I_i[self.start_nodes] = self.forward_I_i[self.start_nodes]
         # Handle channel geometries
         self._shape_ik = links['shape']
         if transects:
             self._transect_ik = links['ts']
         else:
             self._transect_ik = None
-        self._g1_ik = links['g1'].values.astype(float)
-        self._g2_ik = links['g2'].values.astype(float)
-        self._g3_ik = links['g3'].values.astype(float)
-        self._Q_ik = links['Q_0'].values.astype(float)
-        self._dx_ik = links['dx'].values.astype(float)
-        self._n_ik = links['n'].values.astype(float)
-        self._ctrl = links['ctrl'].values.astype(bool)
-        self._A_c_ik = links['A_c'].values.astype(float)
-        self._C_ik = links['C'].values.astype(float)
+        # Handle hydraulic geometries g1, g2, ..., g6 , and g7
+        for i in range(1, 8):
+            geom_number = f'g{i}'
+            if geom_number in links.columns:
+                setattr(self, f'_{geom_number}_ik',
+                        links[geom_number].values.astype(np.float64))
+            else:
+                setattr(self, f'_{geom_number}_ik',
+                        np.zeros(links.shape[0], dtype=np.float64))
+        self._Q_ik = links['Q_0'].values.astype(np.float64)
+        self._dx_ik = links['dx'].values.astype(np.float64)
+        # friction slope method
+        if 'friction_method' in links:
+            _Sf_method = links['friction_method']
+        else:
+            _Sf_method = pd.Series(['cm']*len(links))
+        Sf_map = {'cm' : 0, 'hw' : 1, 'dw' : 2}
+        try:
+            assert _Sf_method.isin(Sf_map).all()
+        except:
+            raise ValueError('Friction method must be one of cm, hw, dw.')
+        self._Sf_method_ik = _Sf_method.map(Sf_map).astype(np.int64).values
+        if 'roughness' in links:
+            self._n_ik = links['roughness'].values.astype(np.float64)
+        else:
+            self._n_ik = links['n'].values.astype(np.float64)
+        self._ctrl = links['ctrl'].values.astype(np.bool8)
+        self._A_c_ik = links['A_c'].values.astype(np.float64)
+        self._C_ik = links['C'].values.astype(np.float64)
         self._storage_type = superjunctions['storage']
         if storages:
             self._storage_table = superjunctions['table']
         else:
             self._storage_table = None
-        self._storage_a = superjunctions['a'].values.astype(float)
-        self._storage_b = superjunctions['b'].values.astype(float)
-        self._storage_c = superjunctions['c'].values.astype(float)
+        self._storage_a = superjunctions['a'].values.astype(np.float64)
+        self._storage_b = superjunctions['b'].values.astype(np.float64)
+        self._storage_c = superjunctions['c'].values.astype(np.float64)
         # Set maximum superjunction depth
         if 'max_depth' in superjunctions:
-            self.max_depth = superjunctions['max_depth'].values.astype(float)
+            self.max_depth = superjunctions['max_depth'].values.astype(np.float64)
         else:
-            self.max_depth = np.full(len(superjunctions), np.inf, dtype=float)
+            self.max_depth = np.full(len(superjunctions), np.inf, dtype=np.float64)
         # Set maximum superlink depth for stability
         if 'max_depth' in superlinks:
-            self.max_depth_k = superlinks['max_depth'].values.astype(float)
+            self.max_depth_k = superlinks['max_depth'].values.astype(np.float64)
         else:
-            self.max_depth_k = np.full(len(superlinks), np.inf, dtype=float)
+            self.max_depth_k = np.full(len(superlinks), np.inf, dtype=np.float64)
         if 'C_uk' in superlinks:
-            self._C_uk = superlinks['C_uk'].values.astype(float)
+            self._C_uk = superlinks['C_uk'].values.astype(np.float64)
         else:
-            self._C_uk = 0.67 * np.ones(self.NK)
+            self._C_uk = (1 / (0.67**2)) * np.ones(self.NK, dtype=np.float64)
         if 'C_dk' in superlinks:
-            self._C_dk = superlinks['C_dk'].values.astype(float)
+            self._C_dk = superlinks['C_dk'].values.astype(np.float64)
         else:
-            self._C_dk = 0.67 * np.ones(self.NK)
-        self._h_Ik = junctions.loc[self._I, 'h_0'].values.astype(float)
-        self._A_SIk = junctions.loc[self._I, 'A_s'].values.astype(float)
-        self._z_inv_Ik = junctions.loc[self._I, 'z_inv'].values.astype(float)
+            self._C_dk = (1 / (0.67**2)) * np.ones(self.NK, dtype=np.float64)
+        self._h_Ik = junctions.loc[self._I, 'h_0'].values.astype(np.float64)
+        self._A_SIk = junctions.loc[self._I, 'A_s'].values.astype(np.float64)
+        self._z_inv_Ik = junctions.loc[self._I, 'z_inv'].values.astype(np.float64)
         self._S_o_ik = ((self._z_inv_Ik[self._Ik] - self._z_inv_Ik[self._Ip1k])
                         / self._dx_ik)
-        self._x_Ik = np.zeros(self._I.size)
-        self._x_Ik[~self._is_start] = links.groupby('k')['dx'].cumsum().values
+        self._x_Ik = np.zeros(self._I.size, dtype=np.float64)
+        self._x_Ik[~self._is_start] = links.groupby('k')['dx'].cumsum().values + self._dx_uk[self._ki]
+        self._x_Ik[self._is_start] = self._dx_uk
         # TODO: Allow specifying initial flows
-        self._Q_0Ik = np.zeros(self._I.size, dtype=float)
+        self._Q_0Ik = np.zeros(self._I.size, dtype=np.float64)
         # Handle orifices
         if orifices is not None:
             self.n_o = self.orifices.shape[0]
-            self._J_uo = self.orifices['sj_0'].values.astype(int)
-            self._J_do = self.orifices['sj_1'].values.astype(int)
-            self._Ao_max = self.orifices['A'].values.astype(float)
+            self._J_uo = self.orifices['sj_0'].values.astype(np.int64)
+            self._J_do = self.orifices['sj_1'].values.astype(np.int64)
+            self._Ao_max = self.orifices['A'].values.astype(np.float64)
             self._Ao = np.copy(self._Ao_max)
-            self._Co = self.orifices['C'].values.astype(float)
-            self._z_o = self.orifices['z_o'].values.astype(float)
-            self._y_max_o = self.orifices['y_max'].values.astype(float)
+            self._Co = self.orifices['C'].values.astype(np.float64)
+            self._z_o = self.orifices['z_o'].values.astype(np.float64)
+            self._y_max_o = self.orifices['y_max'].values.astype(np.float64)
             self._orient_o = self.orifices['orientation'].values
-            self._tau_o = (self._orient_o == 'side').astype(float)
+            self._tau_o = (self._orient_o == 'side').astype(np.float64)
             if 'shape' in self.orifices.columns:
                 self._shape_o = self.orifices['shape']
-                self._g1_o = self.orifices['g1'].values.astype(float)
-                self._g2_o = self.orifices['g2'].values.astype(float)
-                self._g3_o = self.orifices['g3'].values.astype(float)
+                self._g1_o = self.orifices['g1'].values.astype(np.float64)
+                self._g2_o = self.orifices['g2'].values.astype(np.float64)
+                self._g3_o = self.orifices['g3'].values.astype(np.float64)
             else:
                 self._shape_o = pd.Series(['rect_open'] * self.n_o)
                 self._g1_o = np.sqrt(self._Ao_max)
                 self._g2_o = np.sqrt(self._Ao_max)
                 self._g3_o = np.zeros(self.n_o)
-            self._Qo = np.zeros(self.n_o, dtype=float)
-            self._alpha_o = np.zeros(self.n_o, dtype=float)
-            self._beta_o = np.zeros(self.n_o, dtype=float)
-            self._chi_o = np.zeros(self.n_o, dtype=float)
-            self._alpha_uom = np.zeros(self.M, dtype=float)
-            self._beta_dol = np.zeros(self.M, dtype=float)
-            self._chi_uol = np.zeros(self.M, dtype=float)
-            self._chi_dom = np.zeros(self.M, dtype=float)
-        else:
-            self._J_uo = np.array([], dtype=int)
-            self._J_do = np.array([], dtype=int)
-            self._Ao_max = np.array([], dtype=float)
-            self._Ao = np.array([], dtype=float)
-            self._Co = np.array([], dtype=float)
-            self._z_o = np.array([], dtype=float)
-            self._y_max_o = np.array([], dtype=float)
+            self._Qo = np.zeros(self.n_o, dtype=np.float64)
+            self._alpha_o = np.zeros(self.n_o, dtype=np.float64)
+            self._beta_o = np.zeros(self.n_o, dtype=np.float64)
+            self._chi_o = np.zeros(self.n_o, dtype=np.float64)
+            self._alpha_uom = np.zeros(self.M, dtype=np.float64)
+            self._beta_dol = np.zeros(self.M, dtype=np.float64)
+            self._chi_uol = np.zeros(self.M, dtype=np.float64)
+            self._chi_dom = np.zeros(self.M, dtype=np.float64)
+        else:
+            self._J_uo = np.array([], dtype=np.int64)
+            self._J_do = np.array([], dtype=np.int64)
+            self._Ao_max = np.array([], dtype=np.float64)
+            self._Ao = np.array([], dtype=np.float64)
+            self._Co = np.array([], dtype=np.float64)
+            self._z_o = np.array([], dtype=np.float64)
+            self._y_max_o = np.array([], dtype=np.float64)
             self._orient_o = np.array([])
             self._shape_o = pd.Series(np.array([]))
-            self._g1_o = np.array([], dtype=float)
-            self._g2_o = np.array([], dtype=float)
-            self._g3_o = np.array([], dtype=float)
+            self._g1_o = np.array([], dtype=np.float64)
+            self._g2_o = np.array([], dtype=np.float64)
+            self._g3_o = np.array([], dtype=np.float64)
             self.n_o = 0
-            self._Qo = np.array([], dtype=float)
-            self._alpha_o = np.array([], dtype=float)
-            self._beta_o = np.array([], dtype=float)
-            self._chi_o = np.array([], dtype=float)
-            self._alpha_uom = np.array([], dtype=float)
-            self._beta_dol = np.array([], dtype=float)
-            self._chi_uol = np.array([], dtype=float)
-            self._chi_dom = np.array([], dtype=float)
+            self._Qo = np.array([], dtype=np.float64)
+            self._alpha_o = np.array([], dtype=np.float64)
+            self._beta_o = np.array([], dtype=np.float64)
+            self._chi_o = np.array([], dtype=np.float64)
+            self._alpha_uom = np.array([], dtype=np.float64)
+            self._beta_dol = np.array([], dtype=np.float64)
+            self._chi_uol = np.array([], dtype=np.float64)
+            self._chi_dom = np.array([], dtype=np.float64)
         # Handle weirs
         if weirs is not None:
-            self._J_uw = self.weirs['sj_0'].values.astype(int)
-            self._J_dw = self.weirs['sj_1'].values.astype(int)
-            self._Cwr = self.weirs['Cr'].values.astype(float)
-            self._Cwt = self.weirs['Ct'].values.astype(float)
-            self._L_w = self.weirs['L'].values.astype(float)
-            self._s_w = self.weirs['s'].values.astype(float)
-            self._z_w = self.weirs['z_w'].values.astype(float)
-            self._y_max_w = self.weirs['y_max'].values.astype(float)
+            self._J_uw = self.weirs['sj_0'].values.astype(np.int64)
+            self._J_dw = self.weirs['sj_1'].values.astype(np.int64)
+            self._Cwr = self.weirs['Cr'].values.astype(np.float64)
+            self._Cwt = self.weirs['Ct'].values.astype(np.float64)
+            self._L_w = self.weirs['L'].values.astype(np.float64)
+            self._s_w = self.weirs['s'].values.astype(np.float64)
+            self._z_w = self.weirs['z_w'].values.astype(np.float64)
+            self._y_max_w = self.weirs['y_max'].values.astype(np.float64)
             self.n_w = self.weirs.shape[0]
-            self._Hw = np.zeros(self.n_w, dtype=float)
-            self._Qw = np.zeros(self.n_w, dtype=float)
-            self._alpha_w = np.zeros(self.n_w, dtype=float)
-            self._beta_w = np.zeros(self.n_w, dtype=float)
-            self._chi_w = np.zeros(self.n_w, dtype=float)
-            self._alpha_uwm = np.zeros(self.M, dtype=float)
-            self._beta_dwl = np.zeros(self.M, dtype=float)
-            self._chi_uwl = np.zeros(self.M, dtype=float)
-            self._chi_dwm = np.zeros(self.M, dtype=float)
-        else:
-            self._J_uw = np.array([], dtype=int)
-            self._J_dw = np.array([], dtype=int)
-            self._Cwr = np.array([], dtype=float)
-            self._Cwt = np.array([], dtype=float)
-            self._L_w = np.array([], dtype=float)
-            self._s_w = np.array([], dtype=float)
-            self._z_w = np.array([], dtype=float)
-            self._y_max_w = np.array([], dtype=float)
+            self._Hw = np.zeros(self.n_w, dtype=np.float64)
+            self._Qw = np.zeros(self.n_w, dtype=np.float64)
+            self._alpha_w = np.zeros(self.n_w, dtype=np.float64)
+            self._beta_w = np.zeros(self.n_w, dtype=np.float64)
+            self._chi_w = np.zeros(self.n_w, dtype=np.float64)
+            self._alpha_uwm = np.zeros(self.M, dtype=np.float64)
+            self._beta_dwl = np.zeros(self.M, dtype=np.float64)
+            self._chi_uwl = np.zeros(self.M, dtype=np.float64)
+            self._chi_dwm = np.zeros(self.M, dtype=np.float64)
+        else:
+            self._J_uw = np.array([], dtype=np.int64)
+            self._J_dw = np.array([], dtype=np.int64)
+            self._Cwr = np.array([], dtype=np.float64)
+            self._Cwt = np.array([], dtype=np.float64)
+            self._L_w = np.array([], dtype=np.float64)
+            self._s_w = np.array([], dtype=np.float64)
+            self._z_w = np.array([], dtype=np.float64)
+            self._y_max_w = np.array([], dtype=np.float64)
             self.n_w = 0
-            self._Hw = np.array([], dtype=float)
-            self._Qw = np.array([], dtype=float)
-            self._alpha_w = np.array([], dtype=float)
-            self._beta_w = np.array([], dtype=float)
-            self._chi_w = np.array([], dtype=float)
-            self._alpha_uwm = np.array([], dtype=float)
-            self._beta_dwl = np.array([], dtype=float)
-            self._chi_uwl = np.array([], dtype=float)
-            self._chi_dwm = np.array([], dtype=float)
+            self._Hw = np.array([], dtype=np.float64)
+            self._Qw = np.array([], dtype=np.float64)
+            self._alpha_w = np.array([], dtype=np.float64)
+            self._beta_w = np.array([], dtype=np.float64)
+            self._chi_w = np.array([], dtype=np.float64)
+            self._alpha_uwm = np.array([], dtype=np.float64)
+            self._beta_dwl = np.array([], dtype=np.float64)
+            self._chi_uwl = np.array([], dtype=np.float64)
+            self._chi_dwm = np.array([], dtype=np.float64)
         # Handle pumps
         if pumps is not None:
-            self._J_up = self.pumps['sj_0'].values.astype(int)
-            self._J_dp = self.pumps['sj_1'].values.astype(int)
-            self._z_p = self.pumps['z_p'].values.astype(float)
-            self._ap_h = self.pumps['a_h'].values.astype(float)
-            self._ap_q = self.pumps['a_q'].values.astype(float)
-            self._dHp_max = self.pumps['dH_max'].values.astype(float)
-            self._dHp_min = self.pumps['dH_min'].values.astype(float)
+            self._J_up = self.pumps['sj_0'].values.astype(np.int64)
+            self._J_dp = self.pumps['sj_1'].values.astype(np.int64)
+            self._z_p = self.pumps['z_p'].values.astype(np.float64)
+            self._a_p = self.pumps['a_p'].values.astype(np.float64)
+            self._b_p = self.pumps['b_p'].values.astype(np.float64)
+            self._c_p = self.pumps['c_p'].values.astype(np.float64)
+            self._dHp_max = self.pumps['dH_max'].values.astype(np.float64)
+            self._dHp_min = self.pumps['dH_min'].values.astype(np.float64)
             self.n_p = self.pumps.shape[0]
-            self._Qp = np.zeros(self.n_p, dtype=float)
-            self._alpha_p = np.zeros(self.n_p, dtype=float)
-            self._beta_p = np.zeros(self.n_p, dtype=float)
-            self._chi_p = np.zeros(self.n_p, dtype=float)
-            self._alpha_upm = np.zeros(self.M, dtype=float)
-            self._beta_dpl = np.zeros(self.M, dtype=float)
-            self._chi_upl = np.zeros(self.M, dtype=float)
-            self._chi_dpm = np.zeros(self.M, dtype=float)
-        else:
-            self._J_up = np.array([], dtype=int)
-            self._J_dp = np.array([], dtype=int)
-            self._z_p = np.array([], dtype=float)
-            self._ap_h = np.array([], dtype=float)
-            self._ap_q = np.array([], dtype=float)
-            self._dHp_max = np.array([], dtype=float)
-            self._dHp_min = np.array([], dtype=float)
+            self._Qp = np.zeros(self.n_p, dtype=np.float64)
+            self._alpha_p = np.zeros(self.n_p, dtype=np.float64)
+            self._beta_p = np.zeros(self.n_p, dtype=np.float64)
+            self._chi_p = np.zeros(self.n_p, dtype=np.float64)
+            self._alpha_upm = np.zeros(self.M, dtype=np.float64)
+            self._beta_dpl = np.zeros(self.M, dtype=np.float64)
+            self._chi_upl = np.zeros(self.M, dtype=np.float64)
+            self._chi_dpm = np.zeros(self.M, dtype=np.float64)
+        else:
+            self._J_up = np.array([], dtype=np.int64)
+            self._J_dp = np.array([], dtype=np.int64)
+            self._z_p = np.array([], dtype=np.float64)
+            self._ap_h = np.array([], dtype=np.float64)
+            self._ap_q = np.array([], dtype=np.float64)
+            self._dHp_max = np.array([], dtype=np.float64)
+            self._dHp_min = np.array([], dtype=np.float64)
             self.n_p = 0
-            self._Qp = np.array([], dtype=float)
-            self._alpha_p = np.array([], dtype=float)
-            self._beta_p = np.array([], dtype=float)
-            self._chi_p = np.array([], dtype=float)
-            self._alpha_upm = np.array([], dtype=float)
-            self._beta_dpl = np.array([], dtype=float)
-            self._chi_upl = np.array([], dtype=float)
-            self._chi_dpm = np.array([], dtype=float)
+            self._Qp = np.array([], dtype=np.float64)
+            self._alpha_p = np.array([], dtype=np.float64)
+            self._beta_p = np.array([], dtype=np.float64)
+            self._chi_p = np.array([], dtype=np.float64)
+            self._alpha_upm = np.array([], dtype=np.float64)
+            self._beta_dpl = np.array([], dtype=np.float64)
+            self._chi_upl = np.array([], dtype=np.float64)
+            self._chi_dpm = np.array([], dtype=np.float64)
         # Enforce minimum depth
         self._h_Ik = np.maximum(self._h_Ik, self.min_depth)
         # Computational arrays
-        self._A_ik = np.zeros(self._ik.size)
-        self._Pe_ik = np.zeros(self._ik.size)
-        self._R_ik = np.zeros(self._ik.size)
-        self._B_ik = np.zeros(self._ik.size)
+        self._A_ik = np.zeros(self._ik.size, dtype=np.float64)
+        self._Pe_ik = np.zeros(self._ik.size, dtype=np.float64)
+        self._R_ik = np.zeros(self._ik.size, dtype=np.float64)
+        self._B_ik = np.zeros(self._ik.size, dtype=np.float64)
+        self._sigma_ik = np.ones(self._ik.size, dtype=np.float64)
         # Node velocities
-        self._u_ik = np.zeros(self._ik.size, dtype=float)
-        self._u_Ik = np.zeros(self._Ik.size, dtype=float)
-        self._u_Ip1k = np.zeros(self._Ip1k.size, dtype=float)
+        self._u_ik = np.zeros(self._ik.size, dtype=np.float64)
+        self._u_Ik = np.zeros(self._Ik.size, dtype=np.float64)
+        self._u_Ip1k = np.zeros(self._Ip1k.size, dtype=np.float64)
         # Node coefficients
         self._E_Ik = np.zeros(self._I.size)
         self._D_Ik = np.zeros(self._I.size)
         # Forward recurrence relations
-        self._I_end = np.zeros(self._I.size, dtype=bool)
+        self._I_end = np.zeros(self._I.size, dtype=np.bool8)
         self._I_end[self.end_nodes] = True
         self._I_1k = self.start_nodes
         self._I_2k = self.forward_I_I[self._I_1k]
         self._i_1k = self.forward_I_i[self._I_1k]
         self._k_1k = np.cumsum(self.nk - 1) - (self.nk[0] - 1)
         self._T_ik = np.zeros(self._ik.size)
         self._U_Ik = np.zeros(self._I.size)
         self._V_Ik = np.zeros(self._I.size)
         self._W_Ik = np.zeros(self._I.size)
         # Backward recurrence relations
-        self._I_start = np.zeros(self._I.size, dtype=bool)
+        self._I_start = np.zeros(self._I.size, dtype=np.bool8)
         self._I_start[self.start_nodes] = True
         self._I_Np1k = self.end_nodes
         self._I_Nk = self.backward_I_I[self._I_Np1k]
         self._i_nk = self.backward_I_i[self._I_Np1k]
         self._O_ik = np.zeros(self._ik.size)
         self._X_Ik = np.zeros(self._I.size)
         self._Y_Ik = np.zeros(self._I.size)
         self._Z_Ik = np.zeros(self._I.size)
         # Head at superjunctions
-        self._z_inv_j = self.superjunctions['z_inv'].values
-        self.H_j = self.superjunctions['h_0'].values + self._z_inv_j
+        # self._z_inv_j = self.superjunctions['z_inv'].values.astype(np.float64)
+        # self.H_j = self.superjunctions['h_0'].values.astype(np.float64) + self._z_inv_j
         # Enforce minimum depth
-        self.H_j = np.maximum(self.H_j, self._z_inv_j + self.min_depth)
+        # self.H_j = np.maximum(self.H_j, self._z_inv_j + self.min_depth)
         # Coefficients for head at upstream ends of superlink k
-        self._J_uk = self.superlinks['sj_0'].values.astype(int)
-        self._z_inv_uk = np.copy(self._z_inv_Ik[self._I_1k])
+        # self._J_uk = self.superlinks['sj_0'].values.astype(np.int64)
+        # self._z_inv_uk = np.copy(self._z_inv_Ik[self._I_1k])
         # Coefficients for head at downstream ends of superlink k
-        self._J_dk = self.superlinks['sj_1'].values.astype(int)
-        self._z_inv_dk = np.copy(self._z_inv_Ik[self._I_Np1k])
+        # self._J_dk = self.superlinks['sj_1'].values.astype(np.int64)
+        # self._z_inv_dk = np.copy(self._z_inv_Ik[self._I_Np1k])
         # Sparse matrix coefficients
         if sparse:
             self.A = scipy.sparse.lil_matrix((self.M, self.M))
         else:
             self.A = np.zeros((self.M, self.M))
         self.b = np.zeros(self.M)
         self.D = np.zeros(self.M)
-        self.bc = self.superjunctions['bc'].values.astype(bool)
+        self.bc = self.superjunctions['bc'].values.astype(np.bool8)
         if sparse:
             self.B = scipy.sparse.lil_matrix((self.M, self.n_o))
             self.O = scipy.sparse.lil_matrix((self.M, self.M))
             self.W = scipy.sparse.lil_matrix((self.M, self.M))
             self.P = scipy.sparse.lil_matrix((self.M, self.M))
         else:
             self.B = np.zeros((self.M, self.n_o))
             self.O = np.zeros((self.M, self.M))
             self.W = np.zeros((self.M, self.M))
             self.P = np.zeros((self.M, self.M))
         # TODO: Should these be size NK?
         self._theta_uk = np.ones(self.NK)
         self._theta_dk = np.ones(self.NK)
-        self._alpha_ukm = np.zeros(self.M, dtype=float)
-        self._beta_dkl = np.zeros(self.M, dtype=float)
-        self._chi_ukl = np.zeros(self.M, dtype=float)
-        self._chi_dkm = np.zeros(self.M, dtype=float)
-        self._k = self.superlinks.index.values
-        self._A_sj = np.zeros(self.M, dtype=float)
-        self._V_sj = np.zeros(self.M, dtype=float)
-        self._F_jj = np.zeros(self.M, dtype=float)
+        self._alpha_ukm = np.zeros(self.M, dtype=np.float64)
+        self._beta_dkl = np.zeros(self.M, dtype=np.float64)
+        self._chi_ukl = np.zeros(self.M, dtype=np.float64)
+        self._chi_dkm = np.zeros(self.M, dtype=np.float64)
+        self._k = self.superlinks.index.values.astype(np.int64)
+        self._A_sj = np.zeros(self.M, dtype=np.float64)
+        self._V_sj = np.zeros(self.M, dtype=np.float64)
+        self._F_jj = np.zeros(self.M, dtype=np.float64)
         # TODO: Allow initial input to be specified
         self._Q_0j = 0
         # Set upstream and downstream superlink variables
         self._Q_uk = self._Q_ik[self._i_1k]
         self._Q_dk = self._Q_ik[self._i_nk]
         self._h_uk = self._h_Ik[self._I_1k]
         self._h_dk = self._h_Ik[self._I_Np1k]
@@ -663,30 +718,45 @@
         self._A_dk = np.copy(self._A_ik[self._i_nk])
         self._B_uk = np.copy(self._B_ik[self._i_1k])
         self._B_dk = np.copy(self._B_ik[self._i_nk])
         self._Pe_uk = np.copy(self._Pe_ik[self._i_1k])
         self._Pe_dk = np.copy(self._Pe_ik[self._i_nk])
         self._R_uk = np.copy(self._R_ik[self._i_1k])
         self._R_dk = np.copy(self._R_ik[self._i_nk])
-        self._link_start = np.zeros(self._ik.size, dtype=bool)
-        self._link_end = np.zeros(self._ik.size, dtype=bool)
+        # End slopes
+        cond_uk = (self._dx_uk > 0.)
+        cond_dk = (self._dx_uk > 0.)
+        _S_o_uk = np.zeros(self.NK, dtype=np.float64)
+        _S_o_dk = np.zeros(self.NK, dtype=np.float64)
+        _S_o_uk[cond_uk] = (self._z_inv_uk - self._z_inv_Ik[self._I_1k])[cond_uk] / self._dx_uk[cond_uk]
+        _S_o_dk[cond_dk] = (self._z_inv_Ik[self._I_Np1k] - self._z_inv_dk)[cond_dk] / self._dx_dk[cond_dk]
+        self._S_o_uk = _S_o_uk
+        self._S_o_dk = _S_o_dk
+        # Boundary indexers
+        self._link_start = np.zeros(self._ik.size, dtype=np.bool8)
+        self._link_end = np.zeros(self._ik.size, dtype=np.bool8)
         self._link_start[self._i_1k] = True
         self._link_end[self._i_nk] = True
+        # End roughness
+        self._n_uk = np.copy(self._n_ik[self._i_1k])
+        self._n_dk = np.copy(self._n_ik[self._i_nk])
+        self._Sf_method_uk = np.copy(self._Sf_method_ik[self._i_1k])
+        self._Sf_method_dk = np.copy(self._Sf_method_ik[self._i_nk])
         self._h_c = np.zeros(self.NK)
         self._h_n = np.zeros(self.NK)
         # Set up hydraulic geometry computations
         self.configure_storages()
         self.configure_hydraulic_geometry()
         # Get superlink lengths
-        self._dx_k = np.zeros(self.NK, dtype=float)
+        self._dx_k = np.zeros(self.NK, dtype=np.float64)
         np.add.at(self._dx_k, self._ki, self._dx_ik)
-        self._Q_k = np.zeros(self.NK, dtype=float)
-        self._A_k = np.zeros(self.NK, dtype=float)
-        self._dt_ck = np.ones(self.NK, dtype=float)
-        self._Q_in = np.zeros(self.M, dtype=float)
+        self._Q_k = np.zeros(self.NK, dtype=np.float64)
+        self._A_k = np.zeros(self.NK, dtype=np.float64)
+        self._dt_ck = np.ones(self.NK, dtype=np.float64)
+        self._Q_in = np.zeros(self.M, dtype=np.float64)
         # Initialize state dictionary
         self.states = {}
         # Iteration counter
         self.iter_count = 0
         self.t = 0
         # Compute bandwidth
         self._compute_bandwidth()
@@ -757,14 +827,30 @@
         return self._A_ik
 
     @A_ik.setter
     def A_ik(self, value):
         self._A_ik = np.asarray(value)
 
     @property
+    def A_uk(self):
+        return self._A_uk
+
+    @A_uk.setter
+    def A_uk(self, value):
+        self._A_uk = np.asarray(value)
+
+    @property
+    def A_dk(self):
+        return self._A_dk
+
+    @A_dk.setter
+    def A_dk(self, value):
+        self._A_dk = np.asarray(value)
+
+    @property
     def Pe_ik(self):
         return self._Pe_ik
 
     @Pe_ik.setter
     def Pe_ik(self, value):
         self._Pe_ik = np.asarray(value)
 
@@ -789,19 +875,19 @@
         return self._A_sj
 
     @A_sj.setter
     def A_sj(self, value):
         self._A_sj = np.asarray(value)
 
     @property
-    def V_sj(self):
+    def V_j(self):
         return self._V_sj
 
-    @V_sj.setter
-    def V_sj(self, value):
+    @V_j.setter
+    def V_j(self, value):
         self._V_sj = np.asarray(value)
 
     @property
     def z_inv_j(self):
         return self._z_inv_j
 
     @z_inv_j.setter
@@ -903,52 +989,56 @@
         self.superjunctions = superjunctions
         self.superlinks = superlinks
         self.orifices = orifices
         self.weirs = weirs
         self.pumps = pumps
         self.permutations = permutations
 
-    def _configure_internals_variable(self, njunctions_fixed=4):
+    def _configure_internals_variable(self, internal_links=4, mobile_elements=True):
         # Import instance variables
         superlinks = self.superlinks            # Table of superlinks
         superjunctions = self.superjunctions    # Table of superjunctions
         # Set parameters
-        njunctions = njunctions_fixed + 1
+        njunctions = internal_links + 1
         nlinks = njunctions - 1
-        link_ncols = 15
-        junction_ncols = 5
+        link_columns = ['A_c', 'C', 'Q_0', 'ctrl', 'dx', 'g1', 'g2', 'g3',
+                         'g4', 'g5', 'g6', 'g7', 'id', 'j_0', 'j_1', 'k', 'n',
+                        'shape', 'friction_method']
+        junction_columns = ['A_s', 'h_0', 'id', 'k', 'z_inv']
+        link_ncols = len(link_columns)
+        junction_ncols = len(junction_columns)
         n_superlinks = len(superlinks)
         NJ = njunctions * n_superlinks
         NL = nlinks * n_superlinks
-        elems = np.repeat(njunctions_fixed, n_superlinks)
+        elems = np.repeat(internal_links, n_superlinks)
         total_elems = elems + 1
         upstream_nodes = np.cumsum(total_elems) - total_elems
         downstream_nodes = np.cumsum(total_elems) - 2
         # Configure links
         links = pd.DataFrame(np.zeros((NL, link_ncols)))
-        links.columns = ['A_c', 'C', 'Q_0', 'ctrl', 'dx', 'g1', 'g2', 'g3', 'g4',
-                        'id', 'j_0', 'j_1', 'k', 'n', 'shape']
+        links.columns = link_columns
         links['A_c'] = np.repeat(superlinks['A_c'].values, nlinks)
         links['C'] = np.repeat(superlinks['C'].values, nlinks)
         links['Q_0'] = np.repeat(superlinks['Q_0'].values, nlinks)
         links['ctrl'] = np.repeat(superlinks['ctrl'].values, nlinks)
         links['k'] = np.repeat(superlinks.index.values, nlinks)
         links['shape'] = np.repeat(superlinks['shape'].values, nlinks)
-        links['n'] = np.repeat(superlinks['n'].values, nlinks)
-        links['g1'] = np.repeat(superlinks['g1'].values, nlinks)
-        links['g2'] = np.repeat(superlinks['g2'].values, nlinks)
-        links['g3'] = np.repeat(superlinks['g3'].values, nlinks)
-        links['g4'] = np.repeat(superlinks['g4'].values, nlinks)
+        links['roughness'] = np.repeat(superlinks['roughness'].values, nlinks)
+        links['friction_method'] = np.repeat(superlinks['friction_method'].values, nlinks)
+        for i in range(1, 8):
+            geom_number = f'g{i}'
+            if geom_number in superlinks.columns:
+                links[geom_number] = np.repeat(superlinks[geom_number].values, nlinks)
         links['id'] = links.index.values
         j = np.arange(NJ)
         links['j_0'] = np.delete(j, downstream_nodes + 1)
         links['j_1'] = np.delete(j, upstream_nodes)
         # Configure junctions
         junctions = pd.DataFrame(np.zeros((NJ, junction_ncols)))
-        junctions.columns = ['A_s', 'h_0', 'id', 'k', 'z_inv']
+        junctions.columns = junction_columns
         junctions['A_s'] = np.repeat(superlinks['A_s'].values, njunctions)
         junctions['h_0'] = np.repeat(superlinks['h_0'].values, njunctions)
         junctions['k'] = np.repeat(superlinks.index.values, njunctions)
         junctions['id'] = junctions.index.values
         # Configure internal variables
         x = np.zeros(NJ)
         z = np.zeros(NJ)
@@ -957,44 +1047,61 @@
         Q = links['Q_0'].values
         xx = x.reshape(-1, njunctions)
         zz = z.reshape(-1, njunctions)
         dxdx = dx.reshape(-1, nlinks)
         hh = h.reshape(-1, njunctions)
         QQ = Q.reshape(-1, nlinks)
         dx_j = superlinks['dx'].values
-        _z_inv_j = superjunctions['z_inv'].values.astype(float)
-        inoffset = superlinks['in_offset'].values.astype(float)
-        outoffset = superlinks['out_offset'].values.astype(float)
-        _J_uk = superlinks['sj_0'].values.astype(int)
-        _J_dk = superlinks['sj_1'].values.astype(int)
-        if (njunctions % 2):
-            _x0 = (dx_j / 2)
-        else:
-            _x0 = (dx_j / 2) + (dx_j / nlinks / 2)
-        xx[:, :-1] = np.vstack([np.linspace(0, i, njunctions - 1)
-                                for i in dx_j])
-        xx[:, -1] = _x0
-        _b0 = _z_inv_j[_J_uk] + inoffset
-        _b1 = _z_inv_j[_J_dk] + outoffset
-        _m = (_b1 - _b0) / dx_j
-        _z0 = _m * _x0 + _b0
-        zz[:] = xx * _m.reshape(-1, 1) + _b0.reshape(-1, 1)
-        ix = np.argsort(xx)
-        _fixed = (ix < nlinks)
-        r, c = np.where(~_fixed)
-        cm1 = ix[r, c - 1]
-        cp1 = ix[r, c + 1]
-        frac = (xx[r, xx.shape[1] - 1] - xx[r, cm1]) / (xx[r, cp1] - xx[r, cm1])
-        # Set depths and flows
-        hh[:, -1] = (1 - frac) * hh[r, cm1] + (frac) * hh[r, cp1]
-        QQ[:, -1] = QQ[r, cm1]
-        # Write new variables
-        xx = np.take_along_axis(xx, ix, axis=-1)
-        zz = np.take_along_axis(zz, ix, axis=-1)
-        hh = np.take_along_axis(hh, ix, axis=-1)
+        _z_inv_uk = self._z_inv_uk
+        _z_inv_dk = self._z_inv_dk
+        _dx_uk = self._dx_uk
+        _dx_dk = self._dx_dk
+        # TODO: Should dx_uk, dx_dk be generated instead? Probably no, because then orifice cannot be represented.
+        _m = (_z_inv_dk - _z_inv_uk) / (dx_j + _dx_uk + _dx_dk)
+        _b0 = _z_inv_uk + _m * _dx_uk
+        _b1 = _z_inv_dk - _m * _dx_dk
+        if mobile_elements:
+            try:
+                assert (internal_links > 1)
+            except:
+                raise ValueError('If using mobile elements, must have more than one internal link.')
+            if (njunctions % 2):
+                _xc = (dx_j / 2)
+            else:
+                _xc = (dx_j / 2) + (dx_j / nlinks / 2)
+            xx[:, :-1] = np.vstack([np.linspace(0, i, njunctions - 1)
+                                    for i in dx_j])
+            # xx[:, :-1] = np.vstack([np.linspace(j, i + j + k, njunctions - 1)
+            #                         for i, j, k in zip(dx_j, _dx_uk, _dx_dk)])
+            xx[:, -1] = _xc
+            _zc = _m * _xc + _b0
+            zz[:] = xx * _m.reshape(-1, 1) + _b0.reshape(-1, 1)
+            ix = np.argsort(xx)
+            _fixed = (ix < nlinks)
+            r, c = np.where(~_fixed)
+            cm1 = ix[r, c - 1]
+            cp1 = ix[r, c + 1]
+            frac = (xx[r, xx.shape[1] - 1] - xx[r, cm1]) / (xx[r, cp1] - xx[r, cm1])
+            # Set depths and flows
+            hh[:, -1] = (1 - frac) * hh[r, cm1] + (frac) * hh[r, cp1]
+            QQ[:, -1] = QQ[r, cm1]
+            # Write new variables
+            xx = np.take_along_axis(xx, ix, axis=-1)
+            zz = np.take_along_axis(zz, ix, axis=-1)
+            hh = np.take_along_axis(hh, ix, axis=-1)
+        else:
+            xx[:, :] = np.vstack([np.linspace(0, i, njunctions)
+                                  for i in dx_j])
+            # xx[:, :] = np.vstack([np.linspace(j, i + j + k, njunctions)
+            #                       for i, j, k in zip(dx_j, _dx_uk, _dx_dk)])
+            zz[:] = xx * _m.reshape(-1, 1) + _b0.reshape(-1, 1)
+            _fixed = np.ones(xx.shape, dtype=np.bool8)
+            _xc = None
+            _zc = None
+            c = None
         dxdx = np.diff(xx)
         junctions['z_inv'] = zz.ravel()
         junctions['h_0'] = hh.ravel()
         links['dx'] = dxdx.ravel()
         links['Q_0'] = QQ.ravel()
         # Set start and end junctions on superlinks
         superlinks['j_0'] = links.groupby('k')['j_0'].min()
@@ -1004,16 +1111,16 @@
         self.links = links
         self.superlinks = superlinks
         self._fixed = _fixed
         self._elem_pos = c
         self._b0 = _b0
         self._b1 = _b1
         self._m = _m
-        self._x0 = _x0
-        self._z0 = _z0
+        self._xc = _xc
+        self._zc = _zc
 
     def safe_divide(function):
         """
         Allow for division by zero. Division by zero will return zero.
         """
         def inner(*args, **kwargs):
             num, den = function(*args, **kwargs)
@@ -1485,14 +1592,21 @@
         transects = self.transects          # Table of transects
         _shape_ik = self._shape_ik          # Shape of link ik
         _shape_o = self._shape_o
         _transect_ik = self._transect_ik    # Transect associated with link ik
         _link_start = self._link_start      # Link is first link in superlink k
         _link_end = self._link_end          # Link is last link in superlink k
         _geom_numbers = pipedream_solver.geometry.geom_code
+        _g1_ik = self._g1_ik
+        _g2_ik = self._g2_ik
+        _g3_ik = self._g3_ik
+        _g4_ik = self._g4_ik
+        _g5_ik = self._g5_ik
+        _g6_ik = self._g6_ik
+        _g7_ik = self._g7_ik
         nk = self.nk
         n_o = self.n_o
         # Set attributes
         _geom_factory = {}
         _geom_factory_o = {}
         _transect_factory = {}
         _transect_indices = None
@@ -1524,34 +1638,47 @@
                                           index=_irregular_transects.values)
             _uk_transect_indices = _transect_indices[_link_start[_transect_indices]]
             _dk_transect_indices = _transect_indices[_link_end[_transect_indices]]
             for transect_name, transect in transects.items():
                 _transect_factory[transect_name] = pipedream_solver.geometry.Irregular(**transect)
         # Create array of geom codes
         # TODO: Should have a variable that gives total number of links instead of summing
-        _geom_codes = np.zeros(nk.sum(), dtype=int)
+        _geom_codes = np.zeros(nk.sum(), dtype=np.int64)
         for geom, indices in _geom_factory.items():
             _geom_codes[indices] = _geom_numbers[geom]
         # NOTE: Handle case for elliptical geometry
         _ellipse_ix = np.flatnonzero(_geom_codes ==
                                      pipedream_solver.geometry.geom_code['elliptical'])
         # Handle orifices
         if n_o:
             _unique_geom_o = set(_shape_o.str.lower().unique())
             _geom_indices_o = pd.Series(_shape_o.index, index=_shape_o.str.lower().values)
             for geom in _unique_geom_o:
                 _o_g = _geom_indices_o.loc[[geom]].values
                 _geom_factory_o[geom] = _o_g
-            _geom_codes_o = np.zeros(n_o, dtype=int)
+            _geom_codes_o = np.zeros(n_o, dtype=np.int64)
             for geom, indices in _geom_factory_o.items():
                 _geom_codes_o[indices] = _geom_numbers[geom]
             # Export instance variables
             self._geom_factory_o = _geom_factory_o
             self._geom_codes_o = _geom_codes_o
-        # Export instance variables
+        # Add default Preissman slot for circular
+        _g2_ik[(_geom_codes == 1) & (_g2_ik == 0.)] = 0.001
+        # Add default Preissman slot for rect_closed
+        _g3_ik[(_geom_codes == 2) & (_g3_ik == 0.)] = 0.001
+        # Add default Preissman slot for force_main
+        _g2_ik[(_geom_codes == 9) & (_g2_ik == 0.)] = 0.001
+        # Export instance variables
+        self._g1_ik = _g1_ik
+        self._g2_ik = _g2_ik
+        self._g3_ik = _g3_ik
+        self._g4_ik = _g4_ik
+        self._g5_ik = _g5_ik
+        self._g6_ik = _g6_ik
+        self._g7_ik = _g7_ik
         self._has_irregular = _has_irregular
         self._geom_factory = _geom_factory
         self._transect_factory = _transect_factory
         self._transect_indices = _transect_indices
         self._uk_has_irregular = _uk_has_irregular
         self._dk_has_irregular = _dk_has_irregular
         self._uk_geom_factory = _uk_geom_factory
@@ -1783,15 +1910,15 @@
         _z_inv_j = self._z_inv_j
         # Compute effective head
         H_uo = H_j[_J_uo]
         H_do = H_j[_J_do]
         _z_inv_uo = _z_inv_j[_J_uo]
         h_e = np.maximum(H_uo - _z_inv_uo - _z_o, H_do - _z_inv_uo - _z_o)
         if u is None:
-            u = np.zeros(n_o, dtype=float)
+            u = np.zeros(n_o, dtype=np.float64)
         # Compute hydraulic geometry for regular geometries
         for geom, indices in _geom_factory_o.items():
             Geom = geom.title()
             _o_g = indices
             generator = getattr(pipedream_solver.geometry, Geom)
             _g1_g = _g1_o[_o_g] * u[_o_g]
             _g2_g = _g2_o[_o_g]
@@ -1964,23 +2091,21 @@
         if _dt is None:
             _dt = self._dt
         # Compute link coefficients
         _a_ik = self.a_ik(_u_Ik, _sigma_ik)
         _c_ik = self.c_ik(_u_Ip1k, _sigma_ik)
         _b_ik = self.b_ik(_dx_ik, _dt, _n_ik, _Q_ik, _A_ik, _R_ik,
                           _A_c_ik, _C_ik, _a_ik, _c_ik, _ctrl)
-        if first_iter:
-            _P_ik = self.P_ik(_Q_ik, _dx_ik, _dt, _A_ik, _S_o_ik,
-                            _sigma_ik)
+        _P_ik = self.P_ik(_Q_ik, _dx_ik, _dt, _A_ik, _S_o_ik,
+                        _sigma_ik)
         # Export to instance variables
         self._a_ik = _a_ik
         self._b_ik = _b_ik
         self._c_ik = _c_ik
-        if first_iter:
-            self._P_ik = _P_ik
+        self._P_ik = _P_ik
 
     def node_coeffs(self, _Q_0Ik=None, _dt=None, first_iter=True):
         """
         Compute nodal continuity coefficients: D_Ik and E_Ik.
         """
         # Import instance variables
         _I = self._I                         # Indices of all junctions
@@ -2010,27 +2135,26 @@
         _E_Ik[start_nodes] = self.E_Ik(_B_ik[start_links], _dx_ik[start_links],
                                         0.0, 0.0, _A_SIk[start_nodes], _dt)
         _E_Ik[end_nodes] = self.E_Ik(0.0, 0.0, _B_ik[end_links], _dx_ik[end_links],
                                         _A_SIk[end_nodes], _dt)
         _E_Ik[middle_nodes] = self.E_Ik(_B_ik[forward], _dx_ik[forward],
                                         _B_ik[backward], _dx_ik[backward],
                                         _A_SIk[middle_nodes], _dt)
-        if first_iter:
-            _D_Ik[start_nodes] = self.D_Ik(_Q_0Ik[start_nodes], _B_ik[start_links],
-                                            _dx_ik[start_links], 0.0,
-                                            0.0, _A_SIk[start_nodes],
-                                            _h_Ik[start_nodes], _dt)
-            _D_Ik[end_nodes] = self.D_Ik(_Q_0Ik[end_nodes], 0.0,
-                                            0.0, _B_ik[end_links],
-                                            _dx_ik[end_links], _A_SIk[end_nodes],
-                                            _h_Ik[end_nodes], _dt)
-            _D_Ik[middle_nodes] = self.D_Ik(_Q_0Ik[middle_nodes], _B_ik[forward],
-                                            _dx_ik[forward], _B_ik[backward],
-                                            _dx_ik[backward], _A_SIk[middle_nodes],
-                                            _h_Ik[middle_nodes], _dt)
+        _D_Ik[start_nodes] = self.D_Ik(_Q_0Ik[start_nodes], _B_ik[start_links],
+                                        _dx_ik[start_links], 0.0,
+                                        0.0, _A_SIk[start_nodes],
+                                        _h_Ik[start_nodes], _dt)
+        _D_Ik[end_nodes] = self.D_Ik(_Q_0Ik[end_nodes], 0.0,
+                                        0.0, _B_ik[end_links],
+                                        _dx_ik[end_links], _A_SIk[end_nodes],
+                                        _h_Ik[end_nodes], _dt)
+        _D_Ik[middle_nodes] = self.D_Ik(_Q_0Ik[middle_nodes], _B_ik[forward],
+                                        _dx_ik[forward], _B_ik[backward],
+                                        _dx_ik[backward], _A_SIk[middle_nodes],
+                                        _h_Ik[middle_nodes], _dt)
         # Export instance variables
         self._E_Ik = _E_Ik
         self._D_Ik = _D_Ik
 
     def forward_recurrence(self):
         """
         Compute forward recurrence coefficients: T_ik, U_Ik, V_Ik, and W_Ik.
@@ -2369,21 +2493,21 @@
         _Ao = self._Ao               # NOTE: Flow area of orifice now
         _tau_o = self._tau_o
         _alpha_o = self._alpha_o     # Orifice flow coefficient alpha_o
         _beta_o = self._beta_o       # Orifice flow coefficient beta_o
         _chi_o = self._chi_o         # Orifice flow coefficient chi_o
         # If no input signal, assume orifice is closed
         if u is None:
-            u = np.zeros(self.n_o, dtype=float)
+            u = np.zeros(self.n_o, dtype=np.float64)
         # Specify orifice heads at previous timestep
         _H_uo = H_j[_J_uo]
         _H_do = H_j[_J_do]
         _z_inv_uo = _z_inv_j[_J_uo]
         # Create indicator functions
-        _omega_o = (_H_uo >= _H_do).astype(float)
+        _omega_o = (_H_uo >= _H_do).astype(np.float64)
         # Compute universal coefficients
         _gamma_o = self.gamma_o(_Qo, _Ao, _Co)
         # Create conditionals
         cond_0 = (_omega_o * _H_uo + (1 - _omega_o) * _H_do >
                   _z_o + _z_inv_uo + (_tau_o * _y_max_o * u))
         cond_1 = ((1 - _omega_o) * _H_uo + _omega_o * _H_do >
                   _z_o + _z_inv_uo + (_tau_o * _y_max_o * u / 2))
@@ -2437,21 +2561,21 @@
         _L_w = self._L_w           # Transverse length of rectangular section
         _alpha_w = self._alpha_w   # Weir flow coefficient alpha_w
         _beta_w = self._beta_w     # Weir flow coefficient beta_w
         _chi_w = self._chi_w       # Weir flow coefficient chi_w
         _Hw = self._Hw             # Current effective head above weir w
         # If no input signal, assume weir is closed
         if u is None:
-            u = np.zeros(self.n_w, dtype=float)
+            u = np.zeros(self.n_w, dtype=np.float64)
         # Specify weir heads at previous timestep
         _H_uw = H_j[_J_uw]
         _H_dw = H_j[_J_dw]
         _z_inv_uw = _z_inv_j[_J_uw]
         # Create indicator functions
-        _omega_w = (_H_uw >= _H_dw).astype(float)
+        _omega_w = (_H_uw >= _H_dw).astype(np.float64)
         # Create conditionals
         cond_0 = (_omega_w * _H_uw + (1 - _omega_w) * _H_dw >
                   _z_w + _z_inv_uw + (1 - u) * _y_max_w)
         cond_1 = ((1 - _omega_w) * _H_uw + _omega_w * _H_dw >
                   _z_w + _z_inv_uw + (1 - u) * _y_max_w)
         # Effective heads
         a = (cond_0 & cond_1)
@@ -2503,15 +2627,15 @@
         _ap_q = self._ap_q          # Vertical axis length of elliptical pump curve
         _Qp = self._Qp              # Current flow rate through pump p
         _alpha_p = self._alpha_p    # Pump flow coefficient alpha_p
         _beta_p = self._beta_p      # Pump flow coefficient beta_p
         _chi_p = self._chi_p        # Pump flow coefficient chi_p
         # If no input signal, assume pump is closed
         if u is None:
-            u = np.zeros(self.n_p, dtype=float)
+            u = np.zeros(self.n_p, dtype=np.float64)
         # Specify pump heads at previous timestep
         _H_up = H_j[_J_up]
         _H_dp = H_j[_J_dp]
         _z_inv_up = _z_inv_j[_J_up]
         # Create conditionals
         assert (_dHp_min <= _dHp_max).all()
         _dHp = _H_dp - _H_up
@@ -2871,27 +2995,27 @@
         _y_max_o = self._y_max_o      # Maximum height of orifice o
         _Co = self._Co                # Discharge coefficient of orifice o
         _Ao = self._Ao                # Maximum flow area of orifice o
         _tau_o = self._tau_o
         _V_sj = self._V_sj
         # If no input signal, assume orifice is closed
         if u is None:
-            u = np.zeros(self.n_o, dtype=float)
+            u = np.zeros(self.n_o, dtype=np.float64)
         g = 9.81
         # Create arrays to store flow coefficients for current time step
-        _alpha_oo = np.zeros(self.n_o, dtype=float)
-        _beta_oo = np.zeros(self.n_o, dtype=float)
-        _chi_oo = np.zeros(self.n_o, dtype=float)
+        _alpha_oo = np.zeros(self.n_o, dtype=np.float64)
+        _beta_oo = np.zeros(self.n_o, dtype=np.float64)
+        _chi_oo = np.zeros(self.n_o, dtype=np.float64)
         # Specify orifice heads at previous timestep
         _H_uo = H_j[_J_uo]
         _H_do = H_j[_J_do]
         _z_inv_uo = _z_inv_j[_J_uo]
         # Create indicator functions
         upstream_ctrl = (_H_uo >= _H_do)
-        _omega_o = (upstream_ctrl).astype(float)
+        _omega_o = (upstream_ctrl).astype(np.float64)
         # Compute universal coefficients
         _gamma_oo = 2 * g * _Co**2 * _Ao**2
         # Create conditionals
         cond_0 = (_omega_o * _H_uo + (1 - _omega_o) * _H_do >
                   _z_o + _z_inv_uo + (_tau_o * _y_max_o * u))
         cond_1 = ((1 - _omega_o) * _H_uo + _omega_o * _H_do >
                   _z_o + _z_inv_uo + (_tau_o * _y_max_o * u / 2))
@@ -2944,21 +3068,21 @@
         _Cwr = self._Cwr            # Discharge coefficient of rectangular portion of weir w
         _Cwt = self._Cwt            # Discharge coefficient of triangular portion of weir w
         _s_w = self._s_w            # Inverse side slope of triangular portion of weir w
         _L_w = self._L_w            # Transverse length of rectangular portion of weir w
         _Hw = self._Hw              # Current effective head on weir w
         # If no input signal, assume weir is closed
         if u is None:
-            u = np.zeros(self.n_w, dtype=float)
+            u = np.zeros(self.n_w, dtype=np.float64)
         # Specify orifice heads at previous timestep
         _H_uw = H_j[_J_uw]
         _H_dw = H_j[_J_dw]
         _z_inv_uw = _z_inv_j[_J_uw]
         # Create indicator functions
-        _omega_w = (_H_uw >= _H_dw).astype(float)
+        _omega_w = (_H_uw >= _H_dw).astype(np.float64)
         # Create conditionals
         cond_0 = (_omega_w * _H_uw + (1 - _omega_w) * _H_dw >
                   _z_w + _z_inv_uw + (1 - u) * _y_max_w)
         cond_1 = ((1 - _omega_w) * _H_uw + _omega_w * _H_dw >
                   _z_w + _z_inv_uw + (1 - u) * _y_max_w)
         # Effective heads
         a = (cond_0 & cond_1)
@@ -2989,15 +3113,15 @@
         _dHp_max = self._dHp_max    # Maximum pump head difference
         _dHp_min = self._dHp_min    # Minimum pump head difference
         _ap_h = self._ap_h          # Horizontal axis length of elliptical pump curve
         _ap_q = self._ap_q          # Vertical axis length of elliptical pump curve
         _Qp = self._Qp              # Current flow rate through pump p
         # If no input signal, assume pump is closed
         if u is None:
-            u = np.zeros(self.n_p, dtype=float)
+            u = np.zeros(self.n_p, dtype=np.float64)
         # Specify pump heads at previous timestep
         _H_up = H_j[_J_up]
         _H_dp = H_j[_J_dp]
         _z_inv_up = _z_inv_j[_J_up]
         # Create conditionals
         _dHp = _H_dp - _H_up
         _dHp[_dHp > _dHp_max] = _dHp_max
@@ -3022,19 +3146,17 @@
         _lambda_dk = self._lambda_dk    # Superlink head coefficient
         _mu_uk = self._mu_uk            # Superlink head coefficient
         _mu_dk = self._mu_dk            # Superlink head coefficient
         _Q_uk = self._Q_uk              # Flow rate at upstream end of superlink k
         _Q_dk = self._Q_dk              # Flow rate at downstream end of superlink k
         H_j = self.H_j                  # Head at superjunction j
         min_depth = self.min_depth      # Minimum allowable depth at boundaries
-        _theta_uk = self._theta_uk      # Upstream indicator variable
-        _theta_dk = self._theta_dk      # Downstream indicator variable
         # Compute flow at next time step
-        _h_uk_next = _kappa_uk * _Q_uk + _theta_uk * (_lambda_uk * H_j[_J_uk] + _mu_uk)
-        _h_dk_next = _kappa_dk * _Q_dk + _theta_dk * (_lambda_dk * H_j[_J_dk] + _mu_dk)
+        _h_uk_next = _kappa_uk * _Q_uk + _lambda_uk * H_j[_J_uk] + _mu_uk
+        _h_dk_next = _kappa_dk * _Q_dk + _lambda_dk * H_j[_J_dk] + _mu_dk
         # Set minimum values
         # TODO: Is this causing the difference between normal/numba versions?
         # _h_uk_next[_h_uk_next < min_depth] = min_depth
         # _h_dk_next[_h_dk_next < min_depth] = min_depth
         # Export instance variables
         self._h_uk = _h_uk_next
         self._h_dk = _h_dk_next
@@ -3520,44 +3642,47 @@
         """
         Reposition junctions inside superlinks to enable capture of backwater effects.
         """
         # Import instance variables
         _b0 = self._b0                # Vertical coordinate of upstream end of superlink k
         _b1 = self._b1                # Vertical coordinate of downstream end of superlink k
         _m = self._m                  # Slope of superlink k
-        _x0 = self._x0                # Horizontal coordinate of center of superlink k
-        _z0 = self._z0                # Invert elevation of center of superlink k
+        _xc = self._xc                # Horizontal coordinate of center of superlink k
+        _zc = self._zc                # Invert elevation of center of superlink k
         _fixed = self._fixed          # Junction Ik is fixed (y/n)
         _h_Ik = self._h_Ik            # Depth at junction Ik
         _Q_ik = self._Q_ik            # Flow rate at link ik
         _J_dk = self._J_dk            # Index of superjunction downstream of superlink k
         _x_Ik = self._x_Ik            # Horizontal coordinate of junction Ik
         _dx_ik = self._dx_ik          # Length of link ik
         _z_inv_Ik = self._z_inv_Ik    # Invert elevation of junction Ik
         _S_o_ik = self._S_o_ik        # Channel bottom slope of link ik
         _I_1k = self._I_1k            # Index of first junction in superlink k
         _I_Np1k = self._I_Np1k        # Index of last junction in superlink k
         _i_1k = self._i_1k            # Index of first link in superlink k
         H_j = self.H_j                # Head at superjunction j
         _k = self._k                  # List of superlinks
+        # Check if possible to move elements
+        if not self.mobile_elements:
+            raise ValueError('Model must be instantiated with `mobile_elements=True` to reposition junctions.')
         # Configure function variables
         njunctions_fixed = 4
         njunctions = njunctions_fixed + 1
         nlinks = njunctions - 1
         xx = _x_Ik.reshape(-1, njunctions)
         zz = _z_inv_Ik.reshape(-1, njunctions)
         dxdx = _dx_ik.reshape(-1, nlinks)
         hh = _h_Ik.reshape(-1, njunctions)
         QQ = _Q_ik.reshape(-1, nlinks)
         _H_dk = H_j[_J_dk]
         Q_ix = np.tile(np.arange(nlinks), len(QQ)).reshape(-1, nlinks)
         # TODO: Add case where position of movable coord is exactly equal to fixed coord
         move_junction = (_H_dk > _z_inv_Ik[_I_Np1k]) & (_H_dk < _z_inv_Ik[_I_1k])
-        z_m = np.where(move_junction, _H_dk, _z0)
-        x_m = np.where(move_junction, (_H_dk - _b0) / _m, _x0)
+        z_m = np.where(move_junction, _H_dk, _zc)
+        x_m = np.where(move_junction, (_H_dk - _b0) / _m, _xc)
         # TODO: Use instance variable
         r = np.arange(len(xx))
         c = np.array(list(map(np.searchsorted, xx, x_m)))
         frac = (x_m - xx[r, c - 1]) / (xx[r, c] - xx[r, c - 1])
         h_m = (1 - frac) * hh[r, c - 1] + (frac) * hh[r, c]
         pos_prev = np.where(~_fixed)[1]
         xx[:, :-1] = xx[_fixed].reshape(-1, njunctions - 1)
@@ -3784,41 +3909,51 @@
         self.states['h_Ik'] = np.copy(self.h_Ik)
         self.states['Q_ik'] = np.copy(self.Q_ik)
         self.states['Q_uk'] = np.copy(self.Q_uk)
         self.states['Q_dk'] = np.copy(self.Q_dk)
         self.states['x_Ik'] = np.copy(self.x_Ik)
         if self.n_o:
             self.states['Q_o'] = np.copy(self.Q_o)
+            # TODO: Need to add orifice area here
         if self.n_w:
             self.states['Q_w'] = np.copy(self.Q_w)
         if self.n_p:
             self.states['Q_p'] = np.copy(self.Q_p)
+        self.states['A_ik'] = np.copy(self.A_ik)
+        self.states['A_uk'] = np.copy(self.A_uk)
+        self.states['A_dk'] = np.copy(self.A_dk)
+        self.states['A_sj'] = np.copy(self.A_sj)
+        self.states['V_j'] = np.copy(self.V_j)
 
-    def load_state(self, states={}):
+    def load_state(self, states={}, exclude_states=set(),
+                   compute_hydraulic_geometries=True):
         """
         Load model state.
 
         Inputs:
         -------
         states : dict
             Dict of model states. If empty, load current state stored in self.states dict.
         """
         # If no states given, load previous states
         if not states:
             states = self.states
         for key, value in states.items():
-            setattr(self, key, value)
+            if not key in exclude_states:
+                loaded_state = copy.copy(value)
+                setattr(self, key, loaded_state)
         # Ensure consistency of internal states
-        self.link_hydraulic_geometry()
-        self.upstream_hydraulic_geometry()
-        self.downstream_hydraulic_geometry()
-        self.compute_storage_areas()
-        self.node_velocities()
+        if compute_hydraulic_geometries:
+            self.link_hydraulic_geometry()
+            self.upstream_hydraulic_geometry()
+            self.downstream_hydraulic_geometry()
+            self.compute_storage_areas()
+            self.node_velocities()
 
-    def spinup(self, n_steps=100, dt=10, Q_in=None, Q_0Ik=None, reposition_junctions=True,
+    def spinup(self, n_steps=100, dt=10, Q_in=None, Q_0Ik=None, reposition_junctions=False,
                reset_counters=True, **kwargs):
         """
         Spin up solver for a given number of steps to avoid running a completely dry model.
         """
         if Q_in is None:
             Q_in = 1e-6 * np.ones(self.M)
         if Q_0Ik is None:
@@ -3880,31 +4015,33 @@
             self.save_state()
         if dt is None:
             dt = self._dt
         self._Q_in = Q_in
         self._Q_0Ik = Q_0Ik
         if not implicit:
             raise NotImplementedError
+        # Compute all hydraulic geometries
         self.link_hydraulic_geometry()
         self.upstream_hydraulic_geometry()
         self.downstream_hydraulic_geometry()
         self.compute_storage_areas()
         self.compute_storage_volumes()
         self.node_velocities()
+        if self.orifices is not None:
+            self.orifice_hydraulic_geometry(u=u_o)
         if self.inertial_damping:
             self.compute_flow_regime()
         self.link_coeffs(_dt=dt, first_iter=first_iter)
         self.node_coeffs(_Q_0Ik=Q_0Ik, _dt=dt, first_iter=first_iter)
         self.forward_recurrence()
         self.backward_recurrence()
-        self.superlink_upstream_head_coefficients()
-        self.superlink_downstream_head_coefficients()
+        self.superlink_upstream_head_coefficients(_dt=dt)
+        self.superlink_downstream_head_coefficients(_dt=dt)
         self.superlink_flow_coefficients()
         if self.orifices is not None:
-            self.orifice_hydraulic_geometry(u=u_o)
             self.orifice_flow_coefficients(u=u_o)
         if self.weirs is not None:
             self.weir_flow_coefficients(u=u_w)
         if self.pumps is not None:
             self.pump_flow_coefficients(u=u_p)
         self.sparse_matrix_equations(H_bc=H_bc, _Q_0j=Q_in,
                                      first_time=first_time, _dt=dt,
@@ -3939,15 +4076,15 @@
             self.solve_internals_nnls()
         elif _method == 'lsq':
             self.solve_internals_lsq()
         self.iter_count += 1
         self.t += dt
 
     def step(self, H_bc=None, Q_in=None, Q_0Ik=None, u_o=None, u_w=None, u_p=None, dt=None,
-             first_time=False, implicit=True, banded=False, first_iter=True,
+             first_time=False, implicit=True, banded=None, first_iter=True,
              num_iter=1, head_tol=0.0015):
         """
         Advance model forward to next time step, computing hydraulic states.
 
         Inputs:
         -------
         H_bc : np.ndarray (M)
@@ -3963,64 +4100,48 @@
         u_p : np.ndarray (p)
             Pump control signal. Represents fraction of maximum pump flow (0-1).
         dt : float
             Time step to advance (s)
         first_time : bool
             Set True if this is the first step the model has performed.
         banded : bool
-            If True, use banded matrix solver.
+            If True, use banded matrix solver. Set to value of `self.banded` by default.
         first_iter : bool
             True if this is the first iteration when iterating towards convergence.
         num_iter : int
             Number of iterations to perform when iterating towards convergence.
         head_tol : float
             Maximum allowable head tolerance when iterating towards convergence (m).
         implicit : bool
             (Deprecated)
         """
+        if banded is None:
+            banded = self.banded
         self._setup_step(H_bc=H_bc, Q_in=Q_in, Q_0Ik=Q_0Ik, u_o=u_o, u_w=u_w, u_p=u_p, dt=dt,
                          first_time=first_time, implicit=implicit, banded=banded,
                          first_iter=first_iter)
         self._solve_step(H_bc=H_bc, Q_in=Q_in, Q_0Ik=Q_0Ik, u_o=u_o, u_w=u_w, u_p=u_p, dt=dt,
                          first_time=first_time, implicit=implicit, banded=banded,
                          first_iter=first_iter)
         # Perform fixed-point iteration until convergence
         num_iter -= 1
+        iter_elapsed = 1
         if (num_iter > 0):
             H_j_prev = self.states['H_j']
             H_j_next = np.copy(self.H_j)
-            h_Ik_prev = self.states['h_Ik']
-            Q_ik_prev = self.states['Q_ik']
-            Q_uk_prev = self.states['Q_uk']
-            Q_dk_prev = self.states['Q_dk']
-            if self.n_o:
-                Q_o_prev = self.states['Q_o']
-            if self.n_w:
-                Q_w_prev = self.states['Q_w']
-            if self.n_p:
-                Q_p_prev = self.states['Q_p']
             residual = np.abs(H_j_next - H_j_prev)
             if not (residual < head_tol).all():
                 for _ in range(num_iter):
                     self.iter_count -= 1
                     self.t -= dt
-                    self.H_j = H_j_prev
-                    self._h_Ik = (h_Ik_prev + self._h_Ik) / 2
-                    self._Q_ik = (Q_ik_prev + self._Q_ik) / 2
-                    self._Q_uk = (Q_uk_prev + self._Q_uk) / 2
-                    self._Q_dk = (Q_dk_prev + self._Q_dk) / 2
-                    if self.n_o:
-                        self._Qo = (Q_o_prev + self._Qo) / 2
-                    if self.n_w:
-                        self._Qw = (Q_w_prev + self._Qw) / 2
-                    if self.n_p:
-                        self._Qp = (Q_p_prev + self._Qp) / 2
-                    self._setup_step(H_bc=H_bc, Q_in=Q_in, u_o=u_o, u_w=u_w, u_p=u_p, dt=dt,
+                    self._setup_step(H_bc=H_bc, Q_in=Q_in, Q_0Ik=Q_0Ik, u_o=u_o, u_w=u_w, u_p=u_p, dt=dt,
                                      first_time=first_time, implicit=implicit, banded=banded,
                                      first_iter=False)
-                    self._solve_step(H_bc=H_bc, Q_in=Q_in, u_o=u_o, u_w=u_w, u_p=u_p, dt=dt,
+                    self._solve_step(H_bc=H_bc, Q_in=Q_in, Q_0Ik=Q_0Ik, u_o=u_o, u_w=u_w, u_p=u_p, dt=dt,
                                      first_time=first_time, implicit=implicit, banded=banded,
                                      first_iter=False)
+                    iter_elapsed += 1
                     residual = np.abs(H_j_next - self.H_j)
                     if (residual < head_tol).all():
                         break
                     H_j_next = np.copy(self.H_j)
+        self.iter_elapsed = iter_elapsed
```

### Comparing `pipedream-solver-0.2/pipedream_solver/visualization.py` & `pipedream-solver-0.2.2/pipedream_solver/visualization.py`

 * *Files identical despite different names*

### Comparing `pipedream-solver-0.2/pipedream_solver/ninfiltration.py` & `pipedream-solver-0.2.2/pipedream_solver/ninfiltration.py`

 * *Files identical despite different names*

### Comparing `pipedream-solver-0.2/pipedream_solver/utils.py` & `pipedream-solver-0.2.2/pipedream_solver/utils.py`

 * *Files identical despite different names*

### Comparing `pipedream-solver-0.2/pipedream_solver/geometry.py` & `pipedream-solver-0.2.2/pipedream_solver/geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,16 @@
     'rect_closed' : 2,
     'rect_open' : 3,
     'triangular' : 4,
     'trapezoidal' : 5,
     'parabolic' : 6,
     'elliptical' : 7,
     'wide' : 8,
-    'force_main' : 9
+    'force_main' : 9,
+    'floodplain' : 10
 }
 
 # Machine precision
 eps = np.finfo(float).eps
 
 class Circular():
     def __init__(self):
@@ -871,14 +872,35 @@
             Width of Preissman slot (as a ratio of the diameter)
         """
         d = g1
         pslot = g2
         B = d * pslot
         return B
 
+class Floodplain():
+    def __init__(self):
+        pass
+
+    @classmethod
+    def A_ik(self, h_Ik, h_Ip1k, g1, g2, g3, g4, g5, g6, g7, **kwargs):
+        raise NotImplementedError
+
+    @classmethod
+    def Pe_ik(self, h_Ik, h_Ip1k, g1, g2, g3, g4, g5, g6, g7, **kwargs):
+        raise NotImplementedError
+
+    @classmethod
+    def R_ik(self, A_ik, Pe_ik):
+        raise NotImplementedError
+
+    @classmethod
+    def B_ik(self, h_Ik, h_Ip1k, g1, g2, g3, g4, g5, g6, g7, **kwargs):
+        raise NotImplementedError
+
+
 class Irregular():
     def __init__(self, x, y, horiz_points=100, vert_points=100):
         self.x = np.asarray(x)
         self.y = np.asarray(y)
         self.horiz_points = horiz_points
         self.ymin = self.y.min()
         self.ymax = self.y.max()
```

### Comparing `pipedream-solver-0.2/pipedream_solver/storage.py` & `pipedream-solver-0.2.2/pipedream_solver/storage.py`

 * *Files identical despite different names*

### Comparing `pipedream-solver-0.2/pipedream_solver/nquality.py` & `pipedream-solver-0.2.2/pipedream_solver/nquality.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import pandas as pd
 from numba import njit
 import scipy.linalg
 import scipy.sparse
 import scipy.sparse.linalg
-
+#test
 class QualityBuilder():
     """
     An implicit, staggered-grid water quality solver based on the 1D
     advection-reaction-diffusion equations.
 
     Inputs:
     -----------
@@ -95,41 +95,41 @@
     c_dk     : Contaminant concentration exiting downstream end of superlinks (*/m^3)
     """
     def __init__(self, hydraulics, superjunction_params, superlink_params,
                  junction_params=None, link_params=None, c_min=0.0, c_max=np.inf):
         self.hydraulics = hydraulics
         self._ki = self.hydraulics._ki
         self._kI = self.hydraulics._kI
-        self._K_j = superjunction_params['K'].values.astype(float)
-        self._c_j = superjunction_params['c_0'].values.astype(float)
-        self.bc = superjunction_params['bc'].values.astype(bool)
+        self._K_j = superjunction_params['K'].values.astype(np.float64)
+        self._c_j = superjunction_params['c_0'].values.astype(np.float64)
+        self.bc = superjunction_params['bc'].values.astype(np.bool8)
         if junction_params is not None:
-            self._K_Ik = junction_params['K'].values.astype(float)
-            self._c_Ik = junction_params['c_0'].values.astype(float)
+            self._K_Ik = junction_params['K'].values.astype(np.float64)
+            self._c_Ik = junction_params['c_0'].values.astype(np.float64)
         else:
-            self._K_Ik = superlink_params['K'].values[self._kI].astype(float)
-            self._c_Ik = superlink_params['c_0'].values[self._kI].astype(float)
+            self._K_Ik = superlink_params['K'].values[self._kI].astype(np.float64)
+            self._c_Ik = superlink_params['c_0'].values[self._kI].astype(np.float64)
         if link_params is not None:
-            self._D_ik = link_params['D'].values.astype(float)
-            self._K_ik = link_params['K'].values.astype(float)
-            self._c_ik = link_params['c_0'].values.astype(float)
+            self._D_ik = link_params['D'].values.astype(np.float64)
+            self._K_ik = link_params['K'].values.astype(np.float64)
+            self._c_ik = link_params['c_0'].values.astype(np.float64)
         else:
-            self._D_ik = superlink_params['D'].values[self._ki].astype(float)
-            self._K_ik = superlink_params['K'].values[self._ki].astype(float)
-            self._c_ik = superlink_params['c_0'].values[self._ki].astype(float)
-        self._dx_uk = superlink_params['dx_uk'].values.astype(float)
-        self._dx_dk = superlink_params['dx_dk'].values.astype(float)
+            self._D_ik = superlink_params['D'].values[self._ki].astype(np.float64)
+            self._K_ik = superlink_params['K'].values[self._ki].astype(np.float64)
+            self._c_ik = superlink_params['c_0'].values[self._ki].astype(np.float64)
+        self._dx_uk = superlink_params['dx_uk'].values.astype(np.float64)
+        self._dx_dk = superlink_params['dx_dk'].values.astype(np.float64)
         if 'D_uk' in superlink_params.columns:
-            self._D_uk = superlink_params['D_uk'].values.astype(float)
+            self._D_uk = superlink_params['D_uk'].values.astype(np.float64)
         else:
-            self._D_uk = superlink_params['D'].values.astype(float)
+            self._D_uk = superlink_params['D'].values.astype(np.float64)
         if 'D_dk' in superlink_params.columns:
-            self._D_dk = superlink_params['D_dk'].values.astype(float)
+            self._D_dk = superlink_params['D_dk'].values.astype(np.float64)
         else:
-            self._D_dk = superlink_params['D'].values.astype(float)
+            self._D_dk = superlink_params['D'].values.astype(np.float64)
         # Structural parameters of hydraulic model
         self._forward_I_i = self.hydraulics.forward_I_i       # Index of link after junction Ik
         self._backward_I_i = self.hydraulics.backward_I_i     # Index of link before junction Ik
         self._is_start = self.hydraulics._is_start
         self._is_end = self.hydraulics._is_end
         self._ik = self.hydraulics._ik
         self._I = self.hydraulics._I
@@ -179,42 +179,40 @@
         self._Y_uk = np.zeros(self.NK)
         self._Z_uk = np.zeros(self.NK)
         self._U_dk = np.zeros(self.NK)
         self._V_dk = np.zeros(self.NK)
         self._W_dk = np.zeros(self.NK)
         self._rho_uk = np.zeros(self.NK)
         self._tau_uk = np.zeros(self.NK)
-        self._omega_uk = np.zeros(self.NK)
+        self._zeta_uk = np.zeros(self.NK)
         self._rho_dk = np.zeros(self.NK)
         self._tau_dk = np.zeros(self.NK)
-        self._omega_dk = np.zeros(self.NK)
-        self._F_jj = np.zeros(self.M, dtype=float)
-        self._O_diag = np.zeros(self.M, dtype=float)
-        self._W_diag = np.zeros(self.M, dtype=float)
-        self._P_diag = np.zeros(self.M, dtype=float)
+        self._zeta_dk = np.zeros(self.NK)
+        self._F_jj = np.zeros(self.M, dtype=np.float64)
+        self._O_diag = np.zeros(self.M, dtype=np.float64)
+        self._W_diag = np.zeros(self.M, dtype=np.float64)
+        self._P_diag = np.zeros(self.M, dtype=np.float64)
         self.A = np.zeros((self.M, self.M))
         self.O = np.zeros((self.M, self.M))
         self.W = np.zeros((self.M, self.M))
         self.P = np.zeros((self.M, self.M))
         self.D = np.zeros(self.M)
         self.b = np.zeros(self.M)
         self._c_uk = 0.5 * self._c_j[self._J_uk] + 0.5 * self._c_Ik[self._I_1k]
         self._c_dk = 0.5 * self._c_j[self._J_dk] + 0.5 * self._c_Ik[self._I_Np1k]
         self._c_1k = self._c_Ik[self._I_1k]
         self._c_Np1k = self._c_Ik[self._I_Np1k]
         self._c_min = c_min
         self._c_max = c_max
         self._Ik = self.hydraulics._Ik
         self._Ip1k = self.hydraulics._Ip1k
-        self._Q_Ik_next = np.zeros(self._Ik.size, dtype=float)
-        self._Q_Ip1k_next = np.zeros(self._Ip1k.size, dtype=float)
-        self._D_Ik = np.zeros(self._Ik.size, dtype=float)
-        self._D_Ip1k = np.zeros(self._Ip1k.size, dtype=float)
-        self._A_Ik_next = np.zeros(self._Ik.size, dtype=float)
-        self._A_Ip1k_next = np.zeros(self._Ip1k.size, dtype=float)
+        self._Q_Ik_next = np.zeros(self._Ik.size, dtype=np.float64)
+        self._Q_Ip1k_next = np.zeros(self._Ip1k.size, dtype=np.float64)
+        self._D_Ik = np.zeros(self._I.size, dtype=np.float64)
+        self._A_Ik_next = np.zeros(self._I.size, dtype=np.float64)
         self.step(dt=1e-6)
 
     # TODO: It might be safer to have these as @properties
     def import_hydraulic_states(self):
         self._H_j_next = self.hydraulics.H_j
         self._h_Ik_next = self.hydraulics.h_Ik
         self._Q_ik_next = self.hydraulics.Q_ik
@@ -230,24 +228,25 @@
             self._Q_o_prev = self.hydraulics.states['Q_o']
         if self.n_w:
             self._Q_w_next = self.hydraulics.Q_w
             self._Q_w_prev = self.hydraulics.states['Q_w']
         if self.n_p:
             self._Q_p_next = self.hydraulics.Q_p
             self._Q_p_prev = self.hydraulics.states['Q_p']
-        self._u_ik_next = self.hydraulics._u_ik
-        self._u_Ik_next = self.hydraulics._u_Ik
-        self._u_Ip1k_next = self.hydraulics._u_Ip1k
         self._dx_ik_next = self.hydraulics._dx_ik
         self._A_ik_next = self.hydraulics._A_ik
-        self._B_ik_next = self.hydraulics._B_ik
         self._A_uk_next = self.hydraulics._A_uk
         self._A_dk_next = self.hydraulics._A_dk
+        # TODO: Added additional states to superlink
+        self._A_ik_prev = self.hydraulics.states['A_ik']
+        self._A_uk_prev = self.hydraulics.states['A_uk']
+        self._A_dk_prev = self.hydraulics.states['A_dk']
         self._A_sj = self.hydraulics._A_sj
-        self._V_sj = self.hydraulics._V_sj
+        self._V_j_next = self.hydraulics.V_j
+        self._V_j_prev = self.hydraulics.states['V_j']
 
     @property
     def c_j(self):
         return self._c_j
 
     @c_j.setter
     def c_j(self, value):
@@ -296,38 +295,45 @@
         # Import instance variables
         _Ip1k = self._Ip1k                   # Next junction index
         _A_ik_next = self._A_ik_next                   # Flow area at link ik
         _Q_ik_next = self._Q_ik_next                   # Flow rate at link ik
         _Q_Ik_next = self._Q_Ik_next                   # Flow velocity at junction Ik
         _Q_Ip1k_next = self._Q_Ip1k_next               # Flow velocity at junction I + 1k
         _A_Ik_next = self._A_Ik_next                   # Flow velocity at junction Ik
-        _A_Ip1k_next = self._A_Ip1k_next               # Flow velocity at junction I + 1k
         _D_ik = self._D_ik
         _D_Ik = self._D_Ik                   # Flow velocity at junction Ik
-        _D_Ip1k = self._D_Ip1k               # Flow velocity at junction I + 1k
         _dx_ik_next = self._dx_ik_next                 # Length of link ik
         _link_start = self.hydraulics._link_start
         _link_end = self.hydraulics._link_end
         # Determine start and end nodes
         # Compute velocities for start nodes (1 -> Nk)
-        numba_Q_Ik(_dx_ik_next, _Q_ik_next, _link_start, _Q_Ik_next)
-        numba_Q_Ip1k(_dx_ik_next, _Q_ik_next, _link_end, _Q_Ip1k_next)
-        numba_Q_Ik(_dx_ik_next, _A_ik_next, _link_start, _A_Ik_next)
-        numba_Q_Ip1k(_dx_ik_next, _A_ik_next, _link_end, _A_Ip1k_next)
-        numba_Q_Ik(_dx_ik_next, _D_ik, _link_start, _D_Ik)
-        numba_Q_Ip1k(_dx_ik_next, _D_ik, _link_end, _D_Ip1k)
+        # TODO: These are not needed for Min-Gyu's method
+        # numba_Q_Ik(_dx_ik_next, _Q_ik_next, _link_start, _Q_Ik_next)
+        # numba_Q_Ip1k(_dx_ik_next, _Q_ik_next, _link_end, _Q_Ip1k_next)
+        # numba_Q_Ik(_dx_ik_next, _A_ik_next, _link_start, _A_Ik_next)
+        # numba_Q_Ip1k(_dx_ik_next, _A_ik_next, _link_end, _A_Ip1k_next)
+        # numba_Q_Ik(_dx_ik_next, _D_ik, _link_start, _D_Ik)
+        # numba_Q_Ip1k(_dx_ik_next, _D_ik, _link_end, _D_Ip1k)
         # Export to instance variables
-        self._Q_Ik_next = _Q_Ik_next
-        self._Q_Ip1k_next = _Q_Ip1k_next
-        self._A_Ik_next = _A_Ik_next
-        self._A_Ip1k_next = _A_Ip1k_next
-        self._D_Ik = _D_Ik
-        self._D_Ip1k = _D_Ip1k
+        # TODO: Min-Gyu's method
+        self._Q_Ik_next = _Q_ik_next
+        self._Q_Ip1k_next = _Q_ik_next
+        self._A_Ik_next[self._Ik] = _A_ik_next
+        self._A_Ik_next[self._Ip1k] = _A_ik_next
+        self._D_Ik[self._Ik] = _D_ik
+        self._D_Ik[self._Ip1k] = _D_ik
+        # TODO: These are probably more technically correct
+        # self._Q_Ik_next = _Q_Ik_next
+        # self._Q_Ip1k_next = _Q_Ip1k_next
+        # self._A_Ik_next = _A_Ik_next
+        # self._A_Ip1k_next = _A_Ip1k_next
+        # self._D_Ik = _D_Ik
+        # self._D_Ip1k = _D_Ip1k
 
-    def link_coeffs(self, _dt=None, _u_j_frac=0.0, first_iter=True):
+    def link_coeffs(self, _dt=None, first_iter=True):
         """
         Compute link momentum coefficients: a_ik, b_ik, c_ik and P_ik.
         """
         # Import instance variables
         _Q_Ik_next = self._Q_Ik_next         # Flow velocity at junction Ik
         _Q_Ip1k_next = self._Q_Ip1k_next     # Flow velocity at junction I + 1k
         _dx_ik_next = self._dx_ik_next       # Length of link ik
@@ -336,14 +342,17 @@
         _c_ik = self._c_ik
         _Q_uk_next = self._Q_uk_next
         _A_uk_next = self._A_uk_next
         _Q_dk_next = self._Q_dk_next
         _A_dk_next = self._A_dk_next
         _Q_ik_next = self._Q_ik_next
         _A_ik_next = self._A_ik_next
+        _A_ik_prev = self._A_ik_prev
+        _A_uk_prev = self._A_uk_prev
+        _A_dk_prev = self._A_dk_prev
         _D_uk = self._D_uk
         _D_dk = self._D_dk
         _dx_uk = self._dx_uk
         _dx_dk = self._dx_dk
         _i_1k = self._i_1k
         _i_nk = self._i_nk
         _I_1k = self._I_1k
@@ -354,42 +363,47 @@
         _beta_ik = self._beta_ik
         _chi_ik = self._chi_ik
         _gamma_ik = self._gamma_ik
         # If time step not specified, use instance time
         if _dt is None:
             _dt = self._dt
         # Compute link coefficients
-        # TODO: This should happen in hydraulic solver
-        _Q_1k = (_Q_uk_next + _Q_ik_next[_i_1k]) / 2
-        _Q_Np1k = (_Q_dk_next + _Q_ik_next[_i_nk]) / 2
+        # TODO: Min-Gyu's method
+        _Q_1k = _Q_uk_next
+        _Q_Np1k = _Q_dk_next
+        # _Q_1k = _Q_ik_next[_i_1k]
+        # _Q_Np1k = _Q_ik_next[_i_nk]
+        # _Q_1k = (_Q_uk_next + _Q_ik_next[_i_1k]) / 2
+        # _Q_Np1k = (_Q_dk_next + _Q_ik_next[_i_nk]) / 2
         # TODO: Is this even necessary?
         # TODO: Redundant computations
-        _Q_Ik_next[np.cumsum(self.nk) - self.nk[0]] = _Q_1k
-        _Q_Ip1k_next[np.cumsum(self.nk) - 1] = _Q_Np1k
-        _omega_Ik = (_Q_Ik_next > 0).astype(float)
-        _omega_Ip1k = (_Q_Ip1k_next > 0).astype(float)
-        _omega_1k = (_Q_1k > 0.).astype(float)
-        _omega_Np1k = (_Q_Np1k > 0.).astype(float)
-        _omega_uk = (_Q_uk_next > 0.).astype(float)
-        _omega_dk = (_Q_dk_next > 0.).astype(float)
+        # _Q_Ik_next[np.cumsum(self.nk) - self.nk[0]] = _Q_1k
+        # _Q_Ip1k_next[np.cumsum(self.nk) - 1] = _Q_Np1k
+        _omega_Ik = (_Q_Ik_next > 0).astype(np.float64)
+        _omega_Ip1k = (_Q_Ip1k_next > 0).astype(np.float64)
+        _omega_1k = (_Q_1k > 0.).astype(np.float64)
+        _omega_Np1k = (_Q_Np1k > 0.).astype(np.float64)
+        _omega_uk = (_Q_uk_next > 0.).astype(np.float64)
+        _omega_dk = (_Q_dk_next > 0.).astype(np.float64)
         _alpha_ik = alpha_ik(_Q_Ik_next, _omega_Ik, _dx_ik_next, _D_ik, _A_ik_next)
-        _beta_ik = beta_ik(_dt, _D_ik, _A_ik_next, _dx_ik_next, _K_ik, _Q_Ik_next, _Q_Ip1k_next,
-                           _omega_Ik, _omega_Ip1k)
+        _beta_ik = beta_ik(_dt, _D_ik, _A_ik_next, _A_ik_prev, _dx_ik_next, _K_ik,
+                           _Q_Ik_next, _Q_Ip1k_next, _omega_Ik, _omega_Ip1k)
         _chi_ik = chi_ik(_Q_Ip1k_next, _omega_Ip1k, _dx_ik_next, _D_ik, _A_ik_next)
         _gamma_ik = gamma_ik(_dt, _c_ik, _A_ik_next, _dx_ik_next)
-        # Compute link coefficients for boundaries
-        _alpha_uk = alpha_ik(_u_j_frac * _Q_uk_next, _omega_uk, _dx_uk, _D_uk, _A_uk_next)
-        _beta_uk = beta_ik(_dt, _D_uk, _A_uk_next, _dx_uk, 0.0, _u_j_frac * _Q_uk_next, _Q_1k,
+        # Compute link coefficients for upstream boundary
+        _alpha_uk = alpha_ik(_Q_uk_next, _omega_uk, _dx_uk, _D_uk, _A_uk_next)
+        _beta_uk = beta_ik(_dt, _D_uk, _A_uk_next, _A_uk_prev, _dx_uk, 0.0, _Q_uk_next, _Q_1k,
                            _omega_uk, _omega_1k)
         _chi_uk = chi_ik(_Q_1k, _omega_1k, _dx_uk, _D_uk, _A_uk_next)
         _gamma_uk = gamma_ik(_dt, _c_uk, _A_uk_next, _dx_uk)
+        # Compute link coefficients for downstream boundary
         _alpha_dk = alpha_ik(_Q_Np1k, _omega_Np1k, _dx_dk, _D_dk, _A_dk_next)
-        _beta_dk = beta_ik(_dt, _D_dk, _A_dk_next, _dx_dk, 0.0, _Q_Np1k, _u_j_frac * _Q_dk_next,
+        _beta_dk = beta_ik(_dt, _D_dk, _A_dk_next, _A_dk_prev, _dx_dk, 0.0, _Q_Np1k, _Q_dk_next,
                            _omega_Np1k, _omega_dk)
-        _chi_dk = chi_ik(_u_j_frac * _Q_dk_next, _omega_dk, _dx_dk, _D_dk, _A_dk_next)
+        _chi_dk = chi_ik(_Q_dk_next, _omega_dk, _dx_dk, _D_dk, _A_dk_next)
         _gamma_dk = gamma_ik(_dt, _c_dk, _A_dk_next, _dx_dk)
         # Export to instance variables
         self._alpha_ik = _alpha_ik
         self._beta_ik = _beta_ik
         self._chi_ik = _chi_ik
         self._gamma_ik = _gamma_ik
         self._alpha_uk = _alpha_uk
@@ -420,41 +434,45 @@
         _c_Ik_prev = self._c_Ik
         _K_Ik = self._K_Ik
         _kappa_Ik = self._kappa_Ik
         _lambda_Ik = self._lambda_Ik
         _mu_Ik = self._mu_Ik
         _eta_Ik = self._eta_Ik
         _c_ik_prev = self._c_ik
-        _B_ik_next = self._B_ik_next
         _A_ik_next = self._A_ik_next
         _K_ik = self._K_ik
         _dx_ik_next = self._dx_ik_next
         _D_Ik = self._D_Ik
         _A_Ik_next = self._A_Ik_next
         _dx_uk = self._dx_uk
         _dx_dk = self._dx_dk
+        _A_uk_next = self._A_uk_next
+        _A_dk_next = self._A_dk_next
+        _D_uk = self._D_uk
+        _D_dk = self._D_dk
+        _D_ik = self._D_ik
         # If no time step specified, use instance time step
         if _dt is None:
             _dt = self._dt
         # If no nodal input specified, use zero input
         if _Q_0Ik is None:
             _Q_0Ik = np.zeros(_h_Ik_next.size)
         if _c_0Ik is None:
             _c_0Ik = np.zeros(_h_Ik_next.size)
         # Compute continuity coefficients
-        _omega_ik = (_Q_ik_next > 0.).astype(float)
-        _omega_uk = (_Q_uk_next > 0.).astype(float)
-        _omega_dk = (_Q_dk_next > 0.).astype(float)
+        _omega_ik = (_Q_ik_next > 0.).astype(np.float64)
+        _omega_uk = (_Q_uk_next > 0.).astype(np.float64)
+        _omega_dk = (_Q_dk_next > 0.).astype(np.float64)
         numba_node_coeffs(_kappa_Ik, _lambda_Ik, _mu_Ik, _eta_Ik, _Q_ik_next,
                           _h_Ik_next, _h_Ik_prev, _c_Ik_prev, _c_ik_prev,
                           _Q_uk_next, _Q_dk_next, _c_0Ik, _Q_0Ik, _A_SIk,
-                          _K_Ik, _K_ik, _B_ik_next, _A_ik_next, _dx_ik_next,
+                          _K_Ik, _K_ik, _A_ik_next, _dx_ik_next,
                           _forward_I_i, _backward_I_i, _is_start, _is_end, _kI,
-                          _dt, _omega_ik, _omega_uk, _omega_dk, _D_Ik, _A_Ik_next,
-                          _dx_uk, _dx_dk)
+                          _dt, _omega_ik, _omega_uk, _omega_dk, _D_Ik, _D_ik, _A_Ik_next,
+                          _dx_uk, _dx_dk, _D_uk, _D_dk, _A_uk_next, _A_dk_next)
         # Export instance variables
         self._kappa_Ik = _kappa_Ik
         self._lambda_Ik = _lambda_Ik
         self._mu_Ik = _mu_Ik
         self._eta_Ik = _eta_Ik
 
     def forward_recurrence(self):
@@ -546,18 +564,18 @@
         _gamma_uk = self._gamma_uk
         _alpha_dk = self._alpha_dk
         _beta_dk = self._beta_dk
         _chi_dk = self._chi_dk
         _gamma_dk = self._gamma_dk
         _rho_uk = self._rho_uk
         _tau_uk = self._tau_uk
-        _omega_uk = self._omega_uk
+        _zeta_uk = self._zeta_uk
         _rho_dk = self._rho_dk
         _tau_dk = self._tau_dk
-        _omega_dk = self._omega_dk
+        _zeta_dk = self._zeta_dk
         # Compute boundary coefficients
         numba_boundary_coefficients(_X_uk, _Y_uk, _Z_uk, _U_dk, _V_dk, _W_dk,
                                     _X_Ik, _Y_Ik, _Z_Ik, _U_Ik, _V_Ik, _W_Ik,
                                     _kappa_Ik, _lambda_Ik, _mu_Ik, _eta_Ik,
                                     NK, _I_1k, _I_Nk)
         # Compute boundary advection/diffusion coefficients
         _theta_uk = theta_uk(_beta_uk, _chi_uk)
@@ -566,19 +584,19 @@
         _theta_dk = theta_dk(_beta_dk, _alpha_dk)
         _sigma_dk = sigma_dk(_chi_dk, _alpha_dk)
         _xi_dk = xi_dk(_gamma_dk, _alpha_dk)
         # Compute boundary transport coefficients
         _D_k_star = D_k_star(_X_uk, _U_dk, _W_dk, _Z_uk, _theta_uk, _theta_dk)
         _rho_uk = rho_uk(_U_dk, _X_uk, _Z_uk, _W_dk, _theta_dk, _sigma_uk, _D_k_star)
         _tau_uk = tau_uk(_Z_uk, _sigma_dk, _D_k_star)
-        _omega_uk = omega_uk(_Z_uk, _V_dk, _U_dk, _Y_uk, _X_uk, _W_dk,
+        _zeta_uk = zeta_uk(_Z_uk, _V_dk, _U_dk, _Y_uk, _X_uk, _W_dk,
                              _theta_dk, _xi_uk, _xi_dk, _D_k_star)
         _rho_dk = rho_dk(_W_dk, _sigma_uk, _D_k_star)
         _tau_dk = tau_dk(_X_uk, _U_dk, _W_dk, _Z_uk, _theta_uk, _sigma_dk, _D_k_star)
-        _omega_dk = omega_dk(_W_dk, _Y_uk, _X_uk, _V_dk, _Z_uk, _U_dk,
+        _zeta_dk = zeta_dk(_W_dk, _Y_uk, _X_uk, _V_dk, _Z_uk, _U_dk,
                              _theta_uk, _xi_uk, _xi_dk, _D_k_star)
         # Export instance variables
         self._X_uk = _X_uk
         self._Y_uk = _Y_uk
         self._Z_uk = _Z_uk
         self._U_dk = _U_dk
         self._V_dk = _V_dk
@@ -587,37 +605,44 @@
         self._sigma_uk = _sigma_uk
         self._xi_uk = _xi_uk
         self._theta_dk = _theta_dk
         self._sigma_dk = _sigma_dk
         self._xi_dk = _xi_dk
         self._rho_uk = _rho_uk
         self._tau_uk = _tau_uk
-        self._omega_uk = _omega_uk
+        self._zeta_uk = _zeta_uk
         self._rho_dk = _rho_dk
         self._tau_dk = _tau_dk
-        self._omega_dk = _omega_dk
+        self._zeta_dk = _zeta_dk
 
     def sparse_matrix_equations(self, c_bc=None, _Q_0j=None, _c_0j=None, u=None, _dt=None,
                                 implicit=True, first_time=False):
         """
         Construct sparse matrices A, O, W, P and b.
         """
         # Import instance variables
         _k = self._k                     # Superlink indices
         _J_uk = self._J_uk               # Index of superjunction upstream of superlink k
         _J_dk = self._J_dk               # Index of superjunction downstream of superlink k
         _rho_uk = self._rho_uk
         _tau_uk = self._tau_uk
-        _omega_uk = self._omega_uk
+        _zeta_uk = self._zeta_uk
         _rho_dk = self._rho_dk
         _tau_dk = self._tau_dk
-        _omega_dk = self._omega_dk
+        _zeta_dk = self._zeta_dk
         _F_jj = self._F_jj
         _A_sj = self._A_sj               # Surface area of superjunction j
-        _V_sj = self._V_sj
+        _V_j_next = self._V_j_next
+        _V_j_prev = self._V_j_prev
+        _D_uk = self._D_uk
+        _D_dk = self._D_dk
+        _A_uk_next = self._A_uk_next
+        _A_dk_next = self._A_dk_next
+        _dx_uk = self._dx_uk
+        _dx_dk = self._dx_dk
         _c_j = self._c_j
         _Q_uk_next = self._Q_uk_next
         _Q_dk_next = self._Q_dk_next
         _K_j = self._K_j
         NK = self.NK
         n_o = self.n_o                   # Number of orifices in system
         n_w = self.n_w                   # Number of weirs in system
@@ -669,43 +694,47 @@
             u = 0
         # Clear old data
         _F_jj.fill(0)
         D.fill(0)
         numba_clear_off_diagonals(A, bc, _J_uk, _J_dk, NK)
         # Create A matrix
         # TODO: Need to rename other omega_uk and omega_dk
-        _OMEGA_UK = (_Q_uk_next >= 0).astype(float)
-        _OMEGA_DK = (_Q_dk_next >= 0).astype(float)
+        _omega_uk = (_Q_uk_next >= 0).astype(np.float64)
+        _omega_dk = (_Q_dk_next >= 0).astype(np.float64)
         numba_create_A_matrix(A, _F_jj, bc, _J_uk, _J_dk, _rho_uk, _rho_dk, _tau_uk, _tau_dk,
-                              _Q_uk_next, _Q_dk_next, _OMEGA_UK, _OMEGA_DK, _A_sj, _V_sj,
-                              _H_j_next, _dt, _K_j, M, NK)
+                              _Q_uk_next, _Q_dk_next, _omega_uk, _omega_dk, _V_j_next, _V_j_prev,
+                              _H_j_next, _dt, _K_j, _D_uk, _D_dk, _A_uk_next, _A_dk_next,
+                              _dx_uk, _dx_dk, M, NK)
         # Create D vector
-        numba_add_at(D, _J_uk, -_omega_uk * _Q_uk_next)
-        numba_add_at(D, _J_dk, _omega_dk * _Q_dk_next)
+        numba_add_at(D, _J_uk, (-_Q_uk_next * (1 - _omega_uk)
+                                + 2 * _D_uk * _A_uk_next / _dx_uk) * _zeta_uk)
+        numba_add_at(D, _J_dk, (_Q_dk_next * _omega_dk
+                                + 2 * _D_dk * _A_dk_next / _dx_dk) * _zeta_dk)
         # Compute control matrix
         if n_o:
-            _omega_o = (_Q_o_next >= 0).astype(float)
+            _omega_o = (_Q_o_next >= 0).astype(np.float64)
             _O_diag.fill(0)
             numba_clear_off_diagonals(O, bc, _J_uo, _J_do, n_o)
             numba_create_OWP_matrix(O, _O_diag, bc, _J_uo, _J_do, _omega_o,
                                     _Q_o_next, M, n_o)
         if n_w:
-            _omega_w = (_Q_w_next >= 0).astype(float)
+            _omega_w = (_Q_w_next >= 0).astype(np.float64)
             _W_diag.fill(0)
             numba_clear_off_diagonals(W, bc, _J_uw, _J_dw, n_w)
             numba_create_OWP_matrix(W, _W_diag, bc, _J_uw, _J_dw, _omega_w,
                                     _Q_w_next, M, n_w)
         if n_p:
-            _omega_p = (_Q_p_next >= 0).astype(float)
+            _omega_p = (_Q_p_next >= 0).astype(np.float64)
             _P_diag.fill(0)
             numba_clear_off_diagonals(P, bc, _J_up, _J_dp, n_p)
             numba_create_OWP_matrix(P, _P_diag, bc, _J_up, _J_dp, _omega_p,
                                     _Q_p_next, M, n_p)
         b.fill(0)
-        b = (_A_sj * _H_j_prev * _c_j / _dt) + (_Q_0j * _c_0j) + D
+        # TODO: Change to _c_j_prev
+        b = (_V_j_next * _c_j / _dt) + (_Q_0j * _c_0j) + D
         # Ensure boundary condition is specified
         b[bc] = c_bc[bc]
         # Export instance variables
         self.D = D
         self.b = b
 
     def solve_sparse_matrix(self, u=None, implicit=True):
@@ -792,25 +821,34 @@
         _c_j = self._c_j
         _c_uk = self._c_uk
         _c_dk = self._c_dk
         _J_uk = self._J_uk               # Index of superjunction upstream of superlink k
         _J_dk = self._J_dk               # Index of superjunction downstream of superlink k
         _rho_uk = self._rho_uk
         _tau_uk = self._tau_uk
-        _omega_uk = self._omega_uk
+        _zeta_uk = self._zeta_uk
         _rho_dk = self._rho_dk
         _tau_dk = self._tau_dk
-        _omega_dk = self._omega_dk
+        _zeta_dk = self._zeta_dk
+        _theta_uk = self._theta_uk
+        _theta_dk = self._theta_dk
+        _sigma_uk = self._sigma_uk
+        _sigma_dk = self._sigma_dk
+        _xi_uk = self._xi_uk
+        _xi_dk = self._xi_dk
         _c_min = self._c_min
         _c_max = self._c_max
         # Solve for boundary flow concentrations
-        _c_uk_next = _rho_uk * _c_j[_J_uk] + _tau_uk * _c_j[_J_dk] + _omega_uk
-        _c_dk_next = _rho_dk * _c_j[_J_uk] + _tau_dk * _c_j[_J_dk] + _omega_dk
-        _c_1k = 2 * _c_uk_next - _c_j[_J_uk]
-        _c_Np1k = 2 * _c_dk_next - _c_j[_J_dk]
+        _c_uk_next = _rho_uk * _c_j[_J_uk] + _tau_uk * _c_j[_J_dk] + _zeta_uk
+        _c_dk_next = _rho_dk * _c_j[_J_uk] + _tau_dk * _c_j[_J_dk] + _zeta_dk
+        # TODO: Where did this come from?
+        # _c_1k = 2 * _c_uk_next - _c_j[_J_uk]
+        # _c_Np1k = 2 * _c_dk_next - _c_j[_J_dk]
+        _c_1k = _theta_uk * _c_uk_next + _sigma_uk * _c_j[_J_uk] + _xi_uk
+        _c_Np1k = _theta_dk * _c_dk_next + _sigma_dk * _c_j[_J_dk] + _xi_dk
         # Enforce non-negative concentration
         _c_uk_next = np.maximum(_c_uk_next, _c_min)
         _c_dk_next = np.maximum(_c_dk_next, _c_min)
         _c_1k = np.maximum(_c_1k, _c_min)
         _c_Np1k = np.maximum(_c_Np1k, _c_min)
         _c_uk_next = np.minimum(_c_uk_next, _c_max)
         _c_dk_next = np.minimum(_c_dk_next, _c_max)
@@ -918,15 +956,15 @@
                        np.repeat(_c_Np1k, nk))
         c_ik_f = c_i_f(_U_Ik[~_is_end], _c_Ik[~_is_start],
                        _V_Ik[~_is_end], _W_Ik[~_is_end],
                        np.repeat(_c_1k, nk))
         return c_ik_b, c_ik_f
 
     def step(self, dt=None, c_bc=None, c_0j=None, Q_0j=None, c_0Ik=None,
-             Q_0Ik=None, u_j_frac=0.0):
+             Q_0Ik=None):
         """
         Advance model forward to next time step, computing water quality states.
 
         Inputs:
         -------
         dt : float
             Time step to advance (s)
@@ -940,30 +978,28 @@
             Defaults to `_Q_in` of underlying SuperLink model.
         c_0Ik : np.ndarray (M)
             Contaminant concentration in direction junction inflow `Q_0Ik` (*/m^3).
             Defaults to 0.
         Q_0Ik : np.ndarray (M)
             Direct inflow at each junction (m^3/s).
             Defaults to `_Q_0Ik` of underlying SuperLink model.
-        u_j_frac : float
-            (Deprecated).
 
         Returns:
         --------
         None
         """
         self.import_hydraulic_states()
         if dt is None:
             dt = self._dt
         if Q_0j is None:
             Q_0j = self.hydraulics._Q_in
         if Q_0Ik is None:
             Q_0Ik = self.hydraulics._Q_0Ik
         self.node_quantities()
-        self.link_coeffs(_dt=dt, _u_j_frac=u_j_frac)
+        self.link_coeffs(_dt=dt)
         self.node_coeffs(_Q_0Ik=Q_0Ik, _c_0Ik=c_0Ik, _dt=dt)
         self.forward_recurrence()
         self.backward_recurrence()
         self.boundary_coefficients()
         self.sparse_matrix_equations(c_bc=c_bc, _Q_0j=Q_0j,
                                      _c_0j=c_0j, _dt=dt)
         if self.hydraulics.banded:
@@ -987,68 +1023,74 @@
     result[cond] = num[cond] / den[cond]
     return result
 
 @njit
 def alpha_ik(Q_Ik, omega_Ik, dx_ik, D_ik, A_ik):
     # Use upwind scheme
     t_0 = - Q_Ik * omega_Ik
-    t_1 = - 4 * D_ik * A_ik / dx_ik
+    # TODO: Check if this is 4 or 2
+    t_1 = - 2 * D_ik * A_ik / dx_ik
     return t_0 + t_1
 
 @njit
-def beta_ik(dt, D_ik, A_ik, dx_ik, K_ik, Q_Ik, Q_Ip1k, omega_Ik, omega_Ip1k):
-    t_0 = dx_ik * A_ik / dt
-    t_1 = 8 * D_ik * A_ik / dx_ik
-    # Why is sign different on K here?
-    t_2 = K_ik * dx_ik * A_ik
-    t_3 = - Q_Ik * (1 - omega_Ik)
-    t_4 = Q_Ip1k * omega_Ip1k
+def beta_ik(dt, D_ik, A_ik, A_ik_prev, dx_ik, K_ik, Q_Ik, Q_Ip1k, omega_Ik, omega_Ip1k):
+    t_0 = Q_Ip1k * omega_Ip1k
+    t_1 = - Q_Ik * (1 - omega_Ik)
+    # TODO: Check if this is 4 or 8
+    t_2 = 4 * D_ik * A_ik / dx_ik
+    t_3 = K_ik * dx_ik * A_ik
+    t_4 = dx_ik * (2 * A_ik - A_ik_prev) / dt
     return t_0 + t_1 + t_2 + t_3 + t_4
 
 @njit
 def chi_ik(Q_Ip1k, omega_Ip1k, dx_ik, D_ik, A_ik):
     # Use upwind scheme
     t_0 = Q_Ip1k * (1 - omega_Ip1k)
-    t_1 = - 4 * D_ik * A_ik / dx_ik
+    # TODO: Check if this is 4 or 2
+    t_1 = - 2 * D_ik * A_ik / dx_ik
     return t_0 + t_1
 
 @njit
 def gamma_ik(dt, c_ik_prev, A_ik, dx_ik):
     t_0 = c_ik_prev * A_ik * dx_ik / dt
     return t_0
 
 @njit
 def kappa_Ik(Q_im1k_next, omega_im1k, D_Ik, A_Ik, dx_im1k):
     t_0 = - Q_im1k_next * omega_im1k
-    t_1 = - 4 * D_Ik * A_Ik / dx_im1k
-    # return t_0
+    # TODO: Check if this is 4 or 2
+    # TODO: Check if this is D_Ik, A_Ik or D_ik, A_ik
+    t_1 = - 2 * D_Ik * A_Ik / dx_im1k
     return t_0 + t_1
 
 @njit
-def lambda_Ik(A_SIk, h_Ik_next, Q_ik_next, Q_im1k_next, omega_ik, omega_im1k, dt, K_Ik, D_Ik,
-              A_Ik, dx_ik, dx_im1k):
-    t_0 = omega_ik * Q_ik_next
-    t_1 = - (1 - omega_im1k) * Q_im1k_next
-    t_2 = A_SIk * h_Ik_next * (1 / dt + K_Ik)
-    t_3 = 4 * D_Ik * A_Ik / dx_im1k
-    t_4 = 4 * D_Ik * A_Ik / dx_ik
-    return t_0 + t_1 + t_2 + t_3 + t_4
+def lambda_Ik(A_SIk, h_Ik_next, h_Ik_prev, Q_ik_next, Q_im1k_next, omega_ik, omega_im1k, dt,
+              K_Ik, D_ik, D_im1k, A_ik, A_im1k, dx_ik, dx_im1k):
+    t_0 = A_SIk * h_Ik_next * K_Ik
+    t_1 = omega_ik * Q_ik_next
+    t_2 = - (1 - omega_im1k) * Q_im1k_next
+    # TODO: Check if this is 4 or 2
+    t_3 = 2 * D_im1k * A_im1k / dx_im1k
+    t_4 = 2 * D_ik * A_ik / dx_ik
+    # TODO: Need to add h_Ik_prev
+    t_5 = A_SIk * (2 * h_Ik_next - h_Ik_prev) / dt
+    return t_0 + t_1 + t_2 + t_3 + t_4 + t_5
 
 @njit
 def mu_Ik(Q_ik_next, omega_ik, D_Ik, A_Ik, dx_ik):
     t_0 = Q_ik_next * (1 - omega_ik)
-    t_1 = - 4 * D_Ik * A_Ik / dx_ik
-    # return t_0
+    # TODO: Check if this is 4 or 2
+    # TODO: Check if this is D_Ik, A_Ik or D_ik, A_ik
+    t_1 = - 2 * D_Ik * A_Ik / dx_ik
     return t_0 + t_1
 
 @njit
-def eta_Ik(c_0_Ik, Q_0_Ik, A_SIk, h_Ik_prev, c_Ik_prev, B_ik, B_im1k,
-           dx_ik, dx_im1k, c_ik_prev, c_im1k_prev, dt):
+def eta_Ik(c_0_Ik, Q_0_Ik, A_SIk, h_Ik_next, c_Ik_prev, dt):
     t_0 = c_0_Ik * Q_0_Ik
-    t_1 = A_SIk * h_Ik_prev * c_Ik_prev / dt
+    t_1 = A_SIk * h_Ik_next * c_Ik_prev / dt
     return t_0 + t_1
 
 @njit
 def U_1k(chi_1k, beta_1k):
     return safe_divide(-chi_1k, beta_1k)
 
 @njit
@@ -1210,15 +1252,15 @@
     """
     num = Z_uk * sigma_dk
     den = D_k_star
     result = safe_divide_vec(num, den)
     return result
 
 @njit
-def omega_uk(Z_uk, V_dk, U_dk, Y_uk, X_uk, W_dk, theta_dk, xi_uk, xi_dk, D_k_star):
+def zeta_uk(Z_uk, V_dk, U_dk, Y_uk, X_uk, W_dk, theta_dk, xi_uk, xi_dk, D_k_star):
     """
     Compute superlink boundary condition coefficient 'chi' for upstream end
     of superlink k.
     """
     t_0 = (1 - U_dk * theta_dk) * (Y_uk + X_uk * xi_uk + Z_uk * xi_dk)
     t_1 = Z_uk * theta_dk * (V_dk + U_dk * xi_dk + W_dk * xi_uk)
     num = t_0 + t_1
@@ -1245,15 +1287,15 @@
     """
     num = W_dk * theta_uk * Z_uk * sigma_dk + (1 - X_uk * theta_uk) * U_dk * sigma_dk
     den = D_k_star
     result = safe_divide_vec(num, den)
     return result
 
 @njit
-def omega_dk(W_dk, Y_uk, X_uk, V_dk, Z_uk, U_dk, theta_uk, xi_uk, xi_dk, D_k_star):
+def zeta_dk(W_dk, Y_uk, X_uk, V_dk, Z_uk, U_dk, theta_uk, xi_uk, xi_dk, D_k_star):
     """
     Compute superlink boundary condition coefficient 'chi' for downstream end
     of superlink k.
     """
     t_0 = W_dk * theta_uk * (Y_uk + X_uk * xi_uk + Z_uk * xi_dk)
     t_1 = (1 - X_uk * theta_uk) * (V_dk + U_dk * xi_dk + W_dk * xi_uk)
     num = t_0 + t_1
@@ -1261,53 +1303,54 @@
     result = safe_divide_vec(num, den)
     return result
 
 @njit
 def numba_node_coeffs(_kappa_Ik, _lambda_Ik, _mu_Ik, _eta_Ik, _Q_ik_next,
                       _h_Ik_next, _h_Ik_prev, _c_Ik_prev, _c_ik_prev,
                       _Q_uk_next, _Q_dk_next, _c_0Ik, _Q_0Ik, _A_SIk, _K_Ik,
-                      _K_ik, _B_ik_next, _A_ik_next, _dx_ik_next, _forward_I_i,
+                      _K_ik, _A_ik_next, _dx_ik_next, _forward_I_i,
                       _backward_I_i, _is_start, _is_end, _kI, _dt, _omega_ik,
-                      _omega_uk, _omega_dk, _D_Ik, _A_Ik_next, _dx_uk, _dx_dk):
+                      _omega_uk, _omega_dk, _D_Ik, _D_ik, _A_Ik_next, _dx_uk, _dx_dk,
+                      _D_uk, _D_dk, _A_uk_next, _A_dk_next):
     N = _kI.size
     for I in range(N):
         if _is_start[I]:
             i = _forward_I_i[I]
             k = _kI[I]
-            _kappa_Ik[I] = kappa_Ik(_Q_uk_next[k], _omega_uk[k], _D_Ik[I], _A_Ik_next[I], _dx_uk[k])
-            _lambda_Ik[I] = lambda_Ik(_A_SIk[I], _h_Ik_next[I], _Q_ik_next[i], _Q_uk_next[k],
-                                      _omega_ik[i], _omega_uk[k], _dt, _K_Ik[I], _D_Ik[I],
-                                      _A_Ik_next[I], _dx_ik_next[i], _dx_uk[k])
-            _mu_Ik[I] = mu_Ik(_Q_ik_next[i], _omega_ik[i], _D_Ik[I], _A_Ik_next[I], _dx_ik_next[i])
-            _eta_Ik[I] = eta_Ik(_c_0Ik[I], _Q_0Ik[I], _A_SIk[I], _h_Ik_prev[I], _c_Ik_prev[I],
-                                _B_ik_next[i], 0.0, _dx_ik_next[i], 0.0, _c_ik_prev[i], 0.0, _dt)
+            _kappa_Ik[I] = kappa_Ik(_Q_uk_next[k], _omega_uk[k], _D_uk[k], _A_uk_next[k], _dx_uk[k])
+            _lambda_Ik[I] = lambda_Ik(_A_SIk[I], _h_Ik_next[I], _h_Ik_prev[I], _Q_ik_next[i],
+                                      _Q_uk_next[k], _omega_ik[i], _omega_uk[k], _dt, _K_Ik[I],
+                                      _D_ik[i], _D_uk[k], _A_ik_next[i], _A_uk_next[k],
+                                      _dx_ik_next[i], _dx_uk[k])
+            _mu_Ik[I] = mu_Ik(_Q_ik_next[i], _omega_ik[i], _D_ik[i], _A_ik_next[i], _dx_ik_next[i])
+            _eta_Ik[I] = eta_Ik(_c_0Ik[I], _Q_0Ik[I], _A_SIk[I], _h_Ik_next[I], _c_Ik_prev[I], _dt)
         elif _is_end[I]:
             im1 = _backward_I_i[I]
             k = _kI[I]
-            _kappa_Ik[I] = kappa_Ik(_Q_ik_next[im1], _omega_ik[im1], _D_Ik[I], _A_Ik_next[I],
+            # TODO: Possible out-of-bounds error
+            _kappa_Ik[I] = kappa_Ik(_Q_ik_next[im1], _omega_ik[im1], _D_ik[im1], _A_ik_next[im1],
                                     _dx_ik_next[im1])
-            _lambda_Ik[I] = lambda_Ik(_A_SIk[I], _h_Ik_next[I], _Q_dk_next[k], _Q_ik_next[im1],
-                                      _omega_dk[k], _omega_ik[im1], _dt, _K_Ik[I], _D_Ik[I],
-                                      _A_Ik_next[I], _dx_dk[k], _dx_ik_next[im1])
-            _mu_Ik[I] = mu_Ik(_Q_dk_next[k], _omega_dk[k], _D_Ik[I], _A_Ik_next[I], _dx_dk[k])
-            _eta_Ik[I] = eta_Ik(_c_0Ik[I], _Q_0Ik[I], _A_SIk[I], _h_Ik_prev[I],
-                                _c_Ik_prev[I], 0.0, _B_ik_next[im1], 0.0, _dx_ik_next[im1],
-                                0.0, _c_ik_prev[im1], _dt)
+            _lambda_Ik[I] = lambda_Ik(_A_SIk[I], _h_Ik_next[I], _h_Ik_prev[I], _Q_dk_next[k],
+                                      _Q_ik_next[im1], _omega_dk[k], _omega_ik[im1], _dt, _K_Ik[I],
+                                      _D_dk[k], _D_ik[im1], _A_dk_next[k], _A_ik_next[im1],
+                                      _dx_dk[k], _dx_ik_next[im1])
+            _mu_Ik[I] = mu_Ik(_Q_dk_next[k], _omega_dk[k], _D_dk[k], _A_dk_next[k], _dx_dk[k])
+            _eta_Ik[I] = eta_Ik(_c_0Ik[I], _Q_0Ik[I], _A_SIk[I], _h_Ik_next[I],
+                                _c_Ik_prev[I], _dt)
         else:
             i = _forward_I_i[I]
             im1 = i - 1
-            _kappa_Ik[I] = kappa_Ik(_Q_ik_next[im1], _omega_ik[im1], _D_Ik[I], _A_Ik_next[I],
+            _kappa_Ik[I] = kappa_Ik(_Q_ik_next[im1], _omega_ik[im1], _D_ik[im1], _A_ik_next[im1],
                                     _dx_ik_next[im1])
-            _lambda_Ik[I] = lambda_Ik(_A_SIk[I], _h_Ik_next[I], _Q_ik_next[i], _Q_ik_next[im1],
-                                      _omega_ik[i], _omega_ik[im1], _dt, _K_Ik[I], _D_Ik[I],
-                                      _A_Ik_next[I], _dx_ik_next[i], _dx_ik_next[im1])
-            _mu_Ik[I] = mu_Ik(_Q_ik_next[i], _omega_ik[i], _D_Ik[I], _A_Ik_next[I], _dx_ik_next[i])
-            _eta_Ik[I] = eta_Ik(_c_0Ik[I], _Q_0Ik[I], _A_SIk[I], _h_Ik_prev[I], _c_Ik_prev[I],
-                                _B_ik_next[i], _B_ik_next[im1], _dx_ik_next[i], _dx_ik_next[im1],
-                                _c_ik_prev[i], _c_ik_prev[im1], _dt)
+            _lambda_Ik[I] = lambda_Ik(_A_SIk[I], _h_Ik_next[I], _h_Ik_prev[I], _Q_ik_next[i],
+                                      _Q_ik_next[im1], _omega_ik[i], _omega_ik[im1], _dt,
+                                      _K_Ik[I], _D_ik[i], _D_ik[im1], _A_ik_next[i],
+                                      _A_ik_next[im1], _dx_ik_next[i], _dx_ik_next[im1])
+            _mu_Ik[I] = mu_Ik(_Q_ik_next[i], _omega_ik[i], _D_ik[i], _A_ik_next[i], _dx_ik_next[i])
+            _eta_Ik[I] = eta_Ik(_c_0Ik[I], _Q_0Ik[I], _A_SIk[I], _h_Ik_next[I], _c_Ik_prev[I], _dt)
     return 1
 
 @njit
 def numba_forward_recurrence(_T_ik, _U_Ik, _V_Ik, _W_Ik, _alpha_ik, _beta_ik, _chi_ik,
                              _gamma_ik, _kappa_Ik, _lambda_Ik, _mu_Ik, _eta_Ik,
                              NK, nk, _I_1k, _i_1k):
     for k in range(NK):
@@ -1380,15 +1423,15 @@
         _Y_uk[k] = Y_uk(_eta_Ik[_I_1], _mu_Ik[_I_1], _Y_Ik[_I_1], _kappa_Ik[_I_1])
         _Z_uk[k] = Z_uk(_mu_Ik[_I_1], _Z_Ik[_I_1], _kappa_Ik[_I_1])
         _U_dk[k] = U_dk(_kappa_Ik[_I_Np1], _U_Ik[_I_N], _lambda_Ik[_I_Np1], _mu_Ik[_I_Np1])
         _V_dk[k] = V_dk(_eta_Ik[_I_Np1], _kappa_Ik[_I_Np1], _V_Ik[_I_N], _mu_Ik[_I_Np1])
         _W_dk[k] = W_dk(_kappa_Ik[_I_Np1], _W_Ik[_I_N], _mu_Ik[_I_Np1])
     return 1
 
-@njit(fastmath=True)
+@njit(fastmath=False)
 def numba_add_at(a, indices, b):
     n = len(indices)
     for k in range(n):
         i = indices[k]
         a[i] += b[k]
 
 @njit
@@ -1399,40 +1442,45 @@
         _bc_u = bc[_J_u]
         _bc_d = bc[_J_d]
         if not _bc_u:
             A[_J_u, _J_d] = 0.0
         if not _bc_d:
             A[_J_d, _J_u] = 0.0
 
-@njit(fastmath=True)
+@njit(fastmath=False)
 def numba_create_A_matrix(A, _F_jj, bc, _J_uk, _J_dk, _rho_uk, _rho_dk, _tau_uk, _tau_dk,
-                          _Q_uk, _Q_dk, _OMEGA_UK, _OMEGA_DK, _A_sj, _V_sj, _H_j_next, _dt,
-                          _K_j, M, NK):
-    kuj = _rho_uk * _OMEGA_UK * _Q_uk + (1 - _OMEGA_UK)
-    kdj = -(_tau_dk * _OMEGA_DK * _Q_dk + (1 - _OMEGA_DK))
-    numba_add_at(_F_jj, _J_uk, kuj)
-    numba_add_at(_F_jj, _J_dk, kdj)
-    _F_jj += (_A_sj * _H_j_next / _dt) + (_K_j * _V_sj)
+                          _Q_uk, _Q_dk, _omega_uk, _omega_dk, _V_j_next, _V_j_prev, _H_j_next, _dt,
+                          _K_j, _D_uk, _D_dk, _A_uk_next, _A_dk_next, _dx_uk, _dx_dk, M, NK):
+    # TODO: Grouping of Q multiplication changed
+    kuj = (- _Q_uk * (_omega_uk + (1 - _omega_uk) * _rho_uk)
+           + 2 * _D_uk * _A_uk_next * (_rho_uk - 1) / _dx_uk)
+    kdj = (_Q_dk * (_tau_dk * _omega_dk + (1 - _omega_dk))
+           + 2 * _D_dk * _A_dk_next * (_tau_dk - 1) / _dx_dk)
+    numba_add_at(_F_jj, _J_uk, -kuj)
+    numba_add_at(_F_jj, _J_dk, -kdj)
+    _F_jj += (2 * _V_j_next - _V_j_prev) / _dt + (_K_j * _V_j_next)
     # Set diagonal of A matrix
     for i in range(M):
         if bc[i]:
             A[i,i] = 1.0
         else:
             A[i,i] = _F_jj[i]
     for k in range(NK):
         _J_u = _J_uk[k]
         _J_d = _J_dk[k]
         _bc_u = bc[_J_u]
         _bc_d = bc[_J_d]
         if not _bc_u:
-            A[_J_u, _J_d] += (_tau_uk[k] * _Q_uk[k])
+            A[_J_u, _J_d] -= _tau_uk[k] * (-_Q_uk[k] * (1 - _omega_uk[k])
+                              + 2 * _D_uk[k] * _A_uk_next[k] / _dx_uk[k])
         if not _bc_d:
-            A[_J_d, _J_u] -= (_rho_dk[k] * _Q_dk[k])
+            A[_J_d, _J_u] -= _rho_dk[k] * (_Q_dk[k] * _omega_dk[k]
+                              + 2 * _D_dk[k] * _A_dk_next[k] / _dx_dk[k])
 
-@njit(fastmath=True)
+@njit(fastmath=False)
 def numba_create_OWP_matrix(X, diag, bc, _J_uc, _J_dc, _omega_c, _Q_c, M, NC):
     # Set diagonal
     numba_add_at(diag, _J_uc, _Q_c * _omega_c)
     numba_add_at(diag, _J_dc, -_Q_c * (1 - _omega_c))
     for i in range(M):
         if bc[i]:
             X[i,i] = 0.0
```

### Comparing `pipedream-solver-0.2/pipedream_solver/nutils.py` & `pipedream-solver-0.2.2/pipedream_solver/nutils.py`

 * *Files identical despite different names*

### Comparing `pipedream-solver-0.2/pipedream_solver/infiltration.py` & `pipedream-solver-0.2.2/pipedream_solver/infiltration.py`

 * *Files identical despite different names*

