# Comparing `tmp/fhir_analyzer-0.0.5.tar.gz` & `tmp/fhir_analyzer-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fhir_analyzer-0.0.5.tar", last modified: Thu Jun 29 20:12:50 2023, max compression
+gzip compressed data, was "fhir_analyzer-0.0.6.tar", last modified: Sun Jul  9 12:32:00 2023, max compression
```

## Comparing `fhir_analyzer-0.0.5.tar` & `fhir_analyzer-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,29 @@
-drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-06-29 20:12:50.363669 fhir_analyzer-0.0.5/
--rw-r--r--   0 tillrostalski   (501) staff       (20)     1071 2023-06-25 13:13:22.000000 fhir_analyzer-0.0.5/LICENSE
--rw-r--r--   0 tillrostalski   (501) staff       (20)      477 2023-06-29 20:12:50.363498 fhir_analyzer-0.0.5/PKG-INFO
--rw-r--r--   0 tillrostalski   (501) staff       (20)       16 2023-06-24 16:03:53.000000 fhir_analyzer-0.0.5/README.md
--rw-r--r--   0 tillrostalski   (501) staff       (20)      782 2023-06-29 20:12:40.000000 fhir_analyzer-0.0.5/pyproject.toml
--rw-r--r--   0 tillrostalski   (501) staff       (20)       38 2023-06-29 20:12:50.363711 fhir_analyzer-0.0.5/setup.cfg
-drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-06-29 20:12:50.358518 fhir_analyzer-0.0.5/src/
-drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-06-29 20:12:50.361236 fhir_analyzer-0.0.5/src/fhir_analyzer/
--rw-r--r--   0 tillrostalski   (501) staff       (20)        0 2023-06-18 09:07:45.000000 fhir_analyzer-0.0.5/src/fhir_analyzer/__init__.py
--rw-r--r--   0 tillrostalski   (501) staff       (20)     4139 2023-06-18 17:05:10.000000 fhir_analyzer-0.0.5/src/fhir_analyzer/constants.py
--rw-r--r--   0 tillrostalski   (501) staff       (20)     5021 2023-06-29 20:08:59.000000 fhir_analyzer-0.0.5/src/fhir_analyzer/feature_selector.py
--rw-r--r--   0 tillrostalski   (501) staff       (20)     3444 2023-06-19 15:53:02.000000 fhir_analyzer-0.0.5/src/fhir_analyzer/fhirstore.py
--rw-r--r--   0 tillrostalski   (501) staff       (20)     2362 2023-06-29 16:04:29.000000 fhir_analyzer-0.0.5/src/fhir_analyzer/helper.py
-drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-06-29 20:12:50.363160 fhir_analyzer-0.0.5/src/fhir_analyzer/patient_similarity/
--rw-r--r--   0 tillrostalski   (501) staff       (20)        0 2023-06-19 15:56:47.000000 fhir_analyzer-0.0.5/src/fhir_analyzer/patient_similarity/__init__.py
--rw-r--r--   0 tillrostalski   (501) staff       (20)    13134 2023-06-29 20:01:02.000000 fhir_analyzer-0.0.5/src/fhir_analyzer/patient_similarity/comparator.py
--rw-r--r--   0 tillrostalski   (501) staff       (20)     2389 2023-06-29 20:09:09.000000 fhir_analyzer-0.0.5/src/fhir_analyzer/patient_similarity/internal_types.py
--rw-r--r--   0 tillrostalski   (501) staff       (20)     9244 2023-06-29 20:08:44.000000 fhir_analyzer-0.0.5/src/fhir_analyzer/patient_similarity/patsim.py
--rw-r--r--   0 tillrostalski   (501) staff       (20)     2521 2023-06-29 20:10:42.000000 fhir_analyzer-0.0.5/src/fhir_analyzer/tmp.py
-drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-06-29 20:12:50.362367 fhir_analyzer-0.0.5/src/fhir_analyzer.egg-info/
--rw-r--r--   0 tillrostalski   (501) staff       (20)      477 2023-06-29 20:12:50.000000 fhir_analyzer-0.0.5/src/fhir_analyzer.egg-info/PKG-INFO
--rw-r--r--   0 tillrostalski   (501) staff       (20)      621 2023-06-29 20:12:50.000000 fhir_analyzer-0.0.5/src/fhir_analyzer.egg-info/SOURCES.txt
--rw-r--r--   0 tillrostalski   (501) staff       (20)        1 2023-06-29 20:12:50.000000 fhir_analyzer-0.0.5/src/fhir_analyzer.egg-info/dependency_links.txt
--rw-r--r--   0 tillrostalski   (501) staff       (20)       82 2023-06-29 20:12:50.000000 fhir_analyzer-0.0.5/src/fhir_analyzer.egg-info/requires.txt
--rw-r--r--   0 tillrostalski   (501) staff       (20)       14 2023-06-29 20:12:50.000000 fhir_analyzer-0.0.5/src/fhir_analyzer.egg-info/top_level.txt
+drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-07-09 12:32:00.137485 fhir_analyzer-0.0.6/
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     1071 2023-06-25 13:13:22.000000 fhir_analyzer-0.0.6/LICENSE
+-rw-r--r--   0 tillrostalski   (501) staff       (20)       64 2023-07-09 12:29:27.000000 fhir_analyzer-0.0.6/MANIFEST.in
+-rw-r--r--   0 tillrostalski   (501) staff       (20)      477 2023-07-09 12:32:00.137307 fhir_analyzer-0.0.6/PKG-INFO
+-rw-r--r--   0 tillrostalski   (501) staff       (20)       16 2023-06-24 16:03:53.000000 fhir_analyzer-0.0.6/README.md
+-rw-r--r--   0 tillrostalski   (501) staff       (20)      768 2023-07-09 12:31:53.000000 fhir_analyzer-0.0.6/pyproject.toml
+-rw-r--r--   0 tillrostalski   (501) staff       (20)       38 2023-07-09 12:32:00.137532 fhir_analyzer-0.0.6/setup.cfg
+drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-07-09 12:32:00.093293 fhir_analyzer-0.0.6/src/
+drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-07-09 12:32:00.094927 fhir_analyzer-0.0.6/src/fhir_analyzer/
+-rw-r--r--   0 tillrostalski   (501) staff       (20)        0 2023-06-18 09:07:45.000000 fhir_analyzer-0.0.6/src/fhir_analyzer/__init__.py
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     4139 2023-06-18 17:05:10.000000 fhir_analyzer-0.0.6/src/fhir_analyzer/constants.py
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     5021 2023-06-29 20:08:59.000000 fhir_analyzer-0.0.6/src/fhir_analyzer/feature_selector.py
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     3444 2023-07-07 18:29:26.000000 fhir_analyzer-0.0.6/src/fhir_analyzer/fhirstore.py
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     2362 2023-06-29 16:04:29.000000 fhir_analyzer-0.0.6/src/fhir_analyzer/helper.py
+drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-07-09 12:32:00.096401 fhir_analyzer-0.0.6/src/fhir_analyzer/patient_similarity/
+-rw-r--r--   0 tillrostalski   (501) staff       (20)        0 2023-06-19 15:56:47.000000 fhir_analyzer-0.0.6/src/fhir_analyzer/patient_similarity/__init__.py
+-rw-r--r--   0 tillrostalski   (501) staff       (20)    13134 2023-06-29 20:01:02.000000 fhir_analyzer-0.0.6/src/fhir_analyzer/patient_similarity/comparator.py
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     2553 2023-07-07 18:22:57.000000 fhir_analyzer-0.0.6/src/fhir_analyzer/patient_similarity/internal_types.py
+drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-07-09 12:32:00.100017 fhir_analyzer-0.0.6/src/fhir_analyzer/patient_similarity/nx_graphs/
+-rw-r--r--   0 tillrostalski   (501) staff       (20)  1941065 2023-06-25 15:01:20.000000 fhir_analyzer-0.0.6/src/fhir_analyzer/patient_similarity/nx_graphs/icd10_nx.gpickle
+-rw-r--r--   0 tillrostalski   (501) staff       (20) 26243943 2023-06-25 19:57:53.000000 fhir_analyzer-0.0.6/src/fhir_analyzer/patient_similarity/nx_graphs/snomed.gpickle
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     9244 2023-06-30 20:17:38.000000 fhir_analyzer-0.0.6/src/fhir_analyzer/patient_similarity/patsim.py
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     3804 2023-07-07 18:47:00.000000 fhir_analyzer-0.0.6/src/fhir_analyzer/tmp.py
+drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-07-09 12:32:00.095563 fhir_analyzer-0.0.6/src/fhir_analyzer.egg-info/
+-rw-r--r--   0 tillrostalski   (501) staff       (20)      477 2023-07-09 12:32:00.000000 fhir_analyzer-0.0.6/src/fhir_analyzer.egg-info/PKG-INFO
+-rw-r--r--   0 tillrostalski   (501) staff       (20)      759 2023-07-09 12:32:00.000000 fhir_analyzer-0.0.6/src/fhir_analyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 tillrostalski   (501) staff       (20)        1 2023-07-09 12:32:00.000000 fhir_analyzer-0.0.6/src/fhir_analyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 tillrostalski   (501) staff       (20)       73 2023-07-09 12:32:00.000000 fhir_analyzer-0.0.6/src/fhir_analyzer.egg-info/requires.txt
+-rw-r--r--   0 tillrostalski   (501) staff       (20)       14 2023-07-09 12:32:00.000000 fhir_analyzer-0.0.6/src/fhir_analyzer.egg-info/top_level.txt
```

### Comparing `fhir_analyzer-0.0.5/LICENSE` & `fhir_analyzer-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fhir_analyzer-0.0.5/pyproject.toml` & `fhir_analyzer-0.0.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fhir_analyzer"
-version = "0.0.5"
+version = "0.0.6"
 authors = [{ name = "Till Rostalski", email = "tillrostalski@gmail.com" }]
 description = "A small FHIR package"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 dependencies = [
   "fhir.resources",
-  "pydantic",
   "pandas",
   "fhirpathpy",
   "networkx",
   "nxontology",
 ]
 
 [project.optional-dependencies]
```

### Comparing `fhir_analyzer-0.0.5/src/fhir_analyzer/constants.py` & `fhir_analyzer-0.0.6/src/fhir_analyzer/constants.py`

 * *Files identical despite different names*

### Comparing `fhir_analyzer-0.0.5/src/fhir_analyzer/feature_selector.py` & `fhir_analyzer-0.0.6/src/fhir_analyzer/feature_selector.py`

 * *Files identical despite different names*

### Comparing `fhir_analyzer-0.0.5/src/fhir_analyzer/fhirstore.py` & `fhir_analyzer-0.0.6/src/fhir_analyzer/fhirstore.py`

 * *Files identical despite different names*

### Comparing `fhir_analyzer-0.0.5/src/fhir_analyzer/helper.py` & `fhir_analyzer-0.0.6/src/fhir_analyzer/helper.py`

 * *Files identical despite different names*

### Comparing `fhir_analyzer-0.0.5/src/fhir_analyzer/patient_similarity/comparator.py` & `fhir_analyzer-0.0.6/src/fhir_analyzer/patient_similarity/comparator.py`

 * *Files identical despite different names*

### Comparing `fhir_analyzer-0.0.5/src/fhir_analyzer/patient_similarity/internal_types.py` & `fhir_analyzer-0.0.6/src/fhir_analyzer/patient_similarity/internal_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,26 +11,28 @@
     def __init__(self, code: str, system: str, feature_name: str):
         if not isinstance(code, str):
             raise ValueError(
                 f"Feature code for {feature_name} expected str, got {type(code)}: {code}"
             )
         self.code = code
         self.system = system
+        self.feature_name = feature_name
 
     def __str__(self):
         return f"CodedConcept({self.code}, {self.system})"
 
 
 class CategoricalString:
     def __init__(self, value: str, feature_name: str):
         if not isinstance(value, str):
             raise ValueError(
                 f"Feature value for {feature_name} expected str, got {type(value)}: {value}"
             )
         self.value = value
+        self.feature_name = feature_name
 
     def __str__(self):
         return f"CategoricalString({self.value})"
 
 
 class Numerical:
     def __init__(
@@ -39,14 +41,15 @@
         if not isinstance(value, float):
             raise ValueError(
                 f"Feature value for {feature_name} expected float, got {type(value)}: {value}"
             )
         self.value = value
         self.max_value = max_value
         self.min_value = min_value
+        self.feature_name = feature_name
 
     def __str__(self):
         return f"Numerical({self.value}, {self.max_value}, {self.min_value})"
 
 
 class CodedNumerical:
     def __init__(
@@ -68,10 +71,11 @@
             )
         is_abnormal = is_abnormal if is_abnormal is not None else True
         self.value = value
         self.code = code
         self.code_mean = code_mean
         self.code_std_dev = code_std_dev
         self.is_abnormal = is_abnormal
+        self.feature_name = feature_name
 
     def __str__(self):
         return f"CodedNumerical({self.value}, {self.code}, {self.code_mean}, {self.code_std_dev}, {self.is_abnormal})"
```

### Comparing `fhir_analyzer-0.0.5/src/fhir_analyzer/patient_similarity/patsim.py` & `fhir_analyzer-0.0.6/src/fhir_analyzer/patient_similarity/patsim.py`

 * *Files identical despite different names*

### Comparing `fhir_analyzer-0.0.5/src/fhir_analyzer.egg-info/SOURCES.txt` & `fhir_analyzer-0.0.6/src/fhir_analyzer.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 src/fhir_analyzer/__init__.py
 src/fhir_analyzer/constants.py
 src/fhir_analyzer/feature_selector.py
 src/fhir_analyzer/fhirstore.py
 src/fhir_analyzer/helper.py
@@ -11,8 +12,10 @@
 src/fhir_analyzer.egg-info/SOURCES.txt
 src/fhir_analyzer.egg-info/dependency_links.txt
 src/fhir_analyzer.egg-info/requires.txt
 src/fhir_analyzer.egg-info/top_level.txt
 src/fhir_analyzer/patient_similarity/__init__.py
 src/fhir_analyzer/patient_similarity/comparator.py
 src/fhir_analyzer/patient_similarity/internal_types.py
-src/fhir_analyzer/patient_similarity/patsim.py
+src/fhir_analyzer/patient_similarity/patsim.py
+src/fhir_analyzer/patient_similarity/nx_graphs/icd10_nx.gpickle
+src/fhir_analyzer/patient_similarity/nx_graphs/snomed.gpickle
```

