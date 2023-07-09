# Comparing `tmp/astropandas-1.2.1.tar.gz` & `tmp/astropandas-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astropandas-1.2.1.tar", last modified: Tue Jul  4 09:32:36 2023, max compression
+gzip compressed data, was "astropandas-1.2.2.tar", last modified: Sun Jul  9 13:12:54 2023, max compression
```

## Comparing `astropandas-1.2.1.tar` & `astropandas-1.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:32:36.024808 astropandas-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-04 09:32:21.000000 astropandas-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-04 09:32:36.024808 astropandas-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-04 09:32:21.000000 astropandas-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:32:36.024808 astropandas-1.2.1/astropandas/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-04 09:32:21.000000 astropandas-1.2.1/astropandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-07-04 09:32:21.000000 astropandas-1.2.1/astropandas/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    16090 2023-07-04 09:32:21.000000 astropandas-1.2.1/astropandas/match.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:32:36.024808 astropandas-1.2.1/astropandas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-04 09:32:36.000000 astropandas-1.2.1/astropandas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-04 09:32:36.000000 astropandas-1.2.1/astropandas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 09:32:36.000000 astropandas-1.2.1/astropandas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-04 09:32:36.000000 astropandas-1.2.1/astropandas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-04 09:32:36.000000 astropandas-1.2.1/astropandas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-04 09:32:21.000000 astropandas-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-04 09:32:36.028807 astropandas-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-04 09:32:21.000000 astropandas-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:12:54.059323 astropandas-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-09 13:12:42.000000 astropandas-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-09 13:12:54.059323 astropandas-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-09 13:12:42.000000 astropandas-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:12:54.059323 astropandas-1.2.2/astropandas/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-09 13:12:42.000000 astropandas-1.2.2/astropandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-07-09 13:12:42.000000 astropandas-1.2.2/astropandas/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16189 2023-07-09 13:12:42.000000 astropandas-1.2.2/astropandas/match.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:12:54.059323 astropandas-1.2.2/astropandas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-09 13:12:54.000000 astropandas-1.2.2/astropandas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-09 13:12:54.000000 astropandas-1.2.2/astropandas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 13:12:54.000000 astropandas-1.2.2/astropandas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-09 13:12:54.000000 astropandas-1.2.2/astropandas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-09 13:12:54.000000 astropandas-1.2.2/astropandas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-09 13:12:42.000000 astropandas-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 13:12:54.059323 astropandas-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-09 13:12:42.000000 astropandas-1.2.2/setup.py
```

### Comparing `astropandas-1.2.1/LICENSE` & `astropandas-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `astropandas-1.2.1/PKG-INFO` & `astropandas-1.2.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,35 @@
 Metadata-Version: 2.1
 Name: astropandas
-Version: 1.2.1
+Version: 1.2.2
 Summary: Tools to expand on pandas functionality for astronomical operations.
-Author: Jan Luca van den Busch
-License: GPLv3
+Home-page: https://github.com/jlvdb/astropandas
+Author-email: Jan Luca van den Busch <jlvdb@astro.ruhr-uni-bochum.de>
+License: GPL-3.0-or-later
 Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: plot
 License-File: LICENSE
 
 # astropandas
 
 Tools to expand on pandas functionality for astronomical applications.
+The code is publically hosted on github:
+
+https://github.com/jlvdb/yet_another_wizz.git
+
+## Installation
+
+The yet_another_wizz package can be installed directly with pip::
+
+    pip install astropandas
 
 ## Features
 
 - directly read and write FITS table data, see `astropandas.read_fits` and `astropandas.to_fits`
 - match based on sky coordinates, see `astropandas.match`
 
 ## Examples
```

### Comparing `astropandas-1.2.1/README.md` & `astropandas-1.2.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 # astropandas
 
 Tools to expand on pandas functionality for astronomical applications.
+The code is publically hosted on github:
+
+https://github.com/jlvdb/yet_another_wizz.git
+
+## Installation
+
+The yet_another_wizz package can be installed directly with pip::
+
+    pip install astropandas
 
 ## Features
 
 - directly read and write FITS table data, see `astropandas.read_fits` and `astropandas.to_fits`
 - match based on sky coordinates, see `astropandas.match`
 
 ## Examples
```

### Comparing `astropandas-1.2.1/astropandas/io.py` & `astropandas-1.2.2/astropandas/io.py`

 * *Files identical despite different names*

### Comparing `astropandas-1.2.1/astropandas/match.py` & `astropandas-1.2.2/astropandas/match.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import warnings
 
-import matplotlib.patches
-import matplotlib.pyplot as plt
 import numpy as np
 import scipy.spatial
 
 
 class SphericalKDTree(object):
     """
     SphericalKDTree(ra, dec, leaf_size=16)
@@ -193,14 +191,16 @@
     def offset(self):
         return np.nanmean(self.distances, axis=0)
 
     def scatter(self):
         return np.nanstd(self.distances, axis=0)
 
     def plot_threshold(self, ax=None):
+        import matplotlib.pyplot as plt
+
         if ax is None:
             ax = plt.gca()
         ax.plot(self.separations * 3600.0, self.counts)
         if np.isfinite(self.threshold):
             thresh = self.threshold * 3600.0
             ax.axvline(thresh, color="k")
             ax.annotate(
@@ -208,14 +208,17 @@
                 xy=(thresh, np.mean(ax.get_ylim())),
                 xycoords="data", va="center", ha="right", rotation=90)
         ax.grid(alpha=0.3)
         ax.set_xlabel("Point separation / arcsec")
         ax.set_ylabel("Frequency")
 
     def plot_offset(self, ax=None, sigmas=3, aspect=False):
+        import matplotlib.patches
+        import matplotlib.pyplot as plt
+
         mask = np.isfinite(self.distances).all(axis=1)
         delta_ra, delta_dec = np.transpose(self.distances[mask] * 3600.0)
         offset = self.offset() * 3600.0
         scatter = self.scatter() * 3600.0
         ax_range = sigmas * max(scatter)
         # make the plot
         if ax is None:
@@ -238,14 +241,16 @@
         ax.set_ylim(-ax_range, ax_range)
         if aspect:
             ax.set_aspect("equal")
         ax.set_xlabel(r"$\Delta$RA / arcsec")
         ax.set_ylabel(r"$\Delta$DEC / arcsec")
 
     def plot(self):
+        import matplotlib.pyplot as plt
+
         fig, (axt, axo) = plt.subplots(1, 2, figsize=(12, 4))
         self.plot_threshold(axt)
         self.plot_offset(axo, aspect=True)
         fig.tight_layout()
 
 
 class Matcher:
```

### Comparing `astropandas-1.2.1/astropandas.egg-info/PKG-INFO` & `astropandas-1.2.2/astropandas.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,35 @@
 Metadata-Version: 2.1
 Name: astropandas
-Version: 1.2.1
+Version: 1.2.2
 Summary: Tools to expand on pandas functionality for astronomical operations.
-Author: Jan Luca van den Busch
-License: GPLv3
+Home-page: https://github.com/jlvdb/astropandas
+Author-email: Jan Luca van den Busch <jlvdb@astro.ruhr-uni-bochum.de>
+License: GPL-3.0-or-later
 Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: plot
 License-File: LICENSE
 
 # astropandas
 
 Tools to expand on pandas functionality for astronomical applications.
+The code is publically hosted on github:
+
+https://github.com/jlvdb/yet_another_wizz.git
+
+## Installation
+
+The yet_another_wizz package can be installed directly with pip::
+
+    pip install astropandas
 
 ## Features
 
 - directly read and write FITS table data, see `astropandas.read_fits` and `astropandas.to_fits`
 - match based on sky coordinates, see `astropandas.match`
 
 ## Examples
```

