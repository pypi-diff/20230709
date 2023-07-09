# Comparing `tmp/target_permutation_importances-1.0.8.tar.gz` & `tmp/target_permutation_importances-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "target_permutation_importances-1.0.8.tar", max compression
+gzip compressed data, was "target_permutation_importances-1.0.9.tar", max compression
```

## Comparing `target_permutation_importances-1.0.8.tar` & `target_permutation_importances-1.0.9.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0     7532 2023-07-03 06:51:37.433254 target_permutation_importances-1.0.8/README.md
--rw-r--r--   0        0        0     1315 2023-07-03 06:51:37.437256 target_permutation_importances-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     7363 2023-07-03 06:51:37.437256 target_permutation_importances-1.0.8/target_permutation_importances/__init__.py
--rw-r--r--   0        0        0     8507 1970-01-01 00:00:00.000000 target_permutation_importances-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-07-04 09:56:55.328432 target_permutation_importances-1.0.9/LICENSE
+-rw-r--r--   0        0        0     8297 2023-07-04 09:56:55.328432 target_permutation_importances-1.0.9/README.md
+-rw-r--r--   0        0        0     1982 2023-07-04 09:56:55.336432 target_permutation_importances-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0    10406 2023-07-04 09:56:55.336432 target_permutation_importances-1.0.9/target_permutation_importances/__init__.py
+-rw-r--r--   0        0        0     9252 1970-01-01 00:00:00.000000 target_permutation_importances-1.0.9/PKG-INFO
```

### Comparing `target_permutation_importances-1.0.8/README.md` & `target_permutation_importances-1.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # Target Permutation Importances
 
-[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/kingychiu/target-permutation-importances)
 [![image](https://img.shields.io/pypi/v/target-permutation-importances.svg)](https://pypi.python.org/pypi/target-permutation-importances)
+[![Downloads](https://static.pepy.tech/badge/target-permutation-importances)](https://pepy.tech/project/target-permutation-importances)
 [![image](https://img.shields.io/pypi/pyversions/target-permutation-importances.svg)](https://pypi.python.org/pypi/target-permutation-importances)
 [![Actions status](https://github.com/kingychiu/target-permutation-importances/workflows/CI/badge.svg)](https://github.com/kingychiu/target-permutation-importances/actions/workflows/main.yaml)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/kingychiu/target-permutation-importances)
 
-[Source & Bug Report](https://github.com/kingychiu/target-permutation-importances)
+[[Source]](https://github.com/kingychiu/target-permutation-importances/)
+[[Bug Report]](https://github.com/kingychiu/target-permutation-importances/issues/)
+[[Documentation]](https://target-permutation-importances.readthedocs.io/en/latest/)
+[[API Reference]](https://target-permutation-importances.readthedocs.io/en/latest/reference/)
 
 ## Overview
 This method aims to lower the feature attribution due to a feature's variance.
 If a feature shows high importance to a model after the target vector is shuffled, it fits the noise.
 
 Overall, this package 
 
 1. Fit the given model class $M$ times to get $M$ actual feature importances of feature f: $A_f = [a_{f_1},a_{f_2}...a_{f_M}]$.
 2. Fit the given model class with shuffled targets for $N$ times to get $N$ feature random importances: $R_f = [r_{f_1},r_{f_2}...r_{f_N}]$.
 3. Compute the final importances of a feature $f$ by various methods, such as:
-    - $A_f$ - $R_f$
-    - $A_f$ / ($R_f + 1)$
+    - $I_f = Avg(A_f) - Avg(R_f)$
+    - $I_f = Avg(A_f) / (Avg(R_f) + 1)$
 
 Not to be confused with [sklearn.inspection.permutation_importance](https://scikit-learn.org/stable/modules/generated/sklearn.inspection.permutation_importance.html#sklearn.inspection.permutation_importance),
 this sklearn method is about feature permutation instead of target permutation.
 
 This method were originally proposed/implemented by:
 - [Permutation importance: a corrected feature importance measure](https://academic.oup.com/bioinformatics/article/26/10/1340/193348)
 - [Feature Selection with Null Importances
@@ -36,18 +40,17 @@
 or
 ```
 poetry add target-permutation-importances
 ```
 
 ## Basic Usage
 
-[Kaggle Notebook](https://www.kaggle.com/code/kingychiu/target-permutation-importances-basic-usage/notebook)
 ```python
 # Import the function
-from target_permutation_importances import compute
+import target_permutation_importances as tpi
 
 # Prepare a dataset
 import pandas as pd
 from sklearn.datasets import load_breast_cancer
 
 # Models
 from catboost import CatBoostClassifier
@@ -57,28 +60,29 @@
 
 data = load_breast_cancer()
 
 # Convert to a pandas dataframe
 Xpd = pd.DataFrame(data.data, columns=data.feature_names)
 
 # Compute permutation importances with default settings
-result_df = compute(
-    model_cls=RandomForestClassifier, # Or other models
-    model_cls_params={ # The params for the model class construction
+result_df = tpi.compute(
+    model_cls=RandomForestClassifier, # The constructor/class of the model.
+    model_cls_params={ # The parameters to pass to the model constructor.
         "n_estimators": 1,
     },
-    model_fit_params={}, # The params for model.fit
-    X=Xpd,
-    y=data.target,
+    model_fit_params={}, # The parameters to pass to the model fit method.
+    X=Xpd, # pd.DataFrame
+    y=data.target, # pd.Series, np.ndarray
     num_actual_runs=2,
     num_random_runs=10,
 )
 
 print(result_df[["feature", "importance"]].sort_values("importance", ascending=False).head())
 ```
+Fork above code from [Kaggle](https://www.kaggle.com/code/kingychiu/target-permutation-importances-basic-usage/notebook).
 
 Outputs:
 ```
 Running 2 actual runs and 10 random runs
 100%|██████████| 2/2 [00:00<00:00, 167.35it/s]
 100%|██████████| 10/10 [00:00<00:00, 163.71it/s]
                 feature  importance
@@ -89,19 +93,19 @@
 26         worst radius    0.008913
 ```
 
 You can find more detailed examples in the "Feature Selection Examples" section.
 
 ## Advance Usage / Customization
 This package exposes `generic_compute` to allow customization.
-Read [`target_permutation_importances.__init__.py`](target_permutation_importances/__init__.py) for details.
+Read [`target_permutation_importances.__init__.py`](https://github.com/kingychiu/target-permutation-importances/target_permutation_importances/__init__.py) for details.
 
 
 ## Feature Selection Examples
-TODO
+- [Feature Selection for Binary Classification](https://www.kaggle.com/code/kingychiu/feature-selection-for-binary-classification-task)
 
 ## Benchmarks
 
 Benchmark has been done with some tabular datasets from the [Tabular data learning benchmark](https://github.com/LeoGrin/tabular-benchmark/tree/main). It is also
 hosted on [Hugging Face](https://huggingface.co/datasets/inria-soda/tabular-benchmark).
 
 The following models with their default params are used in the benchmark:
@@ -117,15 +121,15 @@
 For the binary classification task, `sklearn.metrics.f1_score` is used for evaluation. For the regression task, `sklearn.metrics.mean_squared_error` is used for evaluation.
 
 The downloaded datasets are divided into 3 sections: `train`: 50%, `val`: 10%, `test`: 40%.
 Feature importance is calculated from the `train` set. Feature selection is done on the `val` set. 
 The final benchmark is evaluated on the `test` set. Therefore the `test` set is unseen to both the feature importance and selection process.
 
 
-Raw result data are in [`benchmarks/results/tabular_benchmark.csv`](benchmarks/results/tabular_benchmark.csv).
+Raw result data are in [`benchmarks/results/tabular_benchmark.csv`](https://github.com/kingychiu/target-permutation-importances/benchmarks/results/tabular_benchmark.csv).
 
 ## Kaggle Competitions
 Many Kaggle Competition top solutions involve this method, here are some examples
 
 | Year | Competition                                                                                                                  | Medal | Link                                                                                                                                        |
 | ---- | ---------------------------------------------------------------------------------------------------------------------------- | ----- | ------------------------------------------------------------------------------------------------------------------------------------------- |
 | 2023 | [Predict Student Performance from Game Play](https://www.kaggle.com/competitions/predict-student-performance-from-game-play) | Gold  | [3rd place solution](https://www.kaggle.com/competitions/predict-student-performance-from-game-play/discussion/420235)                      |
```

### Comparing `target_permutation_importances-1.0.8/pyproject.toml` & `target_permutation_importances-1.0.9/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,34 @@
+[project]
+name = "target-permutation-importances"
+version = "1.0.9"
+description = "Compute (Target) Permutation Importances of a machine learning model"
+authors = [{name = "Anthony Chiu", email = "kingychiu@gmail.com"}]
+maintainers = [{name = "Anthony Chiu", email = "kingychiu@gmail.com"}]
+readme = "README.md"
+requires-python = ">=3.8"
+license = {file = "LICENSE.txt"}
+keywords = ["feature selection", "feature ranking", "feature importances", "kaggle", "machine learning"]
+
 [tool.poetry]
 name = "target-permutation-importances"
-version = "1.0.8"
+version = "1.0.9"
 description = "Compute (Target) Permutation Importances of a machine learning model"
 authors = ["Anthony Chiu <kingychiu@gmail.com>"]
+maintainers = ["Anthony Chiu <kingychiu@gmail.com>"]
 readme = "README.md"
 packages = [{include = "target_permutation_importances"}]
 homepage = "https://github.com/kingychiu/target-permutation-importances"
 repository = "https://github.com/kingychiu/target-permutation-importances"
-documentation = "https://github.com/kingychiu/target-permutation-importances"
-keywords = ["feature selection", "feature ranking", "feature importances", "kaggle", "machine learning"]
+documentation = "https://target-permutation-importances.readthedocs.io/en/latest/"
 
 [project.urls]
 Repository = "https://github.com/kingychiu/target-permutation-importances" 
 Homepage = "https://github.com/kingychiu/target-permutation-importances"
-
+Documentation = "https://target-permutation-importances.readthedocs.io/en/latest/"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = "^1.21.0"
 pandas = "^1.5.3"
 tqdm = "^4.48.2"
 
@@ -34,11 +45,19 @@
 pandas-stubs = "^2.0.2.230605"
 types-tqdm = "^4.65.0.1"
 xgboost = "^1.7.6"
 catboost = "^1.2"
 cmake = "^3.26.4"
 lightgbm = "^3.3.5"
 coverage-badge = "^1.1.0"
+twine = "^4.0.2"
+mkdocs = {extras = ["python"], version = "^1.4.3"}
+mkdocstrings = "^0.22.0"
+mkdocstrings-python = "^1.1.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+
+[tool.ruff]
+line-length = 256
```

### Comparing `target_permutation_importances-1.0.8/PKG-INFO` & `target_permutation_importances-1.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 Metadata-Version: 2.1
 Name: target-permutation-importances
-Version: 1.0.8
+Version: 1.0.9
 Summary: Compute (Target) Permutation Importances of a machine learning model
 Home-page: https://github.com/kingychiu/target-permutation-importances
-Keywords: feature selection,feature ranking,feature importances,kaggle,machine learning
 Author: Anthony Chiu
 Author-email: kingychiu@gmail.com
+Maintainer: Anthony Chiu
+Maintainer-email: kingychiu@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.21.0,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: tqdm (>=4.48.2,<5.0.0)
-Project-URL: Documentation, https://github.com/kingychiu/target-permutation-importances
+Project-URL: Documentation, https://target-permutation-importances.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/kingychiu/target-permutation-importances
 Description-Content-Type: text/markdown
 
 # Target Permutation Importances
 
-[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/kingychiu/target-permutation-importances)
 [![image](https://img.shields.io/pypi/v/target-permutation-importances.svg)](https://pypi.python.org/pypi/target-permutation-importances)
+[![Downloads](https://static.pepy.tech/badge/target-permutation-importances)](https://pepy.tech/project/target-permutation-importances)
 [![image](https://img.shields.io/pypi/pyversions/target-permutation-importances.svg)](https://pypi.python.org/pypi/target-permutation-importances)
 [![Actions status](https://github.com/kingychiu/target-permutation-importances/workflows/CI/badge.svg)](https://github.com/kingychiu/target-permutation-importances/actions/workflows/main.yaml)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/kingychiu/target-permutation-importances)
 
-[Source & Bug Report](https://github.com/kingychiu/target-permutation-importances)
+[[Source]](https://github.com/kingychiu/target-permutation-importances/)
+[[Bug Report]](https://github.com/kingychiu/target-permutation-importances/issues/)
+[[Documentation]](https://target-permutation-importances.readthedocs.io/en/latest/)
+[[API Reference]](https://target-permutation-importances.readthedocs.io/en/latest/reference/)
 
 ## Overview
 This method aims to lower the feature attribution due to a feature's variance.
 If a feature shows high importance to a model after the target vector is shuffled, it fits the noise.
 
 Overall, this package 
 
 1. Fit the given model class $M$ times to get $M$ actual feature importances of feature f: $A_f = [a_{f_1},a_{f_2}...a_{f_M}]$.
 2. Fit the given model class with shuffled targets for $N$ times to get $N$ feature random importances: $R_f = [r_{f_1},r_{f_2}...r_{f_N}]$.
 3. Compute the final importances of a feature $f$ by various methods, such as:
-    - $A_f$ - $R_f$
-    - $A_f$ / ($R_f + 1)$
+    - $I_f = Avg(A_f) - Avg(R_f)$
+    - $I_f = Avg(A_f) / (Avg(R_f) + 1)$
 
 Not to be confused with [sklearn.inspection.permutation_importance](https://scikit-learn.org/stable/modules/generated/sklearn.inspection.permutation_importance.html#sklearn.inspection.permutation_importance),
 this sklearn method is about feature permutation instead of target permutation.
 
 This method were originally proposed/implemented by:
 - [Permutation importance: a corrected feature importance measure](https://academic.oup.com/bioinformatics/article/26/10/1340/193348)
 - [Feature Selection with Null Importances
@@ -57,18 +62,17 @@
 or
 ```
 poetry add target-permutation-importances
 ```
 
 ## Basic Usage
 
-[Kaggle Notebook](https://www.kaggle.com/code/kingychiu/target-permutation-importances-basic-usage/notebook)
 ```python
 # Import the function
-from target_permutation_importances import compute
+import target_permutation_importances as tpi
 
 # Prepare a dataset
 import pandas as pd
 from sklearn.datasets import load_breast_cancer
 
 # Models
 from catboost import CatBoostClassifier
@@ -78,28 +82,29 @@
 
 data = load_breast_cancer()
 
 # Convert to a pandas dataframe
 Xpd = pd.DataFrame(data.data, columns=data.feature_names)
 
 # Compute permutation importances with default settings
-result_df = compute(
-    model_cls=RandomForestClassifier, # Or other models
-    model_cls_params={ # The params for the model class construction
+result_df = tpi.compute(
+    model_cls=RandomForestClassifier, # The constructor/class of the model.
+    model_cls_params={ # The parameters to pass to the model constructor.
         "n_estimators": 1,
     },
-    model_fit_params={}, # The params for model.fit
-    X=Xpd,
-    y=data.target,
+    model_fit_params={}, # The parameters to pass to the model fit method.
+    X=Xpd, # pd.DataFrame
+    y=data.target, # pd.Series, np.ndarray
     num_actual_runs=2,
     num_random_runs=10,
 )
 
 print(result_df[["feature", "importance"]].sort_values("importance", ascending=False).head())
 ```
+Fork above code from [Kaggle](https://www.kaggle.com/code/kingychiu/target-permutation-importances-basic-usage/notebook).
 
 Outputs:
 ```
 Running 2 actual runs and 10 random runs
 100%|██████████| 2/2 [00:00<00:00, 167.35it/s]
 100%|██████████| 10/10 [00:00<00:00, 163.71it/s]
                 feature  importance
@@ -110,19 +115,19 @@
 26         worst radius    0.008913
 ```
 
 You can find more detailed examples in the "Feature Selection Examples" section.
 
 ## Advance Usage / Customization
 This package exposes `generic_compute` to allow customization.
-Read [`target_permutation_importances.__init__.py`](target_permutation_importances/__init__.py) for details.
+Read [`target_permutation_importances.__init__.py`](https://github.com/kingychiu/target-permutation-importances/target_permutation_importances/__init__.py) for details.
 
 
 ## Feature Selection Examples
-TODO
+- [Feature Selection for Binary Classification](https://www.kaggle.com/code/kingychiu/feature-selection-for-binary-classification-task)
 
 ## Benchmarks
 
 Benchmark has been done with some tabular datasets from the [Tabular data learning benchmark](https://github.com/LeoGrin/tabular-benchmark/tree/main). It is also
 hosted on [Hugging Face](https://huggingface.co/datasets/inria-soda/tabular-benchmark).
 
 The following models with their default params are used in the benchmark:
@@ -138,15 +143,15 @@
 For the binary classification task, `sklearn.metrics.f1_score` is used for evaluation. For the regression task, `sklearn.metrics.mean_squared_error` is used for evaluation.
 
 The downloaded datasets are divided into 3 sections: `train`: 50%, `val`: 10%, `test`: 40%.
 Feature importance is calculated from the `train` set. Feature selection is done on the `val` set. 
 The final benchmark is evaluated on the `test` set. Therefore the `test` set is unseen to both the feature importance and selection process.
 
 
-Raw result data are in [`benchmarks/results/tabular_benchmark.csv`](benchmarks/results/tabular_benchmark.csv).
+Raw result data are in [`benchmarks/results/tabular_benchmark.csv`](https://github.com/kingychiu/target-permutation-importances/benchmarks/results/tabular_benchmark.csv).
 
 ## Kaggle Competitions
 Many Kaggle Competition top solutions involve this method, here are some examples
 
 | Year | Competition                                                                                                                  | Medal | Link                                                                                                                                        |
 | ---- | ---------------------------------------------------------------------------------------------------------------------------- | ----- | ------------------------------------------------------------------------------------------------------------------------------------------- |
 | 2023 | [Predict Student Performance from Game Play](https://www.kaggle.com/competitions/predict-student-performance-from-game-play) | Gold  | [3rd place solution](https://www.kaggle.com/competitions/predict-student-performance-from-game-play/discussion/420235)                      |
```

