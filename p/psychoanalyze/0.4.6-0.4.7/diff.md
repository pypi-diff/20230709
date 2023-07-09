# Comparing `tmp/psychoanalyze-0.4.6.tar.gz` & `tmp/psychoanalyze-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychoanalyze-0.4.6.tar", max compression
+gzip compressed data, was "psychoanalyze-0.4.7.tar", max compression
```

## Comparing `psychoanalyze-0.4.6.tar` & `psychoanalyze-0.4.7.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0    35149 2023-07-04 05:09:13.929334 psychoanalyze-0.4.6/LICENSE
--rw-r--r--   0        0        0     1188 2023-07-04 05:09:13.929334 psychoanalyze-0.4.6/README.md
--rw-r--r--   0        0        0       72 2023-07-04 05:10:53.994641 psychoanalyze-0.4.6/psychoanalyze/__init__.py
--rw-r--r--   0        0        0     6733 2023-07-04 05:09:14.001335 psychoanalyze-0.4.6/psychoanalyze/blocks.py
--rw-r--r--   0        0        0     2969 2023-07-04 05:09:14.001335 psychoanalyze-0.4.6/psychoanalyze/data.py
--rw-r--r--   0        0        0      303 2023-07-04 05:09:14.001335 psychoanalyze-0.4.6/psychoanalyze/gescheider.py
--rw-r--r--   0        0        0     6462 2023-07-04 05:09:14.001335 psychoanalyze-0.4.6/psychoanalyze/plot.py
--rw-r--r--   0        0        0     5580 2023-07-04 05:09:14.001335 psychoanalyze-0.4.6/psychoanalyze/points.py
--rw-r--r--   0        0        0     1966 2023-07-04 05:09:14.001335 psychoanalyze-0.4.6/psychoanalyze/schemas.py
--rw-r--r--   0        0        0     2047 2023-07-04 05:09:14.001335 psychoanalyze-0.4.6/psychoanalyze/sessions.py
--rw-r--r--   0        0        0     3007 2023-07-04 05:09:14.001335 psychoanalyze-0.4.6/psychoanalyze/simulate.py
--rw-r--r--   0        0        0      133 2023-07-04 05:09:14.001335 psychoanalyze-0.4.6/psychoanalyze/stimulus.py
--rw-r--r--   0        0        0      583 2023-07-04 05:09:14.001335 psychoanalyze-0.4.6/psychoanalyze/strength_duration.py
--rw-r--r--   0        0        0      965 2023-07-04 05:09:14.001335 psychoanalyze-0.4.6/psychoanalyze/subjects.py
--rw-r--r--   0        0        0     4922 2023-07-04 05:09:14.001335 psychoanalyze-0.4.6/psychoanalyze/trials.py
--rw-r--r--   0        0        0     1521 2023-07-04 05:09:14.001335 psychoanalyze-0.4.6/psychoanalyze/weber.py
--rw-r--r--   0        0        0     1745 2023-07-04 05:10:53.994641 psychoanalyze-0.4.6/pyproject.toml
--rw-r--r--   0        0        0     2656 1970-01-01 00:00:00.000000 psychoanalyze-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-09 13:22:22.800537 psychoanalyze-0.4.7/LICENSE
+-rw-r--r--   0        0        0     1184 2023-07-09 13:22:22.800537 psychoanalyze-0.4.7/README.md
+-rw-r--r--   0        0        0     1350 2023-07-09 13:23:42.584736 psychoanalyze-0.4.7/psychoanalyze/__init__.py
+-rw-r--r--   0        0        0      749 2023-07-09 13:22:22.876537 psychoanalyze-0.4.7/psychoanalyze/analysis/__init__.py
+-rw-r--r--   0        0        0     1281 2023-07-09 13:22:22.876537 psychoanalyze-0.4.7/psychoanalyze/analysis/bayes.py
+-rw-r--r--   0        0        0     1113 2023-07-09 13:22:22.876537 psychoanalyze-0.4.7/psychoanalyze/analysis/ecdf.py
+-rw-r--r--   0        0        0     2294 2023-07-09 13:22:22.876537 psychoanalyze-0.4.7/psychoanalyze/analysis/strength_duration.py
+-rw-r--r--   0        0        0     2366 2023-07-09 13:22:22.876537 psychoanalyze-0.4.7/psychoanalyze/analysis/weber.py
+-rw-r--r--   0        0        0     1643 2023-07-09 13:22:22.876537 psychoanalyze-0.4.7/psychoanalyze/data/__init__.py
+-rw-r--r--   0        0        0     8278 2023-07-09 13:22:22.876537 psychoanalyze-0.4.7/psychoanalyze/data/blocks.py
+-rw-r--r--   0        0        0     7675 2023-07-09 13:22:22.876537 psychoanalyze-0.4.7/psychoanalyze/data/points.py
+-rw-r--r--   0        0        0     2861 2023-07-09 13:22:22.876537 psychoanalyze-0.4.7/psychoanalyze/data/sessions.py
+-rw-r--r--   0        0        0      834 2023-07-09 13:22:22.876537 psychoanalyze-0.4.7/psychoanalyze/data/stimulus.py
+-rw-r--r--   0        0        0     1671 2023-07-09 13:22:22.876537 psychoanalyze-0.4.7/psychoanalyze/data/subjects.py
+-rw-r--r--   0        0        0     4936 2023-07-09 13:22:22.876537 psychoanalyze-0.4.7/psychoanalyze/data/trials.py
+-rw-r--r--   0        0        0     3462 2023-07-09 13:22:22.876537 psychoanalyze-0.4.7/psychoanalyze/data/types.py
+-rw-r--r--   0        0        0     1582 2023-07-09 13:22:22.876537 psychoanalyze-0.4.7/psychoanalyze/plot.py
+-rw-r--r--   0        0        0     1511 2023-07-09 13:22:22.876537 psychoanalyze-0.4.7/psychoanalyze/sigmoids.py
+-rw-r--r--   0        0        0     1985 2023-07-09 13:23:42.584736 psychoanalyze-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0     2796 1970-01-01 00:00:00.000000 psychoanalyze-0.4.7/PKG-INFO
```

### Comparing `psychoanalyze-0.4.6/LICENSE` & `psychoanalyze-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.6/README.md` & `psychoanalyze-0.4.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,11 +18,11 @@
 ```
 pip:
 ```console
 pip install psychoanalyze
 ```
 
 ## Dashboard
-See what `psychoanalyze` can do by [viewing our dashboard](https://app.psychoanalyze.io/).
+See what `psychoanalyze` can do by [viewing our dashboard](https://psychoanalyze.io/).
 
 ## Documentation
 View the full documentation [here](https://docs.psychoanalyze.io).
```

### Comparing `psychoanalyze-0.4.6/psychoanalyze/sessions.py` & `psychoanalyze-0.4.7/psychoanalyze/data/sessions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,31 @@
-"""Utilities for session-level data."""
+# Copyright 2023 Tyler Schlichenmeyer
+
+# This file is part of PsychoAnalyze.
+# PsychoAnalyze is free software: you can redistribute it and/or modify it under the
+# terms of the GNU General Public License as published by the Free Software Foundation,
+# either version 3 of the License, or (at your option) any later version.
+
+# PsychoAnalyze is distributed in the hope that it will be useful, but WITHOUT ANY
+# WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
+# PARTICULAR PURPOSE. See the GNU General Public License for more details.
+
+# You should have received a copy of the GNU General Public License along with Foobar.
+# If not, see <https://www.gnu.org/licenses/>.
+
+"""Utilities for session-level data.
+
+**Sessions** represent a single day of experiments performed by a subject. It may
+contain several blocks.
+"""
 from pathlib import Path
 
 import pandas as pd
 
-from psychoanalyze import blocks
+from psychoanalyze.data import blocks
 
 dims = ["Monkey", "Date"]
 index_levels = dims
 
 
 def generate(n: int) -> list[int]:
     """Generate session-level data."""
```

### Comparing `psychoanalyze-0.4.6/psychoanalyze/trials.py` & `psychoanalyze-0.4.7/psychoanalyze/data/trials.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,97 +1,89 @@
+# Copyright 2023 Tyler Schlichenmeyer
+
+# This file is part of PsychoAnalyze.
+# PsychoAnalyze is free software: you can redistribute it and/or modify it under the
+# terms of the GNU General Public License as published by the Free Software Foundation,
+# either version 3 of the License, or (at your option) any later version.
+
+# PsychoAnalyze is distributed in the hope that it will be useful, but WITHOUT ANY
+# WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
+# PARTICULAR PURPOSE. See the GNU General Public License for more details.
+
+# You should have received a copy of the GNU General Public License along with Foobar.
+# If not, see <https://www.gnu.org/licenses/>.
+
 """Functions for data manipulations at the trial level."""
 import json
 import random
 from pathlib import Path
 from typing import TypedDict
 
 import numpy as np
 import pandas as pd
-from pandera import DataFrameModel, SeriesSchema
-from pandera.typing import Index
+from pandera import SeriesSchema
 from sklearn.linear_model import LogisticRegression
 
-from psychoanalyze import schemas
+from psychoanalyze.data import types
 
 schema = SeriesSchema(bool, name="Test Trials")
 
-
-class Trials(DataFrameModel):
-
-    """Trials data type for pandera + mypy type checking."""
-
-    result: int
-    intensity: Index[float]
-
-
 data_path = Path("data/trials.csv")
 
 codes = {0: "Miss", 1: "Hit"}
 
 
 Trial = TypedDict("Trial", {"Result": bool, "Stimulus Magnitude": float})
 
 
-def generate_hits(n: int, p: float) -> int:
-    """Sample n hits from n trials and probability p from binomial dist."""
-    return np.random.default_rng().binomial(n, p)
-
-
-def generate_block(dim: str = "x") -> pd.DataFrame:
-    """Generate a block of trial data."""
-    hits = pd.Series(
-        [generate_hits(100, p) for p in [0.1, 0.2, 0.5, 0.8, 0.9]],
-        name="Hits",
+def generate_n(n_trials: int, options: list[float]) -> pd.Series:
+    """Generate n trials (no outcomes)."""
+    return pd.Series(
+        [random.choice(options) for _ in range(n_trials)],
+        name="Intensity",
     )
-    x = [0, 1, 2, 3, 4]
-    return pd.DataFrame({"Hits": hits, "n": [100] * 5}, index=pd.Index(x, name=dim))
 
 
-def generate(n: int, options: list[float], outcomes: list[float]) -> pd.DataFrame:
+def generate(
+    n: pd.Series,
+    outcomes: list[int],
+) -> pd.Series:
     """Generate n trials with outcomes."""
-    return pd.DataFrame(
-        {
-            "result": pd.Series(
-                [random.choice(outcomes) for _ in range(n)],
-                dtype=int,
-            ),
-        },
-        index=pd.Index(
-            [random.choice(options) for _ in range(n)],
-            name="intensity",
-            dtype=float,
-        ),
+    return pd.Series(
+        [random.choice(outcomes) for _ in range(n)],
+        name="Result",
+        index=n,
     )
 
 
 def load(data_path: Path = Path("data")) -> pd.DataFrame:
     """Load trials data from csv."""
-    return schemas.trials.validate(
+    return types.trials.validate(
         pd.read_csv(
             data_path / "trials.csv",
-            index_col=schemas.points_index_levels,
+            index_col=types.points_index_levels,
             parse_dates=["Date"],
         ),
     )
 
 
 def from_store(store_data: str) -> pd.DataFrame:
     """Convert JSON-formatted string to DataFrame."""
     df_dict = json.loads(store_data)
     index_names = df_dict.pop("index_names")
     index = pd.MultiIndex.from_tuples(df_dict["index"])
     trials = pd.DataFrame({"Result": df_dict["data"][0]}, index=index)
     trials.index.names = index_names
-    return schemas.trials.validate(trials)
+    return types.trials.validate(trials)
 
 
 def to_store(trials: pd.DataFrame) -> str:
     """Convert data to a JSON-formatted string for dcc.Store."""
     data_dict = trials.to_dict(orient="split")
-    data_dict["index_names"] = schemas.points_index_levels
+    data_dict["index_names"] = types.points_index_levels
     return json.dumps(data_dict)
 
 
 def normalize(trials: pd.DataFrame) -> dict[str, pd.DataFrame]:
     """Normalize denormalized trial data."""
     return {
         "Session": trials[["Monkey", "Block"]].drop_duplicates(),
```

### Comparing `psychoanalyze-0.4.6/pyproject.toml` & `psychoanalyze-0.4.7/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "psychoanalyze"
-version = "0.4.6"
+version = "0.4.7"
 description = "A Pythonic analysis package for psychophysics data"
 authors = ["Ty Schlichenmeyer <t.schlic@wustl.edu>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "3.11.4"
@@ -29,14 +29,17 @@
 mypy = "^1.4.1"
 click = "^8.1.3"
 typer = {extras = ["all"], version = "^0.9.0"}
 tuna = "^0.5.11"
 nbdev = "^2.3.12"
 ruff = "^0.0.276"
 black = "^23.3.0"
+mkdocs = "^1.4.3"
+mkdocs-material = "^9.1.18"
+mkdocstrings = {extras = ["python"], version = "^0.22.0"}
 
 [tool.poetry.scripts]
 psychoanalyze = "psychoanalyze.__main__:main"
 
 
 [tool.poetry.group.dev.dependencies]
 ipython = "^8.14.0"
@@ -53,15 +56,15 @@
 ]
 branch = "main"
 build_command = "poetry build"
 major_on_zero = true
 
 [tool.bandit]
 targets = ["psychoanalyze/"]
-skips = ["B311"]
+skips = ["B311", "B104"]
 
 [tool.mypy]
 exclude = [
     'target'
 ]
 
 [[tool.mypy.overrides]]
@@ -78,9 +81,15 @@
     'bambi',
     'hypothesis'
 ]
 ignore_missing_imports = true
 
 [tool.ruff]
 fix = true
-select = ["ALL"]
+select = ["ALL", "CPY001"]
 ignore = ["S101", "S311", "D211", "D213"]
+
+[tool.ruff.pydocstyle]
+convention = "google"
+
+[tool.ruff.per-file-ignores]
+"tests/*.py" = ["D100", "D103", "ANN201"]
```

### Comparing `psychoanalyze-0.4.6/PKG-INFO` & `psychoanalyze-0.4.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychoanalyze
-Version: 0.4.6
+Version: 0.4.7
 Summary: A Pythonic analysis package for psychophysics data
 License: GPL-3.0-or-later
 Author: Ty Schlichenmeyer
 Author-email: t.schlic@wustl.edu
 Requires-Python: ==3.11.4
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,17 @@
 Requires-Dist: dash (>=2.10.2,<3.0.0)
 Requires-Dist: dash-bootstrap-components (>=1.4.1,<2.0.0)
 Requires-Dist: dash-daq (>=0.5.0,<0.6.0)
 Requires-Dist: datatest (>=0.11.1,<0.12.0)
 Requires-Dist: dbt-duckdb (>=1.5.1,<2.0.0)
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0)
 Requires-Dist: hypothesis (>=6.79.0,<7.0.0)
+Requires-Dist: mkdocs (>=1.4.3,<2.0.0)
+Requires-Dist: mkdocs-material (>=9.1.18,<10.0.0)
+Requires-Dist: mkdocstrings[python] (>=0.22.0,<0.23.0)
 Requires-Dist: mypy (>=1.4.1,<2.0.0)
 Requires-Dist: nbdev (>=2.3.12,<3.0.0)
 Requires-Dist: numpy (>=1.25.0,<2.0.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: pandas-stubs (>=2.0.2.230605,<3.0.0.0)
 Requires-Dist: pandera[mypy] (>=0.15.1,<0.16.0)
 Requires-Dist: pytest (>=7.3.2,<8.0.0)
@@ -55,12 +58,12 @@
 ```
 pip:
 ```console
 pip install psychoanalyze
 ```
 
 ## Dashboard
-See what `psychoanalyze` can do by [viewing our dashboard](https://app.psychoanalyze.io/).
+See what `psychoanalyze` can do by [viewing our dashboard](https://psychoanalyze.io/).
 
 ## Documentation
 View the full documentation [here](https://docs.psychoanalyze.io).
```

