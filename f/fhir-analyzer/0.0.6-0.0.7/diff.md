# Comparing `tmp/fhir_analyzer-0.0.6.tar.gz` & `tmp/fhir_analyzer-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fhir_analyzer-0.0.6.tar", last modified: Sun Jul  9 12:32:00 2023, max compression
+gzip compressed data, was "fhir_analyzer-0.0.7.tar", last modified: Sun Jul  9 18:00:03 2023, max compression
```

## Comparing `fhir_analyzer-0.0.6.tar` & `fhir_analyzer-0.0.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-07-09 12:32:00.137485 fhir_analyzer-0.0.6/
--rw-r--r--   0 tillrostalski   (501) staff       (20)     1071 2023-06-25 13:13:22.000000 fhir_analyzer-0.0.6/LICENSE
--rw-r--r--   0 tillrostalski   (501) staff       (20)       64 2023-07-09 12:29:27.000000 fhir_analyzer-0.0.6/MANIFEST.in
--rw-r--r--   0 tillrostalski   (501) staff       (20)      477 2023-07-09 12:32:00.137307 fhir_analyzer-0.0.6/PKG-INFO
--rw-r--r--   0 tillrostalski   (501) staff       (20)       16 2023-06-24 16:03:53.000000 fhir_analyzer-0.0.6/README.md
--rw-r--r--   0 tillrostalski   (501) staff       (20)      768 2023-07-09 12:31:53.000000 fhir_analyzer-0.0.6/pyproject.toml
--rw-r--r--   0 tillrostalski   (501) staff       (20)       38 2023-07-09 12:32:00.137532 fhir_analyzer-0.0.6/setup.cfg
-drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-07-09 12:32:00.093293 fhir_analyzer-0.0.6/src/
-drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-07-09 12:32:00.094927 fhir_analyzer-0.0.6/src/fhir_analyzer/
--rw-r--r--   0 tillrostalski   (501) staff       (20)        0 2023-06-18 09:07:45.000000 fhir_analyzer-0.0.6/src/fhir_analyzer/__init__.py
--rw-r--r--   0 tillrostalski   (501) staff       (20)     4139 2023-06-18 17:05:10.000000 fhir_analyzer-0.0.6/src/fhir_analyzer/constants.py
--rw-r--r--   0 tillrostalski   (501) staff       (20)     5021 2023-06-29 20:08:59.000000 fhir_analyzer-0.0.6/src/fhir_analyzer/feature_selector.py
--rw-r--r--   0 tillrostalski   (501) staff       (20)     3444 2023-07-07 18:29:26.000000 fhir_analyzer-0.0.6/src/fhir_analyzer/fhirstore.py
--rw-r--r--   0 tillrostalski   (501) staff       (20)     2362 2023-06-29 16:04:29.000000 fhir_analyzer-0.0.6/src/fhir_analyzer/helper.py
-drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-07-09 12:32:00.096401 fhir_analyzer-0.0.6/src/fhir_analyzer/patient_similarity/
--rw-r--r--   0 tillrostalski   (501) staff       (20)        0 2023-06-19 15:56:47.000000 fhir_analyzer-0.0.6/src/fhir_analyzer/patient_similarity/__init__.py
--rw-r--r--   0 tillrostalski   (501) staff       (20)    13134 2023-06-29 20:01:02.000000 fhir_analyzer-0.0.6/src/fhir_analyzer/patient_similarity/comparator.py
--rw-r--r--   0 tillrostalski   (501) staff       (20)     2553 2023-07-07 18:22:57.000000 fhir_analyzer-0.0.6/src/fhir_analyzer/patient_similarity/internal_types.py
-drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-07-09 12:32:00.100017 fhir_analyzer-0.0.6/src/fhir_analyzer/patient_similarity/nx_graphs/
--rw-r--r--   0 tillrostalski   (501) staff       (20)  1941065 2023-06-25 15:01:20.000000 fhir_analyzer-0.0.6/src/fhir_analyzer/patient_similarity/nx_graphs/icd10_nx.gpickle
--rw-r--r--   0 tillrostalski   (501) staff       (20) 26243943 2023-06-25 19:57:53.000000 fhir_analyzer-0.0.6/src/fhir_analyzer/patient_similarity/nx_graphs/snomed.gpickle
--rw-r--r--   0 tillrostalski   (501) staff       (20)     9244 2023-06-30 20:17:38.000000 fhir_analyzer-0.0.6/src/fhir_analyzer/patient_similarity/patsim.py
--rw-r--r--   0 tillrostalski   (501) staff       (20)     3804 2023-07-07 18:47:00.000000 fhir_analyzer-0.0.6/src/fhir_analyzer/tmp.py
-drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-07-09 12:32:00.095563 fhir_analyzer-0.0.6/src/fhir_analyzer.egg-info/
--rw-r--r--   0 tillrostalski   (501) staff       (20)      477 2023-07-09 12:32:00.000000 fhir_analyzer-0.0.6/src/fhir_analyzer.egg-info/PKG-INFO
--rw-r--r--   0 tillrostalski   (501) staff       (20)      759 2023-07-09 12:32:00.000000 fhir_analyzer-0.0.6/src/fhir_analyzer.egg-info/SOURCES.txt
--rw-r--r--   0 tillrostalski   (501) staff       (20)        1 2023-07-09 12:32:00.000000 fhir_analyzer-0.0.6/src/fhir_analyzer.egg-info/dependency_links.txt
--rw-r--r--   0 tillrostalski   (501) staff       (20)       73 2023-07-09 12:32:00.000000 fhir_analyzer-0.0.6/src/fhir_analyzer.egg-info/requires.txt
--rw-r--r--   0 tillrostalski   (501) staff       (20)       14 2023-07-09 12:32:00.000000 fhir_analyzer-0.0.6/src/fhir_analyzer.egg-info/top_level.txt
+drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-07-09 18:00:03.065728 fhir_analyzer-0.0.7/
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     1071 2023-06-25 13:13:22.000000 fhir_analyzer-0.0.7/LICENSE
+-rw-r--r--   0 tillrostalski   (501) staff       (20)       64 2023-07-09 12:29:27.000000 fhir_analyzer-0.0.7/MANIFEST.in
+-rw-r--r--   0 tillrostalski   (501) staff       (20)      477 2023-07-09 18:00:03.065481 fhir_analyzer-0.0.7/PKG-INFO
+-rw-r--r--   0 tillrostalski   (501) staff       (20)       16 2023-06-24 16:03:53.000000 fhir_analyzer-0.0.7/README.md
+-rw-r--r--   0 tillrostalski   (501) staff       (20)      768 2023-07-09 17:59:39.000000 fhir_analyzer-0.0.7/pyproject.toml
+-rw-r--r--   0 tillrostalski   (501) staff       (20)       38 2023-07-09 18:00:03.065782 fhir_analyzer-0.0.7/setup.cfg
+drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-07-09 18:00:03.024936 fhir_analyzer-0.0.7/src/
+drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-07-09 18:00:03.027853 fhir_analyzer-0.0.7/src/fhir_analyzer/
+-rw-r--r--   0 tillrostalski   (501) staff       (20)        0 2023-06-18 09:07:45.000000 fhir_analyzer-0.0.7/src/fhir_analyzer/__init__.py
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     4139 2023-06-18 17:05:10.000000 fhir_analyzer-0.0.7/src/fhir_analyzer/constants.py
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     5960 2023-07-09 14:45:11.000000 fhir_analyzer-0.0.7/src/fhir_analyzer/feature_selector.py
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     3435 2023-07-09 14:19:38.000000 fhir_analyzer-0.0.7/src/fhir_analyzer/fhirstore.py
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     2362 2023-06-29 16:04:29.000000 fhir_analyzer-0.0.7/src/fhir_analyzer/helper.py
+drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-07-09 18:00:03.029950 fhir_analyzer-0.0.7/src/fhir_analyzer/patient_similarity/
+-rw-r--r--   0 tillrostalski   (501) staff       (20)        0 2023-06-19 15:56:47.000000 fhir_analyzer-0.0.7/src/fhir_analyzer/patient_similarity/__init__.py
+-rw-r--r--   0 tillrostalski   (501) staff       (20)    13530 2023-07-09 13:38:13.000000 fhir_analyzer-0.0.7/src/fhir_analyzer/patient_similarity/comparator.py
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     1673 2023-07-09 13:26:10.000000 fhir_analyzer-0.0.7/src/fhir_analyzer/patient_similarity/internal_types.py
+drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-07-09 18:00:03.033285 fhir_analyzer-0.0.7/src/fhir_analyzer/patient_similarity/nx_graphs/
+-rw-r--r--   0 tillrostalski   (501) staff       (20)  1941065 2023-06-25 15:01:20.000000 fhir_analyzer-0.0.7/src/fhir_analyzer/patient_similarity/nx_graphs/icd10_nx.gpickle
+-rw-r--r--   0 tillrostalski   (501) staff       (20) 26243943 2023-06-25 19:57:53.000000 fhir_analyzer-0.0.7/src/fhir_analyzer/patient_similarity/nx_graphs/snomed.gpickle
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     9372 2023-07-09 14:43:15.000000 fhir_analyzer-0.0.7/src/fhir_analyzer/patient_similarity/patsim.py
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     3817 2023-07-09 14:45:13.000000 fhir_analyzer-0.0.7/src/fhir_analyzer/tmp.py
+drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-07-09 18:00:03.028947 fhir_analyzer-0.0.7/src/fhir_analyzer.egg-info/
+-rw-r--r--   0 tillrostalski   (501) staff       (20)      477 2023-07-09 18:00:03.000000 fhir_analyzer-0.0.7/src/fhir_analyzer.egg-info/PKG-INFO
+-rw-r--r--   0 tillrostalski   (501) staff       (20)      759 2023-07-09 18:00:03.000000 fhir_analyzer-0.0.7/src/fhir_analyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 tillrostalski   (501) staff       (20)        1 2023-07-09 18:00:03.000000 fhir_analyzer-0.0.7/src/fhir_analyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 tillrostalski   (501) staff       (20)       73 2023-07-09 18:00:03.000000 fhir_analyzer-0.0.7/src/fhir_analyzer.egg-info/requires.txt
+-rw-r--r--   0 tillrostalski   (501) staff       (20)       14 2023-07-09 18:00:03.000000 fhir_analyzer-0.0.7/src/fhir_analyzer.egg-info/top_level.txt
```

### Comparing `fhir_analyzer-0.0.6/LICENSE` & `fhir_analyzer-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fhir_analyzer-0.0.6/pyproject.toml` & `fhir_analyzer-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fhir_analyzer"
-version = "0.0.6"
+version = "0.0.7"
 authors = [{ name = "Till Rostalski", email = "tillrostalski@gmail.com" }]
 description = "A small FHIR package"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
```

### Comparing `fhir_analyzer-0.0.6/src/fhir_analyzer/constants.py` & `fhir_analyzer-0.0.7/src/fhir_analyzer/constants.py`

 * *Files identical despite different names*

### Comparing `fhir_analyzer-0.0.6/src/fhir_analyzer/feature_selector.py` & `fhir_analyzer-0.0.7/src/fhir_analyzer/feature_selector.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,31 +13,49 @@
                 res = targ_fn(resource)
                 if res:
                     return res
     return None
 
 
 class FeatureSelector:
-    def __init__(self, fhirstore: Fhirstore):
+    def __init__(self, fhirstore: Fhirstore = None):
         self._feature_names: list[str] = []
         self._feature_types: dict[str, str] = {}
         self._patient_features: list[dict[str, list[str]]] = {}
-        self._fhirstore = fhirstore
+        self._fhirstore = fhirstore if fhirstore else Fhirstore()
 
     @property
     def feature_df(self):
         return pd.DataFrame(self._patient_features).T
 
-    def _add_single_feature(
+    def add_feature(
+        self,
+        name: str,
+        resource_types: list[str],
+        target_paths: list[str],
+        conditional_target_paths: list[dict[str, str]] = None,
+    ):
+        target_paths = {"value": target_paths}
+        self._add_feature(
+            feature_name=name,
+            feature_type="unknown",
+            target_resource_types=resource_types,
+            target_paths=target_paths,
+            conditional_target_paths=conditional_target_paths,
+            include_target_names=False,
+        )
+
+    def _add_feature(
         self,
         feature_name: str,
         feature_type: str,
         target_resource_types: list[str],
         target_paths: dict[str, list[str]],
         conditional_target_paths: dict[str, list[dict[str, str]]] = None,
+        include_target_names=False,
     ):
         if feature_name not in self._feature_names:
             self._add_feature_metadata(feature_name, feature_type)
 
         target_fns = {
             targ_n: [compile(targ_path) for targ_path in targ_paths]
             for targ_n, targ_paths in target_paths.items()
@@ -58,41 +76,45 @@
             raise ValueError("No target paths or conditional target paths provided.")
 
         self._process_target_resources(
             target_fns,
             conditional_fns,
             feature_name,
             target_resource_types,
+            include_target_names,
         )
 
     def _add_feature_metadata(self, feature_name: str, feature_type: str):
         self._feature_names.append(feature_name)
         self._feature_types[feature_name] = feature_type
 
     def _process_target_resources(
         self,
         target_fns: list[Callable[[Any], Any]],
         conditional_fns: dict[
             str, list[tuple[Callable[[Any], bool], Callable[[Any], Any]]]
         ],
         feature_name: str,
         target_resource_types: list[str],
+        include_target_names,
     ):
         for (
             patient_id,
             patient_resources,
         ) in self._fhirstore._patient_connections.items():
             self._patient_features.setdefault(patient_id, {})
             if feature_name not in self._patient_features[patient_id]:
                 self._patient_features[patient_id][feature_name] = []
             for resource_type in target_resource_types:
                 if resource_type in patient_resources:
                     for resource in patient_resources[resource_type]:
                         target = self._get_target(resource, target_fns, conditional_fns)
-                        self._update_patient_features(patient_id, feature_name, target)
+                        self._update_patient_features(
+                            patient_id, feature_name, target, include_target_names
+                        )
 
     def _get_target(
         self,
         resource: Any,
         target_fns: Union[list[Callable[[Any], Any]], dict[str, Callable[[Any], Any]]],
         conditional_fns: Union[
             list[tuple[Callable[[Any], bool], Callable[[Any], Any]]],
@@ -131,12 +153,20 @@
             if not len(target_fn(resource)) > 0:
                 continue
             target = target_fn(resource)[0]
             if target:
                 return target
         return None
 
-    def _update_patient_features(self, patient_id: str, feature_name: str, target: Any):
-        if target:
+    def _update_patient_features(
+        self,
+        patient_id: str,
+        feature_name: str,
+        target: dict[str, Any],
+        include_target_names=False,
+    ):
+        if target and include_target_names:
             self._patient_features[patient_id][feature_name].append(target)
-        else:
-            self._patient_features[patient_id][feature_name].append(None)
+        elif target and not include_target_names:
+            self._patient_features[patient_id][feature_name].append(
+                list(target.values())[0]
+            )
```

### Comparing `fhir_analyzer-0.0.6/src/fhir_analyzer/fhirstore.py` & `fhir_analyzer-0.0.7/src/fhir_analyzer/fhirstore.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,14 @@
         if resources:
             self.validate_resources_input(resources)
             self._resources += resources
         if len(self._resources) > 0:
             self._update_patient_dicts(self._resources)
 
     def _update_patient_dicts(self, resources: list[dict]):
-        """resources should not exists already"""
         for resource in resources:
             resource_id = resource["id"]
             resource_type = resource.get("resourceType", None)
             if resource_type == "Patient":
                 if not resource_id in self._patient_ids:
                     self._patient_ids.append(resource_id)
                 self._patient_connections[resource_id] = {resource_type: [resource]}
@@ -55,14 +54,17 @@
         ]
         if len(resources) == 0:
             return
         self.validate_resources_input(resources)
         self._resources += resources
         self._update_patient_dicts(resources)
 
+    def add_feature(self):
+        pass
+
     def _resource_exists(self, resource: dict) -> bool:
         for existing_resource in self._resources:
             if (
                 existing_resource["id"] == resource["id"]
                 and existing_resource["resourceType"] == resource["resourceType"]
             ):
                 return True
```

### Comparing `fhir_analyzer-0.0.6/src/fhir_analyzer/helper.py` & `fhir_analyzer-0.0.7/src/fhir_analyzer/helper.py`

 * *Files identical despite different names*

### Comparing `fhir_analyzer-0.0.6/src/fhir_analyzer/patient_similarity/comparator.py` & `fhir_analyzer-0.0.7/src/fhir_analyzer/patient_similarity/comparator.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,20 +75,28 @@
         set2 = set([i.value for i in feature2])
         intersection = set1.intersection(set2)
         union = set1.union(set2)
         return len(intersection) / len(union)
 
     def compare_numerical(self, feature1: list[Numerical], feature2: list[Numerical]):
         """Compute the mean euclidean distance between two numerical features."""
-        if len(feature1) != 1 or len(feature2) != 1:
+        if not feature1 or not feature2:
             return None
-        feature1 = feature1[0]
-        feature2 = feature2[0]
-        nom = abs(feature1.value - feature2.value) - feature1.min_value
-        denom = feature1.max_value - feature1.min_value
+        min_value = feature1[0].min_value
+        max_value = feature1[0].max_value
+        if len(feature1) > 1:
+            value1 = statistics.mean([i.value for i in feature1])
+        else:
+            value1 = feature1[0].value
+        if len(feature2) > 1:
+            value2 = statistics.mean([i.value for i in feature2])
+        else:
+            value2 = feature2[0].value
+        nom = abs(value1 - value2) - min_value
+        denom = max_value - min_value
         return 1 - (nom / denom)
 
     def compare_coded_concepts(
         self,
         feature1: list[CodedConcept],
         feature2: list[CodedConcept],
         ic_metric: str = "intrinsic_ic_sanchez",
@@ -144,22 +152,25 @@
         feature1: CodedNumerical,
         feature2: CodedNumerical,
     ):
         if feature1.is_abnormal or feature2.is_abnormal:
             mean = float(feature1.code_mean)
             std = float(feature1.code_std_dev)
 
+            if not mean or not std:
+                return None
+
             if std == 0:
                 return None
 
             value1 = float(feature1.value)
             value2 = float(feature2.value)
 
-            p1 = cdf((value1 - mean) / std)
-            p2 = cdf((value2 - mean) / std)
+            p1 = cdf((value1 - mean) / std, mean, std)
+            p2 = cdf((value2 - mean) / std, mean, std)
 
             similarity = 1 - abs(p1 - p2)
 
             mean_percentile = (p1 + p2) / 2
             similarity *= 2 * abs(mean_percentile - 0.5)
             return similarity
         else:
@@ -195,33 +206,35 @@
                     for feature in features:
                         value = feature["value"]
                         if value is not None:
                             values.append(feature["value"])
         if values:
             min_value = min(values)
             max_value = max(values)
-            if name not in numerical_stats:
-                numerical_stats[name] = {
+            numerical_stats[name].update(
+                {
                     "min_value": min_value,
                     "max_value": max_value,
                 }
+            )
         self._numerical_stats.update(numerical_stats)
 
     def _add_coded_numerical_type_data(self, name):
         code_values = {}
         code_stats = {name: {}}
         for _, features_dic in self._feature_selector._patient_features.items():
             for n, features in features_dic.items():
                 if n == name:
                     for feature in features:
                         code = feature["code"]
                         value = feature["value"]
                         if code not in code_values:
                             code_values[code] = []
                         if value:
+                            value = float(value)
                             code_values[code].append(value)
         for code, values in code_values.items():
             if code and len(values) > 1:
                 code_stats[name][code] = {
                     "mean": statistics.mean(values),
                     "std_dev": statistics.stdev(values),
                 }
@@ -236,15 +249,15 @@
             features_dic,
         ) in self._feature_selector._patient_features.items():
             updated_feature_dic[patient_id] = {}
             for name, features in features_dic.items():
                 if self._feature_selector._feature_types[name] == NUMERICAL:
                     parsed_features = [
                         Numerical(
-                            value=feature["value"],
+                            value=float(feature["value"]),
                             min_value=self._numerical_stats[name]["min_value"],
                             max_value=self._numerical_stats[name]["max_value"],
                             feature_name=name,
                         )
                         for feature in features
                         if feature["value"] is not None
                         and self._numerical_stats[name]["min_value"] is not None
```

### Comparing `fhir_analyzer-0.0.6/src/fhir_analyzer/patient_similarity/internal_types.py` & `fhir_analyzer-0.0.7/src/fhir_analyzer/patient_similarity/internal_types.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,47 +5,35 @@
 CATEGORICAL_STRING = "categorical_string"
 NUMERICAL = "numerical"
 CODED_NUMERICAL = "coded_numerical"
 
 
 class CodedConcept:
     def __init__(self, code: str, system: str, feature_name: str):
-        if not isinstance(code, str):
-            raise ValueError(
-                f"Feature code for {feature_name} expected str, got {type(code)}: {code}"
-            )
         self.code = code
         self.system = system
         self.feature_name = feature_name
 
     def __str__(self):
         return f"CodedConcept({self.code}, {self.system})"
 
 
 class CategoricalString:
     def __init__(self, value: str, feature_name: str):
-        if not isinstance(value, str):
-            raise ValueError(
-                f"Feature value for {feature_name} expected str, got {type(value)}: {value}"
-            )
         self.value = value
         self.feature_name = feature_name
 
     def __str__(self):
         return f"CategoricalString({self.value})"
 
 
 class Numerical:
     def __init__(
         self, value: float, max_value: float, min_value: float, feature_name: str
     ):
-        if not isinstance(value, float):
-            raise ValueError(
-                f"Feature value for {feature_name} expected float, got {type(value)}: {value}"
-            )
         self.value = value
         self.max_value = max_value
         self.min_value = min_value
         self.feature_name = feature_name
 
     def __str__(self):
         return f"Numerical({self.value}, {self.max_value}, {self.min_value})"
@@ -57,22 +45,14 @@
         value: float,
         code: str,
         code_mean: float,
         code_std_dev: float,
         feature_name: str,
         is_abnormal: Union[bool, None] = None,
     ):
-        if not isinstance(value, float):
-            raise ValueError(
-                f"Feature value for {feature_name} expected float, got {type(value)}: {value}"
-            )
-        if not isinstance(code, str):
-            raise ValueError(
-                f"Feature code for {feature_name} expected str, got {type(code)}: {code}"
-            )
         is_abnormal = is_abnormal if is_abnormal is not None else True
         self.value = value
         self.code = code
         self.code_mean = code_mean
         self.code_std_dev = code_std_dev
         self.is_abnormal = is_abnormal
         self.feature_name = feature_name
```

### Comparing `fhir_analyzer-0.0.6/src/fhir_analyzer/patient_similarity/nx_graphs/icd10_nx.gpickle` & `fhir_analyzer-0.0.7/src/fhir_analyzer/patient_similarity/nx_graphs/icd10_nx.gpickle`

 * *Files identical despite different names*

### Comparing `fhir_analyzer-0.0.6/src/fhir_analyzer/patient_similarity/nx_graphs/snomed.gpickle` & `fhir_analyzer-0.0.7/src/fhir_analyzer/patient_similarity/nx_graphs/snomed.gpickle`

 * *Files identical despite different names*

### Comparing `fhir_analyzer-0.0.6/src/fhir_analyzer/patient_similarity/patsim.py` & `fhir_analyzer-0.0.7/src/fhir_analyzer/patient_similarity/patsim.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,20 +87,21 @@
         target_paths = {
             "value": target_paths,
         }
         if conditional_target_paths:
             conditional_target_paths = {
                 "value": conditional_target_paths,
             }
-        self._feature_selector._add_single_feature(
+        self._feature_selector._add_feature(
             feature_name=name,
             feature_type=CATEGORICAL_STRING,
             target_resource_types=resource_types,
             target_paths=target_paths,
             conditional_target_paths=conditional_target_paths,
+            include_target_names=True,
         )
 
     def add_numerical_feature(
         self,
         name: str,
         resource_types: Union[list[str], str],
         target_paths: Union[list[str], str, None] = None,
@@ -119,20 +120,21 @@
             path_name="value",
         )
         target_paths = {
             "value": target_paths,
         }
         if conditional_target_paths:
             conditional_target_paths["value"] = conditional_target_paths
-        self._feature_selector._add_single_feature(
+        self._feature_selector._add_feature(
             feature_name=name,
             feature_type=NUMERICAL,
             target_resource_types=resource_types,
             target_paths=target_paths,
             conditional_target_paths=conditional_target_paths,
+            include_target_names=True,
         )
 
     def add_coded_concept_feature(
         self,
         name: str,
         resource_types: Union[list[str], str],
         code_paths: Union[list[str], str, None] = None,
@@ -178,20 +180,21 @@
         if conditional_code_paths:
             conditional_target_paths["code"] = conditional_code_paths
         if conditional_system_paths:
             conditional_target_paths["system"] = conditional_system_paths
         conditional_target_paths = (
             conditional_target_paths if conditional_target_paths else None
         )
-        self._feature_selector._add_single_feature(
+        self._feature_selector._add_feature(
             feature_name=name,
             feature_type=CODED_CONCEPT,
             target_resource_types=resource_types,
             target_paths=target_paths,
             conditional_target_paths=conditional_target_paths,
+            include_target_names=True,
         )
 
     def add_coded_numerical_feature(
         self,
         name: str,
         resource_types: Union[list[str], str],
         value_paths: Union[list[str], str, None] = None,
@@ -237,20 +240,21 @@
         if conditional_code_paths:
             conditional_target_paths["code"] = conditional_code_paths
         if conditional_value_paths:
             conditional_value_paths["value"] = conditional_value_paths
         conditional_target_paths = (
             conditional_target_paths if conditional_target_paths else None
         )
-        self._feature_selector._add_single_feature(
+        self._feature_selector._add_feature(
             feature_name=name,
             feature_type=CODED_NUMERICAL,
             target_resource_types=resource_types,
             target_paths=target_paths,
             conditional_target_paths=conditional_target_paths,
+            include_target_names=True,
         )
 
     @property
     def feature_df(self):
         return self._feature_selector.feature_df
 
     def compute_similarities(self, output_dict: bool = False):
```

### Comparing `fhir_analyzer-0.0.6/src/fhir_analyzer/tmp.py` & `fhir_analyzer-0.0.7/src/fhir_analyzer/tmp.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 import sys
 from fhir_analyzer.fhirstore import Fhirstore
 from fhir_analyzer.feature_selector import FeatureSelector
 
-print(sys.path)
 from fhir_analyzer.patient_similarity.patsim import Patsim
 import json
 import os
 
-print(os.getcwd())
-
 ex = {
     "resourceType": "Observation",
     "id": "f9c5653f-a8c8-4c07-89d9-e7e66dcce4c8",
     "status": "final",
     "category": [
         {
             "coding": [
@@ -96,18 +93,15 @@
 ) as f:
     bundle = json.load(f)
     patsim.add_bundle(bundle)
     fhs.add_bundle(bundle)
 
 
 fs = FeatureSelector(fhirstore=fhs)
-fs._add_single_feature(
-    "he", "categorical_string", ["Patient"], {"name": ["name.given"]}
-)
-print("############", fs._patient_features)
+fs._add_feature("he", "categorical_string", ["Patient"], {"name": ["name.given"]})
 
 patsim.add_categorical_feature(
     name="Diagnoses",
     resource_types=["Condition"],
     target_paths=["code.coding.display"],
 )
 
@@ -125,14 +119,23 @@
 
 patsim.add_numerical_feature(
     name="Age",
     resource_types=["Patient"],
     target_paths=["age"],
 )
 
+fs = FeatureSelector(fhirstore=fhs)
+fs.add_feature(
+    name="Name",
+    resource_types=["Patient"],
+    target_paths=["name.given"],
+)
 
-print("patient features: ", patsim._feature_selector._patient_features)
+fs.add_feature(
+    name="Diagnoses",
+    resource_types=["Condition"],
+    target_paths=["code.coding.display"],
+)
 
-sim_df = patsim.compute_similarities()
 
-sim_df["Diagnoses"].to_csv("sim_df.csv")
-patsim.feature_df.to_csv("feature_df.csv")
+print(fs._patient_features)
+print(fs.feature_df)
```

### Comparing `fhir_analyzer-0.0.6/src/fhir_analyzer.egg-info/SOURCES.txt` & `fhir_analyzer-0.0.7/src/fhir_analyzer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

