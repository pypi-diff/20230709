# Comparing `tmp/fhir_kindling-1.0.0a8.tar.gz` & `tmp/fhir_kindling-1.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fhir_kindling-1.0.0a8.tar", max compression
+gzip compressed data, was "fhir_kindling-1.0.0a9.tar", max compression
```

## Comparing `fhir_kindling-1.0.0a8.tar` & `fhir_kindling-1.0.0a9.tar`

### file list

```diff
@@ -1,55 +1,56 @@
--rwxr-xr-x   0        0        0     1071 2023-03-04 09:55:34.447847 fhir_kindling-1.0.0a8/LICENSE
--rwxr-xr-x   0        0        0    10041 2023-04-15 20:16:55.060230 fhir_kindling-1.0.0a8/README.md
--rwxr-xr-x   0        0        0      133 2023-05-31 12:10:59.853995 fhir_kindling-1.0.0a8/fhir_kindling/__init__.py
--rw-r--r--   0        0        0       53 2023-06-12 10:41:39.764673 fhir_kindling-1.0.0a8/fhir_kindling/benchmark/__init__.py
--rw-r--r--   0        0        0     9251 2023-06-12 10:41:39.764673 fhir_kindling-1.0.0a8/fhir_kindling/benchmark/bench.py
--rw-r--r--   0        0        0     3435 2023-06-12 10:41:39.764673 fhir_kindling-1.0.0a8/fhir_kindling/benchmark/constants.py
--rw-r--r--   0        0        0     8695 2023-06-12 10:41:39.764673 fhir_kindling-1.0.0a8/fhir_kindling/benchmark/data.py
--rw-r--r--   0        0        0     3251 2023-06-12 10:41:39.764673 fhir_kindling-1.0.0a8/fhir_kindling/benchmark/figures.py
--rw-r--r--   0        0        0     1774 2023-06-12 10:41:39.764673 fhir_kindling-1.0.0a8/fhir_kindling/benchmark/results.py
--rwxr-xr-x   0        0        0      268 2023-03-23 12:51:15.067324 fhir_kindling-1.0.0a8/fhir_kindling/fhir_query/__init__.py
--rwxr-xr-x   0        0        0    13598 2023-06-12 10:41:39.764673 fhir_kindling-1.0.0a8/fhir_kindling/fhir_query/base.py
--rwxr-xr-x   0        0        0     9968 2023-03-23 11:28:17.585436 fhir_kindling-1.0.0a8/fhir_kindling/fhir_query/query_async.py
--rwxr-xr-x   0        0        0    10919 2023-03-23 00:16:03.459242 fhir_kindling-1.0.0a8/fhir_kindling/fhir_query/query_parameters.py
--rwxr-xr-x   0        0        0     7939 2023-05-31 12:10:59.853995 fhir_kindling-1.0.0a8/fhir_kindling/fhir_query/query_response.py
--rwxr-xr-x   0        0        0     9972 2023-03-23 12:51:14.937324 fhir_kindling-1.0.0a8/fhir_kindling/fhir_query/query_sync.py
--rwxr-xr-x   0        0        0       36 2023-05-31 12:10:59.853995 fhir_kindling-1.0.0a8/fhir_kindling/fhir_server/__init__.py
--rwxr-xr-x   0        0        0     3936 2023-03-23 00:16:03.319242 fhir_kindling-1.0.0a8/fhir_kindling/fhir_server/auth.py
--rwxr-xr-x   0        0        0    35574 2023-05-31 12:10:59.853995 fhir_kindling-1.0.0a8/fhir_kindling/fhir_server/fhir_server.py
--rwxr-xr-x   0        0        0     3736 2023-03-23 00:47:12.807135 fhir_kindling-1.0.0a8/fhir_kindling/fhir_server/server_responses.py
--rwxr-xr-x   0        0        0     2610 2023-03-09 17:53:02.501330 fhir_kindling-1.0.0a8/fhir_kindling/fhir_server/summary.py
--rwxr-xr-x   0        0        0     5700 2023-03-05 09:03:52.925391 fhir_kindling-1.0.0a8/fhir_kindling/fhir_server/transactions.py
--rwxr-xr-x   0        0        0     8894 2023-06-12 10:41:39.764673 fhir_kindling-1.0.0a8/fhir_kindling/fhir_server/transfer.py
--rwxr-xr-x   0        0        0       89 2023-03-04 09:55:34.717848 fhir_kindling-1.0.0a8/fhir_kindling/figures/__init__.py
--rwxr-xr-x   0        0        0     1240 2023-03-04 09:55:34.717848 fhir_kindling-1.0.0a8/fhir_kindling/figures/resource_plots.py
--rwxr-xr-x   0        0        0      759 2023-03-04 09:55:34.717848 fhir_kindling-1.0.0a8/fhir_kindling/figures/summary.py
--rwxr-xr-x   0        0        0      203 2023-03-04 09:55:34.717848 fhir_kindling-1.0.0a8/fhir_kindling/generators/__init__.py
--rw-r--r--   0        0        0      174 2023-06-12 10:41:39.764673 fhir_kindling-1.0.0a8/fhir_kindling/generators/base.py
--rwxr-xr-x   0        0        0    20029 2023-06-12 10:41:39.764673 fhir_kindling-1.0.0a8/fhir_kindling/generators/dataset.py
--rwxr-xr-x   0        0        0     1530 2023-03-04 09:55:34.717848 fhir_kindling-1.0.0a8/fhir_kindling/generators/field_generator.py
--rwxr-xr-x   0        0        0     4860 2023-06-12 10:41:39.764673 fhir_kindling-1.0.0a8/fhir_kindling/generators/patient.py
--rwxr-xr-x   0        0        0     8165 2023-06-12 10:41:39.764673 fhir_kindling-1.0.0a8/fhir_kindling/generators/resource_generator.py
--rw-r--r--   0        0        0     5924 2023-06-12 10:41:39.764673 fhir_kindling-1.0.0a8/fhir_kindling/generators/time_series_generator.py
--rwxr-xr-x   0        0        0        0 2023-03-04 09:55:34.727848 fhir_kindling-1.0.0a8/fhir_kindling/privacy/__init__.py
--rwxr-xr-x   0        0        0     3774 2023-03-04 09:55:34.727848 fhir_kindling-1.0.0a8/fhir_kindling/privacy/k_anonymity.py
--rwxr-xr-x   0        0        0      103 2023-06-12 10:41:39.764673 fhir_kindling-1.0.0a8/fhir_kindling/serde/__init__.py
--rwxr-xr-x   0        0        0     4128 2023-03-04 09:55:34.727848 fhir_kindling-1.0.0a8/fhir_kindling/serde/flatten.py
--rwxr-xr-x   0        0        0      404 2023-03-04 09:55:34.727848 fhir_kindling-1.0.0a8/fhir_kindling/serde/json.py
--rwxr-xr-x   0        0        0        0 2023-03-04 09:55:34.727848 fhir_kindling-1.0.0a8/fhir_kindling/tests/__init__.py
--rwxr-xr-x   0        0        0      588 2023-03-04 09:55:34.727848 fhir_kindling-1.0.0a8/fhir_kindling/tests/conftest.py
--rwxr-xr-x   0        0        0        0 2023-03-05 13:00:06.671372 fhir_kindling-1.0.0a8/fhir_kindling/tests/server/__init__.py
--rwxr-xr-x   0        0        0     1078 2023-03-23 00:47:12.807135 fhir_kindling-1.0.0a8/fhir_kindling/tests/server/test_transfer.py
--rwxr-xr-x   0        0        0     1482 2023-03-04 09:55:34.727848 fhir_kindling-1.0.0a8/fhir_kindling/tests/test_auth.py
--rw-r--r--   0        0        0      419 2023-06-12 10:41:39.764673 fhir_kindling-1.0.0a8/fhir_kindling/tests/test_benchmark.py
--rwxr-xr-x   0        0        0    55630 2023-03-05 18:48:17.265068 fhir_kindling-1.0.0a8/fhir_kindling/tests/test_fhir_query.py
--rwxr-xr-x   0        0        0    21796 2023-05-23 15:03:19.828369 fhir_kindling-1.0.0a8/fhir_kindling/tests/test_fhir_server.py
--rwxr-xr-x   0        0        0    10914 2023-06-12 10:41:39.764673 fhir_kindling-1.0.0a8/fhir_kindling/tests/test_generators.py
--rwxr-xr-x   0        0        0     1115 2023-03-04 09:55:34.727848 fhir_kindling-1.0.0a8/fhir_kindling/tests/test_plots.py
--rwxr-xr-x   0        0        0     1024 2023-03-04 09:55:34.727848 fhir_kindling-1.0.0a8/fhir_kindling/tests/test_privacy.py
--rwxr-xr-x   0        0        0     2082 2023-05-31 12:10:59.853995 fhir_kindling-1.0.0a8/fhir_kindling/tests/test_serialization.py
--rwxr-xr-x   0        0        0     4736 2023-06-12 10:41:39.764673 fhir_kindling-1.0.0a8/fhir_kindling/tests/test_util.py
--rwxr-xr-x   0        0        0       43 2023-03-04 09:55:34.727848 fhir_kindling-1.0.0a8/fhir_kindling/util/__init__.py
--rwxr-xr-x   0        0        0     4466 2023-03-23 00:16:03.399242 fhir_kindling-1.0.0a8/fhir_kindling/util/references.py
--rwxr-xr-x   0        0        0     1876 2023-03-04 09:55:34.727848 fhir_kindling-1.0.0a8/fhir_kindling/util/resources.py
--rwxr-xr-x   0        0        0     2716 2023-06-12 10:41:39.764673 fhir_kindling-1.0.0a8/pyproject.toml
--rw-r--r--   0        0        0    11758 1970-01-01 00:00:00.000000 fhir_kindling-1.0.0a8/PKG-INFO
+-rw-r--r--   0        0        0      133 2023-05-19 08:12:30.473185 fhir_kindling-1.0.0a9/fhir_kindling/__init__.py
+-rw-r--r--   0        0        0       53 2023-06-12 10:49:45.354737 fhir_kindling-1.0.0a9/fhir_kindling/benchmark/__init__.py
+-rw-r--r--   0        0        0    13487 2023-06-14 11:50:22.471355 fhir_kindling-1.0.0a9/fhir_kindling/benchmark/bench.py
+-rw-r--r--   0        0        0     3435 2023-06-12 10:49:45.363362 fhir_kindling-1.0.0a9/fhir_kindling/benchmark/constants.py
+-rw-r--r--   0        0        0     8695 2023-06-12 10:49:45.363362 fhir_kindling-1.0.0a9/fhir_kindling/benchmark/data.py
+-rw-r--r--   0        0        0     3282 2023-06-13 21:22:44.886849 fhir_kindling-1.0.0a9/fhir_kindling/benchmark/figures.py
+-rw-r--r--   0        0        0     3957 2023-06-13 21:33:50.321717 fhir_kindling-1.0.0a9/fhir_kindling/benchmark/results.py
+-rw-r--r--   0        0        0      268 2023-05-19 08:12:30.487218 fhir_kindling-1.0.0a9/fhir_kindling/fhir_query/__init__.py
+-rw-r--r--   0        0        0    13598 2023-06-12 10:49:45.376260 fhir_kindling-1.0.0a9/fhir_kindling/fhir_query/base.py
+-rw-r--r--   0        0        0     9710 2023-05-19 08:12:30.488696 fhir_kindling-1.0.0a9/fhir_kindling/fhir_query/query_async.py
+-rw-r--r--   0        0        0    10919 2023-05-19 08:12:30.489704 fhir_kindling-1.0.0a9/fhir_kindling/fhir_query/query_parameters.py
+-rw-r--r--   0        0        0     7939 2023-05-19 08:12:30.490712 fhir_kindling-1.0.0a9/fhir_kindling/fhir_query/query_response.py
+-rw-r--r--   0        0        0     9714 2023-05-19 08:12:30.491709 fhir_kindling-1.0.0a9/fhir_kindling/fhir_query/query_sync.py
+-rw-r--r--   0        0        0       36 2023-05-19 08:12:30.494722 fhir_kindling-1.0.0a9/fhir_kindling/fhir_server/__init__.py
+-rw-r--r--   0        0        0     3936 2023-05-19 08:12:30.495707 fhir_kindling-1.0.0a9/fhir_kindling/fhir_server/auth.py
+-rw-r--r--   0        0        0    35574 2023-06-13 12:00:27.891209 fhir_kindling-1.0.0a9/fhir_kindling/fhir_server/fhir_server.py
+-rw-r--r--   0        0        0     3736 2023-05-19 08:12:30.497707 fhir_kindling-1.0.0a9/fhir_kindling/fhir_server/server_responses.py
+-rw-r--r--   0        0        0     2610 2023-05-19 08:12:30.498706 fhir_kindling-1.0.0a9/fhir_kindling/fhir_server/summary.py
+-rw-r--r--   0        0        0     5712 2023-06-14 14:25:16.269949 fhir_kindling-1.0.0a9/fhir_kindling/fhir_server/transactions.py
+-rw-r--r--   0        0        0     8894 2023-06-12 10:49:45.379382 fhir_kindling-1.0.0a9/fhir_kindling/fhir_server/transfer.py
+-rw-r--r--   0        0        0       89 2023-05-19 08:12:30.503726 fhir_kindling-1.0.0a9/fhir_kindling/figures/__init__.py
+-rw-r--r--   0        0        0     1240 2023-05-19 08:12:30.507717 fhir_kindling-1.0.0a9/fhir_kindling/figures/resource_plots.py
+-rw-r--r--   0        0        0      759 2023-05-19 08:12:30.507717 fhir_kindling-1.0.0a9/fhir_kindling/figures/summary.py
+-rw-r--r--   0        0        0      203 2023-05-19 08:12:30.512721 fhir_kindling-1.0.0a9/fhir_kindling/generators/__init__.py
+-rw-r--r--   0        0        0      174 2023-06-12 10:49:45.379382 fhir_kindling-1.0.0a9/fhir_kindling/generators/base.py
+-rw-r--r--   0        0        0    20029 2023-06-12 10:49:45.379382 fhir_kindling-1.0.0a9/fhir_kindling/generators/dataset.py
+-rw-r--r--   0        0        0     1530 2023-05-19 08:12:30.517471 fhir_kindling-1.0.0a9/fhir_kindling/generators/field_generator.py
+-rw-r--r--   0        0        0     5019 2023-06-14 14:22:42.586944 fhir_kindling-1.0.0a9/fhir_kindling/generators/patient.py
+-rw-r--r--   0        0        0     8165 2023-06-12 10:49:45.386430 fhir_kindling-1.0.0a9/fhir_kindling/generators/resource_generator.py
+-rw-r--r--   0        0        0     5924 2023-06-12 10:49:45.386430 fhir_kindling-1.0.0a9/fhir_kindling/generators/time_series_generator.py
+-rw-r--r--   0        0        0        0 2023-05-19 08:12:30.520468 fhir_kindling-1.0.0a9/fhir_kindling/privacy/__init__.py
+-rw-r--r--   0        0        0     3774 2023-05-19 08:12:30.522454 fhir_kindling-1.0.0a9/fhir_kindling/privacy/k_anonymity.py
+-rw-r--r--   0        0        0      103 2023-06-12 10:49:45.386430 fhir_kindling-1.0.0a9/fhir_kindling/serde/__init__.py
+-rw-r--r--   0        0        0     4128 2023-05-19 08:12:30.524150 fhir_kindling-1.0.0a9/fhir_kindling/serde/flatten.py
+-rw-r--r--   0        0        0      404 2023-05-19 08:12:30.524150 fhir_kindling-1.0.0a9/fhir_kindling/serde/json.py
+-rw-r--r--   0        0        0        0 2023-05-19 08:12:30.524150 fhir_kindling-1.0.0a9/fhir_kindling/tests/__init__.py
+-rw-r--r--   0        0        0      588 2023-05-19 08:12:30.524150 fhir_kindling-1.0.0a9/fhir_kindling/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-19 08:12:30.524150 fhir_kindling-1.0.0a9/fhir_kindling/tests/server/__init__.py
+-rw-r--r--   0        0        0     1031 2023-06-14 12:08:09.888924 fhir_kindling-1.0.0a9/fhir_kindling/tests/server/test_transfer.py
+-rw-r--r--   0        0        0     1482 2023-05-19 08:12:30.539605 fhir_kindling-1.0.0a9/fhir_kindling/tests/test_auth.py
+-rw-r--r--   0        0        0      459 2023-06-14 14:28:11.503574 fhir_kindling-1.0.0a9/fhir_kindling/tests/test_benchmark.py
+-rw-r--r--   0        0        0    55630 2023-05-19 08:12:30.544612 fhir_kindling-1.0.0a9/fhir_kindling/tests/test_fhir_query.py
+-rw-r--r--   0        0        0    21796 2023-05-19 08:12:30.547611 fhir_kindling-1.0.0a9/fhir_kindling/tests/test_fhir_server.py
+-rw-r--r--   0        0        0    11123 2023-06-14 14:35:25.368258 fhir_kindling-1.0.0a9/fhir_kindling/tests/test_generators.py
+-rw-r--r--   0        0        0     1115 2023-05-19 08:12:30.555603 fhir_kindling-1.0.0a9/fhir_kindling/tests/test_plots.py
+-rw-r--r--   0        0        0     1024 2023-05-19 08:12:30.560617 fhir_kindling-1.0.0a9/fhir_kindling/tests/test_privacy.py
+-rw-r--r--   0        0        0     2082 2023-05-19 08:12:30.561622 fhir_kindling-1.0.0a9/fhir_kindling/tests/test_serialization.py
+-rw-r--r--   0        0        0     4810 2023-06-14 14:36:36.060848 fhir_kindling-1.0.0a9/fhir_kindling/tests/test_util.py
+-rw-r--r--   0        0        0       43 2023-05-19 08:12:30.563624 fhir_kindling-1.0.0a9/fhir_kindling/util/__init__.py
+-rw-r--r--   0        0        0     4466 2023-05-19 08:12:30.564618 fhir_kindling-1.0.0a9/fhir_kindling/util/references.py
+-rw-r--r--   0        0        0     1876 2023-05-19 08:12:30.565631 fhir_kindling-1.0.0a9/fhir_kindling/util/resources.py
+-rw-r--r--   0        0        0     1071 2023-05-19 08:12:30.422025 fhir_kindling-1.0.0a9/LICENSE
+-rw-r--r--   0        0        0     2788 2023-06-16 07:51:35.400997 fhir_kindling-1.0.0a9/pyproject.toml
+-rw-r--r--   0        0        0    10041 2023-05-19 08:12:30.422025 fhir_kindling-1.0.0a9/README.md
+-rw-r--r--   0        0        0    11720 1970-01-01 00:00:00.000000 fhir_kindling-1.0.0a9/setup.py
+-rw-r--r--   0        0        0    11826 1970-01-01 00:00:00.000000 fhir_kindling-1.0.0a9/PKG-INFO
```

### Comparing `fhir_kindling-1.0.0a8/LICENSE` & `fhir_kindling-1.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a8/README.md` & `fhir_kindling-1.0.0a9/README.md`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a8/fhir_kindling/benchmark/constants.py` & `fhir_kindling-1.0.0a9/fhir_kindling/benchmark/constants.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a8/fhir_kindling/benchmark/data.py` & `fhir_kindling-1.0.0a9/fhir_kindling/benchmark/data.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a8/fhir_kindling/benchmark/figures.py` & `fhir_kindling-1.0.0a9/fhir_kindling/benchmark/figures.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,14 +75,15 @@
     Args:
         fig: _description_
         results: _description_
     """
     ds_fig = go.Bar(
         y=list(results.dataset_insert.values()),
         x=list(results.dataset_insert.keys()),
+        name="Dataset Insert",
     )
     fig.add_trace(ds_fig, row=3, col=1)
 
 
 def add_query_traces(fig: go.Figure, results: "BenchmarkResults"):
     query_results = results.query
     queries = list(list(query_results.values())[0].keys())
```

### Comparing `fhir_kindling-1.0.0a8/fhir_kindling/fhir_query/base.py` & `fhir_kindling-1.0.0a9/fhir_kindling/fhir_query/base.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a8/fhir_kindling/fhir_query/query_async.py` & `fhir_kindling-1.0.0a9/fhir_kindling/fhir_query/query_async.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,258 +1,258 @@
-from typing import Any, Callable, List, Union
-
-import fhir.resources
-import httpx
-import orjson
-import xmltodict
-from fhir.resources import FHIRAbstractModel
-from fhir.resources.fhirresourcemodel import FHIRResourceModel
-
-from fhir_kindling.fhir_query.base import FhirQueryBase
-from fhir_kindling.fhir_query.query_parameters import (
-    FhirQueryParameters,
-)
-from fhir_kindling.fhir_query.query_response import (
-    OutputFormats,
-    QueryResponse,
-    ResponseStatusCodes,
-)
-
-
-class FhirQueryAsync(FhirQueryBase):
-    def __init__(
-        self,
-        base_url: str,
-        resource: Union[
-            FHIRResourceModel, fhir.resources.FHIRAbstractModel, str
-        ] = None,
-        query_parameters: FhirQueryParameters = None,
-        auth: httpx.Auth = None,
-        headers: dict = None,
-        output_format: str = "json",
-        client: httpx.AsyncClient = None,
-        proxies: Union[str, dict] = None,
-    ):
-        super().__init__(
-            base_url, resource, query_parameters, auth, headers, output_format
-        )
-        self.proxies = proxies
-        # set up the async client instance
-        self.client = None
-        if client:
-            self.client = client
-        else:
-            self._setup_client()
-
-    async def all(
-        self,
-        page_callback: Union[
-            Callable[[List[FHIRAbstractModel]], Any], Callable[[], Any], None
-        ] = None,
-        count: int = None,
-    ) -> QueryResponse:
-        """
-        Execute the query and return all results matching the query parameters.
-
-        Args:
-            page_callback: if this argument is set the given callback function will be called for each page of results
-            count: number of results in a page, default value of 50 is used when page_callback is set but no count is
-        Returns:
-            QueryResponse object containing all resources matching the query, as well os optional included
-            resources.
-
-        """
-        self._limit = None
-        self._count = count
-        response = await self._execute_query(page_callback=page_callback, count=count)
-        return response
-
-    async def limit(
-        self,
-        n: int,
-        page_callback: Union[
-            Callable[[List[FHIRAbstractModel]], Any], Callable[[], Any], None
-        ] = None,
-        count: int = None,
-    ) -> QueryResponse:
-        """
-        Execute the query and return the first n results matching the query parameters.
-        Args:
-            n: number of resources to return
-            page_callback: if this argument is set the given callback function will be called for each page of results
-            count: number of results in a page, default value of 50 is used when page_callback is set but no count is
-
-        Returns:
-            QueryResponse object containing the first n resources matching the query, as well os optional included
-            resources.
-
-        """
-        self._limit = n
-        self._count = count
-        response = await self._execute_query(page_callback=page_callback, count=count)
-        return response
-
-    async def first(self) -> QueryResponse:
-        """
-        Return the first resource matching the query parameters.
-        Returns:
-            QueryResponse object containing the first resource matching the query
-
-        """
-        self._limit = 1
-        response = await self._execute_query(count=1)
-        return response
-
-    async def count(self) -> int:
-        """
-        Return the number of resources matching the query parameters.
-        Returns:
-            number of resources matching the query
-
-        """
-
-        response = await self.client.get(self.query_url + "&_summary=count")
-        response.raise_for_status()
-        return response.json()["total"]
-
-    def _setup_client(self):
-        headers = self.headers if self.headers else {}
-        headers["Content-Type"] = "application/fhir+json"
-        self.client = httpx.AsyncClient(auth=self.auth, headers=headers, timeout=None)
-
-    async def _execute_query(
-        self,
-        page_callback: Union[
-            Callable[[List[FHIRAbstractModel]], Any], Callable[[], Any], None
-        ] = None,
-        count: int = None,
-    ) -> QueryResponse:
-        r = await self.client.get(self.query_url)
-        r.raise_for_status()
-        response = await self._resolve_response_pagination(r, page_callback, count)
-        return response
-
-    async def _resolve_response_pagination(
-        self,
-        initial_response: httpx.Response,
-        page_callback: Union[
-            Callable[[List[FHIRAbstractModel]], Any], Callable[[], Any], None
-        ] = None,
-        count: int = None,
-    ) -> QueryResponse:
-        if self.output_format == OutputFormats.JSON:
-            response = await self._resolve_json_pagination(
-                initial_response, page_callback, count
-            )
-
-        else:
-            response = await self._resolve_xml_pagination(initial_response)
-
-        return QueryResponse(
-            response=response,
-            query_params=self.query_parameters,
-            count=count,
-            limit=self._limit,
-            output_format=self.output_format,
-        )
-
-    async def _resolve_json_pagination(
-        self,
-        initial_response: httpx.Response,
-        page_callback: Union[
-            Callable[[List[FHIRAbstractModel]], Any], Callable[[], Any], None
-        ] = None,
-        count: int = None,
-    ) -> dict:
-        response_json = orjson.loads(initial_response.content)
-        link = response_json.get("link", None)
-        # If there is a link, get the next page otherwise return the response
-        if not link:
-            self.status_code = ResponseStatusCodes.OK
-            return response_json
-        else:
-            entries = []
-            initial_entry = response_json.get("entry", None)
-            if not initial_entry:
-                self.status_code = ResponseStatusCodes.NOT_FOUND
-                return response_json
-            else:
-                self.status_code = ResponseStatusCodes.OK
-                response_entries = response_json["entry"]
-                entries.extend(response_entries)
-                self._execute_callback(response_entries, page_callback)
-            # if the limit is reached, stop resolving the pagination
-            if self._limit and len(entries) >= self._limit:
-                response_entries = response_json["entry"][: self._limit]
-                response_json["entry"] = response_entries
-                self._execute_callback(response_entries, page_callback)
-                return response_json
-            # query the linked page and add the entries to the response
-            while response_json.get("link", None):
-                if self._limit and len(entries) >= self._limit:
-                    break
-                next_page = next(
-                    (
-                        link
-                        for link in response_json["link"]
-                        if link.get("relation", None) == "next"
-                    ),
-                    None,
-                )
-                if next_page:
-                    page_response = await self.client.get(next_page["url"])
-                    response_json = page_response.json()
-                    response_entries = response_json["entry"]
-                    entries.extend(response_entries)
-                    self._execute_callback(response_entries, page_callback)
-                else:
-                    break
-
-            response_json["entry"] = entries[: self._limit] if self._limit else entries
-            return response_json
-
-    async def _resolve_xml_pagination(self, server_response: httpx.Response) -> str:
-        # parse the xml response and extract the initial entries
-        initial_response = xmltodict.parse(server_response.text)
-        entries = initial_response["Bundle"].get("entry")
-
-        # if there are no entries, return the initial response
-        if not entries:
-            self.status_code = ResponseStatusCodes.NOT_FOUND
-            print(
-                f"No resources match the query - query url: {self.query_parameters.to_query_string()}"
-            )
-            return server_response.text
-        else:
-            self.status_code = ResponseStatusCodes.OK
-        response = initial_response
-        # resolve the pagination
-        while True:
-            next_page = False
-            for link in response["Bundle"]["link"]:
-                # if there is a next page, get the next page
-                if not isinstance(link, dict):
-                    break
-                relation_dict = link.get("relation", None)
-                if relation_dict.get("@value") == "next":
-                    # get url and extend with xml format
-                    url = link["url"]["@value"]
-                    url = url + "&_format=xml"
-                    r = await self.client.get(url)
-                    r.raise_for_status()
-                    response = xmltodict.parse(r.text)
-                    added_entries = response["Bundle"]["entry"]
-                    entries.extend(added_entries)
-                    # Stop resolving the pagination when the limit is reached
-                    if self._limit:
-                        next_page = len(entries) < self._limit
-                    else:
-                        next_page = True
-
-            if not next_page:
-                break
-        # added the paginated resources to the initial response
-        initial_response["Bundle"]["entry"] = (
-            entries[: self._limit] if self._limit else entries
-        )
-        full_response_xml = xmltodict.unparse(initial_response, pretty=True)
-        return full_response_xml
+from typing import Any, Callable, List, Union
+
+import fhir.resources
+import httpx
+import orjson
+import xmltodict
+from fhir.resources import FHIRAbstractModel
+from fhir.resources.fhirresourcemodel import FHIRResourceModel
+
+from fhir_kindling.fhir_query.base import FhirQueryBase
+from fhir_kindling.fhir_query.query_parameters import (
+    FhirQueryParameters,
+)
+from fhir_kindling.fhir_query.query_response import (
+    OutputFormats,
+    QueryResponse,
+    ResponseStatusCodes,
+)
+
+
+class FhirQueryAsync(FhirQueryBase):
+    def __init__(
+        self,
+        base_url: str,
+        resource: Union[
+            FHIRResourceModel, fhir.resources.FHIRAbstractModel, str
+        ] = None,
+        query_parameters: FhirQueryParameters = None,
+        auth: httpx.Auth = None,
+        headers: dict = None,
+        output_format: str = "json",
+        client: httpx.AsyncClient = None,
+        proxies: Union[str, dict] = None,
+    ):
+        super().__init__(
+            base_url, resource, query_parameters, auth, headers, output_format
+        )
+        self.proxies = proxies
+        # set up the async client instance
+        self.client = None
+        if client:
+            self.client = client
+        else:
+            self._setup_client()
+
+    async def all(
+        self,
+        page_callback: Union[
+            Callable[[List[FHIRAbstractModel]], Any], Callable[[], Any], None
+        ] = None,
+        count: int = None,
+    ) -> QueryResponse:
+        """
+        Execute the query and return all results matching the query parameters.
+
+        Args:
+            page_callback: if this argument is set the given callback function will be called for each page of results
+            count: number of results in a page, default value of 50 is used when page_callback is set but no count is
+        Returns:
+            QueryResponse object containing all resources matching the query, as well os optional included
+            resources.
+
+        """
+        self._limit = None
+        self._count = count
+        response = await self._execute_query(page_callback=page_callback, count=count)
+        return response
+
+    async def limit(
+        self,
+        n: int,
+        page_callback: Union[
+            Callable[[List[FHIRAbstractModel]], Any], Callable[[], Any], None
+        ] = None,
+        count: int = None,
+    ) -> QueryResponse:
+        """
+        Execute the query and return the first n results matching the query parameters.
+        Args:
+            n: number of resources to return
+            page_callback: if this argument is set the given callback function will be called for each page of results
+            count: number of results in a page, default value of 50 is used when page_callback is set but no count is
+
+        Returns:
+            QueryResponse object containing the first n resources matching the query, as well os optional included
+            resources.
+
+        """
+        self._limit = n
+        self._count = count
+        response = await self._execute_query(page_callback=page_callback, count=count)
+        return response
+
+    async def first(self) -> QueryResponse:
+        """
+        Return the first resource matching the query parameters.
+        Returns:
+            QueryResponse object containing the first resource matching the query
+
+        """
+        self._limit = 1
+        response = await self._execute_query(count=1)
+        return response
+
+    async def count(self) -> int:
+        """
+        Return the number of resources matching the query parameters.
+        Returns:
+            number of resources matching the query
+
+        """
+
+        response = await self.client.get(self.query_url + "&_summary=count")
+        response.raise_for_status()
+        return response.json()["total"]
+
+    def _setup_client(self):
+        headers = self.headers if self.headers else {}
+        headers["Content-Type"] = "application/fhir+json"
+        self.client = httpx.AsyncClient(auth=self.auth, headers=headers, timeout=None)
+
+    async def _execute_query(
+        self,
+        page_callback: Union[
+            Callable[[List[FHIRAbstractModel]], Any], Callable[[], Any], None
+        ] = None,
+        count: int = None,
+    ) -> QueryResponse:
+        r = await self.client.get(self.query_url)
+        r.raise_for_status()
+        response = await self._resolve_response_pagination(r, page_callback, count)
+        return response
+
+    async def _resolve_response_pagination(
+        self,
+        initial_response: httpx.Response,
+        page_callback: Union[
+            Callable[[List[FHIRAbstractModel]], Any], Callable[[], Any], None
+        ] = None,
+        count: int = None,
+    ) -> QueryResponse:
+        if self.output_format == OutputFormats.JSON:
+            response = await self._resolve_json_pagination(
+                initial_response, page_callback, count
+            )
+
+        else:
+            response = await self._resolve_xml_pagination(initial_response)
+
+        return QueryResponse(
+            response=response,
+            query_params=self.query_parameters,
+            count=count,
+            limit=self._limit,
+            output_format=self.output_format,
+        )
+
+    async def _resolve_json_pagination(
+        self,
+        initial_response: httpx.Response,
+        page_callback: Union[
+            Callable[[List[FHIRAbstractModel]], Any], Callable[[], Any], None
+        ] = None,
+        count: int = None,
+    ) -> dict:
+        response_json = orjson.loads(initial_response.content)
+        link = response_json.get("link", None)
+        # If there is a link, get the next page otherwise return the response
+        if not link:
+            self.status_code = ResponseStatusCodes.OK
+            return response_json
+        else:
+            entries = []
+            initial_entry = response_json.get("entry", None)
+            if not initial_entry:
+                self.status_code = ResponseStatusCodes.NOT_FOUND
+                return response_json
+            else:
+                self.status_code = ResponseStatusCodes.OK
+                response_entries = response_json["entry"]
+                entries.extend(response_entries)
+                self._execute_callback(response_entries, page_callback)
+            # if the limit is reached, stop resolving the pagination
+            if self._limit and len(entries) >= self._limit:
+                response_entries = response_json["entry"][: self._limit]
+                response_json["entry"] = response_entries
+                self._execute_callback(response_entries, page_callback)
+                return response_json
+            # query the linked page and add the entries to the response
+            while response_json.get("link", None):
+                if self._limit and len(entries) >= self._limit:
+                    break
+                next_page = next(
+                    (
+                        link
+                        for link in response_json["link"]
+                        if link.get("relation", None) == "next"
+                    ),
+                    None,
+                )
+                if next_page:
+                    page_response = await self.client.get(next_page["url"])
+                    response_json = page_response.json()
+                    response_entries = response_json["entry"]
+                    entries.extend(response_entries)
+                    self._execute_callback(response_entries, page_callback)
+                else:
+                    break
+
+            response_json["entry"] = entries[: self._limit] if self._limit else entries
+            return response_json
+
+    async def _resolve_xml_pagination(self, server_response: httpx.Response) -> str:
+        # parse the xml response and extract the initial entries
+        initial_response = xmltodict.parse(server_response.text)
+        entries = initial_response["Bundle"].get("entry")
+
+        # if there are no entries, return the initial response
+        if not entries:
+            self.status_code = ResponseStatusCodes.NOT_FOUND
+            print(
+                f"No resources match the query - query url: {self.query_parameters.to_query_string()}"
+            )
+            return server_response.text
+        else:
+            self.status_code = ResponseStatusCodes.OK
+        response = initial_response
+        # resolve the pagination
+        while True:
+            next_page = False
+            for link in response["Bundle"]["link"]:
+                # if there is a next page, get the next page
+                if not isinstance(link, dict):
+                    break
+                relation_dict = link.get("relation", None)
+                if relation_dict.get("@value") == "next":
+                    # get url and extend with xml format
+                    url = link["url"]["@value"]
+                    url = url + "&_format=xml"
+                    r = await self.client.get(url)
+                    r.raise_for_status()
+                    response = xmltodict.parse(r.text)
+                    added_entries = response["Bundle"]["entry"]
+                    entries.extend(added_entries)
+                    # Stop resolving the pagination when the limit is reached
+                    if self._limit:
+                        next_page = len(entries) < self._limit
+                    else:
+                        next_page = True
+
+            if not next_page:
+                break
+        # added the paginated resources to the initial response
+        initial_response["Bundle"]["entry"] = (
+            entries[: self._limit] if self._limit else entries
+        )
+        full_response_xml = xmltodict.unparse(initial_response, pretty=True)
+        return full_response_xml
```

### Comparing `fhir_kindling-1.0.0a8/fhir_kindling/fhir_query/query_parameters.py` & `fhir_kindling-1.0.0a9/fhir_kindling/fhir_query/query_parameters.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a8/fhir_kindling/fhir_query/query_response.py` & `fhir_kindling-1.0.0a9/fhir_kindling/fhir_query/query_response.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a8/fhir_kindling/fhir_query/query_sync.py` & `fhir_kindling-1.0.0a9/fhir_kindling/fhir_query/query_sync.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,258 +1,258 @@
-from typing import Any, Callable, List, Union
-
-import fhir.resources
-import httpx
-import orjson
-import xmltodict
-from fhir.resources import FHIRAbstractModel
-from fhir.resources.fhirresourcemodel import FHIRResourceModel
-
-from fhir_kindling.fhir_query.base import FhirQueryBase
-from fhir_kindling.fhir_query.query_parameters import (
-    FhirQueryParameters,
-)
-from fhir_kindling.fhir_query.query_response import (
-    OutputFormats,
-    QueryResponse,
-    ResponseStatusCodes,
-)
-
-
-class FhirQuerySync(FhirQueryBase):
-    def __init__(
-        self,
-        base_url: str,
-        resource: Union[
-            FHIRResourceModel, fhir.resources.FHIRAbstractModel, str
-        ] = None,
-        query_parameters: FhirQueryParameters = None,
-        auth: httpx.Auth = None,
-        headers: dict = None,
-        client: httpx.Client = None,
-        output_format: str = "json",
-        proxies: Union[str, dict] = None,
-    ):
-        super().__init__(
-            base_url, resource, query_parameters, auth, headers, output_format
-        )
-        self.proxies = proxies
-        if client:
-            self.client = client
-        else:
-            self.client = self._setup_client()
-
-    def all(
-        self,
-        page_callback: Union[
-            Callable[[List[FHIRAbstractModel]], Any], Callable[[], Any], None
-        ] = None,
-        count: int = None,
-    ) -> QueryResponse:
-        """
-        Execute the query and return all results matching the query parameters.
-
-        Args:
-            page_callback: if this argument is set the given callback function will be called for each page of results
-            count: number of results in a page, default value of 50 is used when page_callback is set but no count is
-        Returns:
-            QueryResponse object containing all resources matching the query, as well os optional included
-            resources.
-
-        """
-        self._limit = None
-        self._count = count
-        return self._execute_query(page_callback=page_callback, count=count)
-
-    def limit(
-        self,
-        n: int,
-        page_callback: Union[
-            Callable[[List[FHIRAbstractModel]], Any], Callable[[], Any], None
-        ] = None,
-        count: int = None,
-    ) -> QueryResponse:
-        """
-        Execute the query and return the first n results matching the query parameters.
-        Args:
-            n: number of resources to return
-            page_callback: if this argument is set the given callback function will be called for each page of results
-            count: number of results in a page, default value of 50 is used when page_callback is set but no count is
-
-        Returns:
-            QueryResponse object containing the first n resources matching the query, as well os optional included
-            resources.
-
-        """
-        self._limit = n
-        self._count = count
-        return self._execute_query(page_callback=page_callback, count=count)
-
-    def first(self) -> QueryResponse:
-        """
-        Return the first resource matching the query parameters.
-        Returns:
-            QueryResponse object containing the first resource matching the query
-
-        """
-        self._limit = 1
-        return self._execute_query()
-
-    def count(self) -> int:
-        self._count = 0
-        with self._setup_client() as client:
-            response = client.get(self._make_query_string() + "&_summary=count")
-        response.raise_for_status()
-        return response.json()["total"]
-
-    def _setup_client(self):
-        headers = self.headers if self.headers else {}
-        headers["Content-Type"] = "application/fhir+json"
-        client = httpx.Client(
-            auth=self.auth, headers=headers, proxies=self.proxies, timeout=None
-        )
-        return client
-
-    def _execute_query(
-        self,
-        page_callback: Union[
-            Callable[[List[FHIRAbstractModel]], Any], Callable[[], Any], None
-        ] = None,
-        count: int = None,
-    ) -> QueryResponse:
-        with self._setup_client() as client:
-            r = client.get(self.query_url)
-            r.raise_for_status()
-
-        response = self._resolve_response_pagination(r, page_callback, count)
-        return response
-
-    def _resolve_response_pagination(
-        self,
-        initial_response: httpx.Response,
-        page_callback: Union[
-            Callable[[List[FHIRAbstractModel]], Any], Callable[[], Any], None
-        ] = None,
-        count: int = None,
-    ) -> QueryResponse:
-        if self.output_format == OutputFormats.JSON:
-            response = self._resolve_json_pagination(
-                initial_response, page_callback, count
-            )
-
-        else:
-            response = self._resolve_xml_pagination(initial_response)
-
-        return QueryResponse(
-            response=response,
-            query_params=self.query_parameters,
-            count=count,
-            limit=self._limit,
-            output_format=self.output_format,
-        )
-
-    def _resolve_json_pagination(
-        self,
-        initial_response: httpx.Response,
-        page_callback: Union[
-            Callable[[List[FHIRAbstractModel]], Any], Callable[[], Any], None
-        ] = None,
-        count: int = None,
-    ) -> dict:
-        response_json = orjson.loads(initial_response.content)
-        link = response_json.get("link", None)
-        # If there is a link, get the next page otherwise return the response
-
-        with self._setup_client() as client:
-            if not link:
-                self.status_code = ResponseStatusCodes.OK
-                return response_json
-            else:
-                entries = []
-                initial_entry = response_json.get("entry", None)
-                if not initial_entry:
-                    self.status_code = ResponseStatusCodes.NOT_FOUND
-                    return response_json
-                else:
-                    self.status_code = ResponseStatusCodes.OK
-                    response_entries = response_json["entry"]
-                    entries.extend(response_entries)
-                    self._execute_callback(response_entries, page_callback)
-                # if the limit is reached, stop resolving the pagination
-                if self._limit and len(entries) >= self._limit:
-                    response_entries = response_json["entry"][: self._limit]
-                    response_json["entry"] = response_entries
-                    self._execute_callback(response_entries, page_callback)
-                    return response_json
-                # query the linked page and add the entries to the response
-
-                while response_json.get("link", None):
-                    if self._limit and len(entries) >= self._limit:
-                        break
-                    next_page = next(
-                        (
-                            link
-                            for link in response_json["link"]
-                            if link.get("relation", None) == "next"
-                        ),
-                        None,
-                    )
-                    if next_page:
-                        response_json = client.get(next_page["url"]).json()
-                        response_entries = response_json["entry"]
-                        entries.extend(response_entries)
-                        self._execute_callback(response_entries, page_callback)
-                    else:
-                        break
-
-            response_json["entry"] = entries[: self._limit] if self._limit else entries
-            return response_json
-
-    def _resolve_xml_pagination(self, server_response: httpx.Response) -> str:
-        # parse the xml response and extract the initial entries
-        initial_response = xmltodict.parse(server_response.text)
-        entries = initial_response["Bundle"].get("entry")
-
-        # if there are no entries, return the initial response
-        if not entries:
-            self.status_code = ResponseStatusCodes.NOT_FOUND
-            print(
-                f"No resources match the query - query url: {self.query_parameters.to_query_string()}"
-            )
-            return server_response.text
-        else:
-            self.status_code = ResponseStatusCodes.OK
-        response = initial_response
-        # resolve the pagination
-        while True:
-            next_page = False
-            for link in response["Bundle"]["link"]:
-                # if there is a next page, get the next page
-                if not isinstance(link, dict):
-                    break
-                relation_dict = link.get("relation", None)
-
-                if relation_dict.get("@value") == "next":
-                    # get url and extend with xml format
-                    url = link["url"]["@value"]
-                    url = url + "&_format=xml"
-                    r = self.client.get(url)
-                    r.raise_for_status()
-                    response = xmltodict.parse(r.text)
-                    if not response["Bundle"].get("entry", None):
-                        break
-                    added_entries = response["Bundle"]["entry"]
-                    entries.extend(added_entries)
-                    # Stop resolving the pagination when the limit is reached
-                    if self._limit:
-                        next_page = len(entries) < self._limit
-                    else:
-                        next_page = True
-
-            if not next_page:
-                break
-        # added the paginated resources to the initial response
-        initial_response["Bundle"]["entry"] = (
-            entries[: self._limit] if self._limit else entries
-        )
-        full_response_xml = xmltodict.unparse(initial_response, pretty=True)
-        return full_response_xml
+from typing import Any, Callable, List, Union
+
+import fhir.resources
+import httpx
+import orjson
+import xmltodict
+from fhir.resources import FHIRAbstractModel
+from fhir.resources.fhirresourcemodel import FHIRResourceModel
+
+from fhir_kindling.fhir_query.base import FhirQueryBase
+from fhir_kindling.fhir_query.query_parameters import (
+    FhirQueryParameters,
+)
+from fhir_kindling.fhir_query.query_response import (
+    OutputFormats,
+    QueryResponse,
+    ResponseStatusCodes,
+)
+
+
+class FhirQuerySync(FhirQueryBase):
+    def __init__(
+        self,
+        base_url: str,
+        resource: Union[
+            FHIRResourceModel, fhir.resources.FHIRAbstractModel, str
+        ] = None,
+        query_parameters: FhirQueryParameters = None,
+        auth: httpx.Auth = None,
+        headers: dict = None,
+        client: httpx.Client = None,
+        output_format: str = "json",
+        proxies: Union[str, dict] = None,
+    ):
+        super().__init__(
+            base_url, resource, query_parameters, auth, headers, output_format
+        )
+        self.proxies = proxies
+        if client:
+            self.client = client
+        else:
+            self.client = self._setup_client()
+
+    def all(
+        self,
+        page_callback: Union[
+            Callable[[List[FHIRAbstractModel]], Any], Callable[[], Any], None
+        ] = None,
+        count: int = None,
+    ) -> QueryResponse:
+        """
+        Execute the query and return all results matching the query parameters.
+
+        Args:
+            page_callback: if this argument is set the given callback function will be called for each page of results
+            count: number of results in a page, default value of 50 is used when page_callback is set but no count is
+        Returns:
+            QueryResponse object containing all resources matching the query, as well os optional included
+            resources.
+
+        """
+        self._limit = None
+        self._count = count
+        return self._execute_query(page_callback=page_callback, count=count)
+
+    def limit(
+        self,
+        n: int,
+        page_callback: Union[
+            Callable[[List[FHIRAbstractModel]], Any], Callable[[], Any], None
+        ] = None,
+        count: int = None,
+    ) -> QueryResponse:
+        """
+        Execute the query and return the first n results matching the query parameters.
+        Args:
+            n: number of resources to return
+            page_callback: if this argument is set the given callback function will be called for each page of results
+            count: number of results in a page, default value of 50 is used when page_callback is set but no count is
+
+        Returns:
+            QueryResponse object containing the first n resources matching the query, as well os optional included
+            resources.
+
+        """
+        self._limit = n
+        self._count = count
+        return self._execute_query(page_callback=page_callback, count=count)
+
+    def first(self) -> QueryResponse:
+        """
+        Return the first resource matching the query parameters.
+        Returns:
+            QueryResponse object containing the first resource matching the query
+
+        """
+        self._limit = 1
+        return self._execute_query()
+
+    def count(self) -> int:
+        self._count = 0
+        with self._setup_client() as client:
+            response = client.get(self._make_query_string() + "&_summary=count")
+        response.raise_for_status()
+        return response.json()["total"]
+
+    def _setup_client(self):
+        headers = self.headers if self.headers else {}
+        headers["Content-Type"] = "application/fhir+json"
+        client = httpx.Client(
+            auth=self.auth, headers=headers, proxies=self.proxies, timeout=None
+        )
+        return client
+
+    def _execute_query(
+        self,
+        page_callback: Union[
+            Callable[[List[FHIRAbstractModel]], Any], Callable[[], Any], None
+        ] = None,
+        count: int = None,
+    ) -> QueryResponse:
+        with self._setup_client() as client:
+            r = client.get(self.query_url)
+            r.raise_for_status()
+
+        response = self._resolve_response_pagination(r, page_callback, count)
+        return response
+
+    def _resolve_response_pagination(
+        self,
+        initial_response: httpx.Response,
+        page_callback: Union[
+            Callable[[List[FHIRAbstractModel]], Any], Callable[[], Any], None
+        ] = None,
+        count: int = None,
+    ) -> QueryResponse:
+        if self.output_format == OutputFormats.JSON:
+            response = self._resolve_json_pagination(
+                initial_response, page_callback, count
+            )
+
+        else:
+            response = self._resolve_xml_pagination(initial_response)
+
+        return QueryResponse(
+            response=response,
+            query_params=self.query_parameters,
+            count=count,
+            limit=self._limit,
+            output_format=self.output_format,
+        )
+
+    def _resolve_json_pagination(
+        self,
+        initial_response: httpx.Response,
+        page_callback: Union[
+            Callable[[List[FHIRAbstractModel]], Any], Callable[[], Any], None
+        ] = None,
+        count: int = None,
+    ) -> dict:
+        response_json = orjson.loads(initial_response.content)
+        link = response_json.get("link", None)
+        # If there is a link, get the next page otherwise return the response
+
+        with self._setup_client() as client:
+            if not link:
+                self.status_code = ResponseStatusCodes.OK
+                return response_json
+            else:
+                entries = []
+                initial_entry = response_json.get("entry", None)
+                if not initial_entry:
+                    self.status_code = ResponseStatusCodes.NOT_FOUND
+                    return response_json
+                else:
+                    self.status_code = ResponseStatusCodes.OK
+                    response_entries = response_json["entry"]
+                    entries.extend(response_entries)
+                    self._execute_callback(response_entries, page_callback)
+                # if the limit is reached, stop resolving the pagination
+                if self._limit and len(entries) >= self._limit:
+                    response_entries = response_json["entry"][: self._limit]
+                    response_json["entry"] = response_entries
+                    self._execute_callback(response_entries, page_callback)
+                    return response_json
+                # query the linked page and add the entries to the response
+
+                while response_json.get("link", None):
+                    if self._limit and len(entries) >= self._limit:
+                        break
+                    next_page = next(
+                        (
+                            link
+                            for link in response_json["link"]
+                            if link.get("relation", None) == "next"
+                        ),
+                        None,
+                    )
+                    if next_page:
+                        response_json = client.get(next_page["url"]).json()
+                        response_entries = response_json["entry"]
+                        entries.extend(response_entries)
+                        self._execute_callback(response_entries, page_callback)
+                    else:
+                        break
+
+            response_json["entry"] = entries[: self._limit] if self._limit else entries
+            return response_json
+
+    def _resolve_xml_pagination(self, server_response: httpx.Response) -> str:
+        # parse the xml response and extract the initial entries
+        initial_response = xmltodict.parse(server_response.text)
+        entries = initial_response["Bundle"].get("entry")
+
+        # if there are no entries, return the initial response
+        if not entries:
+            self.status_code = ResponseStatusCodes.NOT_FOUND
+            print(
+                f"No resources match the query - query url: {self.query_parameters.to_query_string()}"
+            )
+            return server_response.text
+        else:
+            self.status_code = ResponseStatusCodes.OK
+        response = initial_response
+        # resolve the pagination
+        while True:
+            next_page = False
+            for link in response["Bundle"]["link"]:
+                # if there is a next page, get the next page
+                if not isinstance(link, dict):
+                    break
+                relation_dict = link.get("relation", None)
+
+                if relation_dict.get("@value") == "next":
+                    # get url and extend with xml format
+                    url = link["url"]["@value"]
+                    url = url + "&_format=xml"
+                    r = self.client.get(url)
+                    r.raise_for_status()
+                    response = xmltodict.parse(r.text)
+                    if not response["Bundle"].get("entry", None):
+                        break
+                    added_entries = response["Bundle"]["entry"]
+                    entries.extend(added_entries)
+                    # Stop resolving the pagination when the limit is reached
+                    if self._limit:
+                        next_page = len(entries) < self._limit
+                    else:
+                        next_page = True
+
+            if not next_page:
+                break
+        # added the paginated resources to the initial response
+        initial_response["Bundle"]["entry"] = (
+            entries[: self._limit] if self._limit else entries
+        )
+        full_response_xml = xmltodict.unparse(initial_response, pretty=True)
+        return full_response_xml
```

### Comparing `fhir_kindling-1.0.0a8/fhir_kindling/fhir_server/auth.py` & `fhir_kindling-1.0.0a9/fhir_kindling/fhir_server/auth.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a8/fhir_kindling/fhir_server/fhir_server.py` & `fhir_kindling-1.0.0a9/fhir_kindling/fhir_server/fhir_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -444,15 +444,15 @@
         return ResourceCreateResponse(
             server_response_dict=dict(response.headers), resource=resource
         )
 
     def add_all(
         self,
         resources: List[Union[Resource, FHIRAbstractModel, dict]],
-        batch_size: int = 5000,
+        batch_size: int = 1000,
         display: bool = True,
     ) -> BundleCreateResponse:
         """
         Upload a list of resources to the server, after packaging them into a bundle
         Args:
             resources: list of resources to upload to the server, either dictionary or FHIR resource objects
             batch_size: maximum number of resources to upload in one bundle
```

### Comparing `fhir_kindling-1.0.0a8/fhir_kindling/fhir_server/server_responses.py` & `fhir_kindling-1.0.0a9/fhir_kindling/fhir_server/server_responses.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a8/fhir_kindling/fhir_server/summary.py` & `fhir_kindling-1.0.0a9/fhir_kindling/fhir_server/summary.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a8/fhir_kindling/fhir_server/transactions.py` & `fhir_kindling-1.0.0a9/fhir_kindling/fhir_server/transactions.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
                 raise ValueError(
                     f"Unable to construct resource from dict: {resource} \n{e}"
                 )
         # remove the id if the method is POST (create)
         if method == TransactionMethod.PUT and not resource.id:
             raise ValueError("PUT requires a resource with an id")
         if method == TransactionMethod.POST:
-            if resource.id:
+            if hasattr(resource, "id"):
                 del resource.id
         _add_resource_to_entry(entry, resource)
 
     url = _get_transaction_url_for_method(method, url, resource)
 
     entry.request = BundleEntryRequest(**{"method": method.value, "url": url})
```

### Comparing `fhir_kindling-1.0.0a8/fhir_kindling/fhir_server/transfer.py` & `fhir_kindling-1.0.0a9/fhir_kindling/fhir_server/transfer.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a8/fhir_kindling/figures/resource_plots.py` & `fhir_kindling-1.0.0a9/fhir_kindling/figures/resource_plots.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a8/fhir_kindling/figures/summary.py` & `fhir_kindling-1.0.0a9/fhir_kindling/figures/summary.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a8/fhir_kindling/generators/dataset.py` & `fhir_kindling-1.0.0a9/fhir_kindling/generators/dataset.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a8/fhir_kindling/generators/field_generator.py` & `fhir_kindling-1.0.0a9/fhir_kindling/generators/field_generator.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a8/fhir_kindling/generators/patient.py` & `fhir_kindling-1.0.0a9/fhir_kindling/generators/patient.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,23 +38,26 @@
         as_dict: bool = False,
     ):
         patients = self._generate()
         self.resources = patients
 
         if as_dict:
             resources = [json_dict(patient) for patient in patients]
-        if self.n == 1:
-            if references:
-                return resources[0], self._generate_references()[0]
-            return resources[0]
-
-        if references and not self.generate_ids:
-            raise ValueError("Cannot generate references without generating ids")
-        elif references:
-            return resources, self._generate_references()
+            if self.n == 1:
+                if references:
+                    return resources[0], self._generate_references()[0]
+                return resources[0]
+            else:
+                if references:
+                    return resources, self._generate_references()
+        else:
+            if references and not self.generate_ids:
+                raise ValueError("Cannot generate references without generating ids")
+            elif references:
+                return patients, self._generate_references()
 
         return patients
 
     def _generate(self):
         patients = []
         names = self._generate_patient_names(self.n)
         for name in names:
```

### Comparing `fhir_kindling-1.0.0a8/fhir_kindling/generators/resource_generator.py` & `fhir_kindling-1.0.0a9/fhir_kindling/generators/resource_generator.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a8/fhir_kindling/generators/time_series_generator.py` & `fhir_kindling-1.0.0a9/fhir_kindling/generators/time_series_generator.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a8/fhir_kindling/privacy/k_anonymity.py` & `fhir_kindling-1.0.0a9/fhir_kindling/privacy/k_anonymity.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a8/fhir_kindling/serde/flatten.py` & `fhir_kindling-1.0.0a9/fhir_kindling/serde/flatten.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a8/fhir_kindling/tests/conftest.py` & `fhir_kindling-1.0.0a9/fhir_kindling/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a8/fhir_kindling/tests/test_auth.py` & `fhir_kindling-1.0.0a9/fhir_kindling/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a8/fhir_kindling/tests/test_fhir_query.py` & `fhir_kindling-1.0.0a9/fhir_kindling/tests/test_fhir_query.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a8/fhir_kindling/tests/test_fhir_server.py` & `fhir_kindling-1.0.0a9/fhir_kindling/tests/test_fhir_server.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a8/fhir_kindling/tests/test_generators.py` & `fhir_kindling-1.0.0a9/fhir_kindling/tests/test_generators.py`

 * *Files 3% similar despite different names*

```diff
@@ -276,20 +276,23 @@
 def test_generate_covid_dataset(vaccination_code, covid_code, server):
     count = 100
     dataset_generator = DatasetGenerator("Patient", n=count)
 
     covid_params = GeneratorParameters(
         field_values=[
             FieldValue(field="code", value=covid_code),
+            # FieldValue(field="subject", value={"reference": "Patient/123"})
         ]
     )
 
     covid_generator = ResourceGenerator("Condition", generator_parameters=covid_params)
     # add covid conditions to patients
-    dataset_generator.add_resource_generator(covid_generator, name="covid")
+    dataset_generator.add_resource_generator(
+        covid_generator, name="covid", depends_on="base", reference_field="subject"
+    )
 
     patients, patient_ids = PatientGenerator(n=count, generate_ids=True).generate(
         references=True
     )
 
     vaccination_date_generator = FieldGenerator(
         field="occurrenceDateTime",
@@ -304,18 +307,22 @@
         field_generators=[vaccination_date_generator],
     )
     vaccination_generator = ResourceGenerator(
         "Immunization", generator_parameters=first_vax_params
     )
     print(vaccination_generator)
     dataset_generator.add_resource_generator(
-        vaccination_generator, name="first_vaccination", likelihood=0.8
+        vaccination_generator,
+        name="first_vaccination",
+        likelihood=0.8,
+        depends_on="base",
+        reference_field="patient",
     )
 
-    dataset = dataset_generator.generate(ids=True)
+    dataset = dataset_generator.generate()
     print(dataset)
     # pprint(result.dict(exclude_none=True))
 
     dataset.upload(server)
 
 
 def test_time_series_generator():
```

### Comparing `fhir_kindling-1.0.0a8/fhir_kindling/tests/test_plots.py` & `fhir_kindling-1.0.0a9/fhir_kindling/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a8/fhir_kindling/tests/test_privacy.py` & `fhir_kindling-1.0.0a9/fhir_kindling/tests/test_privacy.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a8/fhir_kindling/tests/test_serialization.py` & `fhir_kindling-1.0.0a9/fhir_kindling/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a8/fhir_kindling/tests/test_util.py` & `fhir_kindling-1.0.0a9/fhir_kindling/tests/test_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from fhir.resources.condition import Condition
 from fhir.resources.encounter import Encounter
 from fhir.resources.observation import Observation
 from fhir.resources.organization import Organization
 from fhir.resources.patient import Patient
 
 from fhir_kindling import FhirServer
+from fhir_kindling.benchmark.bench import ServerBenchmark
 from fhir_kindling.fhir_server.transfer import reference_graph
 from fhir_kindling.generators import PatientGenerator
-from fhir_kindling.util.benchmark import ServerBenchmark
 from fhir_kindling.util.references import (
     _resource_ids_from_query_response,
     check_missing_references,
     extract_references,
 )
 from fhir_kindling.util.resources import (
     check_resource_contains_field,
@@ -140,10 +140,12 @@
     check_resource_contains_field("Patient", "birthDate")
     with pytest.raises(ValueError):
         check_resource_contains_field("Patient", "foo")
 
 
 def test_benchmark(server):
     transfer_server = FhirServer(api_address=os.getenv("TRANSFER_API_URL"))
-    benchmark = ServerBenchmark(servers=[server, transfer_server])
-    benchmark.run_suite()
-    benchmark.plot()
+    benchmark = ServerBenchmark(
+        servers=[server, transfer_server], n_attempts=2, dataset_size=10
+    )
+    benchmark.run_suite(progress=False, save=False)
+    # benchmark.plot()
```

### Comparing `fhir_kindling-1.0.0a8/fhir_kindling/util/references.py` & `fhir_kindling-1.0.0a9/fhir_kindling/util/references.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a8/fhir_kindling/util/resources.py` & `fhir_kindling-1.0.0a9/fhir_kindling/util/resources.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a8/pyproject.toml` & `fhir_kindling-1.0.0a9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fhir-kindling"
-version = "1.0.0a8"
+version = "1.0.0a9"
 description = "Python library to simplify working with FHIR servers and resources."
 authors = ["Michael Graf <michael.graf3110@gmail.com>"]
 # todo add changelog when multiple readme bug is fixed
 readme = "README.md"
 packages = [{ include = "fhir_kindling" }]
 homepage = "https://migraf.github.io/fhir-kindling/"
 repository = "https://github.com/migraf/fhir-kindling"
@@ -44,20 +44,21 @@
 pandas = { version = "*", optional = true }
 plotly = { version = "*", optional = true }
 faker = { version = "*", optional = true }
 matplotlib = { version = "*", optional = true }
 notebook = { version = "*", optional = true }
 RISE = { version = "*", optional = true }
 ipywidgets = { version = "*", optional = true }
+kaleido  = { version = "0.2.1", optional = true }
 
 
 
 [tool.poetry.extras]
-ds = ["pandas", "plotly", "faker", "matplotlib"]
-demo = ["pandas", "plotly", "faker", "matplotlib", "notebook", "RISE", "ipywidgets"]
+ds = ["pandas", "plotly", "faker", "matplotlib", "kaleido"]
+demo = ["pandas", "plotly", "faker", "matplotlib", "notebook", "RISE", "ipywidgets", "kaleido"]
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 coverage = "*"
 tox = "*"
 mkdocs = "*"
```

### Comparing `fhir_kindling-1.0.0a8/PKG-INFO` & `fhir_kindling-1.0.0a9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fhir-kindling
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: Python library to simplify working with FHIR servers and resources.
 Home-page: https://migraf.github.io/fhir-kindling/
 License: MIT
 Keywords: python,fhir,hl7,client,medical records,healthcare,data
 Author: Michael Graf
 Author-email: michael.graf3110@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -25,14 +25,15 @@
 Provides-Extra: ds
 Requires-Dist: RISE ; extra == "demo"
 Requires-Dist: authlib
 Requires-Dist: faker ; extra == "ds" or extra == "demo"
 Requires-Dist: fhir.resources (>=6.0.0,<7.0.0)
 Requires-Dist: httpx
 Requires-Dist: ipywidgets ; extra == "demo"
+Requires-Dist: kaleido (==0.2.1) ; extra == "ds" or extra == "demo"
 Requires-Dist: matplotlib ; extra == "ds" or extra == "demo"
 Requires-Dist: networkx
 Requires-Dist: notebook ; extra == "demo"
 Requires-Dist: orjson
 Requires-Dist: pandas ; extra == "ds" or extra == "demo"
 Requires-Dist: pendulum
 Requires-Dist: plotly ; extra == "ds" or extra == "demo"
```

