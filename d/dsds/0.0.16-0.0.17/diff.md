# Comparing `tmp/dsds-0.0.16.tar.gz` & `tmp/dsds-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsds-0.0.16.tar", last modified: Wed Jul  5 02:39:17 2023, max compression
+gzip compressed data, was "dsds-0.0.17.tar", last modified: Sun Jul  9 00:37:04 2023, max compression
```

## Comparing `dsds-0.0.16.tar` & `dsds-0.0.17.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 tq        (1000) tq        (1000)        0 2023-07-05 02:39:17.706042 dsds-0.0.16/
--rw-rw-r--   0 tq        (1000) tq        (1000)     1059 2023-07-02 13:17:50.000000 dsds-0.0.16/LICENSE
--rw-rw-r--   0 tq        (1000) tq        (1000)     2321 2023-07-05 02:39:17.706042 dsds-0.0.16/PKG-INFO
--rw-rw-r--   0 tq        (1000) tq        (1000)     1348 2023-07-05 02:35:55.000000 dsds-0.0.16/pyproject.toml
--rw-rw-r--   0 tq        (1000) tq        (1000)       38 2023-07-05 02:39:17.706042 dsds-0.0.16/setup.cfg
-drwxrwxr-x   0 tq        (1000) tq        (1000)        0 2023-07-05 02:39:17.690042 dsds-0.0.16/src/
-drwxrwxr-x   0 tq        (1000) tq        (1000)        0 2023-07-05 02:39:17.702042 dsds-0.0.16/src/dsds/
--rw-rw-r--   0 tq        (1000) tq        (1000)       81 2023-07-05 02:36:00.000000 dsds-0.0.16/src/dsds/__init__.py
--rw-rw-r--   0 tq        (1000) tq        (1000)     4421 2023-07-02 13:17:50.000000 dsds-0.0.16/src/dsds/blueprint.py
--rw-rw-r--   0 tq        (1000) tq        (1000)     3677 2023-07-02 13:17:50.000000 dsds-0.0.16/src/dsds/eda_text.py
--rw-rw-r--   0 tq        (1000) tq        (1000)    30205 2023-07-05 02:13:42.000000 dsds-0.0.16/src/dsds/fs.py
--rw-rw-r--   0 tq        (1000) tq        (1000)     7699 2023-07-05 02:29:08.000000 dsds-0.0.16/src/dsds/metrics.py
--rw-rw-r--   0 tq        (1000) tq        (1000)    26622 2023-07-04 20:41:15.000000 dsds-0.0.16/src/dsds/prescreen.py
--rw-rw-r--   0 tq        (1000) tq        (1000)     4195 2023-07-05 00:57:20.000000 dsds-0.0.16/src/dsds/sample.py
--rw-rw-r--   0 tq        (1000) tq        (1000)    25127 2023-07-04 17:54:29.000000 dsds-0.0.16/src/dsds/transform.py
--rw-rw-r--   0 tq        (1000) tq        (1000)     1564 2023-07-04 18:43:47.000000 dsds-0.0.16/src/dsds/type_alias.py
--rw-rw-r--   0 tq        (1000) tq        (1000)     1750 2023-07-02 13:17:50.000000 dsds-0.0.16/src/dsds/utils.py
-drwxrwxr-x   0 tq        (1000) tq        (1000)        0 2023-07-05 02:39:17.702042 dsds-0.0.16/src/dsds.egg-info/
--rw-rw-r--   0 tq        (1000) tq        (1000)     2321 2023-07-05 02:39:17.000000 dsds-0.0.16/src/dsds.egg-info/PKG-INFO
--rw-rw-r--   0 tq        (1000) tq        (1000)      384 2023-07-05 02:39:17.000000 dsds-0.0.16/src/dsds.egg-info/SOURCES.txt
--rw-rw-r--   0 tq        (1000) tq        (1000)        1 2023-07-05 02:39:17.000000 dsds-0.0.16/src/dsds.egg-info/dependency_links.txt
--rw-rw-r--   0 tq        (1000) tq        (1000)      173 2023-07-05 02:39:17.000000 dsds-0.0.16/src/dsds.egg-info/requires.txt
--rw-rw-r--   0 tq        (1000) tq        (1000)        5 2023-07-05 02:39:17.000000 dsds-0.0.16/src/dsds.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-09 00:37:04.934278 dsds-0.0.17/
+-rw-rw-rw-   0        0        0     1079 2023-06-23 04:44:14.000000 dsds-0.0.17/LICENSE
+-rw-rw-rw-   0        0        0     5850 2023-07-09 00:37:04.934278 dsds-0.0.17/PKG-INFO
+-rw-rw-rw-   0        0        0     3478 2023-07-09 00:29:00.000000 dsds-0.0.17/README.md
+-rw-rw-rw-   0        0        0     1398 2023-07-09 00:36:45.000000 dsds-0.0.17/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-09 00:37:04.934278 dsds-0.0.17/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-09 00:37:04.896269 dsds-0.0.17/src/
+drwxrwxrwx   0        0        0        0 2023-07-09 00:37:04.914273 dsds-0.0.17/src/dsds/
+-rw-rw-rw-   0        0        0       87 2023-07-09 00:36:50.000000 dsds-0.0.17/src/dsds/__init__.py
+-rw-rw-rw-   0        0        0     4937 2023-07-09 00:31:32.000000 dsds-0.0.17/src/dsds/blueprint.py
+-rw-rw-rw-   0        0        0     3766 2023-06-20 23:18:47.000000 dsds-0.0.17/src/dsds/eda_text.py
+-rw-rw-rw-   0        0        0    31557 2023-07-09 00:29:00.000000 dsds-0.0.17/src/dsds/fs.py
+-rw-rw-rw-   0        0        0     7916 2023-07-09 00:29:00.000000 dsds-0.0.17/src/dsds/metrics.py
+-rw-rw-rw-   0        0        0    27272 2023-07-09 00:29:00.000000 dsds-0.0.17/src/dsds/prescreen.py
+-rw-rw-rw-   0        0        0     9095 2023-07-09 00:29:00.000000 dsds-0.0.17/src/dsds/sample.py
+-rw-rw-rw-   0        0        0    28827 2023-07-09 00:31:23.000000 dsds-0.0.17/src/dsds/transform.py
+-rw-rw-rw-   0        0        0     1771 2023-07-09 00:29:00.000000 dsds-0.0.17/src/dsds/type_alias.py
+-rw-rw-rw-   0        0        0     2085 2023-07-09 00:29:00.000000 dsds-0.0.17/src/dsds/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-09 00:37:04.932278 dsds-0.0.17/src/dsds.egg-info/
+-rw-rw-rw-   0        0        0     5850 2023-07-09 00:37:04.000000 dsds-0.0.17/src/dsds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2023-07-09 00:37:04.000000 dsds-0.0.17/src/dsds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 00:37:04.000000 dsds-0.0.17/src/dsds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      173 2023-07-09 00:37:04.000000 dsds-0.0.17/src/dsds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-09 00:37:04.000000 dsds-0.0.17/src/dsds.egg-info/top_level.txt
```

### Comparing `dsds-0.0.16/LICENSE` & `dsds-0.0.17/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 T.Q
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2023 T.Q
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `dsds-0.0.16/pyproject.toml` & `dsds-0.0.17/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-[build-system]
-requires = ["setuptools"]
-
-[project]
-name = "dsds"
-version = "0.0.16"
-requires-python = ">=3.9"
-readme = "README.md"
-description = "A feature screening, selection, EDA, pipeline building and management tool centered around Polars dataframe."
-authors = [
-    {name = "Tianren Qin", email = "tq9695@gmail.com"}
-]
-license = {file = "LICENSE"}
-dependencies = [
-    "polars >= 0.18.4",
-    "scipy >= 1.11.1",
-    "pandas",
-    "numpy",
-    "typing_extensions >= 4.0.1"
-]
-
-keywords = ["data pipeline", "EDA", "feature-screening", "feature-selection"]
-
-classifiers = [
-  "Development Status :: 2 - Pre-Alpha",
-  "Environment :: Console",
-  "Intended Audience :: Science/Research",
-  "License :: OSI Approved :: MIT License",
-  "Operating System :: OS Independent",
-  "Programming Language :: Python",
-  "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3 :: Only",
-  "Programming Language :: Python :: 3.9",
-  "Programming Language :: Python :: 3.10",
-  "Programming Language :: Python :: 3.11",
-  "Topic :: Scientific/Engineering",
-]
-
-[project.optional-dependencies]
-scikit-learn = ["scikit-learn"]
-xgboost = ["xgboost"]
-lightgbm = ["lightgbm"]
-all = ["scikit-learn", "xgboost", "lightgbm"]
-
-[project.urls]
-"Homepage" = "https://github.com/abstractqqq/dsds"
-
-[tool.ruff]
-line-length = 120
-fix = true
+[build-system]
+requires = ["setuptools"]
+
+[project]
+name = "dsds"
+version = "0.0.17"
+requires-python = ">=3.9"
+readme = "README.md"
+description = "A feature screening, selection, EDA, pipeline building and management tool centered around Polars dataframe."
+authors = [
+    {name = "Tianren Qin", email = "tq9695@gmail.com"}
+]
+license = {file = "LICENSE"}
+dependencies = [
+    "polars >= 0.18.6",
+    "scipy >= 1.11.1",
+    "pandas",
+    "numpy",
+    "typing_extensions >= 4.0.1"
+]
+
+keywords = ["data pipeline", "EDA", "feature-screening", "feature-selection"]
+
+classifiers = [
+  "Development Status :: 2 - Pre-Alpha",
+  "Environment :: Console",
+  "Intended Audience :: Science/Research",
+  "License :: OSI Approved :: MIT License",
+  "Operating System :: OS Independent",
+  "Programming Language :: Python",
+  "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3 :: Only",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Topic :: Scientific/Engineering",
+]
+
+[project.optional-dependencies]
+scikit-learn = ["scikit-learn"]
+xgboost = ["xgboost"]
+lightgbm = ["lightgbm"]
+all = ["scikit-learn", "xgboost", "lightgbm"]
+
+[project.urls]
+"Homepage" = "https://github.com/abstractqqq/dsds"
+
+[tool.ruff]
+line-length = 120
+fix = true
 src = ["src"]
```

### Comparing `dsds-0.0.16/src/dsds/blueprint.py` & `dsds-0.0.17/src/dsds/blueprint.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,107 +1,120 @@
-from pathlib import Path
-import polars as pl
-from polars import LazyFrame
-from dataclasses import dataclass
-import pickle
-from typing import Iterable, Any, Optional
-from polars.type_aliases import IntoExpr
-from .type_alias import (
-    PolarsFrame
-    , StepName
-)
-
-
-@dataclass
-class MapDict:
-    left_col: str # Join on this column, and this column will be replaced by right and dropped.
-    ref: dict # The right table as a dictionary
-    right_col: str
-    default: Optional[Any]
-
-@dataclass
-class Step:
-    name:StepName
-    associated_data: Iterable[IntoExpr] | MapDict | list[str]
-    # First is a with_column, second is a string encoder, third is a drop / a selector
-
-
-@pl.api.register_lazyframe_namespace("blueprint")
-class Blueprint:
-    def __init__(self, ldf: LazyFrame):
-        self._ldf = ldf
-        self.steps:list[Step] = []
-
-    @staticmethod
-    def _map_dict(df:PolarsFrame, map_dict:MapDict) -> PolarsFrame:
-        temp = pl.from_dict(map_dict.ref) # Always an eager read
-        if isinstance(df, pl.LazyFrame): 
-            temp = temp.lazy()
-        
-        if map_dict.default is None:
-            return df.join(temp, on = map_dict.left_col).with_columns(
-                pl.col(map_dict.right_col).alias(map_dict.left_col)
-            ).drop(map_dict.right_col)
-        else:
-            return df.join(temp, on = map_dict.left_col, how = "left").with_columns(
-                pl.col(map_dict.right_col).fill_null(map_dict.default).alias(map_dict.left_col)
-            ).drop(map_dict.right_col)
-
-    # Feature Transformations that requires a 1-1 mapping as given by the ref dict. This will be
-    # carried out using a join logic to avoid the use of Python UDF.
-    def map_dict(self, left_col:str, ref:dict, right_col:str, default:Optional[Any]) -> LazyFrame:
-        map_dict = MapDict(left_col = left_col, ref = ref, right_col = right_col, default = default)
-        self.steps.append(
-            Step(name = "map_dict", associated_data = map_dict)
-        )
-        output = self._map_dict(self._ldf, map_dict)
-        output.blueprint.steps = self.steps # Change "ownership" of this list[Steps] to output.blueprint
-        self.steps = [] # Give up self.steps's ownership of the list[Steps] by setting it to an empty list.
-        return output
-
-    # Transformations are just with_columns(exprs)
-    def with_columns(self, exprs: Iterable[IntoExpr]) -> LazyFrame:
-        self.steps.append(
-            Step(name = "with_column", associated_data = exprs)
-        )
-        output = self._ldf.with_columns(exprs)
-        output.blueprint.steps = self.steps # Change "ownership" of this list[Steps] to output.blueprint
-        self.steps = [] # Give up self.steps's ownership of the list[Steps] by setting it to an empty list.
-        return output
-    
-    # Transformations are just select, used mostly in selector functions
-    def select(self, to_select: Iterable[IntoExpr]) -> LazyFrame:
-        self.steps.append(
-            Step(name = "select", associated_data = to_select)
-        )
-        output = self._ldf.select(to_select)
-        output.blueprint.steps = self.steps # Change "ownership" of this list[Steps] to output.blueprint
-        self.steps = [] # Give up self.steps's ownership of the list[Steps] by setting it to an empty list.
-        return output
-    
-    # Transformations that drops, used mostly in removal functions
-    def drop(self, drop_cols:Iterable[IntoExpr]) -> LazyFrame:
-        self.steps.append(
-            Step(name = "drop", associated_data = drop_cols)
-        )
-        output = self._ldf.drop(drop_cols)
-        output.blueprint.steps = self.steps # Change "ownership" of this list[Steps] to output.blueprint
-        self.steps = []  # Give up self.steps's ownership of the list[Steps] by setting it to an empty list.
-        return output
-        
-    def preserve(self, path:str|Path):
-        f = open(path, "wb")
-        pickle.dump(self, f)
-        f.close()
-
-    def apply(self, df:PolarsFrame) -> PolarsFrame:
-        for s in self.steps:
-            if s.name == "drop":
-                df = df.drop(s.associated_data)
-            elif s.name == "with_column":
-                df = df.with_columns(s.associated_data)
-            elif s.name == "map_dict":
-                df = self._map_dict(df, s.associated_data)
-            elif s.name == "select":
-                df = df.select(s.associated_data)
-            
-        return df
+import pickle
+import polars as pl
+# import importlib
+from pathlib import Path
+from polars import LazyFrame
+from dataclasses import dataclass
+from typing import (
+    Any
+    , Iterable
+    , Optional
+)
+from polars.type_aliases import IntoExpr
+from .type_alias import (
+    PolarsFrame
+    , ActionType
+    # , PipeFunction
+)
+
+
+@dataclass
+class MapDict:
+    left_col: str # Join on this column, and this column will be replaced by right and dropped.
+    ref: dict # The right table as a dictionary
+    right_col: str
+    default: Optional[Any]
+
+@dataclass
+class Step:
+    action:ActionType
+    associated_data: Iterable[IntoExpr] | MapDict | list[str]
+    # First is a with_column, second is a string encoder, third is a drop/select/apply_func
+
+
+@pl.api.register_lazyframe_namespace("blueprint")
+class Blueprint:
+    def __init__(self, ldf: LazyFrame):
+        self._ldf = ldf
+        self.steps:list[Step] = []
+
+    @staticmethod
+    def _map_dict(df:PolarsFrame, map_dict:MapDict) -> PolarsFrame:
+        temp = pl.from_dict(map_dict.ref) # Always an eager read
+        if isinstance(df, pl.LazyFrame): 
+            temp = temp.lazy()
+        
+        if map_dict.default is None:
+            return df.join(temp, on = map_dict.left_col).with_columns(
+                pl.col(map_dict.right_col).alias(map_dict.left_col)
+            ).drop(map_dict.right_col)
+        else:
+            return df.join(temp, on = map_dict.left_col, how = "left").with_columns(
+                pl.col(map_dict.right_col).fill_null(map_dict.default).alias(map_dict.left_col)
+            ).drop(map_dict.right_col)
+
+    # Feature Transformations that requires a 1-1 mapping as given by the ref dict. This will be
+    # carried out using a join logic to avoid the use of Python UDF.
+    def map_dict(self, left_col:str, ref:dict, right_col:str, default:Optional[Any]) -> LazyFrame:
+        map_dict = MapDict(left_col = left_col, ref = ref, right_col = right_col, default = default)
+        self.steps.append(
+            Step(action = "map_dict", associated_data = map_dict)
+        )
+        output = self._map_dict(self._ldf, map_dict)
+        output.blueprint.steps = self.steps # Change "ownership" of this list[Steps] to output.blueprint
+        self.steps = [] # Give up self.steps's ownership of the list[Steps] by setting it to an empty list.
+        return output
+
+    # Transformations are just with_columns(exprs)
+    def with_columns(self, exprs:Iterable[IntoExpr]) -> LazyFrame:
+        self.steps.append(
+            Step(action = "with_column", associated_data = list(exprs))
+        )
+        output = self._ldf.with_columns(exprs)
+        output.blueprint.steps = self.steps # Change "ownership" of this list[Steps] to output.blueprint
+        self.steps = [] # Give up self.steps's ownership of the list[Steps] by setting it to an empty list.
+        return output
+    
+    # Transformations are just select, used mostly in selector functions
+    def select(self, to_select:list[str]) -> LazyFrame:
+        self.steps.append(
+            Step(action = "select", associated_data = to_select)
+        )
+        output = self._ldf.select(to_select)
+        output.blueprint.steps = self.steps # Change "ownership" of this list[Steps] to output.blueprint
+        self.steps = [] # Give up self.steps's ownership of the list[Steps] by setting it to an empty list.
+        return output
+    
+    # Transformations that drops, used mostly in removal functions
+    def drop(self, drop_cols:list[str]) -> LazyFrame:
+        self.steps.append(
+            Step(action = "drop", associated_data = drop_cols)
+        )
+        output = self._ldf.drop(drop_cols)
+        output.blueprint.steps = self.steps # Change "ownership" of this list[Steps] to output.blueprint
+        self.steps = []  # Give up self.steps's ownership of the list[Steps] by setting it to an empty list.
+        return output
+    
+    # # Functional steps are steps like upsample/downsample, which can be persisted in pipeline, but 
+    # # may not be repeatable.
+    # def add_functional_step(self, func:PipeFunction):
+    #     self.steps.append(
+    #         Step(action="apply_func", associated_data=[func.__module__, func.__name__])
+    #     )
+        
+    def preserve(self, path:str|Path):
+        f = open(path, "wb")
+        pickle.dump(self, f)
+        f.close()
+
+    def apply(self, df:PolarsFrame) -> PolarsFrame:
+        for s in self.steps:
+            if s.action == "drop":
+                df = df.drop(s.associated_data)
+            elif s.action == "with_column":
+                df = df.with_columns(s.associated_data)
+            elif s.action == "map_dict":
+                df = self._map_dict(df, s.associated_data)
+            elif s.action == "select":
+                df = df.select(s.associated_data)
+            
+        return df
```

### Comparing `dsds-0.0.16/src/dsds/eda_text.py` & `dsds-0.0.17/src/dsds/eda_text.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-# import polars as pl 
-# import pandas as pd 
-# from typing import Tuple
-# from nltk.corpus import stopwords
-# from nltk.stem import PorterStemmer
-# from scipy.sparse import csr_matrix
-# from sklearn.feature_extraction.text import TfidfVectorizer, CountVectorizer
-
-# # DEVELOPMENT HALTED FOR NOW.
-
-# # nltk.download("punkt")
-# stop = stopwords.words('english')
-
-# def _reverse_memo(memo:dict[str, str]) -> dict[str, list[str]]:
-#     '''
-#     Reverse the memo used in transform_text_data. 
-        
-#     Returns: 
-#         the mapping between stemmed words and the many versions of the word that get stemmed to the same "root".
-    
-#     '''
-#     output:dict[str, list[str]] = {}
-#     for key, item in memo.items():
-#         if item in output:
-#             output[item].append(key)
-#         else:
-#             output[item] = [key]
-
-#     return output 
-
-# def transform_text_data(df:pl.DataFrame|pd.DataFrame
-#     , text_cols:list[str]
-#     , vectorize_method:str = "count"
-#     , max_df:float=0.95, min_df:float=0.05,
-# ) -> Tuple[pl.DataFrame, dict[str, list[str]]]:
-#     ''' 
-#     Given a dataframe, perform one-hot encoding and TFIDF/count transformation for the respective columns.
-#     This may not be optimized.
-
-#     Arguments:
-#         df: input Pandas/Polars dataframe
-#         text_cols: a list of str representing column names that need to be TFIDF/count vectorized
-#         vectorizer: str, either "count" or "tfidf"
-#         max_df: do not consider words with document frequency > max_df. Default 0.95.
-#         min_df: do not consider words with document frequency < min_df. Default 0.05.
-
-#     Returns:
-#         transformed polars dataframe, and a memo of what is being mapped to what.
-
-#     '''
-
-#     df2 = df.with_columns((
-#         # first step in cleaning the data, perform split, so now it is a []
-#         pl.col(t).str.replace_all('[^\s\w\d%]', '').str.to_lowercase().str.split(by=" ")
-#         for t in text_cols
-#     ))
-
-#     print("Perfoming stemming...")
-#     ps = PorterStemmer()
-#     memo = {} # perform memoization for stemming
-#     if vectorize_method == "tfidf":
-#         vectorizer:TfidfVectorizer = TfidfVectorizer(max_df = max_df, min_df = min_df, stop_words=list(stop))
-#     else:
-#         vectorizer:CountVectorizer = CountVectorizer(max_df = max_df, min_df = min_df, stop_words=list(stop))
-    
-#     new_columns = [df2] # df2 will be changed in the for loop, but that is ok.
-#     for c in text_cols:
-#         new_list:list[str] = []
-#         text_column = df2.drop_in_place(c)
-#         for tokens in text_column:
-#             if not tokens.is_empty(): # if tokens is not empty. Tokens is a pl.Series.
-#                 new_tokens:list[str] = [] 
-#                 for w in tokens:
-#                     if w not in memo:
-#                         memo[w] = ps.stem(w)
-#                     new_tokens.append(memo[w])
-#                 # re-map the tokens into sentences, in order to use scikit-learn builtin vectorize methods. Bad for performance? Can this be improved?
-#                 new_list.append(" ".join(new_tokens))
-#             else:
-#                 new_list.append("Unknown")
-
-#         print(f"Performing {vectorize_method.capitalize()} vectorization for {c}...")
-#         # Vectorizer will return Sparse matrix
-#         X:csr_matrix = vectorizer.fit_transform(new_list)
-#         names:list[str] = [c+"::word::"+x for x in vectorizer.get_feature_names_out()]
-#         # Add this new dataframe to a list 
-#         new_columns.append(pl.from_numpy(X.toarray(), schema=names))
-
-#     df_final = pl.concat(new_columns, how="horizontal")
+# import polars as pl 
+# import pandas as pd 
+# from typing import Tuple
+# from nltk.corpus import stopwords
+# from nltk.stem import PorterStemmer
+# from scipy.sparse import csr_matrix
+# from sklearn.feature_extraction.text import TfidfVectorizer, CountVectorizer
+
+# # DEVELOPMENT HALTED FOR NOW.
+
+# # nltk.download("punkt")
+# stop = stopwords.words('english')
+
+# def _reverse_memo(memo:dict[str, str]) -> dict[str, list[str]]:
+#     '''
+#     Reverse the memo used in transform_text_data. 
+        
+#     Returns: 
+#         the mapping between stemmed words and the many versions of the word that get stemmed to the same "root".
+    
+#     '''
+#     output:dict[str, list[str]] = {}
+#     for key, item in memo.items():
+#         if item in output:
+#             output[item].append(key)
+#         else:
+#             output[item] = [key]
+
+#     return output 
+
+# def transform_text_data(df:pl.DataFrame|pd.DataFrame
+#     , text_cols:list[str]
+#     , vectorize_method:str = "count"
+#     , max_df:float=0.95, min_df:float=0.05,
+# ) -> Tuple[pl.DataFrame, dict[str, list[str]]]:
+#     ''' 
+#     Given a dataframe, perform one-hot encoding and TFIDF/count transformation for the respective columns.
+#     This may not be optimized.
+
+#     Arguments:
+#         df: input Pandas/Polars dataframe
+#         text_cols: a list of str representing column names that need to be TFIDF/count vectorized
+#         vectorizer: str, either "count" or "tfidf"
+#         max_df: do not consider words with document frequency > max_df. Default 0.95.
+#         min_df: do not consider words with document frequency < min_df. Default 0.05.
+
+#     Returns:
+#         transformed polars dataframe, and a memo of what is being mapped to what.
+
+#     '''
+
+#     df2 = df.with_columns((
+#         # first step in cleaning the data, perform split, so now it is a []
+#         pl.col(t).str.replace_all('[^\s\w\d%]', '').str.to_lowercase().str.split(by=" ")
+#         for t in text_cols
+#     ))
+
+#     print("Perfoming stemming...")
+#     ps = PorterStemmer()
+#     memo = {} # perform memoization for stemming
+#     if vectorize_method == "tfidf":
+#         vectorizer:TfidfVectorizer = TfidfVectorizer(max_df = max_df, min_df = min_df, stop_words=list(stop))
+#     else:
+#         vectorizer:CountVectorizer = CountVectorizer(max_df = max_df, min_df = min_df, stop_words=list(stop))
+    
+#     new_columns = [df2] # df2 will be changed in the for loop, but that is ok.
+#     for c in text_cols:
+#         new_list:list[str] = []
+#         text_column = df2.drop_in_place(c)
+#         for tokens in text_column:
+#             if not tokens.is_empty(): # if tokens is not empty. Tokens is a pl.Series.
+#                 new_tokens:list[str] = [] 
+#                 for w in tokens:
+#                     if w not in memo:
+#                         memo[w] = ps.stem(w)
+#                     new_tokens.append(memo[w])
+#                 # re-map the tokens into sentences, in order to use scikit-learn builtin vectorize methods. Bad for performance? Can this be improved?
+#                 new_list.append(" ".join(new_tokens))
+#             else:
+#                 new_list.append("Unknown")
+
+#         print(f"Performing {vectorize_method.capitalize()} vectorization for {c}...")
+#         # Vectorizer will return Sparse matrix
+#         X:csr_matrix = vectorizer.fit_transform(new_list)
+#         names:list[str] = [c+"::word::"+x for x in vectorizer.get_feature_names_out()]
+#         # Add this new dataframe to a list 
+#         new_columns.append(pl.from_numpy(X.toarray(), schema=names))
+
+#     df_final = pl.concat(new_columns, how="horizontal")
 #     return df_final, _reverse_memo(memo)
```

### Comparing `dsds-0.0.16/src/dsds/fs.py` & `dsds-0.0.17/src/dsds/fs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,800 +1,812 @@
-from .prescreen import (
-    discrete_inferral
-    , check_binary_target
-    , get_numeric_cols
-    , get_unique_count
-    , get_string_cols
-)
-
-from .type_alias import (
-    PolarsFrame
-    , MRMRStrategy
-    , BinaryModels
-    , CPU_COUNT
-    , clean_strategy_str
-)
-from .blueprint import( # Need this for Polars extension to work
-    Blueprint
-)
-from .sample import (
-    train_test_split
-)
-from .metrics import (
-    logloss
-    , roc_auc
-)
-import polars as pl
-import numpy as np
-from typing import Any, Optional, Tuple
-from scipy.spatial import KDTree
-from scipy.special import fdtrc, psi
-from concurrent.futures import ThreadPoolExecutor, as_completed
-from tqdm import tqdm
-import math
-from itertools import combinations
-
-def _conditional_entropy(
-    df:pl.DataFrame
-    , target:str
-    , predictive:str
-) -> Tuple[str, float]:
-
-    cond_entropy = df.groupby((target, predictive)).agg(
-        pl.count()
-    ).with_columns(
-        (pl.col("count").sum().over(predictive) / len(df)).alias("prob(predictive)"),
-        (pl.col("count") / pl.col("count").sum()).alias("prob(target,predictive)")
-    ).select(
-        (-((pl.col("prob(target,predictive)")/pl.col("prob(predictive)")).log() 
-           * pl.col("prob(target,predictive)")).sum()) # This is the conditional entropy.
-    ).row(0)[0]
-
-    return (predictive, cond_entropy)
-
-# !!!NEED REVIEW FOR CORRECTNESS
-def discrete_ig(
-    df:pl.DataFrame
-    , target:str
-    , cols:Optional[list[str]] = None
-    , n_threads:int = CPU_COUNT
-) -> pl.DataFrame:
-    '''The entropy here is "discrete entropy".
-
-        Computes the information gain: Entropy(target) - Conditional_Entropy(target|c), where c is a column in 
-        discrete_cols. For more information, please take a look at https://en.wikipedia.org/wiki/Entropy_(information_theory)
-
-        Information gain defined in this way suffers from high cardinality (high uniqueness), and therefore a weighted 
-        information gain is provided, weighted by (1 - unique_pct), where unique_pct represents the percentage of unique
-         values in feature.
-
-        Currently this only works for discrete columns. For continuous features vs discrete target, use mutual_info.
-
-        Arguments:
-            df: Eager frame only.
-            target:
-            cols: list of discrete columns. If not provided, they will be inferred.
-            top_k: must be >= 0. If <= 0, the entire DataFrame will be returned.
-            n_threads: 4, 8 ,16 will not make any real difference. But there is a difference between 0 and 4 threads. 
-            
-        Returns:
-            a poalrs dataframe with information gain computed for each categorical column. 
-    '''
-    output = []
-    if isinstance(cols, list):
-        discretes = cols
-    else: # If discrete_cols is not passed, infer it
-        discretes = discrete_inferral(df, exclude=[target])
-
-    # Compute target entropy. This only needs to be done once.
-    target_entropy = df.groupby(target).agg(
-                        (pl.count()).alias("prob(target)") / len(df)
-                    ).get_column("prob(target)").entropy()
-
-    # Get unique count for selected columns. This is because higher unique percentage may skew information gain
-    unique_count = get_unique_count(df.select(discretes)).with_columns(
-        (pl.col("n_unique") / len(df)).alias("unique_pct")
-    ).rename({"column":"feature"})
-
-    with ThreadPoolExecutor(max_workers=n_threads) as ex: # 10% speed gain ? Need to retest this..
-        pbar = tqdm(total=len(discretes), desc = "discrete_ig")
-        for f in as_completed(ex.submit(_conditional_entropy, df, target, pred) for pred in discretes):
-            output.append(f.result())
-            pbar.update(1)
-        pbar.close()
-
-    return pl.from_records(output, schema=["feature", "conditional_entropy"])\
-        .with_columns(
-            target_entropy = pl.lit(target_entropy),
-            information_gain = pl.lit(target_entropy) - pl.col("conditional_entropy")
-        ).join(unique_count, on="feature")\
-        .select("feature", "target_entropy", "conditional_entropy", "unique_pct", "information_gain")\
-        .with_columns(
-            weighted_information_gain = (1 - pl.col("unique_pct")) * pl.col("information_gain")
-        )
-
-discrete_mi = discrete_ig
-
-def discrete_ig_selector(
-    df:PolarsFrame
-    , target:str
-    , top_k:int
-    , n_threads:int = CPU_COUNT
-) -> PolarsFrame:
-    
-    discrete_cols = discrete_inferral(df, exclude=[target])
-    is_lazy = isinstance(df, pl.LazyFrame)
-    if is_lazy:
-        input_data:pl.DataFrame = df.collect()
-    else:
-        input_data:pl.DataFrame = df
-
-    ig = discrete_ig(input_data, target, discrete_cols, n_threads)\
-            .top_k(by="information_gain", k = top_k)
-
-    complement = [f for f in input_data.columns if f not in discrete_cols]
-    selected = ig.get_column("feature").to_list()
-    print(f"Selected {len(selected)} features. There are {len(complement)} columns the algorithm "
-        "cannot process. They are also returned.")
-
-    if is_lazy:
-        return df.blueprint.select(selected + complement)
-    return df.select(selected + complement)
-
-def mutual_info(
-    df:pl.DataFrame
-    , target:str
-    , conti_cols:list[str]
-    , n_neighbors:int=3
-    , seed:int=42
-    , n_threads:int=CPU_COUNT
-) -> pl.DataFrame:
-    '''Approximates mutual information (information gain) between the continuous variables and the target.
-
-        This is essentially a "copy-and-paste" of the mutual_info_classif call in sklearn library. 
-        There are a few important distinctions:
-
-        1. This uses Scipy library's kdtree, instead of sklearn's kdtree and nearneighbors. 
-        2. The use of Scipy enables us to use more cores. 
-        3. There are less "checks" and "safeguards", meaning input data quality is expected to be "good".
-        4. Conti_cols are supposed to be "continuous" variables. In sklearn's mutual_info_classif, if you input a dense 
-            matrix X, it will always be treated as continuous, and if X is sparse, it will be treated as discrete.
-        5. This method is based on method described the sources.
-
-        Arguments:
-            df:
-            conti_cols: 
-            target: list of discrete columns.
-            n_neighbors:
-            random_state: a random seed to generate small noise.
-            n_threads: 
-            
-        Returns:
-
-        Sources:
-            (1). B. C. Ross “Mutual Information between Discrete and Continuous Data Sets”. PLoS ONE 9(2), 2014.\n
-            (2). A. Kraskov, H. Stogbauer and P. Grassberger, “Estimating mutual information”. Phys. Rev. E 69, 2004.
-            
-    '''
-    n = len(df)
-    rng = np.random.default_rng(seed)
-    target_col = df.get_column(target).to_numpy().ravel()
-    unique_targets = np.unique(target_col)
-    all_masks = {}
-    for t in unique_targets:
-        all_masks[t] = target_col == t
-        if np.sum(all_masks[t]) <= n_neighbors:
-            raise ValueError(f"The target class {t} must have more than {n_neighbors} values in the dataset.")        
-
-    estimates = []
-    psi_n_and_k = psi(n) + psi(n_neighbors)
-    for col in tqdm(conti_cols, desc = "Mutual Info"):
-        c = df.get_column(col).cast(pl.Float64).to_numpy().reshape(-1,1)
-        # Add random noise here because if inpute data is too big, then adding
-        # a random matrix of the same size will require a lot of memory upfront.
-        c = c + (1e-10 * np.mean(c) * rng.standard_normal(size=c.shape)) 
-        radius = np.empty(n)
-        label_counts = np.empty(n)
-        for t in unique_targets:
-            mask = all_masks[t]
-            c_masked = c[mask]
-            kd1 = KDTree(data=c_masked, leafsize=40)
-            # dd = distances from the points the the k nearest points. +1 because this starts from 0. It is 1 off from 
-            # sklearn's kdtree.
-            dd, _ = kd1.query(c_masked, k = n_neighbors + 1, workers=n_threads)
-            radius[mask] = np.nextafter(dd[:, -1], 0)
-            label_counts[mask] = np.sum(mask)
-
-        kd2 = KDTree(data=c, leafsize=40) 
-        m_all = kd2.query_ball_point(c, r = radius, return_length=True, workers=n_threads)
-        estimates.append(
-            max(0, psi_n_and_k - np.mean(psi(label_counts) + psi(m_all)))
-        ) # smallest is 0
-
-    return pl.from_records((conti_cols, estimates), schema=["feature", "estimated_mi"])
-
-# Selectors should always return target
-def mutual_info_selector(
-    df:PolarsFrame
-    , target:str
-    , n_neighbors:int=3
-    , seed:int=42
-    , n_threads:int=CPU_COUNT
-    , top_k:int = 50
-) -> PolarsFrame:
-    
-    is_lazy = isinstance(df, pl.LazyFrame)
-    if is_lazy:
-        input_data:pl.DataFrame = df.collect()
-    else:
-        input_data:pl.DataFrame = df
-
-    nums = get_numeric_cols(input_data, exclude=[target])
-    complement = [f for f in input_data.columns if f not in nums]
-
-    mi_scores = mutual_info(input_data, target, nums, n_neighbors, seed, n_threads)\
-                .top_k(by="estimated_mi", k = top_k)
-
-    selected = mi_scores.get_column("feature").to_list()
-    print(f"Selected {len(selected)} features. There are {len(complement)} columns the algorithm "
-        "cannot process. They are also returned.")
-    
-    if is_lazy:
-        return df.blueprint.select(selected + complement)
-    return df.select(selected + complement)
-
-def _f_score(
-    df:pl.DataFrame
-    , target:str
-    , num_list:list[str]
-) -> np.ndarray:
-    '''Same as f_classif, but returns a numpy array of f scores only.'''
-    
-    # See comments in f_classif
-    step_one_expr:list[pl.Expr] = [pl.count().alias("cnt")]
-    step_two_expr:list[pl.Expr] = []
-    step_three_expr:list[pl.Expr] = []
-    for n in num_list:
-        n_avg:str = n + "_avg"
-        n_tavg:str = n + "_tavg"
-        n_var:str = n + "_var"
-        step_one_expr.append(
-            pl.col(n).mean().alias(n_avg)
-        )
-        step_one_expr.append(
-            pl.col(n).var(ddof=0).alias(n_var)
-        )
-        step_two_expr.append(
-            (pl.col(n_avg).dot(pl.col("cnt")) / len(df)).alias(n_tavg)
-        )
-        step_three_expr.append(
-            (pl.col(n_avg) - pl.col(n_tavg)).pow(2).dot(pl.col("cnt"))/ pl.col(n_var).dot(pl.col("cnt"))
-        )
-
-    ref = df.groupby(target).agg(step_one_expr)
-    n_samples = len(df)
-    n_classes = len(ref)
-    df_btw_class = n_classes - 1 
-    df_in_class = n_samples - n_classes
-    # This is f-score, score in the order of num_list
-    return ref.with_columns(step_two_expr).select(step_three_expr)\
-            .to_numpy().ravel() * (df_in_class / df_btw_class)
-
-def f_classif(
-    df:pl.DataFrame
-    , target:str
-    , cols:Optional[list[str]]=None
-) -> pl.DataFrame:
-    '''Computes ANOVA one way test, the f value/score and the p value. 
-        Equivalent to f_classif in sklearn.feature_selection, but is more dataframe-friendly, 
-        and performs better on bigger data.
-
-        Arguments:
-            df: input Polars dataframe.
-            target: the target column.
-            cols: if provided, will run the ANOVA one way test for each column in num_cols. If none,
-                will try to infer from df according to data types. Note that num_cols should be numeric!
-
-        Returns:
-            a polars dataframe with f score and p value.
-    
-    '''
-    if isinstance(cols, list):
-        nums = cols
-    else:
-        nums = get_numeric_cols(df, exclude=[target])
-
-    # Get average within group and sample variance within group.
-    ## Could potentially replace this with generators instead of lists. Not sure how impactful that would be... Probably no diff.
-    step_one_expr:list[pl.Expr] = [pl.count().alias("cnt")] # get cnt, and avg within classes
-    step_two_expr:list[pl.Expr] = [] # Get average for each column
-    step_three_expr:list[pl.Expr] = [] # Get "f score" (without some normalizer, see below)
-    # Minimize the amount of looping and str concating in Python. Use Exprs as much as possible.
-    for n in nums:
-        n_avg:str = n + "_avg" # avg within class
-        n_tavg:str = n + "_tavg" # true avg / overall average
-        n_var:str = n + "_var" # var within class
-        step_one_expr.append(
-            pl.col(n).mean().alias(n_avg)
-        )
-        step_one_expr.append(
-            pl.col(n).var(ddof=0).alias(n_var) # ddof = 0 so that we don't need to compute pl.col("cnt") - 1
-        )
-        step_two_expr.append( # True average of this column, reduce the amount of repeated computation.
-            # by using n_avg column dotted with cnt
-            (pl.col(n_avg).dot(pl.col("cnt")) / len(df)).alias(n_tavg)
-        )
-        step_three_expr.append(
-            # Between class var (without diving by df_btw_class) / Within class var (without dividng by df_in_class) 
-            (pl.col(n_avg) - pl.col(n_tavg)).pow(2).dot(pl.col("cnt"))/ pl.col(n_var).dot(pl.col("cnt"))
-        )
-
-    # Get in class average and var
-    ref = df.groupby(target).agg(step_one_expr)
-    n_samples = len(df)
-    n_classes = len(ref)
-    df_btw_class = n_classes - 1 
-    df_in_class = n_samples - n_classes
-    
-    f_values = ref.with_columns(step_two_expr).select(step_three_expr)\
-            .to_numpy().ravel() * (df_in_class / df_btw_class)
-    # We should scale this by (df_in_class / df_btw_class) because we did not do this earlier
-    # At this point, f_values should be a pretty small dataframe. 
-    # Cast to numpy, so that fdtrc can process it properly.
-
-    p_values = fdtrc(df_btw_class, df_in_class, f_values) # get p values 
-    return pl.from_records((nums, f_values, p_values), schema=["feature","f_value","p_value"])
-
-def f_score_selector(
-    df:PolarsFrame
-    , target:str
-    , top_k:int
-) -> PolarsFrame:
-    
-    is_lazy = isinstance(df, pl.LazyFrame)
-    if is_lazy:
-        input_data:pl.DataFrame = df.collect()
-    else:
-        input_data:pl.DataFrame = df
-
-    nums = get_numeric_cols(input_data, exclude=[target])
-    # Non-numerical columns cannot be analyzed by mrmr. So add back in the end.
-    complement = [f for f in input_data.columns if f not in nums]
-
-    scores = _f_score(input_data, target, nums)
-    temp_df = pl.DataFrame({"feature":nums, "fscore":scores}).top_k(
-        by = "fscore", k = top_k
-    )
-    selected = temp_df.get_column("feature").to_list()
-    
-    print(f"Selected {len(selected)} features. There are {len(complement)} columns the algorithm "
-    "cannot process. They are also returned.")
-
-    if is_lazy:
-        return df.blueprint.select(selected + complement)
-    return df.select(selected + complement)
-
-#---- Below is MRMR
-
-def _mrmr_underlying_score(
-    df:pl.DataFrame
-    , target:str
-    , num_list:list[str]
-    , strategy:MRMRStrategy
-    , params:dict[str,Any]
-) -> np.ndarray:
-    
-    print(f"Running {strategy} to determine feature relevance...")
-    s = clean_strategy_str(strategy)
-    if s in ("fscore", "f", "f_score"):
-        scores = _f_score(df, target, num_list)
-    elif s in ("rf", "random_forest"):
-        from sklearn.ensemble import RandomForestClassifier
-        print("Random forest is not deterministic by default. Results may vary.")
-        rf = RandomForestClassifier(**params)
-        rf.fit(df[num_list].to_numpy(), df[target].to_numpy().ravel())
-        scores = rf.feature_importances_
-    elif s in ("xgb", "xgboost"):
-        from xgboost import XGBClassifier
-        print("XGB is not deterministic by default. Results may vary.")
-        xgb = XGBClassifier(**params)
-        xgb.fit(df[num_list].to_numpy(), df[target].to_numpy().ravel())
-        scores = xgb.feature_importances_
-    elif s in ("mis", "mutual_info_score"):
-        scores = mutual_info(df, conti_cols=num_list, target=target).get_column("estimated_mi").to_numpy().ravel()
-    elif s in ("lgbm", "lightgbm"):
-        from lightgbm import LGBMClassifier
-        print("LightGBM is not deterministic by default. Results may vary.")
-        lgbm = LGBMClassifier(**params)
-        lgbm.fit(df[num_list].to_numpy(), df[target].to_numpy().ravel())
-        scores = lgbm.feature_importances_
-    else: # Pythonic nonsense
-        raise ValueError(f"The strategy {strategy} is not a valid MRMR Strategy.")
-    
-    return scores
-
-def mrmr(
-    df:pl.DataFrame
-    , target:str
-    , k:int
-    , cols:Optional[list[str]] = None
-    , strategy: MRMRStrategy = "fscore"
-    , params:Optional[dict[str,Any]] = None
-    , low_memory:bool=False
-) -> list[str]:
-    '''Implements MRMR. Will add a few more strategies in the future. Likely only strategies for numerators
-        , aka relevance. Right now xgb, lgbm and rf strategies only work for classification problems.
-
-        Currently this only supports classification.
-
-        Arguments:
-            df:
-            target:
-            k:
-            cols: numerical columns
-            strategy: by default, f-score will be used.
-            params: if a RF/XGB strategy is selected, params is a dict of parameters for the model.
-            low_memory: 
-
-        Returns:
-            pl.DataFrame of features and the corresponding ranks according to the mrmr_algo
-    
-    '''
-    if isinstance(cols, list):
-        nums = cols
-    else:
-        nums = get_numeric_cols(df, exclude=[target])
-
-    s = clean_strategy_str(strategy)
-    scores = _mrmr_underlying_score(df
-        , target = target
-        , num_list = nums
-        , strategy = s
-        , params = {} if params is None else params
-    )
-
-    if low_memory:
-        df_local = df.select(nums)
-    else: # this could potentially double memory usage. so I provided a low_memory flag.
-        df_local = df.select(nums).with_columns(
-            (pl.col(f) - pl.col(f).mean())/pl.col(f).std() for f in nums
-        ) # Note that if we get a const column, the entire column will be NaN
-
-    output_size = min(k, len(nums))
-    print(f"Found {len(nums)} total features to select from. Proceeding to select top {output_size} features.")
-    cumulating_abs_corr = np.zeros(len(nums)) # For each feature at index i, we keep a cumulating sum
-    top_idx = np.argmax(scores)
-    selected = [nums[top_idx]]
-    pbar = tqdm(total=output_size, desc = f"MRMR, {s}")
-    pbar.update(1)
-    for j in range(1, output_size): 
-        argmax = -1
-        current_max = -1
-        last_selected_col = df_local.drop_in_place(selected[-1])
-        if low_memory: # normalize if in low memory mode.
-            last_selected_col = (last_selected_col - last_selected_col.mean())/last_selected_col.std()
-        for i,f in enumerate(nums):
-            if f not in selected:
-                # Left = cumulating sum of abs corr
-                # Right = abs correlation btw last_selected and f
-                candidate_col = df_local.get_column(f)
-                if low_memory: # normalize if in low memory mode.
-                    candidate_col = (candidate_col - candidate_col.mean())/candidate_col.std()
-
-                a = (last_selected_col*candidate_col).mean()
-                # In the rare case this calculation yields a NaN, we punish by adding 1.
-                # Otherwise, proceed as usual. +1 is a punishment because
-                # |corr| can be at most 1. So we are enlarging the denominator, thus reducing the score.
-                cumulating_abs_corr[i] += 1 if np.isnan(a) else np.abs(a)
-                denominator = cumulating_abs_corr[i]/j 
-                new_score = scores[i] / denominator
-                if new_score > current_max:
-                    current_max = new_score
-                    argmax = i
-
-        selected.append(nums[argmax])
-        pbar.update(1)
-
-    pbar.close()
-    print("Output is sorted in order of selection (relevance).")
-    return selected
-
-def mrmr_selector(
-    df:PolarsFrame
-    , target:str
-    , top_k:int
-    , strategy:MRMRStrategy = "fscore"
-    , params:Optional[dict[str,Any]] = None
-    , low_memory:bool=False
-) -> PolarsFrame:
-
-    is_lazy = isinstance(df, pl.LazyFrame)
-    if is_lazy:
-        input_data:pl.DataFrame = df.collect()
-    else:
-        input_data:pl.DataFrame = df
-
-    num_cols = get_numeric_cols(input_data, exclude=[target])
-    # Non-numerical columns cannot be analyzed by mrmr. So add back in the end.
-    complement = [f for f in input_data.columns if f not in num_cols]
-
-    s = clean_strategy_str(strategy)
-    selected = mrmr(input_data, target, top_k, num_cols, s, params, low_memory)
-
-    print(f"Selected {len(selected)} features. There are {len(complement)} columns the algorithm "
-          "cannot process. They are also returned.")
-    
-    if is_lazy:
-        return df.blueprint.select(selected + complement)
-    return df.select(selected + complement)
-
-def knock_out_mrmr(
-    df:pl.DataFrame
-    , target:str
-    , k:int 
-    , num_cols:Optional[list[str]] = None
-    , strategy:MRMRStrategy = "fscore"
-    , corr_threshold:float = 0.7
-    , params:Optional[dict[str,Any]] = None
-) -> list[str]:
-    '''
-        Essentially the same as vanilla MRMR. Instead of using sum(abs(corr)) to "weigh down" correlated 
-        variables, here we use a simpler knock out rule based on absolute correlation.
-
-        Inspired by the package Featurewiz and its creator.
-    
-    '''
-    if isinstance(num_cols, list):
-        num_list = num_cols
-    else:
-        num_list = get_numeric_cols(df, exclude=[target])
-
-    s = clean_strategy_str(strategy)
-    scores = _mrmr_underlying_score(df
-        , target = target
-        , num_list = num_list
-        , strategy = s
-        , params = {} if params is None else params
-    )
-
-    # Set up
-    low_corr = np.abs(df[num_list].corr().to_numpy()) < corr_threshold
-    surviving_indices = np.full(shape=len(num_list), fill_value=True) # an array of booleans
-    scores = list(enumerate(scores))
-    scores.sort(key=lambda x:x[1], reverse=True)
-    selected = []
-    count = 0
-    output_size = min(k, len(num_list))
-    pbar = tqdm(total=output_size)
-    # Run the knock outs
-    for i, _ in scores:
-        if surviving_indices[i]:
-            selected.append(num_list[i])
-            surviving_indices = surviving_indices & low_corr[:,i]
-            count += 1
-            pbar.update(1)
-        if count >= output_size:
-            break
-
-    pbar.close()
-    if count < k:
-        print(f"Found only {count}/{k} number of values because most of them are highly correlated and the knock out "
-              "rule eliminates most of them.")
-
-    print("Output is sorted in order of selection (relevance).")
-    return selected
-
-def knock_out_mrmr_selector(
-    df:PolarsFrame
-    , target:str
-    , top_k:int 
-    , strategy:MRMRStrategy = "fscore"
-    , corr_threshold:float = 0.7
-    , params:Optional[dict[str,Any]] = None
-) -> PolarsFrame:
-
-    is_lazy = isinstance(df, pl.LazyFrame)
-    if isinstance(df, pl.LazyFrame):
-        input_data:pl.DataFrame = df.collect()
-    else:
-        input_data:pl.DataFrame = df
-
-    num_cols = get_numeric_cols(df, exclude=[target])
-    # Non-numerical columns cannot be analyzed by mrmr. So add back in the end.
-    complement = [f for f in df.columns if f not in num_cols]
-
-    s = clean_strategy_str(strategy)
-    selected = knock_out_mrmr(input_data, target, top_k, num_cols, s, corr_threshold, params)
-    print(f"Selected {len(selected)} features. There are {len(complement)} columns the algorithm "
-        "cannot process. They are also returned.")
-    
-    if is_lazy:
-        return df.blueprint.select(selected + complement)
-    return df.select(selected + complement)
-
-# Selectors for the methods below are not yet implemented
-
-# Create a numeric + string version of woe_iv in the future
-def woe_iv_cat(
-    df:PolarsFrame
-    , target:str
-    , cols:Optional[list[str]]=None
-    , min_count:float = 1.
-    , check_binary:bool = True
-) -> pl.DataFrame:
-    '''
-        Arguments:
-            df: ..
-            target: ..
-            cols: a list of string or highly discrete numeric columns. Currently woe_iv for continuous values
-            is not implemenented. If not provided, it will use only string columns.
-            min_count: a regularization term that prevents ln(0). This is the same as 
-            category_encoders package's regularization parameter.
-            check_binary: whether to check if target is binary or not
-    '''
-    if isinstance(cols, list):
-        input_cols = cols
-    else:
-        input_cols = get_string_cols(df)
-
-    if check_binary:
-        if not check_binary_target(df, target):
-            raise ValueError("Target is not binary or not properly encoded.")
-
-    # No tqdm then..
-    results = (
-        df.lazy().groupby(s).agg(
-            ev = pl.col(target).sum()
-            , nonev = (pl.lit(1) - pl.col(target)).sum()
-        ).with_columns(
-            ev_rate = (pl.col("ev") + min_count)/(pl.col("ev").sum() + 2.0*min_count)
-            , nonev_rate = (pl.col("nonev") + min_count)/(pl.col("nonev").sum() + 2.0*min_count)
-        ).with_columns(
-            woe = (pl.col("ev_rate")/pl.col("nonev_rate")).log()
-        ).select(
-            pl.lit(s).alias("feature")
-            , pl.col(s).alias("value")
-            , pl.col("woe")
-            , information_value = ((pl.col("ev_rate")-pl.col("nonev_rate")) * pl.col("woe")).sum()
-        )
-        for s in input_cols
-    )
-    return pl.concat(results).collect()
-
-def _binary_model_init(
-    model:BinaryModels
-    , params: dict[str, Any]
-):
-    if "n_jobs" not in params:
-        params["n_jobs"] = -1
-
-    if model in ("logistic", "lr"):
-        from sklearn.linear_model import LogisticRegression
-        model = LogisticRegression(**params)
-    elif model in ("rf", "random_forest"):
-        from sklearn.ensemble import RandomForestClassifier
-        model = RandomForestClassifier(**params)
-    elif model in ("xgb", "xgboost"):
-        from xgboost import XGBClassifier
-        model = XGBClassifier(**params)
-    elif model in ("lgbm", "lightgbm"):
-        from lightgbm import LGBMClassifier
-        model = LGBMClassifier(**params)
-    else:
-        raise ValueError(f"The model {model} is not available.")
-    
-    return model
-
-def _ebfs(
-    model:str
-    , params:dict[str, Any]
-    , target:str
-    , comb: Tuple
-    , train: pl.DataFrame
-    , test:pl.DataFrame
-)-> Tuple[Tuple[Tuple, float, float, float], np.ndarray]:
-    estimator = _binary_model_init(model, params)
-    _ = estimator.fit(train.select(comb), train[target])
-    y_pred = estimator.predict_proba(test.select(comb))[:,1]
-    y_test = test[target].to_numpy()
-    rec = (
-        comb,
-        logloss(y_test, y_pred, check_binary=False),
-        roc_auc(y_test, y_pred, check_binary=False)
-    )
-    if model in ("lr", "logistic"):
-        importances = np.abs(estimator.coef_).ravel()
-    else:
-        importances = estimator.feature_importances_
-
-    return rec, importances
-
-# ebfs: stands for Exhaustive Binary Feature Selection
-def ebfs(
-    df:pl.DataFrame
-    , target:str
-    , model:BinaryModels
-    , params:dict[str, Any]
-    , n_comb: int = 3
-    , train_frac:float = 0.75
-) -> Tuple[pl.DataFrame, pl.DataFrame]:
-    '''Suppose we have n features and n_comb = 2. This method will select all (n choose 2) 
-    combinations of features, split dataset into a train and a test, train a model on train, 
-    and compute feature importance and roc_auc and logloss, and then finally put 
-    everything into two separate dataframes, the first of which will contain the feature
-    combinations and model performances, and the second will contain the min, avg, max and var of 
-    feature importance of each feature in all its occurences in the training rounds.
-
-    This method will be extremely slow if (n choose n_comb) is a big number. All numerical columns 
-    will be taken as potential features. Please encode the string columns if you want to use them
-    as features here.
-
-    Future Improvement? Record progress and skip through results.
-
-    If n_jobs is not provided in params, it will be defaulted to -1.
-
-        Arguments:
-            df: an eager Polars DataFrame
-            target: target column
-            model: one of 'logistic', 'lr', 'lightgbm', 'lgbm', 'xgboost', 'xgb', 'random_forest', 'rf'
-            params: parameters for the model.
-            n_comb: n choose n_comb
-
-        Returns:
-            a feature combination summary, a feature importance summary
-    '''
-    
-    features = get_numeric_cols(df, exclude=[target])
-    train, test = train_test_split(df.select(features + [target]), train_frac)
-    fi = {f:[] for f in features}
-    records = []
-    pbar = tqdm(total=math.comb(len(features), n_comb), desc="Total Combinations")
-    with ThreadPoolExecutor(max_workers=CPU_COUNT) as ex:
-        futures = (
-            ex.submit(
-                _ebfs
-                , model
-                , params
-                , target
-                , comb
-                , train
-                , test
-            )
-            for comb in combinations(features, r=n_comb)
-        )
-        for f in as_completed(futures):
-            fc_rec, fi_rec = f.result()
-            records.append(fc_rec)
-            for f, i in zip(fc_rec[0], fi_rec):
-                fi[f].append(i)
-            pbar.update(1)
-
-    fc_summary = pl.from_records(records, schema=["combination", "logloss", "roc_auc"])
-    stats = [
-        (f, len(fi[f]), np.min(fi[f]), np.mean(fi[f]), np.max(fi[f]), np.std(fi[f])) for f in fi
-    ]
-    fi_summary = pl.from_records(stats, schema=["feature", "occurrences", "min", "mean", "max", "std"])
-    pbar.close()
-    return fc_summary, fi_summary
-
-def ebfs_fc_filter(
-    fc: pl.DataFrame
-    , logloss_threshold:float
-    , roc_auc_threshold:float
-) -> list[str]:
-    '''A filter method based on the feature combination result of ebfs. First, 
-
-        Arguments:
-            fc: the feature combination result from ebfs
-            logloss_threshold: the maximum logloss for the combination to be kept
-            roc_auc_threshold: the minumum roc_auc for the combination to be kept
-
-        Returns:
-            a list of string representing all features in the combinations after filtering
-    '''
-    return fc.filter(
-        pl.col("logloss") <= logloss_threshold
-        & pl.col("roc_auc") >= roc_auc_threshold
-    ).get_column("combination").explode().unique().to_list()
-
-
+from .prescreen import (
+    discrete_inferral
+    , check_binary_target
+    , get_numeric_cols
+    , get_unique_count
+    , get_string_cols
+)
+
+from .type_alias import (
+    PolarsFrame
+    , MRMRStrategy
+    , BinaryModels
+    , CPU_COUNT
+    , clean_strategy_str
+)
+from .blueprint import( # Need this for Polars extension to work
+    Blueprint
+)
+from .sample import (
+    train_test_split
+)
+from .metrics import (
+    logloss
+    , roc_auc
+)
+import polars as pl
+import numpy as np
+from typing import Any, Optional, Tuple
+from scipy.spatial import KDTree
+from scipy.special import fdtrc, psi
+from concurrent.futures import ThreadPoolExecutor, as_completed
+from tqdm import tqdm
+import math
+from itertools import combinations
+
+def _conditional_entropy(
+    df:pl.DataFrame
+    , target:str
+    , predictive:str
+) -> Tuple[str, float]:
+
+    cond_entropy = df.groupby((target, predictive)).agg(
+        pl.count()
+    ).with_columns(
+        (pl.col("count").sum().over(predictive) / len(df)).alias("prob(predictive)"),
+        (pl.col("count") / pl.col("count").sum()).alias("prob(target,predictive)")
+    ).select(
+        (-((pl.col("prob(target,predictive)")/pl.col("prob(predictive)")).log() 
+           * pl.col("prob(target,predictive)")).sum()) # This is the conditional entropy.
+    ).row(0)[0]
+
+    return (predictive, cond_entropy)
+
+# !!!NEED REVIEW FOR CORRECTNESS
+def discrete_ig(
+    df:pl.DataFrame
+    , target:str
+    , cols:Optional[list[str]] = None
+    , n_threads:int = CPU_COUNT
+) -> pl.DataFrame:
+    '''The entropy here is "discrete entropy".
+
+        Computes the information gain: Entropy(target) - Conditional_Entropy(target|c), where c is a column in 
+        discrete_cols. For more information, please take a look at https://en.wikipedia.org/wiki/Entropy_(information_theory)
+
+        Information gain defined in this way suffers from high cardinality (high uniqueness), and therefore a weighted 
+        information gain is provided, weighted by (1 - unique_pct), where unique_pct represents the percentage of unique
+         values in feature.
+
+        Currently this only works for discrete columns. For continuous features vs discrete target, use mutual_info.
+
+        Arguments:
+            df: Eager frame only.
+            target:
+            cols: list of discrete columns. If not provided, they will be inferred.
+            top_k: must be >= 0. If <= 0, the entire DataFrame will be returned.
+            n_threads: 4, 8 ,16 will not make any real difference. But there is a difference between 0 and 4 threads. 
+            
+        Returns:
+            a poalrs dataframe with information gain computed for each categorical column. 
+    '''
+    output = []
+    if isinstance(cols, list):
+        discretes = cols
+    else: # If discrete_cols is not passed, infer it
+        discretes = discrete_inferral(df, exclude=[target])
+
+    # Compute target entropy. This only needs to be done once.
+    target_entropy = df.groupby(target).agg(
+                        (pl.count()).alias("prob(target)") / len(df)
+                    ).get_column("prob(target)").entropy()
+
+    # Get unique count for selected columns. This is because higher unique percentage may skew information gain
+    unique_count = get_unique_count(df.select(discretes)).with_columns(
+        (pl.col("n_unique") / len(df)).alias("unique_pct")
+    ).rename({"column":"feature"})
+
+    with ThreadPoolExecutor(max_workers=n_threads) as ex: # 10% speed gain ? Need to retest this..
+        pbar = tqdm(total=len(discretes), desc = "discrete_ig")
+        for f in as_completed(ex.submit(_conditional_entropy, df, target, pred) for pred in discretes):
+            output.append(f.result())
+            pbar.update(1)
+        pbar.close()
+
+    return pl.from_records(output, schema=["feature", "conditional_entropy"])\
+        .with_columns(
+            target_entropy = pl.lit(target_entropy),
+            information_gain = pl.lit(target_entropy) - pl.col("conditional_entropy")
+        ).join(unique_count, on="feature")\
+        .select("feature", "target_entropy", "conditional_entropy", "unique_pct", "information_gain")\
+        .with_columns(
+            weighted_information_gain = (1 - pl.col("unique_pct")) * pl.col("information_gain")
+        )
+
+discrete_mi = discrete_ig
+
+def discrete_ig_selector(
+    df:PolarsFrame
+    , target:str
+    , top_k:int
+    , n_threads:int = CPU_COUNT
+) -> PolarsFrame:
+    
+    discrete_cols = discrete_inferral(df, exclude=[target])
+    is_lazy = isinstance(df, pl.LazyFrame)
+    if is_lazy:
+        input_data:pl.DataFrame = df.collect()
+    else:
+        input_data:pl.DataFrame = df
+
+    ig = discrete_ig(input_data, target, discrete_cols, n_threads)\
+            .top_k(by="information_gain", k = top_k)
+
+    complement = [f for f in input_data.columns if f not in discrete_cols]
+    selected = ig.get_column("feature").to_list()
+    print(f"Selected {len(selected)} features. There are {len(complement)} columns the algorithm "
+        "cannot process. They are also returned.")
+
+    if is_lazy:
+        return df.blueprint.select(selected + complement)
+    return df.select(selected + complement)
+
+def mutual_info(
+    df:pl.DataFrame
+    , target:str
+    , conti_cols:list[str]
+    , n_neighbors:int=3
+    , seed:int=42
+    , n_threads:int=CPU_COUNT
+) -> pl.DataFrame:
+    '''Approximates mutual information (information gain) between the continuous variables and the target.
+
+        This is essentially a "copy-and-paste" of the mutual_info_classif call in sklearn library. 
+        There are a few important distinctions:
+
+        1. This uses Scipy library's kdtree, instead of sklearn's kdtree and nearneighbors. 
+        2. The use of Scipy enables us to use more cores. 
+        3. There are less "checks" and "safeguards", meaning input data quality is expected to be "good".
+        4. Conti_cols are supposed to be "continuous" variables. In sklearn's mutual_info_classif, if you input a dense 
+            matrix X, it will always be treated as continuous, and if X is sparse, it will be treated as discrete.
+        5. This method is based on method described the sources.
+
+        Arguments:
+            df:
+            conti_cols: 
+            target: list of discrete columns.
+            n_neighbors:
+            random_state: a random seed to generate small noise.
+            n_threads: 
+            
+        Returns:
+
+        Sources:
+            (1). B. C. Ross “Mutual Information between Discrete and Continuous Data Sets”. PLoS ONE 9(2), 2014.\n
+            (2). A. Kraskov, H. Stogbauer and P. Grassberger, “Estimating mutual information”. Phys. Rev. E 69, 2004.
+            
+    '''
+    n = len(df)
+    rng = np.random.default_rng(seed)
+    target_col = df.get_column(target).to_numpy().ravel()
+    unique_targets = np.unique(target_col)
+    all_masks = {}
+    for t in unique_targets:
+        all_masks[t] = target_col == t
+        if np.sum(all_masks[t]) <= n_neighbors:
+            raise ValueError(f"The target class {t} must have more than {n_neighbors} values in the dataset.")        
+
+    estimates = []
+    psi_n_and_k = psi(n) + psi(n_neighbors)
+    for col in tqdm(conti_cols, desc = "Mutual Info"):
+        c = df.get_column(col).cast(pl.Float64).to_numpy().reshape(-1,1)
+        # Add random noise here because if inpute data is too big, then adding
+        # a random matrix of the same size will require a lot of memory upfront.
+        c = c + (1e-10 * np.mean(c) * rng.standard_normal(size=c.shape)) 
+        radius = np.empty(n)
+        label_counts = np.empty(n)
+        for t in unique_targets:
+            mask = all_masks[t]
+            c_masked = c[mask]
+            kd1 = KDTree(data=c_masked, leafsize=40)
+            # dd = distances from the points the the k nearest points. +1 because this starts from 0. It is 1 off from 
+            # sklearn's kdtree.
+            dd, _ = kd1.query(c_masked, k = n_neighbors + 1, workers=n_threads)
+            radius[mask] = np.nextafter(dd[:, -1], 0)
+            label_counts[mask] = np.sum(mask)
+
+        kd2 = KDTree(data=c, leafsize=40) 
+        m_all = kd2.query_ball_point(c, r = radius, return_length=True, workers=n_threads)
+        estimates.append(
+            max(0, psi_n_and_k - np.mean(psi(label_counts) + psi(m_all)))
+        ) # smallest is 0
+
+    return pl.from_records((conti_cols, estimates), schema=["feature", "estimated_mi"])
+
+# Selectors should always return target
+def mutual_info_selector(
+    df:PolarsFrame
+    , target:str
+    , n_neighbors:int=3
+    , seed:int=42
+    , n_threads:int=CPU_COUNT
+    , top_k:int = 50
+) -> PolarsFrame:
+    
+    is_lazy = isinstance(df, pl.LazyFrame)
+    if is_lazy:
+        input_data:pl.DataFrame = df.collect()
+    else:
+        input_data:pl.DataFrame = df
+
+    nums = get_numeric_cols(input_data, exclude=[target])
+    complement = [f for f in input_data.columns if f not in nums]
+
+    mi_scores = mutual_info(input_data, target, nums, n_neighbors, seed, n_threads)\
+                .top_k(by="estimated_mi", k = top_k)
+
+    selected = mi_scores.get_column("feature").to_list()
+    print(f"Selected {len(selected)} features. There are {len(complement)} columns the algorithm "
+        "cannot process. They are also returned.")
+
+    if is_lazy:
+        return df.blueprint.select(selected + complement)
+    return df.select(selected + complement)
+
+def _f_score(
+    df:pl.DataFrame
+    , target:str
+    , num_list:list[str]
+) -> np.ndarray:
+    '''Same as f_classif, but returns a numpy array of f scores only.'''
+    
+    # See comments in f_classif
+    step_one_expr:list[pl.Expr] = [pl.count().alias("cnt")]
+    step_two_expr:list[pl.Expr] = []
+    step_three_expr:list[pl.Expr] = []
+    for n in num_list:
+        n_avg:str = n + "_avg"
+        n_tavg:str = n + "_tavg"
+        n_var:str = n + "_var"
+        step_one_expr.append(
+            pl.col(n).mean().alias(n_avg)
+        )
+        step_one_expr.append(
+            pl.col(n).var(ddof=0).alias(n_var)
+        )
+        step_two_expr.append(
+            (pl.col(n_avg).dot(pl.col("cnt")) / len(df)).alias(n_tavg)
+        )
+        step_three_expr.append(
+            (pl.col(n_avg) - pl.col(n_tavg)).pow(2).dot(pl.col("cnt"))/ pl.col(n_var).dot(pl.col("cnt"))
+        )
+
+    ref = df.groupby(target).agg(step_one_expr)
+    n_samples = len(df)
+    n_classes = len(ref)
+    df_btw_class = n_classes - 1 
+    df_in_class = n_samples - n_classes
+    # This is f-score, score in the order of num_list
+    return ref.with_columns(step_two_expr).select(step_three_expr)\
+            .to_numpy().ravel() * (df_in_class / df_btw_class)
+
+def f_classif(
+    df:pl.DataFrame
+    , target:str
+    , cols:Optional[list[str]]=None
+) -> pl.DataFrame:
+    '''Computes ANOVA one way test, the f value/score and the p value. 
+        Equivalent to f_classif in sklearn.feature_selection, but is more dataframe-friendly, 
+        and performs better on bigger data.
+
+        Arguments:
+            df: input Polars dataframe.
+            target: the target column.
+            cols: if provided, will run the ANOVA one way test for each column in num_cols. If none,
+                will try to infer from df according to data types. Note that num_cols should be numeric!
+
+        Returns:
+            a polars dataframe with f score and p value.
+    
+    '''
+    if isinstance(cols, list):
+        nums = cols
+    else:
+        nums = get_numeric_cols(df, exclude=[target])
+
+    # Get average within group and sample variance within group.
+    ## Could potentially replace this with generators instead of lists. Not sure how impactful that would be... Probably no diff.
+    step_one_expr:list[pl.Expr] = [pl.count().alias("cnt")] # get cnt, and avg within classes
+    step_two_expr:list[pl.Expr] = [] # Get average for each column
+    step_three_expr:list[pl.Expr] = [] # Get "f score" (without some normalizer, see below)
+    # Minimize the amount of looping and str concating in Python. Use Exprs as much as possible.
+    for n in nums:
+        n_avg:str = n + "_avg" # avg within class
+        n_tavg:str = n + "_tavg" # true avg / overall average
+        n_var:str = n + "_var" # var within class
+        step_one_expr.append(
+            pl.col(n).mean().alias(n_avg)
+        )
+        step_one_expr.append(
+            pl.col(n).var(ddof=0).alias(n_var) # ddof = 0 so that we don't need to compute pl.col("cnt") - 1
+        )
+        step_two_expr.append( # True average of this column, reduce the amount of repeated computation.
+            # by using n_avg column dotted with cnt
+            (pl.col(n_avg).dot(pl.col("cnt")) / len(df)).alias(n_tavg)
+        )
+        step_three_expr.append(
+            # Between class var (without diving by df_btw_class) / Within class var (without dividng by df_in_class) 
+            (pl.col(n_avg) - pl.col(n_tavg)).pow(2).dot(pl.col("cnt"))/ pl.col(n_var).dot(pl.col("cnt"))
+        )
+
+    # Get in class average and var
+    ref = df.groupby(target).agg(step_one_expr)
+    n_samples = len(df)
+    n_classes = len(ref)
+    df_btw_class = n_classes - 1 
+    df_in_class = n_samples - n_classes
+    
+    f_values = ref.with_columns(step_two_expr).select(step_three_expr)\
+            .to_numpy().ravel() * (df_in_class / df_btw_class)
+    # We should scale this by (df_in_class / df_btw_class) because we did not do this earlier
+    # At this point, f_values should be a pretty small dataframe. 
+    # Cast to numpy, so that fdtrc can process it properly.
+
+    p_values = fdtrc(df_btw_class, df_in_class, f_values) # get p values 
+    return pl.from_records((nums, f_values, p_values), schema=["feature","f_value","p_value"])
+
+def f_score_selector(
+    df:PolarsFrame
+    , target:str
+    , top_k:int
+) -> PolarsFrame:
+    
+    is_lazy = isinstance(df, pl.LazyFrame)
+    if is_lazy:
+        input_data:pl.DataFrame = df.collect()
+    else:
+        input_data:pl.DataFrame = df
+
+    nums = get_numeric_cols(input_data, exclude=[target])
+    # Non-numerical columns cannot be analyzed by mrmr. So add back in the end.
+    complement = [f for f in input_data.columns if f not in nums]
+
+    scores = _f_score(input_data, target, nums)
+    temp_df = pl.DataFrame({"feature":nums, "fscore":scores}).top_k(
+        by = "fscore", k = top_k
+    )
+    selected = temp_df.get_column("feature").to_list()
+    
+    print(f"Selected {len(selected)} features. There are {len(complement)} columns the algorithm "
+    "cannot process. They are also returned.")
+
+    if is_lazy:
+        return df.blueprint.select(selected + complement)
+    return df.select(selected + complement)
+
+def _mrmr_underlying_score(
+    df:pl.DataFrame
+    , target:str
+    , num_list:list[str]
+    , strategy:MRMRStrategy
+    , params:dict[str,Any]
+) -> np.ndarray:
+    
+    print(f"Running {strategy} to determine feature relevance...")
+    s = clean_strategy_str(strategy)
+    if s in ("fscore", "f", "f_score"):
+        scores = _f_score(df, target, num_list)
+    elif s in ("rf", "random_forest"):
+        from sklearn.ensemble import RandomForestClassifier
+        print("Random forest is not deterministic by default. Results may vary.")
+        rf = RandomForestClassifier(**params)
+        rf.fit(df[num_list].to_numpy(), df[target].to_numpy().ravel())
+        scores = rf.feature_importances_
+    elif s in ("xgb", "xgboost"):
+        from xgboost import XGBClassifier
+        print("XGB is not deterministic by default. Results may vary.")
+        xgb = XGBClassifier(**params)
+        xgb.fit(df[num_list].to_numpy(), df[target].to_numpy().ravel())
+        scores = xgb.feature_importances_
+    elif s in ("mis", "mutual_info_score"):
+        scores = mutual_info(df, conti_cols=num_list, target=target).get_column("estimated_mi").to_numpy().ravel()
+    elif s in ("lgbm", "lightgbm"):
+        from lightgbm import LGBMClassifier
+        print("LightGBM is not deterministic by default. Results may vary.")
+        lgbm = LGBMClassifier(**params)
+        lgbm.fit(df[num_list].to_numpy(), df[target].to_numpy().ravel())
+        scores = lgbm.feature_importances_
+    else: # Pythonic nonsense
+        raise ValueError(f"The strategy {strategy} is not a valid MRMR Strategy.")
+    
+    return scores
+
+def mrmr(
+    df:pl.DataFrame
+    , target:str
+    , k:int
+    , cols:Optional[list[str]] = None
+    , strategy: MRMRStrategy = "fscore"
+    , params:Optional[dict[str,Any]] = None
+    , low_memory:bool=False
+) -> list[str]:
+    '''
+    Implements MRMR. Will add a few more strategies in the future. Likely only strategies for numerators
+    , aka relevance. Right now xgb, lgbm and rf strategies only work for classification problems.
+
+    Currently this only supports classification.
+
+    Parameters
+    ----------
+    df
+        An eager Polars Dataframe
+    target
+        Target column
+    k
+        Top k features to keep
+    cols
+        Optional. A list of numerical columns. If not provided, all numerical columns will be used.
+    strategy
+        MRMR strategy. By default, `fscore` will be used.
+    params
+        Optional. If a model strategy is selected (`rf`, `xgb`, `lgbm`), params is a dict of 
+        parameters for the model.
+    low_memory
+        Whether to do some computation all at once, which uses more memory at once, or do some 
+        computation when needed, which uses less memory at any given time.
+
+    Returns
+    -------
+        A list of top k features
+    
+    '''
+    if isinstance(cols, list):
+        nums = cols
+    else:
+        nums = get_numeric_cols(df, exclude=[target])
+
+    s = clean_strategy_str(strategy)
+    scores = _mrmr_underlying_score(df
+        , target = target
+        , num_list = nums
+        , strategy = s
+        , params = {} if params is None else params
+    )
+
+    if low_memory:
+        df_local = df.select(nums)
+    else: # this could potentially double memory usage. so I provided a low_memory flag.
+        df_local = df.select(nums).with_columns(
+            (pl.col(f) - pl.col(f).mean())/pl.col(f).std() for f in nums
+        ) # Note that if we get a const column, the entire column will be NaN
+
+    output_size = min(k, len(nums))
+    print(f"Found {len(nums)} total features to select from. Proceeding to select top {output_size} features.")
+    cumulating_abs_corr = np.zeros(len(nums)) # For each feature at index i, we keep a cumulating sum
+    top_idx = np.argmax(scores)
+    selected = [nums[top_idx]]
+    pbar = tqdm(total=output_size, desc = f"MRMR, {s}")
+    pbar.update(1)
+    for j in range(1, output_size): 
+        argmax = -1
+        current_max = -1
+        last_selected_col = df_local.drop_in_place(selected[-1])
+        if low_memory: # normalize if in low memory mode.
+            last_selected_col = (last_selected_col - last_selected_col.mean())/last_selected_col.std()
+        for i,f in enumerate(nums):
+            if f not in selected:
+                # Left = cumulating sum of abs corr
+                # Right = abs correlation btw last_selected and f
+                candidate_col = df_local.get_column(f)
+                if low_memory: # normalize if in low memory mode.
+                    candidate_col = (candidate_col - candidate_col.mean())/candidate_col.std()
+
+                a = (last_selected_col*candidate_col).mean()
+                # In the rare case this calculation yields a NaN, we punish by adding 1.
+                # Otherwise, proceed as usual. +1 is a punishment because
+                # |corr| can be at most 1. So we are enlarging the denominator, thus reducing the score.
+                cumulating_abs_corr[i] += 1 if np.isnan(a) else np.abs(a)
+                denominator = cumulating_abs_corr[i]/j 
+                new_score = scores[i] / denominator
+                if new_score > current_max:
+                    current_max = new_score
+                    argmax = i
+        selected.append(nums[argmax])
+        pbar.update(1)
+
+    pbar.close()
+    print("Output is sorted in order of selection (max relevance min redundancy).")
+    return selected
+
+def mrmr_selector(
+    df:PolarsFrame
+    , target:str
+    , top_k:int
+    , strategy:MRMRStrategy = "fscore"
+    , params:Optional[dict[str,Any]] = None
+    , low_memory:bool=False
+) -> PolarsFrame:
+
+    is_lazy = isinstance(df, pl.LazyFrame)
+    if is_lazy:
+        input_data:pl.DataFrame = df.collect()
+    else:
+        input_data:pl.DataFrame = df
+
+    nums = get_numeric_cols(input_data, exclude=[target])
+    # Non-numerical columns cannot be analyzed by mrmr. So add back in the end.
+    complement = [f for f in input_data.columns if f not in nums]
+    s = clean_strategy_str(strategy)
+    selected = mrmr(input_data, target, top_k, nums, s, params, low_memory)
+
+    print(f"Selected {len(selected)} features. There are {len(complement)} columns the algorithm "
+          "cannot process. They are also returned.")
+    
+    if is_lazy:
+        return df.blueprint.select(selected + complement)
+    return df.select(selected + complement)
+
+def knock_out_mrmr(
+    df:pl.DataFrame
+    , target:str
+    , k:int 
+    , num_cols:Optional[list[str]] = None
+    , strategy:MRMRStrategy = "fscore"
+    , corr_threshold:float = 0.7
+    , params:Optional[dict[str,Any]] = None
+) -> list[str]:
+    '''
+    Essentially the same as vanilla MRMR. Instead of using sum(abs(corr)) to "weigh down" correlated 
+    variables, here we use a simpler knock out rule based on absolute correlation. We go down the list
+    according to importance, take top one, knock out all other features that are highly correlated with
+    it, take the next top feature that has not been knocked out, continue, until we pick enough features
+    or there is no feature left.
+
+    Inspired by the package Featurewiz and its creator.
+
+
+    
+    '''
+    if isinstance(num_cols, list):
+        num_list = num_cols
+    else:
+        num_list = get_numeric_cols(df, exclude=[target])
+
+    s = clean_strategy_str(strategy)
+    scores = _mrmr_underlying_score(df
+        , target = target
+        , num_list = num_list
+        , strategy = s
+        , params = {} if params is None else params
+    )
+
+    # Set up
+    low_corr = np.abs(df[num_list].corr().to_numpy()) < corr_threshold
+    surviving_indices = np.full(shape=len(num_list), fill_value=True) # an array of booleans
+    scores = sorted(enumerate(scores), key=lambda x:x[1], reverse=True)
+    selected = []
+    count = 0
+    output_size = min(k, len(num_list))
+    pbar = tqdm(total=output_size)
+    # Run the knock outs
+    for i, _ in scores:
+        if surviving_indices[i]:
+            selected.append(num_list[i])
+            surviving_indices = surviving_indices & low_corr[:,i]
+            count += 1
+            pbar.update(1)
+        if count >= output_size:
+            break
+
+    pbar.close()
+    if count < k:
+        print(f"Found only {count}/{k} number of values because most of them are highly correlated and the knock out "
+              "rule eliminates most of them.")
+
+    print("Output is sorted in order of selection (max relevance min redundancy).")
+    return selected
+
+def knock_out_mrmr_selector(
+    df:PolarsFrame
+    , target:str
+    , top_k:int 
+    , strategy:MRMRStrategy = "fscore"
+    , corr_threshold:float = 0.7
+    , params:Optional[dict[str,Any]] = None
+) -> PolarsFrame:
+
+    is_lazy = isinstance(df, pl.LazyFrame)
+    if isinstance(df, pl.LazyFrame):
+        input_data:pl.DataFrame = df.collect()
+    else:
+        input_data:pl.DataFrame = df
+
+    num_cols = get_numeric_cols(df, exclude=[target])
+    # Non-numerical columns cannot be analyzed by mrmr. So add back in the end.
+    complement = [f for f in df.columns if f not in num_cols]
+
+    s = clean_strategy_str(strategy)
+    selected = knock_out_mrmr(input_data, target, top_k, num_cols, s, corr_threshold, params)
+    print(f"Selected {len(selected)} features. There are {len(complement)} columns the algorithm "
+        "cannot process. They are also returned.")
+    
+    if is_lazy:
+        return df.blueprint.select(selected + complement)
+    return df.select(selected + complement)
+
+# Selectors for the methods below are not yet implemented
+
+# Create a numeric + string version of woe_iv in the future
+def woe_iv_cat(
+    df:PolarsFrame
+    , target:str
+    , cols:Optional[list[str]]=None
+    , min_count:float = 1.
+    , check_binary:bool = True
+) -> pl.DataFrame:
+    '''
+        Arguments:
+            df: ..
+            target: ..
+            cols: a list of string or highly discrete numeric columns. Currently woe_iv for continuous values
+            is not implemenented. If not provided, it will use only string columns.
+            min_count: a regularization term that prevents ln(0). This is the same as 
+            category_encoders package's regularization parameter.
+            check_binary: whether to check if target is binary or not
+    '''
+    if isinstance(cols, list):
+        input_cols = cols
+    else:
+        input_cols = get_string_cols(df)
+
+    if check_binary:
+        if not check_binary_target(df, target):
+            raise ValueError("Target is not binary or not properly encoded.")
+
+    # No tqdm then..
+    results = (
+        df.lazy().groupby(s).agg(
+            ev = pl.col(target).sum()
+            , nonev = (pl.lit(1) - pl.col(target)).sum()
+        ).with_columns(
+            ev_rate = (pl.col("ev") + min_count)/(pl.col("ev").sum() + 2.0*min_count)
+            , nonev_rate = (pl.col("nonev") + min_count)/(pl.col("nonev").sum() + 2.0*min_count)
+        ).with_columns(
+            woe = (pl.col("ev_rate")/pl.col("nonev_rate")).log()
+        ).select(
+            pl.lit(s).alias("feature")
+            , pl.col(s).alias("value")
+            , pl.col("woe")
+            , information_value = ((pl.col("ev_rate")-pl.col("nonev_rate")) * pl.col("woe")).sum()
+        )
+        for s in input_cols
+    )
+    return pl.concat(results).collect()
+
+def _binary_model_init(
+    model:BinaryModels
+    , params: dict[str, Any]
+):
+    if "n_jobs" not in params:
+        params["n_jobs"] = -1
+
+    if model in ("logistic", "lr"):
+        from sklearn.linear_model import LogisticRegression
+        model = LogisticRegression(**params)
+    elif model in ("rf", "random_forest"):
+        from sklearn.ensemble import RandomForestClassifier
+        model = RandomForestClassifier(**params)
+    elif model in ("xgb", "xgboost"):
+        from xgboost import XGBClassifier
+        model = XGBClassifier(**params)
+    elif model in ("lgbm", "lightgbm"):
+        from lightgbm import LGBMClassifier
+        model = LGBMClassifier(**params)
+    else:
+        raise ValueError(f"The model {model} is not available.")
+    
+    return model
+
+def _ebfs(
+    model:str
+    , params:dict[str, Any]
+    , target:str
+    , comb: Tuple
+    , train: pl.DataFrame
+    , test:pl.DataFrame
+)-> Tuple[Tuple[Tuple, float, float, float], np.ndarray]:
+    estimator = _binary_model_init(model, params)
+    _ = estimator.fit(train.select(comb), train[target])
+    y_pred = estimator.predict_proba(test.select(comb))[:,1]
+    y_test = test[target].to_numpy()
+    rec = (
+        comb,
+        logloss(y_test, y_pred, check_binary=False),
+        roc_auc(y_test, y_pred, check_binary=False)
+    )
+    if model in ("lr", "logistic"):
+        importances = np.abs(estimator.coef_).ravel()
+    else:
+        importances = estimator.feature_importances_
+
+    return rec, importances
+
+# ebfs: stands for Exhaustive Binary Feature Selection
+def ebfs(
+    df:pl.DataFrame
+    , target:str
+    , model:BinaryModels
+    , params:dict[str, Any]
+    , n_comb: int = 3
+    , train_frac:float = 0.75
+) -> Tuple[pl.DataFrame, pl.DataFrame]:
+    '''Suppose we have n features and n_comb = 2. This method will select all (n choose 2) 
+    combinations of features, split dataset into a train and a test, train a model on train, 
+    and compute feature importance and roc_auc and logloss, and then finally put 
+    everything into two separate dataframes, the first of which will contain the feature
+    combinations and model performances, and the second will contain the min, avg, max and var of 
+    feature importance of each feature in all its occurences in the training rounds.
+
+    This method will be extremely slow if (n choose n_comb) is a big number. All numerical columns 
+    will be taken as potential features. Please encode the string columns if you want to use them
+    as features here.
+
+    Future Improvement? Record progress and skip through results.
+
+    If n_jobs is not provided in params, it will be defaulted to -1.
+
+        Arguments:
+            df: an eager Polars DataFrame
+            target: target column
+            model: one of 'logistic', 'lr', 'lightgbm', 'lgbm', 'xgboost', 'xgb', 'random_forest', 'rf'
+            params: parameters for the model.
+            n_comb: n choose n_comb
+
+        Returns:
+            a feature combination summary, a feature importance summary
+    '''
+    
+    features = get_numeric_cols(df, exclude=[target])
+    train, test = train_test_split(df.select(features + [target]), train_frac)
+    fi = {f:[] for f in features}
+    records = []
+    pbar = tqdm(total=math.comb(len(features), n_comb), desc="Total Combinations")
+    with ThreadPoolExecutor(max_workers=CPU_COUNT) as ex:
+        futures = (
+            ex.submit(
+                _ebfs
+                , model
+                , params
+                , target
+                , comb
+                , train
+                , test
+            )
+            for comb in combinations(features, r=n_comb)
+        )
+        for f in as_completed(futures):
+            fc_rec, fi_rec = f.result()
+            records.append(fc_rec)
+            for f, i in zip(fc_rec[0], fi_rec):
+                fi[f].append(i)
+            pbar.update(1)
+
+    fc_summary = pl.from_records(records, schema=["combination", "logloss", "roc_auc"])
+    stats = [
+        (f, len(fi[f]), np.min(fi[f]), np.mean(fi[f]), np.max(fi[f]), np.std(fi[f])) for f in fi
+    ]
+    fi_summary = pl.from_records(stats, schema=["feature", "occurrences", "min", "mean", "max", "std"])
+    pbar.close()
+    return fc_summary, fi_summary
+
+def ebfs_fc_filter(
+    fc: pl.DataFrame
+    , logloss_threshold:float
+    , roc_auc_threshold:float
+) -> list[str]:
+    '''A filter method based on the feature combination result of ebfs. First, 
+
+        Arguments:
+            fc: the feature combination result from ebfs
+            logloss_threshold: the maximum logloss for the combination to be kept
+            roc_auc_threshold: the minumum roc_auc for the combination to be kept
+
+        Returns:
+            a list of string representing all features in the combinations after filtering
+    '''
+    return fc.filter(
+        pl.col("logloss") <= logloss_threshold
+        & pl.col("roc_auc") >= roc_auc_threshold
+    ).get_column("combination").explode().unique().to_list()
+
+
```

### Comparing `dsds-0.0.16/src/dsds/metrics.py` & `dsds-0.0.17/src/dsds/metrics.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,217 +1,217 @@
-import numpy as np 
-import polars as pl
-from typing import Tuple, Optional
-import logging
-
-logger = logging.getLogger(__name__)
-
-# No need to do length checking (len(y_1) == len(y_2)) because NumPy / Polars will complain for us.
-# Everything here is essentially fun stuff.
-# Ideally speaking, you should never convert things to dataframes when you compute these metrics.
-# But using only NumPy means we loss parallelism, and using Python concurrent module will not help
-# in this case (haha Python). 
-# So funnily enough, we can convert things to dataframes and get a performance boost.
-# Ideally, all of these should be re-written in Rust using some kind of parallel stuff in Rust.
-
-def _flatten_input(y_actual: np.ndarray, y_predicted:np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
-    y_a = y_actual.ravel()
-    if y_predicted.ndim == 2:
-        y_p = y_predicted[:, 1] # .ravel()
-    else:
-        y_p = y_predicted.ravel()
-
-    return y_a, y_p
-
-def get_tp_fp(
-    y_actual:np.ndarray
-    , y_predicted:np.ndarray
-    , ratio:bool = True
-) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
-    '''
-        Get true positive and false positive counts at various thresholds.
-
-        Arguments:
-            y_actual: actual binary labels
-            y_predicted: predicted labels
-            ratio: if true, return true positive rate and false positive rate at the threholds; 
-            if false return the count.
-
-        Returns:
-            True positive count/rate, False positive count/rate, the thresholds
-    '''
-   
-    df = pl.from_records((y_predicted, y_actual), schema=["predicted", "actual"])
-    all_positives = pl.lit(np.sum(y_actual))
-    n = len(df)
-    temp = df.lazy().groupby("predicted").agg(
-        pl.count().alias("cnt")
-        , pl.col("actual").sum().alias("true_positive")
-    ).sort("predicted").with_columns(
-        predicted_positive = n - pl.col("cnt").cumsum() + pl.col("cnt")
-        , tp = (all_positives - pl.col("true_positive").cumsum()).shift_and_fill(fill_value=all_positives, periods=1)
-    ).select(
-        pl.col("predicted")
-        , pl.col("tp")
-        , fp = pl.col("predicted_positive") - pl.col("tp")
-    ).collect()
-
-    # We are relatively sure that y_actual and y_predicted won't have null values.
-    # So we can do temp["tp"].view() to get some more performance. 
-    # But that might confuse users.
-    tp = temp["tp"].to_numpy()
-    fp = temp["fp"].to_numpy()
-    if ratio:
-        return tp/tp[0], fp/fp[0], temp["predicted"].to_numpy()
-    return tp, fp, temp["predicted"].to_numpy()
-
-def roc_auc(y_actual:np.ndarray, y_predicted:np.ndarray, check_binary:bool=True) -> float:
-    '''Return the Area Under the Curve metric for the model's predictions.
-
-        Arguments:
-            y_actual: actual target
-            y_predicted: predicted probability
-
-        Returns:
-            the auc value
-    ''' 
-    
-    # This currently has difference of magnitude 1e-10 from the sklearn implementation, 
-    # which is likely caused by sklearn adding zeros to the front? Not 100% sure
-    # This is about 50% faster than sklearn's implementation. I know, not that this matters
-    # that much...
-    
-    y_a, y_p = _flatten_input(y_actual, y_predicted)
-    # No need to check if length matches because Polars will complain for us
-    if check_binary:
-        uniques = np.unique(y_a)
-        if uniques.size != 2:
-            raise ValueError("Currently this only supports binary classification.")
-        if not (0 in uniques and 1 in uniques):
-            raise ValueError("Currently this only supports binary classification with 0 and 1 target.")
-
-    tpr, fpr, _ = get_tp_fp(y_a.astype(np.int8), y_p, ratio=True)
-    return float(-np.trapz(tpr, fpr))
-
-def logloss(
-    y_actual:np.ndarray
-    , y_predicted:np.ndarray
-    , sample_weights:Optional[np.ndarray]=None
-    , min_prob:float = 1e-12
-    , check_binary:bool = True
-) -> float:
-    '''Return the logloss of the prediction.
-
-        Arguments:
-            y_actual: actual target
-            y_predicted: predicted probability
-            sample_weights: an array of size (n_sample, ) which provides weights to each sample
-            min_prob: minimum probability to clip so that we can prevent illegal computations like 
-            log(0). If p < min_prob, log(min_prob) will be computed instead.
-
-        Returns:
-            the average logloss
-
-    '''
-    # Takes about 1/3 time of sklearn's log_loss because we parallelized some computations
-
-    y_a, y_p = _flatten_input(y_actual, y_predicted)
-    if check_binary:
-        uniques = np.unique(y_a)
-        if uniques.size != 2:
-            raise ValueError("Currently this only supports binary classification.")
-        if not (0 in uniques and 1 in uniques):
-            raise ValueError("Currently this only supports binary classification with 0 and 1 target.")
-
-    if sample_weights is None:
-        return pl.from_records((y_a, y_p), schema=["y", "p"]).with_columns(
-            l = pl.col("p").clip_min(min_prob).log(),
-            o = (1- pl.col("p")).clip_min(min_prob).log(),
-            ny = 1 - pl.col("y")
-        ).select(
-            pl.lit(-1, dtype=pl.Float64) * (pl.col("y") * pl.col("l") + pl.col("ny") * pl.col("o")).mean()
-        ).row(0)[0]
-    else:
-        s = sample_weights.ravel()
-        return pl.from_records((y_a, y_p, s), schema=["y", "p", "s"]).with_columns(
-            l = pl.col("p").clip_min(min_prob).log(),
-            o = (1- pl.col("p")).clip_min(min_prob).log(),
-            ny = 1 - pl.col("y")
-        ).select(
-            pl.lit(-1, dtype=pl.Float64)
-            * pl.col("s") 
-            * (pl.col("y") * pl.col("l") + pl.col("ny") * pl.col("o")).mean()
-        ).row(0)[0]
-
-
-def l2_loss(
-    y_actual:np.ndarray
-    , y_predicted:np.ndarray
-    , sample_weights:Optional[np.ndarray]=None
-) -> float:
-    diff = y_actual - y_predicted
-    if sample_weights is None:
-        return np.mean(diff.dot(diff))
-    else:
-        return (sample_weights/(len(diff))).dot(diff.dot(diff))
-    
-mse = l2_loss
-
-def l1_loss(
-    y_actual:np.ndarray
-    , y_predicted:np.ndarray
-    , sample_weights:Optional[np.ndarray]=None
-) -> float:
-    diff = np.abs(y_actual - y_predicted)
-    if sample_weights is None:
-        return np.mean(diff)
-    else:
-        return (sample_weights/(len(diff))).dot(diff)
-
-mae = l1_loss 
-
-def r2(y_actual:np.ndarray, y_predicted:np.ndarray) -> float:
-    '''Returns the r2 of the prediction.'''
-
-    # This is trivial, and we won't really have any performance gain by using Polars' or other stuff.
-    # This is here just for completeness
-    d1 = y_actual - y_predicted
-    d2 = y_actual - np.mean(y_actual)
-    # ss_res = d1.dot(d1), ss_tot = d2.dot(d2) 
-    return 1 - d1.dot(d1)/d2.dot(d2)
-
-def adjusted_r2(
-    y_actual:np.ndarray
-    , y_predicted:np.ndarray
-    , p:int
-) -> float:
-    '''Computes the adjusted r2 of the prediction.
-
-        p: number of predictive variables
-    '''
-    df_tot = len(y_actual) - 1
-    return 1 - (1 - r2(y_actual, y_predicted)) * df_tot / (df_tot - p)
-
-def huber_loss(
-    y_actual:np.ndarray
-    , y_predicted:np.ndarray
-    , delta:float
-    , sample_weights:Optional[np.ndarray]=None  
-) -> float:
-    
-    y_a = y_actual.ravel()
-    y_p = y_predicted.ravel()
-    
-    if delta <= 0:
-        raise ValueError("Delta in Huber loss must be positive.")
-
-    abs_diff = np.abs(y_a - y_p)
-    mask = abs_diff <= delta
-    not_mask = ~mask
-    loss = np.zeros(shape=abs_diff.shape)
-    loss[mask] = 0.5 * (abs_diff[mask]**2)
-    loss[not_mask] = delta * (abs_diff[not_mask] - 0.5 * delta)
-
-    if sample_weights is None:
-        return np.mean(loss)
-    else:
-        return (sample_weights/(len(loss))).dot(loss)
+import numpy as np 
+import polars as pl
+from typing import Tuple, Optional
+import logging
+
+logger = logging.getLogger(__name__)
+
+# No need to do length checking (len(y_1) == len(y_2)) because NumPy / Polars will complain for us.
+# Everything here is essentially fun stuff.
+# Ideally speaking, you should never convert things to dataframes when you compute these metrics.
+# But using only NumPy means we loss parallelism, and using Python concurrent module will not help
+# in this case (haha Python). 
+# So funnily enough, we can convert things to dataframes and get a performance boost.
+# Ideally, all of these should be re-written in Rust using some kind of parallel stuff in Rust.
+
+def _flatten_input(y_actual: np.ndarray, y_predicted:np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
+    y_a = y_actual.ravel()
+    if y_predicted.ndim == 2:
+        y_p = y_predicted[:, 1] # .ravel()
+    else:
+        y_p = y_predicted.ravel()
+
+    return y_a, y_p
+
+def get_tp_fp(
+    y_actual:np.ndarray
+    , y_predicted:np.ndarray
+    , ratio:bool = True
+) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
+    '''
+        Get true positive and false positive counts at various thresholds.
+
+        Arguments:
+            y_actual: actual binary labels
+            y_predicted: predicted labels
+            ratio: if true, return true positive rate and false positive rate at the threholds; 
+            if false return the count.
+
+        Returns:
+            True positive count/rate, False positive count/rate, the thresholds
+    '''
+   
+    df = pl.from_records((y_predicted, y_actual), schema=["predicted", "actual"])
+    all_positives = pl.lit(np.sum(y_actual))
+    n = len(df)
+    temp = df.lazy().groupby("predicted").agg(
+        pl.count().alias("cnt")
+        , pl.col("actual").sum().alias("true_positive")
+    ).sort("predicted").with_columns(
+        predicted_positive = n - pl.col("cnt").cumsum() + pl.col("cnt")
+        , tp = (all_positives - pl.col("true_positive").cumsum()).shift_and_fill(fill_value=all_positives, periods=1)
+    ).select(
+        pl.col("predicted")
+        , pl.col("tp")
+        , fp = pl.col("predicted_positive") - pl.col("tp")
+    ).collect()
+
+    # We are relatively sure that y_actual and y_predicted won't have null values.
+    # So we can do temp["tp"].view() to get some more performance. 
+    # But that might confuse users.
+    tp = temp["tp"].to_numpy()
+    fp = temp["fp"].to_numpy()
+    if ratio:
+        return tp/tp[0], fp/fp[0], temp["predicted"].to_numpy()
+    return tp, fp, temp["predicted"].to_numpy()
+
+def roc_auc(y_actual:np.ndarray, y_predicted:np.ndarray, check_binary:bool=True) -> float:
+    '''Return the Area Under the Curve metric for the model's predictions.
+
+        Arguments:
+            y_actual: actual target
+            y_predicted: predicted probability
+
+        Returns:
+            the auc value
+    ''' 
+    
+    # This currently has difference of magnitude 1e-10 from the sklearn implementation, 
+    # which is likely caused by sklearn adding zeros to the front? Not 100% sure
+    # This is about 50% faster than sklearn's implementation. I know, not that this matters
+    # that much...
+    
+    y_a, y_p = _flatten_input(y_actual, y_predicted)
+    # No need to check if length matches because Polars will complain for us
+    if check_binary:
+        uniques = np.unique(y_a)
+        if uniques.size != 2:
+            raise ValueError("Currently this only supports binary classification.")
+        if not (0 in uniques and 1 in uniques):
+            raise ValueError("Currently this only supports binary classification with 0 and 1 target.")
+
+    tpr, fpr, _ = get_tp_fp(y_a.astype(np.int8), y_p, ratio=True)
+    return float(-np.trapz(tpr, fpr))
+
+def logloss(
+    y_actual:np.ndarray
+    , y_predicted:np.ndarray
+    , sample_weights:Optional[np.ndarray]=None
+    , min_prob:float = 1e-12
+    , check_binary:bool = True
+) -> float:
+    '''Return the logloss of the prediction.
+
+        Arguments:
+            y_actual: actual target
+            y_predicted: predicted probability
+            sample_weights: an array of size (n_sample, ) which provides weights to each sample
+            min_prob: minimum probability to clip so that we can prevent illegal computations like 
+            log(0). If p < min_prob, log(min_prob) will be computed instead.
+
+        Returns:
+            the average logloss
+
+    '''
+    # Takes about 1/3 time of sklearn's log_loss because we parallelized some computations
+
+    y_a, y_p = _flatten_input(y_actual, y_predicted)
+    if check_binary:
+        uniques = np.unique(y_a)
+        if uniques.size != 2:
+            raise ValueError("Currently this only supports binary classification.")
+        if not (0 in uniques and 1 in uniques):
+            raise ValueError("Currently this only supports binary classification with 0 and 1 target.")
+
+    if sample_weights is None:
+        return pl.from_records((y_a, y_p), schema=["y", "p"]).with_columns(
+            l = pl.col("p").clip_min(min_prob).log(),
+            o = (1- pl.col("p")).clip_min(min_prob).log(),
+            ny = 1 - pl.col("y")
+        ).select(
+            pl.lit(-1, dtype=pl.Float64) * (pl.col("y") * pl.col("l") + pl.col("ny") * pl.col("o")).mean()
+        ).row(0)[0]
+    else:
+        s = sample_weights.ravel()
+        return pl.from_records((y_a, y_p, s), schema=["y", "p", "s"]).with_columns(
+            l = pl.col("p").clip_min(min_prob).log(),
+            o = (1- pl.col("p")).clip_min(min_prob).log(),
+            ny = 1 - pl.col("y")
+        ).select(
+            pl.lit(-1, dtype=pl.Float64)
+            * pl.col("s") 
+            * (pl.col("y") * pl.col("l") + pl.col("ny") * pl.col("o")).mean()
+        ).row(0)[0]
+
+
+def l2_loss(
+    y_actual:np.ndarray
+    , y_predicted:np.ndarray
+    , sample_weights:Optional[np.ndarray]=None
+) -> float:
+    diff = y_actual - y_predicted
+    if sample_weights is None:
+        return np.mean(diff.dot(diff))
+    else:
+        return (sample_weights/(len(diff))).dot(diff.dot(diff))
+    
+mse = l2_loss
+
+def l1_loss(
+    y_actual:np.ndarray
+    , y_predicted:np.ndarray
+    , sample_weights:Optional[np.ndarray]=None
+) -> float:
+    diff = np.abs(y_actual - y_predicted)
+    if sample_weights is None:
+        return np.mean(diff)
+    else:
+        return (sample_weights/(len(diff))).dot(diff)
+
+mae = l1_loss 
+
+def r2(y_actual:np.ndarray, y_predicted:np.ndarray) -> float:
+    '''Returns the r2 of the prediction.'''
+
+    # This is trivial, and we won't really have any performance gain by using Polars' or other stuff.
+    # This is here just for completeness
+    d1 = y_actual - y_predicted
+    d2 = y_actual - np.mean(y_actual)
+    # ss_res = d1.dot(d1), ss_tot = d2.dot(d2) 
+    return 1 - d1.dot(d1)/d2.dot(d2)
+
+def adjusted_r2(
+    y_actual:np.ndarray
+    , y_predicted:np.ndarray
+    , p:int
+) -> float:
+    '''Computes the adjusted r2 of the prediction.
+
+        p: number of predictive variables
+    '''
+    df_tot = len(y_actual) - 1
+    return 1 - (1 - r2(y_actual, y_predicted)) * df_tot / (df_tot - p)
+
+def huber_loss(
+    y_actual:np.ndarray
+    , y_predicted:np.ndarray
+    , delta:float
+    , sample_weights:Optional[np.ndarray]=None  
+) -> float:
+    
+    y_a = y_actual.ravel()
+    y_p = y_predicted.ravel()
+    
+    if delta <= 0:
+        raise ValueError("Delta in Huber loss must be positive.")
+
+    abs_diff = np.abs(y_a - y_p)
+    mask = abs_diff <= delta
+    not_mask = ~mask
+    loss = np.zeros(shape=abs_diff.shape)
+    loss[mask] = 0.5 * (abs_diff[mask]**2)
+    loss[not_mask] = delta * (abs_diff[not_mask] - 0.5 * delta)
+
+    if sample_weights is None:
+        return np.mean(loss)
+    else:
+        return (sample_weights/(len(loss))).dot(loss)
```

### Comparing `dsds-0.0.16/src/dsds/prescreen.py` & `dsds-0.0.17/src/dsds/prescreen.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,651 +1,651 @@
-from .type_alias import (
-    PolarsFrame
-    , KSAlternatives
-    , CommonContinuousDist
-    , CPU_COUNT
-    , POLARS_DATETIME_TYPES
-    , POLARS_NUMERICAL_TYPES
-)
-from .sample import (
-    lazy_sample
-)
-from .blueprint import(
-    Blueprint
-)
-
-import polars.selectors as cs
-import polars as pl
-import logging  
-from datetime import datetime 
-from typing import Any, Optional, Tuple
-from itertools import combinations
-from scipy.stats import (
-    ks_2samp
-    , kstest
-)
-from concurrent.futures import as_completed, ThreadPoolExecutor
-from tqdm import tqdm
-from math import comb
-
-logger = logging.getLogger(__name__)
-
-#----------------------------------------------------------------------------------------------#
-# Generic columns checks | Only works with Polars because Pandas's data types suck!            #
-#----------------------------------------------------------------------------------------------#
-
-def get_numeric_cols(df:PolarsFrame, exclude:Optional[list[str]]=None) -> list[str]:
-    if exclude is None:
-        selector = cs.numeric()
-    else:
-        selector = cs.numeric() & ~cs.by_name(exclude)
-    return df.select(selector).columns
-
-def get_string_cols(df:PolarsFrame, exclude:Optional[list[str]]=None) -> list[str]:
-    if exclude is None:
-        selector = cs.string()
-    else:
-        selector = cs.string() & ~cs.by_name(exclude)
-    return df.select(selector).columns
-
-def get_datetime_cols(df:PolarsFrame) -> list[str]:
-    '''Only gets datetime columns, will not infer from strings.'''
-    return df.select(cs.datetime()).columns
-
-def get_bool_cols(df:PolarsFrame) -> list[str]:
-    return df.select(cs.by_dtype(pl.Boolean)).columns
-
-def get_cols_regex(df:PolarsFrame, pattern:str) -> list[str]:
-    return df.select(cs.matches(pattern=pattern)).columns
-
-def lowercase_columns(df:PolarsFrame) -> PolarsFrame:
-    return df.rename({c: c.lower() for c in df.columns})
-
-def check_binary_target(df:PolarsFrame, target:str) -> bool:
-    target_uniques = df.lazy().select(pl.col(target).unique()).collect().get_column(target)
-    if len(target_uniques) != 2:
-        logger.error("Target is not binary.")
-        return False
-    elif not (0 in target_uniques and 1 in target_uniques):
-        logger.error("The binary target is not encoded as 0s and 1s.")
-        return False
-    return True
-    
-def check_target_cardinality(df:PolarsFrame, target:str) -> pl.DataFrame:
-    return df.lazy().groupby(target).count().sort(target).collect()
-
-def check_columns_types(df:PolarsFrame, cols:Optional[list[str]]=None) -> str:
-    '''Returns the unique types of given columns in a single string. If multiple types are present
-    they are joined by a |. If cols is not given, automatically uses all df's columns.'''
-    if cols is None:
-        check_cols:list[str] = df.columns
-    else:
-        check_cols:list[str] = cols 
-
-    types = set(dtype_mapping(t) for t in df.select(check_cols).dtypes)
-    return "|".join(types) if len(types) > 0 else "unknown"
-    
-# dtype can be a "pl.datatype" or just some random data for which we want to infer a generic type.
-def dtype_mapping(d: Any) -> str:
-    if isinstance(d, str) or d == pl.Utf8:
-        return "string"
-    elif isinstance(d, bool) or d == pl.Boolean:
-        return "bool"
-    elif isinstance(d, (int,float)) or d in POLARS_NUMERICAL_TYPES:
-        return "numeric"
-    elif isinstance(d, datetime) or d in POLARS_DATETIME_TYPES:
-        return "datetime"
-    else:
-        return "other/unknown"
-
-#----------------------------------------------------------------------------------------------#
-# Prescreen Inferral, Removal Methods                                                          #
-#----------------------------------------------------------------------------------------------#
-
-# Add a slim option that returns fewer stats? This is generic describe.
-# Separate str and numeric?
-def describe(
-    df:PolarsFrame
-    , sample_frac:float = 0.75
-) -> pl.DataFrame:
-    '''Profile the data.
-
-        Arguments:
-            df: Either an eager dataframe or a lazy dataframe
-            sample_frac: If input is a LazyFrame, a sample of sample_frac will be used. If input is eager,
-            no sampling will be done.
-
-        Returns:
-            a dataframe containing the necessary information.
-    '''
-
-    if isinstance(df, pl.LazyFrame):
-        df_local = lazy_sample(df, sample_frac=sample_frac)
-    else:
-        df_local = df
-    
-    temp = df_local.describe()
-    desc = temp.drop_in_place("describe")
-    # Get unique
-    unique_counts = get_unique_count(df_local).with_columns(
-        unique_pct = pl.col("n_unique") / len(df_local)
-    )
-    # Skew and Kurtosis
-    skew_and_kt_data = df_local.lazy().select(
-        pl.all().skew().prefix("skew:")
-        , pl.all().skew().prefix("kurtosis:")
-    ).collect().row(0)
-
-    n_cols = len(df_local.columns)
-    skew_and_kt = pl.from_records((df_local.columns, skew_and_kt_data[:n_cols], skew_and_kt_data[n_cols:])
-                                  , schema=["column", "skew", "kurtosis"])
-
-    # Get a basic string description of the data type.
-    dtypes_dict = dict(zip(df_local.columns, map(dtype_mapping, df_local.dtypes)))
-    # Combine all
-    nums = ("count", "null_count", "mean", "std", "median", "25%", "75%")
-    final = temp.transpose(include_header=True, column_names=desc).with_columns(
-        pl.col(c).cast(pl.Float64) for c in nums
-    ).with_columns(
-        null_pct = pl.col("null_count")/pl.col("count")
-        , dtype = pl.col("column").map_dict(dtypes_dict)
-    ).join(unique_counts, on="column").join(skew_and_kt, on="column")
-    
-    return final.select('column','count','null_count','null_pct','n_unique'
-                        , 'unique_pct','mean','std','min','max','25%'
-                        , 'median','75%', "skew", "kurtosis",'dtype')
-
-# Numeric only describe. Be more detailed.
-
-# String only describe. Be more detailed about interesting string stats.
-
-def describe_str(df:PolarsFrame
-    , words_to_count:Optional[list[str]]=None
-    , sample_frac:float = 0.75
-) -> pl.DataFrame:
-    '''Gives some statistics about the string columns. Optionally you may pass a list
-    of strings to compute the total occurrances of each of the words in the string columns. If input is a LazyFrame, 
-    a sample of sample_pct will be used, and sample_pct will only be used in the lazy case. 
-
-    '''
-    strs = get_string_cols(df)
-    df_str = df.select(strs)
-    if isinstance(df, pl.LazyFrame):
-        df_str = lazy_sample(df_str, sample_frac=sample_frac).collect()
-
-    nstrs = len(strs)
-    stats = df.select(strs).select(
-        pl.all().null_count().prefix("nc:"),
-        pl.all().max().prefix("max:"),
-        pl.all().min().prefix("min:"),
-        pl.all().mode().first().prefix("mode:"),
-        pl.all().str.lengths().min().prefix("min_byte_len:"),
-        pl.all().str.lengths().max().prefix("max_byte_len:"),
-        pl.all().str.lengths().mean().prefix("avg_byte_len:"),
-        pl.all().str.lengths().median().prefix("median_byte_len:"),
-        pl.all().str.count_match(r"\s").mean().prefix("avg_space_cnt:"),
-        pl.all().str.count_match(r"[0-9]").mean().prefix("avg_digit_cnt:"),
-        pl.all().str.count_match(r"[A-Z]").mean().prefix("avg_cap_cnt:"),
-        pl.all().str.count_match(r"[a-z]").mean().prefix("avg_lower_cnt:")
-    ).row(0)
-    output = {
-        "features":strs,
-        "null_count": stats[:nstrs],
-        "min": stats[nstrs: 2*nstrs],
-        "max": stats[2*nstrs: 3*nstrs],
-        "mode": stats[3*nstrs: 4*nstrs],
-        "min_byte_len": stats[4*nstrs: 5*nstrs],
-        "max_byte_len": stats[5*nstrs: 6*nstrs],
-        "avg_byte_len": stats[6*nstrs: 7*nstrs],
-        "median_byte_len": stats[7*nstrs: 8*nstrs],
-        "avg_space_cnt": stats[8*nstrs: 9*nstrs],
-        "avg_digit_cnt": stats[9*nstrs: 10*nstrs],
-        "avg_cap_cnt": stats[10*nstrs: 11*nstrs],
-        "avg_lower_cnt": stats[11*nstrs: ],
-    }
-
-    if isinstance(words_to_count, list):
-        for w in words_to_count:
-            t = df_str.select(pl.all().str.count_match(w).sum().prefix("wc:")).row(0)
-            output["total_"+ w + "_count"] = t
-
-    return pl.from_dict(output)
-
-# -----------------------------------------------------------------------------------------------
-def drop(df:PolarsFrame, to_drop:list[str]) -> PolarsFrame:
-    if isinstance(df, pl.LazyFrame):
-        return df.blueprint.drop(to_drop)
-    return df.drop(to_drop)
-
-def non_numeric_removal(df:PolarsFrame, include_bools:bool=True) -> PolarsFrame:
-    '''Removes all non-numeric columns. If include_bools = True, then keep boolean columns.'''
-    
-    if include_bools:
-        selector = ~(cs.numeric()|cs.by_dtype(pl.Boolean))
-    else:
-        selector = ~cs.numeric()
-
-    non_nums = df.select(selector).columns
-    logger.info(f"The following columns are dropped because they are not numeric: {non_nums}.\n"
-                f"Removed a total of {len(non_nums)} columns.")
-    
-    return drop(df, non_nums)
-
-# Check if columns are duplicates. Might take time.
-def duplicate_inferral():
-    # Get profiles first.
-    # Divide into categories: bools, strings, numerics, datetimes.
-    # Then cut down list to columns that have the same min, max, n_unique and null_count.
-    # Then check equality..
-    pass
-
-def pattern_inferral(
-    df: PolarsFrame
-    , pattern:str
-    , sample_frac:float = 0.75
-    , sample_count:int = 100_000
-    , sample_rounds:int = 3
-    , threshold:float = 0.9
-    , count_null:bool = True
-) -> list[str]:
-    '''Find all string columns whose elements reasonably match the given pattern. The match logic can 
-    be tuned using the all the parameters.
-
-    Arguments:
-        sample_frac: the pct of the total dataframe to use as basis
-        sample_count: from the basis, how many rows to sample for each round 
-        sample_rounds: how many rounds of sampling we are doing
-        threhold: For each round, what is the match% that is needed to be a counted as a success. For instance, 
-        in round 1, for column x, we have 92% match rate, and threshold = 0.9. We count column x as a match for 
-        this round. In the end, the column must match for every round to be considered a real match.
-        count_null: for individual matches, do we want to count null as a match or not? If the column has high null pct,
-        the non-null values might mostly match the pattern. In this case, using count_null = True will match the column, 
-        while count_null = False will most likely exclude the column.
-
-    Returns:
-        a list of columns that pass the matching test
-    
-    '''
-    
-    strs = get_string_cols(df)
-    df_local = lazy_sample(df.lazy(), sample_frac=sample_frac).collect()    
-    matches:set[str] = set(strs)
-    sample_size = min(sample_count, len(df_local))
-    for _ in range(sample_rounds):
-        df_sample = df_local.sample(n = sample_size)
-        fail = df_sample.select(
-            (pl.when(pl.col(s).is_null()).then(count_null).otherwise(
-                pl.col(s).str.contains(pattern)
-            ).sum()/sample_size).alias(s) for s in strs
-        ).transpose(include_header=True, column_names=["pattern_match_pct"])\
-        .filter(pl.col("pattern_match_pct") < threshold).get_column("column")
-        # If the match failes in this round, remove the column.
-        matches.difference_update(fail)
-
-    return list(matches)
-
-def pattern_removal(
-    df: PolarsFrame
-    , pattern:str
-    , sample_pct:float = 0.75
-    , sample_count:int = 100_000
-    , sample_rounds:int = 3
-    , threshold:float = 0.9
-    , count_null:bool = True
-) -> PolarsFrame:
-    
-    remove_cols = pattern_inferral(
-        df
-        , pattern
-        , sample_pct
-        , sample_count
-        , sample_rounds
-        , threshold 
-        , count_null
-    )
-    logger.info(f"The following columns are dropped because they match the element pattern: {pattern}.\n"
-                f"{remove_cols}\n"
-                f"Removed a total of {len(remove_cols)} columns.")
-    
-    return drop(df, remove_cols)
-
-def email_inferral(
-    df: PolarsFrame
-    , sample_pct:float = 0.75
-    , sample_count:int = 100_000
-    , sample_rounds:int = 3
-    , threshold:float = 0.9
-    , count_null:bool = True
-) -> list[str]:
-    # Why does this regex not work?
-    # r'([A-Za-z0-9]+[.-_])*[A-Za-z0-9]+@[A-Za-z0-9-]+(\.[A-Z|a-z]{2,})+'
-    return pattern_inferral(
-        df
-        , r'\S+@\S+\.\S+'
-        , sample_pct
-        , sample_count
-        , sample_rounds
-        , threshold 
-        , count_null
-    )
-
-def email_removal(
-    df: PolarsFrame
-    , sample_pct:float = 0.75
-    , sample_count:int = 100_000
-    , sample_rounds:int = 3
-    , threshold:float = 0.9
-    , count_null:bool = True
-) -> PolarsFrame:
-    
-    emails = email_inferral(df, sample_pct, sample_count, sample_rounds, threshold, count_null)
-    logger.info(f"The following columns are dropped because they are emails. {emails}.\n"
-            f"Removed a total of {len(emails)} columns.")
-    
-    return drop(df, emails)
-
-# Check for columns that are US zip codes.
-# Might add options for other countries later.
-def zipcode_inferral():
-    # Match string using pattern inferral
-    # Take a look at integers too, are they always 5 digits? 
-    pass
-
-def date_inferral(df:PolarsFrame) -> list[str]:
-    '''Infers date columns in dataframe. This inferral is not perfect.'''
-    logger.info("Date Inferral is error prone due to the huge variety of date formats. Please use with caution.")
-    
-    dates = [c for c,t in zip(df.columns, df.dtypes) if t in POLARS_DATETIME_TYPES]
-    strings = get_string_cols(df)
-    # MIGHT REWRITE THIS LOGIC
-    # Might be memory intensive on big dataframes.
-    sample_size = min(len(df), 100_000)
-    sample_df = df.lazy().select(strings)\
-        .drop_nulls().collect()\
-        .sample(n = sample_size).select(
-            # Cleaning the string first. Only try to catch string dates which are in the first split by space
-           pl.col(s).str.strip().str.replace_all("(/|\.)", "-").str.split(by=" ").list.first() 
-           for s in strings
-        )
-    for s in strings:
-        try:
-            c = sample_df[s].str.to_date(strict=False)
-            if 1 - c.null_count()/sample_size >= 0.15: # if at least 15% valid (able to be converted)
-                # This last check is to account for single digit months.
-                # 3/3/1995 will not be parsed to a string because standard formats require 03/03/1995
-                # At least 15% of dates naturally have both month and day as 2 digits numbers
-                dates.append(s)
-        except: # noqa: E722
-            # Very stupid code, but I have to do it...
-            pass
-    
-    return dates
-
-def date_removal(df:PolarsFrame) -> PolarsFrame:
-    '''Removes all date columns from dataframe. This algorithm will try to infer if string column is date.'''
-
-    remove_cols = date_inferral(df) 
-    logger.info(f"The following columns are dropped because they are dates. {remove_cols}.\n"
-                f"Removed a total of {len(remove_cols)} columns.")
-    return drop(df, remove_cols)
-
-def null_inferral(df:PolarsFrame, threshold:float=0.5) -> list[str]:
-    '''Infers columns that have more than threshold pct of null values. Threshold should be between 0 and 1.'''
-    return (df.lazy().null_count().collect()/len(df)).transpose(include_header=True, column_names=["null_pct"])\
-                    .filter(pl.col("null_pct") >= threshold)\
-                    .get_column("column").to_list()
-
-def null_removal(df:PolarsFrame, threshold:float=0.5) -> PolarsFrame:
-    '''Removes columns with more than threshold pct of null values. Threshold should be between 0 and 1.'''
-
-    remove_cols = null_inferral(df, threshold) 
-    logger.info(f"The following columns are dropped because they have more than {threshold*100:.2f}%"
-                f" null values. {remove_cols}.\n"
-                f"Removed a total of {len(remove_cols)} columns.")
-    return drop(df, remove_cols)
-
-def var_inferral(df:PolarsFrame, threshold:float, target:str) -> list[str]:
-    '''Infers columns that have lower than threshold variance. Target will not be included.'''
-    return df.lazy().select(
-                pl.col(x).var() for x in get_numeric_cols(df) if x != target
-            ).collect().transpose(include_header=True, column_names=["var"])\
-            .filter(pl.col("var") < threshold).get_column("column").to_list() 
-
-def var_removal(df:PolarsFrame, threshold:float, target:str) -> PolarsFrame:
-    '''Removes features with low variance. Features with > threshold variance will be kept. 
-        Threshold should be positive.'''
-
-    remove_cols = var_inferral(df, threshold, target) 
-    logger.info(f"The following columns are dropped because they have lower than {threshold} variance. {remove_cols}.\n"
-                f"Removed a total of {len(remove_cols)} columns.")
-    return drop(df, remove_cols)
-
-# Really this is just an alias
-regex_inferral = get_cols_regex
-
-def regex_removal(df:PolarsFrame, pattern:str, lowercase:bool=False) -> PolarsFrame:
-    '''Remove columns if they satisfy some regex rules.'''
-    remove_cols = get_cols_regex(df, pattern, lowercase)
-    logger.info(f"The following columns are dropped because their names satisfy the regex rule: {pattern}."
-                f" {remove_cols}.\n"
-                f"Removed a total of {len(remove_cols)} columns.")
-    
-    return drop(df, remove_cols)
-
-def get_unique_count(df:PolarsFrame) -> pl.DataFrame:
-    '''Gets unique counts for columns.'''
-    return df.lazy().select(
-        pl.col(x).n_unique() for x in df.columns
-    ).collect().transpose(include_header=True, column_names=["n_unique"])
-
-# Really this is just an alias
-def unique_inferral(df:PolarsFrame, threshold:float=0.9) -> list[str]:
-    '''Infers columns that have higher than threshold pct of unique values.'''
-    return get_unique_count(df).with_columns(
-        (pl.col("n_unique")/len(df)).alias("unique_pct")
-    ).filter(pl.col("unique_pct") >= threshold)\
-    .get_column("column").to_list()
-
-def unique_removal(df:PolarsFrame, threshold:float=0.9) -> PolarsFrame:
-    '''Remove columns that have higher than threshold pct of unique values.'''
-
-    remove_cols = unique_inferral(df, threshold)
-    logger.info(f"The following columns are dropped because more than {threshold*100:.2f}% of unique values."
-                f" {remove_cols}.\n"
-                f"Removed a total of {len(remove_cols)} columns.")
-    return drop(df, remove_cols)
-
-# Is this a good definition?
-def discrete_inferral(df:PolarsFrame
-    , threshold:float=0.1
-    , max_n_unique:int=100
-    , exclude:Optional[list[str]]=None
-) -> list[str]:
-    '''
-        A column that satisfies either n_unique < max_n_unique or unique_pct < threshold 
-        will be considered discrete.
-    '''
-    exclude_list = [] if exclude is None else exclude
-    return get_unique_count(df).filter(
-        ((pl.col("n_unique") < max_n_unique) | (pl.col("n_unique")/len(df) < threshold)) 
-        & (~pl.col("column").is_in(exclude_list)) # is not in
-    ).get_column("column").to_list()
-
-def conti_inferral(
-    df:PolarsFrame
-    , discrete_threshold:float = 0.1
-    , discrete_max_n_unique:int = 100
-    , exclude:Optional[list[str]]=None
-) -> list[str]:
-    exclude_list = [] if exclude is None else exclude
-    discrete = discrete_inferral(df, discrete_threshold, discrete_max_n_unique)
-    return df.select(cs.numeric() & ~cs.by_name(exclude_list) & ~cs.by_name(discrete)).columns
-
-def constant_inferral(df:PolarsFrame, include_null:bool=True) -> list[str]:
-    temp = get_unique_count(df).filter(pl.col("n_unique") <= 2)
-    remove_cols = temp.filter(pl.col("n_unique") == 1).get_column("column").to_list() 
-    if include_null: # This step is kind of inefficient right now.
-        binary = temp.filter(pl.col("n_unique") == 2).get_column("column")
-        nc = df.lazy().select(binary).null_count().collect().row(0)
-        remove_cols.extend(
-            binary[i] for i in range(len(nc)) if nc[i] > 0
-        )
-
-    return remove_cols
-
-def constant_removal(df:PolarsFrame, include_null:bool=True) -> PolarsFrame:
-    '''Removes all constant columns from dataframe.
-    
-        Arguments:
-            df:
-            include_null: if true, then columns with two distinct values like [value_1, null] will be considered a 
-                constant column.
-
-        Returns: 
-            the df without constant columns
-    '''
-    remove_cols = constant_inferral(df, include_null)
-    logger.info(f"The following columns are dropped because they are constants. {remove_cols}.\n"
-                f"Removed a total of {len(remove_cols)} columns.")
-    return drop(df, remove_cols)
-
-def remove_if_exists(df:PolarsFrame, cols:list[str]) -> PolarsFrame:
-    '''Removes the given columns if they exist in the dataframe.'''
-    remove_cols = list(set(cols).intersection(set(df.columns)))
-    logger.info(f"The following columns are dropped. {remove_cols}.\nRemoved a total of {len(remove_cols)} columns.")
-    return drop(df, remove_cols)
-
-#----------------------------------------------------------------------------------------------#
-# More advanced Methods
-#----------------------------------------------------------------------------------------------#
-
-def _ks_compare(
-    df:pl.DataFrame
-    , pair:Tuple[str, str]
-    , alt:KSAlternatives="two-sided"
-) -> Tuple[Tuple[str, str], float, float]:
-    
-    res = ks_2samp(df.get_column(pair[0]), df.get_column(pair[1]), alt)
-    return (pair, res.statistic, res.pvalue)
-
-def ks_compare(
-    df:PolarsFrame
-    , target:Optional[str] = None
-    , smaple_frac:float = 0.75
-    , test_cols:Optional[list[str]] = None
-    , alt: KSAlternatives = "two-sided"
-    , skip:int = 0
-    , max_comp:int = 1000
-) -> pl.DataFrame:
-    '''Run ks-stats on all non-discrete columns in the dataframe. If test_cols is None, it will infer non-discrete 
-    continuous columns. See docstring of discrete_inferral to see what is considered discrete. Provide the target 
-    so that it will not be included in the comparisons. Since ks 2 sample comparison is relatively expensive, we will
-    always sample 75% of the dataset, unless the user specifies a different sample_frac.
-
-    Note: this will only run on all 2 combinations of columns, starting from skip and end at 
-    skip + max_comp.
-
-    Note: The null hypothesis is that the two columns come from the same distribution. Therefore a small p-value means
-    that they do not come from the same distribution. Having p-value > threshold does not mean they have the same 
-    distribution automatically, and it requires more examination to reach the conclusion.
-    '''
-    if test_cols is None:
-        nums = [f for f in get_numeric_cols(df) if f not in discrete_inferral(df)]
-    else:
-        nums = test_cols
-
-    if target in nums:
-        nums.remove(target)
-    sorted(nums)
-    if isinstance(df, pl.LazyFrame):
-        df_test = lazy_sample(df.select(nums).lazy(), sample_frac=smaple_frac).collect()
-    else:
-        df_test = df.select(nums).sample(fraction=smaple_frac)
-
-    n_c2 = comb(len(nums), 2)
-    last_index = min(skip + max_comp, n_c2)
-    results = []
-    to_test = enumerate(combinations(nums, 2), start=skip)
-    pbar = tqdm(total=min(max_comp, n_c2 - skip), desc="Comparisons")
-    with ThreadPoolExecutor(max_workers=CPU_COUNT) as ex:
-        for f in as_completed(ex.submit(_ks_compare, df_test, p, alt) for i, p in to_test if i < last_index):
-            results.append(f.result())
-            pbar.update(1)
-
-    pbar.close()
-    return pl.from_records(results, schema=["combination", "ks-stats", "p-value"])
-
-def _dist_inferral(df:pl.DataFrame, c:str, dist:CommonContinuousDist) -> Tuple[str, float, float]:
-    res = kstest(df[c], dist)
-    return (c, res.statistic, res.pvalue)
-
-def dist_test(
-    df: PolarsFrame
-    , which_dist:CommonContinuousDist
-    , smaple_frac:float = 0.75
-    , target: Optional[str] = None
-) -> pl.DataFrame:
-    '''Tests if the numeric columns follow the given distribution by using the KS test. If
-    target is provided it will be excluded. The null hypothesis is that the columns follow the given distribution. 
-    We sample 75% of data because ks test is relatively expensive.
-    '''
-    
-    nums = get_numeric_cols(df, exclude=[target])
-    if isinstance(df, pl.LazyFrame):
-        df_test = lazy_sample(df.select(nums).lazy(), sample_frac=smaple_frac).collect()
-    else:
-        df_test = df.select(nums).sample(fraction=smaple_frac)
-
-    results = []
-    pbar = tqdm(total=len(nums), desc="Comparisons")
-    with ThreadPoolExecutor(max_workers=CPU_COUNT) as ex:
-        for f in as_completed(ex.submit(_dist_inferral, df_test, c, which_dist) for c in nums):
-            results.append(f.result())
-            pbar.update(1)
-
-    pbar.close()
-    return pl.from_records(results, schema=["feature", "ks-stats", "p-value"])
-
-def suggest_normal(
-    df:PolarsFrame
-    , target: Optional[str] = None
-    , threshold:float = 0.05
-) -> list[str]:
-    '''Suggests which columns are normally distributed. This takes the columns for which the null hypothesis
-    cannot be rejected in the dist_test (KS test).
-    '''
-    return dist_test(df, "norm", target=target).filter(pl.col("p-value") > threshold)\
-        .get_column("feature").to_list()
-
-def suggest_uniform(
-    df:PolarsFrame
-    , target: Optional[str] = None
-    , threshold:float = 0.05
-) -> list[str]:
-    '''Suggests which columns are uniformly distributed. This takes the columns for which the null hypothesis
-    cannot be rejected in the dist_test (KS test).
-    '''
-    return dist_test(df, "uniform", target=target).filter(pl.col("p-value") > threshold)\
-        .get_column("feature").to_list()
-
-def suggest_lognormal(
-    df:PolarsFrame
-    , target: Optional[str] = None
-    , threshold:float = 0.05
-) -> list[str]:
-    '''Suggests which columns are log-normally distributed. This takes the columns which the null hypothesis
-    cannot be rejected in the dist_test (KS test).
-    '''
-    return dist_test(df, "lognorm", target=target).filter(pl.col("p-value") > threshold)\
-        .get_column("feature").to_list()
-
-def suggest_dist(
-    df:PolarsFrame
-    , target: Optional[str] = None
-    , threshold:float = 0.05
-    , dist: CommonContinuousDist = "norm"
-) -> list[str]:
-    '''Suggests which columns follow the given distribution. This takes the columns which the null hypothesis
-    cannot be rejected in the dist_test (KS test).
-    '''
-    return dist_test(df, dist, target=target).filter(pl.col("p-value") > threshold)\
+from .type_alias import (
+    PolarsFrame
+    , KSAlternatives
+    , CommonContinuousDist
+    , CPU_COUNT
+    , POLARS_DATETIME_TYPES
+    , POLARS_NUMERICAL_TYPES
+)
+from .sample import (
+    lazy_sample
+)
+from .blueprint import(
+    Blueprint
+)
+
+import polars.selectors as cs
+import polars as pl
+import logging  
+from datetime import datetime 
+from typing import Any, Optional, Tuple
+from itertools import combinations
+from scipy.stats import (
+    ks_2samp
+    , kstest
+)
+from concurrent.futures import as_completed, ThreadPoolExecutor
+from tqdm import tqdm
+from math import comb
+
+logger = logging.getLogger(__name__)
+
+#----------------------------------------------------------------------------------------------#
+# Generic columns checks | Only works with Polars because Pandas's data types suck!            #
+#----------------------------------------------------------------------------------------------#
+
+def get_numeric_cols(df:PolarsFrame, exclude:Optional[list[str]]=None) -> list[str]:
+    if exclude is None:
+        selector = cs.numeric()
+    else:
+        selector = cs.numeric() & ~cs.by_name(exclude)
+    return df.select(selector).columns
+
+def get_string_cols(df:PolarsFrame, exclude:Optional[list[str]]=None) -> list[str]:
+    if exclude is None:
+        selector = cs.string()
+    else:
+        selector = cs.string() & ~cs.by_name(exclude)
+    return df.select(selector).columns
+
+def get_datetime_cols(df:PolarsFrame) -> list[str]:
+    '''Only gets datetime columns, will not infer from strings.'''
+    return df.select(cs.datetime()).columns
+
+def get_bool_cols(df:PolarsFrame) -> list[str]:
+    return df.select(cs.by_dtype(pl.Boolean)).columns
+
+def get_cols_regex(df:PolarsFrame, pattern:str) -> list[str]:
+    return df.select(cs.matches(pattern=pattern)).columns
+
+def lowercase_columns(df:PolarsFrame) -> PolarsFrame:
+    return df.rename({c: c.lower() for c in df.columns})
+
+def check_binary_target(df:PolarsFrame, target:str) -> bool:
+    target_uniques = df.lazy().select(pl.col(target).unique()).collect().get_column(target)
+    if len(target_uniques) != 2:
+        logger.error("Target is not binary.")
+        return False
+    elif not (0 in target_uniques and 1 in target_uniques):
+        logger.error("The binary target is not encoded as 0s and 1s.")
+        return False
+    return True
+    
+def check_target_cardinality(df:PolarsFrame, target:str) -> pl.DataFrame:
+    return df.lazy().groupby(target).count().sort(target).collect()
+
+def check_columns_types(df:PolarsFrame, cols:Optional[list[str]]=None) -> str:
+    '''Returns the unique types of given columns in a single string. If multiple types are present
+    they are joined by a |. If cols is not given, automatically uses all df's columns.'''
+    if cols is None:
+        check_cols:list[str] = df.columns
+    else:
+        check_cols:list[str] = cols 
+
+    types = set(dtype_mapping(t) for t in df.select(check_cols).dtypes)
+    return "|".join(types) if len(types) > 0 else "unknown"
+    
+# dtype can be a "pl.datatype" or just some random data for which we want to infer a generic type.
+def dtype_mapping(d: Any) -> str:
+    if isinstance(d, str) or d == pl.Utf8:
+        return "string"
+    elif isinstance(d, bool) or d == pl.Boolean:
+        return "bool"
+    elif isinstance(d, (int,float)) or d in POLARS_NUMERICAL_TYPES:
+        return "numeric"
+    elif isinstance(d, datetime) or d in POLARS_DATETIME_TYPES:
+        return "datetime"
+    else:
+        return "other/unknown"
+
+#----------------------------------------------------------------------------------------------#
+# Prescreen Inferral, Removal Methods                                                          #
+#----------------------------------------------------------------------------------------------#
+
+# Add a slim option that returns fewer stats? This is generic describe.
+# Separate str and numeric?
+def describe(
+    df:PolarsFrame
+    , sample_frac:float = 0.75
+) -> pl.DataFrame:
+    '''Profile the data.
+
+        Arguments:
+            df: Either an eager dataframe or a lazy dataframe
+            sample_frac: If input is a LazyFrame, a sample of sample_frac will be used. If input is eager,
+            no sampling will be done.
+
+        Returns:
+            a dataframe containing the necessary information.
+    '''
+
+    if isinstance(df, pl.LazyFrame):
+        df_local = lazy_sample(df, sample_frac=sample_frac)
+    else:
+        df_local = df
+    
+    temp = df_local.describe()
+    desc = temp.drop_in_place("describe")
+    # Get unique
+    unique_counts = get_unique_count(df_local).with_columns(
+        unique_pct = pl.col("n_unique") / len(df_local)
+    )
+    # Skew and Kurtosis
+    skew_and_kt_data = df_local.lazy().select(
+        pl.all().skew().prefix("skew:")
+        , pl.all().skew().prefix("kurtosis:")
+    ).collect().row(0)
+
+    n_cols = len(df_local.columns)
+    skew_and_kt = pl.from_records((df_local.columns, skew_and_kt_data[:n_cols], skew_and_kt_data[n_cols:])
+                                  , schema=["column", "skew", "kurtosis"])
+
+    # Get a basic string description of the data type.
+    dtypes_dict = dict(zip(df_local.columns, map(dtype_mapping, df_local.dtypes)))
+    # Combine all
+    nums = ("count", "null_count", "mean", "std", "median", "25%", "75%")
+    final = temp.transpose(include_header=True, column_names=desc).with_columns(
+        pl.col(c).cast(pl.Float64) for c in nums
+    ).with_columns(
+        null_pct = pl.col("null_count")/pl.col("count")
+        , dtype = pl.col("column").map_dict(dtypes_dict)
+    ).join(unique_counts, on="column").join(skew_and_kt, on="column")
+    
+    return final.select('column','count','null_count','null_pct','n_unique'
+                        , 'unique_pct','mean','std','min','max','25%'
+                        , 'median','75%', "skew", "kurtosis",'dtype')
+
+# Numeric only describe. Be more detailed.
+
+# String only describe. Be more detailed about interesting string stats.
+
+def describe_str(df:PolarsFrame
+    , words_to_count:Optional[list[str]]=None
+    , sample_frac:float = 0.75
+) -> pl.DataFrame:
+    '''Gives some statistics about the string columns. Optionally you may pass a list
+    of strings to compute the total occurrances of each of the words in the string columns. If input is a LazyFrame, 
+    a sample of sample_pct will be used, and sample_pct will only be used in the lazy case. 
+
+    '''
+    strs = get_string_cols(df)
+    df_str = df.select(strs)
+    if isinstance(df, pl.LazyFrame):
+        df_str = lazy_sample(df_str, sample_frac=sample_frac).collect()
+
+    nstrs = len(strs)
+    stats = df.select(strs).select(
+        pl.all().null_count().prefix("nc:"),
+        pl.all().max().prefix("max:"),
+        pl.all().min().prefix("min:"),
+        pl.all().mode().first().prefix("mode:"),
+        pl.all().str.lengths().min().prefix("min_byte_len:"),
+        pl.all().str.lengths().max().prefix("max_byte_len:"),
+        pl.all().str.lengths().mean().prefix("avg_byte_len:"),
+        pl.all().str.lengths().median().prefix("median_byte_len:"),
+        pl.all().str.count_match(r"\s").mean().prefix("avg_space_cnt:"),
+        pl.all().str.count_match(r"[0-9]").mean().prefix("avg_digit_cnt:"),
+        pl.all().str.count_match(r"[A-Z]").mean().prefix("avg_cap_cnt:"),
+        pl.all().str.count_match(r"[a-z]").mean().prefix("avg_lower_cnt:")
+    ).row(0)
+    output = {
+        "features":strs,
+        "null_count": stats[:nstrs],
+        "min": stats[nstrs: 2*nstrs],
+        "max": stats[2*nstrs: 3*nstrs],
+        "mode": stats[3*nstrs: 4*nstrs],
+        "min_byte_len": stats[4*nstrs: 5*nstrs],
+        "max_byte_len": stats[5*nstrs: 6*nstrs],
+        "avg_byte_len": stats[6*nstrs: 7*nstrs],
+        "median_byte_len": stats[7*nstrs: 8*nstrs],
+        "avg_space_cnt": stats[8*nstrs: 9*nstrs],
+        "avg_digit_cnt": stats[9*nstrs: 10*nstrs],
+        "avg_cap_cnt": stats[10*nstrs: 11*nstrs],
+        "avg_lower_cnt": stats[11*nstrs: ],
+    }
+
+    if isinstance(words_to_count, list):
+        for w in words_to_count:
+            t = df_str.select(pl.all().str.count_match(w).sum().prefix("wc:")).row(0)
+            output["total_"+ w + "_count"] = t
+
+    return pl.from_dict(output)
+
+# -----------------------------------------------------------------------------------------------
+def drop(df:PolarsFrame, to_drop:list[str]) -> PolarsFrame:
+    if isinstance(df, pl.LazyFrame):
+        return df.blueprint.drop(to_drop)
+    return df.drop(to_drop)
+
+def non_numeric_removal(df:PolarsFrame, include_bools:bool=True) -> PolarsFrame:
+    '''Removes all non-numeric columns. If include_bools = True, then keep boolean columns.'''
+    
+    if include_bools:
+        selector = ~(cs.numeric()|cs.by_dtype(pl.Boolean))
+    else:
+        selector = ~cs.numeric()
+
+    non_nums = df.select(selector).columns
+    logger.info(f"The following columns are dropped because they are not numeric: {non_nums}.\n"
+                f"Removed a total of {len(non_nums)} columns.")
+    
+    return drop(df, non_nums)
+
+# Check if columns are duplicates. Might take time.
+def duplicate_inferral():
+    # Get profiles first.
+    # Divide into categories: bools, strings, numerics, datetimes.
+    # Then cut down list to columns that have the same min, max, n_unique and null_count.
+    # Then check equality..
+    pass
+
+def pattern_inferral(
+    df: PolarsFrame
+    , pattern:str
+    , sample_frac:float = 0.75
+    , sample_count:int = 100_000
+    , sample_rounds:int = 3
+    , threshold:float = 0.9
+    , count_null:bool = True
+) -> list[str]:
+    '''Find all string columns whose elements reasonably match the given pattern. The match logic can 
+    be tuned using the all the parameters.
+
+    Arguments:
+        sample_frac: the pct of the total dataframe to use as basis
+        sample_count: from the basis, how many rows to sample for each round 
+        sample_rounds: how many rounds of sampling we are doing
+        threhold: For each round, what is the match% that is needed to be a counted as a success. For instance, 
+        in round 1, for column x, we have 92% match rate, and threshold = 0.9. We count column x as a match for 
+        this round. In the end, the column must match for every round to be considered a real match.
+        count_null: for individual matches, do we want to count null as a match or not? If the column has high null pct,
+        the non-null values might mostly match the pattern. In this case, using count_null = True will match the column, 
+        while count_null = False will most likely exclude the column.
+
+    Returns:
+        a list of columns that pass the matching test
+    
+    '''
+    
+    strs = get_string_cols(df)
+    df_local = lazy_sample(df.lazy(), sample_frac=sample_frac).collect()    
+    matches:set[str] = set(strs)
+    sample_size = min(sample_count, len(df_local))
+    for _ in range(sample_rounds):
+        df_sample = df_local.sample(n = sample_size)
+        fail = df_sample.select(
+            (pl.when(pl.col(s).is_null()).then(count_null).otherwise(
+                pl.col(s).str.contains(pattern)
+            ).sum()/sample_size).alias(s) for s in strs
+        ).transpose(include_header=True, column_names=["pattern_match_pct"])\
+        .filter(pl.col("pattern_match_pct") < threshold).get_column("column")
+        # If the match failes in this round, remove the column.
+        matches.difference_update(fail)
+
+    return list(matches)
+
+def pattern_removal(
+    df: PolarsFrame
+    , pattern:str
+    , sample_pct:float = 0.75
+    , sample_count:int = 100_000
+    , sample_rounds:int = 3
+    , threshold:float = 0.9
+    , count_null:bool = True
+) -> PolarsFrame:
+    
+    remove_cols = pattern_inferral(
+        df
+        , pattern
+        , sample_pct
+        , sample_count
+        , sample_rounds
+        , threshold 
+        , count_null
+    )
+    logger.info(f"The following columns are dropped because they match the element pattern: {pattern}.\n"
+                f"{remove_cols}\n"
+                f"Removed a total of {len(remove_cols)} columns.")
+    
+    return drop(df, remove_cols)
+
+def email_inferral(
+    df: PolarsFrame
+    , sample_pct:float = 0.75
+    , sample_count:int = 100_000
+    , sample_rounds:int = 3
+    , threshold:float = 0.9
+    , count_null:bool = True
+) -> list[str]:
+    # Why does this regex not work?
+    # r'([A-Za-z0-9]+[.-_])*[A-Za-z0-9]+@[A-Za-z0-9-]+(\.[A-Z|a-z]{2,})+'
+    return pattern_inferral(
+        df
+        , r'\S+@\S+\.\S+'
+        , sample_pct
+        , sample_count
+        , sample_rounds
+        , threshold 
+        , count_null
+    )
+
+def email_removal(
+    df: PolarsFrame
+    , sample_pct:float = 0.75
+    , sample_count:int = 100_000
+    , sample_rounds:int = 3
+    , threshold:float = 0.9
+    , count_null:bool = True
+) -> PolarsFrame:
+    
+    emails = email_inferral(df, sample_pct, sample_count, sample_rounds, threshold, count_null)
+    logger.info(f"The following columns are dropped because they are emails. {emails}.\n"
+            f"Removed a total of {len(emails)} columns.")
+    
+    return drop(df, emails)
+
+# Check for columns that are US zip codes.
+# Might add options for other countries later.
+def zipcode_inferral():
+    # Match string using pattern inferral
+    # Take a look at integers too, are they always 5 digits? 
+    pass
+
+def date_inferral(df:PolarsFrame) -> list[str]:
+    '''Infers date columns in dataframe. This inferral is not perfect.'''
+    logger.info("Date Inferral is error prone due to the huge variety of date formats. Please use with caution.")
+    
+    dates = [c for c,t in zip(df.columns, df.dtypes) if t in POLARS_DATETIME_TYPES]
+    strings = get_string_cols(df)
+    # MIGHT REWRITE THIS LOGIC
+    # Might be memory intensive on big dataframes.
+    sample_size = min(len(df), 100_000)
+    sample_df = df.lazy().select(strings)\
+        .drop_nulls().collect()\
+        .sample(n = sample_size).select(
+            # Cleaning the string first. Only try to catch string dates which are in the first split by space
+           pl.col(s).str.strip().str.replace_all("(/|\.)", "-").str.split(by=" ").list.first() 
+           for s in strings
+        )
+    for s in strings:
+        try:
+            c = sample_df[s].str.to_date(strict=False)
+            if 1 - c.null_count()/sample_size >= 0.15: # if at least 15% valid (able to be converted)
+                # This last check is to account for single digit months.
+                # 3/3/1995 will not be parsed to a string because standard formats require 03/03/1995
+                # At least 15% of dates naturally have both month and day as 2 digits numbers
+                dates.append(s)
+        except: # noqa: E722
+            # Very stupid code, but I have to do it...
+            pass
+    
+    return dates
+
+def date_removal(df:PolarsFrame) -> PolarsFrame:
+    '''Removes all date columns from dataframe. This algorithm will try to infer if string column is date.'''
+
+    remove_cols = date_inferral(df) 
+    logger.info(f"The following columns are dropped because they are dates. {remove_cols}.\n"
+                f"Removed a total of {len(remove_cols)} columns.")
+    return drop(df, remove_cols)
+
+def null_inferral(df:PolarsFrame, threshold:float=0.5) -> list[str]:
+    '''Infers columns that have more than threshold pct of null values. Threshold should be between 0 and 1.'''
+    return (df.lazy().null_count().collect()/len(df)).transpose(include_header=True, column_names=["null_pct"])\
+                    .filter(pl.col("null_pct") >= threshold)\
+                    .get_column("column").to_list()
+
+def null_removal(df:PolarsFrame, threshold:float=0.5) -> PolarsFrame:
+    '''Removes columns with more than threshold pct of null values. Threshold should be between 0 and 1.'''
+
+    remove_cols = null_inferral(df, threshold) 
+    logger.info(f"The following columns are dropped because they have more than {threshold*100:.2f}%"
+                f" null values. {remove_cols}.\n"
+                f"Removed a total of {len(remove_cols)} columns.")
+    return drop(df, remove_cols)
+
+def var_inferral(df:PolarsFrame, threshold:float, target:str) -> list[str]:
+    '''Infers columns that have lower than threshold variance. Target will not be included.'''
+    return df.lazy().select(
+                pl.col(x).var() for x in get_numeric_cols(df) if x != target
+            ).collect().transpose(include_header=True, column_names=["var"])\
+            .filter(pl.col("var") < threshold).get_column("column").to_list() 
+
+def var_removal(df:PolarsFrame, threshold:float, target:str) -> PolarsFrame:
+    '''Removes features with low variance. Features with > threshold variance will be kept. 
+        Threshold should be positive.'''
+
+    remove_cols = var_inferral(df, threshold, target) 
+    logger.info(f"The following columns are dropped because they have lower than {threshold} variance. {remove_cols}.\n"
+                f"Removed a total of {len(remove_cols)} columns.")
+    return drop(df, remove_cols)
+
+# Really this is just an alias
+regex_inferral = get_cols_regex
+
+def regex_removal(df:PolarsFrame, pattern:str, lowercase:bool=False) -> PolarsFrame:
+    '''Remove columns if they satisfy some regex rules.'''
+    remove_cols = get_cols_regex(df, pattern, lowercase)
+    logger.info(f"The following columns are dropped because their names satisfy the regex rule: {pattern}."
+                f" {remove_cols}.\n"
+                f"Removed a total of {len(remove_cols)} columns.")
+    
+    return drop(df, remove_cols)
+
+def get_unique_count(df:PolarsFrame) -> pl.DataFrame:
+    '''Gets unique counts for columns.'''
+    return df.lazy().select(
+        pl.col(x).n_unique() for x in df.columns
+    ).collect().transpose(include_header=True, column_names=["n_unique"])
+
+# Really this is just an alias
+def unique_inferral(df:PolarsFrame, threshold:float=0.9) -> list[str]:
+    '''Infers columns that have higher than threshold pct of unique values.'''
+    return get_unique_count(df).with_columns(
+        (pl.col("n_unique")/len(df)).alias("unique_pct")
+    ).filter(pl.col("unique_pct") >= threshold)\
+    .get_column("column").to_list()
+
+def unique_removal(df:PolarsFrame, threshold:float=0.9) -> PolarsFrame:
+    '''Remove columns that have higher than threshold pct of unique values.'''
+
+    remove_cols = unique_inferral(df, threshold)
+    logger.info(f"The following columns are dropped because more than {threshold*100:.2f}% of unique values."
+                f" {remove_cols}.\n"
+                f"Removed a total of {len(remove_cols)} columns.")
+    return drop(df, remove_cols)
+
+# Is this a good definition?
+def discrete_inferral(df:PolarsFrame
+    , threshold:float=0.1
+    , max_n_unique:int=100
+    , exclude:Optional[list[str]]=None
+) -> list[str]:
+    '''
+        A column that satisfies either n_unique < max_n_unique or unique_pct < threshold 
+        will be considered discrete.
+    '''
+    exclude_list = [] if exclude is None else exclude
+    return get_unique_count(df).filter(
+        ((pl.col("n_unique") < max_n_unique) | (pl.col("n_unique")/len(df) < threshold)) 
+        & (~pl.col("column").is_in(exclude_list)) # is not in
+    ).get_column("column").to_list()
+
+def conti_inferral(
+    df:PolarsFrame
+    , discrete_threshold:float = 0.1
+    , discrete_max_n_unique:int = 100
+    , exclude:Optional[list[str]]=None
+) -> list[str]:
+    exclude_list = [] if exclude is None else exclude
+    discrete = discrete_inferral(df, discrete_threshold, discrete_max_n_unique)
+    return df.select(cs.numeric() & ~cs.by_name(exclude_list) & ~cs.by_name(discrete)).columns
+
+def constant_inferral(df:PolarsFrame, include_null:bool=True) -> list[str]:
+    temp = get_unique_count(df).filter(pl.col("n_unique") <= 2)
+    remove_cols = temp.filter(pl.col("n_unique") == 1).get_column("column").to_list() 
+    if include_null: # This step is kind of inefficient right now.
+        binary = temp.filter(pl.col("n_unique") == 2).get_column("column")
+        nc = df.lazy().select(binary).null_count().collect().row(0)
+        remove_cols.extend(
+            binary[i] for i in range(len(nc)) if nc[i] > 0
+        )
+
+    return remove_cols
+
+def constant_removal(df:PolarsFrame, include_null:bool=True) -> PolarsFrame:
+    '''Removes all constant columns from dataframe.
+    
+        Arguments:
+            df:
+            include_null: if true, then columns with two distinct values like [value_1, null] will be considered a 
+                constant column.
+
+        Returns: 
+            the df without constant columns
+    '''
+    remove_cols = constant_inferral(df, include_null)
+    logger.info(f"The following columns are dropped because they are constants. {remove_cols}.\n"
+                f"Removed a total of {len(remove_cols)} columns.")
+    return drop(df, remove_cols)
+
+def remove_if_exists(df:PolarsFrame, cols:list[str]) -> PolarsFrame:
+    '''Removes the given columns if they exist in the dataframe.'''
+    remove_cols = list(set(cols).intersection(set(df.columns)))
+    logger.info(f"The following columns are dropped. {remove_cols}.\nRemoved a total of {len(remove_cols)} columns.")
+    return drop(df, remove_cols)
+
+#----------------------------------------------------------------------------------------------#
+# More advanced Methods
+#----------------------------------------------------------------------------------------------#
+
+def _ks_compare(
+    df:pl.DataFrame
+    , pair:Tuple[str, str]
+    , alt:KSAlternatives="two-sided"
+) -> Tuple[Tuple[str, str], float, float]:
+    
+    res = ks_2samp(df.get_column(pair[0]), df.get_column(pair[1]), alt)
+    return (pair, res.statistic, res.pvalue)
+
+def ks_compare(
+    df:PolarsFrame
+    , target:Optional[str] = None
+    , smaple_frac:float = 0.75
+    , test_cols:Optional[list[str]] = None
+    , alt: KSAlternatives = "two-sided"
+    , skip:int = 0
+    , max_comp:int = 1000
+) -> pl.DataFrame:
+    '''Run ks-stats on all non-discrete columns in the dataframe. If test_cols is None, it will infer non-discrete 
+    continuous columns. See docstring of discrete_inferral to see what is considered discrete. Provide the target 
+    so that it will not be included in the comparisons. Since ks 2 sample comparison is relatively expensive, we will
+    always sample 75% of the dataset, unless the user specifies a different sample_frac.
+
+    Note: this will only run on all 2 combinations of columns, starting from skip and end at 
+    skip + max_comp.
+
+    Note: The null hypothesis is that the two columns come from the same distribution. Therefore a small p-value means
+    that they do not come from the same distribution. Having p-value > threshold does not mean they have the same 
+    distribution automatically, and it requires more examination to reach the conclusion.
+    '''
+    if test_cols is None:
+        nums = [f for f in get_numeric_cols(df) if f not in discrete_inferral(df)]
+    else:
+        nums = test_cols
+
+    if target in nums:
+        nums.remove(target)
+    sorted(nums)
+    if isinstance(df, pl.LazyFrame):
+        df_test = lazy_sample(df.select(nums).lazy(), sample_frac=smaple_frac).collect()
+    else:
+        df_test = df.select(nums).sample(fraction=smaple_frac)
+
+    n_c2 = comb(len(nums), 2)
+    last_index = min(skip + max_comp, n_c2)
+    results = []
+    to_test = enumerate(combinations(nums, 2), start=skip)
+    pbar = tqdm(total=min(max_comp, n_c2 - skip), desc="Comparisons")
+    with ThreadPoolExecutor(max_workers=CPU_COUNT) as ex:
+        for f in as_completed(ex.submit(_ks_compare, df_test, p, alt) for i, p in to_test if i < last_index):
+            results.append(f.result())
+            pbar.update(1)
+
+    pbar.close()
+    return pl.from_records(results, schema=["combination", "ks-stats", "p-value"])
+
+def _dist_inferral(df:pl.DataFrame, c:str, dist:CommonContinuousDist) -> Tuple[str, float, float]:
+    res = kstest(df[c], dist)
+    return (c, res.statistic, res.pvalue)
+
+def dist_test(
+    df: PolarsFrame
+    , which_dist:CommonContinuousDist
+    , smaple_frac:float = 0.75
+    , target: Optional[str] = None
+) -> pl.DataFrame:
+    '''Tests if the numeric columns follow the given distribution by using the KS test. If
+    target is provided it will be excluded. The null hypothesis is that the columns follow the given distribution. 
+    We sample 75% of data because ks test is relatively expensive.
+    '''
+    
+    nums = get_numeric_cols(df, exclude=[target])
+    if isinstance(df, pl.LazyFrame):
+        df_test = lazy_sample(df.select(nums).lazy(), sample_frac=smaple_frac).collect()
+    else:
+        df_test = df.select(nums).sample(fraction=smaple_frac)
+
+    results = []
+    pbar = tqdm(total=len(nums), desc="Comparisons")
+    with ThreadPoolExecutor(max_workers=CPU_COUNT) as ex:
+        for f in as_completed(ex.submit(_dist_inferral, df_test, c, which_dist) for c in nums):
+            results.append(f.result())
+            pbar.update(1)
+
+    pbar.close()
+    return pl.from_records(results, schema=["feature", "ks-stats", "p-value"])
+
+def suggest_normal(
+    df:PolarsFrame
+    , target: Optional[str] = None
+    , threshold:float = 0.05
+) -> list[str]:
+    '''Suggests which columns are normally distributed. This takes the columns for which the null hypothesis
+    cannot be rejected in the dist_test (KS test).
+    '''
+    return dist_test(df, "norm", target=target).filter(pl.col("p-value") > threshold)\
+        .get_column("feature").to_list()
+
+def suggest_uniform(
+    df:PolarsFrame
+    , target: Optional[str] = None
+    , threshold:float = 0.05
+) -> list[str]:
+    '''Suggests which columns are uniformly distributed. This takes the columns for which the null hypothesis
+    cannot be rejected in the dist_test (KS test).
+    '''
+    return dist_test(df, "uniform", target=target).filter(pl.col("p-value") > threshold)\
+        .get_column("feature").to_list()
+
+def suggest_lognormal(
+    df:PolarsFrame
+    , target: Optional[str] = None
+    , threshold:float = 0.05
+) -> list[str]:
+    '''Suggests which columns are log-normally distributed. This takes the columns which the null hypothesis
+    cannot be rejected in the dist_test (KS test).
+    '''
+    return dist_test(df, "lognorm", target=target).filter(pl.col("p-value") > threshold)\
+        .get_column("feature").to_list()
+
+def suggest_dist(
+    df:PolarsFrame
+    , target: Optional[str] = None
+    , threshold:float = 0.05
+    , dist: CommonContinuousDist = "norm"
+) -> list[str]:
+    '''Suggests which columns follow the given distribution. This takes the columns which the null hypothesis
+    cannot be rejected in the dist_test (KS test).
+    '''
+    return dist_test(df, dist, target=target).filter(pl.col("p-value") > threshold)\
         .get_column("feature").to_list()
```

### Comparing `dsds-0.0.16/src/dsds/transform.py` & `dsds-0.0.17/src/dsds/transform.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,644 +1,748 @@
-from __future__ import annotations
-
-from .type_alias import (
-    PolarsFrame
-    , ImputationStrategy
-    , ScalingStrategy
-    , PowerTransformStrategy
-    , clean_strategy_str
-    , CPU_COUNT
-)
-from .prescreen import (
-    get_bool_cols
-    , get_string_cols
-    , get_unique_count
-    , check_binary_target
-    , check_columns_types
-)
-from .blueprint import( # Need this for Polars extension to work
-    Blueprint
-)
-import logging
-import polars as pl
-from typing import Optional, Tuple
-from scipy.stats._morestats import (
-    yeojohnson_normmax
-    , boxcox_normmax
-)
-from concurrent.futures import as_completed, ThreadPoolExecutor
-from tqdm import tqdm
-
-# A lot of companies are still using Python < 3.10
-# So I am not using match statements
-# Well, it does say in project description that we need Python 3.10.
-
-logger = logging.getLogger(__name__)
-
-
-def impute(
-    df:PolarsFrame
-    , cols:list[str]
-    , strategy:ImputationStrategy = 'median'
-    , const:float = 1.
-) -> PolarsFrame:
-    '''Imputes the given columns using the given strategy.
-
-        Arguments:
-            df: either a eager/lazy Polars dataframe
-            cols: cols to impute
-            strategy: one of 'mean', 'avg', 'average', 'median', 'const', 'constant', 'mode', 'most_frequent'. Some are 
-            just alternative names for the same strategy.
-            const: only uses this value if strategy = const
-
-        Returns:
-            the imputed lazy / eager dataframe.
-    '''
-    s = clean_strategy_str(strategy)
-    # Given Strategy, define expressions
-    if s == "median":
-        all_medians = df.lazy().select(cols).median().collect().row(0)
-        exprs = (pl.col(c).fill_null(all_medians[i]) for i,c in enumerate(cols))
-    elif s in ("mean", "avg", "average"):
-        all_means = df.lazy().select(cols).mean().collect().row(0)
-        exprs = (pl.col(c).fill_null(all_means[i]) for i,c in enumerate(cols))
-    elif s in ("const", "constant"):
-        exprs = (pl.col(c).fill_null(const) for c in cols)
-    elif s in ("mode", "most_frequent"):
-        all_modes = df.lazy().select(cols).select(pl.all().mode().first()).collect().row(0)
-        exprs = (pl.col(c).fill_null(all_modes[i]) for i,c in enumerate(cols))
-    else:
-        raise TypeError(f"Unknown imputation strategy: {strategy}")
-
-    # Need to cast to list so that pickle can work with it
-    # This is unfortunate because we will be looping over this list twice... Whatever...
-    if isinstance(df, pl.LazyFrame):
-        return df.blueprint.with_columns(list(exprs)) 
-    return df.with_columns(exprs)
-
-def scale(
-    df:PolarsFrame
-    , cols:list[str]
-    , strategy:ScalingStrategy="normal"
-    , const:float = 1.0
-) -> PolarsFrame:
-    '''Scale given columns using the given strategy.
-        Arguments:
-            df: either a lazy or eager dataframe
-            cols: list of columns to scale
-            strategy: one of 'normal', 'standard', 'normalize', 'min_max', 'const', 'constant',
-            where normal = standard = normalize.
-            const: only uses this value if strategy = const
-
-        Returns:
-            the scaled lazy / eager dataframe.
-    
-    '''
-    types = check_columns_types(df, cols)
-    if types != "numeric":
-        raise TypeError(f"Scaling can only be used on numeric columns, not {types} types.")
-
-    s = clean_strategy_str(strategy)
-    if s in ("normal", "standard", "normalize"):
-        mean_std = df.select(cols).lazy().select(
-            pl.all().mean().prefix("mean:")
-            , pl.all().std().prefix("std:")
-        ).collect().row(0)
-        exprs = ( (pl.col(c) - mean_std[i])/(mean_std[i + len(cols)]) for i,c in enumerate(cols) )
-    elif s == "min_max":
-        min_max = df.select(cols).lazy().select(
-            pl.all().min().prefix("min:"),
-            pl.all().max().prefix("max:")
-        ).collect().row(0) # All mins come first, then maxs
-        exprs = ( (pl.col(c) - min_max[i])/((min_max[i + len(cols)] - min_max[i])) for i,c in enumerate(cols) )
-    elif s in ("const", "constant"):
-        exprs = (pl.col(c)/const for c in cols)
-    else:
-        raise TypeError(f"Unknown scaling strategy: {strategy}")
-
-    if isinstance(df, pl.LazyFrame):
-        return df.blueprint.with_columns(list(exprs))
-    return df.with_columns(exprs)
-
-def boolean_transform(df:PolarsFrame, keep_null:bool=True) -> PolarsFrame:
-    '''Converts all boolean columns into binary columns.
-
-        Arguments:
-            df: either a lazy or eager Polars DataFrame
-            keep_null: if true, null will be kept. If false, null will be mapped to 0.
-
-        Returns:
-            a dataframe with booleans mapped to 0s and 1s.
-    '''
-    bool_cols = get_bool_cols(df)
-    if keep_null: # Directly cast. If null, then cast will also return null
-        exprs = (pl.col(c).cast(pl.UInt8) for c in bool_cols)
-    else: # Cast. Then fill null to 0s.
-        exprs = (pl.col(c).cast(pl.UInt8).fill_null(0) for c in bool_cols)
-
-    if isinstance(df, pl.LazyFrame):
-        return df.blueprint.with_columns(list(exprs))
-    return df.with_columns(exprs)
-
-def one_hot_encode(
-    df:PolarsFrame
-    , cols:Optional[list[str]]=None
-    , separator:str="_"
-    , drop_first:bool=False
-) -> PolarsFrame:
-    '''One hot encoding. The separator must be a single character.'''
-    
-    if isinstance(cols, list):
-        types = check_columns_types(df, cols)
-        if types != "string":
-            raise TypeError(f"One-hot encoding can only be used on string columns, not {types} types.")
-        str_cols = cols
-    else:
-        str_cols = get_string_cols(df)
-
-    if isinstance(df, pl.LazyFrame):
-        temp = df.lazy().select(str_cols).groupby(1).agg(
-            pl.all().unique().sort()
-        ).select(str_cols)
-        exprs:list[pl.Expr] = []
-        start_index = int(drop_first)
-        one = pl.lit(1, dtype=pl.UInt8) # Avoid casting 
-        zero = pl.lit(0, dtype=pl.UInt8) # Avoid casting
-        for t in temp.collect().get_columns():
-            u:pl.List = t[0] # t is a Series which contains a single series/list, so u is a series/list
-            if len(u) > 1:
-                exprs.extend(
-                    pl.when(pl.col(t.name) == u[i]).then(one).otherwise(zero).alias(t.name + separator + u[i])
-                    for i in range(start_index, len(u)) 
-                )
-            else:
-                logger.info(f"During one-hot-encoding, the column {t.name} is found to have 1 unique value. Dropped.")
-        
-        return df.blueprint.with_columns(exprs).blueprint.drop(str_cols)
-    else:
-        return df.to_dummies(columns=str_cols, separator=separator, drop_first=drop_first)
-
-# def fixed_sized_encode(df:pl.DataFrame, num_cols:list[str], bin_size:int=50) -> TransformationResult:
-#     '''Given a continuous variable, take the smallest `bin_size` of them, and call them bin 1, take the next
-#     smallest `bin_size` of them and call them bin 2, etc...
-    
-#     '''
-#     pass
-
-
-# REWRITE THIS
-# def percentile_encode(df:pl.DataFrame
-#     , cols:list[str]=None
-#     , exclude:list[str]=None
-# ) -> FitTransform:
-#     '''Bin your continuous variable X into X_percentiles. This will create at most 100 + 1 bins, 
-#         where each percentile could potentially be a bin and null will be mapped to bin = 0. 
-#         Bin 1 means percentile 0 to 1. Generally, bin X groups the population from bin X-1 to 
-#         bin X into one bucket.
-
-#         I see some potential optimization opportunities here.
-
-#         Arguments:
-#             df:
-#             num_cols: 
-#             exclude:
-
-#         Returns:
-#             (A transformed dataframe, a mapping table (value to percentile))
-    
-#     '''
-
-#     # Percentile Binning
-
-#     num_list:list[str] = []
-#     exclude_list:list[str] = [] if exclude is None else exclude
-#     if isinstance(cols, list):
-#         types = check_columns_types(df, cols)
-#         if types != "numeric":
-#             raise ValueError(f"Percentile encoding can only be used on numeric columns, not {types} types.")
-#         num_list.extend(cols)
-#     else:
-#         num_list.extend(get_numeric_cols(df, exclude=exclude_list))
-
-#     exprs:list[pl.Expr] = []
-#     all_mappings = []
-#     for c in num_list:
-#         percentile = df.groupby(c).agg(pl.count().alias("cnt"))\
-#             .sort(c)\
-#             .with_columns(
-#                 ((pl.col("cnt").cumsum()*100)/len(df)).ceil().alias("percentile")
-#             ).groupby("percentile")\
-#             .agg(
-#                 pl.col(c).min().alias("min"),
-#                 pl.col(c).max().alias("max"),
-#                 pl.col("cnt").sum().alias("cnt"),
-#             ).sort("percentile").select(
-#                 pl.lit(c).alias("feature"),
-#                 pl.col("percentile").cast(pl.UInt8),
-#                 "min",
-#                 "max",
-#                 "cnt",
-#             )
-        
-#         first_row = percentile.select("percentile","min", "max").to_numpy()[0, :] # First row
-#         # Need to handle an extreme case when percentile looks like 
-#         # percentile   min   max
-#         #  p1         null  null
-#         #  p2          ...   ...
-#         # This happens when there are so many nulls in the column.
-#         if np.isnan(first_row[2]):
-#             # Discard the first row if this is the case. 
-#             percentile = percentile.slice(1, length = None)
-
-#         # Only work on non null values. Null will be mapped to default value anyway.
-#         temp_df = df.lazy().filter(pl.col(c).is_not_null()).sort(c).set_sorted(c)\
-#             .join_asof(other=percentile.lazy().set_sorted("max"), left_on=c, right_on="max", strategy="forward")\
-#             .select(c, "percentile")\
-#             .unique().collect()
-        
-#         real_mapping = dict(zip(temp_df[c], temp_df["percentile"]))
-#         # a representation of the mapping, needed for recreating this.
-#         repr_mapping = dict(zip(percentile["max"], percentile["percentile"]))
-#         all_mappings.append(repr_mapping)
-#         exprs.append(
-#             pl.col(c).map_dict(real_mapping, default=0).cast(pl.UInt8)
-#         )
-
-#     res = df.with_columns(exprs)
-#     encoder_rec = EncoderRecord(features=num_list, strategy=EncodingStrategy.PERCENTILE, mappings=all_mappings)
-#     return FitTransform(transformed=res, mapping=encoder_rec)
-
-def binary_encode(
-    df:PolarsFrame
-    , cols:Optional[list[str]]=None
-    , exclude:Optional[list[str]]=None
-) -> PolarsFrame:
-    '''Encode the given columns as binary values. Only hands string binaries at this moment. Just a short-hand for 
-        one-hot-encoding for binary string columns.
-
-        Arguments:
-            df:
-            binary_cols: the binary_cols you wish to convert. If no input, will infer.
-            exclude: the columns you wish to exclude in this transformation. 
-
-        Returns: 
-            (the transformed dataframe, mapping table between old values to [0,1])
-    '''
-
-    if cols is None:
-        str_cols = get_string_cols(df)
-        exclude = [] if exclude is None else exclude
-        binary_list = get_unique_count(df)\
-            .filter( # Binary + Not Exclude + Only String
-                (pl.col("n_unique") == 2) & (~pl.col("column").is_in(exclude)) & (pl.col("column").is_in(str_cols))
-            ).get_column("column").to_list()
-
-    else: # No need to do all that type checking steps because we are gonna do that in one-hot anyways
-        binary_list = cols
-    
-    return one_hot_encode(df, cols=binary_list, drop_first=True)
-
-def force_binary(
-    df:PolarsFrame
-    , cols:Optional[list[str]]=None
-):
-    '''
-    Force every binary column, no matter what data type, to be turned into 0s and 1s by the order of the elements. If a 
-    column has two unique values like [null, "haha"], then null will be mapped to 0 and "haha" to 1.
-    '''
-    if cols is None:
-        binary_list = get_unique_count(df)\
-            .filter(pl.col("n_unique") == 2)\
-            .get_column("column").to_list()
-    else:
-        binary_list = cols
-
-    temp = df.lazy().select(binary_list).groupby(1).agg(
-            pl.all().unique().sort()
-        ).select(binary_list) # Need this to get rid of the literal 1 column
-    exprs:list[pl.Expr] = []
-    one = pl.lit(1, dtype=pl.UInt8) # Avoid casting 
-    zero = pl.lit(0, dtype=pl.UInt8) # Avoid casting
-    for t in temp.collect().get_columns():
-        u:pl.List = t[0] # t is a Series which contains a single list which contains the 2 unique values 
-        if len(u) == 2:
-            exprs.append(
-                pl.when(pl.col(t.name) == u[0]).then(zero).otherwise(one).alias(t.name)
-            )
-        else:
-            logger.info(f"During force_binary, the column {t.name} is found to have != 2 unique values. Ignored.")
-    
-    if isinstance(df, pl.LazyFrame):
-        return df.blueprint.with_columns(exprs)
-    return df.with_columns(exprs)    
-
-def get_mapping_table(ordinal_mapping:dict[str, dict[str,int]]) -> pl.DataFrame:
-    '''
-        Helper function to get a table from an ordinal_mapping dict.
-
-        >>> {
-        >>> "a": 
-        >>>    {"a1": 1, "a2": 2,},
-        >>> "b":
-        >>>    {"b1": 3, "b2": 4,},
-        >>> }
-
-
-        Arguments:
-            ordinal_mapping: {name_of_feature: {value_1 : mapped_to_number_1, value_2 : mapped_to_number_2, ...}, ...}
-
-        Returns:
-            A table with feature name, value, and mapped_to
-    
-    '''
-    mapping_tables:list[pl.DataFrame] = []
-    for feature, mapping in ordinal_mapping.items():
-        table = pl.from_records(list(mapping.items()), schema=["value", "mapped_to"]).with_columns(
-            pl.lit(feature).alias("feature")
-        ).select("feature", "value", "mapped_to")
-        mapping_tables.append(table)
-
-    return pl.concat(mapping_tables)
-
-def ordinal_auto_encode(
-    df:PolarsFrame
-    , cols:Optional[list[str]]=None
-    , exclude:Optional[list[str]]=None
-) -> PolarsFrame:
-    '''
-        Automatically applies ordinal encoding to the provided columns by the following logic:
-            Sort the column, smallest value will be assigned to 0, second smallest will be assigned to 1...
-
-        This will automatically detect string columns and apply this operation if ordinal_cols is not provided. 
-        This method is great for string columns like age ranges, with values like ["10-20", "20-30"], etc...
-        
-        Arguments:
-            df:
-            default:
-            ordinal_cols:
-            exclude: the columns you wish to exclude in this transformation.
-        
-        Returns:
-            (encoded df, mapping table)
-    '''
-    if isinstance(cols, list):
-        types = check_columns_types(df, cols)
-        if types != "string":
-            raise TypeError(f"Ordinal encoding can only be used on string columns, not {types} types.")
-        ordinal_list = cols
-    else:
-        ordinal_list = get_string_cols(df, exclude=exclude)
-
-    temp = df.lazy().groupby(1).agg(
-        pl.col(c).unique().sort() for c in ordinal_list
-    ).select(ordinal_list)
-    for t in temp.collect().get_columns():
-        uniques:pl.Series = t[0]
-        mapping = {t.name: uniques, "to": list(range(len(uniques)))} 
-        if isinstance(df, pl.LazyFrame):
-            # Use a list here because Python cannot pickle a generator
-            df = df.blueprint.map_dict(t.name, mapping, "to", None)
-        else:
-            map_tb = pl.DataFrame(mapping)
-            df = df.join(map_tb, on = t.name).with_columns(
-                pl.col("to").alias(t.name)
-            ).drop("to")
-
-    return df
-
-def ordinal_encode(
-    df:PolarsFrame
-    , ordinal_mapping:dict[str, dict[str,int]]
-    , default:int|None=None
-) -> PolarsFrame:
-    '''
-        Ordinal encode the data with given mapping.
-
-        Notice that this function assumes that you already have the mapping, in correct mapping format.
-        since you have to supply the ordinal_mapping argument. If you still want the tabular output format,
-        please call get_ordinal_mapping_table with ordinal_mapping, which will create a table from this.
-
-        Arguments:
-            df:
-            ordinal_mapping:
-            default: if a value for a feature does not exist in ordinal_mapping, use default.
-
-        Returns:
-            encoded df
-    '''
-
-    for c in ordinal_mapping:
-        if c in df.columns:
-            mapping = ordinal_mapping[c]
-            if isinstance(df, pl.LazyFrame):
-                # This relies on the fact that dicts in Python is ordered
-                mapping = {c: mapping.keys(), "to": mapping.values()}
-                df = df.blueprint.map_dict(c, mapping, "to", default)
-            else:
-                mapping = pl.DataFrame((mapping.keys(), mapping.values()), schema=[c, "to"])
-                df = df.join(mapping, on = c, how="left").with_columns(
-                    pl.col("to").fill_null(default).alias(c)
-                ).drop("to")
-        else:
-            logger.warning(f"Found that column {c} is not in df. Skipped.")
-
-    return df
-
-def smooth_target_encode(
-    df:PolarsFrame
-    , target:str
-    , cols:list[str]
-    , min_samples_leaf:int
-    , smoothing:float
-    , check_binary:bool=True
-) -> PolarsFrame:
-    '''Smooth target encoding for binary classification. Currently only implemented for binary target.
-
-        See https://towardsdatascience.com/dealing-with-categorical-variables-by-using-target-encoder-a0f1733a4c69
-
-        Arguments:
-            df:
-            target:
-            cat_cols:
-            min_samples_leaf:
-            smoothing:
-            check_binary:
-    '''
-    if isinstance(cols, list):
-        types = check_columns_types(df, cols)
-        if types != "string":
-            raise ValueError(f"Target encoding can only be used on string columns, not {types} types.")
-        str_cols = cols
-    else:
-        str_cols = get_string_cols(df)
-    
-    # Only works for binary target for now. There is a non-binary ver of target encode, but I
-    # am just delaying the implementation...
-    if check_binary:
-        if not check_binary_target(df, target):
-            raise ValueError("Target is not binary or not properly encoded.")
-
-    # probability of target = 1
-    p = df.lazy().select(pl.col(target).mean()).collect().row(0)[0]
-    is_lazy = isinstance(df, pl.LazyFrame)
-    # If c has null, null will become a group when we group by.
-    for c in str_cols:
-        ref = df.groupby(c).agg(
-            pl.count().alias("cnt"),
-            pl.col(target).mean().alias("cond_p")
-        ).with_columns(
-            (1./(1. + ((-(pl.col("cnt").cast(pl.Float64) - min_samples_leaf))/smoothing).exp())).alias("alpha")
-        ).select(
-            pl.col(c).alias(c),
-            to = pl.col("alpha") * pl.col("cond_p") + (pl.lit(1) - pl.col("alpha")) * pl.lit(p)
-        ) # If df is lazy, ref is lazy. If df is eager, ref is eager
-        if is_lazy:
-            df = df.blueprint.map_dict(c, ref.collect().to_dict(), "to", None)
-        else: # It is ok to do inner join because all values of c are present in ref.
-            df = df.join(ref, on = c).with_columns(
-                pl.col("to").alias(c)
-            ).drop("to")
-    return df
-
-def woe_cat_encode(
-    df:PolarsFrame
-    , target:str
-    , cols:Optional[list[str]]=None
-    , min_count:float = 1.
-    , default: float = -10.
-    , check_binary:bool = True
-) -> PolarsFrame:
-    '''Performs WOE encoding for categorical features. Currently woe encoding is only available
-    for categorical (string) features. Numerical WOE encoding requires binning and the binning
-    transform is being considered (Need it to be comptible with blueprints and all that).
-
-        Arguments:
-            df: either a lazy or eager dataframe
-            target: target column
-            cols: string columns to be encoded. If none, it will use all from the df.
-            min_count: a regularization term that prevents ln(0).
-            default: default value for nulls resulted in the left-join.
-            check_binary: whether to check if target is binary or not
-
-        Returns:
-            an woe encoded lazy or eager Polars dataframe
-    '''
-    if isinstance(cols, list):
-        types = check_columns_types(df, cols)
-        if types != "string":
-            raise ValueError(f"woe_cat_encode encoding can only be used on string columns, not {types} types.")
-        str_cols = cols
-    else:
-        str_cols = get_string_cols(df)
-
-    if check_binary:
-        if not check_binary_target(df, target):
-            raise ValueError("Target is not binary or not properly encoded.")
-
-    is_lazy = isinstance(df, pl.LazyFrame)
-    for s in str_cols:
-        ref = df.lazy().groupby(s).agg(
-            ev = pl.col(target).sum()
-            , nonev = (pl.lit(1) - pl.col(target)).sum()
-        ).with_columns(
-            ev_rate = (pl.col("ev") + min_count)/(pl.col("ev").sum() + 2.0*min_count)
-            , nonev_rate = (pl.col("nonev") + min_count)/(pl.col("nonev").sum() + 2.0*min_count)
-        ).with_columns(
-            woe = (pl.col("ev_rate")/pl.col("nonev_rate")).log()
-        ).select(
-            pl.col(s)
-            , pl.col("woe")
-        ).collect()
-        if is_lazy:
-            df = df.blueprint.map_dict(s, ref.to_dict(), "woe", default)
-        else:
-            df = df.join(ref, on = s, how="left").with_columns(
-                pl.col("woe").fill_null(default).alias(s)
-            ).drop("woe")
-
-    return df
-
-def _lmax_estimate_step(df:PolarsFrame, c:str, s:PowerTransformStrategy) -> Tuple[str, float]:
-    np_col = df.lazy().select(pl.col(c).cast(pl.Float64)).collect().get_column(c).view()
-    if s in ("yeo_johnson", "yeojohnson"):
-        lmax:float = yeojohnson_normmax(np_col)
-    else:
-        lmax:float = boxcox_normmax(np_col, method="mle")
-    
-    return (c, lmax)
-
-def power_transform(
-    df: PolarsFrame
-    , cols: list[str]
-    , strategy: PowerTransformStrategy = "yeo_johnson"
-    , n_threads:int = CPU_COUNT
-    # , lmbda: Optional[float] = None
-) -> PolarsFrame:
-    '''Performs power transform on the numerical columns.
-
-        Arguments:
-            df: either a lazy or eager Polars dataframe
-            cols: a list of numerical columns to perform the transform.
-            strategy: either yeo_johnson or box_cox
-            n_threads: max number of threads you want to use. Default = CPU_COUNT
-
-        Returns:
-            the transformed lazy or eager dataframe
-    '''
-
-    types = check_columns_types(df, cols)
-    if types != "numeric":
-        raise ValueError(f"Power Transform can only be used on numeric columns, not {types} types.")
-    
-    s = clean_strategy_str(strategy)
-    exprs:list[pl.Expr] = []
-    # Ensure columns do not have missing values
-    exclude_columns_w_nulls = df.lazy().select(cols).null_count().collect().transpose(
-        include_header=True, column_names=["null_count"]
-    ).filter(pl.col("null_count") > 0).get_column("column").to_list()
-
-    if len(exclude_columns_w_nulls) > 0:
-        logger.info("The following columns will not be processed by power_transform because they contain missing "
-                    f"values. Please impute them.\n{exclude_columns_w_nulls}")
-        
-    non_null_list = [c for c in cols if c not in exclude_columns_w_nulls]
-    pbar = tqdm(non_null_list, desc = "Inferring best paramters")
-    if s in ("yeo_johnson", "yeojohnson"):
-        with ThreadPoolExecutor(max_workers=n_threads) as ex:
-            for future in as_completed(ex.submit(_lmax_estimate_step, df, c, s) for c in non_null_list):
-                c, lmax = future.result()
-                if lmax == 0: # log(x + 1)
-                    x_ge_0_sub_expr = (pl.col(c).add(1)).log()
-                else: # ((x + 1)**lmbda - 1) / lmbda
-                    x_ge_0_sub_expr = ((pl.col(c).add(1)).pow(lmax) - 1) / lmax
-
-                if lmax == 2: # -log(-x + 1)
-                    x_lt_0_sub_expr = pl.lit(-1) * (1 - pl.col(c)).log()
-                else: #  -((-x + 1)**(2 - lmbda) - 1) / (2 - lmbda)
-                    t = 2 - lmax
-                    x_lt_0_sub_expr = pl.lit(-1/t) * ((1 - pl.col(c)).pow(t) - 1)
-
-                exprs.append(
-                    pl.when(pl.col(c).ge(0)).then(x_ge_0_sub_expr).otherwise(x_lt_0_sub_expr).alias(c)
-                )
-                pbar.update(1)
-
-    elif s in ("box_cox", "boxcox"):
-        with ThreadPoolExecutor(max_workers=n_threads) as ex:
-            for future in as_completed(ex.submit(_lmax_estimate_step, df, c, s) for c in non_null_list):
-                c, lmax = future.result()
-                if lmax == 0: # log(x)
-                    exprs.append(pl.col(c).log())
-                else: # (x**lmbda - 1) / lmbda
-                    exprs.append(
-                        (pl.col(c).pow(lmax) - 1) / lmax
-                    )
-                pbar.update(1)
-    else:
-        raise TypeError(f"The input strategy {strategy} is not a valid strategy. Valid strategies are: yeo_johnson "
-                        "or box_cox")
-    pbar.close()
-    if isinstance(df, pl.LazyFrame):
-        return df.lazy().blueprint.with_columns(exprs)
-    return df.with_columns(exprs)
-
+from __future__ import annotations
+
+from .type_alias import (
+    PolarsFrame
+    , ImputationStrategy
+    , ScalingStrategy
+    , PowerTransformStrategy
+    , clean_strategy_str
+    , CPU_COUNT
+)
+from .prescreen import (
+    get_bool_cols
+    , get_string_cols
+    , get_unique_count
+    , check_binary_target
+    , check_columns_types
+)
+from .blueprint import( # Need this for Polars extension to work
+    Blueprint
+)
+import logging
+import numpy as np
+import polars as pl
+from typing import Optional, Tuple
+from scipy.stats._morestats import (
+    yeojohnson_normmax
+    , boxcox_normmax
+)
+from concurrent.futures import as_completed, ThreadPoolExecutor
+from tqdm import tqdm
+
+# Rewrite all docstrings using Polars' format.
+
+# A lot of companies are still using Python < 3.10
+# So I am not using match statements
+
+logger = logging.getLogger(__name__)
+
+def impute(
+    df:PolarsFrame
+    , cols:list[str]
+    , strategy:ImputationStrategy = 'median'
+    , const:float = 1.
+) -> PolarsFrame:
+    '''Imputes the given columns using the given strategy.
+
+        Arguments:
+            df: either a eager/lazy Polars dataframe
+            cols: cols to impute
+            strategy: one of 'mean', 'avg', 'average', 'median', 'const', 'constant', 'mode', 'most_frequent'. Some are 
+            just alternative names for the same strategy.
+            const: only uses this value if strategy = const
+
+        Returns:
+            the imputed lazy / eager dataframe.
+    '''
+    s = clean_strategy_str(strategy)
+    # Given Strategy, define expressions
+    if s == "median":
+        all_medians = df.lazy().select(cols).median().collect().row(0)
+        exprs = (pl.col(c).fill_null(all_medians[i]) for i,c in enumerate(cols))
+    elif s in ("mean", "avg", "average"):
+        all_means = df.lazy().select(cols).mean().collect().row(0)
+        exprs = (pl.col(c).fill_null(all_means[i]) for i,c in enumerate(cols))
+    elif s in ("const", "constant"):
+        exprs = (pl.col(c).fill_null(const) for c in cols)
+    elif s in ("mode", "most_frequent"):
+        all_modes = df.lazy().select(cols).select(pl.all().mode().first()).collect().row(0)
+        exprs = (pl.col(c).fill_null(all_modes[i]) for i,c in enumerate(cols))
+    else:
+        raise TypeError(f"Unknown imputation strategy: {strategy}")
+
+    # Need to cast to list so that pickle can work with it
+    # This is unfortunate because we will be looping over this list twice... Whatever...
+    if isinstance(df, pl.LazyFrame):
+        return df.blueprint.with_columns(exprs)
+    return df.with_columns(exprs)
+
+def scale(
+    df:PolarsFrame
+    , cols:list[str]
+    , strategy:ScalingStrategy="normal"
+    , const:float = 1.0
+) -> PolarsFrame:
+    '''
+    Scale given columns using the given strategy. Will skip null values.
+
+        Arguments:
+            df: either a lazy or eager dataframe
+            cols: list of columns to scale
+            strategy: one of 'normal', 'standard', 'normalize', 'min_max', 'const', 'constant',
+            where normal = standard = normalize.
+            const: only uses this value if strategy = const
+
+        Returns:
+            the scaled lazy / eager dataframe.
+    
+    '''
+    types = check_columns_types(df, cols)
+    if types != "numeric":
+        raise TypeError(f"Scaling can only be used on numeric columns, not {types} types.")
+
+    s = clean_strategy_str(strategy)
+    if s in ("normal", "standard", "normalize"):
+        mean_std = df.select(cols).lazy().select(
+            pl.all().mean().prefix("mean:")
+            , pl.all().std().prefix("std:")
+        ).collect().row(0)
+        exprs = ( (pl.col(c) - mean_std[i])/(mean_std[i + len(cols)]) for i,c in enumerate(cols) )
+    elif s == "min_max":
+        min_max = df.select(cols).lazy().select(
+            pl.all().min().prefix("min:"),
+            pl.all().max().prefix("max:")
+        ).collect().row(0) # All mins come first, then maxs
+        exprs = ( (pl.col(c) - min_max[i])/((min_max[i + len(cols)] - min_max[i])) for i,c in enumerate(cols) )
+    elif s in ("const", "constant"):
+        exprs = (pl.col(c)/const for c in cols)
+    else:
+        raise TypeError(f"Unknown scaling strategy: {strategy}")
+
+    if isinstance(df, pl.LazyFrame):
+        return df.blueprint.with_columns(exprs)
+    return df.with_columns(exprs)
+
+def boolean_transform(df:PolarsFrame, keep_null:bool=True) -> PolarsFrame:
+    '''Converts all boolean columns into binary columns.
+
+        Arguments:
+            df: either a lazy or eager Polars DataFrame
+            keep_null: if true, null will be kept. If false, null will be mapped to 0.
+
+        Returns:
+            a dataframe with booleans mapped to 0s and 1s.
+    '''
+    bool_cols = get_bool_cols(df)
+    if keep_null: # Directly cast. If null, then cast will also return null
+        exprs = (pl.col(c).cast(pl.UInt8) for c in bool_cols)
+    else: # Cast. Then fill null to 0s.
+        exprs = (pl.col(c).cast(pl.UInt8).fill_null(0) for c in bool_cols)
+
+    if isinstance(df, pl.LazyFrame):
+        return df.blueprint.with_columns(exprs)
+    return df.with_columns(exprs)
+
+def one_hot_encode(
+    df:PolarsFrame
+    , cols:Optional[list[str]]=None
+    , separator:str="_"
+    , drop_first:bool=False
+) -> PolarsFrame:
+    '''One hot encoding. The separator must be a single character.'''
+    
+    if isinstance(cols, list):
+        types = check_columns_types(df, cols)
+        if types != "string":
+            raise TypeError(f"One-hot encoding can only be used on string columns, not {types} types.")
+        str_cols = cols
+    else:
+        str_cols = get_string_cols(df)
+
+    if isinstance(df, pl.LazyFrame):
+        temp = df.lazy().select(str_cols).groupby(1).agg(
+            pl.all().unique().sort()
+        ).select(str_cols)
+        exprs:list[pl.Expr] = []
+        start_index = int(drop_first)
+        one = pl.lit(1, dtype=pl.UInt8) # Avoid casting 
+        zero = pl.lit(0, dtype=pl.UInt8) # Avoid casting
+        for t in temp.collect().get_columns():
+            u:pl.List = t[0] # t is a Series which contains a single series/list, so u is a series/list
+            if len(u) > 1:
+                exprs.extend(
+                    pl.when(pl.col(t.name) == u[i]).then(one).otherwise(zero).alias(t.name + separator + u[i])
+                    for i in range(start_index, len(u)) 
+                )
+            else:
+                logger.info(f"During one-hot-encoding, the column {t.name} is found to have 1 unique value. Dropped.")
+        
+        return df.blueprint.with_columns(exprs).blueprint.drop(str_cols)
+    else:
+        return df.to_dummies(columns=str_cols, separator=separator, drop_first=drop_first)
+    
+# def bin(df:PolarsFrame):
+    
+#     df.get_column("c").cut()
+
+# def fixed_sized_encode(df:pl.DataFrame, num_cols:list[str], bin_size:int=50) -> TransformationResult:
+#     '''Given a continuous variable, take the smallest `bin_size` of them, and call them bin 1, take the next
+#     smallest `bin_size` of them and call them bin 2, etc...
+    
+#     '''
+#     pass
+
+
+# REWRITE THIS
+# def percentile_encode(df:pl.DataFrame
+#     , cols:list[str]=None
+#     , exclude:list[str]=None
+# ) -> FitTransform:
+#     '''Bin your continuous variable X into X_percentiles. This will create at most 100 + 1 bins, 
+#         where each percentile could potentially be a bin and null will be mapped to bin = 0. 
+#         Bin 1 means percentile 0 to 1. Generally, bin X groups the population from bin X-1 to 
+#         bin X into one bucket.
+
+#         I see some potential optimization opportunities here.
+
+#         Arguments:
+#             df:
+#             num_cols: 
+#             exclude:
+
+#         Returns:
+#             (A transformed dataframe, a mapping table (value to percentile))
+    
+#     '''
+
+#     # Percentile Binning
+
+#     num_list:list[str] = []
+#     exclude_list:list[str] = [] if exclude is None else exclude
+#     if isinstance(cols, list):
+#         types = check_columns_types(df, cols)
+#         if types != "numeric":
+#             raise ValueError(f"Percentile encoding can only be used on numeric columns, not {types} types.")
+#         num_list.extend(cols)
+#     else:
+#         num_list.extend(get_numeric_cols(df, exclude=exclude_list))
+
+#     exprs:list[pl.Expr] = []
+#     all_mappings = []
+#     for c in num_list:
+#         percentile = df.groupby(c).agg(pl.count().alias("cnt"))\
+#             .sort(c)\
+#             .with_columns(
+#                 ((pl.col("cnt").cumsum()*100)/len(df)).ceil().alias("percentile")
+#             ).groupby("percentile")\
+#             .agg(
+#                 pl.col(c).min().alias("min"),
+#                 pl.col(c).max().alias("max"),
+#                 pl.col("cnt").sum().alias("cnt"),
+#             ).sort("percentile").select(
+#                 pl.lit(c).alias("feature"),
+#                 pl.col("percentile").cast(pl.UInt8),
+#                 "min",
+#                 "max",
+#                 "cnt",
+#             )
+        
+#         first_row = percentile.select("percentile","min", "max").to_numpy()[0, :] # First row
+#         # Need to handle an extreme case when percentile looks like 
+#         # percentile   min   max
+#         #  p1         null  null
+#         #  p2          ...   ...
+#         # This happens when there are so many nulls in the column.
+#         if np.isnan(first_row[2]):
+#             # Discard the first row if this is the case. 
+#             percentile = percentile.slice(1, length = None)
+
+#         # Only work on non null values. Null will be mapped to default value anyway.
+#         temp_df = df.lazy().filter(pl.col(c).is_not_null()).sort(c).set_sorted(c)\
+#             .join_asof(other=percentile.lazy().set_sorted("max"), left_on=c, right_on="max", strategy="forward")\
+#             .select(c, "percentile")\
+#             .unique().collect()
+        
+#         real_mapping = dict(zip(temp_df[c], temp_df["percentile"]))
+#         # a representation of the mapping, needed for recreating this.
+#         repr_mapping = dict(zip(percentile["max"], percentile["percentile"]))
+#         all_mappings.append(repr_mapping)
+#         exprs.append(
+#             pl.col(c).map_dict(real_mapping, default=0).cast(pl.UInt8)
+#         )
+
+#     res = df.with_columns(exprs)
+#     encoder_rec = EncoderRecord(features=num_list, strategy=EncodingStrategy.PERCENTILE, mappings=all_mappings)
+#     return FitTransform(transformed=res, mapping=encoder_rec)
+
+def binary_encode(
+    df:PolarsFrame
+    , cols:Optional[list[str]]=None
+    , exclude:Optional[list[str]]=None
+) -> PolarsFrame:
+    '''
+    Encode the given columns as binary values. Only handles string binary at this moment. This is equivalent
+    to using one-hot-encoding on binary columns using drop_first=True.
+
+        Arguments:
+            df:
+            binary_cols: the binary_cols you wish to convert. If no input, will infer.
+            exclude: the columns you wish to exclude in this transformation. 
+
+        Returns: 
+            (the transformed dataframe, mapping table between old values to [0,1])
+    '''
+
+    if cols is None:
+        str_cols = get_string_cols(df)
+        exclude = [] if exclude is None else exclude
+        binary_list = get_unique_count(df)\
+            .filter( # Binary + Not Exclude + Only String
+                (pl.col("n_unique") == 2) & (~pl.col("column").is_in(exclude)) & (pl.col("column").is_in(str_cols))
+            ).get_column("column").to_list()
+
+    else: # No need to do all that type checking steps because we are gonna do that in one-hot anyways
+        binary_list = cols
+    
+    return one_hot_encode(df, cols=binary_list, drop_first=True)
+
+def force_binary(
+    df:PolarsFrame
+    , cols:Optional[list[str]]=None
+):
+    '''
+    Force every binary column, no matter what data type, to be turned into 0s and 1s by the order of the elements. If a 
+    column has two unique values like [null, "haha"], then null will be mapped to 0 and "haha" to 1.
+    '''
+    if cols is None:
+        binary_list = get_unique_count(df)\
+            .filter(pl.col("n_unique") == 2)\
+            .get_column("column").to_list()
+    else:
+        binary_list = cols
+
+    temp = df.lazy().select(binary_list).groupby(1).agg(
+            pl.all().unique().sort()
+        ).select(binary_list) # Need this to get rid of the literal 1 column
+    exprs:list[pl.Expr] = []
+    one = pl.lit(1, dtype=pl.UInt8) # Avoid casting 
+    zero = pl.lit(0, dtype=pl.UInt8) # Avoid casting
+    for t in temp.collect().get_columns():
+        u:pl.List = t[0] # t is a Series which contains a single list which contains the 2 unique values 
+        if len(u) == 2:
+            exprs.append(
+                pl.when(pl.col(t.name) == u[0]).then(zero).otherwise(one).alias(t.name)
+            )
+        else:
+            logger.info(f"During force_binary, the column {t.name} is found to have != 2 unique values. Ignored.")
+    
+    if isinstance(df, pl.LazyFrame):
+        return df.blueprint.with_columns(exprs)
+    return df.with_columns(exprs)    
+
+def get_mapping_table(ordinal_mapping:dict[str, dict[str,int]]) -> pl.DataFrame:
+    '''
+        Helper function to get a table from an ordinal_mapping dict.
+
+        >>> {
+        >>> "a": 
+        >>>    {"a1": 1, "a2": 2,},
+        >>> "b":
+        >>>    {"b1": 3, "b2": 4,},
+        >>> }
+
+
+        Arguments:
+            ordinal_mapping: {name_of_feature: {value_1 : mapped_to_number_1, value_2 : mapped_to_number_2, ...}, ...}
+
+        Returns:
+            A table with feature name, value, and mapped_to
+    
+    '''
+    mapping_tables:list[pl.DataFrame] = []
+    for feature, mapping in ordinal_mapping.items():
+        table = pl.from_records(list(mapping.items()), schema=["value", "mapped_to"]).with_columns(
+            pl.lit(feature).alias("feature")
+        ).select("feature", "value", "mapped_to")
+        mapping_tables.append(table)
+
+    return pl.concat(mapping_tables)
+
+def ordinal_auto_encode(
+    df:PolarsFrame
+    , cols:Optional[list[str]]=None
+    , descending:bool = False
+    , exclude:Optional[list[str]]=None
+) -> PolarsFrame:
+    '''
+        Automatically applies ordinal encoding to the provided columns by the following logic:
+            Sort the column, smallest value will be assigned to 0, second smallest will be assigned to 1...
+
+        This will automatically detect string columns and apply this operation if ordinal_cols is not provided. 
+        This method is great for string columns like age ranges, with values like ["10-20", "20-30"], etc...
+        
+        Arguments:
+            df:
+            default:
+            cols:
+            exclude: the columns you wish to exclude in this transformation.
+        
+        Returns:
+            (encoded df, mapping table)
+    '''
+    if isinstance(cols, list):
+        types = check_columns_types(df, cols)
+        if types != "string":
+            raise TypeError(f"Ordinal encoding can only be used on string columns, not {types} types.")
+        ordinal_list = cols
+    else:
+        ordinal_list = get_string_cols(df, exclude=exclude)
+
+    temp = df.lazy().groupby(1).agg(
+        pl.col(c).unique().sort(descending=descending) for c in ordinal_list
+    ).select(ordinal_list)
+    for t in temp.collect().get_columns():
+        uniques:pl.Series = t[0]
+        mapping = {t.name: uniques, "to": list(range(len(uniques)))} 
+        if isinstance(df, pl.LazyFrame):
+            # Use a list here because Python cannot pickle a generator
+            df = df.blueprint.map_dict(t.name, mapping, "to", None)
+        else:
+            map_tb = pl.DataFrame(mapping)
+            df = df.join(map_tb, on = t.name).with_columns(
+                pl.col("to").alias(t.name)
+            ).drop("to")
+
+    return df
+
+def ordinal_encode(
+    df:PolarsFrame
+    , ordinal_mapping:dict[str, dict[str,int]]
+    , default:int|None=None
+) -> PolarsFrame:
+    '''
+        Ordinal encode the data with given mapping.
+
+        Notice that this function assumes that you already have the mapping, in correct mapping format.
+        since you have to supply the ordinal_mapping argument. If you still want the tabular output format,
+        please call get_ordinal_mapping_table with ordinal_mapping, which will create a table from this.
+
+        Arguments:
+            df:
+            ordinal_mapping:
+            default: if a value for a feature does not exist in ordinal_mapping, use default.
+
+        Returns:
+            encoded df
+    '''
+
+    for c in ordinal_mapping:
+        if c in df.columns:
+            mapping = ordinal_mapping[c]
+            if isinstance(df, pl.LazyFrame):
+                # This relies on the fact that dicts in Python is ordered
+                mapping = {c: mapping.keys(), "to": mapping.values()}
+                df = df.blueprint.map_dict(c, mapping, "to", default)
+            else:
+                mapping = pl.DataFrame((mapping.keys(), mapping.values()), schema=[c, "to"])
+                df = df.join(mapping, on = c, how="left").with_columns(
+                    pl.col("to").fill_null(default).alias(c)
+                ).drop("to")
+        else:
+            logger.warning(f"Found that column {c} is not in df. Skipped.")
+
+    return df
+
+def smooth_target_encode(
+    df:PolarsFrame
+    , target:str
+    , cols:list[str]
+    , min_samples_leaf:int
+    , smoothing:float
+    , check_binary:bool=True
+) -> PolarsFrame:
+    '''Smooth target encoding for binary classification. Currently only implemented for binary target.
+
+        See https://towardsdatascience.com/dealing-with-categorical-variables-by-using-target-encoder-a0f1733a4c69
+
+        Arguments:
+            df:
+            target:
+            cat_cols:
+            min_samples_leaf:
+            smoothing:
+            check_binary:
+    '''
+    if isinstance(cols, list):
+        types = check_columns_types(df, cols)
+        if types != "string":
+            raise ValueError(f"Target encoding can only be used on string columns, not {types} types.")
+        str_cols = cols
+    else:
+        str_cols = get_string_cols(df)
+    
+    # Only works for binary target for now. There is a non-binary ver of target encode, but I
+    # am just delaying the implementation...
+    if check_binary:
+        if not check_binary_target(df, target):
+            raise ValueError("Target is not binary or not properly encoded.")
+
+    # probability of target = 1
+    p = df.lazy().select(pl.col(target).mean()).collect().row(0)[0]
+    is_lazy = isinstance(df, pl.LazyFrame)
+    # If c has null, null will become a group when we group by.
+    for c in str_cols:
+        ref = df.groupby(c).agg(
+            pl.count().alias("cnt"),
+            pl.col(target).mean().alias("cond_p")
+        ).with_columns(
+            (1./(1. + ((-(pl.col("cnt").cast(pl.Float64) - min_samples_leaf))/smoothing).exp())).alias("alpha")
+        ).select(
+            pl.col(c).alias(c),
+            to = pl.col("alpha") * pl.col("cond_p") + (pl.lit(1) - pl.col("alpha")) * pl.lit(p)
+        ) # If df is lazy, ref is lazy. If df is eager, ref is eager
+        if is_lazy:
+            df = df.blueprint.map_dict(c, ref.collect().to_dict(), "to", None)
+        else: # It is ok to do inner join because all values of c are present in ref.
+            df = df.join(ref, on = c).with_columns(
+                pl.col("to").alias(c)
+            ).drop("to")
+    return df
+
+def custom_binning(
+    df:PolarsFrame
+    , cols:list[str]
+    , cuts:list[float]
+) -> PolarsFrame:
+    '''
+    Bins according to the cuts provided.
+    '''
+
+    if isinstance(df, pl.LazyFrame):
+        exprs = [
+            pl.col(c).cut(cuts).cast(pl.Utf8) for c in cols
+        ]
+        return df.blueprint.with_columns(exprs)
+    else:
+        return df.with_columns(
+            pl.col(c).cut(cuts).cast(pl.Utf8) for c in cols
+        )
+
+def quantile_binning(
+    df:PolarsFrame
+    , cols:list[str]
+    , n_bins:int
+) -> PolarsFrame:
+    '''
+    Bin a continuous variable into categories, based on quantile. Null values will be its own category.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars dataframe
+    cols
+        A list of numeric columns. This has to be supplied by the user because it is not recommended
+        to bin all numerical variables
+    n_bins
+        The number of desired bins. If n_bins = 4, the quantile cuts will be [0.25,0.5,0.74], and 4 
+        categories will be created, which represent values ranging from (-inf, 0.25 quantile value],
+        (0.25 quantile value, 0.5 quantile value],...(0.75 quantile value, inf]
+    
+    Returns
+    -------
+        A lazy or eager frame with the columns binned.
+
+    Example
+    -------
+    >>> df = pl.DataFrame({
+    ...     "a":range(5)
+    ... })
+    >>> df
+    shape: (5, 1)
+    ┌─────┐
+    │ a   │
+    │ --- │
+    │ i64 │
+    ╞═════╡
+    │ 0   │
+    │ 1   │
+    │ 2   │
+    │ 3   │
+    │ 4   │
+    └─────┘
+    >>> quantile_binning(df, cols=["a"], n_bins=4)
+    shape: (5, 1)
+    ┌───────────┐
+    │ a         │
+    │ ---       │
+    │ str       │
+    ╞═══════════╡
+    │ (-inf, 1] │
+    │ (-inf, 1] │
+    │ (1, 2]    │
+    │ (2, 3]    │
+    │ (3, inf]  │
+    └───────────┘
+    '''
+    types = check_columns_types(df, cols)
+    if types != "numeric":
+        raise ValueError(f"Quantile binning can only be used on numeric columns, not {types} types.")
+    
+    qcuts = np.arange(start=1/n_bins, stop=1.0, step = 1/n_bins)
+    if isinstance(df, pl.LazyFrame):
+        cuts = df.select(cols).select(
+            pl.all().qcut(qcuts).unique().cast(pl.Utf8).str.extract(r"\((.*?),")
+            .cast(pl.Float64).sort().tail(len(qcuts))
+        ).collect()
+        # For some reasons a generator here doesn't work. Use list instead
+        exprs = [
+            pl.col(c).cut(cuts.drop_in_place(c).to_list()).cast(pl.Utf8) for c in cols
+        ]
+        return df.blueprint.with_columns(exprs)
+    else: # Eager frame
+        return df.with_columns(
+            pl.col(c).qcut(qcuts).cast(pl.Utf8) for c in cols 
+        )
+
+def woe_cat_encode(
+    df:PolarsFrame
+    , target:str
+    , cols:Optional[list[str]]=None
+    , min_count:float = 1.
+    , default: float = -10.
+    , check_binary:bool = True
+) -> PolarsFrame:
+    '''Performs WOE encoding for categorical features. Currently woe encoding is only available
+    for categorical (string) features. Numerical WOE encoding requires binning and the binning
+    transform is being considered (Need it to be comptible with blueprints and all that).
+
+        Arguments:
+            df: either a lazy or eager dataframe
+            target: target column
+            cols: string columns to be encoded. If none, it will use all from the df.
+            min_count: a regularization term that prevents ln(0).
+            default: default value for nulls resulted in the left-join.
+            check_binary: whether to check if target is binary or not
+
+        Returns:
+            an woe encoded lazy or eager Polars dataframe
+    '''
+    if isinstance(cols, list):
+        types = check_columns_types(df, cols)
+        if types != "string":
+            raise ValueError(f"woe_cat_encode encoding can only be used on string columns, not {types} types.")
+        str_cols = cols
+    else:
+        str_cols = get_string_cols(df)
+
+    if check_binary:
+        if not check_binary_target(df, target):
+            raise ValueError("Target is not binary or not properly encoded.")
+
+    is_lazy = isinstance(df, pl.LazyFrame)
+    for s in str_cols:
+        ref = df.lazy().groupby(s).agg(
+            ev = pl.col(target).sum()
+            , nonev = (pl.lit(1) - pl.col(target)).sum()
+        ).with_columns(
+            ev_rate = (pl.col("ev") + min_count)/(pl.col("ev").sum() + 2.0*min_count)
+            , nonev_rate = (pl.col("nonev") + min_count)/(pl.col("nonev").sum() + 2.0*min_count)
+        ).with_columns(
+            woe = (pl.col("ev_rate")/pl.col("nonev_rate")).log()
+        ).select(
+            pl.col(s)
+            , pl.col("woe")
+        ).collect()
+        if is_lazy:
+            df = df.blueprint.map_dict(s, ref.to_dict(), "woe", default)
+        else:
+            df = df.join(ref, on = s, how="left").with_columns(
+                pl.col("woe").fill_null(default).alias(s)
+            ).drop("woe")
+
+    return df
+
+def _lmax_estimate_step(df:PolarsFrame, c:str, s:PowerTransformStrategy) -> Tuple[str, float]:
+    np_col = df.lazy().select(pl.col(c).cast(pl.Float64)).collect().get_column(c).view()
+    if s in ("yeo_johnson", "yeojohnson"):
+        lmax:float = yeojohnson_normmax(np_col)
+    else:
+        lmax:float = boxcox_normmax(np_col, method="mle")
+    
+    return (c, lmax)
+
+def power_transform(
+    df: PolarsFrame
+    , cols: list[str]
+    , strategy: PowerTransformStrategy = "yeo_johnson"
+    , n_threads:int = CPU_COUNT
+    # , lmbda: Optional[float] = None
+) -> PolarsFrame:
+    '''Performs power transform on the numerical columns.
+
+        Arguments:
+            df: either a lazy or eager Polars dataframe
+            cols: a list of numerical columns to perform the transform.
+            strategy: either yeo_johnson or box_cox
+            n_threads: max number of threads you want to use. Default = CPU_COUNT
+
+        Returns:
+            the transformed lazy or eager dataframe
+    '''
+
+    types = check_columns_types(df, cols)
+    if types != "numeric":
+        raise ValueError(f"Power Transform can only be used on numeric columns, not {types} types.")
+    
+    s = clean_strategy_str(strategy)
+    exprs:list[pl.Expr] = []
+    # Ensure columns do not have missing values
+    exclude_columns_w_nulls = df.lazy().select(cols).null_count().collect().transpose(
+        include_header=True, column_names=["null_count"]
+    ).filter(pl.col("null_count") > 0).get_column("column").to_list()
+
+    if len(exclude_columns_w_nulls) > 0:
+        logger.info("The following columns will not be processed by power_transform because they contain missing "
+                    f"values. Please impute them.\n{exclude_columns_w_nulls}")
+        
+    non_null_list = [c for c in cols if c not in exclude_columns_w_nulls]
+    pbar = tqdm(non_null_list, desc = "Inferring best paramters")
+    if s in ("yeo_johnson", "yeojohnson"):
+        with ThreadPoolExecutor(max_workers=n_threads) as ex:
+            for future in as_completed(ex.submit(_lmax_estimate_step, df, c, s) for c in non_null_list):
+                c, lmax = future.result()
+                if lmax == 0: # log(x + 1)
+                    x_ge_0_sub_expr = (pl.col(c).add(1)).log()
+                else: # ((x + 1)**lmbda - 1) / lmbda
+                    x_ge_0_sub_expr = ((pl.col(c).add(1)).pow(lmax) - 1) / lmax
+
+                if lmax == 2: # -log(-x + 1)
+                    x_lt_0_sub_expr = pl.lit(-1) * (1 - pl.col(c)).log()
+                else: #  -((-x + 1)**(2 - lmbda) - 1) / (2 - lmbda)
+                    t = 2 - lmax
+                    x_lt_0_sub_expr = pl.lit(-1/t) * ((1 - pl.col(c)).pow(t) - 1)
+
+                exprs.append(
+                    pl.when(pl.col(c).ge(0)).then(x_ge_0_sub_expr).otherwise(x_lt_0_sub_expr).alias(c)
+                )
+                pbar.update(1)
+
+    elif s in ("box_cox", "boxcox"):
+        with ThreadPoolExecutor(max_workers=n_threads) as ex:
+            for future in as_completed(ex.submit(_lmax_estimate_step, df, c, s) for c in non_null_list):
+                c, lmax = future.result()
+                if lmax == 0: # log(x)
+                    exprs.append(pl.col(c).log())
+                else: # (x**lmbda - 1) / lmbda
+                    exprs.append(
+                        (pl.col(c).pow(lmax) - 1) / lmax
+                    )
+                pbar.update(1)
+    else:
+        raise TypeError(f"The input strategy {strategy} is not a valid strategy. Valid strategies are: yeo_johnson "
+                        "or box_cox")
+    pbar.close()
+    if isinstance(df, pl.LazyFrame):
+        return df.lazy().blueprint.with_columns(exprs)
+    return df.with_columns(exprs)
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dsds-0.0.16/src/dsds/type_alias.py` & `dsds-0.0.17/src/dsds/type_alias.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,34 @@
-from typing import TypeAlias, Literal, Final, Tuple
-import polars as pl
-import os
-
-CPU_COUNT:Final[int] = os.cpu_count()
-POLARS_NUMERICAL_TYPES:Final[Tuple[pl.DataType]] = (pl.UInt8, pl.UInt16, pl.UInt32, pl.UInt64, pl.Float32, pl.Float64, pl.Int8, pl.Int16, pl.Int32, pl.Int64)  # noqa: E501
-POLARS_DATETIME_TYPES:Final[Tuple[pl.DataType]] = (pl.Datetime, pl.Date, pl.Time)
-
-PolarsFrame:TypeAlias = pl.DataFrame | pl.LazyFrame
-StepName = Literal["with_column", "map_dict", "drop", "select"]
-MRMRStrategy = Literal["fscore", "f", "f_score", "xgb", "xgboost", "rf", "random_forest", "mis"
-                       , "mutual_info_score", "lgbm", "lightgbm"]
-ScalingStrategy = Literal["normal", "standard", "normalize", "min_max", "const", "constant"]
-ImputationStrategy = Literal["mean", "avg", "average", "median", "const", "constant", "mode", "most_frequent"]
-PowerTransformStrategy = Literal["yeo_johnson", "yeojohnson", "box_cox", "boxcox"]
-KSAlternatives = Literal["two-sided", "greater", "less"]
-
-BinaryModels = Literal["logistic", "lr", "lightgbm", "lgbm", "xgboost", "xgb", "random_forest", "rf"]
-# This is just a subset of Scipy.stats's distributions which can be named by strings. All scipy.stats's string-name-able
-# distributions should work when the arguments asks for a CommonContinuousDist.
-CommonContinuousDist = Literal["norm", "lognorm", "truncnorm", "uniform", "t", "beta", "cauchy", "expon", "gamma"]
-def clean_strategy_str(s:str):
-    '''Strategy strings will only have _, no -, and all lowercase.'''
+from typing import (
+    TypeAlias
+    , Literal
+    , Final
+    , Tuple
+    , Callable
+    , Concatenate
+    , ParamSpec
+)
+import polars as pl
+import os
+
+P = ParamSpec('P')
+CPU_COUNT:Final[int] = os.cpu_count()
+POLARS_NUMERICAL_TYPES:Final[Tuple[pl.DataType]] = (pl.UInt8, pl.UInt16, pl.UInt32, pl.UInt64, pl.Float32, pl.Float64, pl.Int8, pl.Int16, pl.Int32, pl.Int64)  # noqa: E501
+POLARS_DATETIME_TYPES:Final[Tuple[pl.DataType]] = (pl.Datetime, pl.Date, pl.Time)
+
+PolarsFrame:TypeAlias = pl.DataFrame | pl.LazyFrame
+PipeFunction = Callable[Concatenate[PolarsFrame, P], PolarsFrame]
+ActionType = Literal["with_column", "map_dict", "drop", "select"] # "apply_func"
+MRMRStrategy = Literal["fscore", "f", "f_score", "xgb", "xgboost", "rf", "random_forest", "mis"
+                       , "mutual_info_score", "lgbm", "lightgbm"]
+ScalingStrategy = Literal["normal", "standard", "normalize", "min_max", "const", "constant"]
+ImputationStrategy = Literal["mean", "avg", "average", "median", "const", "constant", "mode", "most_frequent"]
+PowerTransformStrategy = Literal["yeo_johnson", "yeojohnson", "box_cox", "boxcox"]
+KSAlternatives = Literal["two-sided", "greater", "less"]
+
+BinaryModels = Literal["logistic", "lr", "lightgbm", "lgbm", "xgboost", "xgb", "random_forest", "rf"]
+# This is just a subset of Scipy.stats's distributions which can be named by strings. All scipy.stats's string-name-able
+# distributions should work when the arguments asks for a CommonContinuousDist.
+CommonContinuousDist = Literal["norm", "lognorm", "truncnorm", "uniform", "t", "beta", "cauchy", "expon", "gamma"]
+def clean_strategy_str(s:str):
+    '''Strategy strings will only have _, no -, and all lowercase.'''
     return s.strip().replace("-", "_").lower()
```

