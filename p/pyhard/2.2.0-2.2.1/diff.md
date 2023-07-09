# Comparing `tmp/pyhard-2.2.0.tar.gz` & `tmp/pyhard-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhard-2.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyhard-2.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyhard-2.2.0.tar` & `pyhard-2.2.1.tar`

### file list

```diff
@@ -1,129 +1,129 @@
--rw-r--r--   0        0        0     8692 2023-07-07 15:38:37.949955 pyhard-2.2.0/README.md
--rw-r--r--   0        0        0     1297 2023-07-07 15:38:38.023956 pyhard-2.2.0/pyhard/__init__.py
--rw-r--r--   0        0        0       66 2023-07-07 15:38:38.023956 pyhard-2.2.0/pyhard/__main__.py
--rw-r--r--   0        0        0    38272 2023-07-07 15:38:38.024956 pyhard-2.2.0/pyhard/app.py
--rw-r--r--   0        0        0    19119 2023-07-07 15:38:38.024956 pyhard-2.2.0/pyhard/base.py
--rw-r--r--   0        0        0    12613 2023-07-07 15:38:38.024956 pyhard-2.2.0/pyhard/classification.py
--rw-r--r--   0        0        0    20574 2023-07-07 15:38:38.024956 pyhard-2.2.0/pyhard/cli.py
--rw-r--r--   0        0        0     5199 2023-07-07 15:38:38.024956 pyhard-2.2.0/pyhard/conf/config.yaml
--rw-r--r--   0        0        0     3469 2023-07-07 15:38:38.024956 pyhard-2.2.0/pyhard/conf/config_old.yaml
--rw-r--r--   0        0        0      703 2023-07-07 15:38:38.024956 pyhard-2.2.0/pyhard/conf/options.json
--rw-r--r--   0        0        0    12210 2023-07-07 15:38:38.024956 pyhard-2.2.0/pyhard/context.py
--rw-r--r--   0        0        0    64554 2023-07-07 15:38:38.025956 pyhard-2.2.0/pyhard/data/2normals/2normals.pdf
--rw-r--r--   0        0        0    39390 2023-07-07 15:38:38.025956 pyhard-2.2.0/pyhard/data/2normals/coordinates.csv
--rw-r--r--   0        0        0    39209 2023-07-07 15:38:38.025956 pyhard-2.2.0/pyhard/data/2normals/data.csv
--rw-r--r--   0        0        0   242683 2023-07-07 15:38:38.026956 pyhard-2.2.0/pyhard/data/2normals/feature_process.csv
--rw-r--r--   0        0        0   168248 2023-07-07 15:38:38.027956 pyhard-2.2.0/pyhard/data/2normals/feature_raw.csv
--rw-r--r--   0        0        0   328455 2023-07-07 15:38:38.028956 pyhard-2.2.0/pyhard/data/2normals/metadata.csv
--rw-r--r--   0        0        0      598 2023-07-07 15:38:38.028956 pyhard-2.2.0/pyhard/data/2normals/options.json
--rw-r--r--   0        0        0    64659 2023-07-07 15:38:38.028956 pyhard-2.2.0/pyhard/data/2normalsSd030/2normals030.pdf
--rw-r--r--   0        0        0    39624 2023-07-07 15:38:38.029956 pyhard-2.2.0/pyhard/data/2normalsSd030/coordinates.csv
--rw-r--r--   0        0        0    38990 2023-07-07 15:38:38.029956 pyhard-2.2.0/pyhard/data/2normalsSd030/data.csv
--rw-r--r--   0        0        0   130100 2023-07-07 15:38:38.029956 pyhard-2.2.0/pyhard/data/2normalsSd030/feature_process.csv
--rw-r--r--   0        0        0    94130 2023-07-07 15:38:38.030956 pyhard-2.2.0/pyhard/data/2normalsSd030/feature_raw.csv
--rw-r--r--   0        0        0   284473 2023-07-07 15:38:38.031956 pyhard-2.2.0/pyhard/data/2normalsSd030/metadata.csv
--rw-r--r--   0        0        0      597 2023-07-07 15:38:38.031956 pyhard-2.2.0/pyhard/data/2normalsSd030/options.json
--rw-r--r--   0        0        0    64807 2023-07-07 15:38:38.031956 pyhard-2.2.0/pyhard/data/2normalsSd045/2normals045.pdf
--rw-r--r--   0        0        0    39780 2023-07-07 15:38:38.031956 pyhard-2.2.0/pyhard/data/2normalsSd045/coordinates.csv
--rw-r--r--   0        0        0    39157 2023-07-07 15:38:38.032956 pyhard-2.2.0/pyhard/data/2normalsSd045/data.csv
--rw-r--r--   0        0        0   178828 2023-07-07 15:38:38.032956 pyhard-2.2.0/pyhard/data/2normalsSd045/feature_process.csv
--rw-r--r--   0        0        0   131886 2023-07-07 15:38:38.033956 pyhard-2.2.0/pyhard/data/2normalsSd045/feature_raw.csv
--rw-r--r--   0        0        0   318453 2023-07-07 15:38:38.034956 pyhard-2.2.0/pyhard/data/2normalsSd045/metadata.csv
--rw-r--r--   0        0        0      597 2023-07-07 15:38:38.034956 pyhard-2.2.0/pyhard/data/2normalsSd045/options.json
--rw-r--r--   0        0        0    15846 2023-07-07 15:38:38.034956 pyhard-2.2.0/pyhard/data/circle/circle.png
--rw-r--r--   0        0        0    39346 2023-07-07 15:38:38.034956 pyhard-2.2.0/pyhard/data/circle/coordinates.csv
--rw-r--r--   0        0        0    40231 2023-07-07 15:38:38.035956 pyhard-2.2.0/pyhard/data/circle/data.csv
--rw-r--r--   0        0        0   226405 2023-07-07 15:38:38.035956 pyhard-2.2.0/pyhard/data/circle/feature_process.csv
--rw-r--r--   0        0        0   145447 2023-07-07 15:38:38.036956 pyhard-2.2.0/pyhard/data/circle/feature_raw.csv
--rw-r--r--   0        0        0   320526 2023-07-07 15:38:38.037956 pyhard-2.2.0/pyhard/data/circle/metadata.csv
--rw-r--r--   0        0        0      595 2023-07-07 15:38:38.037956 pyhard-2.2.0/pyhard/data/circle/options.json
--rw-r--r--   0        0        0    40190 2023-07-07 15:38:38.038956 pyhard-2.2.0/pyhard/data/easy/coordinates.csv
--rw-r--r--   0        0        0    40952 2023-07-07 15:38:38.038956 pyhard-2.2.0/pyhard/data/easy/data.csv
--rw-r--r--   0        0        0   147238 2023-07-07 15:38:38.038956 pyhard-2.2.0/pyhard/data/easy/feature_process.csv
--rw-r--r--   0        0        0    54473 2023-07-07 15:38:38.039956 pyhard-2.2.0/pyhard/data/easy/feature_raw_color.csv
--rw-r--r--   0        0        0   282881 2023-07-07 15:38:38.040956 pyhard-2.2.0/pyhard/data/easy/metadata.csv
--rw-r--r--   0        0        0      595 2023-07-07 15:38:38.040956 pyhard-2.2.0/pyhard/data/easy/options.json
--rw-r--r--   0        0        0    39957 2023-07-07 15:38:38.040956 pyhard-2.2.0/pyhard/data/easy2/coordinates.csv
--rw-r--r--   0        0        0    40817 2023-07-07 15:38:38.040956 pyhard-2.2.0/pyhard/data/easy2/data.csv
--rw-r--r--   0        0        0    42676 2023-07-07 15:38:38.040956 pyhard-2.2.0/pyhard/data/easy2/easy2.png
--rw-r--r--   0        0        0   285261 2023-07-07 15:38:38.042956 pyhard-2.2.0/pyhard/data/easy2/metadata.csv
--rw-r--r--   0        0        0      597 2023-07-07 15:38:38.042956 pyhard-2.2.0/pyhard/data/easy2/options.json
--rw-r--r--   0        0        0      190 2023-07-07 15:38:38.042956 pyhard-2.2.0/pyhard/data/easy2/projection_matrix.csv
--rw-r--r--   0        0        0     5787 2023-07-07 15:38:38.042956 pyhard-2.2.0/pyhard/data/iris/coordinates.csv
--rw-r--r--   0        0        0     3877 2023-07-07 15:38:38.042956 pyhard-2.2.0/pyhard/data/iris/data.csv
--rw-r--r--   0        0        0    42802 2023-07-07 15:38:38.042956 pyhard-2.2.0/pyhard/data/iris/metadata.csv
--rw-r--r--   0        0        0      597 2023-07-07 15:38:38.042956 pyhard-2.2.0/pyhard/data/iris/options.json
--rw-r--r--   0        0        0    39716 2023-07-07 15:38:38.042956 pyhard-2.2.0/pyhard/data/mix/coordinates.csv
--rw-r--r--   0        0        0    40903 2023-07-07 15:38:38.043956 pyhard-2.2.0/pyhard/data/mix/data.csv
--rw-r--r--   0        0        0   193499 2023-07-07 15:38:38.043956 pyhard-2.2.0/pyhard/data/mix/feature_process.csv
--rw-r--r--   0        0        0   144369 2023-07-07 15:38:38.044956 pyhard-2.2.0/pyhard/data/mix/feature_raw.csv
--rw-r--r--   0        0        0   296920 2023-07-07 15:38:38.045956 pyhard-2.2.0/pyhard/data/mix/metadata.csv
--rw-r--r--   0        0        0    66400 2023-07-07 15:38:38.045956 pyhard-2.2.0/pyhard/data/mix/mix.png
--rw-r--r--   0        0        0      597 2023-07-07 15:38:38.045956 pyhard-2.2.0/pyhard/data/mix/options.json
--rw-r--r--   0        0        0    39233 2023-07-07 15:38:38.046956 pyhard-2.2.0/pyhard/data/overlap/coordinates.csv
--rw-r--r--   0        0        0    39752 2023-07-07 15:38:38.046956 pyhard-2.2.0/pyhard/data/overlap/data.csv
--rw-r--r--   0        0        0   321095 2023-07-07 15:38:38.047956 pyhard-2.2.0/pyhard/data/overlap/metadata.csv
--rw-r--r--   0        0        0      598 2023-07-07 15:38:38.047956 pyhard-2.2.0/pyhard/data/overlap/options.json
--rw-r--r--   0        0        0    13099 2023-07-07 15:38:38.047956 pyhard-2.2.0/pyhard/data/overlap/overlap.png
--rw-r--r--   0        0        0    39995 2023-07-07 15:38:38.048956 pyhard-2.2.0/pyhard/data/separate/coordinates.csv
--rw-r--r--   0        0        0    42167 2023-07-07 15:38:38.048956 pyhard-2.2.0/pyhard/data/separate/data.csv
--rw-r--r--   0        0        0   177556 2023-07-07 15:38:38.049956 pyhard-2.2.0/pyhard/data/separate/feature_process.csv
--rw-r--r--   0        0        0   113525 2023-07-07 15:38:38.049956 pyhard-2.2.0/pyhard/data/separate/feature_raw.csv
--rw-r--r--   0        0        0   287283 2023-07-07 15:38:38.050956 pyhard-2.2.0/pyhard/data/separate/metadata.csv
--rw-r--r--   0        0        0      597 2023-07-07 15:38:38.050956 pyhard-2.2.0/pyhard/data/separate/options.json
--rw-r--r--   0        0        0    29361 2023-07-07 15:38:38.050956 pyhard-2.2.0/pyhard/data/wine/algorithm_bin.csv
--rw-r--r--   0        0        0   226327 2023-07-07 15:38:38.051956 pyhard-2.2.0/pyhard/data/wine/algorithm_process.csv
--rw-r--r--   0        0        0   218520 2023-07-07 15:38:38.052956 pyhard-2.2.0/pyhard/data/wine/algorithm_raw.csv
--rw-r--r--   0        0        0    10101 2023-07-07 15:38:38.052956 pyhard-2.2.0/pyhard/data/wine/beta_easy.csv
--rw-r--r--   0        0        0     4375 2023-07-07 15:38:38.052956 pyhard-2.2.0/pyhard/data/wine/config.yaml
--rw-r--r--   0        0        0    69563 2023-07-07 15:38:38.053956 pyhard-2.2.0/pyhard/data/wine/coordinates.csv
--rw-r--r--   0        0        0   100951 2023-07-07 15:38:38.053956 pyhard-2.2.0/pyhard/data/wine/data.csv
--rw-r--r--   0        0        0   163688 2023-07-07 15:38:38.054956 pyhard-2.2.0/pyhard/data/wine/feature_process.csv
--rw-r--r--   0        0        0   163380 2023-07-07 15:38:38.055956 pyhard-2.2.0/pyhard/data/wine/feature_raw.csv
--rw-r--r--   0        0        0       12 2023-07-07 15:38:38.055956 pyhard-2.2.0/pyhard/data/wine/footprint_bagging_best.csv
--rw-r--r--   0        0        0     1634 2023-07-07 15:38:38.055956 pyhard-2.2.0/pyhard/data/wine/footprint_bagging_good.csv
--rw-r--r--   0        0        0      174 2023-07-07 15:38:38.055956 pyhard-2.2.0/pyhard/data/wine/footprint_gradient_boosting_best.csv
--rw-r--r--   0        0        0     1726 2023-07-07 15:38:38.055956 pyhard-2.2.0/pyhard/data/wine/footprint_gradient_boosting_good.csv
--rw-r--r--   0        0        0      720 2023-07-07 15:38:38.055956 pyhard-2.2.0/pyhard/data/wine/footprint_instance_easiness_good.csv
--rw-r--r--   0        0        0       12 2023-07-07 15:38:38.055956 pyhard-2.2.0/pyhard/data/wine/footprint_logistic_regression_best.csv
--rw-r--r--   0        0        0     1696 2023-07-07 15:38:38.055956 pyhard-2.2.0/pyhard/data/wine/footprint_logistic_regression_good.csv
--rw-r--r--   0        0        0       12 2023-07-07 15:38:38.055956 pyhard-2.2.0/pyhard/data/wine/footprint_mlp_best.csv
--rw-r--r--   0        0        0     1663 2023-07-07 15:38:38.055956 pyhard-2.2.0/pyhard/data/wine/footprint_mlp_good.csv
--rw-r--r--   0        0        0      893 2023-07-07 15:38:38.055956 pyhard-2.2.0/pyhard/data/wine/footprint_performance.csv
--rw-r--r--   0        0        0     2760 2023-07-07 15:38:38.055956 pyhard-2.2.0/pyhard/data/wine/footprint_random_forest_best.csv
--rw-r--r--   0        0        0     1903 2023-07-07 15:38:38.055956 pyhard-2.2.0/pyhard/data/wine/footprint_random_forest_good.csv
--rw-r--r--   0        0        0      259 2023-07-07 15:38:38.055956 pyhard-2.2.0/pyhard/data/wine/footprint_svc_linear_best.csv
--rw-r--r--   0        0        0     1434 2023-07-07 15:38:38.055956 pyhard-2.2.0/pyhard/data/wine/footprint_svc_linear_good.csv
--rw-r--r--   0        0        0       12 2023-07-07 15:38:38.055956 pyhard-2.2.0/pyhard/data/wine/footprint_svc_rbf_best.csv
--rw-r--r--   0        0        0     1516 2023-07-07 15:38:38.055956 pyhard-2.2.0/pyhard/data/wine/footprint_svc_rbf_good.csv
--rw-r--r--   0        0        0    10103 2023-07-07 15:38:38.055956 pyhard-2.2.0/pyhard/data/wine/good_algos.csv
--rw-r--r--   0        0        0    37458 2023-07-07 15:38:38.056956 pyhard-2.2.0/pyhard/data/wine/ih.csv
--rw-r--r--   0        0        0   317680 2023-07-07 15:38:38.057956 pyhard-2.2.0/pyhard/data/wine/metadata.csv
--rw-r--r--   0        0        0   522841 2023-07-07 15:38:38.059956 pyhard-2.2.0/pyhard/data/wine/metadata_full.csv
--rw-r--r--   0        0        0   409402 2023-07-07 15:38:38.061956 pyhard-2.2.0/pyhard/data/wine/model.pkl
--rw-r--r--   0        0        0      790 2023-07-07 15:38:38.061956 pyhard-2.2.0/pyhard/data/wine/options.json
--rw-r--r--   0        0        0    10105 2023-07-07 15:38:38.061956 pyhard-2.2.0/pyhard/data/wine/portfolio.csv
--rw-r--r--   0        0        0      231 2023-07-07 15:38:38.061956 pyhard-2.2.0/pyhard/data/wine/projection_matrix.csv
--rw-r--r--   0        0        0    40143 2023-07-07 15:38:38.062956 pyhard-2.2.0/pyhard/data/xor/coordinates.csv
--rw-r--r--   0        0        0    40214 2023-07-07 15:38:38.062956 pyhard-2.2.0/pyhard/data/xor/data.csv
--rw-r--r--   0        0        0   272866 2023-07-07 15:38:38.063956 pyhard-2.2.0/pyhard/data/xor/metadata.csv
--rw-r--r--   0        0        0      598 2023-07-07 15:38:38.064956 pyhard-2.2.0/pyhard/data/xor/options.json
--rw-r--r--   0        0        0      196 2023-07-07 15:38:38.064956 pyhard-2.2.0/pyhard/data/xor/projection_matrix.csv
--rw-r--r--   0        0        0    65163 2023-07-07 15:38:38.064956 pyhard-2.2.0/pyhard/data/xor/xor.pdf
--rw-r--r--   0        0        0     7659 2023-07-07 15:38:38.064956 pyhard-2.2.0/pyhard/feature_selection.py
--rw-r--r--   0        0        0    10144 2023-07-07 15:38:38.066956 pyhard-2.2.0/pyhard/hpo.py
--rw-r--r--   0        0        0    10847 2023-07-07 15:38:38.066956 pyhard-2.2.0/pyhard/integrator.py
--rw-r--r--   0        0        0    43485 2023-07-07 15:38:38.066956 pyhard-2.2.0/pyhard/measures.py
--rw-r--r--   0        0        0     3787 2023-07-07 15:38:38.066956 pyhard-2.2.0/pyhard/metrics.py
--rw-r--r--   0        0        0   157445 2023-07-07 15:38:38.067956 pyhard-2.2.0/pyhard/midia/blobs.svg
--rw-r--r--   0        0        0    11042 2023-07-07 15:38:38.067956 pyhard-2.2.0/pyhard/regression.py
--rw-r--r--   0        0        0     4123 2023-07-07 15:38:38.067956 pyhard-2.2.0/pyhard/structures.py
--rw-r--r--   0        0        0        0 2023-07-07 15:38:38.104956 pyhard-2.2.0/pyhard/thirdparty/__init__.py
--rwxr-xr-x   0        0        0    10787 2023-07-07 15:38:38.068956 pyhard-2.2.0/pyhard/thirdparty/entropy_estimators.py
--rw-r--r--   0        0        0     4948 2023-07-07 15:38:38.068956 pyhard-2.2.0/pyhard/thirdparty/rank_aggregation.py
--rw-r--r--   0        0        0    21966 2023-07-07 15:38:38.068956 pyhard-2.2.0/pyhard/thirdparty/skfeature.py
--rw-r--r--   0        0        0     5221 2023-07-07 15:38:38.068956 pyhard-2.2.0/pyhard/utils.py
--rw-r--r--   0        0        0     2359 2023-07-07 15:38:38.068956 pyhard-2.2.0/pyhard/validator.py
--rw-r--r--   0        0        0    38600 2023-07-07 15:38:38.068956 pyhard-2.2.0/pyhard/visualization.py
--rw-r--r--   0        0        0     1587 2023-07-07 15:38:38.068956 pyhard-2.2.0/pyproject.toml
--rw-r--r--   0        0        0    10287 1970-01-01 00:00:00.000000 pyhard-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     8692 2023-07-09 18:56:33.062388 pyhard-2.2.1/README.md
+-rw-r--r--   0        0        0     1297 2023-07-09 18:56:33.129388 pyhard-2.2.1/pyhard/__init__.py
+-rw-r--r--   0        0        0       66 2023-07-09 18:56:33.129388 pyhard-2.2.1/pyhard/__main__.py
+-rw-r--r--   0        0        0    38272 2023-07-09 18:56:33.129388 pyhard-2.2.1/pyhard/app.py
+-rw-r--r--   0        0        0    19119 2023-07-09 18:56:33.129388 pyhard-2.2.1/pyhard/base.py
+-rw-r--r--   0        0        0    13778 2023-07-09 18:56:33.129388 pyhard-2.2.1/pyhard/classification.py
+-rw-r--r--   0        0        0    20574 2023-07-09 18:56:33.129388 pyhard-2.2.1/pyhard/cli.py
+-rw-r--r--   0        0        0     5429 2023-07-09 18:56:33.129388 pyhard-2.2.1/pyhard/conf/config.yaml
+-rw-r--r--   0        0        0     3469 2023-07-09 18:56:33.129388 pyhard-2.2.1/pyhard/conf/config_old.yaml
+-rw-r--r--   0        0        0      703 2023-07-09 18:56:33.129388 pyhard-2.2.1/pyhard/conf/options.json
+-rw-r--r--   0        0        0    12210 2023-07-09 18:56:33.130389 pyhard-2.2.1/pyhard/context.py
+-rw-r--r--   0        0        0    64554 2023-07-09 18:56:33.130389 pyhard-2.2.1/pyhard/data/2normals/2normals.pdf
+-rw-r--r--   0        0        0    39390 2023-07-09 18:56:33.130389 pyhard-2.2.1/pyhard/data/2normals/coordinates.csv
+-rw-r--r--   0        0        0    39209 2023-07-09 18:56:33.130389 pyhard-2.2.1/pyhard/data/2normals/data.csv
+-rw-r--r--   0        0        0   242683 2023-07-09 18:56:33.131389 pyhard-2.2.1/pyhard/data/2normals/feature_process.csv
+-rw-r--r--   0        0        0   168248 2023-07-09 18:56:33.132388 pyhard-2.2.1/pyhard/data/2normals/feature_raw.csv
+-rw-r--r--   0        0        0   328455 2023-07-09 18:56:33.133389 pyhard-2.2.1/pyhard/data/2normals/metadata.csv
+-rw-r--r--   0        0        0      598 2023-07-09 18:56:33.133389 pyhard-2.2.1/pyhard/data/2normals/options.json
+-rw-r--r--   0        0        0    64659 2023-07-09 18:56:33.133389 pyhard-2.2.1/pyhard/data/2normalsSd030/2normals030.pdf
+-rw-r--r--   0        0        0    39624 2023-07-09 18:56:33.134389 pyhard-2.2.1/pyhard/data/2normalsSd030/coordinates.csv
+-rw-r--r--   0        0        0    38990 2023-07-09 18:56:33.134389 pyhard-2.2.1/pyhard/data/2normalsSd030/data.csv
+-rw-r--r--   0        0        0   130100 2023-07-09 18:56:33.134389 pyhard-2.2.1/pyhard/data/2normalsSd030/feature_process.csv
+-rw-r--r--   0        0        0    94130 2023-07-09 18:56:33.135389 pyhard-2.2.1/pyhard/data/2normalsSd030/feature_raw.csv
+-rw-r--r--   0        0        0   284473 2023-07-09 18:56:33.136389 pyhard-2.2.1/pyhard/data/2normalsSd030/metadata.csv
+-rw-r--r--   0        0        0      597 2023-07-09 18:56:33.136389 pyhard-2.2.1/pyhard/data/2normalsSd030/options.json
+-rw-r--r--   0        0        0    64807 2023-07-09 18:56:33.136389 pyhard-2.2.1/pyhard/data/2normalsSd045/2normals045.pdf
+-rw-r--r--   0        0        0    39780 2023-07-09 18:56:33.136389 pyhard-2.2.1/pyhard/data/2normalsSd045/coordinates.csv
+-rw-r--r--   0        0        0    39157 2023-07-09 18:56:33.136389 pyhard-2.2.1/pyhard/data/2normalsSd045/data.csv
+-rw-r--r--   0        0        0   178828 2023-07-09 18:56:33.137389 pyhard-2.2.1/pyhard/data/2normalsSd045/feature_process.csv
+-rw-r--r--   0        0        0   131886 2023-07-09 18:56:33.138389 pyhard-2.2.1/pyhard/data/2normalsSd045/feature_raw.csv
+-rw-r--r--   0        0        0   318453 2023-07-09 18:56:33.139389 pyhard-2.2.1/pyhard/data/2normalsSd045/metadata.csv
+-rw-r--r--   0        0        0      597 2023-07-09 18:56:33.139389 pyhard-2.2.1/pyhard/data/2normalsSd045/options.json
+-rw-r--r--   0        0        0    15846 2023-07-09 18:56:33.139389 pyhard-2.2.1/pyhard/data/circle/circle.png
+-rw-r--r--   0        0        0    39346 2023-07-09 18:56:33.139389 pyhard-2.2.1/pyhard/data/circle/coordinates.csv
+-rw-r--r--   0        0        0    40231 2023-07-09 18:56:33.139389 pyhard-2.2.1/pyhard/data/circle/data.csv
+-rw-r--r--   0        0        0   226405 2023-07-09 18:56:33.140389 pyhard-2.2.1/pyhard/data/circle/feature_process.csv
+-rw-r--r--   0        0        0   145447 2023-07-09 18:56:33.141389 pyhard-2.2.1/pyhard/data/circle/feature_raw.csv
+-rw-r--r--   0        0        0   320526 2023-07-09 18:56:33.142389 pyhard-2.2.1/pyhard/data/circle/metadata.csv
+-rw-r--r--   0        0        0      595 2023-07-09 18:56:33.142389 pyhard-2.2.1/pyhard/data/circle/options.json
+-rw-r--r--   0        0        0    40190 2023-07-09 18:56:33.142389 pyhard-2.2.1/pyhard/data/easy/coordinates.csv
+-rw-r--r--   0        0        0    40952 2023-07-09 18:56:33.142389 pyhard-2.2.1/pyhard/data/easy/data.csv
+-rw-r--r--   0        0        0   147238 2023-07-09 18:56:33.143389 pyhard-2.2.1/pyhard/data/easy/feature_process.csv
+-rw-r--r--   0        0        0    54473 2023-07-09 18:56:33.143389 pyhard-2.2.1/pyhard/data/easy/feature_raw_color.csv
+-rw-r--r--   0        0        0   282881 2023-07-09 18:56:33.144389 pyhard-2.2.1/pyhard/data/easy/metadata.csv
+-rw-r--r--   0        0        0      595 2023-07-09 18:56:33.144389 pyhard-2.2.1/pyhard/data/easy/options.json
+-rw-r--r--   0        0        0    39957 2023-07-09 18:56:33.144389 pyhard-2.2.1/pyhard/data/easy2/coordinates.csv
+-rw-r--r--   0        0        0    40817 2023-07-09 18:56:33.145389 pyhard-2.2.1/pyhard/data/easy2/data.csv
+-rw-r--r--   0        0        0    42676 2023-07-09 18:56:33.145389 pyhard-2.2.1/pyhard/data/easy2/easy2.png
+-rw-r--r--   0        0        0   285261 2023-07-09 18:56:33.146389 pyhard-2.2.1/pyhard/data/easy2/metadata.csv
+-rw-r--r--   0        0        0      597 2023-07-09 18:56:33.146389 pyhard-2.2.1/pyhard/data/easy2/options.json
+-rw-r--r--   0        0        0      190 2023-07-09 18:56:33.146389 pyhard-2.2.1/pyhard/data/easy2/projection_matrix.csv
+-rw-r--r--   0        0        0     5787 2023-07-09 18:56:33.146389 pyhard-2.2.1/pyhard/data/iris/coordinates.csv
+-rw-r--r--   0        0        0     3877 2023-07-09 18:56:33.146389 pyhard-2.2.1/pyhard/data/iris/data.csv
+-rw-r--r--   0        0        0    42802 2023-07-09 18:56:33.146389 pyhard-2.2.1/pyhard/data/iris/metadata.csv
+-rw-r--r--   0        0        0      597 2023-07-09 18:56:33.146389 pyhard-2.2.1/pyhard/data/iris/options.json
+-rw-r--r--   0        0        0    39716 2023-07-09 18:56:33.147389 pyhard-2.2.1/pyhard/data/mix/coordinates.csv
+-rw-r--r--   0        0        0    40903 2023-07-09 18:56:33.147389 pyhard-2.2.1/pyhard/data/mix/data.csv
+-rw-r--r--   0        0        0   193499 2023-07-09 18:56:33.147389 pyhard-2.2.1/pyhard/data/mix/feature_process.csv
+-rw-r--r--   0        0        0   144369 2023-07-09 18:56:33.148389 pyhard-2.2.1/pyhard/data/mix/feature_raw.csv
+-rw-r--r--   0        0        0   296920 2023-07-09 18:56:33.149389 pyhard-2.2.1/pyhard/data/mix/metadata.csv
+-rw-r--r--   0        0        0    66400 2023-07-09 18:56:33.149389 pyhard-2.2.1/pyhard/data/mix/mix.png
+-rw-r--r--   0        0        0      597 2023-07-09 18:56:33.150389 pyhard-2.2.1/pyhard/data/mix/options.json
+-rw-r--r--   0        0        0    39233 2023-07-09 18:56:33.150389 pyhard-2.2.1/pyhard/data/overlap/coordinates.csv
+-rw-r--r--   0        0        0    39752 2023-07-09 18:56:33.150389 pyhard-2.2.1/pyhard/data/overlap/data.csv
+-rw-r--r--   0        0        0   321095 2023-07-09 18:56:33.151389 pyhard-2.2.1/pyhard/data/overlap/metadata.csv
+-rw-r--r--   0        0        0      598 2023-07-09 18:56:33.151389 pyhard-2.2.1/pyhard/data/overlap/options.json
+-rw-r--r--   0        0        0    13099 2023-07-09 18:56:33.151389 pyhard-2.2.1/pyhard/data/overlap/overlap.png
+-rw-r--r--   0        0        0    39995 2023-07-09 18:56:33.152389 pyhard-2.2.1/pyhard/data/separate/coordinates.csv
+-rw-r--r--   0        0        0    42167 2023-07-09 18:56:33.152389 pyhard-2.2.1/pyhard/data/separate/data.csv
+-rw-r--r--   0        0        0   177556 2023-07-09 18:56:33.152389 pyhard-2.2.1/pyhard/data/separate/feature_process.csv
+-rw-r--r--   0        0        0   113525 2023-07-09 18:56:33.153389 pyhard-2.2.1/pyhard/data/separate/feature_raw.csv
+-rw-r--r--   0        0        0   287283 2023-07-09 18:56:33.154389 pyhard-2.2.1/pyhard/data/separate/metadata.csv
+-rw-r--r--   0        0        0      597 2023-07-09 18:56:33.154389 pyhard-2.2.1/pyhard/data/separate/options.json
+-rw-r--r--   0        0        0    29361 2023-07-09 18:56:33.154389 pyhard-2.2.1/pyhard/data/wine/algorithm_bin.csv
+-rw-r--r--   0        0        0   226327 2023-07-09 18:56:33.155389 pyhard-2.2.1/pyhard/data/wine/algorithm_process.csv
+-rw-r--r--   0        0        0   218520 2023-07-09 18:56:33.156389 pyhard-2.2.1/pyhard/data/wine/algorithm_raw.csv
+-rw-r--r--   0        0        0    10101 2023-07-09 18:56:33.156389 pyhard-2.2.1/pyhard/data/wine/beta_easy.csv
+-rw-r--r--   0        0        0     4375 2023-07-09 18:56:33.156389 pyhard-2.2.1/pyhard/data/wine/config.yaml
+-rw-r--r--   0        0        0    69563 2023-07-09 18:56:33.156389 pyhard-2.2.1/pyhard/data/wine/coordinates.csv
+-rw-r--r--   0        0        0   100951 2023-07-09 18:56:33.157389 pyhard-2.2.1/pyhard/data/wine/data.csv
+-rw-r--r--   0        0        0   163688 2023-07-09 18:56:33.157389 pyhard-2.2.1/pyhard/data/wine/feature_process.csv
+-rw-r--r--   0        0        0   163380 2023-07-09 18:56:33.158389 pyhard-2.2.1/pyhard/data/wine/feature_raw.csv
+-rw-r--r--   0        0        0       12 2023-07-09 18:56:33.158389 pyhard-2.2.1/pyhard/data/wine/footprint_bagging_best.csv
+-rw-r--r--   0        0        0     1634 2023-07-09 18:56:33.158389 pyhard-2.2.1/pyhard/data/wine/footprint_bagging_good.csv
+-rw-r--r--   0        0        0      174 2023-07-09 18:56:33.158389 pyhard-2.2.1/pyhard/data/wine/footprint_gradient_boosting_best.csv
+-rw-r--r--   0        0        0     1726 2023-07-09 18:56:33.158389 pyhard-2.2.1/pyhard/data/wine/footprint_gradient_boosting_good.csv
+-rw-r--r--   0        0        0      720 2023-07-09 18:56:33.158389 pyhard-2.2.1/pyhard/data/wine/footprint_instance_easiness_good.csv
+-rw-r--r--   0        0        0       12 2023-07-09 18:56:33.158389 pyhard-2.2.1/pyhard/data/wine/footprint_logistic_regression_best.csv
+-rw-r--r--   0        0        0     1696 2023-07-09 18:56:33.158389 pyhard-2.2.1/pyhard/data/wine/footprint_logistic_regression_good.csv
+-rw-r--r--   0        0        0       12 2023-07-09 18:56:33.158389 pyhard-2.2.1/pyhard/data/wine/footprint_mlp_best.csv
+-rw-r--r--   0        0        0     1663 2023-07-09 18:56:33.159389 pyhard-2.2.1/pyhard/data/wine/footprint_mlp_good.csv
+-rw-r--r--   0        0        0      893 2023-07-09 18:56:33.159389 pyhard-2.2.1/pyhard/data/wine/footprint_performance.csv
+-rw-r--r--   0        0        0     2760 2023-07-09 18:56:33.159389 pyhard-2.2.1/pyhard/data/wine/footprint_random_forest_best.csv
+-rw-r--r--   0        0        0     1903 2023-07-09 18:56:33.159389 pyhard-2.2.1/pyhard/data/wine/footprint_random_forest_good.csv
+-rw-r--r--   0        0        0      259 2023-07-09 18:56:33.159389 pyhard-2.2.1/pyhard/data/wine/footprint_svc_linear_best.csv
+-rw-r--r--   0        0        0     1434 2023-07-09 18:56:33.159389 pyhard-2.2.1/pyhard/data/wine/footprint_svc_linear_good.csv
+-rw-r--r--   0        0        0       12 2023-07-09 18:56:33.159389 pyhard-2.2.1/pyhard/data/wine/footprint_svc_rbf_best.csv
+-rw-r--r--   0        0        0     1516 2023-07-09 18:56:33.159389 pyhard-2.2.1/pyhard/data/wine/footprint_svc_rbf_good.csv
+-rw-r--r--   0        0        0    10103 2023-07-09 18:56:33.159389 pyhard-2.2.1/pyhard/data/wine/good_algos.csv
+-rw-r--r--   0        0        0    37458 2023-07-09 18:56:33.159389 pyhard-2.2.1/pyhard/data/wine/ih.csv
+-rw-r--r--   0        0        0   317680 2023-07-09 18:56:33.160389 pyhard-2.2.1/pyhard/data/wine/metadata.csv
+-rw-r--r--   0        0        0   522841 2023-07-09 18:56:33.162389 pyhard-2.2.1/pyhard/data/wine/metadata_full.csv
+-rw-r--r--   0        0        0   409402 2023-07-09 18:56:33.164389 pyhard-2.2.1/pyhard/data/wine/model.pkl
+-rw-r--r--   0        0        0      790 2023-07-09 18:56:33.164389 pyhard-2.2.1/pyhard/data/wine/options.json
+-rw-r--r--   0        0        0    10105 2023-07-09 18:56:33.164389 pyhard-2.2.1/pyhard/data/wine/portfolio.csv
+-rw-r--r--   0        0        0      231 2023-07-09 18:56:33.164389 pyhard-2.2.1/pyhard/data/wine/projection_matrix.csv
+-rw-r--r--   0        0        0    40143 2023-07-09 18:56:33.164389 pyhard-2.2.1/pyhard/data/xor/coordinates.csv
+-rw-r--r--   0        0        0    40214 2023-07-09 18:56:33.165389 pyhard-2.2.1/pyhard/data/xor/data.csv
+-rw-r--r--   0        0        0   272866 2023-07-09 18:56:33.166389 pyhard-2.2.1/pyhard/data/xor/metadata.csv
+-rw-r--r--   0        0        0      598 2023-07-09 18:56:33.166389 pyhard-2.2.1/pyhard/data/xor/options.json
+-rw-r--r--   0        0        0      196 2023-07-09 18:56:33.166389 pyhard-2.2.1/pyhard/data/xor/projection_matrix.csv
+-rw-r--r--   0        0        0    65163 2023-07-09 18:56:33.166389 pyhard-2.2.1/pyhard/data/xor/xor.pdf
+-rw-r--r--   0        0        0     7659 2023-07-09 18:56:33.166389 pyhard-2.2.1/pyhard/feature_selection.py
+-rw-r--r--   0        0        0    10144 2023-07-09 18:56:33.168389 pyhard-2.2.1/pyhard/hpo.py
+-rw-r--r--   0        0        0    10919 2023-07-09 18:56:33.168389 pyhard-2.2.1/pyhard/integrator.py
+-rw-r--r--   0        0        0    43485 2023-07-09 18:56:33.168389 pyhard-2.2.1/pyhard/measures.py
+-rw-r--r--   0        0        0     3787 2023-07-09 18:56:33.168389 pyhard-2.2.1/pyhard/metrics.py
+-rw-r--r--   0        0        0   157445 2023-07-09 18:56:33.168389 pyhard-2.2.1/pyhard/midia/blobs.svg
+-rw-r--r--   0        0        0    11042 2023-07-09 18:56:33.169389 pyhard-2.2.1/pyhard/regression.py
+-rw-r--r--   0        0        0     4188 2023-07-09 18:56:33.169389 pyhard-2.2.1/pyhard/structures.py
+-rw-r--r--   0        0        0        0 2023-07-09 18:56:33.209389 pyhard-2.2.1/pyhard/thirdparty/__init__.py
+-rwxr-xr-x   0        0        0    10787 2023-07-09 18:56:33.169389 pyhard-2.2.1/pyhard/thirdparty/entropy_estimators.py
+-rw-r--r--   0        0        0     4948 2023-07-09 18:56:33.169389 pyhard-2.2.1/pyhard/thirdparty/rank_aggregation.py
+-rw-r--r--   0        0        0    21966 2023-07-09 18:56:33.169389 pyhard-2.2.1/pyhard/thirdparty/skfeature.py
+-rw-r--r--   0        0        0     5221 2023-07-09 18:56:33.169389 pyhard-2.2.1/pyhard/utils.py
+-rw-r--r--   0        0        0     2359 2023-07-09 18:56:33.169389 pyhard-2.2.1/pyhard/validator.py
+-rw-r--r--   0        0        0    38600 2023-07-09 18:56:33.169389 pyhard-2.2.1/pyhard/visualization.py
+-rw-r--r--   0        0        0     1579 2023-07-09 18:56:33.170389 pyhard-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0    10279 1970-01-01 00:00:00.000000 pyhard-2.2.1/PKG-INFO
```

### Comparing `pyhard-2.2.0/README.md` & `pyhard-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/__init__.py` & `pyhard-2.2.1/pyhard/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import os
 from pathlib import Path
 from typing import Union
 
 
-__version__ = "2.2.0"
+__version__ = "2.2.1"
 
 
 def get_seed() -> Union[int, None]:
     seed = os.environ.get("PYHARD_SEED")
     if seed is None:
         return seed
     else:
```

### Comparing `pyhard-2.2.0/pyhard/app.py` & `pyhard-2.2.1/pyhard/app.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/base.py` & `pyhard-2.2.1/pyhard/base.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/classification.py` & `pyhard-2.2.1/pyhard/classification.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 
 import inspect
 import logging
 import os
 import sys
 import time
 import warnings
-from typing import Any, Dict, List, Optional, Union, Type, Tuple
+from collections import Counter
+from typing import Any, Dict, List, Literal, Optional, Union, Type, Tuple
 
 import hyperopt
 import numpy as np
 import pandas as pd
 from imblearn.over_sampling import SMOTE
+from imblearn.under_sampling import RandomUnderSampler
 from sklearn.base import ClassifierMixin, RegressorMixin
 from sklearn.calibration import CalibratedClassifierCV
 from sklearn.dummy import DummyClassifier
 from sklearn.ensemble import RandomForestClassifier, GradientBoostingClassifier, BaggingClassifier
 from sklearn.exceptions import ConvergenceWarning
 from sklearn.linear_model import LogisticRegression
 from sklearn.model_selection import StratifiedKFold
@@ -44,14 +46,15 @@
     'gaussian_nb': GaussianNB,
     'logistic_regression': LogisticRegression,
     'dummy': DummyClassifier
 }
 
 _overlap_params = {
     'svc_rbf': {'probability': False, 'kernel': 'rbf'},
+    'svc_linear': {'dual': 'auto'},
     'mlp': {'solver': 'lbfgs'}
 }
 
 
 class ClassifiersPool(LearnersPool):
     """
     Pool of classifiers class.
@@ -100,32 +103,33 @@
         Returns:
             dict: the updated parameters
 
         """
         if new_params is None:
             new_params = _overlap_params.copy()
         else:
-            new_params['svc_rbf'] = {**new_params.get('svc_rbf'), **_overlap_params['svc_rbf']} if \
-                new_params.get('svc_rbf') is not None else _overlap_params['svc_rbf']
-
-            new_params['mlp'] = {**new_params.get('mlp'), **_overlap_params['mlp']} if \
-                new_params.get('mlp') is not None else _overlap_params['mlp']
+            for algo in _overlap_params.keys():
+                new_params[algo] = {
+                    **new_params.get(algo),
+                    **_overlap_params[algo]
+                } if new_params.get(algo) is not None else _overlap_params[algo]
 
         return new_params
 
     def run(
             self,
             algo: Union[Type[ClassifierMixin], Type[RegressorMixin]],
             metric: str = 'logloss',
             n_folds: int = 10,
             n_iter: int = 10,
             hyper_param_optm: bool = False,
             hpo_evals: int = 100,
             hpo_timeout: int = 90,
             hpo_name: str = None,
+            resampling: Literal['under', 'over', 'no'] = 'over',
             verbose: bool = False,
             **kwargs
     ) -> Tuple[np.ndarray, np.ndarray]:
         """
         Evaluates the performance obtained in each instance. A cross-validation score, with `n_folds` folds, is
         estimated `n_iter` times for each instance, and the mean value is then computed at the end. During training,
         hyperparameter optimization may be performed optionally.
@@ -136,14 +140,15 @@
             n_folds (int): number of cross-validation folds for evaluating algorithm performance
             n_iter (int): number of times the cross-validation is repeated. Instance metric is the mean over the
                 iterations
             hyper_param_optm (bool): enables HPO (default False)
             hpo_evals (int): maximum number of evaluations
             hpo_timeout (int): timeout (seconds) for a single classifier HPO
             hpo_name (str): see ``algo_list`` in ``config.yaml``
+            resampling (str): resampling strategy used for imbalanced datasets during cross-validation
             verbose (bool): turn verbose mode on
             **kwargs: fixed classifier parameters, which won't be optimized
 
         Returns:
             tuple of numpy.ndarrray: Array of scores per instance, and array of probabilities per instance
 
         """
@@ -182,16 +187,24 @@
                 self.logger.info(f"Evaluating testing fold #{k}")
 
                 X_train_ = self.X[train_index, :]
                 y_train = self.y[train_index]
                 X_test_ = self.X[test_index, :]
 
                 if imbalanced:
-                    self.logger.info("Over-sampling training fold with SMOTE")
-                    X_train_, y_train = SMOTE().fit_resample(X_train_, y_train)
+                    if resampling == 'over':
+                        self.logger.info("Over-sampling training fold with SMOTE")
+                        self.logger.debug("Original training fold shape %s" % Counter(y_train))
+                        X_train_, y_train = SMOTE().fit_resample(X_train_, y_train)
+                        self.logger.debug("Resampled training fold shape %s" % Counter(y_train))
+                    elif resampling == 'under':
+                        self.logger.info("Under-sampling training fold with SMOTE")
+                        self.logger.debug("Original training fold shape %s" % Counter(y_train))
+                        X_train_, y_train = RandomUnderSampler().fit_resample(X_train_, y_train)
+                        self.logger.debug("Resampled training fold shape %s" % Counter(y_train))
 
                 self.logger.debug("Normalizing values with standard scaler")
                 scaler = StandardScaler()
                 X_train = scaler.fit_transform(X_train_)
                 X_test = scaler.transform(X_test_)
 
                 if hyper_param_optm:
@@ -249,29 +262,31 @@
     def run_all(
             self,
             metric: str = 'logloss',
             n_folds: int = 10,
             n_iter: int = 10,
             algo_list: Optional[List[str]] = None,
             parameters: Optional[Dict[str, Any]] = None,
+            resampling: Literal['under', 'over', 'no'] = 'over',
             hyper_param_optm: bool = False,
             hpo_evals: int = 100,
             hpo_timeout: int = 90,
             verbose: bool = False
     ) -> pd.DataFrame:
         """
         Wrapper function that runs all the classifiers in the dataset.
 
         Args:
             metric (str): performance metric (default `logloss`)
             n_folds (int): number of cross-validation folds for evaluating algorithm performance
             n_iter (int): number of times the cross-validation is repeated. Instance metric is the mean over the
                 iterations
-            algo_list (list, optional):
-            parameters (dict, optional):
+            algo_list (list, optional): list of algorithms in the pool
+            parameters (dict, optional): dictionary with specific parametrization for the algorithms
+            resampling (str): resampling strategy used for imbalanced datasets during cross-validation
             hyper_param_optm (bool): enables hyperparameter optimization (HPO) (default False)
             hpo_evals (int): maximum number of evaluations
             hpo_timeout (int): timeout (seconds) for a single classifier HPO
             verbose (bool): turn verbose mode on
 
         Returns:
             pd.DataFrame: An `(n_instances, n_classifiers)` dataframe with classifiers performance by instance
@@ -307,14 +322,15 @@
                 metric=metric,
                 n_folds=n_folds,
                 n_iter=n_iter,
                 hyper_param_optm=hyper_param_optm,
                 hpo_evals=hpo_evals,
                 hpo_timeout=hpo_timeout,
                 hpo_name=name,
+                resampling=resampling,
                 verbose=verbose,
                 **algo_params
             )
 
         df_result = pd.DataFrame(result)
 
         warnings.resetwarnings()
```

### Comparing `pyhard-2.2.0/pyhard/cli.py` & `pyhard-2.2.1/pyhard/cli.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/conf/config.yaml` & `pyhard-2.2.1/pyhard/conf/config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -134,14 +134,19 @@
     n_iter: 1
 
     # score metric used to evaluate instance performance
     # either 'logloss' (recommended) or 'brier' for classification
     # either 'normalized_absolute_error' (recommended) or 'normalized_squared_error' for regression
     metric: logloss
 
+    # sampling strategy used for imbalanced datasets
+    # during cross-validation, each training fold is resampled accordingly
+    # possible strategies are: 'over', 'under', or 'no' (no attempt to balance)
+    resampling: over
+
     # which algorithms (classifiers) to use
     pool:
         # classifiers
         - svc_linear
         - svc_rbf
         - random_forest
         - gradient_boosting
```

### Comparing `pyhard-2.2.0/pyhard/conf/config_old.yaml` & `pyhard-2.2.1/pyhard/conf/config_old.yaml`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/conf/options.json` & `pyhard-2.2.1/pyhard/conf/options.json`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/context.py` & `pyhard-2.2.1/pyhard/context.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/2normals/2normals.pdf` & `pyhard-2.2.1/pyhard/data/2normals/2normals.pdf`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/2normals/coordinates.csv` & `pyhard-2.2.1/pyhard/data/2normals/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/2normals/data.csv` & `pyhard-2.2.1/pyhard/data/2normals/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/2normals/feature_process.csv` & `pyhard-2.2.1/pyhard/data/2normals/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/2normals/feature_raw.csv` & `pyhard-2.2.1/pyhard/data/2normals/feature_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/2normals/metadata.csv` & `pyhard-2.2.1/pyhard/data/2normals/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/2normals/options.json` & `pyhard-2.2.1/pyhard/data/2normals/options.json`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/2normalsSd030/2normals030.pdf` & `pyhard-2.2.1/pyhard/data/2normalsSd030/2normals030.pdf`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/2normalsSd030/coordinates.csv` & `pyhard-2.2.1/pyhard/data/2normalsSd030/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/2normalsSd030/data.csv` & `pyhard-2.2.1/pyhard/data/2normalsSd030/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/2normalsSd030/feature_process.csv` & `pyhard-2.2.1/pyhard/data/2normalsSd030/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/2normalsSd030/feature_raw.csv` & `pyhard-2.2.1/pyhard/data/2normalsSd030/feature_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/2normalsSd030/metadata.csv` & `pyhard-2.2.1/pyhard/data/2normalsSd030/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/2normalsSd030/options.json` & `pyhard-2.2.1/pyhard/data/2normalsSd030/options.json`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/2normalsSd045/2normals045.pdf` & `pyhard-2.2.1/pyhard/data/2normalsSd045/2normals045.pdf`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/2normalsSd045/coordinates.csv` & `pyhard-2.2.1/pyhard/data/2normalsSd045/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/2normalsSd045/data.csv` & `pyhard-2.2.1/pyhard/data/2normalsSd045/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/2normalsSd045/feature_process.csv` & `pyhard-2.2.1/pyhard/data/2normalsSd045/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/2normalsSd045/feature_raw.csv` & `pyhard-2.2.1/pyhard/data/2normalsSd045/feature_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/2normalsSd045/metadata.csv` & `pyhard-2.2.1/pyhard/data/2normalsSd045/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/2normalsSd045/options.json` & `pyhard-2.2.1/pyhard/data/2normalsSd045/options.json`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/circle/circle.png` & `pyhard-2.2.1/pyhard/data/circle/circle.png`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/circle/coordinates.csv` & `pyhard-2.2.1/pyhard/data/circle/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/circle/data.csv` & `pyhard-2.2.1/pyhard/data/circle/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/circle/feature_process.csv` & `pyhard-2.2.1/pyhard/data/circle/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/circle/feature_raw.csv` & `pyhard-2.2.1/pyhard/data/circle/feature_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/circle/metadata.csv` & `pyhard-2.2.1/pyhard/data/circle/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/circle/options.json` & `pyhard-2.2.1/pyhard/data/circle/options.json`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/easy/coordinates.csv` & `pyhard-2.2.1/pyhard/data/easy/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/easy/data.csv` & `pyhard-2.2.1/pyhard/data/easy/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/easy/feature_process.csv` & `pyhard-2.2.1/pyhard/data/easy/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/easy/feature_raw_color.csv` & `pyhard-2.2.1/pyhard/data/easy/feature_raw_color.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/easy/metadata.csv` & `pyhard-2.2.1/pyhard/data/easy/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/easy/options.json` & `pyhard-2.2.1/pyhard/data/easy/options.json`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/easy2/coordinates.csv` & `pyhard-2.2.1/pyhard/data/easy2/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/easy2/data.csv` & `pyhard-2.2.1/pyhard/data/easy2/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/easy2/easy2.png` & `pyhard-2.2.1/pyhard/data/easy2/easy2.png`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/easy2/metadata.csv` & `pyhard-2.2.1/pyhard/data/easy2/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/easy2/options.json` & `pyhard-2.2.1/pyhard/data/easy2/options.json`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/iris/coordinates.csv` & `pyhard-2.2.1/pyhard/data/iris/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/iris/data.csv` & `pyhard-2.2.1/pyhard/data/iris/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/iris/metadata.csv` & `pyhard-2.2.1/pyhard/data/iris/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/iris/options.json` & `pyhard-2.2.1/pyhard/data/iris/options.json`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/mix/coordinates.csv` & `pyhard-2.2.1/pyhard/data/mix/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/mix/data.csv` & `pyhard-2.2.1/pyhard/data/mix/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/mix/feature_process.csv` & `pyhard-2.2.1/pyhard/data/mix/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/mix/feature_raw.csv` & `pyhard-2.2.1/pyhard/data/mix/feature_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/mix/metadata.csv` & `pyhard-2.2.1/pyhard/data/mix/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/mix/mix.png` & `pyhard-2.2.1/pyhard/data/mix/mix.png`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/mix/options.json` & `pyhard-2.2.1/pyhard/data/mix/options.json`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/overlap/coordinates.csv` & `pyhard-2.2.1/pyhard/data/overlap/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/overlap/data.csv` & `pyhard-2.2.1/pyhard/data/overlap/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/overlap/metadata.csv` & `pyhard-2.2.1/pyhard/data/overlap/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/overlap/options.json` & `pyhard-2.2.1/pyhard/data/overlap/options.json`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/overlap/overlap.png` & `pyhard-2.2.1/pyhard/data/overlap/overlap.png`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/separate/coordinates.csv` & `pyhard-2.2.1/pyhard/data/separate/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/separate/data.csv` & `pyhard-2.2.1/pyhard/data/separate/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/separate/feature_process.csv` & `pyhard-2.2.1/pyhard/data/separate/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/separate/feature_raw.csv` & `pyhard-2.2.1/pyhard/data/separate/feature_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/separate/metadata.csv` & `pyhard-2.2.1/pyhard/data/separate/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/separate/options.json` & `pyhard-2.2.1/pyhard/data/separate/options.json`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/wine/algorithm_bin.csv` & `pyhard-2.2.1/pyhard/data/wine/algorithm_bin.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/wine/algorithm_process.csv` & `pyhard-2.2.1/pyhard/data/wine/algorithm_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/wine/algorithm_raw.csv` & `pyhard-2.2.1/pyhard/data/wine/algorithm_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/wine/beta_easy.csv` & `pyhard-2.2.1/pyhard/data/wine/beta_easy.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/wine/config.yaml` & `pyhard-2.2.1/pyhard/data/wine/config.yaml`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/wine/coordinates.csv` & `pyhard-2.2.1/pyhard/data/wine/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/wine/data.csv` & `pyhard-2.2.1/pyhard/data/wine/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/wine/feature_process.csv` & `pyhard-2.2.1/pyhard/data/wine/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/wine/feature_raw.csv` & `pyhard-2.2.1/pyhard/data/wine/feature_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/wine/footprint_bagging_good.csv` & `pyhard-2.2.1/pyhard/data/wine/footprint_bagging_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/wine/footprint_gradient_boosting_good.csv` & `pyhard-2.2.1/pyhard/data/wine/footprint_gradient_boosting_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/wine/footprint_instance_easiness_good.csv` & `pyhard-2.2.1/pyhard/data/wine/footprint_instance_easiness_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/wine/footprint_logistic_regression_good.csv` & `pyhard-2.2.1/pyhard/data/wine/footprint_logistic_regression_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/wine/footprint_mlp_good.csv` & `pyhard-2.2.1/pyhard/data/wine/footprint_mlp_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/wine/footprint_performance.csv` & `pyhard-2.2.1/pyhard/data/wine/footprint_performance.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/wine/footprint_random_forest_best.csv` & `pyhard-2.2.1/pyhard/data/wine/footprint_random_forest_best.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/wine/footprint_random_forest_good.csv` & `pyhard-2.2.1/pyhard/data/wine/footprint_random_forest_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/wine/footprint_svc_linear_good.csv` & `pyhard-2.2.1/pyhard/data/wine/footprint_svc_linear_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/wine/footprint_svc_rbf_good.csv` & `pyhard-2.2.1/pyhard/data/wine/footprint_svc_rbf_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/wine/good_algos.csv` & `pyhard-2.2.1/pyhard/data/wine/good_algos.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/wine/ih.csv` & `pyhard-2.2.1/pyhard/data/wine/ih.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/wine/metadata.csv` & `pyhard-2.2.1/pyhard/data/wine/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/wine/metadata_full.csv` & `pyhard-2.2.1/pyhard/data/wine/metadata_full.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/wine/model.pkl` & `pyhard-2.2.1/pyhard/data/wine/model.pkl`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/wine/options.json` & `pyhard-2.2.1/pyhard/data/wine/options.json`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/wine/portfolio.csv` & `pyhard-2.2.1/pyhard/data/wine/portfolio.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/xor/coordinates.csv` & `pyhard-2.2.1/pyhard/data/xor/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/xor/data.csv` & `pyhard-2.2.1/pyhard/data/xor/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/xor/metadata.csv` & `pyhard-2.2.1/pyhard/data/xor/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/xor/options.json` & `pyhard-2.2.1/pyhard/data/xor/options.json`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/data/xor/xor.pdf` & `pyhard-2.2.1/pyhard/data/xor/xor.pdf`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/feature_selection.py` & `pyhard-2.2.1/pyhard/feature_selection.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/hpo.py` & `pyhard-2.2.1/pyhard/hpo.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/integrator.py` & `pyhard-2.2.1/pyhard/integrator.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import shutil
 import warnings
 from importlib import import_module
 from inspect import signature, Parameter
 from pathlib import Path
 from typing import Union, Tuple
 
+import numpy as np
 import pandas as pd
 from deprecation import deprecated
 from pyispace import train_is
 from pyispace.train import Model
 from pyispace.utils import scriptcsv
 
 from .classification import ClassifiersPool
@@ -76,29 +77,32 @@
 
     df_algo = learners.run_all(
         metric=config.algos.metric,
         n_folds=config.algos.n_folds,
         n_iter=config.algos.n_iter,
         algo_list=config.algos.pool,
         parameters=config.algos.parameters,
+        resampling=config.algos.resampling,
         hyper_param_optm=config.hpo.enabled,
         hpo_evals=config.hpo.evals,
         hpo_timeout=config.hpo.timeout,
         verbose=verbose
     )
 
     df_metadata = pd.concat([df_measures, df_algo], axis=1)
     n_inst = len(df_metadata)
-    df_metadata.insert(0, instances_index, range(1, n_inst + 1))
+    df_metadata.insert(0, instances_index, np.arange(1, n_inst + 1))
     df_metadata.set_index(instances_index, inplace=True)
 
     if return_ih:
         ih_values = learners.estimate_ih()
-        df_ih = pd.DataFrame({'instance_hardness': ih_values},
-                             index=pd.Index(range(1, n_inst + 1), name=instances_index))
+        df_ih = pd.DataFrame(
+            {'instance_hardness': ih_values},
+            index=pd.Index(range(1, n_inst + 1), name=instances_index)
+        )
         return df_metadata, df_ih
     else:
         return df_metadata
 
 
 def run_isa(
         rootdir: Path,
```

### Comparing `pyhard-2.2.0/pyhard/measures.py` & `pyhard-2.2.1/pyhard/measures.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/metrics.py` & `pyhard-2.2.1/pyhard/metrics.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/midia/blobs.svg` & `pyhard-2.2.1/pyhard/midia/blobs.svg`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/regression.py` & `pyhard-2.2.1/pyhard/regression.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/structures.py` & `pyhard-2.2.1/pyhard/structures.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 This module provides structures (dataclasses) that accommodate configurations for each step of the framework.
 """
 
 from copy import deepcopy
 from dataclasses import asdict, dataclass, field, fields
 from pathlib import Path
-from typing import Dict, Optional, Union, List
+from typing import Dict, Optional, Union, List, Literal
 
 
 @dataclass
 class GeneralConfig:
     """
     General configurations.
     """
@@ -41,14 +41,15 @@
     Configurations relative to the pool of algorithms.
     """
     pool: List[str]
     parameters: dict = field(default_factory=dict)
     n_folds: int = 5
     n_iter: int = 1
     metric: str = 'logloss'
+    resampling: Literal['under', 'over', 'no'] = 'over'
 
 
 @dataclass(frozen=True)
 class ISAConfig:
     """
     Instance Space Analysis configurations.
     """
```

### Comparing `pyhard-2.2.0/pyhard/thirdparty/entropy_estimators.py` & `pyhard-2.2.1/pyhard/thirdparty/entropy_estimators.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/thirdparty/rank_aggregation.py` & `pyhard-2.2.1/pyhard/thirdparty/rank_aggregation.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/thirdparty/skfeature.py` & `pyhard-2.2.1/pyhard/thirdparty/skfeature.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/utils.py` & `pyhard-2.2.1/pyhard/utils.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/validator.py` & `pyhard-2.2.1/pyhard/validator.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyhard/visualization.py` & `pyhard-2.2.1/pyhard/visualization.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.2.0/pyproject.toml` & `pyhard-2.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,16 @@
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Intended Audience :: Science/Research"
 ]
 dynamic = ["version"]
 dependencies = [
     "pandas>=1.3.0",
-    "scikit-learn>=1.2.0, <1.3.0",
-    "imbalanced-learn>=0.10.0",
+    "scikit-learn>=1.3.0",
+    "imbalanced-learn>=0.11.0",
     "numpy>=1.18.4",
     "PyYAML>=5.3",
     "scipy>=1.4.1",
     "panel~=0.14.1",
     "param>=1.12.2",
     "bokeh>=2.4.3",
     "holoviews>=1.15.0",
```

### Comparing `pyhard-2.2.0/PKG-INFO` & `pyhard-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyhard
-Version: 2.2.0
+Version: 2.2.1
 Summary: Analyze, explore and visualize instance hardness within datasets
 Author-email: Pedro Paiva <paiva@ita.br>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Intended Audience :: Science/Research
 Requires-Dist: pandas>=1.3.0
-Requires-Dist: scikit-learn>=1.2.0, <1.3.0
-Requires-Dist: imbalanced-learn>=0.10.0
+Requires-Dist: scikit-learn>=1.3.0
+Requires-Dist: imbalanced-learn>=0.11.0
 Requires-Dist: numpy>=1.18.4
 Requires-Dist: PyYAML>=5.3
 Requires-Dist: scipy>=1.4.1
 Requires-Dist: panel~=0.14.1
 Requires-Dist: param>=1.12.2
 Requires-Dist: bokeh>=2.4.3
 Requires-Dist: holoviews>=1.15.0
```

