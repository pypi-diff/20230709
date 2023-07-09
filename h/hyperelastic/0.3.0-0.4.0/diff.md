# Comparing `tmp/hyperelastic-0.3.0.tar.gz` & `tmp/hyperelastic-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperelastic-0.3.0.tar", last modified: Tue Jul  4 09:06:04 2023, max compression
+gzip compressed data, was "hyperelastic-0.4.0.tar", last modified: Sun Jul  9 10:55:35 2023, max compression
```

## Comparing `hyperelastic-0.3.0.tar` & `hyperelastic-0.4.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:06:04.807304 hyperelastic-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    50329 2023-07-04 09:06:04.807304 hyperelastic-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 09:06:04.807304 hyperelastic-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:06:04.795304 hyperelastic-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:06:04.799304 hyperelastic-0.3.0/src/hyperelastic/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/src/hyperelastic/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/src/hyperelastic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:06:04.803304 hyperelastic-0.3.0/src/hyperelastic/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/src/hyperelastic/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/src/hyperelastic/frameworks/_invariants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/src/hyperelastic/frameworks/_stretches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:06:04.803304 hyperelastic-0.3.0/src/hyperelastic/math/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/src/hyperelastic/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/src/hyperelastic/math/_voigt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:06:04.803304 hyperelastic-0.3.0/src/hyperelastic/models/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/src/hyperelastic/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:06:04.803304 hyperelastic-0.3.0/src/hyperelastic/models/invariants/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/src/hyperelastic/models/invariants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/src/hyperelastic/models/invariants/_third_order_deformation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:06:04.803304 hyperelastic-0.3.0/src/hyperelastic/models/stretches/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/src/hyperelastic/models/stretches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/src/hyperelastic/models/stretches/_ogden.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:06:04.803304 hyperelastic-0.3.0/src/hyperelastic/spaces/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/src/hyperelastic/spaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/src/hyperelastic/spaces/_deformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/src/hyperelastic/spaces/_dilatational.py
--rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/src/hyperelastic/spaces/_distortional.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:06:04.799304 hyperelastic-0.3.0/src/hyperelastic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    50329 2023-07-04 09:06:04.000000 hyperelastic-0.3.0/src/hyperelastic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-04 09:06:04.000000 hyperelastic-0.3.0/src/hyperelastic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 09:06:04.000000 hyperelastic-0.3.0/src/hyperelastic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-04 09:06:04.000000 hyperelastic-0.3.0/src/hyperelastic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-04 09:06:04.000000 hyperelastic-0.3.0/src/hyperelastic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:06:04.807304 hyperelastic-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/tests/test_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-04 09:05:54.000000 hyperelastic-0.3.0/tests/test_sympy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:55:35.268506 hyperelastic-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-09 10:55:23.000000 hyperelastic-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    50628 2023-07-09 10:55:35.268506 hyperelastic-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-07-09 10:55:23.000000 hyperelastic-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-09 10:55:23.000000 hyperelastic-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 10:55:35.268506 hyperelastic-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:55:35.264506 hyperelastic-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:55:35.264506 hyperelastic-0.4.0/src/hyperelastic/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-09 10:55:23.000000 hyperelastic-0.4.0/src/hyperelastic/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-09 10:55:23.000000 hyperelastic-0.4.0/src/hyperelastic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:55:35.268506 hyperelastic-0.4.0/src/hyperelastic/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-09 10:55:23.000000 hyperelastic-0.4.0/src/hyperelastic/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-07-09 10:55:23.000000 hyperelastic-0.4.0/src/hyperelastic/frameworks/_invariants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-07-09 10:55:23.000000 hyperelastic-0.4.0/src/hyperelastic/frameworks/_stretches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:55:35.268506 hyperelastic-0.4.0/src/hyperelastic/math/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-09 10:55:23.000000 hyperelastic-0.4.0/src/hyperelastic/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23093 2023-07-09 10:55:23.000000 hyperelastic-0.4.0/src/hyperelastic/math/_voigt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:55:35.268506 hyperelastic-0.4.0/src/hyperelastic/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-09 10:55:23.000000 hyperelastic-0.4.0/src/hyperelastic/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:55:35.268506 hyperelastic-0.4.0/src/hyperelastic/models/invariants/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-09 10:55:23.000000 hyperelastic-0.4.0/src/hyperelastic/models/invariants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-07-09 10:55:23.000000 hyperelastic-0.4.0/src/hyperelastic/models/invariants/_third_order_deformation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:55:35.268506 hyperelastic-0.4.0/src/hyperelastic/models/stretches/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-09 10:55:23.000000 hyperelastic-0.4.0/src/hyperelastic/models/stretches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-09 10:55:23.000000 hyperelastic-0.4.0/src/hyperelastic/models/stretches/_ogden.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:55:35.268506 hyperelastic-0.4.0/src/hyperelastic/spaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-09 10:55:23.000000 hyperelastic-0.4.0/src/hyperelastic/spaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-07-09 10:55:23.000000 hyperelastic-0.4.0/src/hyperelastic/spaces/_deformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-09 10:55:23.000000 hyperelastic-0.4.0/src/hyperelastic/spaces/_dilatational.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-07-09 10:55:23.000000 hyperelastic-0.4.0/src/hyperelastic/spaces/_distortional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:55:35.268506 hyperelastic-0.4.0/src/hyperelastic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    50628 2023-07-09 10:55:35.000000 hyperelastic-0.4.0/src/hyperelastic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-09 10:55:35.000000 hyperelastic-0.4.0/src/hyperelastic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 10:55:35.000000 hyperelastic-0.4.0/src/hyperelastic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-09 10:55:35.000000 hyperelastic-0.4.0/src/hyperelastic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-09 10:55:35.000000 hyperelastic-0.4.0/src/hyperelastic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:55:35.268506 hyperelastic-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-09 10:55:23.000000 hyperelastic-0.4.0/tests/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-09 10:55:23.000000 hyperelastic-0.4.0/tests/test_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-09 10:55:23.000000 hyperelastic-0.4.0/tests/test_sympy.py
```

### Comparing `hyperelastic-0.3.0/LICENSE` & `hyperelastic-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.3.0/PKG-INFO` & `hyperelastic-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperelastic
-Version: 0.3.0
+Version: 0.4.0
 Summary: Constitutive hyperelastic material formulations for FElupe
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -704,15 +704,15 @@
 License-File: LICENSE
 
 <p align="center">
   <a href="https://github.com/adtzlr/hyperelastic"><img src="https://github.com/adtzlr/hyperelastic/assets/5793153/d875ecd0-a23f-4c11-87c4-0aa99297ab6d" height="160px"/></a>
   <p align="center">Constitutive <b>hyperelastic</b> material formulations for <a href="https://github.com/adtzlr/felupe">FElupe</a>.</p>
 </p>
 
-[![PyPI version shields.io](https://img.shields.io/pypi/v/hyperelastic.svg)](https://pypi.python.org/pypi/hyperelastic/) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Made with love in Graz (Austria)](https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20in-Graz%20(Austria)-0c674a) [![codecov](https://codecov.io/gh/adtzlr/hyperelastic/branch/main/graph/badge.svg)](https://codecov.io/gh/adtzlr/hyperelastic) [![DOI](https://zenodo.org/badge/656860854.svg)](https://zenodo.org/badge/latestdoi/656860854) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black)
+[![PyPI version shields.io](https://img.shields.io/pypi/v/hyperelastic.svg)](https://pypi.python.org/pypi/hyperelastic/) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Made with love in Graz (Austria)](https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20in-Graz%20(Austria)-0c674a) [![codecov](https://codecov.io/gh/adtzlr/hyperelastic/branch/main/graph/badge.svg)](https://codecov.io/gh/adtzlr/hyperelastic) [![DOI](https://zenodo.org/badge/656860854.svg)](https://zenodo.org/badge/latestdoi/656860854) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black) [![Documentation Status](https://readthedocs.org/projects/hyperelastic/badge/?version=latest)](https://hyperelastic.readthedocs.io/en/latest/?badge=latest) [![PDF Documentation](https://img.shields.io/badge/PDF%20Documentation-8A2BE2)](https://hyperelastic.readthedocs.io/_/downloads/en/latest/pdf/)
 
 This package provides the essential building blocks for constitutive hyperelastic material formulations. This includes material behaviour-independent spaces and frameworks as well as material behaviour-dependent model formulations.
 
 **Spaces** ([`hyperelastic.spaces`](https://github.com/adtzlr/hyperelastic/tree/main/src/hyperelastic/spaces)) are full or partial deformations on which a given material formulation should be projected to, e.g. to the distortional (part of the deformation) space. Generalized *Total-Lagrange* **Frameworks** ([`hyperelastic.frameworks`](https://github.com/adtzlr/hyperelastic/tree/main/src/hyperelastic/frameworks)) for isotropic hyperelastic material formulations based on the invariants of the right Cauchy-Green deformation tensor and the principal stretches enable a clean coding of isotropic material formulations.
 
 The [`hyperelastic.math`](https://github.com/adtzlr/hyperelastic/tree/main/src/hyperelastic/math)-module provides helpers in reduced vector ([Voigt](https://en.wikipedia.org/wiki/Voigt_notation)) storage for symmetric three-dimensional second-order tensors along with a matrix storage for (at least minor) symmetric three-dimensional fourth-order tensors. Shear terms are not doubled for strain-like tensors, instead all math operations take care of the reduced vector storage.
 
@@ -779,15 +779,14 @@
 ```
 
 ### Available isotropic hyperelastic invariant-based material formulations
 The typical polynomial-based material formulations ([Neo-Hooke](https://en.wikipedia.org/wiki/Neo-Hookean_solid), [Mooney-Rivlin](https://en.wikipedia.org/wiki/Mooney%E2%80%93Rivlin_solid), [Yeoh](https://en.wikipedia.org/wiki/Yeoh_hyperelastic_model) are all available as submodels of the third order deformation material formulation.
 
 - [Third-Order-Deformation (James-Green-Simpson)](https://onlinelibrary.wiley.com/doi/abs/10.1002/app.1975.070190723) ([code](https://github.com/adtzlr/hyperelastic/blob/main/src/hyperelastic/models/invariants/_third_order_deformation.py))
 
-
 ## Principal stretch-based material formulations
 A minimal template for a principal stretch-based material formulation applied on the distortional space:
 
 ```python
 class MyStretchesModel:
     def gradient(self, λ, statevars):
         """The gradient as the partial derivative of the strain energy function w.r.t.
```

### Comparing `hyperelastic-0.3.0/README.md` & `hyperelastic-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <p align="center">
   <a href="https://github.com/adtzlr/hyperelastic"><img src="https://github.com/adtzlr/hyperelastic/assets/5793153/d875ecd0-a23f-4c11-87c4-0aa99297ab6d" height="160px"/></a>
   <p align="center">Constitutive <b>hyperelastic</b> material formulations for <a href="https://github.com/adtzlr/felupe">FElupe</a>.</p>
 </p>
 
-[![PyPI version shields.io](https://img.shields.io/pypi/v/hyperelastic.svg)](https://pypi.python.org/pypi/hyperelastic/) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Made with love in Graz (Austria)](https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20in-Graz%20(Austria)-0c674a) [![codecov](https://codecov.io/gh/adtzlr/hyperelastic/branch/main/graph/badge.svg)](https://codecov.io/gh/adtzlr/hyperelastic) [![DOI](https://zenodo.org/badge/656860854.svg)](https://zenodo.org/badge/latestdoi/656860854) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black)
+[![PyPI version shields.io](https://img.shields.io/pypi/v/hyperelastic.svg)](https://pypi.python.org/pypi/hyperelastic/) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Made with love in Graz (Austria)](https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20in-Graz%20(Austria)-0c674a) [![codecov](https://codecov.io/gh/adtzlr/hyperelastic/branch/main/graph/badge.svg)](https://codecov.io/gh/adtzlr/hyperelastic) [![DOI](https://zenodo.org/badge/656860854.svg)](https://zenodo.org/badge/latestdoi/656860854) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black) [![Documentation Status](https://readthedocs.org/projects/hyperelastic/badge/?version=latest)](https://hyperelastic.readthedocs.io/en/latest/?badge=latest) [![PDF Documentation](https://img.shields.io/badge/PDF%20Documentation-8A2BE2)](https://hyperelastic.readthedocs.io/_/downloads/en/latest/pdf/)
 
 This package provides the essential building blocks for constitutive hyperelastic material formulations. This includes material behaviour-independent spaces and frameworks as well as material behaviour-dependent model formulations.
 
 **Spaces** ([`hyperelastic.spaces`](https://github.com/adtzlr/hyperelastic/tree/main/src/hyperelastic/spaces)) are full or partial deformations on which a given material formulation should be projected to, e.g. to the distortional (part of the deformation) space. Generalized *Total-Lagrange* **Frameworks** ([`hyperelastic.frameworks`](https://github.com/adtzlr/hyperelastic/tree/main/src/hyperelastic/frameworks)) for isotropic hyperelastic material formulations based on the invariants of the right Cauchy-Green deformation tensor and the principal stretches enable a clean coding of isotropic material formulations.
 
 The [`hyperelastic.math`](https://github.com/adtzlr/hyperelastic/tree/main/src/hyperelastic/math)-module provides helpers in reduced vector ([Voigt](https://en.wikipedia.org/wiki/Voigt_notation)) storage for symmetric three-dimensional second-order tensors along with a matrix storage for (at least minor) symmetric three-dimensional fourth-order tensors. Shear terms are not doubled for strain-like tensors, instead all math operations take care of the reduced vector storage.
 
@@ -74,15 +74,14 @@
 ```
 
 ### Available isotropic hyperelastic invariant-based material formulations
 The typical polynomial-based material formulations ([Neo-Hooke](https://en.wikipedia.org/wiki/Neo-Hookean_solid), [Mooney-Rivlin](https://en.wikipedia.org/wiki/Mooney%E2%80%93Rivlin_solid), [Yeoh](https://en.wikipedia.org/wiki/Yeoh_hyperelastic_model) are all available as submodels of the third order deformation material formulation.
 
 - [Third-Order-Deformation (James-Green-Simpson)](https://onlinelibrary.wiley.com/doi/abs/10.1002/app.1975.070190723) ([code](https://github.com/adtzlr/hyperelastic/blob/main/src/hyperelastic/models/invariants/_third_order_deformation.py))
 
-
 ## Principal stretch-based material formulations
 A minimal template for a principal stretch-based material formulation applied on the distortional space:
 
 ```python
 class MyStretchesModel:
     def gradient(self, λ, statevars):
         """The gradient as the partial derivative of the strain energy function w.r.t.
```

### Comparing `hyperelastic-0.3.0/pyproject.toml` & `hyperelastic-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.3.0/src/hyperelastic/__init__.py` & `hyperelastic-0.4.0/src/hyperelastic/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.3.0/src/hyperelastic/frameworks/_invariants.py` & `hyperelastic-0.4.0/src/hyperelastic/frameworks/_invariants.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,16 @@
             \frac{\partial I_3}{\partial \boldsymbol{C}}
 
     Furthermore, the second partial derivatives of the elasticity tensor are carried
     out.
 
     ..  math::
 
-        \mathbb{C} &= \frac{\partial^2 \psi}{\partial I_1~\partial I_1}
+        \frac{\partial^2 \psi}{\partial \boldsymbol{C}~\partial \boldsymbol{C}} &=
+            \frac{\partial^2 \psi}{\partial I_1~\partial I_1}
             \left( \frac{\partial I_1}{\partial \boldsymbol{C}} \otimes
             \frac{\partial I_1}{\partial \boldsymbol{C}} \right)
 
             &+ \frac{\partial^2 \psi}{\partial I_2~\partial I_2}
             \left( \frac{\partial I_2}{\partial \boldsymbol{C}} \otimes
             \frac{\partial I_2}{\partial \boldsymbol{C}} \right)
 
@@ -120,15 +121,15 @@
 
     The only non material behaviour-related terms which are not already defined during
     stress evaluation are the second partial derivatives of the invariants w.r.t.
     the right Cauchy-Green deformation tensor.
 
     ..  math::
 
-        \frac{\partial^2 I_12}{\partial \boldsymbol{C}~\partial \boldsymbol{C}} &=
+        \frac{\partial^2 I_1}{\partial \boldsymbol{C}~\partial \boldsymbol{C}} &=
             \mathbb{0}
 
         \frac{\partial^2 I_2}{\partial \boldsymbol{C}~\partial \boldsymbol{C}} &=
             \boldsymbol{I} \otimes \boldsymbol{I} - \boldsymbol{I} \odot \boldsymbol{I}
 
         \frac{\partial^2 I_3}{\partial \boldsymbol{C}~\partial \boldsymbol{C}} &=
             I_3 \left( \boldsymbol{C}^{-1} \otimes \boldsymbol{C}^{-1}
```

### Comparing `hyperelastic-0.3.0/src/hyperelastic/frameworks/_stretches.py` & `hyperelastic-0.4.0/src/hyperelastic/frameworks/_stretches.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     The first partial derivative of the strain energy function w.r.t. a principal
     stretch
 
     ..  math::
 
         \psi_{,\alpha} = \frac{\partial \psi}{\partial \lambda_\alpha}
 
-    and the partial derivative of a principal strech w.r.t. the right Cauchy-Green
+    and the partial derivative of a principal stretch w.r.t. the right Cauchy-Green
     deformation tensor is defined
 
     ..  math::
 
         \frac{\partial \lambda_\alpha}{\partial \boldsymbol{C}} =
             \frac{\partial (\lambda^2_\alpha)^{1/2}}{\partial \boldsymbol{C}} =
             \frac{1}{2 \lambda_\alpha} \boldsymbol{M}_\alpha
@@ -174,12 +174,10 @@
                 v = λ[α] ** 2 - λ[β] ** 2
                 mask = np.isclose(v, 0)
 
                 f = np.zeros_like(v)
                 f[~mask] = (dWdλC[α][~mask] - dWdλC[β][~mask]) / v[~mask]
                 f[mask] = d2WdλC2[β][mask] - d2WdλC2[m][mask]
 
-                d2WdCdC += d2WdλC2[m] * transpose(M4) + f * (
-                    cdya(M[α], M[β]) + cdya(M[β], M[α])
-                )
+                d2WdCdC += d2WdλC2[m] * transpose(M4) + f * 2 * cdya(M[α], M[β])
 
         return d2WdCdC
```

### Comparing `hyperelastic-0.3.0/src/hyperelastic/models/stretches/_ogden.py` & `hyperelastic-0.4.0/src/hyperelastic/models/stretches/_ogden.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.3.0/src/hyperelastic/spaces/_deformation.py` & `hyperelastic-0.4.0/src/hyperelastic/spaces/_deformation.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,33 @@
     r"""The deformation space.
 
     This class takes a Total-Lagrange material formulation and applies it on the
     deformation space.
 
     ..  math::
 
-        psi = \psi(\boldsymbol{F})
+        \psi = \psi(\boldsymbol{C}(\boldsymbol{F}))
+
+    The gradient of the strain energy function is carried out w.r.t. the Green Lagrange
+    strain tensor. Hence, the work-conjugate stress tensor here refers to the second
+    Piola-Kirchhoff stress tensor.
+
+    ..  math::
+
+        \boldsymbol{S} = \frac{\partial \psi}{\partial \frac{1}{2}\boldsymbol{C}}
+
+    The hessian of the strain energy function is carried out w.r.t. the Green-Lagrange
+    strain tensor. Hence, the work-conjugate elasticity tensor here refers to the
+    fourth-order Total-Lagrangian elasticity tensor.
+
+    ..  math::
+
+        \mathbb{C} = \frac{\partial^2 \psi}{\partial \frac{1}{2}\boldsymbol{C}~
+            \frac{1}{2}\boldsymbol{C}}
+
 
     Given a Total-Lagrange material formulation, for the variation and linearization of
     the virtual work of internal forces, the output quantities have to be transformed:
     The second Piola-Kirchhoff stress tensor is converted into the deformation gradient
     work-conjugate first Piola-Kirchhoff stress tensor, along with its fourth-order
     elasticity tensor. Also, the so-called geometric tangent stiffness component
     (initial stress matrix) is added to the fourth-order elasticity tensor.
```

### Comparing `hyperelastic-0.3.0/src/hyperelastic/spaces/_dilatational.py` & `hyperelastic-0.4.0/src/hyperelastic/spaces/_dilatational.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.3.0/src/hyperelastic/spaces/_distortional.py` & `hyperelastic-0.4.0/src/hyperelastic/spaces/_distortional.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import numpy as np
 
 from ..math import astensor, asvoigt, cdya, cdya_ik, ddot, det, dya, eye, inv, transpose
 
 
 class Distortional:
     r"""The distortional (part of the deformation) space is a partial deformation with
-    constant volume. For a given deformation map :math:`x(X)` and its deformation
-    gradient :math:`\boldsymbol{F}`, the distortional part of the deformation gradient
-    :math:`\hat{\boldsymbol{F}}` is obtained by a multiplicative (consecutive) split
-    into a volume-changing (dilatational) and a constant-volume (distortional) part of
-    the deformation gradient. Due to the fact that the dilatational part is proportional
-    to the unit tensor, the order of these partial deformations is not unique.
+    constant volume. For a given deformation map :math:`\boldsymbol{x}(\boldsymbol{x})`
+    and its deformation gradient :math:`\boldsymbol{F}`, the distortional part of the
+    deformation gradient :math:`\hat{\boldsymbol{F}}` is obtained by a multiplicative
+    (consecutive) split into a volume-changing (dilatational) and a constant-volume
+    (distortional) part of the deformation gradient. Due to the fact that the
+    dilatational part is proportional to the unit tensor, the order of these partial
+    deformations is not unique.
 
     ..  math::
 
         \boldsymbol{F} = \overset{\circ}{\boldsymbol{F}} \hat{\boldsymbol{F}} =
             \hat{\boldsymbol{F}} \overset{\circ}{\boldsymbol{F}}
 
     This class takes a Total-Lagrange material formulation and applies it only on the
@@ -83,15 +84,15 @@
     ..  math::
 
         \boldsymbol{S}' = \bar{\boldsymbol{S}}
             - \frac{\bar{\boldsymbol{S}}:\boldsymbol{C}}{3} \boldsymbol{C}^{-1}
             = \text{dev}(\bar{\boldsymbol{S}} \boldsymbol{C}) \boldsymbol{C}^{-1}
 
     The hessian of the strain energy function is carried out w.r.t. the Green-Lagrange
-    strain tensor. Hence, the work-conjugate stress tensor used in this space
+    strain tensor. Hence, the work-conjugate elasticity tensor used in this space
     projection refers to the fourth-order Total-Lagrangian elasticity tensor.
 
     ..  math::
 
         \mathbb{C}' = \frac{\partial^2 \hat{\psi}}{\partial \frac{1}{2}\boldsymbol{C}~
             \frac{1}{2}\boldsymbol{C}}
```

### Comparing `hyperelastic-0.3.0/src/hyperelastic.egg-info/PKG-INFO` & `hyperelastic-0.4.0/src/hyperelastic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperelastic
-Version: 0.3.0
+Version: 0.4.0
 Summary: Constitutive hyperelastic material formulations for FElupe
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -704,15 +704,15 @@
 License-File: LICENSE
 
 <p align="center">
   <a href="https://github.com/adtzlr/hyperelastic"><img src="https://github.com/adtzlr/hyperelastic/assets/5793153/d875ecd0-a23f-4c11-87c4-0aa99297ab6d" height="160px"/></a>
   <p align="center">Constitutive <b>hyperelastic</b> material formulations for <a href="https://github.com/adtzlr/felupe">FElupe</a>.</p>
 </p>
 
-[![PyPI version shields.io](https://img.shields.io/pypi/v/hyperelastic.svg)](https://pypi.python.org/pypi/hyperelastic/) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Made with love in Graz (Austria)](https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20in-Graz%20(Austria)-0c674a) [![codecov](https://codecov.io/gh/adtzlr/hyperelastic/branch/main/graph/badge.svg)](https://codecov.io/gh/adtzlr/hyperelastic) [![DOI](https://zenodo.org/badge/656860854.svg)](https://zenodo.org/badge/latestdoi/656860854) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black)
+[![PyPI version shields.io](https://img.shields.io/pypi/v/hyperelastic.svg)](https://pypi.python.org/pypi/hyperelastic/) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Made with love in Graz (Austria)](https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20in-Graz%20(Austria)-0c674a) [![codecov](https://codecov.io/gh/adtzlr/hyperelastic/branch/main/graph/badge.svg)](https://codecov.io/gh/adtzlr/hyperelastic) [![DOI](https://zenodo.org/badge/656860854.svg)](https://zenodo.org/badge/latestdoi/656860854) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black) [![Documentation Status](https://readthedocs.org/projects/hyperelastic/badge/?version=latest)](https://hyperelastic.readthedocs.io/en/latest/?badge=latest) [![PDF Documentation](https://img.shields.io/badge/PDF%20Documentation-8A2BE2)](https://hyperelastic.readthedocs.io/_/downloads/en/latest/pdf/)
 
 This package provides the essential building blocks for constitutive hyperelastic material formulations. This includes material behaviour-independent spaces and frameworks as well as material behaviour-dependent model formulations.
 
 **Spaces** ([`hyperelastic.spaces`](https://github.com/adtzlr/hyperelastic/tree/main/src/hyperelastic/spaces)) are full or partial deformations on which a given material formulation should be projected to, e.g. to the distortional (part of the deformation) space. Generalized *Total-Lagrange* **Frameworks** ([`hyperelastic.frameworks`](https://github.com/adtzlr/hyperelastic/tree/main/src/hyperelastic/frameworks)) for isotropic hyperelastic material formulations based on the invariants of the right Cauchy-Green deformation tensor and the principal stretches enable a clean coding of isotropic material formulations.
 
 The [`hyperelastic.math`](https://github.com/adtzlr/hyperelastic/tree/main/src/hyperelastic/math)-module provides helpers in reduced vector ([Voigt](https://en.wikipedia.org/wiki/Voigt_notation)) storage for symmetric three-dimensional second-order tensors along with a matrix storage for (at least minor) symmetric three-dimensional fourth-order tensors. Shear terms are not doubled for strain-like tensors, instead all math operations take care of the reduced vector storage.
 
@@ -779,15 +779,14 @@
 ```
 
 ### Available isotropic hyperelastic invariant-based material formulations
 The typical polynomial-based material formulations ([Neo-Hooke](https://en.wikipedia.org/wiki/Neo-Hookean_solid), [Mooney-Rivlin](https://en.wikipedia.org/wiki/Mooney%E2%80%93Rivlin_solid), [Yeoh](https://en.wikipedia.org/wiki/Yeoh_hyperelastic_model) are all available as submodels of the third order deformation material formulation.
 
 - [Third-Order-Deformation (James-Green-Simpson)](https://onlinelibrary.wiley.com/doi/abs/10.1002/app.1975.070190723) ([code](https://github.com/adtzlr/hyperelastic/blob/main/src/hyperelastic/models/invariants/_third_order_deformation.py))
 
-
 ## Principal stretch-based material formulations
 A minimal template for a principal stretch-based material formulation applied on the distortional space:
 
 ```python
 class MyStretchesModel:
     def gradient(self, λ, statevars):
         """The gradient as the partial derivative of the strain energy function w.r.t.
```

### Comparing `hyperelastic-0.3.0/src/hyperelastic.egg-info/SOURCES.txt` & `hyperelastic-0.4.0/src/hyperelastic.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -18,9 +18,10 @@
 src/hyperelastic/models/invariants/_third_order_deformation.py
 src/hyperelastic/models/stretches/__init__.py
 src/hyperelastic/models/stretches/_ogden.py
 src/hyperelastic/spaces/__init__.py
 src/hyperelastic/spaces/_deformation.py
 src/hyperelastic/spaces/_dilatational.py
 src/hyperelastic/spaces/_distortional.py
+tests/test_math.py
 tests/test_space.py
 tests/test_sympy.py
```

### Comparing `hyperelastic-0.3.0/tests/test_space.py` & `hyperelastic-0.4.0/tests/test_space.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.3.0/tests/test_sympy.py` & `hyperelastic-0.4.0/tests/test_sympy.py`

 * *Files identical despite different names*

