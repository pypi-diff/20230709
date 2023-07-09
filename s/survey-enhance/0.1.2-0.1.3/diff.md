# Comparing `tmp/survey-enhance-0.1.2.tar.gz` & `tmp/survey-enhance-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "survey-enhance-0.1.2.tar", last modified: Fri Mar 31 07:35:17 2023, max compression
+gzip compressed data, was "survey-enhance-0.1.3.tar", last modified: Sun Jul  9 17:44:03 2023, max compression
```

## Comparing `survey-enhance-0.1.2.tar` & `survey-enhance-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 07:35:17.524814 survey-enhance-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-31 07:32:29.000000 survey-enhance-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-31 07:35:17.524814 survey-enhance-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-31 07:32:29.000000 survey-enhance-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 07:35:17.524814 survey-enhance-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-31 07:32:29.000000 survey-enhance-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 07:35:17.524814 survey-enhance-0.1.2/survey_enhance/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-31 07:32:29.000000 survey-enhance-0.1.2/survey_enhance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-03-31 07:32:29.000000 survey-enhance-0.1.2/survey_enhance/impute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-03-31 07:32:29.000000 survey-enhance-0.1.2/survey_enhance/percentile_match.py
--rw-r--r--   0 runner    (1001) docker     (123)    21109 2023-03-31 07:32:29.000000 survey-enhance-0.1.2/survey_enhance/reweight.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 07:35:17.524814 survey-enhance-0.1.2/survey_enhance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-31 07:35:17.000000 survey-enhance-0.1.2/survey_enhance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-03-31 07:35:17.000000 survey-enhance-0.1.2/survey_enhance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 07:35:17.000000 survey-enhance-0.1.2/survey_enhance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-31 07:35:17.000000 survey-enhance-0.1.2/survey_enhance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-31 07:35:17.000000 survey-enhance-0.1.2/survey_enhance.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:44:03.686404 survey-enhance-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-09 17:41:05.000000 survey-enhance-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-09 17:44:03.686404 survey-enhance-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-09 17:41:05.000000 survey-enhance-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 17:44:03.686404 survey-enhance-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-09 17:41:06.000000 survey-enhance-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:44:03.686404 survey-enhance-0.1.3/survey_enhance/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-09 17:41:06.000000 survey-enhance-0.1.3/survey_enhance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-07-09 17:41:06.000000 survey-enhance-0.1.3/survey_enhance/impute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-07-09 17:41:06.000000 survey-enhance-0.1.3/survey_enhance/percentile_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21801 2023-07-09 17:41:06.000000 survey-enhance-0.1.3/survey_enhance/reweight.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:44:03.686404 survey-enhance-0.1.3/survey_enhance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-09 17:44:03.000000 survey-enhance-0.1.3/survey_enhance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-09 17:44:03.000000 survey-enhance-0.1.3/survey_enhance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 17:44:03.000000 survey-enhance-0.1.3/survey_enhance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-09 17:44:03.000000 survey-enhance-0.1.3/survey_enhance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-09 17:44:03.000000 survey-enhance-0.1.3/survey_enhance.egg-info/top_level.txt
```

### Comparing `survey-enhance-0.1.2/LICENSE` & `survey-enhance-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `survey-enhance-0.1.2/setup.py` & `survey-enhance-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="survey-enhance",
-    version="0.1.2",
+    version="0.1.3",
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "microdf_python",
         "torch",
         "policyengine_core",
```

### Comparing `survey-enhance-0.1.2/survey_enhance/impute.py` & `survey-enhance-0.1.3/survey_enhance/impute.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,30 +75,33 @@
             y_ = to_array(Y[Y.columns[i]])
             model = ManyToOneImputation()
             model.encode_categories = self.encode_categories
             model.train(X_, y_, num_trees=num_trees)
             self.models.append(model)
 
     def predict(
-        self, X: pd.DataFrame, mean_quantile: float = 0.5, verbose: bool = False
+        self,
+        X: pd.DataFrame,
+        mean_quantile: float = 0.5,
+        verbose: bool = False,
     ) -> pd.DataFrame:
         """
         Predict the output variables for the input dataset.
 
         Args:
             X (pd.DataFrame): The dataset to predict on.
             mean_quantile (float): The beta parameter for the imputation.
 
         Returns:
             pd.DataFrame: The predicted dataset.
         """
 
         if isinstance(X, list):
             X = pd.DataFrame(X, columns=self.X_columns)
-        
+
         X = pd.DataFrame(X, columns=self.X_columns)
 
         if self.random_generator is None:
             self.random_generator = np.random.default_rng()
         X = to_array(self.encode_categories(X))
         Y = np.zeros((X.shape[0], len(self.models)))
         for i, model in enumerate(self.models):
```

### Comparing `survey-enhance-0.1.2/survey_enhance/percentile_match.py` & `survey-enhance-0.1.3/survey_enhance/percentile_match.py`

 * *Files identical despite different names*

### Comparing `survey-enhance-0.1.2/survey_enhance/reweight.py` & `survey-enhance-0.1.3/survey_enhance/reweight.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,17 @@
 
     diagnostic_tree: Dict[str, float] = None
     """The tree of losses."""
 
     def __init__(
         self,
         dataset: Dataset,
-        calibration_parameters: ParameterNodeAtInstant,
+        calibration_parameters_at_instant: ParameterNodeAtInstant,
+        instant: str = None,
+        calibration_parameters: ParameterNode = None,
         weight: float = None,
         ancestor: "LossCategory" = None,
         static_dataset: bool = None,
         comparison_white_list: List[str] = None,
         comparison_black_list: List[str] = None,
         name: str = None,
         normalise: bool = None,
@@ -56,15 +58,19 @@
         if normalise is not None:
             self.normalise = normalise
 
         if diagnostic is not None:
             self.diagnostic = diagnostic
 
         self.dataset = dataset
+        self.calibration_parameters_at_instant = (
+            calibration_parameters_at_instant
+        )
         self.calibration_parameters = calibration_parameters
+        self.instant = instant
         self.comparison_log = []
         self.initial_loss_value = None
 
         self.comparison_white_list = comparison_white_list
         self.comparison_black_list = comparison_black_list
 
         self.comparisons = None
@@ -84,15 +90,15 @@
             else self.__class__.__name__
         )
 
         self.sublosses = torch.nn.ModuleList(
             [
                 subcategory(
                     dataset,
-                    calibration_parameters,
+                    calibration_parameters_at_instant=calibration_parameters_at_instant,
                     ancestor=self.ancestor,
                     static_dataset=self.static_dataset,
                     comparison_white_list=self.comparison_white_list,
                     comparison_black_list=self.comparison_black_list,
                     name=self.name,
                     diagnostic=self.diagnostic,
                 )
@@ -205,15 +211,15 @@
                 name, y_pred_array, y_true, weight = comparison
             y_pred_array = torch.tensor(
                 np.array(y_pred_array).astype(np.float32), device=device
             )
             y_pred = torch.sum(household_weights * y_pred_array)
             BUFFER = 1e4
             loss_addition = (
-                (y_pred + BUFFER) / (y_true + BUFFER) - 1
+                (((y_pred + BUFFER) / (y_true + BUFFER) - 1))
             ) ** 2 * weight
             if torch.isnan(loss_addition):
                 raise ValueError(
                     f"Loss for {name} is NaN (y_pred={y_pred}, y_true={y_true})"
                 )
             loss = loss + loss_addition
             self.comparison_log.append(
@@ -405,14 +411,15 @@
         self.loss_type = loss_type
         self.calibration_parameters = calibration_parameters
 
     def calibrate(
         self,
         time_instant: str,
         epochs: int = 1_000,
+        min_loss: float = None,
         learning_rate: float = 1e-1,
         validation_split: float = 0.0,
         validation_blacklist: List[str] = None,
         rotate_holdout_sets: bool = False,
         log_dir: str = None,
         tensorboard_log_dir: str = None,
         log_frequency: int = 15,
@@ -420,16 +427,18 @@
     ) -> np.ndarray:
         self.verbose = verbose
         calibration_parameters_at_instant = self.calibration_parameters(
             time_instant
         )
         loss = self.loss_type(
             self.dataset,
-            calibration_parameters_at_instant,
+            calibration_parameters_at_instant=calibration_parameters_at_instant,
             static_dataset=True,
+            instant=time_instant,
+            calibration_parameters=self.calibration_parameters,
         )
 
         if tensorboard_log_dir is not None:
             tensorboard_log_dir = Path(tensorboard_log_dir)
             tensorboard_log_dir.mkdir(parents=True, exist_ok=True)
             writer = SummaryWriter(log_dir=tensorboard_log_dir)
         else:
@@ -477,29 +486,34 @@
                     epochs,
                     learning_rate,
                     log_df,
                     log_dir,
                     writer,
                     log_frequency,
                     i,
+                    min_loss=min_loss,
+                    time_period=time_instant,
                 )
         else:
             weights = self._train(
                 train_loss_fn,
                 validation_loss_fn,
                 epochs,
                 learning_rate,
                 log_df,
                 log_dir,
                 writer,
                 log_frequency,
+                min_loss=min_loss,
+                time_period=time_instant,
             )
 
         if log_dir is not None:
             log_df = train_loss_fn.collect_comparison_log()
+            log_df["time_period"] = time_instant
             log_df.to_csv(log_dir / "log.csv.gz", compression="gzip")
 
         return weights
 
     def _train(
         self,
         training_loss_fn: LossCategory,
@@ -507,35 +521,34 @@
         epochs: int,
         learning_rate: float,
         log_df: pd.DataFrame = None,
         log_dir: Path = None,
         tensorboard_log_writer: SummaryWriter = None,
         log_every: int = 1e6,
         holdout_set_index: int = None,
+        min_loss: float = None,
+        time_period: str = None,
     ) -> np.ndarray:
         household_weights = torch.tensor(
             self.initial_weights.astype(np.float32),
-            requires_grad=False,
-            device=device,
-        )
-        weight_adjustment = torch.tensor(
-            np.ones(len(self.initial_weights)).astype(np.float32),
             requires_grad=True,
             device=device,
         )
-        optimizer = torch.optim.Adam([weight_adjustment], lr=learning_rate)
+        optimizer = torch.optim.Adam([household_weights], lr=learning_rate)
         relu = torch.nn.ReLU()
-
+        if min_loss is not None:
+            epochs = int(1e6)
         for epoch in range(epochs):
             optimizer.zero_grad()
-            loss = training_loss_fn(
-                relu(household_weights + weight_adjustment), self.dataset
-            )
+            loss = training_loss_fn(relu(household_weights), self.dataset)
             loss.backward()
             optimizer.step()
+            if min_loss is not None:
+                if loss.item() < min_loss:
+                    break
             if self.verbose:
                 print(f"Epoch {epoch}: {loss.item()}")
 
             if log_df is not None and (epoch + 1) % log_every == 0:
                 training_log = training_loss_fn.collect_comparison_log()
                 training_log["validation"] = False
                 if holdout_set_index is not None:
@@ -546,14 +559,15 @@
                     )
                     validation_log["validation"] = True
                     if holdout_set_index is not None:
                         validation_log["holdout_set"] = holdout_set_index
                 else:
                     validation_log = pd.DataFrame()
                 log_df = pd.concat([log_df, training_log, validation_log])
+                log_df["time_period"] = time_period
                 log_df.to_csv(
                     log_dir / "calibration_log.csv.gz",
                     index=False,
                     compression="gzip",
                 )
 
                 if tensorboard_log_writer is not None:
@@ -583,8 +597,8 @@
                                 )
                                 tensorboard_log_writer.add_scalar(
                                     f"target/{loss_name}/{validation_status}",
                                     y_true_value,
                                     epoch,
                                 )
 
-        return relu(household_weights + weight_adjustment).detach().cpu().numpy()
+        return relu(household_weights).detach().cpu().numpy()
```

