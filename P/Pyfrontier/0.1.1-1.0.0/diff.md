# Comparing `tmp/Pyfrontier-0.1.1.tar.gz` & `tmp/Pyfrontier-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pyfrontier-0.1.1.tar", last modified: Sun Sep 11 04:49:19 2022, max compression
+gzip compressed data, was "Pyfrontier-1.0.0.tar", last modified: Sun Jul  9 12:53:24 2023, max compression
```

## Comparing `Pyfrontier-0.1.1.tar` & `Pyfrontier-1.0.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 morinibu   (501) staff       (20)        0 2022-09-11 04:49:19.273518 Pyfrontier-0.1.1/
--rw-r--r--   0 morinibu   (501) staff       (20)     1065 2022-07-03 08:51:57.000000 Pyfrontier-0.1.1/LICENSE
--rw-r--r--   0 morinibu   (501) staff       (20)     2560 2022-09-11 04:49:19.273742 Pyfrontier-0.1.1/PKG-INFO
--rwxrwxrwx   0 morinibu   (501) staff       (20)     1654 2022-09-11 03:15:04.000000 Pyfrontier-0.1.1/README.md
--rw-r--r--   0 morinibu   (501) staff       (20)      101 2022-09-03 03:56:55.000000 Pyfrontier-0.1.1/pyproject.toml
--rwxrwxrwx   0 morinibu   (501) staff       (20)       73 2022-09-11 04:49:19.274459 Pyfrontier-0.1.1/setup.cfg
--rwxrwxrwx   0 morinibu   (501) staff       (20)     1785 2022-09-11 01:46:46.000000 Pyfrontier-0.1.1/setup.py
-drwxr-xr-x   0 morinibu   (501) staff       (20)        0 2022-09-11 04:49:19.257984 Pyfrontier-0.1.1/src/
-drwxr-xr-x   0 morinibu   (501) staff       (20)        0 2022-09-11 04:49:19.260723 Pyfrontier-0.1.1/src/Pyfrontier/
--rwxrwxrwx   0 morinibu   (501) staff       (20)       22 2022-09-10 11:40:40.000000 Pyfrontier-0.1.1/src/Pyfrontier/__init__.py
-drwxr-xr-x   0 morinibu   (501) staff       (20)        0 2022-09-11 04:49:19.267097 Pyfrontier-0.1.1/src/Pyfrontier/domain/
--rw-r--r--   0 morinibu   (501) staff       (20)      394 2022-08-11 05:33:06.000000 Pyfrontier-0.1.1/src/Pyfrontier/domain/__init__.py
--rw-r--r--   0 morinibu   (501) staff       (20)      300 2022-08-07 01:54:52.000000 Pyfrontier-0.1.1/src/Pyfrontier/domain/assurance_region.py
--rw-r--r--   0 morinibu   (501) staff       (20)      800 2022-07-31 05:00:20.000000 Pyfrontier-0.1.1/src/Pyfrontier/domain/dmu.py
--rw-r--r--   0 morinibu   (501) staff       (20)        0 2022-07-30 13:18:39.000000 Pyfrontier-0.1.1/src/Pyfrontier/domain/metrics.py
--rw-r--r--   0 morinibu   (501) staff       (20)     1749 2022-09-10 07:49:12.000000 Pyfrontier-0.1.1/src/Pyfrontier/domain/result.py
--rw-r--r--   0 morinibu   (501) staff       (20)      943 2022-08-11 05:33:06.000000 Pyfrontier-0.1.1/src/Pyfrontier/domain/slack_weight.py
-drwxr-xr-x   0 morinibu   (501) staff       (20)        0 2022-09-11 04:49:19.270287 Pyfrontier-0.1.1/src/Pyfrontier/frontier_model/
--rw-r--r--   0 morinibu   (501) staff       (20)      274 2022-08-11 05:33:06.000000 Pyfrontier-0.1.1/src/Pyfrontier/frontier_model/__init__.py
--rw-r--r--   0 morinibu   (501) staff       (20)     1692 2022-09-10 07:52:25.000000 Pyfrontier-0.1.1/src/Pyfrontier/frontier_model/_additive_dea.py
--rw-r--r--   0 morinibu   (501) staff       (20)      684 2022-08-07 04:47:01.000000 Pyfrontier-0.1.1/src/Pyfrontier/frontier_model/_base.py
--rw-r--r--   0 morinibu   (501) staff       (20)     5985 2022-09-10 07:49:12.000000 Pyfrontier-0.1.1/src/Pyfrontier/frontier_model/_dea.py
--rw-r--r--   0 morinibu   (501) staff       (20)      733 2022-08-07 05:04:34.000000 Pyfrontier-0.1.1/src/Pyfrontier/frontier_model/_hierarchical_dea.py
-drwxr-xr-x   0 morinibu   (501) staff       (20)        0 2022-09-11 04:49:19.273066 Pyfrontier-0.1.1/src/Pyfrontier/solver/
--rw-r--r--   0 morinibu   (501) staff       (20)      252 2022-08-11 05:33:06.000000 Pyfrontier-0.1.1/src/Pyfrontier/solver/__init__.py
--rw-r--r--   0 morinibu   (501) staff       (20)     2581 2022-09-03 03:56:55.000000 Pyfrontier-0.1.1/src/Pyfrontier/solver/_additive_solver.py
--rw-r--r--   0 morinibu   (501) staff       (20)      789 2022-08-06 02:21:59.000000 Pyfrontier-0.1.1/src/Pyfrontier/solver/_base.py
--rw-r--r--   0 morinibu   (501) staff       (20)     6982 2022-09-03 02:24:13.000000 Pyfrontier-0.1.1/src/Pyfrontier/solver/_envelope_solver.py
--rw-r--r--   0 morinibu   (501) staff       (20)     4409 2022-08-07 01:54:52.000000 Pyfrontier-0.1.1/src/Pyfrontier/solver/_multiple_solver.py
-drwxr-xr-x   0 morinibu   (501) staff       (20)        0 2022-09-11 04:49:19.263085 Pyfrontier-0.1.1/src/Pyfrontier.egg-info/
--rw-r--r--   0 morinibu   (501) staff       (20)     2560 2022-09-11 04:49:19.000000 Pyfrontier-0.1.1/src/Pyfrontier.egg-info/PKG-INFO
--rw-r--r--   0 morinibu   (501) staff       (20)      920 2022-09-11 04:49:19.000000 Pyfrontier-0.1.1/src/Pyfrontier.egg-info/SOURCES.txt
--rw-r--r--   0 morinibu   (501) staff       (20)        1 2022-09-11 04:49:19.000000 Pyfrontier-0.1.1/src/Pyfrontier.egg-info/dependency_links.txt
--rw-r--r--   0 morinibu   (501) staff       (20)        0 2022-08-01 11:27:37.000000 Pyfrontier-0.1.1/src/Pyfrontier.egg-info/not-zip-safe
--rw-r--r--   0 morinibu   (501) staff       (20)       24 2022-09-11 04:49:19.000000 Pyfrontier-0.1.1/src/Pyfrontier.egg-info/requires.txt
--rw-r--r--   0 morinibu   (501) staff       (20)       11 2022-09-11 04:49:19.000000 Pyfrontier-0.1.1/src/Pyfrontier.egg-info/top_level.txt
+drwxr-xr-x   0 morinibu   (501) staff       (20)        0 2023-07-09 12:53:24.138852 Pyfrontier-1.0.0/
+-rw-r--r--   0 morinibu   (501) staff       (20)     1065 2022-07-03 08:51:57.000000 Pyfrontier-1.0.0/LICENSE
+-rw-r--r--   0 morinibu   (501) staff       (20)     2621 2023-07-09 12:53:24.139105 Pyfrontier-1.0.0/PKG-INFO
+-rwxrwxrwx   0 morinibu   (501) staff       (20)     1719 2023-07-09 12:20:00.000000 Pyfrontier-1.0.0/README.md
+-rw-r--r--   0 morinibu   (501) staff       (20)      101 2022-09-03 03:56:55.000000 Pyfrontier-1.0.0/pyproject.toml
+-rwxrwxrwx   0 morinibu   (501) staff       (20)       73 2023-07-09 12:53:24.140045 Pyfrontier-1.0.0/setup.cfg
+-rwxr-xr-x   0 morinibu   (501) staff       (20)     1783 2023-07-09 12:45:16.000000 Pyfrontier-1.0.0/setup.py
+drwxr-xr-x   0 morinibu   (501) staff       (20)        0 2023-07-09 12:53:24.113484 Pyfrontier-1.0.0/src/
+drwxr-xr-x   0 morinibu   (501) staff       (20)        0 2023-07-09 12:53:24.118303 Pyfrontier-1.0.0/src/Pyfrontier/
+-rwxrwxrwx   0 morinibu   (501) staff       (20)       22 2022-09-10 11:40:40.000000 Pyfrontier-1.0.0/src/Pyfrontier/__init__.py
+drwxr-xr-x   0 morinibu   (501) staff       (20)        0 2023-07-09 12:53:24.128516 Pyfrontier-1.0.0/src/Pyfrontier/domain/
+-rw-r--r--   0 morinibu   (501) staff       (20)      394 2022-08-11 05:33:06.000000 Pyfrontier-1.0.0/src/Pyfrontier/domain/__init__.py
+-rw-r--r--   0 morinibu   (501) staff       (20)      300 2022-08-07 01:54:52.000000 Pyfrontier-1.0.0/src/Pyfrontier/domain/assurance_region.py
+-rw-r--r--   0 morinibu   (501) staff       (20)      800 2023-07-09 12:45:21.000000 Pyfrontier-1.0.0/src/Pyfrontier/domain/dmu.py
+-rw-r--r--   0 morinibu   (501) staff       (20)        0 2022-07-30 13:18:39.000000 Pyfrontier-1.0.0/src/Pyfrontier/domain/metrics.py
+-rw-r--r--   0 morinibu   (501) staff       (20)     1749 2022-09-10 07:49:12.000000 Pyfrontier-1.0.0/src/Pyfrontier/domain/result.py
+-rw-r--r--   0 morinibu   (501) staff       (20)      943 2022-08-11 05:33:06.000000 Pyfrontier-1.0.0/src/Pyfrontier/domain/slack_weight.py
+drwxr-xr-x   0 morinibu   (501) staff       (20)        0 2023-07-09 12:53:24.133293 Pyfrontier-1.0.0/src/Pyfrontier/frontier_model/
+-rw-r--r--   0 morinibu   (501) staff       (20)      274 2022-08-11 05:33:06.000000 Pyfrontier-1.0.0/src/Pyfrontier/frontier_model/__init__.py
+-rw-r--r--   0 morinibu   (501) staff       (20)     1692 2022-09-10 07:52:25.000000 Pyfrontier-1.0.0/src/Pyfrontier/frontier_model/_additive_dea.py
+-rw-r--r--   0 morinibu   (501) staff       (20)      684 2022-08-07 04:47:01.000000 Pyfrontier-1.0.0/src/Pyfrontier/frontier_model/_base.py
+-rw-r--r--   0 morinibu   (501) staff       (20)     5985 2022-09-10 07:49:12.000000 Pyfrontier-1.0.0/src/Pyfrontier/frontier_model/_dea.py
+-rw-r--r--   0 morinibu   (501) staff       (20)      733 2022-08-07 05:04:34.000000 Pyfrontier-1.0.0/src/Pyfrontier/frontier_model/_hierarchical_dea.py
+drwxr-xr-x   0 morinibu   (501) staff       (20)        0 2023-07-09 12:53:24.138154 Pyfrontier-1.0.0/src/Pyfrontier/solver/
+-rw-r--r--   0 morinibu   (501) staff       (20)      252 2022-08-11 05:33:06.000000 Pyfrontier-1.0.0/src/Pyfrontier/solver/__init__.py
+-rw-r--r--   0 morinibu   (501) staff       (20)     2581 2022-09-03 03:56:55.000000 Pyfrontier-1.0.0/src/Pyfrontier/solver/_additive_solver.py
+-rw-r--r--   0 morinibu   (501) staff       (20)      789 2022-08-06 02:21:59.000000 Pyfrontier-1.0.0/src/Pyfrontier/solver/_base.py
+-rw-r--r--   0 morinibu   (501) staff       (20)     6982 2022-09-03 02:24:13.000000 Pyfrontier-1.0.0/src/Pyfrontier/solver/_envelope_solver.py
+-rw-r--r--   0 morinibu   (501) staff       (20)     4409 2022-08-07 01:54:52.000000 Pyfrontier-1.0.0/src/Pyfrontier/solver/_multiple_solver.py
+drwxr-xr-x   0 morinibu   (501) staff       (20)        0 2023-07-09 12:53:24.122672 Pyfrontier-1.0.0/src/Pyfrontier.egg-info/
+-rw-r--r--   0 morinibu   (501) staff       (20)     2621 2023-07-09 12:53:24.000000 Pyfrontier-1.0.0/src/Pyfrontier.egg-info/PKG-INFO
+-rw-r--r--   0 morinibu   (501) staff       (20)      920 2023-07-09 12:53:24.000000 Pyfrontier-1.0.0/src/Pyfrontier.egg-info/SOURCES.txt
+-rw-r--r--   0 morinibu   (501) staff       (20)        1 2023-07-09 12:53:24.000000 Pyfrontier-1.0.0/src/Pyfrontier.egg-info/dependency_links.txt
+-rw-r--r--   0 morinibu   (501) staff       (20)        0 2022-08-01 11:27:37.000000 Pyfrontier-1.0.0/src/Pyfrontier.egg-info/not-zip-safe
+-rw-r--r--   0 morinibu   (501) staff       (20)       24 2023-07-09 12:53:24.000000 Pyfrontier-1.0.0/src/Pyfrontier.egg-info/requires.txt
+-rw-r--r--   0 morinibu   (501) staff       (20)       11 2023-07-09 12:53:24.000000 Pyfrontier-1.0.0/src/Pyfrontier.egg-info/top_level.txt
```

### Comparing `Pyfrontier-0.1.1/LICENSE` & `Pyfrontier-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Pyfrontier-0.1.1/PKG-INFO` & `Pyfrontier-1.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pyfrontier
-Version: 0.1.1
+Version: 1.0.0
 Summary: Pyfrontier is a data envelopment analysis for Python user.
 Home-page: https://nibutake.github.io/PyDEA/index.html?
 Download-URL: https://github.com/NibuTake/PyDEA
 Author: Takeshi Morinibu
 Author-email: takeshi715tech@gmail.com
 License: MIT
 Classifier: Intended Audience :: Science/Research
@@ -19,45 +19,49 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Pyfrontier: A data envelopment analysis module
+
 <div align="center"><img src="./images/logo.png" height="200"/></div>
 
-[![Python](https://img.shields.io/badge/Python-3.8%20%7C%203.9-blue)](https://codecov.io/gh/NibuTake/PyDEA)
+[![Python](https://img.shields.io/badge/Python-3.8%20%7C%203.9%20%7C%203.10%20-blue)](https://codecov.io/gh/NibuTake/PyDEA)
 [![License](https://img.shields.io/github/license/NibuTake/PyDEA?color=blue)](LICENSE)
 [![codecov](https://codecov.io/gh/NibuTake/PyDEA/branch/main/graph/badge.svg?token=EL44JBAYOT)](https://codecov.io/gh/NibuTake/PyDEA)
 
-
 [Install](#installation) | [Tutorial](https://nibutake.github.io/PyDEA/tutorials/index.html#) | [Docs](https://nibutake.github.io/PyDEA/index.html) | [Contribution](./CONTRIBUTING.md)
 
 Pyfrontier is a data envelopment analysis for Python user. Our main motivation is to encourage more people to use DEA effectively and contribute to the development of DEA field.
 
 ## Installation
-This module is offered by PyPI.
+
+This module is provided by [PyPI](https://pypi.org/project/Pyfrontier/).
 
 ```
 pip install Pyfrontier
 ```
 
 ## Tutorial
+
 A brief example is provided below. For more information, please click [here](https://nibutake.github.io/PyDEA/tutorials/index.html#).
 
 ```python
 import numpy as np
 from Pyfrontier.frontier_model import EnvelopeDEA
 
 dea = EnvelopeDEA(frontier="CRS", orient="in")
 
 dea.fit(inputs, outputs)
 dea.result
 ```
 
 ## Communication
+
 - [Issues](https://github.com/NibuTake/PyDEA/issues) for bug reports and feature requests.
 - [Discussion](https://github.com/NibuTake/PyDEA/discussions) for any questions.
 
 ## References
+
 We use [ref.bib](./tutorials/ref.bib) for tutorial.
 These are read by [bibtexparser](https://bibtexparser.readthedocs.io/en/master/) and automatically quoted and displayed at the specified location.
```

### Comparing `Pyfrontier-0.1.1/README.md` & `Pyfrontier-1.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 # Pyfrontier: A data envelopment analysis module
+
 <div align="center"><img src="./images/logo.png" height="200"/></div>
 
-[![Python](https://img.shields.io/badge/Python-3.8%20%7C%203.9-blue)](https://codecov.io/gh/NibuTake/PyDEA)
+[![Python](https://img.shields.io/badge/Python-3.8%20%7C%203.9%20%7C%203.10%20-blue)](https://codecov.io/gh/NibuTake/PyDEA)
 [![License](https://img.shields.io/github/license/NibuTake/PyDEA?color=blue)](LICENSE)
 [![codecov](https://codecov.io/gh/NibuTake/PyDEA/branch/main/graph/badge.svg?token=EL44JBAYOT)](https://codecov.io/gh/NibuTake/PyDEA)
 
-
 [Install](#installation) | [Tutorial](https://nibutake.github.io/PyDEA/tutorials/index.html#) | [Docs](https://nibutake.github.io/PyDEA/index.html) | [Contribution](./CONTRIBUTING.md)
 
 Pyfrontier is a data envelopment analysis for Python user. Our main motivation is to encourage more people to use DEA effectively and contribute to the development of DEA field.
 
 ## Installation
-This module is offered by PyPI.
+
+This module is provided by [PyPI](https://pypi.org/project/Pyfrontier/).
 
 ```
 pip install Pyfrontier
 ```
 
 ## Tutorial
+
 A brief example is provided below. For more information, please click [here](https://nibutake.github.io/PyDEA/tutorials/index.html#).
 
 ```python
 import numpy as np
 from Pyfrontier.frontier_model import EnvelopeDEA
 
 dea = EnvelopeDEA(frontier="CRS", orient="in")
 
 dea.fit(inputs, outputs)
 dea.result
 ```
 
 ## Communication
+
 - [Issues](https://github.com/NibuTake/PyDEA/issues) for bug reports and feature requests.
 - [Discussion](https://github.com/NibuTake/PyDEA/discussions) for any questions.
 
 ## References
+
 We use [ref.bib](./tutorials/ref.bib) for tutorial.
 These are read by [bibtexparser](https://bibtexparser.readthedocs.io/en/master/) and automatically quoted and displayed at the specified location.
```

### Comparing `Pyfrontier-0.1.1/setup.py` & `Pyfrontier-1.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from glob import glob
 from os.path import basename, splitext
 
 from setuptools import find_packages, setup
 
 # import Pyfrontier
 
-
 URL = "https://nibutake.github.io/PyDEA/index.html?"
 DOWNLOAD_URL = "https://github.com/NibuTake/PyDEA"
 
 DESCRIPTION = "Pyfrontier is a data envelopment analysis for Python user."
 
 PYTHON_REQUIRES = ">=3.8"
 INSTALL_REQUIRES = ["numpy>=1.21", "pulp>=2.6.0"]
@@ -33,15 +32,15 @@
     "Topic :: Software Development :: Libraries",
 ]
 
 
 setup(
     name="Pyfrontier",
     # version=Pyfrontier.__version__,
-    version="0.1.1",
+    version="1.0.0",
     license="MIT",
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Takeshi Morinibu",
     author_email="takeshi715tech@gmail.com",
     url=URL,
```

### Comparing `Pyfrontier-0.1.1/src/Pyfrontier/domain/dmu.py` & `Pyfrontier-1.0.0/src/Pyfrontier/domain/dmu.py`

 * *Files identical despite different names*

### Comparing `Pyfrontier-0.1.1/src/Pyfrontier/domain/result.py` & `Pyfrontier-1.0.0/src/Pyfrontier/domain/result.py`

 * *Files identical despite different names*

### Comparing `Pyfrontier-0.1.1/src/Pyfrontier/domain/slack_weight.py` & `Pyfrontier-1.0.0/src/Pyfrontier/domain/slack_weight.py`

 * *Files identical despite different names*

### Comparing `Pyfrontier-0.1.1/src/Pyfrontier/frontier_model/_additive_dea.py` & `Pyfrontier-1.0.0/src/Pyfrontier/frontier_model/_additive_dea.py`

 * *Files identical despite different names*

### Comparing `Pyfrontier-0.1.1/src/Pyfrontier/frontier_model/_base.py` & `Pyfrontier-1.0.0/src/Pyfrontier/frontier_model/_base.py`

 * *Files identical despite different names*

### Comparing `Pyfrontier-0.1.1/src/Pyfrontier/frontier_model/_dea.py` & `Pyfrontier-1.0.0/src/Pyfrontier/frontier_model/_dea.py`

 * *Files identical despite different names*

### Comparing `Pyfrontier-0.1.1/src/Pyfrontier/frontier_model/_hierarchical_dea.py` & `Pyfrontier-1.0.0/src/Pyfrontier/frontier_model/_hierarchical_dea.py`

 * *Files identical despite different names*

### Comparing `Pyfrontier-0.1.1/src/Pyfrontier/solver/_additive_solver.py` & `Pyfrontier-1.0.0/src/Pyfrontier/solver/_additive_solver.py`

 * *Files identical despite different names*

### Comparing `Pyfrontier-0.1.1/src/Pyfrontier/solver/_base.py` & `Pyfrontier-1.0.0/src/Pyfrontier/solver/_base.py`

 * *Files identical despite different names*

### Comparing `Pyfrontier-0.1.1/src/Pyfrontier/solver/_envelope_solver.py` & `Pyfrontier-1.0.0/src/Pyfrontier/solver/_envelope_solver.py`

 * *Files identical despite different names*

### Comparing `Pyfrontier-0.1.1/src/Pyfrontier/solver/_multiple_solver.py` & `Pyfrontier-1.0.0/src/Pyfrontier/solver/_multiple_solver.py`

 * *Files identical despite different names*

### Comparing `Pyfrontier-0.1.1/src/Pyfrontier.egg-info/PKG-INFO` & `Pyfrontier-1.0.0/src/Pyfrontier.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pyfrontier
-Version: 0.1.1
+Version: 1.0.0
 Summary: Pyfrontier is a data envelopment analysis for Python user.
 Home-page: https://nibutake.github.io/PyDEA/index.html?
 Download-URL: https://github.com/NibuTake/PyDEA
 Author: Takeshi Morinibu
 Author-email: takeshi715tech@gmail.com
 License: MIT
 Classifier: Intended Audience :: Science/Research
@@ -19,45 +19,49 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Pyfrontier: A data envelopment analysis module
+
 <div align="center"><img src="./images/logo.png" height="200"/></div>
 
-[![Python](https://img.shields.io/badge/Python-3.8%20%7C%203.9-blue)](https://codecov.io/gh/NibuTake/PyDEA)
+[![Python](https://img.shields.io/badge/Python-3.8%20%7C%203.9%20%7C%203.10%20-blue)](https://codecov.io/gh/NibuTake/PyDEA)
 [![License](https://img.shields.io/github/license/NibuTake/PyDEA?color=blue)](LICENSE)
 [![codecov](https://codecov.io/gh/NibuTake/PyDEA/branch/main/graph/badge.svg?token=EL44JBAYOT)](https://codecov.io/gh/NibuTake/PyDEA)
 
-
 [Install](#installation) | [Tutorial](https://nibutake.github.io/PyDEA/tutorials/index.html#) | [Docs](https://nibutake.github.io/PyDEA/index.html) | [Contribution](./CONTRIBUTING.md)
 
 Pyfrontier is a data envelopment analysis for Python user. Our main motivation is to encourage more people to use DEA effectively and contribute to the development of DEA field.
 
 ## Installation
-This module is offered by PyPI.
+
+This module is provided by [PyPI](https://pypi.org/project/Pyfrontier/).
 
 ```
 pip install Pyfrontier
 ```
 
 ## Tutorial
+
 A brief example is provided below. For more information, please click [here](https://nibutake.github.io/PyDEA/tutorials/index.html#).
 
 ```python
 import numpy as np
 from Pyfrontier.frontier_model import EnvelopeDEA
 
 dea = EnvelopeDEA(frontier="CRS", orient="in")
 
 dea.fit(inputs, outputs)
 dea.result
 ```
 
 ## Communication
+
 - [Issues](https://github.com/NibuTake/PyDEA/issues) for bug reports and feature requests.
 - [Discussion](https://github.com/NibuTake/PyDEA/discussions) for any questions.
 
 ## References
+
 We use [ref.bib](./tutorials/ref.bib) for tutorial.
 These are read by [bibtexparser](https://bibtexparser.readthedocs.io/en/master/) and automatically quoted and displayed at the specified location.
```

### Comparing `Pyfrontier-0.1.1/src/Pyfrontier.egg-info/SOURCES.txt` & `Pyfrontier-1.0.0/src/Pyfrontier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

