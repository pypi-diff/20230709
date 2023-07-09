# Comparing `tmp/cev-0.1.0.tar.gz` & `tmp/cev-0.1.1.tar.gz`

## Comparing `cev-0.1.0.tar` & `cev-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 cev-0.1.0/.editorconfig
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 cev-0.1.0/.gitattributes
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 cev-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 cev-0.1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     9760 2020-02-02 00:00:00.000000 cev-0.1.0/notebooks/abundance-analysis.ipynb
--rw-r--r--   0        0        0     9044 2020-02-02 00:00:00.000000 cev-0.1.0/notebooks/getting-started.ipynb
--rw-r--r--   0        0        0     9042 2020-02-02 00:00:00.000000 cev-0.1.0/notebooks/lui-2021.ipynb
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 cev-0.1.0/cev/__init__.py
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 cev-0.1.0/cev/_compare.py
--rw-r--r--   0        0        0     5962 2020-02-02 00:00:00.000000 cev-0.1.0/cev/_compare_metric_dropdown.py
--rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 cev-0.1.0/cev/_compare_selection_type_dropdown.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 cev-0.1.0/cev/_compare_zoom_toggle.py
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 cev-0.1.0/cev/_embedding.py
--rw-r--r--   0        0        0     7069 2020-02-02 00:00:00.000000 cev-0.1.0/cev/_embedding_comparison_widget.py
--rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 cev-0.1.0/cev/_embedding_widget.py
--rw-r--r--   0        0        0     8661 2020-02-02 00:00:00.000000 cev-0.1.0/cev/_widget_utils.py
--rw-r--r--   0        0        0     9051 2020-02-02 00:00:00.000000 cev-0.1.0/cev/metrics.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 cev-0.1.0/cev/widgets.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 cev-0.1.0/cev/components/__init__.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 cev-0.1.0/cev/components/_html_widget.py
--rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 cev-0.1.0/cev/components/_marker_composition_logo.py
--rw-r--r--   0        0        0     7725 2020-02-02 00:00:00.000000 cev-0.1.0/cev/components/_marker_selection_indicator.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 cev-0.1.0/cev/components/_width_optimizer.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 cev-0.1.0/tests/test_cev.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 cev-0.1.0/tests/test_widget_utils.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 cev-0.1.0/.gitignore
--rw-r--r--   0        0        0    11349 2020-02-02 00:00:00.000000 cev-0.1.0/LICENSE
--rw-r--r--   0        0        0     4671 2020-02-02 00:00:00.000000 cev-0.1.0/README.md
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 cev-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 cev-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 cev-0.1.1/.editorconfig
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 cev-0.1.1/.gitattributes
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 cev-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 cev-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 cev-0.1.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     9760 2020-02-02 00:00:00.000000 cev-0.1.1/notebooks/abundance-analysis.ipynb
+-rw-r--r--   0        0        0     9044 2020-02-02 00:00:00.000000 cev-0.1.1/notebooks/getting-started.ipynb
+-rw-r--r--   0        0        0     9042 2020-02-02 00:00:00.000000 cev-0.1.1/notebooks/lui-2021.ipynb
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 cev-0.1.1/cev/__init__.py
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 cev-0.1.1/cev/_compare.py
+-rw-r--r--   0        0        0     5962 2020-02-02 00:00:00.000000 cev-0.1.1/cev/_compare_metric_dropdown.py
+-rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 cev-0.1.1/cev/_compare_selection_type_dropdown.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 cev-0.1.1/cev/_compare_zoom_toggle.py
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 cev-0.1.1/cev/_embedding.py
+-rw-r--r--   0        0        0     7069 2020-02-02 00:00:00.000000 cev-0.1.1/cev/_embedding_comparison_widget.py
+-rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 cev-0.1.1/cev/_embedding_widget.py
+-rw-r--r--   0        0        0     8661 2020-02-02 00:00:00.000000 cev-0.1.1/cev/_widget_utils.py
+-rw-r--r--   0        0        0     9051 2020-02-02 00:00:00.000000 cev-0.1.1/cev/metrics.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 cev-0.1.1/cev/widgets.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 cev-0.1.1/cev/components/__init__.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 cev-0.1.1/cev/components/_html_widget.py
+-rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 cev-0.1.1/cev/components/_marker_composition_logo.py
+-rw-r--r--   0        0        0     7725 2020-02-02 00:00:00.000000 cev-0.1.1/cev/components/_marker_selection_indicator.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 cev-0.1.1/cev/components/_width_optimizer.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 cev-0.1.1/tests/test_cev.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 cev-0.1.1/tests/test_widget_utils.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 cev-0.1.1/.gitignore
+-rw-r--r--   0        0        0    11349 2020-02-02 00:00:00.000000 cev-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 cev-0.1.1/README.md
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 cev-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6160 2020-02-02 00:00:00.000000 cev-0.1.1/PKG-INFO
```

### Comparing `cev-0.1.0/.pre-commit-config.yaml` & `cev-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cev-0.1.0/.github/workflows/ci.yml` & `cev-0.1.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `cev-0.1.0/notebooks/abundance-analysis.ipynb` & `cev-0.1.1/notebooks/abundance-analysis.ipynb`

 * *Files identical despite different names*

### Comparing `cev-0.1.0/notebooks/getting-started.ipynb` & `cev-0.1.1/notebooks/getting-started.ipynb`

 * *Files identical despite different names*

### Comparing `cev-0.1.0/notebooks/lui-2021.ipynb` & `cev-0.1.1/notebooks/lui-2021.ipynb`

 * *Files identical despite different names*

### Comparing `cev-0.1.0/cev/_compare.py` & `cev-0.1.1/cev/_compare.py`

 * *Files identical despite different names*

### Comparing `cev-0.1.0/cev/_compare_metric_dropdown.py` & `cev-0.1.1/cev/_compare_metric_dropdown.py`

 * *Files identical despite different names*

### Comparing `cev-0.1.0/cev/_compare_selection_type_dropdown.py` & `cev-0.1.1/cev/_compare_selection_type_dropdown.py`

 * *Files identical despite different names*

### Comparing `cev-0.1.0/cev/_compare_zoom_toggle.py` & `cev-0.1.1/cev/_compare_zoom_toggle.py`

 * *Files identical despite different names*

### Comparing `cev-0.1.0/cev/_embedding.py` & `cev-0.1.1/cev/_embedding.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,18 +29,18 @@
         )
 
     @classmethod
     def from_ozette(cls, df: pd.DataFrame, **kwargs):
         coords, labels, robust = _prepare_ozette(df, **kwargs)
         return cls(coords=coords, labels=labels, robust=robust)
 
-    def widgets(self):
+    def widgets(self, **kwargs):
         from ._embedding_widget import EmbeddingWidgetCollection
 
-        return EmbeddingWidgetCollection.from_embedding(self)
+        return EmbeddingWidgetCollection.from_embedding(self, **kwargs)
 
 
 def _prepare_ozette(df: pd.DataFrame, robust_only: bool = True):
     # ISMB data
     if "cellType" in df.columns:
         robust = (df["cellType"] != NON_ROBUST_LABEL).to_numpy()
         if robust_only:
```

### Comparing `cev-0.1.0/cev/_embedding_comparison_widget.py` & `cev-0.1.1/cev/_embedding_comparison_widget.py`

 * *Files identical despite different names*

### Comparing `cev-0.1.0/cev/_embedding_widget.py` & `cev-0.1.1/cev/_embedding_widget.py`

 * *Files identical despite different names*

### Comparing `cev-0.1.0/cev/_widget_utils.py` & `cev-0.1.1/cev/_widget_utils.py`

 * *Files identical despite different names*

### Comparing `cev-0.1.0/cev/metrics.py` & `cev-0.1.1/cev/metrics.py`

 * *Files identical despite different names*

### Comparing `cev-0.1.0/cev/components/_html_widget.py` & `cev-0.1.1/cev/components/_html_widget.py`

 * *Files identical despite different names*

### Comparing `cev-0.1.0/cev/components/_marker_composition_logo.py` & `cev-0.1.1/cev/components/_marker_composition_logo.py`

 * *Files identical despite different names*

### Comparing `cev-0.1.0/cev/components/_marker_selection_indicator.py` & `cev-0.1.1/cev/components/_marker_selection_indicator.py`

 * *Files identical despite different names*

### Comparing `cev-0.1.0/tests/test_widget_utils.py` & `cev-0.1.1/tests/test_widget_utils.py`

 * *Files identical despite different names*

### Comparing `cev-0.1.0/LICENSE` & `cev-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cev-0.1.0/README.md` & `cev-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -57,14 +57,18 @@
     selection="synced",
     auto_zoom=True,
     row_height=320,
 )
 umap_vs_ozette
 ```
 
+<img width="1269" alt="User interface of cev's comparison widget" src="https://github.com/OzetteTech/comparative-embedding-visualization/assets/84813279/db28944b-fa36-475c-b3b9-efd07272e1b9">
+
+
+
 See [notebooks/getting-started.ipynb](notebooks/getting-started.ipynb) for the complete example.
 
 ## Development
 
 First, create a virtual environment with all the required dependencies. We highly recommend to use [`hatch`](https://github.com/pypa/hatch), which installs and sync all dependencies from `pyproject.toml` automatically.
 
 ```sh
@@ -93,14 +97,15 @@
 ### Commands Cheatsheet
 
 If using `hatch` CLI, the following commands are available in the default environment:
 
 | Command                | Action                                                              |
 | :--------------------- | :------------------------------------------------------------------ |
 | `hatch run fix`        | Format project with `black .` and apply linting with `ruff --fix .` |
+| `hatch run fmt`        | Format project with `black .` and apply linting with `ruff --fix .` |
 | `hatch run check`      | Check formatting and linting with `black --check .` and `ruff .`.   |
 | `hatch run test`       | Run unittests with `pytest` in base environment.                    |
 | `hatch run test:test`  | Run unittests with `pytest` in all supported environments.          |
 
 Alternatively, you can devlop **cev** by manually creating a virtual environment and managing
 dependencies with `pip`.
```

### Comparing `cev-0.1.0/pyproject.toml` & `cev-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -13,23 +13,24 @@
 ]
 classifiers = [
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 requires-python = ">=3.8"
 dependencies = [
     "anywidget>=0.2.3",
     "cev-metrics>=0.1.2",
     "ipywidgets>=8.0.0",
     "jinja2>=3.0.0",
     "jupyter-scatter>=0.12.2",
-    "pandas>=1.0,<2.0",
+    "pandas>=1.0",
 ]
 dynamic = ["version"]
 
 # https://peps.python.org/pep-0621/#dependencies-optional-dependencies
 [project.optional-dependencies]
 dev = [
     "black[jupyter]",
```

### Comparing `cev-0.1.0/PKG-INFO` & `cev-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: cev
-Version: 0.1.0
+Version: 0.1.1
 Summary: comparative embedding visualization
 Project-URL: homepage, https://github.com/OzetteTech/comparative-embedding-visualization
 Author: Trevor Manz, Fritz Lekschas
 License: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Requires-Dist: anywidget>=0.2.3
 Requires-Dist: cev-metrics>=0.1.2
 Requires-Dist: ipywidgets>=8.0.0
 Requires-Dist: jinja2>=3.0.0
 Requires-Dist: jupyter-scatter>=0.12.2
-Requires-Dist: pandas<2.0,>=1.0
+Requires-Dist: pandas>=1.0
 Provides-Extra: dev
 Requires-Dist: black[jupyter]; extra == 'dev'
 Requires-Dist: jupyterlab; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: rich; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
 Provides-Extra: notebooks
@@ -89,14 +90,18 @@
     selection="synced",
     auto_zoom=True,
     row_height=320,
 )
 umap_vs_ozette
 ```
 
+<img width="1269" alt="User interface of cev's comparison widget" src="https://github.com/OzetteTech/comparative-embedding-visualization/assets/84813279/db28944b-fa36-475c-b3b9-efd07272e1b9">
+
+
+
 See [notebooks/getting-started.ipynb](notebooks/getting-started.ipynb) for the complete example.
 
 ## Development
 
 First, create a virtual environment with all the required dependencies. We highly recommend to use [`hatch`](https://github.com/pypa/hatch), which installs and sync all dependencies from `pyproject.toml` automatically.
 
 ```sh
@@ -125,14 +130,15 @@
 ### Commands Cheatsheet
 
 If using `hatch` CLI, the following commands are available in the default environment:
 
 | Command                | Action                                                              |
 | :--------------------- | :------------------------------------------------------------------ |
 | `hatch run fix`        | Format project with `black .` and apply linting with `ruff --fix .` |
+| `hatch run fmt`        | Format project with `black .` and apply linting with `ruff --fix .` |
 | `hatch run check`      | Check formatting and linting with `black --check .` and `ruff .`.   |
 | `hatch run test`       | Run unittests with `pytest` in base environment.                    |
 | `hatch run test:test`  | Run unittests with `pytest` in all supported environments.          |
 
 Alternatively, you can devlop **cev** by manually creating a virtual environment and managing
 dependencies with `pip`.
```

