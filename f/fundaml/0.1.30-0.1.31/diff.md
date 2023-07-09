# Comparing `tmp/fundaml-0.1.30.tar.gz` & `tmp/fundaml-0.1.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fundaml-0.1.30.tar", max compression
+gzip compressed data, was "fundaml-0.1.31.tar", max compression
```

## Comparing `fundaml-0.1.30.tar` & `fundaml-0.1.31.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0     1069 2023-07-08 20:50:13.472075 fundaml-0.1.30/LICENSE
--rw-r--r--   0        0        0     2328 2023-07-08 20:50:13.472075 fundaml-0.1.30/README.md
--rw-r--r--   0        0        0     1614 2023-07-08 21:01:13.009164 fundaml-0.1.30/pyproject.toml
--rw-r--r--   0        0        0      109 2023-07-08 20:50:13.868074 fundaml-0.1.30/src/fundaml/__init__.py
--rw-r--r--   0        0        0     1058 2023-07-08 20:50:13.868074 fundaml-0.1.30/src/fundaml/eda.py
--rw-r--r--   0        0        0     1400 2023-07-08 20:50:13.868074 fundaml-0.1.30/src/fundaml/models.py
--rw-r--r--   0        0        0     1032 2023-07-08 20:50:13.868074 fundaml-0.1.30/src/fundaml/scores.py
--rw-r--r--   0        0        0    17645 2023-07-08 20:50:13.868074 fundaml-0.1.30/src/fundaml/trainers.py
--rw-r--r--   0        0        0     3199 1970-01-01 00:00:00.000000 fundaml-0.1.30/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2023-07-09 19:32:10.338305 fundaml-0.1.31/LICENSE
+-rw-r--r--   0        0        0     2314 2023-07-09 19:32:10.338305 fundaml-0.1.31/README.md
+-rw-r--r--   0        0        0     1614 2023-07-09 19:44:02.670575 fundaml-0.1.31/pyproject.toml
+-rw-r--r--   0        0        0      109 2023-07-09 19:32:10.710312 fundaml-0.1.31/src/fundaml/__init__.py
+-rw-r--r--   0        0        0     1058 2023-07-09 19:32:10.710312 fundaml-0.1.31/src/fundaml/eda.py
+-rw-r--r--   0        0        0     1400 2023-07-09 19:32:10.710312 fundaml-0.1.31/src/fundaml/models.py
+-rw-r--r--   0        0        0     1032 2023-07-09 19:32:10.710312 fundaml-0.1.31/src/fundaml/scores.py
+-rw-r--r--   0        0        0    17645 2023-07-09 19:32:10.710312 fundaml-0.1.31/src/fundaml/trainers.py
+-rw-r--r--   0        0        0     3185 1970-01-01 00:00:00.000000 fundaml-0.1.31/PKG-INFO
```

### Comparing `fundaml-0.1.30/LICENSE` & `fundaml-0.1.31/LICENSE`

 * *Files identical despite different names*

### Comparing `fundaml-0.1.30/README.md` & `fundaml-0.1.31/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
-[![codecov](https://codecov.io/github/tzoght/mltz-base/branch/main/graph/badge.svg?token=UB03POGOUB)](https://codecov.io/github/tzoght/mltz-base)
-[![ci-cd](https://github.com/tzoght/mltz-base/actions/workflows/ci-cd.yml/badge.svg?branch=main)](https://github.com/tzoght/mltz-base/actions/workflows/ci-cd.yml) [![Documentation Status](https://readthedocs.org/projects/mltz-base/badge/?version=latest)](https://mltz-base.readthedocs.io/en/latest/?badge=latest) ![PyPI](https://img.shields.io/pypi/v/mltz_base)
+[![codecov](https://codecov.io/github/tzoght/fundaml/branch/main/graph/badge.svg?token=UB03POGOUB)](https://codecov.io/github/tzoght/fundaml)
+[![ci-cd](https://github.com/tzoght/fundaml/actions/workflows/ci-cd.yml/badge.svg?branch=main)](https://github.com/tzoght/fundaml/actions/workflows/ci-cd.yml) [![Documentation Status](https://readthedocs.org/projects/fundaml/badge/?version=latest)](https://fundaml.readthedocs.io/en/stable/?badge=stable) ![PyPI](https://img.shields.io/pypi/v/fundaml)
 
 # fundaml
 
 The purpose of this module is simply to simplify ML learning and use best practices while developing ML models. 
 
 **Standardization**: The fundaml project is an attempt to standardize the way ML projects are structured within a team or organization, promoting best practices for organization, testing, and documentation.
```

### Comparing `fundaml-0.1.30/pyproject.toml` & `fundaml-0.1.31/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fundaml"
-version = "0.1.30"
+version = "0.1.31"
 description = "A foundational machine learning library designed to streamline the end-to-end process of developing and deploying machine learning models. FundAML offers a broad array of tools and utilities for data preprocessing, model training, evaluation, and deployment, making it a fundamental solution for machine learning tasks."
 authors = ["Tony Zoght"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10"
```

### Comparing `fundaml-0.1.30/src/fundaml/eda.py` & `fundaml-0.1.31/src/fundaml/eda.py`

 * *Files identical despite different names*

### Comparing `fundaml-0.1.30/src/fundaml/models.py` & `fundaml-0.1.31/src/fundaml/models.py`

 * *Files identical despite different names*

### Comparing `fundaml-0.1.30/src/fundaml/scores.py` & `fundaml-0.1.31/src/fundaml/scores.py`

 * *Files identical despite different names*

### Comparing `fundaml-0.1.30/src/fundaml/trainers.py` & `fundaml-0.1.31/src/fundaml/trainers.py`

 * *Files identical despite different names*

### Comparing `fundaml-0.1.30/PKG-INFO` & `fundaml-0.1.31/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fundaml
-Version: 0.1.30
+Version: 0.1.31
 Summary: A foundational machine learning library designed to streamline the end-to-end process of developing and deploying machine learning models. FundAML offers a broad array of tools and utilities for data preprocessing, model training, evaluation, and deployment, making it a fundamental solution for machine learning tasks.
 License: MIT
 Author: Tony Zoght
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -13,16 +13,16 @@
 Requires-Dist: pandas (>=1.4.0)
 Requires-Dist: torch (>=2.0.1,<3.0.0)
 Requires-Dist: torchaudio (>=2.0.2,<3.0.0)
 Requires-Dist: torchvision (>=0.15.2,<0.16.0)
 Description-Content-Type: text/markdown
 
 
-[![codecov](https://codecov.io/github/tzoght/mltz-base/branch/main/graph/badge.svg?token=UB03POGOUB)](https://codecov.io/github/tzoght/mltz-base)
-[![ci-cd](https://github.com/tzoght/mltz-base/actions/workflows/ci-cd.yml/badge.svg?branch=main)](https://github.com/tzoght/mltz-base/actions/workflows/ci-cd.yml) [![Documentation Status](https://readthedocs.org/projects/mltz-base/badge/?version=latest)](https://mltz-base.readthedocs.io/en/latest/?badge=latest) ![PyPI](https://img.shields.io/pypi/v/mltz_base)
+[![codecov](https://codecov.io/github/tzoght/fundaml/branch/main/graph/badge.svg?token=UB03POGOUB)](https://codecov.io/github/tzoght/fundaml)
+[![ci-cd](https://github.com/tzoght/fundaml/actions/workflows/ci-cd.yml/badge.svg?branch=main)](https://github.com/tzoght/fundaml/actions/workflows/ci-cd.yml) [![Documentation Status](https://readthedocs.org/projects/fundaml/badge/?version=latest)](https://fundaml.readthedocs.io/en/stable/?badge=stable) ![PyPI](https://img.shields.io/pypi/v/fundaml)
 
 # fundaml
 
 The purpose of this module is simply to simplify ML learning and use best practices while developing ML models. 
 
 **Standardization**: The fundaml project is an attempt to standardize the way ML projects are structured within a team or organization, promoting best practices for organization, testing, and documentation.
```

