# Comparing `tmp/scml-vis-0.2.9.tar.gz` & `tmp/scml-vis-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scml-vis-0.2.9.tar", max compression
+gzip compressed data, was "scml-vis-0.3.0.tar", last modified: Sun Jul  9 07:43:41 2023, max compression
```

## Comparing `scml-vis-0.2.9.tar` & `scml-vis-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,82 @@
--rw-r--r--   0        0        0    10255 2021-04-11 06:40:25.098144 scml-vis-0.2.9/LICENSE
--rw-r--r--   0        0        0     4954 2021-06-14 07:44:48.001545 scml-vis-0.2.9/README.md
--rw-r--r--   0        0        0     2017 2021-06-30 08:24:57.648611 scml-vis-0.2.9/pyproject.toml
--rw-r--r--   0        0        0      176 2021-04-11 06:40:25.221840 scml-vis-0.2.9/src/scml_vis/__init__.py
--rw-r--r--   0        0        0      342 2021-04-11 06:40:25.218489 scml-vis-0.2.9/src/scml_vis/__main__.py
--rwxr-xr-x   0        0        0     3261 2021-06-30 04:03:55.466807 scml-vis-0.2.9/src/scml_vis/cli.py
--rwxr-xr-x   0        0        0    34542 2021-06-30 04:04:00.688794 scml-vis-0.2.9/src/scml_vis/compiler.py
--rwxr-xr-x   0        0        0    46850 2021-06-27 04:53:42.678063 scml-vis-0.2.9/src/scml_vis/presenter.py
--rw-r--r--   0        0        0    22584 2021-06-30 04:03:32.304366 scml-vis-0.2.9/src/scml_vis/utils.py
--rw-r--r--   0        0        0        0 2021-04-11 07:13:19.617409 scml-vis-0.2.9/src/scml_vis/vendor/__init__.py
--rw-r--r--   0        0        0    35147 2021-04-11 07:13:19.637343 scml-vis-0.2.9/src/scml_vis/vendor/quick/LICENSE
--rw-r--r--   0        0        0     2465 2021-04-11 07:13:19.716574 scml-vis-0.2.9/src/scml_vis/vendor/quick/README.md
--rw-r--r--   0        0        0        0 2021-04-11 07:13:19.648539 scml-vis-0.2.9/src/scml_vis/vendor/quick/__init__.py
--rw-r--r--   0        0        0    29282 2021-05-27 04:04:11.166046 scml-vis-0.2.9/src/scml_vis/vendor/quick/quick.py
--rw-r--r--   0        0        0       17 2021-04-11 07:13:19.644254 scml-vis-0.2.9/src/scml_vis/vendor/quick/requirements.txt
--rw-r--r--   0        0        0     6356 2021-06-30 08:25:07.370112 scml-vis-0.2.9/setup.py
--rw-r--r--   0        0        0     6001 2021-06-30 08:25:07.370957 scml-vis-0.2.9/PKG-INFO
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-07-09 07:43:41.326635 scml-vis-0.3.0/
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-07-09 07:43:41.281155 scml-vis-0.3.0/.github/
+-rw-r--r--   0 yasser     (501) staff       (20)     6148 2023-06-21 08:32:23.000000 scml-vis-0.3.0/.github/.DS_Store
+-rw-r--r--   0 yasser     (501) staff       (20)      148 2022-04-11 08:17:37.000000 scml-vis-0.3.0/.github/FUNDING.yml
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-07-09 07:43:41.282340 scml-vis-0.3.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 yasser     (501) staff       (20)      688 2022-04-11 08:17:37.000000 scml-vis-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 yasser     (501) staff       (20)      600 2022-04-11 08:17:37.000000 scml-vis-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-07-09 07:43:41.283138 scml-vis-0.3.0/.github/workflows/
+-rw-r--r--   0 yasser     (501) staff       (20)     1736 2023-03-17 04:06:53.000000 scml-vis-0.3.0/.github/workflows/main.yml
+-rw-r--r--   0 yasser     (501) staff       (20)      149 2022-04-11 08:17:37.000000 scml-vis-0.3.0/.gitignore
+-rw-r--r--   0 yasser     (501) staff       (20)     3959 2022-04-11 08:17:37.000000 scml-vis-0.3.0/.vimspector.json
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-07-09 07:43:41.284209 scml-vis-0.3.0/.vscode/
+-rw-r--r--   0 yasser     (501) staff       (20)      695 2022-04-11 08:17:37.000000 scml-vis-0.3.0/.vscode/launch.json
+-rw-r--r--   0 yasser     (501) staff       (20)      115 2022-04-11 08:17:37.000000 scml-vis-0.3.0/.vscode/settings.json
+-rw-r--r--   0 yasser     (501) staff       (20)        1 2022-05-18 03:00:49.000000 scml-vis-0.3.0/CHANGELOG.md
+-rw-r--r--   0 yasser     (501) staff       (20)     3230 2022-04-11 08:17:37.000000 scml-vis-0.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 yasser     (501) staff       (20)     3456 2022-04-11 08:17:37.000000 scml-vis-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0 yasser     (501) staff       (20)    10255 2022-04-11 08:17:37.000000 scml-vis-0.3.0/LICENSE
+-rw-r--r--   0 yasser     (501) staff       (20)      757 2022-04-11 08:17:37.000000 scml-vis-0.3.0/Makefile
+-rw-r--r--   0 yasser     (501) staff       (20)     5696 2023-07-09 07:43:41.326739 scml-vis-0.3.0/PKG-INFO
+-rw-r--r--   0 yasser     (501) staff       (20)     4927 2022-05-18 03:03:33.000000 scml-vis-0.3.0/README.md
+-rw-r--r--   0 yasser     (501) staff       (20)     5331 2023-03-17 04:06:53.000000 scml-vis-0.3.0/README.rst
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-07-09 07:43:41.287014 scml-vis-0.3.0/config/
+-rw-r--r--   0 yasser     (501) staff       (20)      340 2022-04-11 08:17:37.000000 scml-vis-0.3.0/config/coverage.ini
+-rw-r--r--   0 yasser     (501) staff       (20)     2554 2022-04-11 08:17:37.000000 scml-vis-0.3.0/config/flake8.ini
+-rw-r--r--   0 yasser     (501) staff       (20)       63 2022-04-11 08:17:37.000000 scml-vis-0.3.0/config/mypy.ini
+-rw-r--r--   0 yasser     (501) staff       (20)      184 2022-04-11 08:17:37.000000 scml-vis-0.3.0/config/pytest.ini
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-07-09 07:43:41.316740 scml-vis-0.3.0/docs/
+-rw-r--r--   0 yasser     (501) staff       (20)     6148 2023-06-21 08:32:23.000000 scml-vis-0.3.0/docs/.DS_Store
+-rw-r--r--   0 yasser     (501) staff       (20)   353348 2022-04-11 08:17:37.000000 scml-vis-0.3.0/docs/aftercompile.png
+-rw-r--r--   0 yasser     (501) staff       (20)       21 2022-04-11 08:17:37.000000 scml-vis-0.3.0/docs/changelog.md
+-rw-r--r--   0 yasser     (501) staff       (20)       27 2022-04-11 08:17:37.000000 scml-vis-0.3.0/docs/code_of_conduct.md
+-rw-r--r--   0 yasser     (501) staff       (20)    86443 2022-04-11 08:17:37.000000 scml-vis-0.3.0/docs/compile.png
+-rw-r--r--   0 yasser     (501) staff       (20)       24 2022-04-11 08:17:37.000000 scml-vis-0.3.0/docs/contributing.md
+-rw-r--r--   0 yasser     (501) staff       (20)       16 2022-04-11 08:17:37.000000 scml-vis-0.3.0/docs/credits.md
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-07-09 07:43:41.317841 scml-vis-0.3.0/docs/css/
+-rw-r--r--   0 yasser     (501) staff       (20)      688 2022-04-11 08:17:37.000000 scml-vis-0.3.0/docs/css/mkdocstrings.css
+-rw-r--r--   0 yasser     (501) staff       (20)    89541 2022-04-11 08:17:37.000000 scml-vis-0.3.0/docs/datasette.png
+-rw-r--r--   0 yasser     (501) staff       (20)   293912 2022-04-11 08:17:37.000000 scml-vis-0.3.0/docs/datasettelarge.png
+-rw-r--r--   0 yasser     (501) staff       (20)       18 2022-04-11 08:17:37.000000 scml-vis-0.3.0/docs/index.md
+-rw-r--r--   0 yasser     (501) staff       (20)       24 2022-04-11 08:17:37.000000 scml-vis-0.3.0/docs/license.md
+-rw-r--r--   0 yasser     (501) staff       (20)     2673 2022-04-11 08:17:37.000000 scml-vis-0.3.0/docs/macros.py
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-07-09 07:43:41.318252 scml-vis-0.3.0/docs/reference/
+-rw-r--r--   0 yasser     (501) staff       (20)       17 2022-04-11 08:17:37.000000 scml-vis-0.3.0/docs/reference/cli.md
+-rw-r--r--   0 yasser     (501) staff       (20)  1316811 2022-04-11 08:17:37.000000 scml-vis-0.3.0/docs/shot1.png
+-rw-r--r--   0 yasser     (501) staff       (20)  1125356 2022-04-11 08:17:37.000000 scml-vis-0.3.0/docs/shot2.png
+-rw-r--r--   0 yasser     (501) staff       (20)   190689 2022-04-11 08:17:37.000000 scml-vis-0.3.0/docs/show.png
+-rw-r--r--   0 yasser     (501) staff       (20)     9474 2022-04-11 08:17:37.000000 scml-vis-0.3.0/duties.py
+-rw-r--r--   0 yasser     (501) staff       (20)     1035 2022-04-11 08:17:37.000000 scml-vis-0.3.0/mkdocs.yml
+-rw-r--r--   0 yasser     (501) staff       (20)      100 2022-05-17 23:37:59.000000 scml-vis-0.3.0/pyproject.toml
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-07-09 07:43:41.319034 scml-vis-0.3.0/scripts/
+-rwxr-xr-x   0 yasser     (501) staff       (20)      735 2022-04-11 08:17:37.000000 scml-vis-0.3.0/scripts/multirun.sh
+-rwxr-xr-x   0 yasser     (501) staff       (20)      871 2022-04-11 08:17:37.000000 scml-vis-0.3.0/scripts/setup.sh
+-rw-r--r--   0 yasser     (501) staff       (20)     2128 2023-07-09 07:43:41.329619 scml-vis-0.3.0/setup.cfg
+-rwxr-xr-x   0 yasser     (501) staff       (20)       69 2022-05-17 23:37:39.000000 scml-vis-0.3.0/setup.py
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-07-09 07:43:41.271878 scml-vis-0.3.0/src/
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-07-09 07:43:41.321776 scml-vis-0.3.0/src/scml_vis/
+-rw-r--r--   0 yasser     (501) staff       (20)      199 2023-07-09 07:43:10.000000 scml-vis-0.3.0/src/scml_vis/__init__.py
+-rw-r--r--   0 yasser     (501) staff       (20)      342 2022-04-11 08:17:37.000000 scml-vis-0.3.0/src/scml_vis/__main__.py
+-rwxr-xr-x   0 yasser     (501) staff       (20)     3279 2023-03-17 03:05:07.000000 scml-vis-0.3.0/src/scml_vis/cli.py
+-rwxr-xr-x   0 yasser     (501) staff       (20)    36616 2023-06-21 08:31:13.000000 scml-vis-0.3.0/src/scml_vis/compiler.py
+-rwxr-xr-x   0 yasser     (501) staff       (20)    50003 2023-06-21 05:13:25.000000 scml-vis-0.3.0/src/scml_vis/presenter.py
+-rw-r--r--   0 yasser     (501) staff       (20)    23687 2023-06-21 05:44:07.000000 scml-vis-0.3.0/src/scml_vis/utils.py
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-07-09 07:43:41.323826 scml-vis-0.3.0/src/scml_vis/vendor/
+-rw-r--r--   0 yasser     (501) staff       (20)        0 2022-04-11 08:17:37.000000 scml-vis-0.3.0/src/scml_vis/vendor/__init__.py
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-07-09 07:43:41.325419 scml-vis-0.3.0/src/scml_vis/vendor/quick/
+-rw-r--r--   0 yasser     (501) staff       (20)    35147 2022-04-11 08:17:37.000000 scml-vis-0.3.0/src/scml_vis/vendor/quick/LICENSE
+-rw-r--r--   0 yasser     (501) staff       (20)     2465 2022-04-11 08:17:37.000000 scml-vis-0.3.0/src/scml_vis/vendor/quick/README.md
+-rw-r--r--   0 yasser     (501) staff       (20)        0 2022-04-11 08:17:37.000000 scml-vis-0.3.0/src/scml_vis/vendor/quick/__init__.py
+-rw-r--r--   0 yasser     (501) staff       (20)    29282 2022-04-11 08:17:37.000000 scml-vis-0.3.0/src/scml_vis/vendor/quick/quick.py
+-rw-r--r--   0 yasser     (501) staff       (20)       17 2022-04-11 08:17:37.000000 scml-vis-0.3.0/src/scml_vis/vendor/quick/requirements.txt
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-07-09 07:43:41.323506 scml-vis-0.3.0/src/scml_vis.egg-info/
+-rw-r--r--   0 yasser     (501) staff       (20)     5696 2023-07-09 07:43:41.000000 scml-vis-0.3.0/src/scml_vis.egg-info/PKG-INFO
+-rw-r--r--   0 yasser     (501) staff       (20)     1409 2023-07-09 07:43:41.000000 scml-vis-0.3.0/src/scml_vis.egg-info/SOURCES.txt
+-rw-r--r--   0 yasser     (501) staff       (20)        1 2023-07-09 07:43:41.000000 scml-vis-0.3.0/src/scml_vis.egg-info/dependency_links.txt
+-rw-r--r--   0 yasser     (501) staff       (20)      101 2023-07-09 07:43:41.000000 scml-vis-0.3.0/src/scml_vis.egg-info/entry_points.txt
+-rw-r--r--   0 yasser     (501) staff       (20)      226 2023-07-09 07:43:41.000000 scml-vis-0.3.0/src/scml_vis.egg-info/requires.txt
+-rw-r--r--   0 yasser     (501) staff       (20)        9 2023-07-09 07:43:41.000000 scml-vis-0.3.0/src/scml_vis.egg-info/top_level.txt
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-07-09 07:43:41.326387 scml-vis-0.3.0/tests/
+-rw-r--r--   0 yasser     (501) staff       (20)      161 2022-04-11 08:17:37.000000 scml-vis-0.3.0/tests/__init__.py
+-rw-r--r--   0 yasser     (501) staff       (20)       47 2022-04-11 08:17:37.000000 scml-vis-0.3.0/tests/conftest.py
+-rw-r--r--   0 yasser     (501) staff       (20)      410 2022-04-11 08:17:37.000000 scml-vis-0.3.0/tests/test_cli.py
```

### Comparing `scml-vis-0.2.9/LICENSE` & `scml-vis-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scml-vis-0.2.9/README.md` & `scml-vis-0.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -30,18 +30,17 @@
 ## Installation
 
 With `pip`:
 ```bash
 python3 -m pip install scml-vis
 ```
 
-With [`pipx`](https://github.com/pipxproject/pipx):
+With `pipx`:
 ```bash
 python3 -m pip install --user pipx
-
 pipx install scml-vis
 ```
 
 ## Usage
 
 The visualizer can be run using any of the following commands:
 ```bash
@@ -57,34 +56,34 @@
 	```
 	This will open your browser and allow you to choose a world or a tournament to
 	display.
 	![show without parameters](docs/show.png)
 
 	- If this is the first time you visualize logs in this folder, you will be asked
 	  to compile visualization data
-		![compile visualization data](docs/compile.png)
+	  ![compile visualization data](docs/compile.png)
 	- If visualization data is available (or your pressed the `compile visualization data` button), you can now start visualizing the logs
-		![compile visualization data](docs/aftercompile.png)
+	  ![compile visualization data](docs/aftercompile.png)
 - To visualize the logs in a specific folder, you can directly pass the folder as in:
   ```bash
-	scmlv show -f path-to-your-folder
-	```
+  scmlv show -f path-to-your-folder
+  ```
 - It is also possible to just compile visualization data without running the visualizer using:
   ```bash
-	scmlv compile path-to-your-folder
-	```
+  scmlv compile path-to-your-folder
+  ```
 - The visualizer creates a database that it uses to create all the figures you see. You can directly explore this database using:
   ```bash
-	scmlv explore path-to-your-folder
-	```
-	This will open a [datasette](https://docs.datasette.io/en/stable/getting_started.html) page allowing you to explore this database
-	![datasette](docs/datasette.png)
-	This dataset will contain 8 tables describing everything that was logged in the world or tournament. 
-	![datasette](docs/datasettelarge.png)
-	Please consult [datasette documentation](https://docs.datasette.io/en/stable/getting_started.html) for all the ways you can interact with this dataset.
+  scmlv explore path-to-your-folder
+  ```
+  This will open a [datasette](https://docs.datasette.io/en/stable/getting_started.html) page allowing you to explore this database
+  ![datasette](docs/datasette.png)
+  This dataset will contain 8 tables describing everything that was logged in the world or tournament. 
+  ![datasette](docs/datasettelarge.png)
+  Please consult [datasette documentation](https://docs.datasette.io/en/stable/getting_started.html) for all the ways you can interact with this dataset.
 
 ## Available visualizations
 
 To visualize your logs, you need to follow three steps:
 
 1. Filter the dataset using the `Data Selection` section of the sidebar.
 2. Choose the **family** of figures you would like to show from the `Figure Selection` dropdown in the sidebar. Currently we provide `Time-series`, `Tables` and `others` that are always available as well as `Networks`  that are only available when you visualize a single world or filter the tournament to focus on a single world.
```

### Comparing `scml-vis-0.2.9/src/scml_vis/cli.py` & `scml-vis-0.3.0/src/scml_vis/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import subprocess
 import sys
 from functools import partial
 from pathlib import Path
 
 import click
 import click_config_file
-from streamlit import cli as stcli
+from streamlit.web import cli as stcli
 
 try:
     from scml_vis.vendor.quick.quick import gui_option
 except:
 
     def gui_option(x):
         return x
@@ -42,15 +42,15 @@
     "-w",
     "--max-worlds",
     default=None,
     type=int,
     help="Maximum number of worlds to keep in the compiled visualization data",
 )
 def show(folder: Path, max_worlds: int):
-    folder = Path(folder) if folder else None
+    # folder = Path(folder) if folder is not None else None
     if folder and not has_visdata(folder):
         try:
             compiler.main(folder, max_worlds)
         except Exception as e:
             print(f"Failed to compile visualization data for {folder}:\nException: {str(e)}")
     if folder:
         sys.argv = ["streamlit", "run", str(Path(__file__).parent / "presenter.py"), str(folder)]
```

### Comparing `scml-vis-0.2.9/src/scml_vis/compiler.py` & `scml-vis-0.3.0/src/scml_vis/compiler.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,20 @@
 from typing import Dict, Iterable, Optional
 
 import numpy as np
 import pandas as pd
 
 __all__ = ["has_visdata", "has_logs", "main", "VISDATA_FOLDER"]
 
-BASE_IGNORE_SET = {"agent_types", "agent_params", "non_competitors", "non_competitor_params"}
+BASE_IGNORE_SET = {
+    "agent_types",
+    "agent_params",
+    "non_competitors",
+    "non_competitor_params",
+}
 BASE_WORLD_PARAMS_IGNORE_SET = {
     "__dir_name",
     "agent_params",
     "agent_types",
     "name",
     "catalog_prices",
     "profiles",
@@ -83,62 +88,79 @@
         df[c] = df[c].str.split(".").str[0] + "." + df[c].str.split(".").str[-1]
     return df
 
 
 def adjust_column_names(df):
     if df is None or len(df) == 0:
         return df
-    return df.rename(dict(config_id="config", tournament_id="tournament", world_id="world", group_id="group"), axis=1)
+    return df.rename(
+        dict(
+            config_id="config",
+            tournament_id="tournament",
+            world_id="world",
+            group_id="group",
+        ),
+        axis=1,
+    )
 
 
 def nonzero(f):
     return f.exists() and f.stat().st_size > 0
 
 
 def get_folders(base_folder, main_file, required, ignore=None):
     return [
         _.parent
         for _ in base_folder.glob(f"**/{main_file}")
-        if (not ignore or not re.match(ignore, _.name)) and all(nonzero(f) for f in [_.parent / n for n in required])
+        if (not ignore or not re.match(ignore, _.name))
+        and all(nonzero(f) for f in [_.parent / n for n in required])
     ]
 
 
 def is_tournament(base_folder):
     return all(nonzero(f) for f in [base_folder / n for n in TOURNAMENT_REQUIRED])
 
 
 def is_world(base_folder):
     return all(nonzero(f) for f in [base_folder / n for n in WORLD_REQUIRED])
 
 
 def get_torunaments(base_folder, ignore=None):
-    return get_folders(base_folder, main_file=ASSIGNED_CONFIGS_FILE, required=TOURNAMENT_REQUIRED, ignore=ignore)
+    return get_folders(
+        base_folder,
+        main_file=ASSIGNED_CONFIGS_FILE,
+        required=TOURNAMENT_REQUIRED,
+        ignore=ignore,
+    )
 
 
 def get_worlds(base_folder, ignore=None):
-    return get_folders(base_folder, main_file=AGENTS_FILE, required=WORLD_REQUIRED, ignore=ignore)
+    return get_folders(
+        base_folder, main_file=AGENTS_FILE, required=WORLD_REQUIRED, ignore=ignore
+    )
 
 
 def parse_tournament(
     path,
     t_indx,
     base_indx,
     config_ignore_set=BASE_IGNORE_SET,
     assigned_config_ignore_set=ASSIGNED_IGNORE_SET,
     base_world_ignore_set=BASE_WORLD_PARAMS_IGNORE_SET,
     assigned_world_ignore_set=ASSIGNED_WORLD_PARAMS_IGNORE_SET,
+    printer=print,
 ):
     base_configs = json.load(open(path / BASE_CONFIGS_FILE))
     if not base_configs:
         return None, None, None, None
     configs = []
     config_groups = []
     group_map = dict()
 
-    def copy_with_ignore(d, rename_dict, ignore_set, recurse_set):
+    def copy_with_ignore(d, rename_dict, ignore_set, recurse_set, printer=printer):
         c = dict()
         for k, v in d.items():
             if k in ignore_set:
                 continue
             if k in recurse_set:
                 c = {**c, **copy_with_ignore(v, dict(), ignore_set, recurse_set)}
                 continue
@@ -149,16 +171,25 @@
         return c
 
     recurse_set = ["world_params", "__exact_params", "info"]
     for aconfig in base_configs:
         conf_group_id = ""
         config_set = []
         for c in aconfig:
-            conf_group_id = (conf_group_id + ":" + c["config_id"]) if conf_group_id else c["config_id"]
-            d = copy_with_ignore(c, dict(config_id="id"), config_ignore_set.union(base_world_ignore_set), recurse_set)
+            conf_group_id = (
+                (conf_group_id + ":" + c["config_id"])
+                if conf_group_id
+                else c["config_id"]
+            )
+            d = copy_with_ignore(
+                c,
+                dict(config_id="id"),
+                config_ignore_set.union(base_world_ignore_set),
+                recurse_set,
+            )
             config_set.append(d)
         config_groups.append(dict(id=conf_group_id))
         for c in config_set:
             c["group"] = conf_group_id
             configs.append(c)
             group_map[c["id"]] = conf_group_id
 
@@ -184,22 +215,31 @@
                 id=c["world_params"]["name"],
                 path=p,
                 n_agents=len(c["is_default"]),
                 tournament=path.name,
                 tournament_indx=t_indx,
             )
             d = {
-                **copy_with_ignore(c, dict(), assigned_config_ignore_set.union(assigned_world_ignore_set), recurse_set),
+                **copy_with_ignore(
+                    c,
+                    dict(),
+                    assigned_config_ignore_set.union(assigned_world_ignore_set),
+                    recurse_set,
+                ),
                 **d,
             }
             d["name"] = c["world_params"]["name"]
             worlds.append(d)
             world_indx[worlds[-1]["id"]] = worlds[-1]["name"]
             _, wa = get_basic_world_info(
-                Path(p), path.name, worlds[-1]["config_id"], group_map.get(worlds[-1]["config_id"], "none")
+                Path(p),
+                path.name,
+                worlds[-1]["config_id"],
+                group_map.get(worlds[-1]["config_id"], "none"),
+                printer=printer,
             )
             if not _:
                 continue
             agents.append(wa)
 
     agents = pd.concat(agents)
 
@@ -215,17 +255,21 @@
     if (path / AGENTS_JSON_FILE).exists():
         scored_agents = set(agents["name"].to_list())
         ag_dict = json.load(open(path / AGENTS_JSON_FILE))
         for k, v in ag_dict.items():
             if k in ("BUYER", "SELLER"):
                 v["final_score"] = float("nan")
             elif k in scored_agents:
-                a, b = stats[f"score_{k}"].values[-1], float(agents.loc[agents["name"] == k, "final_score"].values)
+                a, b = stats[f"score_{k}"].values[-1], float(
+                    agents.loc[agents["name"] == k, "final_score"].values
+                )
                 assert a == b
-                v["final_score"] = float(agents.loc[agents["name"] == k, "final_score"].values)
+                v["final_score"] = float(
+                    agents.loc[agents["name"] == k, "final_score"].values
+                )
             else:
                 v["final_score"] = stats[f"score_{k}"].values[-1]
         world_agents = pd.DataFrame.from_records(list(ag_dict.values()))
         world_agents["official_score"] = world_agents["name"].isin(scored_agents)
     else:
         world_agents = agents
         world_agents["official_score"] = True
@@ -333,15 +377,17 @@
                 "step",
                 "offers",
                 "ended_at",
             ],
         ]
         negotiations = negotiations.rename(columns=dict(step="rounds"))
         negotiations = negotiations.rename(columns=dict(ended_at="step"))
-        negotiations["offers"] = negotiations.offers.apply(lambda x: eval(x) if isinstance(x, str) else x)
+        negotiations["offers"] = negotiations.offers.apply(
+            lambda x: eval(x) if isinstance(x, str) else x
+        )
         negotiations["rounds"] = negotiations["rounds"] - 1
         for indx, neg in negotiations.iterrows():
             d = dict(
                 sender=None,
                 receiver=None,
                 delivery_step=None,
                 quantity=None,
@@ -354,22 +400,26 @@
                 caller=neg["caller"],
                 product=neg["product"],
                 world=wname,
                 tournament=tname,
             )
             if not neg["offers"]:
                 continue
-            offers = eval(neg["offers"]) if isinstance(neg["offers"], str) else neg["offers"]
+            offers = (
+                eval(neg["offers"]) if isinstance(neg["offers"], str) else neg["offers"]
+            )
             current_offers = []
             for k, vs in offers.items():
                 for r, v in enumerate(vs):
                     dd = {**d}
                     dd["sender"] = k
                     dd["negotiation"] = neg["id"]
-                    dd["receiver"] = neg["seller"] if k == neg["buyer"] else neg["buyer"]
+                    dd["receiver"] = (
+                        neg["seller"] if k == neg["buyer"] else neg["buyer"]
+                    )
                     dd["round"] = r
                     if v:
                         dd["quantity"] = v[0]
                         dd["delivery_step"] = v[1]
                         dd["unit_price"] = v[2]
                     else:
                         dd["quantity"] = None
@@ -377,15 +427,17 @@
                         dd["unit_price"] = None
 
                     current_offers.append(dd)
             for indx, v in enumerate(current_offers):
                 v["index"] = indx
             offers_list += current_offers
 
-        atmap = dict(zip(world_agents["name"].to_list(), world_agents["type"].to_list()))
+        atmap = dict(
+            zip(world_agents["name"].to_list(), world_agents["type"].to_list())
+        )
         # atmap = dict(zip(all_agents["name"].to_list(), all_agents["type"].to_list()))
         # negotiations.agreement[negotiations.agreement.isna(), "agreement"] = None
         for c in ["quantity", "delivery_step", "unit_price"]:
             negotiations[c] = None
 
         def lst(x):
             return (
@@ -393,15 +445,17 @@
                 if not x or (isinstance(x, str) and x.lower() == "none")
                 else list(eval(x))
                 if isinstance(x, str)
                 else list(x)
             )
 
         negotiations.agreement = negotiations.agreement.apply(lst)
-        agreements = pd.DataFrame(negotiations.agreement.tolist(), index=negotiations.index)
+        agreements = pd.DataFrame(
+            negotiations.agreement.tolist(), index=negotiations.index
+        )
         agreements.columns = ["quantity", "delivery_step", "unit_price"]
         for c in ["quantity", "delivery_step", "unit_price"]:
             negotiations[c] = agreements[c]
             negotiations.loc[negotiations.loc[:, c] < 0, c] = float("nan")
 
         def do_map(x):
             return atmap[x]
@@ -439,24 +493,28 @@
         negotiations = pd.concat((negotiations, issues), axis=1)
         if len(negotiations):
             negotiations.drop("issues", axis=1, inplace=True)
             for c in negotiations.columns:
                 if not c.endswith("step") and not c.endswith("steps"):
                     continue
                 negotiations.loc[negotiations[c] < 0, c] = float("nan")
-                negotiations[c.replace("step", "relative_time")] = negotiations[c] / nsteps if nsteps else 0.0
+                negotiations[c.replace("step", "relative_time")] = (
+                    negotiations[c] / nsteps if nsteps else 0.0
+                )
         offers = pd.DataFrame.from_records(offers_list)
         if len(offers):
             offers["receiver_type"] = offers.receiver.apply(do_map)
             offers["sender_type"] = offers.sender.apply(do_map)
             for c in offers.columns:
                 if not c.endswith("step") and not c.endswith("steps"):
                     continue
                 offers.loc[offers[c] < 0, c] = float("nan")
-                offers[c.replace("step", "relative_time")] = offers[c] / nsteps if nsteps else 0.0
+                offers[c.replace("step", "relative_time")] = (
+                    offers[c] / nsteps if nsteps else 0.0
+                )
 
     contracts = contracts.loc[
         :,
         [
             "id",
             "seller_type",
             "buyer_type",
@@ -482,19 +540,23 @@
         columns=dict(
             delivery_time="delivery_step",
             negotiation_id="negotiation",
             product_name="product",
         )
     )
     contracts["product"] = contracts["product"].str[1:].astype(int)
-    contracts.columns = [_.replace("_at", "_step") if _.endswith("_at") else _ for _ in contracts.columns]
+    contracts.columns = [
+        _.replace("_at", "_step") if _.endswith("_at") else _ for _ in contracts.columns
+    ]
     # contracts["step"] = contracts["concluded_step"]
     contracts["breached_step"] = contracts["executed_step"]
     contracts["breaches"] = contracts.breaches.astype(str)
-    contracts.loc[(contracts.signed_step >= 0) & (contracts.executed_step < 0), "breached_step"] = -1
+    contracts.loc[
+        (contracts.signed_step >= 0) & (contracts.executed_step < 0), "breached_step"
+    ] = -1
     contracts.loc[
         (contracts.signed_step >= 0) & (contracts.breaches.str.len() > 0),
         "breached_step",
     ] = -1
     contracts["world"] = wname
     contracts["tournament"] = tname
     # step_cols = (
@@ -507,15 +569,17 @@
     #     "nullified_",
     #     "breached_",
     # )
     for c in contracts.columns:
         if not c.endswith("step") and not c.endswith("steps"):
             continue
         contracts.loc[contracts[c] < 0, c] = float("nan")
-        contracts[c.replace("step", "relative_time")] = contracts[c] / nsteps if nsteps else 0.0
+        contracts[c.replace("step", "relative_time")] = (
+            contracts[c] / nsteps if nsteps else 0.0
+        )
 
     contract_stats, negotiation_stats = [], []
     non_step_cols = [
         "unit_price",
         "quantity",
         "product",
         "buyer",
@@ -534,24 +598,34 @@
 
     for step in range(nsteps):
         s = None
         for c in contracts.columns:
             if not c.endswith("step"):
                 continue
             base = c.replace("step", "").replace("_", "")
-            qp = contracts.loc[contracts[c] == step, non_step_cols].groupby(non_step_cols[2:]).apply(calc_qp)
+            qp = (
+                contracts.loc[contracts[c] == step, non_step_cols]
+                .groupby(non_step_cols[2:])
+                .apply(calc_qp)
+            )
             if not isinstance(qp, pd.DataFrame):
                 qp = pd.DataFrame(data=qp, index=qp.index)
             if len(qp) < 1:
                 continue
             # breakpoint()
             qp.columns = ["qp"]
             # breakpoint()
             qp = pd.DataFrame(qp["qp"].tolist(), index=qp.index)
-            qp = qp.rename(columns={0: base + "_quantity", 1: base + "_count", 2: base + "_unit_price"})
+            qp = qp.rename(
+                columns={
+                    0: base + "_quantity",
+                    1: base + "_count",
+                    2: base + "_unit_price",
+                }
+            )
             # qp = qp.reset_index()
             qp["step"] = step
             qp.set_index(["step"], append=True, inplace=True)
             qp = qp.melt(
                 value_vars=[base + "_quantity", base + "_count", base + "_unit_price"],
                 ignore_index=False,
             )
@@ -564,23 +638,26 @@
     # contract_stats = pd.DataFrame.from_records(contract_stats)
     contract_stats = pd.concat(contract_stats, ignore_index=True)
     contract_stats = contract_stats.pivot(
         index=[_ for _ in contract_stats.columns if _ not in ("variable", "value")],
         columns="variable",
         values="value",
     ).reset_index()
-    contract_stats["relative_time"] = (contract_stats["step"] / nsteps) if nsteps else 0.0
+    contract_stats["relative_time"] = (
+        (contract_stats["step"] / nsteps) if nsteps else 0.0
+    )
     contract_stats = contract_stats.fillna(0)
     contract_stats["world"] = wname
     contract_stats["tournament"] = tname
     for col in [_ for _ in contract_stats.columns if _.endswith("unit_price")]:
         field = col.split("_")[0]
         if f"{field}_quantity" in contract_stats.columns:
             contract_stats[f"{field}_total_price"] = (
-                contract_stats[f"{field}_quantity"] * contract_stats[f"{field}_unit_price"]
+                contract_stats[f"{field}_quantity"]
+                * contract_stats[f"{field}_unit_price"]
             )
 
     for c in contract_stats.columns:
         if c.endswith("quantity"):
             contract_stats[c] = contract_stats[c].astype(int)
         if c.endswith("count"):
             contract_stats[c] = contract_stats[c].astype(int)
@@ -618,21 +695,29 @@
             "perpetrator",
             "perpetrator_type",
             "victims",
             "resolved",
         ],
     ]
     breaches = breaches.rename(columns=dict(contract_id="contract"))
-    breaches["victim"] = breaches["victims"].apply(lambda x: x[0] if not isinstance(x, str) else eval(x)[0])
+    breaches["victim"] = breaches["victims"].apply(
+        lambda x: x[0] if not isinstance(x, str) else eval(x)[0]
+    )
     # contracts["relative_time"] = breaches["step"] / nsteps
     breaches.drop(["victims"], axis=1)
     agent_names = world_agents["name"].unique()
     # inventory_{}_input", output
     product_stat_names = ["trading_price", "sold_quantity", "unit_price"]
-    products = set([_.split("_")[-1] for _ in stats.columns if any(_.startswith(p) for p in product_stat_names)])
+    products = set(
+        [
+            _.split("_")[-1]
+            for _ in stats.columns
+            if any(_.startswith(p) for p in product_stat_names)
+        ]
+    )
     agent_stat_names = [
         "balance",
         "productivity",
         "bankrupt",
         "score",
         "assets",
         "inventory-input",
@@ -640,30 +725,40 @@
         "spot_market_loss",
         "spot_market_quantity",
     ]
     agents_info, product_info = [], []
     world_stat_names = list(
         str(_)
         for _ in stats.columns
-        if not any(_.startswith(n.split("-")[0]) for n in (agent_stat_names + product_stat_names))
+        if not any(
+            _.startswith(n.split("-")[0])
+            for n in (agent_stat_names + product_stat_names)
+        )
     )
     for aname in agent_names:
+        if aname in ("BUYER", "SELLER"):
+            continue
         colnames = []
-        ainfo = world_agents.loc[world_agents["name"] == aname, ["type", "final_score"]].to_dict("records")[0]
+        ainfo = world_agents.loc[
+            world_agents["name"] == aname, ["type", "final_score"]
+        ].to_dict("records")[0]
         for n in agent_stat_names:
             ns = n.split("-")
             if len(ns) > 1:
                 col_name = f"{ns[0]}_{aname}_{ns[-1]}"
             else:
                 col_name = f"{n}_{aname}"
             if col_name not in stats.columns:
                 continue
             colnames.append(col_name)
         x = stats.loc[:, colnames].reset_index().rename(columns=dict(index="step"))
-        x.columns = [_ if aname not in _ else _.replace(f"_{aname}", "").replace("-", "_") for _ in x.columns]
+        x.columns = [
+            _ if aname not in _ else _.replace(f"_{aname}", "").replace("-", "_")
+            for _ in x.columns
+        ]
         if len(x):
             x["relative_time"] = x["step"] / nsteps
         else:
             x["relative_time"] = 0.0
         x["name"] = aname
         x["world"] = wname
         x["tournament"] = tname
@@ -673,25 +768,29 @@
 
     for p in products:
         colnames = []
         for n in product_stat_names:
             col_name = f"{n}_{p}"
             colnames.append(col_name)
         x = stats.loc[:, colnames].reset_index().rename(columns=dict(index="step"))
-        x.columns = ["_".join(_.split("_")[:-1]) if _.endswith(f"_{p}") else _ for _ in x.columns]
+        x.columns = [
+            "_".join(_.split("_")[:-1]) if _.endswith(f"_{p}") else _ for _ in x.columns
+        ]
         if len(x):
             x["relative_time"] = x["step"] / nsteps
         else:
             x["relative_time"] = 0.0
         x["product"] = p
         x["world"] = wname
         x["tournament"] = tname
         product_info.append(x)
 
-    world_info = stats.loc[:, world_stat_names].reset_index().rename(columns=dict(index="step"))
+    world_info = (
+        stats.loc[:, world_stat_names].reset_index().rename(columns=dict(index="step"))
+    )
     if len(world_info):
         world_info["relative_time"] = world_info["step"] / nsteps
     else:
         world_info["relative_time"] = 0.0
     world_info["world"] = wname
     world_info["tournament"] = tname
 
@@ -704,21 +803,21 @@
         negotiations,
         offers,
         negotiation_stats,
         breaches,
     )
 
 
-def get_basic_world_info(path, tname, gname, cname):
+def get_basic_world_info(path, tname, gname, cname, printer=print):
     try:
         stats = pd.read_csv(path / STATS_FILE, index_col=0).to_dict("list")
         adata = json.load(open(path / AGENTS_JSON_FILE))
         winfo = json.load(open(path / INFO_FILE))
     except:
-        print(f"FAILED {path.name}", flush=True)
+        printer(f"FAILED {path.name}", flush=True)
         return [], None
     worlds = [
         dict(
             name=path.name,
             tournament=tname,
             config=cname,
             group=gname,
@@ -726,48 +825,60 @@
             path=path,
             n_steps=winfo["n_steps"],
         )
     ]
     agents = []
     definfo = winfo.get("is_default", None)
     agent_key = None
-    for k in ("agent_initial_balances", "agent_profiles", "agent_inputs", "agent_outputs", "agent_processes"):
+    for k in (
+        "agent_initial_balances",
+        "agent_profiles",
+        "agent_inputs",
+        "agent_outputs",
+        "agent_processes",
+    ):
         if k in winfo.keys():
             agent_key = k
             break
     if definfo:
         is_default = dict(zip(winfo[agent_key].keys(), definfo))
     else:
         is_default = dict(zip(winfo[agent_key].keys(), itertools.repeat(False)))
+    # print(stats.keys())
     for i, (aname, info) in enumerate(adata.items()):
-        if f"score_{aname}" not in stats.keys():
+        if aname in ("SELLER", "BUYER"):
             continue
-        score = stats[f"score_{aname}"][-1]
-        aginfo = winfo["agent_profiles"][aname]
-        aginfo["initial_balance"] = winfo.get("agent_initial_balances", dict()).get(aname, float("nan"))
+        if f"score_{aname}" not in stats.keys():
+            score = float("nan")
+        else:
+            score = stats[f"score_{aname}"][-1]
+        aginfo = winfo["agent_profiles"].get(aname, dict())
+        aginfo["initial_balance"] = winfo.get("agent_initial_balances", dict()).get(
+            aname, float("nan")
+        )
         aginfo["is_default"] = is_default.get(aname, True)
         if "costs" in aginfo.keys():
             aginfo["cost"] = float(np.asarray(aginfo["costs"]).min())
             del aginfo["costs"]
         dd = dict(
             id=i,
             name=aname,
             world=worlds[0]["name"],
             tournament=tname,
             group=gname,
             config=cname,
             final_score=score,
             type=info["type"],
         )
-        dd = {**dd, **aginfo}
+        dd = {**dd, **info, **aginfo}
         agents.append(dd)
     return worlds, pd.DataFrame.from_records(agents)
 
 
-def get_data(base_folder, ignore: Optional[str] = None):
+def get_data(base_folder, ignore: Optional[str] = None, printer=print):
     base_folder = Path(base_folder)
     tournaments, worlds, agents, agent_stats, product_stats, world_stats = (
         [],
         [],
         [],
         [],
         [],
@@ -791,54 +902,64 @@
     for i, t in enumerate(paths):
         indx = i + 1
         base_indx = (i + 1) * 1_000_000
         if t is not None:
             if is_tournament(t):
                 print(f"Tournament {t.name} [{i} of {len(paths)}]", flush=True)
                 tournaments.append(dict(id=indx, path=t, name=t.name))
-                g, con, w, a = parse_tournament(t, indx, base_indx)
+                g, con, w, a = parse_tournament(t, indx, base_indx, printer=printer)
                 tname = t.name
             else:
                 print(f"World {t.name} [{i} of {len(paths)}]", flush=True)
                 if not none_added:
                     tournaments.append(none_tournament)
                     none_added = True
-                w, a = get_basic_world_info(base_folder, "none", "none", "none")
+                w, a = get_basic_world_info(
+                    base_folder, "none", "none", "none", printer=printer
+                )
                 g = [{k: v for k, v in none_group.items()}]
                 con = [{k: v for k, v in none_config.items()}]
                 tname = "none"
         else:
             print(f"No tournament found ... reading world info")
             tname = "none"
             tournaments.append(dict(id=tname, path=base_folder.parent, name=tname))
             g = [{k: v for k, v in none_group.items()}]
             con = [{k: v for k, v in none_config.items()}]
-            w, a = get_basic_world_info(base_folder, tname, "none", "none")
+            w, a = get_basic_world_info(
+                base_folder, tname, "none", "none", printer=printer
+            )
+        if w is None or len(w) < 1:
+            printer(f"No world data found!!")
+            return None
+        if a is None or len(a) < 1:
+            printer(f"No agent data found!!")
+            return None
         for gg in g:
             gg["tournament"] = tname
         for cc in con:
             cc["tournament"] = tname
         groups += g
         configs += con
         if not w:
             continue
         for j, world in enumerate(w):
-            wagents = a.loc[a.world == world["name"]]
             try:
+                wagents = a.loc[a.world == world["name"]]
                 ag, pr, wo, co, cs, ng, of, ns, br = parse_world(
                     Path(world["path"]),
                     tname,
                     world["name"],
                     world["n_steps"],
                     wagents,
                     base_indx + j + 1,
                     base_indx + j + 1,
                 )
             except:
-                print(f"\tParse Error {world['name']}", flush=True)
+                printer(f"\tParse Error {world['name']}", flush=True)
                 continue
             print(f"\tWorld {world['name']} [{j} of {len(w)}]", flush=True)
             if ag is not None and len(ag):
                 agent_stats.append(ag)
             if pr is not None and len(pr):
                 product_stats.append(pr)
             if wo is not None and len(wo):
@@ -916,29 +1037,39 @@
             s = infile.read()
         for k, v in m.items():
             s = s.replace(k, v)
         with open(fname, "w") as outfile:
             outfile.write(s)
 
 
-def main(folder: Path, max_worlds: Optional[int], ignore: Optional[str] = None, pathmap: Optional[str] = None):
+def main(
+    folder: Path,
+    max_worlds: Optional[int],
+    ignore: Optional[str] = None,
+    pathmap: Optional[str] = None,
+    printer=print,
+):
     folder = Path(folder)
     if max_worlds is None:
         max_worlds = float("inf")
     dst_folder = folder / VISDATA_FOLDER
     if dst_folder.exists():
         raise ValueError(
             f"Destiantion folder {dst_folder} exists. Delete it if you want to recompile visualization data"
         )
     folder = Path(folder)
 
     if pathmap:
         m = pathmap.split(":")
         map_paths(folder, dict(zip(m[0::2], m[1::2])))
 
+    data__ = get_data(folder, ignore=ignore, printer=printer)
+    if not data__:
+        printer(f"Cannot parse data!!")
+        return
     (
         tournaments,
         groups,
         configs,
         worlds,
         agents,
         agent_stats,
@@ -946,15 +1077,15 @@
         world_stats,
         contracts,
         contract_stats,
         negotiations,
         offers,
         neg_stats,
         breaches,
-    ) = get_data(folder, ignore=ignore)
+    ) = data__
     dst_folder = folder / VISDATA_FOLDER
     dst_folder.mkdir(parents=True, exist_ok=True)
     for df, name in zip(
         (
             tournaments,
             groups,
             configs,
@@ -984,15 +1115,15 @@
             "negotiations",
             "offers",
             "neg_stats",
             "breaches",
         ),
     ):
         if df is None or len(df) == 0:
-            print(f"\tDid not find {name}")
+            printer(f"\tDid not find {name}")
             continue
         df = adjust_type_names(df)
         df = adjust_column_names(df)
         df.to_csv(dst_folder / f"{name}.csv", index=False)
 
 
 def has_visdata(folder: Path):
```

### Comparing `scml-vis-0.2.9/src/scml_vis/presenter.py` & `scml-vis-0.3.0/src/scml_vis/presenter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 #!/usr/bin/env python
-import shutil
 import itertools
 import random
+import shutil
 import sys
 import traceback
+from math import isnan
 from pathlib import Path
 
 import altair as alt
 import pandas as pd
 import plotly as plotly
 import plotly.express as px
 import plotly.graph_objects as go
 import streamlit as st
+from negmas.helpers import unique_name
 from pandas.api.types import is_numeric_dtype
 from plotly.validators.scatter.marker import SymbolValidator
-from streamlit import cli as stcli
+from streamlit.web import cli as stcli
 
 import scml_vis.compiler as compiler
 from scml_vis.compiler import VISDATA_FOLDER
 from scml_vis.utils import (
     add_selector,
     add_stats_display,
     add_stats_selector,
@@ -28,26 +30,29 @@
     score_factors,
 )
 
 __all__ = ["main"]
 
 
 MARKERS = SymbolValidator().values[2::3]
-MARKERS = [_ for _ in MARKERS if not any(_.startswith(x) for x in ("star", "circle", "square"))]
+MARKERS = [
+    _ for _ in MARKERS if not any(_.startswith(x) for x in ("star", "circle", "square"))
+]
 random.shuffle(MARKERS)
 MARKERS = ["circle", "square"] + MARKERS
 
 DB_FOLDER = Path.home() / "negmas" / "runsdb"
 DB_NAME = "rundb.csv"
 BASE_FOLDERS = [
     Path.home() / "negmas" / "logs" / "scml" / "scml2020",
     Path.home() / "negmas" / "logs" / "scml" / "scml2020oneshot",
     Path.home() / "negmas" / "logs" / "scml" / "scml2021oneshot",
     Path.home() / "negmas" / "logs" / "scml" / "scml2021",
     Path.home() / "negmas" / "logs" / "tournaments",
+    Path.home() / "negmas" / "tournaments",
 ]
 
 
 def main(folder: Path):
     st.set_page_config(layout="wide")
     if folder is None:
         add_base = st.sidebar.checkbox("Add Default paths", True)
@@ -65,126 +70,155 @@
             for base in BASE_FOLDERS:
                 type_ = base.name == "tournaments"
                 for child in base.glob("*"):
                     if not child.is_dir() or not compiler.has_logs(child):
                         continue
                     options[child] = f"{'t' if type_ else 'w'}:{child.name}"
 
-        folder = st.sidebar.selectbox("Select a run", list(options.keys()), format_func=lambda x: options[x])
+        folder = st.sidebar.selectbox(
+            "Select a run", list(options.keys()), format_func=lambda x: options[x]
+        )
     if not folder or (isinstance(folder, str) and folder == "none"):
         st.text(
-            "Cannot find any folders with logs.\nTry looking in default paths by checking 'Add Default paths' \nin the side bar or start the app with a folder containing log data using -f"
+            "Cannot find any folders with logs in the command line arguments.\nTry looking in default paths by checking 'Add Default paths' \nin the side bar or start the app with a folder containing log data using -f"
         )
         return
     folder = Path(folder)
     if folder.name != VISDATA_FOLDER:
         folder = folder / VISDATA_FOLDER
     if folder.exists():
         re_compile = st.sidebar.button("Recompile visualization data?")
         if re_compile:
-            st.error("Do you really, really, want to remove all visuallization data and recopmile?")
+            st.error(
+                "Do you really, really, want to remove all visuallization data and recopmile?"
+            )
             if st.button("Yes I'm OK with that"):
                 shutil.rmtree(folder)
 
     if not folder.exists():
         try:
             do_compile = st.sidebar.button("Compile visualization data?")
             if do_compile:
                 try:
-                    compiler.main(folder.parent, max_worlds=None)
+                    compiler.main(folder.parent, max_worlds=None, printer=st.write)
                 except Exception as e:
-                    st.write(f"*Failed to compile visualization data for {folder}*\n### Exception:\n{str(e)}")
+                    st.write(
+                        f"*Failed to compile visualization data for {folder}*\n### Exception:\n{str(e)}"
+                    )
                     st.write(f"\n### Traceback:\n```\n{traceback.format_exc()}```")
             else:
-                st.text("Either press 'Compile visualization data' to view logs of this folder or choose another one.")
+                st.text(
+                    "Either press 'Compile visualization data' to view logs of this folder or choose another one."
+                )
                 return
         except:
             st.write(f"Folder {folder} contains no logs to use")
         # folder = folder / VISDATA_FOLDER
         # if not folder.exists():
         #     st.write(
         #         f"## SCML Visualizer\nError: No {VISDATA_FOLDER} folder found with visualization data at {str(folder)}"
         #     )
         #     return
     if folder.name != VISDATA_FOLDER:
         folder = folder / VISDATA_FOLDER
     if not folder.exists():
-        st.write("Cannot find visualiation data")
+        st.write("Cannot find visualization data")
         return
+    else:
+        print(f"{folder} exists")
 
     st.write(f"## SCML Visualizer\n{str(folder.parent)}")
 
     st.sidebar.markdown("## Data Selection")
+    st.write(folder)
     tournaments = load_data(folder, "tournaments")
-    tournament_expander = st.sidebar.beta_expander("Tournament Selection")
-    with tournament_expander:
-        selected_tournaments, _, _ = add_selector(
-            st,
-            "",
-            tournaments["name"].unique(),
-            key="tournaments",
-            none=False,
-            default="one",
-        )
+    if tournaments is not None and len(tournaments) > 0:
+        tournament_expander = st.sidebar.expander("Tournament Selection")
+        with tournament_expander:
+            selected_tournaments, _, _ = add_selector(
+                st,
+                "",
+                tournaments["name"].unique(),
+                key="tournaments",
+                none=False,
+                default="one",
+            )
     worlds = None
     configs = load_data(folder, "configs")
     if configs is None:
         worlds = load_data(folder, "worlds")
-        config_names = worlds.loc[:, "name"].str.split("_").str[0].unique()
-        configs = pd.DataFrame(data=config_names, columns=["id"])
-    config_expander = st.sidebar.beta_expander("Config Selection")
-    with config_expander:
-        selected_configs, _, _ = add_selector(
-            st,
-            "",
-            configs["id"].unique(),
-            key="configs",
-            none=False,
-            default="all",
-        )
+        if worlds is not None and len(worlds) > 0:
+            config_names = worlds.loc[:, "name"].str.split("_").str[0].unique()
+            configs = pd.DataFrame(data=config_names, columns=["id"])
+    config_expander = st.sidebar.expander("Config Selection")
+    if configs is not None and len(configs):
+        with config_expander:
+            selected_configs, _, _ = add_selector(
+                st,
+                "",
+                configs["id"].unique(),
+                key="configs",
+                none=False,
+                default="all",
+            )
 
     if worlds is None:
         worlds = load_data(folder, "worlds")
     if "config" not in worlds.columns:
         worlds["config"] = worlds.loc[:, "name"].str.split("_").str[0]
-    worlds = worlds.loc[worlds.tournament.isin(selected_tournaments) & worlds.config.isin(selected_configs), :]
-    world_expander = st.sidebar.beta_expander("World Selection")
+    worlds = worlds.loc[
+        worlds.tournament.isin(selected_tournaments)
+        & worlds.config.isin(selected_configs),
+        :,
+    ]
+    world_expander = st.sidebar.expander("World Selection")
     with world_expander:
-        selected_worlds, _, _ = add_selector(st, "", worlds.name, key="worlds", none=False, default="all")
+        selected_worlds, _, _ = add_selector(
+            st, "", worlds.name, key="worlds", none=False, default="all"
+        )
     worlds = worlds.loc[(worlds.name.isin(selected_worlds)), :]
 
     agents = load_data(folder, "agents")
-    type_expander = st.sidebar.beta_expander("Type Selection")
+    type_expander = st.sidebar.expander("Type Selection")
     with type_expander:
-        selected_types, _, _ = add_selector(st, "", agents.type.unique(), key="types", none=False, default="all")
+        selected_types, _, _ = add_selector(
+            st, "", agents.type.unique(), key="types", none=False, default="all"
+        )
     agents = agents.loc[(agents.type.isin(selected_types)), :]
 
-    agent_expander = st.sidebar.beta_expander("Agent Selection")
+    agent_expander = st.sidebar.expander("Agent Selection")
     with agent_expander:
-        selected_agents, _, _ = add_selector(st, "", agents.name.unique(), key="agents", none=False, default="all")
+        selected_agents, _, _ = add_selector(
+            st, "", agents.name.unique(), key="agents", none=False, default="all"
+        )
 
     products = load_data(folder, "product_stats")
-    product_expander = st.sidebar.beta_expander("Product Selection")
+    product_expander = st.sidebar.expander("Product Selection")
     with product_expander:
         selected_products, _, _ = add_selector(
-            st, "", products["product"].unique(), key="products", none=False, default="all"
+            st,
+            "",
+            products["product"].unique(),
+            key="products",
+            none=False,
+            default="all",
         )
 
     agents = agents.loc[(agents.type.isin(selected_types)), :]
 
     nsteps = worlds.loc[worlds.name.isin(selected_worlds), "n_steps"].max()
     nsteps = int(nsteps)
     selected_steps = st.sidebar.slider("Steps", 0, nsteps, (0, nsteps))
     selected_times = st.sidebar.slider("Relative Times", 0.0, 1.0, (0.0, 1.0))
 
     st.sidebar.markdown("## Figure Selection")
-    # ts_figs = st.sidebar.beta_expander("Time Series")
-    # net_figs = st.sidebar.beta_expander("Networks")
-    # tbl_figs = st.sidebar.beta_expander("Tables")
-    # other_figs = st.sidebar.beta_expander("Others")
+    # ts_figs = st.sidebar.expander("Time Series")
+    # net_figs = st.sidebar.expander("Networks")
+    # tbl_figs = st.sidebar.expander("Tables")
+    # other_figs = st.sidebar.expander("Others")
     #     if len(selected_worlds) == 1:
     #         fig_type = st.sidebar.selectbox(label="", options=["Time-series", "Networks", "Tables", "Others"], index=1)
     #     else:
     #         fig_type = st.sidebar.selectbox(label="", options=["Time-series", "Tables", "Others"], index=1)
     #
     #     if fig_type == "Time-series":
     #         runner = display_time_series
@@ -194,15 +228,17 @@
     #         runner = display_tables
     #     elif fig_type == "Others":
     #         runner = display_others
     #     else:
     #         st.text("Please choose what type of figures are you interested in")
     #         return
     products_summary = (
-        products.loc[:, [_ for _ in products.columns if _ not in ("step", "relative_time")]]
+        products.loc[
+            :, [_ for _ in products.columns if _ not in ("step", "relative_time")]
+        ]
         .groupby(["tournament", "world", "product"])
         .agg(["min", "max", "mean", "std"])
     )
     products_summary.columns = [f"{a}_{b}" for a, b in products_summary.columns]
     products_summary = products_summary.reset_index()
     data = dict(t=tournaments, w=worlds, a=agents, p=products_summary)
 
@@ -230,16 +266,18 @@
     for runner, section_name in [
         (display_networks, "Networks"),
         (display_others, "Overview"),
         (display_tables, "Tables"),
         (display_time_series, "Time Series"),
     ]:
         if section_name != "Time Series":
-            expander = st.sidebar.beta_expander(section_name, section_name == "Networks")
-            do_expand = expander.checkbox(f"Show {section_name}", section_name == "Networks")
+            expander = st.sidebar.expander(section_name, section_name == "Networks")
+            do_expand = expander.checkbox(
+                f"Show {section_name}", section_name == "Networks"
+            )
         else:
             expander = st.sidebar
             do_expand = st.sidebar.checkbox(section_name, True)
         if do_expand:
             runner(
                 folder,
                 selected_worlds,
@@ -285,75 +323,102 @@
     gallery,
 ):
     nodes = data["a"].loc[data["a"].world == world, :]
     nodes["score*cost"] = nodes["final_score"] * nodes["cost"]
     fields = [_ for _ in nodes.columns]
     nodes = nodes.to_dict("records")
     added = -data["a"].input_product.min()
-    nlevels = data["a"].input_product.max() + 1 + added
+    nlevels = int(data["a"].input_product.max() + 1 + added)
 
     level_max = [0] * (nlevels)
     dx, dy = 10, 10
     for node in nodes:
-        l = node["input_product"] + added
+        if isnan(node["input_product"]):
+            print(node)
+            continue
+        l = int(node["input_product"] + added)
         node["pos"] = ((l + 1) * dx, level_max[l] * dy)
         level_max[l] += 1
 
     nodes = {n["name"]: n for n in nodes}
     seller_dict = dict(zip(fields, itertools.repeat(float("nan"))))
     buyer_dict = dict(zip(fields, itertools.repeat(float("nan"))))
-    nodes["SELLER"] = {**seller_dict, **dict(pos=(0, dy * (level_max[0] // 2)), name="Seller", type="System")}
+    nodes["SELLER"] = {
+        **seller_dict,
+        **dict(pos=(0, dy * (level_max[0] // 2)), name="Seller", type="System"),
+    }
     nodes["BUYER"] = {
         **buyer_dict,
-        **dict(pos=((nlevels + 1) * dx, dy * (level_max[-1] // 2)), name="Buyer", type="System"),
+        **dict(
+            pos=((nlevels + 1) * dx, dy * (level_max[-1] // 2)),
+            name="Buyer",
+            type="System",
+        ),
     }
     edges, weights = [], []
     weight_field_name = "quantity" if weight_field == "count" else weight_field
     time_cols = (
         [condition_field + "_step", condition_field + "_relative_time"]
         if condition_field != "step"
         else ["step", "relative_time"]
     )
     x = x.loc[x.world == world, [weight_field_name, "seller", "buyer"] + time_cols]
-    x = filter_by_time(x, [condition_field + "_" if condition_field != "step" else ""], selected_steps, selected_times)
+    x = filter_by_time(
+        x,
+        [condition_field + "_" if condition_field != "step" else ""],
+        selected_steps,
+        selected_times,
+    )
     x.drop(time_cols, axis=1, inplace=True)
     if weight_field == "unit_price":
         x = x.groupby(["seller", "buyer"]).mean().reset_index()
         x["unit_price"].fillna(0.0, inplace=True)
     elif weight_field == "count":
         x = x.groupby(["seller", "buyer"]).count().reset_index()
         x.rename(columns=dict(quantity="count"), inplace=True)
     else:
         x = x.groupby(["seller", "buyer"]).sum().reset_index()
     for _, d in x.iterrows():
         edges.append((d["seller"], d["buyer"], d[weight_field]))
     parent.plotly_chart(
         plot_network(
-            fields, nodes, edges=edges, node_weights=node_weight, edge_colors=edge_colors, edge_weights=edge_weights
+            fields,
+            nodes,
+            edges=edges,
+            node_weights=node_weight,
+            edge_colors=edge_colors,
+            edge_weights=edge_weights,
         )
     )
     if gallery:
         return
 
-    col1, col2 = parent.beta_columns(2)
+    col1, col2 = parent.columns(2)
     mydata = data[src]
     myselected = mydata.loc[(mydata.world == world), :]
     myselected = filter_by_time(
-        myselected, [condition_field + "_" if condition_field != "step" else ""], selected_steps, selected_times
+        myselected,
+        [condition_field + "_" if condition_field != "step" else ""],
+        selected_steps,
+        selected_times,
+    )
+    seller = col1.selectbox(
+        "Seller", [""] + sorted(x["seller"].unique()), key=f"seller-{world}"
+    )
+    buyer = col2.selectbox(
+        "Buyer", [""] + sorted(x["buyer"].unique()), key=unique_name(f"seller-{world}")
     )
-    seller = col1.selectbox("Seller", [""] + sorted(x["seller"].unique()), key=f"seller-{world}")
-    buyer = col2.selectbox("Buyer", [""] + sorted(x["buyer"].unique()), key=f"seller-{world}")
     if seller:
         myselected = myselected.loc[(myselected.seller == seller), :]
     if buyer:
         myselected = myselected.loc[(myselected.buyer == buyer), :]
     myselected = myselected.reset_index()
     options = myselected
     if src == "n":
-        col1, col2 = parent.beta_columns(2)
+        col1, col2 = parent.columns(2)
         broken = col1.checkbox("Broken", False, key=f"broken-{world}")
         timedout = col2.checkbox("Timedout", False, key=f"timedout-{world}")
         if not broken:
             options = options.loc[~options.broken, :]
         if not timedout:
             options = options.loc[~options.timedout, :]
 
@@ -373,42 +438,62 @@
                 "executed_step",
                 "negotiation",
             ]
             + (["buyer"] if not buyer else [])
             + (["seller"] if not seller else [])
         )
     elif src == "n":
-        displayed_cols = ["id", "delivery_step", "quantity", "unit_price", "timedout", "broken", "step", "rounds"]
+        displayed_cols = [
+            "id",
+            "delivery_step",
+            "quantity",
+            "unit_price",
+            "timedout",
+            "broken",
+            "step",
+            "rounds",
+        ]
     else:
         return
     parent.dataframe(
         myselected.loc[:, displayed_cols].sort_values(
-            ["signed_step", "delivery_step"] if src == "c" else ["step", "delivery_step"]
+            ["signed_step", "delivery_step"]
+            if src == "c"
+            else ["step", "delivery_step"]
         )
     )
     contract = None
 
     options = filter_by_time(
-        options, [condition_field + "_" if condition_field != "step" else ""], selected_steps, selected_times
+        options,
+        [condition_field + "_" if condition_field != "step" else ""],
+        selected_steps,
+        selected_times,
     )
     if parent.checkbox("Ignore Exogenous", key=f"ignore-exogenous-{world}", value=True):
-        options = options.loc[(options["buyer"] != "BUYER") & (options["seller"] != "SELLER"), :]
+        options = options.loc[
+            (options["buyer"] != "BUYER") & (options["seller"] != "SELLER"), :
+        ]
     if src == "n":
         options = options.loc[:, "id"].values
         if len(options) < 1:
             return
-        neg = parent.selectbox(label="Negotiation", options=options, key=f"negotiationselect-{world}")
+        neg = parent.selectbox(
+            label="Negotiation", options=options, key=f"negotiationselect-{world}"
+        )
     elif src == "c":
         options = options.loc[:, "id"].values
         if len(options) < 1:
             return
         elif len(options) == 1:
             contract = options[0]
         else:
-            contract = parent.selectbox(label="Contract", options=options, key=f"contractselect-{world}")
+            contract = parent.selectbox(
+                label="Contract", options=options, key=f"contractselect-{world}"
+            )
         neg = myselected.loc[myselected["id"] == contract, "negotiation"]
         if len(neg) > 0:
             neg = neg.values[0]
         else:
             neg = None
     else:
         return
@@ -435,20 +520,22 @@
             total_price=neg_info["unit_price"] * neg_info["quantity"],
         )
     else:
         agreement = None
     parent.markdown(f"**Agreement**: {agreement}")
 
     trange = (neg_info["min_delivery_step"], neg_info["max_delivery_step"])
-    c1, c2 = parent.beta_columns(2)
+    c1, c2 = parent.columns(2)
     if trange[1] > trange[0]:
         is_3d = c2.checkbox("3D Graph", key=f"threed-{world}")
     else:
         is_3d = False
-    use_ranges = c1.checkbox("Use issue ranges to set axes", True, key=f"useissueranges-{world}")
+    use_ranges = c1.checkbox(
+        "Use issue ranges to set axes", True, key=f"useissueranges-{world}"
+    )
     qrange = (neg_info["min_quantity"] - 1, neg_info["max_quantity"] + 1)
     urange = (neg_info["min_unit_price"] - 1, neg_info["max_unit_price"] + 1)
     if is_3d:
         fig = go.Figure()
         for i, sender in enumerate(offers["sender"].unique()):
             myoffers = offers.loc[offers["sender"] == sender, :]
             fig.add_trace(
@@ -499,15 +586,15 @@
                     name="Agreement",
                     marker_symbol="star",
                 )
             )
         fig.update_layout(xaxis_title="quantity", yaxis_title="unit_price")
         if use_ranges:
             fig.update_layout(xaxis_range=qrange, yaxis_range=urange)
-    col1, col2 = parent.beta_columns(2)
+    col1, col2 = parent.columns(2)
 
     def fig_1d(y):
         fig = go.Figure()
         for i, sender in enumerate(offers["sender"].unique()):
             myoffers = offers.loc[offers["sender"] == sender, :]
             fig.add_trace(
                 go.Scatter(
@@ -527,15 +614,21 @@
                     mode="markers",
                     marker=dict(size=20),
                     name="Agreement",
                     marker_symbol="star",
                 )
             )
         fig.update_layout(xaxis_title="Round", yaxis_title=y)
-        fig.update_layout(yaxis_range=urange if y == "unit_price" else qrange if y == "quantity" else trange)
+        fig.update_layout(
+            yaxis_range=urange
+            if y == "unit_price"
+            else qrange
+            if y == "quantity"
+            else trange
+        )
         return fig
 
     col1.plotly_chart(fig_1d("quantity"))
     col1.plotly_chart(fig)
     col2.plotly_chart(fig_1d("unit_price"))
     if trange[1] > trange[0]:
         col2.plotly_chart(fig_1d("delivery_step"))
@@ -560,16 +653,18 @@
     global WORLD_INDEX
     max_worlds = parent.number_input("Max. Worlds", 1, None, 4)
 
     if len(selected_worlds) < 1:
         st.write("No worlds selected. Cannot show any networks")
         return
     if len(selected_worlds) > max_worlds:
-        st.write(f"More than {max_worlds} world selected ({len(selected_worlds)}). Will show the first {max_worlds}")
-        cols = st.beta_columns([1, 5, 1, 3])
+        st.write(
+            f"More than {max_worlds} world selected ({len(selected_worlds)}). Will show the first {max_worlds}"
+        )
+        cols = st.columns([1, 5, 1, 3])
         # prev = cols[0].button("<")
         # next = cols[2].button(">")
         # if prev:
         #     WORLD_INDEX = (WORLD_INDEX - max_worlds) % len(selected_worlds)
         # if next:
         #     WORLD_INDEX = (WORLD_INDEX + max_worlds) % len(selected_worlds)
         WORLD_INDEX = cols[1].slider("", 0, len(selected_worlds) - 1, WORLD_INDEX)
@@ -586,37 +681,49 @@
         src = "o"
     x = data[src]
     if x is None:
         st.markdown(f"**{what}** data is **not** available in the logs.")
         return
     gallery = parent.checkbox("Gallery Mode", len(selected_worlds) > 1)
     node_weight_options = sorted(
-        [_ for _ in data["a"].columns if is_numeric_dtype(data["a"][_]) and _ not in ("id", "is_default")]
+        [
+            _
+            for _ in data["a"].columns
+            if is_numeric_dtype(data["a"][_]) and _ not in ("id", "is_default")
+        ]
     )
     default_node_weight = node_weight_options.index("final_score")
     if default_node_weight is None:
         default_node_weight = 0
-    with st.beta_expander("Networks Settings"):
-        cols = st.beta_columns(5 + int(gallery))
-        weight_field = cols[2].selectbox("Edge Weight", ["total_price", "unit_price", "quantity", "count"])
-        node_weight = cols[3].selectbox("Node Weight", ["none"] + node_weight_options, default_node_weight + 1)
+    with st.expander("Networks Settings"):
+        cols = st.columns(5 + int(gallery))
+        weight_field = cols[2].selectbox(
+            "Edge Weight", ["total_price", "unit_price", "quantity", "count"]
+        )
+        node_weight = cols[3].selectbox(
+            "Node Weight", ["none"] + node_weight_options, default_node_weight + 1
+        )
         per_step = cols[0].checkbox("Show one step only")
         edge_weights = cols[0].checkbox("Variable Edge Width", True)
         edge_colors = cols[0].checkbox("Variable Edge Colors", True)
         if per_step:
-            selected_step = cols[1].number_input("Step", selected_steps[0], selected_steps[1], selected_steps[0])
+            selected_step = cols[1].number_input(
+                "Step", selected_steps[0], selected_steps[1], selected_steps[0]
+            )
             selected_steps = [selected_step] * 2
         x["total_price"] = x.quantity * x.unit_price
         options = [_[: -len("_step")] for _ in x.columns if _.endswith("_step")]
         if src != "c":
             options.append("step")
-        condition_field = cols[4].selectbox("Condition", options, 0 if src != "n" else options.index("step"))
+        condition_field = cols[4].selectbox(
+            "Condition", options, 0 if src != "n" else options.index("step")
+        )
     if gallery:
         n_cols = cols[5].number_input("Columns", 1, 5, 2)
-        cols = st.beta_columns(n_cols)
+        cols = st.columns(n_cols)
     else:
         n_cols, cols = 1, [st]
 
     for i, world in enumerate(selected_worlds):
         show_a_world(
             world,
             selected_steps=selected_steps,
@@ -703,43 +810,59 @@
         ("Worlds", "w", False),
         ("Products", "p", False),
         ("Agents", "a", False),
         ("Contracts", "c", True),
         ("Negotiations", "n", True),
         ("Offers", "o", True),
     ):
-
         if data[k] is None or not len(data[k]):
             continue
         if not parent.checkbox(label=lbl, key=f"tbl-{lbl}-c1"):
             continue
         if has_step:
             df = filter_by_time(
-                data[k], ["signed_", "concluded_"] if k == "c" else [""], selected_steps, selected_times
+                data[k],
+                ["signed_", "concluded_"] if k == "c" else [""],
+                selected_steps,
+                selected_times,
             )
         else:
             df = data[k]
         if lbl == "Agents":
-            if st.checkbox("Ignore Default Agents", True, key=f"tbl-{lbl}-ignore-default"):
+            if st.checkbox(
+                "Ignore Default Agents", True, key=f"tbl-{lbl}-ignore-default"
+            ):
                 df = df.loc[~df["is_default"], :]
         elif lbl == "Contracts":
-            if st.checkbox("Ignore Exogenous Contracts", True, key=f"tbl-{lbl}-ignore-exogenous"):
+            if st.checkbox(
+                "Ignore Exogenous Contracts", True, key=f"tbl-{lbl}-ignore-exogenous"
+            ):
                 df = df.loc[df["n_neg_steps"] < 1, :]
         show_table(df)
         st.text(f"{len(df)} records found")
-        cols = st.beta_columns(6)
-        type_ = cols[0].selectbox("Chart", ["Scatter", "Line", "Bar", "Box"], 0, key=f"select-{lbl}-chart")
+        cols = st.columns(6)
+        type_ = cols[0].selectbox(
+            "Chart", ["Scatter", "Line", "Bar", "Box"], 0, key=f"select-{lbl}-chart"
+        )
         x = cols[1].selectbox("x", ["none"] + list(df.columns), key=f"select-{lbl}-x")
         y = m = c = s = "none"
         if x != "none":
-            y = cols[2].selectbox("y", ["none"] + list(df.columns), key=f"select-{lbl}-y")
+            y = cols[2].selectbox(
+                "y", ["none"] + list(df.columns), key=f"select-{lbl}-y"
+            )
             if y != "none":
-                m = cols[3].selectbox("Mark", ["none"] + list(df.columns), key=f"select-{lbl}-mark")
-                c = cols[4].selectbox("Color", ["none"] + list(df.columns), key=f"select-{lbl}-color")
-                s = cols[5].selectbox("Size", ["none"] + list(df.columns), key=f"select-{lbl}-size")
+                m = cols[3].selectbox(
+                    "Mark", ["none"] + list(df.columns), key=f"select-{lbl}-mark"
+                )
+                c = cols[4].selectbox(
+                    "Color", ["none"] + list(df.columns), key=f"select-{lbl}-color"
+                )
+                s = cols[5].selectbox(
+                    "Size", ["none"] + list(df.columns), key=f"select-{lbl}-size"
+                )
                 kwargs = dict(x=x, y=y)
                 if m != "none":
                     kwargs["shape"] = m
                 if s != "none":
                     kwargs["size"] = s
                 if c != "none":
                     kwargs["color"] = c
@@ -756,42 +879,87 @@
     selected_agents,
     selected_types,
     selected_steps,
     selected_times,
     data,
     parent=st.sidebar,
 ):
-    settings = st.beta_expander("Time Series Settings")
+    settings = st.expander("Time Series Settings")
     ncols = settings.number_input("N. Columns", 1, 6, 2)
-    xvar = settings.selectbox("x-variable", ["step", "relative_time"], 1 - int(len(selected_worlds) == 1))
+    xvar = settings.selectbox(
+        "x-variable", ["step", "relative_time"], 1 - int(len(selected_worlds) == 1)
+    )
     dynamic = settings.checkbox("Dynamic Figures", value=True)
     sectioned = settings.checkbox("Figure Sections", True)
     ci_level = settings.selectbox(options=[80, 90, 95], label="CI Level", index=2)
-    world_stats, selected_world_stats, combine_world_stats, overlay_world_stats = add_stats_selector(
+    (
+        world_stats,
+        selected_world_stats,
+        combine_world_stats,
+        overlay_world_stats,
+    ) = add_stats_selector(
         folder,
         "world_stats",
-        [[("world", selected_worlds), ("step", selected_steps), ("relative_time", selected_times)]],
+        [
+            [
+                ("world", selected_worlds),
+                ("step", selected_steps),
+                ("relative_time", selected_times),
+            ]
+        ],
         xvar=xvar,
         label="World Statistics",
         choices=lambda x: [
-            _ for _ in x.columns if _ not in ("name", "world", "name", "tournament", "type", "step", "relative_time")
+            _
+            for _ in x.columns
+            if _
+            not in (
+                "name",
+                "world",
+                "name",
+                "tournament",
+                "type",
+                "step",
+                "relative_time",
+            )
         ],
         default_selector="one",
     )
 
-    product_stats, selected_product_stats, combine_product_stats, overlay_product_stats = add_stats_selector(
+    (
+        product_stats,
+        selected_product_stats,
+        combine_product_stats,
+        overlay_product_stats,
+    ) = add_stats_selector(
         folder,
         "product_stats",
-        [[("product", selected_products), ("step", selected_steps), ("relative_time", selected_times)]],
+        [
+            [
+                ("product", selected_products),
+                ("step", selected_steps),
+                ("relative_time", selected_times),
+            ]
+        ],
         xvar=xvar,
         label="Product Statistics",
         choices=lambda x: [
             _
             for _ in x.columns
-            if _ not in ("name", "world", "name", "tournament", "type", "step", "product", "relative_time")
+            if _
+            not in (
+                "name",
+                "world",
+                "name",
+                "tournament",
+                "type",
+                "step",
+                "product",
+                "relative_time",
+            )
         ],
         default_selector="some",
         default_choice=["trading_price"],
         combine=False,
         overlay=False,
     )
     default_agent_stats = [
@@ -801,52 +969,84 @@
         "inventory_output",
         "balance",
         "assets",
         "spot_market_loss",
         "spot_market_quantity",
     ]
 
-    type_stats, selected_type_stats, combine_type_stats, overlay_type_stats = add_stats_selector(
+    (
+        type_stats,
+        selected_type_stats,
+        combine_type_stats,
+        overlay_type_stats,
+    ) = add_stats_selector(
         folder,
         "agent_stats",
         [
             [
                 ("world", selected_worlds),
                 ("type", selected_types),
                 ("step", selected_steps),
                 ("relative_time", selected_times),
             ]
         ],
         xvar=xvar,
         label="Type Statistics",
         choices=lambda x: [
-            _ for _ in x.columns if _ not in ("name", "world", "name", "tournament", "type", "step", "relative_time")
+            _
+            for _ in x.columns
+            if _
+            not in (
+                "name",
+                "world",
+                "name",
+                "tournament",
+                "type",
+                "step",
+                "relative_time",
+            )
         ],
         key="type",
         default_selector="some" if len(selected_worlds) != 1 else "none",
         default_choice=default_agent_stats if len(selected_worlds) != 1 else None,
         combine=False,
         overlay=False,
     )
 
-    agent_stats, selected_agent_stats, combine_agent_stats, overlay_agent_stats = add_stats_selector(
+    (
+        agent_stats,
+        selected_agent_stats,
+        combine_agent_stats,
+        overlay_agent_stats,
+    ) = add_stats_selector(
         folder,
         "agent_stats",
         [
             [
                 ("world", selected_worlds),
                 ("name", selected_agents),
                 ("step", selected_steps),
                 ("relative_time", selected_times),
             ]
         ],
         xvar=xvar,
         label="Agent Statistics",
         choices=lambda x: [
-            _ for _ in x.columns if _ not in ("name", "world", "name", "tournament", "type", "step", "relative_time")
+            _
+            for _ in x.columns
+            if _
+            not in (
+                "name",
+                "world",
+                "name",
+                "tournament",
+                "type",
+                "step",
+                "relative_time",
+            )
         ],
         default_selector="some" if len(selected_worlds) == 1 else "none",
         default_choice=default_agent_stats if len(selected_worlds) == 1 else None,
         combine=False,
         overlay=False,
     )
 
@@ -872,15 +1072,17 @@
                 ("relative_time", selected_times),
             ],
         ],
         xvar=xvar,
         label="Contract Statistics (World)",
         default_selector="none",
         choices=lambda x: [
-            _ for _ in x.columns if _.endswith("quantity") or _.endswith("count") or _.endswith("price")
+            _
+            for _ in x.columns
+            if _.endswith("quantity") or _.endswith("count") or _.endswith("price")
         ],
         key="world",
     )
 
     (
         contract_stats_type,
         selected_contract_stats_type,
@@ -903,15 +1105,17 @@
                 ("relative_time", selected_times),
             ],
         ],
         xvar=xvar,
         label="Contract Statistics (Types)",
         default_selector="none",
         choices=lambda x: [
-            _ for _ in x.columns if _.endswith("quantity") or _.endswith("count") or _.endswith("price")
+            _
+            for _ in x.columns
+            if _.endswith("quantity") or _.endswith("count") or _.endswith("price")
         ],
         key="type",
     )
     (
         contract_stats_agent,
         selected_contract_stats_agent,
         combine_contract_stats_agent,
@@ -933,21 +1137,27 @@
                 ("relative_time", selected_times),
             ],
         ],
         xvar=xvar,
         label="Contract Statistics (Agents)",
         default_selector="none",
         choices=lambda x: [
-            _ for _ in x.columns if _.endswith("quantity") or _.endswith("count") or _.endswith("price")
+            _
+            for _ in x.columns
+            if _.endswith("quantity") or _.endswith("count") or _.endswith("price")
         ],
         key="name",
     )
 
     def aggregate_contract_stats(stats, ignored_cols):
-        cols = [_ for _ in stats.columns if not any(_.endswith(x) for x in ["price", "quantity", "count"])]
+        cols = [
+            _
+            for _ in stats.columns
+            if not any(_.endswith(x) for x in ["price", "quantity", "count"])
+        ]
         ignored_cols = [_ for _ in cols if _.startswith(ignored_cols)]
         cols = [_ for _ in cols if not _ in ignored_cols]
         allcols = [_ for _ in stats.columns if not _ in ignored_cols]
         # st.text(stats.columns)
         # st.text(allcols)
         # st.text(cols)
         # st.text(len(stats))
@@ -978,15 +1188,17 @@
             ],
             # [("world", selected_worlds), ("seller", selected_agents)],
         ],
         xvar=xvar,
         label="Contract Statistics (Buyer Types)",
         default_selector="none",
         choices=lambda x: [
-            _ for _ in x.columns if _.endswith("quantity") or _.endswith("count") or _.endswith("price")
+            _
+            for _ in x.columns
+            if _.endswith("quantity") or _.endswith("count") or _.endswith("price")
         ],
         key="buyer_type",
     )
     (
         contract_stats_seller_type,
         selected_contract_stats_seller_type,
         combine_contract_stats_seller_type,
@@ -1003,15 +1215,17 @@
                 ("relative_time", selected_times),
             ],
         ],
         xvar=xvar,
         label="Contract Statistics (Seller Types)",
         default_selector="none",
         choices=lambda x: [
-            _ for _ in x.columns if _.endswith("quantity") or _.endswith("count") or _.endswith("price")
+            _
+            for _ in x.columns
+            if _.endswith("quantity") or _.endswith("count") or _.endswith("price")
         ],
         key="seller_type",
     )
     (
         contract_stats_buyer,
         selected_contract_stats_buyer,
         combine_contract_stats_buyer,
@@ -1028,15 +1242,17 @@
             ],
             # [("world", selected_worlds), ("seller", selected_agents)],
         ],
         xvar=xvar,
         label="Contract Statistics (Buyer)",
         default_selector="none",
         choices=lambda x: [
-            _ for _ in x.columns if _.endswith("quantity") or _.endswith("count") or _.endswith("price")
+            _
+            for _ in x.columns
+            if _.endswith("quantity") or _.endswith("count") or _.endswith("price")
         ],
         key="buyer",
     )
 
     (
         contract_stats_seller,
         selected_contract_stats_seller,
@@ -1054,28 +1270,42 @@
                 ("relative_time", selected_times),
             ],
         ],
         xvar=xvar,
         label="Contract Statistics (Seller)",
         default_selector="none",
         choices=lambda x: [
-            _ for _ in x.columns if _.endswith("quantity") or _.endswith("count") or _.endswith("price")
+            _
+            for _ in x.columns
+            if _.endswith("quantity") or _.endswith("count") or _.endswith("price")
         ],
         key="seller",
     )
 
     contract_stats_buyer = aggregate_contract_stats(contract_stats_buyer, "seller")
     contract_stats_seller = aggregate_contract_stats(contract_stats_seller, "buyer")
-    contract_stats_buyer_type = aggregate_contract_stats(contract_stats_buyer, "seller_type")
-    contract_stats_seller_type = aggregate_contract_stats(contract_stats_seller, "buyer_type")
+    contract_stats_buyer_type = aggregate_contract_stats(
+        contract_stats_buyer, "seller_type"
+    )
+    contract_stats_seller_type = aggregate_contract_stats(
+        contract_stats_seller, "buyer_type"
+    )
 
-    contract_stats_agent["agent"] = contract_stats_agent["seller"] + "->" + contract_stats_agent["buyer"]
-    contract_stats_agent["agent_type"] = contract_stats_agent["seller_type"] + "->" + contract_stats_agent["buyer_type"]
-    contract_stats_type["agent"] = contract_stats_type["seller"] + "->" + contract_stats_type["buyer"]
-    contract_stats_type["agent_type"] = contract_stats_type["seller_type"] + "->" + contract_stats_type["buyer_type"]
+    contract_stats_agent["agent"] = (
+        contract_stats_agent["seller"] + "->" + contract_stats_agent["buyer"]
+    )
+    contract_stats_agent["agent_type"] = (
+        contract_stats_agent["seller_type"] + "->" + contract_stats_agent["buyer_type"]
+    )
+    contract_stats_type["agent"] = (
+        contract_stats_type["seller"] + "->" + contract_stats_type["buyer"]
+    )
+    contract_stats_type["agent_type"] = (
+        contract_stats_type["seller_type"] + "->" + contract_stats_type["buyer_type"]
+    )
 
     (
         contract_stats_product,
         selected_contract_stats_product,
         combine_contract_stats_product,
         overlay_contract_stats_product,
     ) = add_stats_selector(
@@ -1095,15 +1325,17 @@
                 ("relative_time", selected_times),
             ],
         ],
         xvar=xvar,
         label="Contract Statistics (Product)",
         default_selector="none",
         choices=lambda x: [
-            _ for _ in x.columns if _.endswith("quantity") or _.endswith("count") or _.endswith("price")
+            _
+            for _ in x.columns
+            if _.endswith("quantity") or _.endswith("count") or _.endswith("price")
         ],
         key="product",
     )
 
     cols, start_col = add_stats_display(
         world_stats,
         selected_world_stats,
@@ -1297,29 +1529,33 @@
     selected_agents,
     selected_types,
     selected_steps,
     selected_times,
     data,
     parent=st.sidebar,
 ):
-    # settings = parent.beta_expander("Settings")
+    # settings = parent.expander("Settings")
     # ncols = settings.number_input("N. Columns", min_value=1, max_value=6)
     if parent.checkbox("Score Distribution", False):
-        score_distribution(selected_worlds, selected_agents, selected_types, data, parent=parent)
+        score_distribution(
+            selected_worlds, selected_agents, selected_types, data, parent=parent
+        )
     if parent.checkbox("Final Score Factors", False):
-        score_factors(selected_worlds, selected_agents, selected_types, data, parent=parent)
+        score_factors(
+            selected_worlds, selected_agents, selected_types, data, parent=parent
+        )
 
 
 if __name__ == "__main__":
     import sys
 
-    from streamlit import cli as stcli
+    from streamlit.web import cli as stcli
 
     folder = None
     if len(sys.argv) > 1:
         folder = Path(sys.argv[1])
 
-    if st._is_running_with_streamlit:
-        main(folder)
-    else:
-        sys.argv = ["streamlit", "run"] + sys.argv
-        sys.exit(stcli.main())
+    # if st._is_running_with_streamlit:
+    main(folder)
+    # else:
+    # sys.argv = ["streamlit", "run"] + sys.argv
+    # sys.exit(stcli.main())
```

### Comparing `scml-vis-0.2.9/src/scml_vis/utils.py` & `scml-vis-0.3.0/src/scml_vis/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 #!/usr/bin/env python
-from pathlib import Path
-from collections import defaultdict
-from pprint import pprint
-from pprint import pformat
 import random
+from collections import defaultdict
+from pathlib import Path
+from pprint import pformat, pprint
+from typing import Callable
+
 import numpy as np
 import pandas as pd
-from matplotlib import pyplot as plt
-import seaborn as sns
-from typing import Callable
-import streamlit as st
-import seaborn as sns
+import plotly as plotly
 import plotly.express as px
 import plotly.graph_objects as go
+import seaborn as sns
 import streamlit as st
-import plotly as plotly
 from matplotlib import pyplot as plt
 
 DEFAULT_CI_LEVEL = 95
 __all__ = [
     "add_selctor",
     "add_stats_selector",
     "add_stats_display_sns",
@@ -28,15 +25,15 @@
     "load_data",
     "plot_netowrk",
     "score_distribution",
     "score_factors",
 ]
 
 
-@st.cache(allow_output_mutation=False)
+@st.cache_resource
 def load_data(folder: Path, name: str):
     file = folder / f"{name}.csv"
     if not file.exists():
         return None
     data = pd.read_csv(file, index_col=None)
     if name == "agents":
         data["is-default"] = data["is_default"].astype(int)
@@ -66,36 +63,40 @@
     content = sorted(content)
     for a, v in zip((all, some, one, none), ("all", "some", "one", "none")):
         if a:
             options.append(v)
             if v == default:
                 indx = len(options) - 1
     parent.text(title)
-    col1, col2 = parent.beta_columns([1, 4])
+    col1, col2 = parent.columns([1, 4])
     if check:
         combine = st.checkbox("Combine", value=default_combine, key=f"{key}_sel_check")
     else:
         combine = False
     if check2:
-        overlay = st.checkbox("Overlay", value=default_overlay, key=f"{key}_sel_overlay")
+        overlay = st.checkbox(
+            "Overlay", value=default_overlay, key=f"{key}_sel_overlay"
+        )
     else:
         overlay = False
     with col1:
         selection_type = st.radio(title, options, index=indx, key=f"{key}_sel_type")
     if selection_type == "none":
         return [], combine, overlay
     if selection_type == "all":
         return content, combine, overlay
     with col2:
         if selection_type == "some":
             if default_choice is not None:
                 default_choice = [_ for _ in default_choice if _ in content]
                 if len(default_choice) == 0:
                     default_choice = content[0] if len(content) > 0 else None
-            selector = st.multiselect("", content, key=f"{key}_multi", default=default_choice)
+            selector = st.multiselect(
+                "", content, key=f"{key}_multi", default=default_choice
+            )
             return selector, combine, overlay
         if default_choice is not None:
             try:
                 indx = content.index(default_choice)
             except ValueError:
                 indx = 0
         else:
@@ -124,16 +125,24 @@
     if filters:
         filtered = None
         for fset in filters:
             x = world_stats.copy()
             for field, values in fset:
                 if len(x) < 1:
                     break
-                if field.endswith("step") or field.endswith("steps") or field.endswith("relative_time"):
-                    x = x.loc[(world_stats[field] >= values[0]) & (world_stats[field] <= values[1]), :]
+                if (
+                    field.endswith("step")
+                    or field.endswith("steps")
+                    or field.endswith("relative_time")
+                ):
+                    x = x.loc[
+                        (world_stats[field] >= values[0])
+                        & (world_stats[field] <= values[1]),
+                        :,
+                    ]
                     continue
                 x = x.loc[world_stats[field].isin(values), :]
             if len(x) > 0:
                 x = x.index
                 if filtered is None:
                     filtered = x
                 else:
@@ -145,15 +154,15 @@
         # world_stats = pd.concat(filtered, ignore_index=False)
 
     if choices is None:
         choices = [_ for _ in world_stats.columns if _ not in ("step", "relative_time")]
     elif isinstance(choices, Callable):
         choices = choices(world_stats)
 
-    world_stats_expander = st.sidebar.beta_expander(label)
+    world_stats_expander = st.sidebar.expander(label)
     with world_stats_expander:
         selected_world_stats, combine_world_stats, overlay_world_stats = add_selector(
             st,
             "",
             choices,
             key=f"{file_name}_{key}",
             none=True,
@@ -203,19 +212,28 @@
     if overlay:
         with cols[(displayed + start_col) % ncols_effective]:
             displayed += 1
             st.pyplot(fig)
     return cols, displayed + start_col
 
 
-def line_with_band(fig, stats, xvar, yvar, color, i, color_val=None, ci_level=DEFAULT_CI_LEVEL):
+def line_with_band(
+    fig, stats, xvar, yvar, color, i, color_val=None, ci_level=DEFAULT_CI_LEVEL
+):
     if color is not None:
         for i, v in enumerate(stats[color].unique()):
             fig = line_with_band(
-                fig, stats.loc[stats[color] == v, :], xvar, yvar, None, i, color_val=v, ci_level=ci_level
+                fig,
+                stats.loc[stats[color] == v, :],
+                xvar,
+                yvar,
+                None,
+                i,
+                color_val=v,
+                ci_level=ci_level,
             )
             fig.update_layout(yaxis_title=yvar)
         return fig
     colors = px.colors.qualitative.Plotly
     if color:
         stats = stats.groupby([xvar, color]).agg(["mean", "std", "count"])
     else:
@@ -228,29 +246,44 @@
         if not f"{base}_std" in stats.columns or not f"{base}_count" in stats.columns:
             stats[f"{base}"] = stats[c]
             stats = stats.drop([c])
             continue
         stats[f"{base}_ci_hi"] = stats[c]
         stats[f"{base}_ci_lo"] = stats[c]
         indx = stats[f"{base}_count"] > 0
-        stats.loc[indx, f"{base}_ci_hi"] = stats.loc[indx, c] + (1 + ci_level / 100.0) * stats.loc[
-            indx, f"{base}_std"
-        ] / stats.loc[indx, f"{base}_count"].apply(np.sqrt)
-        stats.loc[indx, f"{base}_ci_lo"] = stats.loc[indx, c] - (1 + ci_level / 100.0) * stats.loc[
-            indx, f"{base}_std"
-        ] / stats.loc[indx, f"{base}_count"].apply(np.sqrt)
+        stats.loc[indx, f"{base}_ci_hi"] = stats.loc[indx, c] + (
+            1 + ci_level / 100.0
+        ) * stats.loc[indx, f"{base}_std"] / stats.loc[indx, f"{base}_count"].apply(
+            np.sqrt
+        )
+        stats.loc[indx, f"{base}_ci_lo"] = stats.loc[indx, c] - (
+            1 + ci_level / 100.0
+        ) * stats.loc[indx, f"{base}_std"] / stats.loc[indx, f"{base}_count"].apply(
+            np.sqrt
+        )
         stats[f"{base}"] = stats[c]
         stats = stats.drop([c, f"{base}_std", f"{base}_count"], axis=1)
     stats = stats.reset_index()
-    x, y, hi, lo = stats[xvar], stats[f"{yvar}"], stats[f"{yvar}_ci_hi"], stats[f"{yvar}_ci_lo"]
+    x, y, hi, lo = (
+        stats[xvar],
+        stats[f"{yvar}"],
+        stats[f"{yvar}_ci_hi"],
+        stats[f"{yvar}_ci_lo"],
+    )
     if fig is None:
         fig = go.Figure()
     if not isinstance(color_val, str):
         color_val = str(color_val)
-    yname = yvar if not color_val else f"{color_val}:{yvar}" if ":" not in color_val else color_val
+    yname = (
+        yvar
+        if not color_val
+        else f"{color_val}:{yvar}"
+        if ":" not in color_val
+        else color_val
+    )
     fig.add_trace(go.Scatter(x=x, y=y, name=yname, line_color=colors[i % len(colors)]))
     clr = str(tuple(plotly.colors.hex_to_rgb(colors[i % len(colors)]))).replace(" ", "")
     clr = f"rgba{clr[:-1]},0.2)"
     fig.add_trace(
         go.Scatter(
             x=x.tolist() + x[::-1].tolist(),  # x, then x reversed
             y=(hi).tolist() + (lo[::-1]).tolist(),  # upper, then lower reversed
@@ -285,24 +318,34 @@
     # stats = stats.loc[:, allcols]
     if combine:
         stats = stats.loc[:, [_ for _ in stats.columns if _ != hue or _ in selected]]
     # st.text([xvar, hue, selected])
     # st.table(stats.loc[(stats.step==0) & (stats.agent=="03SyR@1->05Dec@1"), :])
     for i, field in enumerate(selected):
         if not overlay:
-            fig = line_with_band(None, stats, xvar, field, color=hue if not combine else None, i=i, ci_level=ci_level)
+            fig = line_with_band(
+                None,
+                stats,
+                xvar,
+                field,
+                color=hue if not combine else None,
+                i=i,
+                ci_level=ci_level,
+            )
             fig.update_layout(showlegend=not combine)
             if combine:
                 fig.update_layout(yaxis_title=field)
             with cols[(i + start_col) % ncols_effective]:
                 displayed += 1
                 st.plotly_chart(fig)
             continue
         col_name = "value" if len(selected) > 1 else field.split(":")[-1]
-        fig = line_with_band(fig, stats, xvar, field, color=None, i=i, ci_level=ci_level)
+        fig = line_with_band(
+            fig, stats, xvar, field, color=None, i=i, ci_level=ci_level
+        )
         fig.update_layout(yaxis_title=col_name)
         fig.update_layout(showlegend=len(selected) > 1 or not combine)
     if overlay:
         with cols[(displayed + start_col) % ncols_effective]:
             displayed += 1
             st.plotly_chart(fig)
     return cols, displayed + start_col
@@ -320,50 +363,54 @@
     start_col=0,
     title=None,
     sectioned=False,
     dynamic=False,
     ci_level=DEFAULT_CI_LEVEL,
 ):
     if "bankrupt" in stats.columns:
-        stats["bankrupt"] = stats.bankrupt.astype(int)
+        stats["bankrupt"] = stats.bankrupt.fillna(0).astype(int)
     add_section = False
     if sectioned:
         start_col, cols = 0, None
         if title:
             add_section = True
     if len(selected) < 1:
         return cols, start_col
     allcols = [xvar] + ([hue] if hue else []) + selected
     stats = stats.loc[:, allcols]
     if add_section:
         st.markdown(f"### {title}")
     if sectioned or cols is None:
-        ncols_effective = max(1, min(len(stats), ncols))
-        cols = st.beta_columns(ncols_effective)
+        ncols_effective = int(max(1, min(len(stats), ncols)))
+        cols = st.columns(ncols_effective)
     else:
         ncols_effective = len(cols)
     displayed = 0
     if overlay and not combine:
         data = stats.loc[:, [hue, xvar] + selected]
         data = data.melt(id_vars=[xvar, hue], value_vars=selected)
         data["variable"] = data[hue].astype(str) + ":" + data["variable"]
         if len(selected) == 1:
             col_name = selected[0].split(":")[-1]
             data = data.rename(columns=dict(value=col_name))
         else:
             col_name = "value"
         if dynamic:
             presenter = st.plotly_chart
-            fig = line_with_band(None, data, xvar, col_name, color="variable", i=0, ci_level=ci_level)
+            fig = line_with_band(
+                None, data, xvar, col_name, color="variable", i=0, ci_level=ci_level
+            )
             fig.update_layout(yaxis_title=col_name)
             fig.update_layout(showlegend=len(selected) > 1 or not combine)
         else:
             presenter = st.pyplot
             fig, ax = plt.subplots()
-            sns.lineplot(data=data, x=xvar, y=col_name, hue="variable", ax=ax, style=None)
+            sns.lineplot(
+                data=data, x=xvar, y=col_name, hue="variable", ax=ax, style=None
+            )
         with cols[(displayed + start_col) % ncols_effective]:
             displayed += 1
             presenter(fig)
         return cols, displayed + start_col
     runner = add_stats_display_plotly if dynamic else add_stats_display_sns
     cols, end_col = runner(
         stats,
@@ -377,15 +424,22 @@
         ncols_effective=ncols_effective,
         ci_level=ci_level,
     )
     return cols, end_col
 
 
 def plot_network(
-    fields, nodes, node_weights=None, color_title=None, edges=[], title="", edge_weights=True, edge_colors=True
+    fields,
+    nodes,
+    node_weights=None,
+    color_title=None,
+    edges=[],
+    title="",
+    edge_weights=True,
+    edge_colors=True,
 ):
     edge_x = []
     edge_y = []
     annotations = []
     min_width, max_width = 1, 7
     weights = []
     colors = []
@@ -403,45 +457,54 @@
         slope = (y1 - y0) / (x1 - x0)
         dx = fraction * (x1 - x0)
         x = x0 + dx
         y = slope * dx + y0
         # x = min(x0, x1) + fraction * (max(x0, x1) - min(x0, x1))
         # y = min(y0, y1) + fraction * (max(y0, y1) - min(y0, y1))
         if edge_colors:
-            clr = tuple([random.randint(0, 255), random.randint(0, 255), random.randint(0, 255)])
+            clr = tuple(
+                [random.randint(0, 255), random.randint(0, 255), random.randint(0, 255)]
+            )
             clr = f"rgb{clr}"
         else:
             clr = "#888"
         annotations.append((x, y, edge[2]))
         weights.append(edge[2])
         colors.append(clr)
 
     if weights and len(weights):
         mn, mx = min(weights), max(weights)
         if mx == mn:
             weights = [1] * len(weights)
         else:
-            weights = [(_ - mn) * (max_width - min_width) / (mx - mn) + min_width for _ in weights]
+            weights = [
+                (_ - mn) * (max_width - min_width) / (mx - mn) + min_width
+                for _ in weights
+            ]
 
     edge_traces = []
     if edge_weights or edge_colors:
         for x, y, w, clr in zip(edge_x, edge_y, weights, colors):
             if np.isnan(w):
                 continue
             # "#888"
             line = dict()
             if edge_colors:
                 line["color"] = clr
             else:
                 line["color"] = "#888"
             if edge_weights:
                 line["width"] = w
-            edge_traces.append(go.Scatter(x=x, y=y, line=line, hoverinfo="text", mode="lines"))
+            edge_traces.append(
+                go.Scatter(x=x, y=y, line=line, hoverinfo="text", mode="lines")
+            )
     else:
-        edge_traces.append(go.Scatter(x=edge_x, y=edge_y, hoverinfo="text", mode="lines"))
+        edge_traces.append(
+            go.Scatter(x=edge_x, y=edge_y, hoverinfo="text", mode="lines")
+        )
 
     node_x = []
     node_y = []
     node_info = []
     node_w = []
     for node in nodes.keys():
         n = nodes[node]
@@ -472,15 +535,19 @@
             #'Reds' | 'Blues' | 'Picnic' | 'Rainbow' | 'Portland' | 'Jet' |
             #'Hot' | 'Blackbody' | 'Earth' | 'Electric' | 'Viridis' |
             # colorscale=plotly.colors.col
             colorscale="plotly3",
             reversescale=True,
             color=node_w,
             size=30,
-            colorbar=dict(thickness=12, title=color_title, xanchor="left", titleside="right") if color_title else None,
+            colorbar=dict(
+                thickness=12, title=color_title, xanchor="left", titleside="right"
+            )
+            if color_title
+            else None,
             line_width=2,
         ),
     )
 
     node_text = []
     for node in nodes:
         node_text.append(str(node))
@@ -501,31 +568,39 @@
             #     xref="paper", yref="paper",
             #     x=0.005, y=-0.002 ) ],
             xaxis=dict(showgrid=False, zeroline=False, showticklabels=False),
             yaxis=dict(showgrid=False, zeroline=False, showticklabels=False),
         ),
     )
 
-    for ((x, y, txt), clr) in zip(annotations, colors):
+    for (x, y, txt), clr in zip(annotations, colors):
         if edge_colors:
-            fig.add_annotation(x=x, y=y, text=txt, showarrow=False, yshift=10, font=dict(color=clr))
+            fig.add_annotation(
+                x=x, y=y, text=txt, showarrow=False, yshift=10, font=dict(color=clr)
+            )
         else:
             fig.add_annotation(x=x, y=y, text=txt, showarrow=False, yshift=10)
     # st.write(st.get_option("theme"))
     return fig
 
 
-def score_distribution(selected_worlds, selected_agents, selected_types, data, parent=st.sidebar):
+def score_distribution(
+    selected_worlds, selected_agents, selected_types, data, parent=st.sidebar
+):
     # st.write(data["a"])
     # st.write(data["a"].groupby(["world", "type", "input_product"])["final_score"].count())
-    expander = st.beta_expander("Score Distribution", True)
-    col1, col2, col3, col4 = expander.beta_columns(4)
+    expander = st.expander("Score Distribution", True)
+    col1, col2, col3, col4 = expander.columns(4)
     is_type = col1.checkbox("Agent Types", value=True, key=f"is_type_check")
-    independent_levels = col2.checkbox("Independent Production Levels", value=True, key=f"is_independent_levels")
-    no_default = col3.checkbox("No Default Agents", value=True, key=f"no_default_agents")
+    independent_levels = col2.checkbox(
+        "Independent Production Levels", value=True, key=f"is_independent_levels"
+    )
+    no_default = col3.checkbox(
+        "No Default Agents", value=True, key=f"no_default_agents"
+    )
     selected = selected_types if is_type else selected_agents
     col = "type" if is_type else "name"
     data = data["a"].loc[
         data["a"].world.isin(selected_worlds),
         [col, "world", "tournament", "final_score", "input_product", "is_default"],
     ]
     if no_default:
@@ -559,34 +634,38 @@
     for (world, agent), score in counts.items():
         for opponent in world_agents[world]:
             if opponent == agent:
                 continue
             count_img[map[agent], map[opponent]] += 1
 
     expander.write("## Scores")
-    col1, col2 = expander.beta_columns(2)
+    col1, col2 = expander.columns(2)
     fig = px.imshow(img, x=agnts, y=agnts)
     col1.plotly_chart(fig)
     col2.plotly_chart(px.bar(data, x="agent", y="final_score"))
 
     expander.write("## Counts")
-    col1, col2 = expander.beta_columns(2)
+    col1, col2 = expander.columns(2)
     fig = px.imshow(count_img, x=agnts, y=agnts)
     col1.plotly_chart(fig)
     scores = data.groupby("agent")["final_score"].count().reset_index()
     scores = scores.rename(columns=dict(final_score="count"))
     col2.plotly_chart(px.bar(scores, x="agent", y="count"))
 
 
-def score_factors(selected_worlds, selected_agents, selected_types, data, parent=st.sidebar):
-    expander = st.beta_expander("Final Score Factors", True)
-    col1, col2, col3 = expander.beta_columns(3)
+def score_factors(
+    selected_worlds, selected_agents, selected_types, data, parent=st.sidebar
+):
+    expander = st.expander("Final Score Factors", True)
+    col1, col2, col3 = expander.columns(3)
     show_counts = col2.checkbox("Show counts only", value=False)
     is_type = col1.checkbox("Agent Types", value=True, key=f"is_type_check_factors")
-    no_default = col3.checkbox("Ignore Default Agents", value=True, key=f"no_default_agents_factors")
+    no_default = col3.checkbox(
+        "Ignore Default Agents", value=True, key=f"no_default_agents_factors"
+    )
     selected = selected_types if is_type else selected_agents
     col = "type" if is_type else "name"
     data = data["a"].loc[data["a"].world.isin(selected_worlds), :]
     data["config"] = data["world"].str.split("_").str[0]
     data["n"] = 1
     target = "final_score" if not show_counts else "n"
     if no_default:
@@ -607,29 +686,52 @@
     if facet_col == "none":
         facet_col = None
     else:
         data = data.sort_values(facet_col)
     factors = expander.selectbox("Factors", cols)
     expander.write(f"**Final score vs {factors}**")
     tbl = (
-        data.groupby(([] if not facet_col else [facet_col]) + ["agent"] + [factors])[target]
+        data.groupby(([] if not facet_col else [facet_col]) + ["agent"] + [factors])[
+            target
+        ]
         .describe()
         .reset_index()
         .set_index("agent" if not facet_col else ["agent", facet_col])
     )
     tbl.reset_index(inplace=True)
     graph_type = expander.selectbox("Graph type", ["Scatter", "Bar", "Box", "Line"])
 
     fig = None
     if graph_type == "Scatter":
-        fig = px.scatter(data, x=factors, y=target, color="agent", facet_col=facet_col, facet_col_wrap=3)
+        fig = px.scatter(
+            data,
+            x=factors,
+            y=target,
+            color="agent",
+            facet_col=facet_col,
+            facet_col_wrap=3,
+        )
     elif graph_type == "Bar":
-        fig = px.bar(data, x=factors, y=target, color="agent", facet_col=facet_col, facet_col_wrap=3)
+        fig = px.bar(
+            data,
+            x=factors,
+            y=target,
+            color="agent",
+            facet_col=facet_col,
+            facet_col_wrap=3,
+        )
     elif graph_type == "Box":
-        fig = px.box(data, x=factors, y=target, color="agent", facet_col=facet_col, facet_col_wrap=3)
+        fig = px.box(
+            data,
+            x=factors,
+            y=target,
+            color="agent",
+            facet_col=facet_col,
+            facet_col_wrap=3,
+        )
     elif graph_type == "Line":
         fig = px.line(
             tbl,
             x=factors,
             y="count" if show_counts else "mean",
             color="agent",
             facet_col=facet_col,
```

### Comparing `scml-vis-0.2.9/src/scml_vis/vendor/quick/LICENSE` & `scml-vis-0.3.0/src/scml_vis/vendor/quick/LICENSE`

 * *Files identical despite different names*

### Comparing `scml-vis-0.2.9/src/scml_vis/vendor/quick/README.md` & `scml-vis-0.3.0/src/scml_vis/vendor/quick/README.md`

 * *Files identical despite different names*

### Comparing `scml-vis-0.2.9/src/scml_vis/vendor/quick/quick.py` & `scml-vis-0.3.0/src/scml_vis/vendor/quick/quick.py`

 * *Files identical despite different names*

### Comparing `scml-vis-0.2.9/setup.py` & `scml-vis-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,127 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: scml-vis
+Version: 0.3.0
+Summary: "A simple visualiser for SCML worlds and tournaments"
+Home-page: https://github.com/yasserfarouk/negmas
+Author-email: yasserfarouk@gmail.com
+License: Apache License 2.0
+Keywords: negotiation,mas,multi-agent,simulation,AI,negmas,scml,scml-agents
+Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+Provides-Extra: dev
+License-File: LICENSE
+
+# scml-vis
+
+[![ci](https://github.com/yasserfarouk/scml-vis/actions/workflows/main.yml/badge.svg)](https://github.com/yasserfarouk/scml-vis/actions/workflows/main.yml)
+[![documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://scml-vis.github.io/scml-vis/)
+[![pypi version](https://img.shields.io/pypi/v/scml-vis.svg)](https://pypi.org/project/scml-vis/)
+[![gitter](https://badges.gitter.im/join%20chat.svg)](https://gitter.im/scml-vis/community)
+
+A simple visualiser for SCML worlds and tournaments.
+You can watch [a demo on YouTube](https://youtu.be/BCDjnnSmIsk)
+[![Alt text](https://img.youtube.com/vi/BCDjnnSmIsk/0.jpg)](https://youtu.be/BCDjnnSmIsk)
+<!-- <iframe width="560" height="315" src="https://www.youtube.com/embed/BCDjnnSmIsk" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> -->
+<!--  -->
+## Screenshots
+![Screen Shot 1](docs/shot1.png)
+![Screen Shot 2](docs/shot2.png)
+
+## Main Features
+
+- Displays any world/tournament run using the [SCML package](https://www.github.com/yasserfarouk/scml)
+- Allows filtering using worlds, agent types, and agent instances
+- Shows world statistics, agent type and instance statistics and contract
+  statistics as functions of simulation step/time
+
+
+## Requirements
+
+- scml-vis requires Python 3.8 or above.
+- scml-vis can visualize worlds created by [scml](https://github.com/yasserfarouk/scml) 0.4.2 or later (simulations created using older versions of scml can be visualized in most cases but are not officially supported).
+
+## Installation
+
+With `pip`:
+```bash
+python3 -m pip install scml-vis
+```
+
+With `pipx`:
+```bash
+python3 -m pip install --user pipx
+pipx install scml-vis
+```
+
+## Usage
+
+The visualizer can be run using any of the following commands:
+```bash
+scmlv
+scmlvis
+scml-vis
+```
+Hereafter we will use the shorter version.
+
+- To visualize any of the recently run worlds and tournaments just run:
+	```bash
+	scmlv show
+	```
+	This will open your browser and allow you to choose a world or a tournament to
+	display.
+	![show without parameters](docs/show.png)
+
+	- If this is the first time you visualize logs in this folder, you will be asked
+	  to compile visualization data
+	  ![compile visualization data](docs/compile.png)
+	- If visualization data is available (or your pressed the `compile visualization data` button), you can now start visualizing the logs
+	  ![compile visualization data](docs/aftercompile.png)
+- To visualize the logs in a specific folder, you can directly pass the folder as in:
+  ```bash
+  scmlv show -f path-to-your-folder
+  ```
+- It is also possible to just compile visualization data without running the visualizer using:
+  ```bash
+  scmlv compile path-to-your-folder
+  ```
+- The visualizer creates a database that it uses to create all the figures you see. You can directly explore this database using:
+  ```bash
+  scmlv explore path-to-your-folder
+  ```
+  This will open a [datasette](https://docs.datasette.io/en/stable/getting_started.html) page allowing you to explore this database
+  ![datasette](docs/datasette.png)
+  This dataset will contain 8 tables describing everything that was logged in the world or tournament. 
+  ![datasette](docs/datasettelarge.png)
+  Please consult [datasette documentation](https://docs.datasette.io/en/stable/getting_started.html) for all the ways you can interact with this dataset.
+
+## Available visualizations
+
+To visualize your logs, you need to follow three steps:
+
+1. Filter the dataset using the `Data Selection` section of the sidebar.
+2. Choose the **family** of figures you would like to show from the `Figure Selection` dropdown in the sidebar. Currently we provide `Time-series`, `Tables` and `others` that are always available as well as `Networks`  that are only available when you visualize a single world or filter the tournament to focus on a single world.
+3. Choose the specific graph you want to see from the family selected in the previous step.
+
+You can watch [a demo of this process here](https://youtu.be/BCDjnnSmIsk)
+
+## TODO List (Good Ideas for PRs)
+
+- ~~Show negotiation logs (i.e. negotiation results)~~
+- ~~Display all contracts (i.e. in a table) based on selection criteria~~
+- ~~Zoom on negotiation details (i.e. exchanged offers)~~
+- ~~Add dynamic figures using plotly/altair~~
+- ~~Add networkx like graphs of contracts / negotiations / offers~~
+- ~~Allow starting the app without specifying a folder.~~
+- ~~Add new figure types that do not have time/step in the x-axis.~~
+- ~~Correcting the placement of weights on edges in network views.~~
+- Adding a graph showing negotiation history in the ufun-space of negotiators (will require a change in the scml package).
+- Add saving and loading of the visualizer's state (i.e. what is visible).
+- Resolving the strange behavior of CI bands in plotly in some cases.
 
-package_dir = \
-{'': 'src'}
 
-packages = \
-['scml_vis', 'scml_vis.vendor', 'scml_vis.vendor.quick']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['PyQt5>=5.15.4,<6.0.0',
- 'click-config-file>=0.6.0,<0.7.0',
- 'click>=7.1.2,<8.0.0',
- 'csvs-to-sqlite>=1.2,<2.0',
- 'datasette-vega>=0.6.2,<0.7.0',
- 'numpy>=1.20.2,<2.0.0',
- 'pandas>=1.2.3,<2.0.0',
- 'plotly>=4.14.3,<5.0.0',
- 'seaborn>=0.11.1,<0.12.0',
- 'streamlit>=0.80.0,<0.81.0',
- 'watchdog>=2.0.2,<3.0.0']
-
-entry_points = \
-{'console_scripts': ['scml-vis = scml_vis.cli:main',
-                     'scmlv = scml_vis.cli:main',
-                     'scmlvis = scml_vis.cli:main']}
-
-setup_kwargs = {
-    'name': 'scml-vis',
-    'version': '0.2.9',
-    'description': 'A simple visualiser for SCML worlds and tournaments',
-    'long_description': '# scml-vis\n\n[![ci](https://github.com/yasserfarouk/scml-vis/actions/workflows/main.yml/badge.svg)](https://github.com/yasserfarouk/scml-vis/actions/workflows/main.yml)\n[![documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://scml-vis.github.io/scml-vis/)\n[![pypi version](https://img.shields.io/pypi/v/scml-vis.svg)](https://pypi.org/project/scml-vis/)\n[![gitter](https://badges.gitter.im/join%20chat.svg)](https://gitter.im/scml-vis/community)\n\nA simple visualiser for SCML worlds and tournaments.\nYou can watch [a demo on YouTube](https://youtu.be/BCDjnnSmIsk)\n[![Alt text](https://img.youtube.com/vi/BCDjnnSmIsk/0.jpg)](https://youtu.be/BCDjnnSmIsk)\n<!-- <iframe width="560" height="315" src="https://www.youtube.com/embed/BCDjnnSmIsk" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> -->\n<!--  -->\n## Screenshots\n![Screen Shot 1](docs/shot1.png)\n![Screen Shot 2](docs/shot2.png)\n\n## Main Features\n\n- Displays any world/tournament run using the [SCML package](https://www.github.com/yasserfarouk/scml)\n- Allows filtering using worlds, agent types, and agent instances\n- Shows world statistics, agent type and instance statistics and contract\n  statistics as functions of simulation step/time\n\n\n## Requirements\n\n- scml-vis requires Python 3.8 or above.\n- scml-vis can visualize worlds created by [scml](https://github.com/yasserfarouk/scml) 0.4.2 or later (simulations created using older versions of scml can be visualized in most cases but are not officially supported).\n\n## Installation\n\nWith `pip`:\n```bash\npython3 -m pip install scml-vis\n```\n\nWith [`pipx`](https://github.com/pipxproject/pipx):\n```bash\npython3 -m pip install --user pipx\n\npipx install scml-vis\n```\n\n## Usage\n\nThe visualizer can be run using any of the following commands:\n```bash\nscmlv\nscmlvis\nscml-vis\n```\nHereafter we will use the shorter version.\n\n- To visualize any of the recently run worlds and tournaments just run:\n\t```bash\n\tscmlv show\n\t```\n\tThis will open your browser and allow you to choose a world or a tournament to\n\tdisplay.\n\t![show without parameters](docs/show.png)\n\n\t- If this is the first time you visualize logs in this folder, you will be asked\n\t  to compile visualization data\n\t\t![compile visualization data](docs/compile.png)\n\t- If visualization data is available (or your pressed the `compile visualization data` button), you can now start visualizing the logs\n\t\t![compile visualization data](docs/aftercompile.png)\n- To visualize the logs in a specific folder, you can directly pass the folder as in:\n  ```bash\n\tscmlv show -f path-to-your-folder\n\t```\n- It is also possible to just compile visualization data without running the visualizer using:\n  ```bash\n\tscmlv compile path-to-your-folder\n\t```\n- The visualizer creates a database that it uses to create all the figures you see. You can directly explore this database using:\n  ```bash\n\tscmlv explore path-to-your-folder\n\t```\n\tThis will open a [datasette](https://docs.datasette.io/en/stable/getting_started.html) page allowing you to explore this database\n\t![datasette](docs/datasette.png)\n\tThis dataset will contain 8 tables describing everything that was logged in the world or tournament. \n\t![datasette](docs/datasettelarge.png)\n\tPlease consult [datasette documentation](https://docs.datasette.io/en/stable/getting_started.html) for all the ways you can interact with this dataset.\n\n## Available visualizations\n\nTo visualize your logs, you need to follow three steps:\n\n1. Filter the dataset using the `Data Selection` section of the sidebar.\n2. Choose the **family** of figures you would like to show from the `Figure Selection` dropdown in the sidebar. Currently we provide `Time-series`, `Tables` and `others` that are always available as well as `Networks`  that are only available when you visualize a single world or filter the tournament to focus on a single world.\n3. Choose the specific graph you want to see from the family selected in the previous step.\n\nYou can watch [a demo of this process here](https://youtu.be/BCDjnnSmIsk)\n\n## TODO List (Good Ideas for PRs)\n\n- ~~Show negotiation logs (i.e. negotiation results)~~\n- ~~Display all contracts (i.e. in a table) based on selection criteria~~\n- ~~Zoom on negotiation details (i.e. exchanged offers)~~\n- ~~Add dynamic figures using plotly/altair~~\n- ~~Add networkx like graphs of contracts / negotiations / offers~~\n- ~~Allow starting the app without specifying a folder.~~\n- ~~Add new figure types that do not have time/step in the x-axis.~~\n- ~~Correcting the placement of weights on edges in network views.~~\n- Adding a graph showing negotiation history in the ufun-space of negotiators (will require a change in the scml package).\n- Add saving and loading of the visualizer\'s state (i.e. what is visible).\n- Resolving the strange behavior of CI bands in plotly in some cases.\n',
-    'author': 'Yasser Mohammad',
-    'author_email': 'yasserfarouk@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/scml-vis/scml-vis',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

### Comparing `scml-vis-0.2.9/PKG-INFO` & `scml-vis-0.3.0/src/scml_vis.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,25 @@
 Metadata-Version: 2.1
 Name: scml-vis
-Version: 0.2.9
-Summary: A simple visualiser for SCML worlds and tournaments
-Home-page: https://github.com/scml-vis/scml-vis
-License: Apache-2.0
-Author: Yasser Mohammad
+Version: 0.3.0
+Summary: "A simple visualiser for SCML worlds and tournaments"
+Home-page: https://github.com/yasserfarouk/negmas
 Author-email: yasserfarouk@gmail.com
-Requires-Python: >=3.8,<4.0
-Classifier: License :: OSI Approved :: Apache Software License
+License: Apache License 2.0
+Keywords: negotiation,mas,multi-agent,simulation,AI,negmas,scml,scml-agents
+Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: PyQt5 (>=5.15.4,<6.0.0)
-Requires-Dist: click (>=7.1.2,<8.0.0)
-Requires-Dist: click-config-file (>=0.6.0,<0.7.0)
-Requires-Dist: csvs-to-sqlite (>=1.2,<2.0)
-Requires-Dist: datasette-vega (>=0.6.2,<0.7.0)
-Requires-Dist: numpy (>=1.20.2,<2.0.0)
-Requires-Dist: pandas (>=1.2.3,<2.0.0)
-Requires-Dist: plotly (>=4.14.3,<5.0.0)
-Requires-Dist: seaborn (>=0.11.1,<0.12.0)
-Requires-Dist: streamlit (>=0.80.0,<0.81.0)
-Requires-Dist: watchdog (>=2.0.2,<3.0.0)
-Project-URL: Repository, https://github.com/scml-vis/scml-vis
-Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+Provides-Extra: dev
+License-File: LICENSE
 
 # scml-vis
 
 [![ci](https://github.com/yasserfarouk/scml-vis/actions/workflows/main.yml/badge.svg)](https://github.com/yasserfarouk/scml-vis/actions/workflows/main.yml)
 [![documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://scml-vis.github.io/scml-vis/)
 [![pypi version](https://img.shields.io/pypi/v/scml-vis.svg)](https://pypi.org/project/scml-vis/)
 [![gitter](https://badges.gitter.im/join%20chat.svg)](https://gitter.im/scml-vis/community)
@@ -57,18 +49,17 @@
 ## Installation
 
 With `pip`:
 ```bash
 python3 -m pip install scml-vis
 ```
 
-With [`pipx`](https://github.com/pipxproject/pipx):
+With `pipx`:
 ```bash
 python3 -m pip install --user pipx
-
 pipx install scml-vis
 ```
 
 ## Usage
 
 The visualizer can be run using any of the following commands:
 ```bash
@@ -84,34 +75,34 @@
 	```
 	This will open your browser and allow you to choose a world or a tournament to
 	display.
 	![show without parameters](docs/show.png)
 
 	- If this is the first time you visualize logs in this folder, you will be asked
 	  to compile visualization data
-		![compile visualization data](docs/compile.png)
+	  ![compile visualization data](docs/compile.png)
 	- If visualization data is available (or your pressed the `compile visualization data` button), you can now start visualizing the logs
-		![compile visualization data](docs/aftercompile.png)
+	  ![compile visualization data](docs/aftercompile.png)
 - To visualize the logs in a specific folder, you can directly pass the folder as in:
   ```bash
-	scmlv show -f path-to-your-folder
-	```
+  scmlv show -f path-to-your-folder
+  ```
 - It is also possible to just compile visualization data without running the visualizer using:
   ```bash
-	scmlv compile path-to-your-folder
-	```
+  scmlv compile path-to-your-folder
+  ```
 - The visualizer creates a database that it uses to create all the figures you see. You can directly explore this database using:
   ```bash
-	scmlv explore path-to-your-folder
-	```
-	This will open a [datasette](https://docs.datasette.io/en/stable/getting_started.html) page allowing you to explore this database
-	![datasette](docs/datasette.png)
-	This dataset will contain 8 tables describing everything that was logged in the world or tournament. 
-	![datasette](docs/datasettelarge.png)
-	Please consult [datasette documentation](https://docs.datasette.io/en/stable/getting_started.html) for all the ways you can interact with this dataset.
+  scmlv explore path-to-your-folder
+  ```
+  This will open a [datasette](https://docs.datasette.io/en/stable/getting_started.html) page allowing you to explore this database
+  ![datasette](docs/datasette.png)
+  This dataset will contain 8 tables describing everything that was logged in the world or tournament. 
+  ![datasette](docs/datasettelarge.png)
+  Please consult [datasette documentation](https://docs.datasette.io/en/stable/getting_started.html) for all the ways you can interact with this dataset.
 
 ## Available visualizations
 
 To visualize your logs, you need to follow three steps:
 
 1. Filter the dataset using the `Data Selection` section of the sidebar.
 2. Choose the **family** of figures you would like to show from the `Figure Selection` dropdown in the sidebar. Currently we provide `Time-series`, `Tables` and `others` that are always available as well as `Networks`  that are only available when you visualize a single world or filter the tournament to focus on a single world.
@@ -129,7 +120,8 @@
 - ~~Allow starting the app without specifying a folder.~~
 - ~~Add new figure types that do not have time/step in the x-axis.~~
 - ~~Correcting the placement of weights on edges in network views.~~
 - Adding a graph showing negotiation history in the ufun-space of negotiators (will require a change in the scml package).
 - Add saving and loading of the visualizer's state (i.e. what is visible).
 - Resolving the strange behavior of CI bands in plotly in some cases.
 
+
```

