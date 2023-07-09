# Comparing `tmp/meow-sim-0.7.0.tar.gz` & `tmp/meow-sim-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meow-sim-0.7.0.tar", last modified: Thu Jul  6 21:21:34 2023, max compression
+gzip compressed data, was "meow-sim-0.7.1.tar", last modified: Sun Jul  9 20:23:05 2023, max compression
```

## Comparing `meow-sim-0.7.0.tar` & `meow-sim-0.7.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:21:34.937969 meow-sim-0.7.0/
--rw-r--r--   0 root         (0) root         (0)    11347 2023-07-06 21:21:30.000000 meow-sim-0.7.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3241 2023-07-06 21:21:34.937969 meow-sim-0.7.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2223 2023-07-06 21:21:30.000000 meow-sim-0.7.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:21:34.933969 meow-sim-0.7.0/meow/
--rw-r--r--   0 root         (0) root         (0)     1414 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:21:34.933969 meow-sim-0.7.0/meow/assets/
--rw-r--r--   0 root         (0) root         (0)    10307 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/assets/silicon.csv
--rw-r--r--   0 root         (0) root         (0)     8535 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/assets/silicon_oxide.csv
--rw-r--r--   0 root         (0) root         (0)     8378 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/base_model.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/cache.py
--rw-r--r--   0 root         (0) root         (0)     8650 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/cell.py
--rw-r--r--   0 root         (0) root         (0)     4277 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/cross_section.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:21:34.933969 meow-sim-0.7.0/meow/eme/
--rw-r--r--   0 root         (0) root         (0)      623 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/eme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6217 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/eme/common.py
--rw-r--r--   0 root         (0) root         (0)     4895 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/eme/propagate.py
--rw-r--r--   0 root         (0) root         (0)     4351 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/eme/sax.py
--rw-r--r--   0 root         (0) root         (0)      551 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/environment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:21:34.933969 meow-sim-0.7.0/meow/fde/
--rw-r--r--   0 root         (0) root         (0)      324 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/fde/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4915 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/fde/lumerical.py
--rw-r--r--   0 root         (0) root         (0)     3259 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/fde/tidy3d.py
--rw-r--r--   0 root         (0) root         (0)     2326 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/gds_structures.py
--rw-r--r--   0 root         (0) root         (0)    12464 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/geometries.py
--rw-r--r--   0 root         (0) root         (0)      960 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/integrate.py
--rw-r--r--   0 root         (0) root         (0)    12796 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/materials.py
--rw-r--r--   0 root         (0) root         (0)     5376 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/mesh.py
--rw-r--r--   0 root         (0) root         (0)    17433 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/mode.py
--rw-r--r--   0 root         (0) root         (0)     4445 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/structures.py
--rw-r--r--   0 root         (0) root         (0)     8090 2023-07-06 21:21:30.000000 meow-sim-0.7.0/meow/visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:21:34.933969 meow-sim-0.7.0/meow_sim.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3241 2023-07-06 21:21:34.000000 meow-sim-0.7.0/meow_sim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      708 2023-07-06 21:21:34.000000 meow-sim-0.7.0/meow_sim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 21:21:34.000000 meow-sim-0.7.0/meow_sim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      444 2023-07-06 21:21:34.000000 meow-sim-0.7.0/meow_sim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-07-06 21:21:34.000000 meow-sim-0.7.0/meow_sim.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1864 2023-07-06 21:21:30.000000 meow-sim-0.7.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 21:21:34.937969 meow-sim-0.7.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 21:21:34.937969 meow-sim-0.7.0/tests/
--rw-r--r--   0 root         (0) root         (0)      359 2023-07-06 21:21:30.000000 meow-sim-0.7.0/tests/test_deserialization.py
--rw-r--r--   0 root         (0) root         (0)      687 2023-07-06 21:21:30.000000 meow-sim-0.7.0/tests/test_mode_operators.py
--rw-r--r--   0 root         (0) root         (0)     1322 2023-07-06 21:21:30.000000 meow-sim-0.7.0/tests/test_nbs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:23:05.004513 meow-sim-0.7.1/
+-rw-r--r--   0 root         (0) root         (0)    11347 2023-07-09 20:23:00.000000 meow-sim-0.7.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-07-09 20:23:05.004513 meow-sim-0.7.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2223 2023-07-09 20:23:00.000000 meow-sim-0.7.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:23:05.000513 meow-sim-0.7.1/meow/
+-rw-r--r--   0 root         (0) root         (0)     3747 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:23:05.000513 meow-sim-0.7.1/meow/assets/
+-rw-r--r--   0 root         (0) root         (0)    10307 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/assets/silicon.csv
+-rw-r--r--   0 root         (0) root         (0)     8535 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/assets/silicon_oxide.csv
+-rw-r--r--   0 root         (0) root         (0)     8378 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/base_model.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/cache.py
+-rw-r--r--   0 root         (0) root         (0)     8828 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/cell.py
+-rw-r--r--   0 root         (0) root         (0)     4279 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/cross_section.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:23:05.000513 meow-sim-0.7.1/meow/eme/
+-rw-r--r--   0 root         (0) root         (0)      623 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/eme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6217 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/eme/common.py
+-rw-r--r--   0 root         (0) root         (0)     4895 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/eme/propagate.py
+-rw-r--r--   0 root         (0) root         (0)     4351 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/eme/sax.py
+-rw-r--r--   0 root         (0) root         (0)      551 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/environment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:23:05.000513 meow-sim-0.7.1/meow/fde/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/fde/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4915 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/fde/lumerical.py
+-rw-r--r--   0 root         (0) root         (0)     3259 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/fde/tidy3d.py
+-rw-r--r--   0 root         (0) root         (0)     2326 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/gds_structures.py
+-rw-r--r--   0 root         (0) root         (0)    12464 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/geometries.py
+-rw-r--r--   0 root         (0) root         (0)      960 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/integrate.py
+-rw-r--r--   0 root         (0) root         (0)    12796 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/materials.py
+-rw-r--r--   0 root         (0) root         (0)     5376 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/mesh.py
+-rw-r--r--   0 root         (0) root         (0)    17433 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/mode.py
+-rw-r--r--   0 root         (0) root         (0)     4454 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/structures.py
+-rw-r--r--   0 root         (0) root         (0)     8092 2023-07-09 20:23:00.000000 meow-sim-0.7.1/meow/visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:23:05.004513 meow-sim-0.7.1/meow_sim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-07-09 20:23:04.000000 meow-sim-0.7.1/meow_sim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      708 2023-07-09 20:23:04.000000 meow-sim-0.7.1/meow_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 20:23:04.000000 meow-sim-0.7.1/meow_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      444 2023-07-09 20:23:04.000000 meow-sim-0.7.1/meow_sim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-09 20:23:04.000000 meow-sim-0.7.1/meow_sim.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-07-09 20:23:00.000000 meow-sim-0.7.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-09 20:23:05.004513 meow-sim-0.7.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:23:05.004513 meow-sim-0.7.1/tests/
+-rw-r--r--   0 root         (0) root         (0)      359 2023-07-09 20:23:00.000000 meow-sim-0.7.1/tests/test_deserialization.py
+-rw-r--r--   0 root         (0) root         (0)      687 2023-07-09 20:23:00.000000 meow-sim-0.7.1/tests/test_mode_operators.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-07-09 20:23:00.000000 meow-sim-0.7.1/tests/test_nbs.py
```

### Comparing `meow-sim-0.7.0/LICENSE` & `meow-sim-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.0/PKG-INFO` & `meow-sim-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.7.0
+Version: 0.7.1
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.7.0/README.md` & `meow-sim-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.0/meow/assets/silicon.csv` & `meow-sim-0.7.1/meow/assets/silicon.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.0/meow/assets/silicon_oxide.csv` & `meow-sim-0.7.1/meow/assets/silicon_oxide.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.0/meow/base_model.py` & `meow-sim-0.7.1/meow/base_model.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.0/meow/cache.py` & `meow-sim-0.7.1/meow/cache.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.0/meow/cell.py` & `meow-sim-0.7.1/meow/cell.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """ an EME Cell """
 
+import warnings
 from typing import Dict, List, Tuple, Union, cast
 
 import numpy as np
 from pydantic import Field
 from scipy.ndimage import convolve
 
 from .base_model import BaseModel, _array, cached_property
 from .materials import Material
 from .mesh import Mesh2D
 from .structures import (
     Structure2D,
     Structure3D,
-    classify_structures_by_mesh_order_and_material,
-    sort_structures,
+    _classify_structures_by_mesh_order_and_material,
+    _sort_structures,
 )
 
 
 class Cell(BaseModel):
     """A Cell defines an interval in z (the direction of propagation) within
     the simulation domain. The intersecting Structure3Ds are discretized by
     a given mesh at the center of the Cell"""
@@ -36,15 +37,15 @@
     @property
     def length(self):
         return np.abs(self.z_max - self.z_min)
 
     @cached_property
     def materials(self):
         materials = {}
-        for i, structure in enumerate(sort_structures(self.structures), start=1):
+        for i, structure in enumerate(_sort_structures(self.structures), start=1):
             if not structure.material in materials:
                 materials[structure.material] = i
         return materials
 
     @cached_property
     def structures_2d(self) -> List[Structure2D]:
         z = 0.5 * (self.z_min + self.z_max)
@@ -102,14 +103,18 @@
 def create_cells(
     structures: List[Structure3D],
     mesh: Union[Mesh2D, List[Mesh2D]],
     Ls: np.ndarray[Tuple[int], np.dtype[np.float_]],
     z_min: float = 0.0,
 ) -> List[Cell]:
     """easily create multiple `Cell` objects given a `Mesh` and a collection of cell lengths"""
+    warnings.warn(
+        "create_cells will be removed in a future version. Please create your cells in a loop instead.",
+        DeprecationWarning,
+    )
 
     Ls = np.asarray(Ls, float)
     if Ls.ndim != 1:
         raise ValueError(f"Ls should be 1D. Got shape: {Ls.shape}.")
     if Ls.shape[0] < 0:
         raise ValueError(f"length of Ls array should be nonzero. Got: {Ls}.")
 
@@ -135,15 +140,15 @@
 
 def _create_full_material_array(
     mesh: Mesh2D,
     structures: List[Structure2D],
     materials: Dict[Material, int],
 ):
     m_full = np.zeros_like(mesh.X_full, dtype=np.int_)
-    structures_dict = classify_structures_by_mesh_order_and_material(
+    structures_dict = _classify_structures_by_mesh_order_and_material(
         structures, materials
     )
     for structures in structures_dict.values():
         _m_full = _create_material_array(mesh, materials, structures)
         mask = _m_full > 0
         m_full[mask] = _m_full[mask]
```

### Comparing `meow-sim-0.7.0/meow/cross_section.py` & `meow-sim-0.7.1/meow/cross_section.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from typing import List, Optional
 
 import numpy as np
 from pydantic import Field
 
 from .base_model import BaseModel, _array, cached_property
-from .cell import Cell, _create_full_material_array, sort_structures
+from .cell import Cell, _create_full_material_array, _sort_structures
 from .environment import Environment
 from .mesh import Mesh2D
 from .structures import Structure2D
 
 
 class CrossSection(BaseModel):
     """A `CrossSection` is created from the association of a `Cell` with an `Environment`,
@@ -29,15 +29,15 @@
         cs = cls(structures=cell.structures_2d, mesh=cell.mesh, env=env)
         cs._cache["cell"] = cell
         return cs
 
     @cached_property
     def materials(self):
         materials = {}
-        for i, structure in enumerate(sort_structures(self.structures), start=1):
+        for i, structure in enumerate(_sort_structures(self.structures), start=1):
             if not structure.material in materials:
                 materials[structure.material] = i
         return materials
 
     @cached_property
     def n_full(self):
         m_full = _create_full_material_array(self.mesh, self.structures, self.materials)
```

### Comparing `meow-sim-0.7.0/meow/eme/__init__.py` & `meow-sim-0.7.1/meow/eme/__init__.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.0/meow/eme/common.py` & `meow-sim-0.7.1/meow/eme/common.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.0/meow/eme/propagate.py` & `meow-sim-0.7.1/meow/eme/propagate.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.0/meow/eme/sax.py` & `meow-sim-0.7.1/meow/eme/sax.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.0/meow/environment.py` & `meow-sim-0.7.1/meow/environment.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.0/meow/fde/lumerical.py` & `meow-sim-0.7.1/meow/fde/lumerical.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.0/meow/fde/tidy3d.py` & `meow-sim-0.7.1/meow/fde/tidy3d.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.0/meow/gds_structures.py` & `meow-sim-0.7.1/meow/gds_structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.0/meow/geometries.py` & `meow-sim-0.7.1/meow/geometries.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.0/meow/integrate.py` & `meow-sim-0.7.1/meow/integrate.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.0/meow/materials.py` & `meow-sim-0.7.1/meow/materials.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.0/meow/mesh.py` & `meow-sim-0.7.1/meow/mesh.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.0/meow/mode.py` & `meow-sim-0.7.1/meow/mode.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.0/meow/structures.py` & `meow-sim-0.7.1/meow/structures.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,65 +74,65 @@
             scale=scale,
         )
 
     def _visualize(self, scale=None):
         return self._trimesh(scale=scale).show()
 
 
-def visualize_structures(structures: List[Structure3D], scale=None):
+def _visualize_structures(structures: List[Structure3D], scale=None):
     """easily visualize a collection (list) of `Structure3D` objects"""
     from trimesh.scene import Scene  # fmt: skip
     from trimesh.transformations import rotation_matrix  # fmt: skip
 
     scene = Scene(
-        geometry=[s._trimesh(scale=scale) for s in sort_structures(structures)]
+        geometry=[s._trimesh(scale=scale) for s in _sort_structures(structures)]
     )
     scene.apply_transform(rotation_matrix(np.pi - np.pi / 6, (0, 1, 0)))
     return scene.show()
 
 
 @overload
-def sort_structures(structures: List[Structure3D]) -> List[Structure3D]:
+def _sort_structures(structures: List[Structure3D]) -> List[Structure3D]:
     ...
 
 
 @overload
-def sort_structures(structures: List[Structure2D]) -> List[Structure2D]:
+def _sort_structures(structures: List[Structure2D]) -> List[Structure2D]:
     ...
 
 
-def sort_structures(
+def _sort_structures(
     structures: Union[List[Structure3D], List[Structure2D]]
 ) -> Union[List[Structure2D], List[Structure3D]]:
     struct_info = [(s.mesh_order, -i, s) for i, s in enumerate(structures)]
     sorted_struct_info = sorted(struct_info, key=lambda I: (I[0], I[1]), reverse=True)
     return [s for _, _, s in sorted_struct_info]  # type: ignore
 
 
 @overload
-def classify_structures_by_mesh_order_and_material(
+def _classify_structures_by_mesh_order_and_material(
     structures: List[Structure3D], materials: Dict[Material, int]
 ) -> Dict[Tuple[int, int], List[Structure3D]]:
     ...
 
 
 @overload
-def classify_structures_by_mesh_order_and_material(
+def _classify_structures_by_mesh_order_and_material(
     structures: List[Structure2D], materials: Dict[Material, int]
 ) -> Dict[Tuple[int, int], List[Structure2D]]:
     ...
 
 
-def classify_structures_by_mesh_order_and_material(
+def _classify_structures_by_mesh_order_and_material(
     structures: Union[List[Structure3D], List[Structure2D]],
     materials: Dict[Material, int],
 ) -> Union[
     Dict[Tuple[int, int], List[Structure2D]], Dict[Tuple[int, int], List[Structure3D]]
 ]:
-    structures = sort_structures(structures)
+    structures = _sort_structures(structures)
     structures_dict = {}
     for structure in structures:
         mo = structure.mesh_order
         mat = materials[structure.material]
         if (mo, mat) not in structures_dict:
             structures_dict[mo, mat] = []
         structures_dict[mo, mat].append(structure)
```

### Comparing `meow-sim-0.7.0/meow/visualize.py` & `meow-sim-0.7.1/meow/visualize.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ Visualizations for common meow-datatypes """
 
 from collections.abc import Iterable
 from typing import Any, Callable
 
 import numpy as np
 
-from meow.structures import visualize_structures
+from meow.structures import _visualize_structures
 
 try:
     import matplotlib.pyplot as plt  # fmt: skip
 
 
 except ImportError:
     plt = None
@@ -286,15 +286,15 @@
 def _is_gf_component(obj):
     return gf is not None and isinstance(obj, gf.Component)
 
 
 VISUALIZATION_MAPPING: dict[Callable, Callable] = {
     _is_base_model: _visualize_base_model,
     _is_mode_list: _visualize_modes,
-    _is_structure_3d_list: visualize_structures,
+    _is_structure_3d_list: _visualize_structures,
     _is_mode_overlap: _visualize_overlap_density,
     _is_s_matrix: _visualize_s_matrix,
     _is_s_pm_matrix: _visualize_s_pm_matrix,
     _is_gf_component: _visualize_gf_component,
 }
```

### Comparing `meow-sim-0.7.0/meow_sim.egg-info/PKG-INFO` & `meow-sim-0.7.1/meow_sim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.7.0
+Version: 0.7.1
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.7.0/meow_sim.egg-info/SOURCES.txt` & `meow-sim-0.7.1/meow_sim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.0/pyproject.toml` & `meow-sim-0.7.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["build", "pip", "setuptools", "wheel", "pybind11"]
 
 [project]
 name = "meow-sim"
-version = "0.7.0"
+version = "0.7.1"
 authors = [
 { name = "Rockley Photonics" },
 { name = "Floris Laporte", email = "floris.laporte@rockleyphotonics.com" },
 ]
 description = "Modeling of Eigenmodes and Overlaps in Waveguide Structures"
 requires-python = ">=3.8"
 keywords = [
```

### Comparing `meow-sim-0.7.0/tests/test_mode_operators.py` & `meow-sim-0.7.1/tests/test_mode_operators.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.7.0/tests/test_nbs.py` & `meow-sim-0.7.1/tests/test_nbs.py`

 * *Files identical despite different names*

