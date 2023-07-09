# Comparing `tmp/redplanet-0.0.1.dev0.tar.gz` & `tmp/redplanet-0.0.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redplanet-0.0.1.dev0.tar", last modified: Sun Jul  9 17:28:05 2023, max compression
+gzip compressed data, was "redplanet-0.0.1.dev1.tar", last modified: Sun Jul  9 17:42:29 2023, max compression
```

## Comparing `redplanet-0.0.1.dev0.tar` & `redplanet-0.0.1.dev1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 17:28:05.842551 redplanet-0.0.1.dev0/
--rw-rw-rw-   0        0        0    35821 2023-06-23 07:09:38.000000 redplanet-0.0.1.dev0/LICENSE.txt
--rw-rw-rw-   0        0        0    45691 2023-07-09 17:28:05.841295 redplanet-0.0.1.dev0/PKG-INFO
--rw-rw-rw-   0        0        0     3267 2023-07-09 16:44:42.000000 redplanet-0.0.1.dev0/README.md
--rw-rw-rw-   0        0        0     3336 2023-07-09 17:26:21.000000 redplanet-0.0.1.dev0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-09 17:28:05.843290 redplanet-0.0.1.dev0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-09 17:28:05.781000 redplanet-0.0.1.dev0/src/
-drwxrwxrwx   0        0        0        0 2023-07-09 17:28:05.790822 redplanet-0.0.1.dev0/src/redplanet/
-drwxrwxrwx   0        0        0        0 2023-07-09 17:28:05.831414 redplanet-0.0.1.dev0/src/redplanet/Crust/
--rw-rw-rw-   0        0        0    30071 2023-07-09 04:30:43.000000 redplanet-0.0.1.dev0/src/redplanet/Crust/Crust.py
--rw-rw-rw-   0        0        0     5800 2023-07-09 04:44:31.000000 redplanet-0.0.1.dev0/src/redplanet/Crust/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 17:28:05.838303 redplanet-0.0.1.dev0/src/redplanet/GRS/
--rw-rw-rw-   0        0        0    23508 2023-07-09 04:07:45.000000 redplanet-0.0.1.dev0/src/redplanet/GRS/GRS.py
--rw-rw-rw-   0        0        0     3226 2023-07-09 04:04:41.000000 redplanet-0.0.1.dev0/src/redplanet/GRS/__init__.py
--rw-rw-rw-   0        0        0     4529 2023-07-09 04:39:11.000000 redplanet-0.0.1.dev0/src/redplanet/__init__.py
--rw-rw-rw-   0        0        0     4733 2023-07-09 04:36:21.000000 redplanet-0.0.1.dev0/src/redplanet/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-09 17:28:05.827335 redplanet-0.0.1.dev0/src/redplanet.egg-info/
--rw-rw-rw-   0        0        0    45691 2023-07-09 17:28:05.000000 redplanet-0.0.1.dev0/src/redplanet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      385 2023-07-09 17:28:05.000000 redplanet-0.0.1.dev0/src/redplanet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 17:28:05.000000 redplanet-0.0.1.dev0/src/redplanet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2023-07-09 17:28:05.000000 redplanet-0.0.1.dev0/src/redplanet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-09 17:28:05.000000 redplanet-0.0.1.dev0/src/redplanet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-09 17:42:29.573420 redplanet-0.0.1.dev1/
+-rw-rw-rw-   0        0        0    35821 2023-06-23 07:09:38.000000 redplanet-0.0.1.dev1/LICENSE.txt
+-rw-rw-rw-   0        0        0    46226 2023-07-09 17:42:29.573420 redplanet-0.0.1.dev1/PKG-INFO
+-rw-rw-rw-   0        0        0     3791 2023-07-09 17:40:53.000000 redplanet-0.0.1.dev1/README.md
+-rw-rw-rw-   0        0        0     3348 2023-07-09 17:41:36.000000 redplanet-0.0.1.dev1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-09 17:42:29.573420 redplanet-0.0.1.dev1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-09 17:42:29.528037 redplanet-0.0.1.dev1/src/
+drwxrwxrwx   0        0        0        0 2023-07-09 17:42:29.534127 redplanet-0.0.1.dev1/src/redplanet/
+drwxrwxrwx   0        0        0        0 2023-07-09 17:42:29.568437 redplanet-0.0.1.dev1/src/redplanet/Crust/
+-rw-rw-rw-   0        0        0    30071 2023-07-09 04:30:43.000000 redplanet-0.0.1.dev1/src/redplanet/Crust/Crust.py
+-rw-rw-rw-   0        0        0     5800 2023-07-09 04:44:31.000000 redplanet-0.0.1.dev1/src/redplanet/Crust/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 17:42:29.571608 redplanet-0.0.1.dev1/src/redplanet/GRS/
+-rw-rw-rw-   0        0        0    23508 2023-07-09 04:07:45.000000 redplanet-0.0.1.dev1/src/redplanet/GRS/GRS.py
+-rw-rw-rw-   0        0        0     3226 2023-07-09 04:04:41.000000 redplanet-0.0.1.dev1/src/redplanet/GRS/__init__.py
+-rw-rw-rw-   0        0        0     4529 2023-07-09 04:39:11.000000 redplanet-0.0.1.dev1/src/redplanet/__init__.py
+-rw-rw-rw-   0        0        0     4733 2023-07-09 04:36:21.000000 redplanet-0.0.1.dev1/src/redplanet/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-09 17:42:29.565474 redplanet-0.0.1.dev1/src/redplanet.egg-info/
+-rw-rw-rw-   0        0        0    46226 2023-07-09 17:42:29.000000 redplanet-0.0.1.dev1/src/redplanet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2023-07-09 17:42:29.000000 redplanet-0.0.1.dev1/src/redplanet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 17:42:29.000000 redplanet-0.0.1.dev1/src/redplanet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2023-07-09 17:42:29.000000 redplanet-0.0.1.dev1/src/redplanet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-09 17:42:29.000000 redplanet-0.0.1.dev1/src/redplanet.egg-info/top_level.txt
```

### Comparing `redplanet-0.0.1.dev0/LICENSE.txt` & `redplanet-0.0.1.dev1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `redplanet-0.0.1.dev0/PKG-INFO` & `redplanet-0.0.1.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: redplanet
-Version: 0.0.1.dev0
-Summary: User-friendly access (i.e. APIs) for various Mars datasets and derived quantities. Create publication-ready plots on the fly or access the underlying data for more involved calculations.
+Version: 0.0.1.dev1
+Summary: User-friendly access (i.e. APIs) for various Mars datasets and derived geophysics quantities. Create publication-ready plots on the fly or access the underlying data for more involved calculations.
 Author-email: Zain Eris Kamal <zain.eris.kamal@rutgers.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -702,24 +702,25 @@
 RedPlanet is a Python package that gives an easy way to work with various Mars datasets. With straightforward methods and high customizability, you can either create publication-ready plots on the fly, or access the underlying data for more involved calculations.
 
 
 # Usage:
 
 Install with `pip install redplanet`.
 
-## `GRS`
+## GRS
 
 Access/visualize chemical abundance maps derived from the 2001 Mars Odyssey Gamma Ray Spectrometer. The original data is defined in 5 degree bins, but this module allows you to programmatically estimate values at exact coordinates by interpolating between points. Concentrations can be extracted for both the shallow subsurface (raw data) and bulk crustal composition (normalized to volatile-free basis, i.e. zero H2O/Cl/Si).
 
 &nbsp;
 
 - Example 1: Iron concentrations in Arabia Terra. Data is normalized to a volatile-free basis (H2O/Cl/Si free), so it is representative of the bulk crustal composition rather than shallow subsurface. 
 
 <p align="center">
-  <img width="600" src="docs/figures/GRS_fe_norm_ArabiaTerra.png">
+  <!-- <img width="600" src="docs/figures/GRS_fe_norm_ArabiaTerra.png"> -->
+  <img width="600" src="https://files.catbox.moe/irjxsp.png">
 </p>
 
 
 
 Recreate with: 
 ```python
 from redplanet import GRS
@@ -733,25 +734,26 @@
 )
 ```
 
 &nbsp;
 
 ----
 
-## `Crust`
+## Crust
 
 
 Access/visualize maps of topography, Moho, crustal thickness, and crustal density from spherical harmonics. We offer ~22,000 models of the crust-mantle interface parameterized by reference interior models, crustal thickness at the InSight landing, and homogeneous/inhomogeneous crustal densities across the dichotomy. 
 
 &nbsp;
 
 - Example 1: Topography, Moho, and crustal thickness of the Valles Marineris region. Model parameters are 41 km crustal thickness at the InSight landing, 2,900 kg/m^3 crustal density in the North, and 2,700 kg/m^3 crustal density in the South.
 
 <p align="center">
-  <img src="docs/figures/Crust_various_VallesMarineris.png">
+  <!-- <img src="docs/figures/Crust_various_VallesMarineris.png"> -->
+  <img src="https://files.catbox.moe/tnk9io.png">
 </p>
 
 
 Recreate with:
 ```python
 from redplanet import Crust
 lons = (-100,-20)
@@ -763,31 +765,34 @@
 ```
 
 &nbsp;
 
 - Example 2: Crustal thickness profile of Henry Crater with various crust-mantle interface models.
 
 <p align="center">
-  <img src="docs/figures/Crust_thick-profile_Henry.png">
+  <!-- <img src="docs/figures/Crust_thick-profile_Henry.png"> -->
+  <img src="https://files.catbox.moe/nnnm3l.png">
 </p>
 
 
-Recreate with: See [docs/notebooks/demo/demo.ipynb](docs/notebooks/demo/demo.ipynb) section 2.2.
+Recreate with: See section 2.2 in [demo.ipynb](https://github.com/Humboldt-Penguin/redplanet/blob/main/docs/notebooks/demo/demo.ipynb).
 
 &nbsp;
 
 ---
 
 # Documentation
 
-For a more in-depth tutorial in interactive notebook format, see [docs/notebooks/demo/demo.ipynb](docs/notebooks/demo/demo.ipynb).
+<!-- For a more in-depth tutorial in interactive notebook format, see [docs/notebooks/demo/demo.ipynb](docs/notebooks/demo/demo.ipynb). -->
+For a more in-depth tutorial in interactive notebook format, see [demo.ipynb](https://github.com/Humboldt-Penguin/redplanet/blob/main/docs/notebooks/demo/demo.ipynb).
 
+&nbsp;
 
 ---
 
 # Links
 
 - Don't hesitate to reach out: [zain.eris.kamal@rutgers.edu](mailto:zain.eris.kamal@rutgers.edu)
-- Acknowledgements: [docs/thanks.txt](docs/thanks.txt)
-- References: [docs/references.txt](docs/references.txt)
+- Acknowledgements: [docs/thanks.txt](https://github.com/Humboldt-Penguin/redplanet/blob/main/docs/thanks.txt)
+- References: [docs/references.txt](https://github.com/Humboldt-Penguin/redplanet/blob/main/docs/references.txt)
 - Other work: [github.com/Humboldt-Penguin](https://github.com/Humboldt-Penguin)
```

### Comparing `redplanet-0.0.1.dev0/README.md` & `redplanet-0.0.1.dev1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 RedPlanet is a Python package that gives an easy way to work with various Mars datasets. With straightforward methods and high customizability, you can either create publication-ready plots on the fly, or access the underlying data for more involved calculations.
 
 
 # Usage:
 
 Install with `pip install redplanet`.
 
-## `GRS`
+## GRS
 
 Access/visualize chemical abundance maps derived from the 2001 Mars Odyssey Gamma Ray Spectrometer. The original data is defined in 5 degree bins, but this module allows you to programmatically estimate values at exact coordinates by interpolating between points. Concentrations can be extracted for both the shallow subsurface (raw data) and bulk crustal composition (normalized to volatile-free basis, i.e. zero H2O/Cl/Si).
 
 &nbsp;
 
 - Example 1: Iron concentrations in Arabia Terra. Data is normalized to a volatile-free basis (H2O/Cl/Si free), so it is representative of the bulk crustal composition rather than shallow subsurface. 
 
 <p align="center">
-  <img width="600" src="docs/figures/GRS_fe_norm_ArabiaTerra.png">
+  <!-- <img width="600" src="docs/figures/GRS_fe_norm_ArabiaTerra.png"> -->
+  <img width="600" src="https://files.catbox.moe/irjxsp.png">
 </p>
 
 
 
 Recreate with: 
 ```python
 from redplanet import GRS
@@ -34,25 +35,26 @@
 )
 ```
 
 &nbsp;
 
 ----
 
-## `Crust`
+## Crust
 
 
 Access/visualize maps of topography, Moho, crustal thickness, and crustal density from spherical harmonics. We offer ~22,000 models of the crust-mantle interface parameterized by reference interior models, crustal thickness at the InSight landing, and homogeneous/inhomogeneous crustal densities across the dichotomy. 
 
 &nbsp;
 
 - Example 1: Topography, Moho, and crustal thickness of the Valles Marineris region. Model parameters are 41 km crustal thickness at the InSight landing, 2,900 kg/m^3 crustal density in the North, and 2,700 kg/m^3 crustal density in the South.
 
 <p align="center">
-  <img src="docs/figures/Crust_various_VallesMarineris.png">
+  <!-- <img src="docs/figures/Crust_various_VallesMarineris.png"> -->
+  <img src="https://files.catbox.moe/tnk9io.png">
 </p>
 
 
 Recreate with:
 ```python
 from redplanet import Crust
 lons = (-100,-20)
@@ -64,31 +66,34 @@
 ```
 
 &nbsp;
 
 - Example 2: Crustal thickness profile of Henry Crater with various crust-mantle interface models.
 
 <p align="center">
-  <img src="docs/figures/Crust_thick-profile_Henry.png">
+  <!-- <img src="docs/figures/Crust_thick-profile_Henry.png"> -->
+  <img src="https://files.catbox.moe/nnnm3l.png">
 </p>
 
 
-Recreate with: See [docs/notebooks/demo/demo.ipynb](docs/notebooks/demo/demo.ipynb) section 2.2.
+Recreate with: See section 2.2 in [demo.ipynb](https://github.com/Humboldt-Penguin/redplanet/blob/main/docs/notebooks/demo/demo.ipynb).
 
 &nbsp;
 
 ---
 
 # Documentation
 
-For a more in-depth tutorial in interactive notebook format, see [docs/notebooks/demo/demo.ipynb](docs/notebooks/demo/demo.ipynb).
+<!-- For a more in-depth tutorial in interactive notebook format, see [docs/notebooks/demo/demo.ipynb](docs/notebooks/demo/demo.ipynb). -->
+For a more in-depth tutorial in interactive notebook format, see [demo.ipynb](https://github.com/Humboldt-Penguin/redplanet/blob/main/docs/notebooks/demo/demo.ipynb).
 
+&nbsp;
 
 ---
 
 # Links
 
 - Don't hesitate to reach out: [zain.eris.kamal@rutgers.edu](mailto:zain.eris.kamal@rutgers.edu)
-- Acknowledgements: [docs/thanks.txt](docs/thanks.txt)
-- References: [docs/references.txt](docs/references.txt)
+- Acknowledgements: [docs/thanks.txt](https://github.com/Humboldt-Penguin/redplanet/blob/main/docs/thanks.txt)
+- References: [docs/references.txt](https://github.com/Humboldt-Penguin/redplanet/blob/main/docs/references.txt)
 - Other work: [github.com/Humboldt-Penguin](https://github.com/Humboldt-Penguin)
```

### Comparing `redplanet-0.0.1.dev0/pyproject.toml` & `redplanet-0.0.1.dev1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 
 
 
 #######################################################################
 [project]
 
 name = "redplanet" 
-version = "0.0.1.dev" 
+version = "0.0.1.dev1" 
 
-description = "User-friendly access (i.e. APIs) for various Mars datasets and derived quantities. Create publication-ready plots on the fly or access the underlying data for more involved calculations." 
+description = "User-friendly access (i.e. APIs) for various Mars datasets and derived geophysics quantities. Create publication-ready plots on the fly or access the underlying data for more involved calculations." 
 readme = "README.md"
 
 authors = [{name = "Zain Eris Kamal", email = "zain.eris.kamal@rutgers.edu" }]
 
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
```

### Comparing `redplanet-0.0.1.dev0/src/redplanet/Crust/Crust.py` & `redplanet-0.0.1.dev1/src/redplanet/Crust/Crust.py`

 * *Files identical despite different names*

### Comparing `redplanet-0.0.1.dev0/src/redplanet/Crust/__init__.py` & `redplanet-0.0.1.dev1/src/redplanet/Crust/__init__.py`

 * *Files identical despite different names*

### Comparing `redplanet-0.0.1.dev0/src/redplanet/GRS/GRS.py` & `redplanet-0.0.1.dev1/src/redplanet/GRS/GRS.py`

 * *Files identical despite different names*

### Comparing `redplanet-0.0.1.dev0/src/redplanet/GRS/__init__.py` & `redplanet-0.0.1.dev1/src/redplanet/GRS/__init__.py`

 * *Files identical despite different names*

### Comparing `redplanet-0.0.1.dev0/src/redplanet/__init__.py` & `redplanet-0.0.1.dev1/src/redplanet/__init__.py`

 * *Files identical despite different names*

### Comparing `redplanet-0.0.1.dev0/src/redplanet/utils.py` & `redplanet-0.0.1.dev1/src/redplanet/utils.py`

 * *Files identical despite different names*

### Comparing `redplanet-0.0.1.dev0/src/redplanet.egg-info/PKG-INFO` & `redplanet-0.0.1.dev1/src/redplanet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: redplanet
-Version: 0.0.1.dev0
-Summary: User-friendly access (i.e. APIs) for various Mars datasets and derived quantities. Create publication-ready plots on the fly or access the underlying data for more involved calculations.
+Version: 0.0.1.dev1
+Summary: User-friendly access (i.e. APIs) for various Mars datasets and derived geophysics quantities. Create publication-ready plots on the fly or access the underlying data for more involved calculations.
 Author-email: Zain Eris Kamal <zain.eris.kamal@rutgers.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -702,24 +702,25 @@
 RedPlanet is a Python package that gives an easy way to work with various Mars datasets. With straightforward methods and high customizability, you can either create publication-ready plots on the fly, or access the underlying data for more involved calculations.
 
 
 # Usage:
 
 Install with `pip install redplanet`.
 
-## `GRS`
+## GRS
 
 Access/visualize chemical abundance maps derived from the 2001 Mars Odyssey Gamma Ray Spectrometer. The original data is defined in 5 degree bins, but this module allows you to programmatically estimate values at exact coordinates by interpolating between points. Concentrations can be extracted for both the shallow subsurface (raw data) and bulk crustal composition (normalized to volatile-free basis, i.e. zero H2O/Cl/Si).
 
 &nbsp;
 
 - Example 1: Iron concentrations in Arabia Terra. Data is normalized to a volatile-free basis (H2O/Cl/Si free), so it is representative of the bulk crustal composition rather than shallow subsurface. 
 
 <p align="center">
-  <img width="600" src="docs/figures/GRS_fe_norm_ArabiaTerra.png">
+  <!-- <img width="600" src="docs/figures/GRS_fe_norm_ArabiaTerra.png"> -->
+  <img width="600" src="https://files.catbox.moe/irjxsp.png">
 </p>
 
 
 
 Recreate with: 
 ```python
 from redplanet import GRS
@@ -733,25 +734,26 @@
 )
 ```
 
 &nbsp;
 
 ----
 
-## `Crust`
+## Crust
 
 
 Access/visualize maps of topography, Moho, crustal thickness, and crustal density from spherical harmonics. We offer ~22,000 models of the crust-mantle interface parameterized by reference interior models, crustal thickness at the InSight landing, and homogeneous/inhomogeneous crustal densities across the dichotomy. 
 
 &nbsp;
 
 - Example 1: Topography, Moho, and crustal thickness of the Valles Marineris region. Model parameters are 41 km crustal thickness at the InSight landing, 2,900 kg/m^3 crustal density in the North, and 2,700 kg/m^3 crustal density in the South.
 
 <p align="center">
-  <img src="docs/figures/Crust_various_VallesMarineris.png">
+  <!-- <img src="docs/figures/Crust_various_VallesMarineris.png"> -->
+  <img src="https://files.catbox.moe/tnk9io.png">
 </p>
 
 
 Recreate with:
 ```python
 from redplanet import Crust
 lons = (-100,-20)
@@ -763,31 +765,34 @@
 ```
 
 &nbsp;
 
 - Example 2: Crustal thickness profile of Henry Crater with various crust-mantle interface models.
 
 <p align="center">
-  <img src="docs/figures/Crust_thick-profile_Henry.png">
+  <!-- <img src="docs/figures/Crust_thick-profile_Henry.png"> -->
+  <img src="https://files.catbox.moe/nnnm3l.png">
 </p>
 
 
-Recreate with: See [docs/notebooks/demo/demo.ipynb](docs/notebooks/demo/demo.ipynb) section 2.2.
+Recreate with: See section 2.2 in [demo.ipynb](https://github.com/Humboldt-Penguin/redplanet/blob/main/docs/notebooks/demo/demo.ipynb).
 
 &nbsp;
 
 ---
 
 # Documentation
 
-For a more in-depth tutorial in interactive notebook format, see [docs/notebooks/demo/demo.ipynb](docs/notebooks/demo/demo.ipynb).
+<!-- For a more in-depth tutorial in interactive notebook format, see [docs/notebooks/demo/demo.ipynb](docs/notebooks/demo/demo.ipynb). -->
+For a more in-depth tutorial in interactive notebook format, see [demo.ipynb](https://github.com/Humboldt-Penguin/redplanet/blob/main/docs/notebooks/demo/demo.ipynb).
 
+&nbsp;
 
 ---
 
 # Links
 
 - Don't hesitate to reach out: [zain.eris.kamal@rutgers.edu](mailto:zain.eris.kamal@rutgers.edu)
-- Acknowledgements: [docs/thanks.txt](docs/thanks.txt)
-- References: [docs/references.txt](docs/references.txt)
+- Acknowledgements: [docs/thanks.txt](https://github.com/Humboldt-Penguin/redplanet/blob/main/docs/thanks.txt)
+- References: [docs/references.txt](https://github.com/Humboldt-Penguin/redplanet/blob/main/docs/references.txt)
 - Other work: [github.com/Humboldt-Penguin](https://github.com/Humboldt-Penguin)
```

