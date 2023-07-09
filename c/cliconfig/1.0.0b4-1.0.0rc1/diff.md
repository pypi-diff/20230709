# Comparing `tmp/cliconfig-1.0.0b4.tar.gz` & `tmp/cliconfig-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliconfig-1.0.0b4.tar", last modified: Thu Jun  1 11:59:58 2023, max compression
+gzip compressed data, was "cliconfig-1.0.0rc1.tar", last modified: Sat Jul  8 20:46:59 2023, max compression
```

## Comparing `cliconfig-1.0.0b4.tar` & `cliconfig-1.0.0rc1.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.560691 cliconfig-1.0.0b4/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.548691 cliconfig-1.0.0b4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.552691 cliconfig-1.0.0b4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/.github/workflows/flake.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/.github/workflows/pipy_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/.github/workflows/pydocstyle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/.github/workflows/pylint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/.markdownlint.json
--rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-06-01 11:59:58.560691 cliconfig-1.0.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12789 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.552691 cliconfig-1.0.0b4/cliconfig/
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/cliconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-01 11:59:58.000000 cliconfig-1.0.0b4/cliconfig/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/cliconfig/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/cliconfig/cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/cliconfig/config_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)    15588 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/cliconfig/dict_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/cliconfig/process_routines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.556692 cliconfig-1.0.0b4/cliconfig/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/cliconfig/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/cliconfig/processing/_type_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/cliconfig/processing/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    30509 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/cliconfig/processing/builtin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/cliconfig/processing/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/cliconfig/tag_routines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.556692 cliconfig-1.0.0b4/cliconfig/yaml_tags/
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/cliconfig/yaml_tags/_yaml_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.552691 cliconfig-1.0.0b4/cliconfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-06-01 11:59:58.000000 cliconfig-1.0.0b4/cliconfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-01 11:59:58.000000 cliconfig-1.0.0b4/cliconfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 11:59:58.000000 cliconfig-1.0.0b4/cliconfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-01 11:59:58.000000 cliconfig-1.0.0b4/cliconfig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-01 11:59:58.000000 cliconfig-1.0.0b4/cliconfig.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.556692 cliconfig-1.0.0b4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/docs/README_pypi.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.556692 cliconfig-1.0.0b4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/docs/_static/logo_extend.png
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/docs/cliconfig.processing_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/docs/cliconfig_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/docs/contribute.md
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/docs/edge_cases.md
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)    16459 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/docs/processing.md
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/docs/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.556692 cliconfig-1.0.0b4/github_actions_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/github_actions_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/github_actions_utils/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/github_actions_utils/pydocstyle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/github_actions_utils/pylint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/github_actions_utils/pytest_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.556692 cliconfig-1.0.0b4/licenses_tier/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/licenses_tier/FLATTEN_DICT_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/pre-commit-checks.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 11:59:58.560691 cliconfig-1.0.0b4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.556692 cliconfig-1.0.0b4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.556692 cliconfig-1.0.0b4/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/config1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/config2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/configtag1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/configtag2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/default1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/default2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.560691 cliconfig-1.0.0b4/tests/configs/delete/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/delete/config1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/delete/config2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/fallback.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.548691 cliconfig-1.0.0b4/tests/configs/integration/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.560691 cliconfig-1.0.0b4/tests/configs/integration/test1/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/integration/test1/main.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/integration/test1/sub1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/integration/test1/sub2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.560691 cliconfig-1.0.0b4/tests/configs/integration/test2/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/integration/test2/data.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/integration/test2/default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/integration/test2/exp1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/integration/test2/exp2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/integration/test2/exp3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.560691 cliconfig-1.0.0b4/tests/configs/integration/test2/models/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/integration/test2/models/resnet100.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/integration/test2/models/resnet50.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/integration/test2/models/vit_b16.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.560691 cliconfig-1.0.0b4/tests/configs/merge/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/merge/additional1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/merge/additional2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/merge/additional3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/merge/default1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/merge/default2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/merge/default3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/configs/multi_files_with_tags.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.560691 cliconfig-1.0.0b4/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/integration/test_inte_multiple_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.560691 cliconfig-1.0.0b4/tests/unit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:59:58.560691 cliconfig-1.0.0b4/tests/unit/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/unit/processing/test_base_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/unit/processing/test_builtin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/unit/processing/test_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/unit/processing/test_type_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/unit/test_base_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/unit/test_cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/unit/test_config_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/unit/test_dict_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/unit/test_ex_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/unit/test_process_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-06-01 11:59:43.000000 cliconfig-1.0.0b4/tests/unit/test_tag_routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:46:59.686845 cliconfig-1.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:46:59.666844 cliconfig-1.0.0rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:46:59.674844 cliconfig-1.0.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/.github/workflows/flake.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/.github/workflows/pipy_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/.github/workflows/pydocstyle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/.github/workflows/pylint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/.github/workflows/ruff.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/.markdownlint.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-07-08 20:46:59.686845 cliconfig-1.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:46:59.674844 cliconfig-1.0.0rc1/cliconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/cliconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-08 20:46:59.000000 cliconfig-1.0.0rc1/cliconfig/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/cliconfig/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/cliconfig/cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/cliconfig/config_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15588 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/cliconfig/dict_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/cliconfig/process_routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:46:59.674844 cliconfig-1.0.0rc1/cliconfig/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/cliconfig/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/cliconfig/processing/_type_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/cliconfig/processing/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30503 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/cliconfig/processing/builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14901 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/cliconfig/processing/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/cliconfig/tag_routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:46:59.674844 cliconfig-1.0.0rc1/cliconfig/yaml_tags/
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/cliconfig/yaml_tags/_yaml_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:46:59.674844 cliconfig-1.0.0rc1/cliconfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-07-08 20:46:59.000000 cliconfig-1.0.0rc1/cliconfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-08 20:46:59.000000 cliconfig-1.0.0rc1/cliconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 20:46:59.000000 cliconfig-1.0.0rc1/cliconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-08 20:46:59.000000 cliconfig-1.0.0rc1/cliconfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-08 20:46:59.000000 cliconfig-1.0.0rc1/cliconfig.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:46:59.678844 cliconfig-1.0.0rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/docs/README_pypi.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:46:59.678844 cliconfig-1.0.0rc1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/docs/_static/logo_extend.png
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/docs/cliconfig.processing_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/docs/cliconfig_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/docs/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/docs/edge_cases.md
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    17015 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/docs/processing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:46:59.678844 cliconfig-1.0.0rc1/github_actions_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/github_actions_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/github_actions_utils/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/github_actions_utils/pydocstyle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/github_actions_utils/pylint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/github_actions_utils/pytest_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:46:59.678844 cliconfig-1.0.0rc1/licenses_tier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/licenses_tier/FLATTEN_DICT_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/pre-commit-checks.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 20:46:59.686845 cliconfig-1.0.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:46:59.678844 cliconfig-1.0.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:46:59.678844 cliconfig-1.0.0rc1/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/configs/config1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/configs/config2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/configs/configtag1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/configs/configtag2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/configs/default1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/configs/default2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:46:59.682845 cliconfig-1.0.0rc1/tests/configs/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/configs/delete/config1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/configs/delete/config2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/configs/fallback.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:46:59.670844 cliconfig-1.0.0rc1/tests/configs/integration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:46:59.682845 cliconfig-1.0.0rc1/tests/configs/integration/test1/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/configs/integration/test1/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/configs/integration/test1/sub1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/configs/integration/test1/sub2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:46:59.682845 cliconfig-1.0.0rc1/tests/configs/integration/test2/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/configs/integration/test2/data.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/configs/integration/test2/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/configs/integration/test2/exp1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/configs/integration/test2/exp2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/configs/integration/test2/exp3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:46:59.682845 cliconfig-1.0.0rc1/tests/configs/integration/test2/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/configs/integration/test2/models/resnet100.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/configs/integration/test2/models/resnet50.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/configs/integration/test2/models/vit_b16.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:46:59.682845 cliconfig-1.0.0rc1/tests/configs/merge/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/configs/merge/additional1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/configs/merge/additional2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/configs/merge/additional3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/configs/merge/default1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/configs/merge/default2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/configs/merge/default3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/configs/multi_files_with_tags.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:46:59.682845 cliconfig-1.0.0rc1/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/integration/test_ex_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/integration/test_inte_multiple_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:46:59.682845 cliconfig-1.0.0rc1/tests/unit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:46:59.686845 cliconfig-1.0.0rc1/tests/unit/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/unit/processing/test_base_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/unit/processing/test_builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/unit/processing/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/unit/processing/test_type_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/unit/test_base_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/unit/test_cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/unit/test_config_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/unit/test_dict_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/unit/test_process_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-07-08 20:46:37.000000 cliconfig-1.0.0rc1/tests/unit/test_tag_routines.py
```

### Comparing `cliconfig-1.0.0b4/.github/workflows/pipy_deployment.yaml` & `cliconfig-1.0.0rc1/.github/workflows/pipy_deployment.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b4/.github/workflows/pydocstyle.yaml` & `cliconfig-1.0.0rc1/.github/workflows/pydocstyle.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b4/.github/workflows/pylint.yaml` & `cliconfig-1.0.0rc1/.github/workflows/pylint.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b4/.github/workflows/tests.yaml` & `cliconfig-1.0.0rc1/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b4/.pylintrc` & `cliconfig-1.0.0rc1/.pylintrc`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b4/CONTRIBUTING.md` & `cliconfig-1.0.0rc1/CONTRIBUTING.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 Before submitting a PR you should run this pipeline:
 
 ```script
 sh scripts/pre-commit-checks.sh
 ```
 
 **Try to not decrease the global Pylint score** after a pull request. A minimum
-of 8.5/10.0 is required but **we preferably want above 9.0/10.0.**
+of 8.5/10.0 is required, but **we preferably want above 9.0/10.0.**
 
 ## Commit message
 
 Commits should start with an emoji and directly followed by a descriptive and
 precise message that starts with a capital letter and should be written in present
 tense. E.g:
 
@@ -45,41 +45,41 @@
 
 *✨ Add function to save configuration file* ✅ Good
 
 Emojis not only look great but also makes you rethink what to add to a commit.
 The goal is to dedicate each single kind of change to a single commit. Make many
 but small commits!
 
-Emojis of commit message follow mainly the [Gitmoji](https://gitmoji.dev/) guidline
-(the different ones start with an asterisk *). The most usefull are:
+Emojis of commit message follow mainly the [Gitmoji](https://gitmoji.dev/) guideline
+(the different ones start with an asterisk *). The most useful are:
 
-| Emoji                                 | Description                                            |
-| ------------------------------------- | ------------------------------------------------------ |
-| 🎉 `:tada:`                        | Initial commit                                         |
-| ✨ `:sparkles:`                    | New cool feature                                       |
-| ➕ `:heavy_plus_sign:` *           | Add file and/or folder                                 |
-| 🔥 `:fire:`                        | Remove some code or file                               |
-| 📝 `:memo:`                        | Add or improve readme, docstring or comments           |
-| 🐛 `:bug:`                         | Fix a bug                                              |
-| 🎨 `:art:`                         | Improve style, or format the code                      |
-| ♻️ `:recycle:`                       | Refactor the code                                      |
-| 🚚 `:truck:`                       | Rename and/or move files and folders                   |
-| 🏗️ `:building_construction:`       | Change a part of the repository architecture           |
-| ✏️  `:pencil2:`                      | Fix typo                                               |
-| ⚙️  `:gear:` *                       | Add or update configuration file (config/exp.yaml, ...)|
-| 🔧 `:wrench:`                      | Add or update tool configuration (pyproject.toml, ...) |
-| 🍱 `:bento:`                       | Add or update assets                                   |
-| 🚀 `:rocket:` *                    | Improve performance                                    |
-| ⚗️ `:alembic:`                       | Perform experiment                                     |
-| 🚸 `:children_crossing:`           | Improve user experience                                |
-| 🆙 `:up:` * OR 🔖 `:bookmark:`  | Update the version/tag                                 |
-| ⬆️  `:arrow_up:`                     | Upgrade dependency                                     |
-| 🚧 `:construction:`                | Work in progress                                       |
-| 🔀 `:twisted_rightwards_arrows:`   | Merge a branch                                         |
-| Check [Gitmoji](https://gitmoji.dev/) | *OTHER*                                                |
+| Emoji                                 | Description                                             |
+| ------------------------------------- | ------------------------------------------------------- |
+| 🎉 `:tada:`                            | Initial commit                                          |
+| ✨ `:sparkles:`                        | New cool feature                                        |
+| ➕ `:heavy_plus_sign:` *               | Add file and/or folder                                  |
+| 🔥 `:fire:`                            | Remove some code or file                                |
+| 📝 `:memo:`                            | Add or improve readme, docstring or comments            |
+| 🐛 `:bug:`                             | Fix a bug                                               |
+| 🎨 `:art:`                             | Improve style, or format the code                       |
+| ♻️ `:recycle:`                         | Refactor the code                                       |
+| 🚚 `:truck:`                           | Rename and/or move files and folders                    |
+| 🏗️ `:building_construction:`           | Change a part of the repository architecture            |
+| ✏️  `:pencil2:`                        | Fix typo                                                |
+| ⚙️  `:gear:` *                         | Add or update configuration file (config/exp.yaml, ...) |
+| 🔧 `:wrench:`                          | Add or update tool configuration (pyproject.toml, ...)  |
+| 🍱 `:bento:`                           | Add or update assets                                    |
+| 🚀 `:rocket:` *                        | Improve performance                                     |
+| ⚗️ `:alembic:`                         | Perform experiment                                      |
+| 🚸 `:children_crossing:`               | Improve user experience                                 |
+| 🆙 `:up:` * OR 🔖 `:bookmark:`          | Update the version/tag                                  |
+| ⬆️  `:arrow_up:`                       | Upgrade dependency                                      |
+| 🚧 `:construction:`                    | Work in progress                                        |
+| 🔀 `:twisted_rightwards_arrows:`       | Merge a branch                                          |
+| Check [Gitmoji](https://gitmoji.dev/) | *OTHER*                                                 |
 
 Installing the [Gitmoji VSCode extension](https://marketplace.visualstudio.com/items?itemName=seatonjiang.gitmoji-vscode)
 can be useful to get the emoji you want.
 
 ## Version and tag numbers
 
 Version/tag numbers will be assigned according to the [Semantic Versioning scheme](https://semver.org/).
```

### Comparing `cliconfig-1.0.0b4/LICENSE` & `cliconfig-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b4/PKG-INFO` & `cliconfig-1.0.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cliconfig
-Version: 1.0.0b4
+Version: 1.0.0rc1
 Summary: Merge your config files and set parameters from the command line in a simple way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/cliconfig
 Keywords: cli,config,cliconfig,python,yaml,merge
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
@@ -22,15 +22,15 @@
 
 |
 
 *CLI Config*: Lightweight library that provides routines to merge nested configs
 and set parameters from command line. It is also provide processing functions
 that can change the whole configuration before and after each config merge, config
 saving, config loading and at the end of config building. It also contains many
-routines to manipulate the config as flatten or nested dicts.
+routines to manipulate the config as flatten or nested dictionaries.
 
 `Pypi project <https://pypi.org/project/cliconfig/>`_
 
 `Github project <https://github.com/valentingol/cliconfig>`_
 
 
 |PyPI version| |PythonVersion| |License| |Waka_Time|
@@ -47,15 +47,15 @@
 
    # main.py
    from cliconfig import make_config
 
    config = make_config('default1.yaml', 'default2.yaml')
 
 Then launch your script with additional config(s) file(s) and parameters by command line.
-The additional configs are merge on the default ones then the parameters are set.
+The additional configs are merged on the default one's then the parameters are set.
 
 .. code:: bash
 
    python main.py --config first.yaml,second.yaml --param1=1 --subconfig.param2='foo'
 
 **By default, these additional configs cannot add new parameters to the default config
 (for security and retro-compatibility reasons).**
@@ -71,15 +71,15 @@
 
 You can also load and save configs with `cliconfig.save_config` and `cliconfig.load_config`.
 
 
 With processing
 ---------------
 
-The library provide powerful tools to modify the configuration called "processings".
+The library provides powerful tools to modify the configuration called "processings".
 One of the possibility they add is to merge multiple configurations,
 copy a parameter on another, enforce type and more. To do so, simply adding the
 corresponding tags to your parameter names (on config files or CLI parameters).
 
 For instance with these config files:
 
 .. code:: yaml
```

### Comparing `cliconfig-1.0.0b4/README.md` & `cliconfig-1.0.0rc1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <img src="docs/_static/logo_extend.png" />
 </p>
 
 *CLI Config*: Lightweight library that provides routines to merge nested configs
 and set parameters from command line. It is also provide processing functions
 that can change the whole configuration before and after each config merge, config
 saving, config loading and at the end of config building. It also contains many
-routines to manipulate the config as flatten or nested dicts.
+routines to manipulate the config as flatten or nested dictionaries.
 
 ## Documentation :memo: [here](https://cliconfig.readthedocs.io/en/stable)
 
 ## Pypi :package: [here](https://pypi.org/project/cliconfig/)
 
 [![Release](https://img.shields.io/github/v/tag/valentingol/cliconfig?label=Pypi&logo=pypi&logoColor=yellow)](https://pypi.org/project/cliconfig/)
 ![PythonVersion](https://img.shields.io/badge/Python-3.7%20%7E%203.11-informational)
@@ -106,15 +106,15 @@
 For example:
 
 ```bash
 python main.py --config first.yaml,second.yaml --param2=-2 --letters.letter2='B'
 ```
 
 *Note*: the additional configs are detected with `--config` followed by space
-and separated by comma(s) **without space**. It also possible to pass a list.
+and separated by comma(s) **without space**. It is also possible to pass a list.
 The parameters are detected with the pattern `--<param>=<value>` without spaces.
 
 It will show:
 
 ```text
 [CONFIG] Merge 2 default configs, 2 additional configs and 2 CLI parameter(s).
 
@@ -163,15 +163,15 @@
   (except for tuples and sets, which are not handled by YAML) as well as unions
   (using "Union" or "|"), optional values, nested list, and nested dict.
   For instance: `@type:List[Dict[str, int|float]]`.
 * `@select`: This tag select sub-config(s) to keep and delete the other
   sub-configs in the same parent config. The tagged key is not deleted if it is
   in the parent config.
 * `@delete`: This tag deletes the key from the config before merging.
-* `@new`: This tag allows to add new key(s) to the config that are not already
+* `@new`: This tag allows adding new key(s) to the config that are not already
   present in the default config(s). It can be used for single parameter or a
   sub-config. Disclaimer: it is preferable to have exhaustive default config(s)
   instead of abusing this tag for readability and for security concerning typos.
 
 The tags are applied in the following order: `@merge`, `@select`, `@copy`, `@type`
 and then `@delete`.
 
@@ -273,36 +273,27 @@
 pip install -e .
 pip install -r requirements-dev.txt
 ```
 
 Everyone can contribute to CLI Config, and we value everyone’s contributions.
 Please see our [contributing guidelines](CONTRIBUTING.md) for more information 🤗
 
-## Todo
+## To-do
 
-Priority:
-
-* [x] Add end-build processing that trigger at the end of `make_config` and `load_config`.
-* [x] Continue `test_multi_tags2` integration test with cases that raise errors, and
-  pre-save processing.
-* [x] Support multi-files in yaml file (with separator "---")
-* [ ] Fix mistakes in all docstrings (🚧  in progress)
-
-Secondary:
-
-* [x] Add a `@delete` tag to delete a key from the config after pre-merge. Useful to make
-  processing action without introducing new keys in the config.
-* [x] Set a default value to True if no value are specified for parameter in command line.
-* [x] Support yaml tags "!tag" in config files.
+* [x] Add a parameter to change the type (pre-merge, post-merge, ...) of processings
+  created by `create_processing_XXX`
+* [x] Allow the flat config to be passed as a 2nd argument of the fonctions `func` used
+  in `create_processing_XXX`
+* [x] Correct grammar and syntax errors in the documentation with LTex
 
 ## License
 
-Copyright (C) 2023  Valentin Goldité
+Copyright © 2023 Valentin Goldité
 
 This program is free software: you can redistribute it and/or modify it under the
 terms of the [MIT License](LICENSE). This program is distributed in the hope that
 it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 
-This project is free to use for COMMERCIAL USE, MODIFICATION, DISTRIBUTION and
-PRIVATE USE as long as the original license is include as well as this copy
+The project is free to use for COMMERCIAL USE, MODIFICATION, DISTRIBUTION and
+PRIVATE USE as long as the original license is included as well as this copy
 right notice at the top of the modified files.
```

### Comparing `cliconfig-1.0.0b4/cliconfig/__init__.py` & `cliconfig-1.0.0rc1/cliconfig/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """CLI Config: build your configuration from CLI by merging with processing.
 
-Copyright (C) 2023  Valentin Goldité
+Copyright © 2023  Valentin Goldité
 
     This program is free software: you can redistribute it and/or modify
     it under the terms of the MIT License.
     This program is distributed in the hope that it will be useful,
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
     This project is free to use for COMMERCIAL USE, MODIFICATION,
```

### Comparing `cliconfig-1.0.0b4/cliconfig/base.py` & `cliconfig-1.0.0rc1/cliconfig/base.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b4/cliconfig/cli_parser.py` & `cliconfig-1.0.0rc1/cliconfig/cli_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b4/cliconfig/config_routines.py` & `cliconfig-1.0.0rc1/cliconfig/config_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b4/cliconfig/dict_routines.py` & `cliconfig-1.0.0rc1/cliconfig/dict_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b4/cliconfig/process_routines.py` & `cliconfig-1.0.0rc1/cliconfig/process_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b4/cliconfig/processing/_type_parser.py` & `cliconfig-1.0.0rc1/cliconfig/processing/_type_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b4/cliconfig/processing/base.py` & `cliconfig-1.0.0rc1/cliconfig/processing/base.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b4/cliconfig/processing/builtin.py` & `cliconfig-1.0.0rc1/cliconfig/processing/builtin.py`

 * *Files 1% similar despite different names*

```diff
@@ -523,15 +523,15 @@
                 del flat_config.dict[key]
         return flat_config
 
 
 class ProcessDelete(Processing):
     """Delete the parameters tagged with ``@delete`` on pre-merge.
 
-    This processing is usefull to activate a processing without adding
+    This processing is useful to activate a processing without adding
     an additional parameter in the default configuration to avoid the error
     on merge with ``allow_new_keys=False``. This processing is applied very
     late on pre-merge to allow the others processing to be applied before
     deleting the parameters.
     Pre-merge order: 30.0
 
     Examples
@@ -657,17 +657,17 @@
         self.new_vals = {}
         return flat_config
 
     def presave(self, flat_config: Config) -> Config:
         """Pre-save processing."""
         # Restore the tag @new to allow loading the config later by allowing
         # these new parameters.
-        for key in self.new_vals_backup:
+        for key, value in self.new_vals_backup.items():
             if key in flat_config.dict:
-                flat_config.dict[key + "@new"] = self.new_vals_backup[key]
+                flat_config.dict[key + "@new"] = value
                 del flat_config.dict[key]
         return flat_config
 
 
 class ProcessCheckTags(Processing):
     """Raise an error if a tag is present in a key after pre-merging processes.
```

### Comparing `cliconfig-1.0.0b4/cliconfig/tag_routines.py` & `cliconfig-1.0.0rc1/cliconfig/tag_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b4/cliconfig/yaml_tags/_yaml_tags.py` & `cliconfig-1.0.0rc1/cliconfig/yaml_tags/_yaml_tags.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b4/cliconfig.egg-info/PKG-INFO` & `cliconfig-1.0.0rc1/cliconfig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cliconfig
-Version: 1.0.0b4
+Version: 1.0.0rc1
 Summary: Merge your config files and set parameters from the command line in a simple way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/cliconfig
 Keywords: cli,config,cliconfig,python,yaml,merge
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
@@ -22,15 +22,15 @@
 
 |
 
 *CLI Config*: Lightweight library that provides routines to merge nested configs
 and set parameters from command line. It is also provide processing functions
 that can change the whole configuration before and after each config merge, config
 saving, config loading and at the end of config building. It also contains many
-routines to manipulate the config as flatten or nested dicts.
+routines to manipulate the config as flatten or nested dictionaries.
 
 `Pypi project <https://pypi.org/project/cliconfig/>`_
 
 `Github project <https://github.com/valentingol/cliconfig>`_
 
 
 |PyPI version| |PythonVersion| |License| |Waka_Time|
@@ -47,15 +47,15 @@
 
    # main.py
    from cliconfig import make_config
 
    config = make_config('default1.yaml', 'default2.yaml')
 
 Then launch your script with additional config(s) file(s) and parameters by command line.
-The additional configs are merge on the default ones then the parameters are set.
+The additional configs are merged on the default one's then the parameters are set.
 
 .. code:: bash
 
    python main.py --config first.yaml,second.yaml --param1=1 --subconfig.param2='foo'
 
 **By default, these additional configs cannot add new parameters to the default config
 (for security and retro-compatibility reasons).**
@@ -71,15 +71,15 @@
 
 You can also load and save configs with `cliconfig.save_config` and `cliconfig.load_config`.
 
 
 With processing
 ---------------
 
-The library provide powerful tools to modify the configuration called "processings".
+The library provides powerful tools to modify the configuration called "processings".
 One of the possibility they add is to merge multiple configurations,
 copy a parameter on another, enforce type and more. To do so, simply adding the
 corresponding tags to your parameter names (on config files or CLI parameters).
 
 For instance with these config files:
 
 .. code:: yaml
```

### Comparing `cliconfig-1.0.0b4/cliconfig.egg-info/SOURCES.txt` & `cliconfig-1.0.0rc1/cliconfig.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -84,19 +84,19 @@
 tests/configs/integration/test2/models/vit_b16.yaml
 tests/configs/merge/additional1.yaml
 tests/configs/merge/additional2.yaml
 tests/configs/merge/additional3.yaml
 tests/configs/merge/default1.yaml
 tests/configs/merge/default2.yaml
 tests/configs/merge/default3.yaml
+tests/integration/test_ex_docs.py
 tests/integration/test_inte_multiple_tags.py
 tests/unit/test_base_config.py
 tests/unit/test_cli_parser.py
 tests/unit/test_config_routines.py
 tests/unit/test_dict_routines.py
-tests/unit/test_ex_docs.py
 tests/unit/test_process_routines.py
 tests/unit/test_tag_routines.py
 tests/unit/processing/test_base_processing.py
 tests/unit/processing/test_builtin.py
 tests/unit/processing/test_create.py
 tests/unit/processing/test_type_parser.py
```

### Comparing `cliconfig-1.0.0b4/docs/Makefile` & `cliconfig-1.0.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b4/docs/README_pypi.rst` & `cliconfig-1.0.0rc1/docs/README_pypi.rst`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 |
 
 *CLI Config*: Lightweight library that provides routines to merge nested configs
 and set parameters from command line. It is also provide processing functions
 that can change the whole configuration before and after each config merge, config
 saving, config loading and at the end of config building. It also contains many
-routines to manipulate the config as flatten or nested dicts.
+routines to manipulate the config as flatten or nested dictionaries.
 
 `Pypi project <https://pypi.org/project/cliconfig/>`_
 
 `Github project <https://github.com/valentingol/cliconfig>`_
 
 
 |PyPI version| |PythonVersion| |License| |Waka_Time|
@@ -35,15 +35,15 @@
 
    # main.py
    from cliconfig import make_config
 
    config = make_config('default1.yaml', 'default2.yaml')
 
 Then launch your script with additional config(s) file(s) and parameters by command line.
-The additional configs are merge on the default ones then the parameters are set.
+The additional configs are merged on the default one's then the parameters are set.
 
 .. code:: bash
 
    python main.py --config first.yaml,second.yaml --param1=1 --subconfig.param2='foo'
 
 **By default, these additional configs cannot add new parameters to the default config
 (for security and retro-compatibility reasons).**
@@ -59,15 +59,15 @@
 
 You can also load and save configs with `cliconfig.save_config` and `cliconfig.load_config`.
 
 
 With processing
 ---------------
 
-The library provide powerful tools to modify the configuration called "processings".
+The library provides powerful tools to modify the configuration called "processings".
 One of the possibility they add is to merge multiple configurations,
 copy a parameter on another, enforce type and more. To do so, simply adding the
 corresponding tags to your parameter names (on config files or CLI parameters).
 
 For instance with these config files:
 
 .. code:: yaml
```

### Comparing `cliconfig-1.0.0b4/docs/_static/logo.png` & `cliconfig-1.0.0rc1/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b4/docs/_static/logo_extend.png` & `cliconfig-1.0.0rc1/docs/_static/logo_extend.png`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b4/docs/cliconfig_api.rst` & `cliconfig-1.0.0rc1/docs/cliconfig_api.rst`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b4/docs/conf.py` & `cliconfig-1.0.0rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b4/docs/edge_cases.md` & `cliconfig-1.0.0rc1/docs/edge_cases.md`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b4/docs/license.md` & `cliconfig-1.0.0rc1/docs/license.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # License
 
-Copyright (C) 2023 Valentin Goldité
+Copyright © 2023 Valentin Goldité
 
 This program is free software: you can redistribute it and/or modify it
 under the terms of the `MIT License <LICENSE>`__. This program is
 distributed in the hope that it will be useful, but WITHOUT ANY
 WARRANTY; without even the implied warranty of MERCHANTABILITY or
 FITNESS FOR A PARTICULAR PURPOSE.
 
-This project is free to use for COMMERCIAL USE, MODIFICATION,
-DISTRIBUTION and PRIVATE USE as long as the original license is include
+The project is free to use for COMMERCIAL USE, MODIFICATION,
+DISTRIBUTION and PRIVATE USE as long as the original license is included
 as well as this copy right notice at the top of the modified files.
```

### Comparing `cliconfig-1.0.0b4/docs/make.bat` & `cliconfig-1.0.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b4/docs/processing.md` & `cliconfig-1.0.0rc1/docs/processing.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,37 +3,37 @@
 Processings are powerful tools to modify the config at each step of the lifecycle of
 a configuration. More precisely, you can use processings to modify the full
 configuration before and after each merge, after loading, and before saving the config.
 
 The processings are applied via a processing object that have five methods
 (called "processing" to simplify): `premerge`, `postmerge`, `endbuild`, `postload`
 and `presave`. These names correspond to the timing they are applied. Each processing
-have the signature:
+has the signature:
 
 ```python
 def premerge(self, flat_config: Config) -> Config:
     ...
     return flat_config
 ```
 
 Where `Config` is a simple class containing only two attributes (and no methods):
 `dict` that is the configuration dict and `process_list`, the list of processing objects
-(we discuss about this in a section below). Note that it is
+(we discuss this in a section below). Note that it is
 also the class of the object returned by the `make_config` function.
 
 They only take a flat config as input i.e a config containing a dict of depth 1 with
 dot-separated keys and return the modified flat dict (and keep it flat!).
 
 In this section, you will learn how they work and how to create your own to make
 whatever you want with the config (we hope!).
 
 ## Why a flat dict?
 
 The idea is that when we construct a config, we manipulate dictionaries that contain
-both nested sub-dicts and flat keys simultaneously. To simplify this process, the
+both nested sub-dictionaries and flat keys simultaneously. To simplify this process, the
 dictionaries are systematically flattened before merging. This approach makes things
 simpler and prevents duplicated keys within the same configuration, as shown in the
 example:
 
 ```python
 config = {'a': {'b': 1}, 'a.b': 2}
 ```
@@ -61,19 +61,19 @@
 merge@merge_add@delete: config2.yaml
 param: 1
 # config2.yaml
 param2: 2
 ```
 
 In this example, we want to build a global config using `config1.yaml`. This file contains only
-half of the paramers, and the other half is in `config2.yaml`. Then, we add a key
+half of the parameters, and the other half is in `config2.yaml`. Then, we add a key
 with the name of our choice, here "merge", tagged with `@merge_add` to merge
 `config2.yaml` before the global config update. We add the `@delete` tag to delete
 the key "merge" before merging with the global config because in this case, there is
-no key with the name "merge" in the global config and it would raise an error as
+no key with the name "merge" in the global config, and it would raise an error as
 it is not possible to ass new keys.
 
 `@merge_add` and `@delete` has both only a pre-merge effect. Let's check the orders.
 It is `-20.0` for merge and `30.0` for delete. So merge trigger first, add `param2` and
 the "merge" key is deleted after it. If the orders were reversed, the key would have been
 deleted before merge processing and so the `param2` would not have been updated with the
 value of 2 and the resulting configuration would potentially not have been
@@ -81,123 +81,144 @@
 
 Therefore, it is crucial to carefully manage the order when creating your own
 processings!
 
 Some useful ranges to choose your order:
 
 * not important: order = 0 (default)
-* if it check/modify the config before applying any processing: order < -25
-* if it add new parameters: -25 < order < -5
-* if it update a value based on itself: -5 < order < 5
-* if it update a value based on other keys: 5 < order < 15
-* if it checks a property on a value: 15 < order < 25
-* if it delete other key(s) but you want to trigger the tags before: 25 < order < 35
+* if it checks/modifies the config before applying any processing: order < -25
+* if it adds new parameters: -25 < order < -5
+* if it updates a value based on itself: -5 < order < 5
+* if it updates a value based on other keys: 5 < order < 15
+* if it checkss a property on a value: 15 < order < 25
+* if it deletes other key(s) but you want to trigger the tags before: 25 < order < 35
 * final check/modification after all processings: order > 35
 
 Note: a pre-merge order should not be greater than 1000, the order of the default
 processing `ProcessCheckTags` that raise an error if tags still exist at the end
 of the pre-merge step.
 
 ## Create basic processing
 
-### Pre-merge processing that modify a single value
+### Processing that modify a single value
 
-The pre-merge processing is particularly useful as it allows you to modify the input
-config provided by the user and create the resulting Python dictionary that stores the
-configuration for your experiment. It serves as the interface between the user config
-and the final config.
-
-In some cases, you may need to get parameters which names match a certain
-patterns (e.g a prefix or a suffix) or contain a specific tag and modify their values
+One of the most useful kind of processing look for parameters which names match a certain
+pattern (e.g a prefix or a suffix) or contain a specific tag and modify their values
 depending on their current ones.
 
 To simplify the creation of such a process, we provide the `cliconfig.create_processing_value` function.
 This function allows you to quickly create a processing that matches a regular
 expression or a specific tag name (in which case the tag is removed after pre-merging).
 You specify the function to be applied on the value to modify it, and optionally,
 the order of the processing. Additionally, there is a `persistent` argument, which is
 a boolean value indicating whether encountering the tag (if a tag is used) once in
 a parameter name will continue to trigger the processing for this parameter
-even after the tag is removed. By default, it is `True`.
+even after the tag is removed. By default, it is `False`. Finally, you can set
+the processing type (pre-merge, post-merge, etc.) at your convenience. Default is pre-merge.
 
 Here's an example to illustrate:
 
 ```python
-proc = create_processing_value(lambda x: str(x), tag='convert_str', persistent=True)
+proc = create_processing_value(lambda x: str(x), 'premerge', tag_name='convert_str', persistent=True)
 config = make_config(default_config, process_list=[proc])
 ```
 
 In this example, the config `{"subconfig.param@convert_str": 1}` will
 be converted to `{"subconfig.param": "1"}`. Moreover, the keys `subconfig.param`
 will be permanently converted to strings before every merge.
 
 It's worth noting that you can also use functions that have side effects without
 necessarily changing the value itself. For example, you can use a function to
 check if a certain condition is met by the value.
 
+It is also possible to pass the flat config as a second argument to the function.
+For example:
+
+```yaml
+# config.yaml
+param: 1
+param2@eval: "config.param + 1"
+```
+
+```python
+proc = create_processing_value(
+    lambda x, config: eval(x, {"config": config}),
+    tag_name="eval",
+    persistent=False,
+)
+# (Note that the `eval` function is not safe and the code above
+# should not be used in case of untrusted config)
+```
+
+Here the value of `param2` will be evaluated to 2 at pre-merge step.
+
 ### Pre-merge/post-merge processing that protect a property from being modified
 
-An other useful kind of processing is a processing that ensure to keep a certain
+Another useful kind of processing is a processing that ensure to keep a certain
 property on the value. For this kind of processing, you can use
 `cliconfig.create_processing_keep_property`. It takes a function that returns
 the property from the value, the regex or the tag name like the previous function,
 and the order of the pre-merge and the post-merge.
 
 The pre-merge processing looks for keys that match the tag or the regex, apply
 the function on the value and store the result (= the "property").
-The post-merge processing will check that the property is the same as the one
-stored during pre-merge. If not, it will raise an error.
+The post-merge and end-build processing will check that the property is the same as
+the one stored during pre-merge. If not, it will raise an error.
 
 Examples:
 
 A processing that enforce the types of all the parameters to be constant
 (equal to the type of the first value encountered):
 
 ```python
 create_processing_keep_property(type, regex=".*", premerge_order=15.0,
-                                postmerge_order=15.0)
+                                postmerge_order=15.0, endbuild_order=15.0)
 ```
 
 A processing that protect parameters tagged with @protect from being changed:
 
 ```python
 create_processing_keep_property(lambda x: x, tag_name="protect",
-                                premerge_order=15.0, postmerge_order=15.0)
+                                premerge_order=15.0, postmerge_order=15.0,
+                                endbuild_order=15.0)
 ```
 
-Each time you choose the order `15.0` because it is a good values for processing that
-made checks on the values. Indeed processings that change the values such as
-`ProcessCopy` have an order that is generally <= 10.0.
+Each time you choose the order `15.0` because it is a good value for processing that
+made checks on the values. Indeed, processings that change the values such as
+`ProcessCopy` have an order that is generally $\leq$ 10.0.
+
+It is also possible to pass the flat config as a second argument to the function
+similarly to `create_processing_value`.
 
 ## Create your processing classes (Advanced)
 
 To create your own processing classes and unlock more possibilities, you simply
 need to overload the methods of the Processing class to modify the config at the
 desired timings. To do so, you often need to manipulate tags.
 
 ### Manipulate the tags
 
 Tags are useful for triggering a processing, as we have seen. However, we need
 to be cautious because tagging a key modifies its name and can lead to conflicts
 when using processing. To address this issue, we provide tag routines in
 `cliconfig.tag_routines`. These routines include:
 
-* `is_tag_in`: Checks if a tag is in a key. It look for the exact tag name.
-  If `full_key` is True, it looks for all the fkat key, including sub-configs
+* `is_tag_in`: Checks if a tag is in a key. It looks for the exact tag name.
+  If `full_key` is True, it looks for all the flat key, including sub-configs
   (default: False)
 * `clean_tag`: Removes a specific tag (based on its exact name) from a key.
   It is helpful to remove the tag after pre-merging.
 * `clean_all_tags`: Removes all tags from a key. This is helpful each time you
   need the true parameter name.
 * `clean_dict_tags`: Removes all tags from a dictionary and returns the cleaned
   dict along with a list of keys that contained tags. This is helpful to get all
   the parameter names of a full dict with tags.
 
 With these tools, we can write a processing, for example, that searches for all
-parameters with a tag @look ant that prints their sorted values at the end of
+parameters with a tag `@look` ant that prints their sorted values at the end of
 the post-merging.
 
 ```python
 class ProcessPrintSorted(Processing):
     """Print the parameters tagged with "@look", sorted by value on post-merge."""
 
     def __init__(self) -> None:
@@ -261,21 +282,21 @@
 These three operations are in `cliconfig.process_routines` and called
 `merge_processing`, `save_processing`, and `load_processing`, respectively. They
 takes as input a Config object that contains as we see the list of processing.
 
 Now, the trick is that sometimes we want to apply these operations to the processing
 themselves, particularly when we want to modify a part of the configuration instead
 of just a single parameter (such as merging two configurations). This is why it is
-particularly useful to have an access to the full Config object and not only the
+particularly useful to have access to the full Config object and not only the
 dict.
 
-For example, consider the tag "@merge_add," which triggers a processing before
+For example, consider the tag `@merge_add`, which triggers a processing before
 merging and merges the config loaded from a specified path (the value) into the
 current config. We may want to see what happens if we merge a config that also
-contains an "@merge_add" tag within it:
+contains a `@merge_add` tag within it:
 
 ```yaml
 # main.yaml
 config_path1@merge_add: path1.yaml
 # path1.yaml
 param1: 1
 config_path2@merge_add: path2.yaml
@@ -304,21 +325,21 @@
 
 ### Change processing list in processing (Still more advanced)
 
 Note that the processing functions receive the list of processing objects as an
 input and update as an attribute of the processing object. This means that it
 is possible to manually modify this list in processing functions.
 
-**Disclaimer**: The processing list to apply during pre/post-merge, pre-save and
+**Warning**: The processing list to apply during pre/post-merge, pre-save and
 post-load are determined before the first processing is applied. Therefore, you can't
 add or remove processing and expect it to be effective during the current merge/save/load.
 However, if you modify their internal variables it will be effective immediately.
 
 Here an example of a processing that remove the type check of a parameter in
-`ProcessTyping` processing. It is then possible for instance to force an other
+`ProcessTyping` processing. It is then possible for instance to force another
 type (it is not possible otherwise).
 
 ```python
 from cliconfig.processing.builtin import ProcessTyping
 
 class ProcessBypassTyping(Processing):
     """Bypass type check of ProcessTyping for parameters tagged with "@bypass_typing".
@@ -348,17 +369,17 @@
                             and clean_key in processing.forced_types):
                         forced_type = processing.forced_types.pop(clean_key)
                         self.bypassed_forced_types[clean_key] = forced_type
         return flat_config
 
 # Without bypass:
 config1 = Config({"a@type:int": 0}, [ProcessBypassTyping(), ProcessTyping()])
-config2 = Config({"a@bypass_typing@type:str": "a"}, [])
+config2 = Config({"a@type:str": "a"}, [])
 config = merge_flat_processing(config1, config2)
-# Error: try to change the forced type of "a" from int to str
+# > Error: try to change the forced type of "a" from int to str
 
 # With bypass:
 config1 = Config({"a@type:int": 0}, [ProcessBypassTyping(), ProcessTyping()])
 config2 = Config({"a@bypass_typing@type:str": "a"}, [])
 config = merge_flat_processing(config1, config2)
-# No error
+# > No error
 ```
```

### Comparing `cliconfig-1.0.0b4/docs/quickstart.md` & `cliconfig-1.0.0rc1/docs/quickstart.md`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 For example:
 
 ```bash
 python main.py --config first.yaml,second.yaml --param2=-2 --letters.letter2='B'
 ```
 
 *Note*: the additional configs are detected with `--config` followed by space
-and separated by comma(s) **without space**. It also possible to pass a list.
+and separated by comma(s) **without space**. It is also possible to pass a list.
 The parameters are detected with the pattern `--<param>=<value>` without spaces.
 
 It will show:
 
 ```text
 [CONFIG] Merge 2 default configs, 2 additional configs and 2 CLI parameter(s).
 
@@ -119,15 +119,15 @@
   after each update, even if the tag is no longer present. It supports basic types
   (except for tuples and sets, which are not handled by YAML) as well as unions
   (using "Union" or "|"), optional values, nested list, and nested dict.
   For instance: `@type:List[Dict[str, int|float]]`.
 * `@select`: This tag select sub-config(s) to keep and delete the other
   sub-configs in the same parent config
 * `@delete`: This tag deletes the key from the config before merging.
-* `@new`: This tag allows to add new key(s) to the config that are not already
+* `@new`: This tag allows adding new key(s) to the config that are not already
   present in the default config(s). It can be used for single parameter or a
   sub-config. Disclaimer: it is preferable to have exhaustive default config(s)
   instead of abusing this tag for readability and for security concerning typos.
 
 The tags are applied in the following order: `@merge`, `@select`, `@copy`, `@type`
 and then `@delete`.
```

### Comparing `cliconfig-1.0.0b4/github_actions_utils/pydocstyle_manager.py` & `cliconfig-1.0.0rc1/github_actions_utils/pydocstyle_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b4/github_actions_utils/pylint_manager.py` & `cliconfig-1.0.0rc1/github_actions_utils/pylint_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b4/github_actions_utils/pytest_manager.py` & `cliconfig-1.0.0rc1/github_actions_utils/pytest_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b4/licenses_tier/FLATTEN_DICT_LICENSE` & `cliconfig-1.0.0rc1/licenses_tier/FLATTEN_DICT_LICENSE`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b4/pre-commit-checks.sh` & `cliconfig-1.0.0rc1/pre-commit-checks.sh`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b4/pyproject.toml` & `cliconfig-1.0.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b4/tests/configs/integration/test2/default.yaml` & `cliconfig-1.0.0rc1/tests/configs/integration/test2/default.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b4/tests/conftest.py` & `cliconfig-1.0.0rc1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b4/tests/integration/test_inte_multiple_tags.py` & `cliconfig-1.0.0rc1/tests/integration/test_inte_multiple_tags.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b4/tests/unit/processing/test_base_processing.py` & `cliconfig-1.0.0rc1/tests/unit/processing/test_base_processing.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b4/tests/unit/processing/test_builtin.py` & `cliconfig-1.0.0rc1/tests/unit/processing/test_builtin.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b4/tests/unit/processing/test_create.py` & `cliconfig-1.0.0rc1/tests/unit/test_process_routines.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,104 +1,137 @@
-"""Test helpers to create processing functions."""
+"""Tests for dict routines with preprocessing."""
 import re
+import shutil
 
 import pytest
 import pytest_check as check
+import yaml
 
 from cliconfig.base import Config
-from cliconfig.processing.create import (
-    create_processing_keep_property,
-    create_processing_value,
+from cliconfig.process_routines import (
+    end_build_processing,
+    load_processing,
+    merge_flat_paths_processing,
+    merge_flat_processing,
+    save_processing,
 )
+from cliconfig.processing.base import Processing
+from tests.conftest import ProcessAdd1, ProcessKeep
 
 
-def test_create_processing_value() -> None:
-    """Test create_processing_value."""
-    # Persistent
-    proc1 = create_processing_value(
-        lambda x: x + 1, tag_name="add1", order=1.0, persistent=True
-    )
-    proc2 = create_processing_value(
-        lambda x: -x, regex="neg_number.*", order=0.0, persistent=True
-    )
-    in_dict = {"neg_number1": 1, "neg_number2": 1, "neg_number3@add1": 1}
-    config = Config(in_dict, [proc1, proc2])
-    config = config.process_list[1].premerge(config)
-    config = config.process_list[0].premerge(config)
-    check.equal(in_dict, {"neg_number1": -1, "neg_number2": -1, "neg_number3": 0})
-    config = config.process_list[1].premerge(config)
-    config = config.process_list[0].premerge(config)
-    check.equal(in_dict, {"neg_number1": 1, "neg_number2": 1, "neg_number3": 1})
-    # Non persistent
-    proc2 = create_processing_value(
-        lambda x: -x, regex="neg_number.*", order=0.0, persistent=False
-    )
-    proc1 = create_processing_value(
-        lambda x: x + 1, tag_name="add1", order=1.0, persistent=False
-    )
-    in_dict = {"neg_number1": 1, "neg_number2": 1, "neg_number3@add1": 1}
-    config = Config(in_dict, [proc1, proc2])
-    config = config.process_list[1].premerge(config)
-    config = config.process_list[0].premerge(config)
-    check.equal(in_dict, {"neg_number1": -1, "neg_number2": -1, "neg_number3": 0})
-    config = config.process_list[1].premerge(config)
-    config = config.process_list[0].premerge(config)
-    check.equal(in_dict, {"neg_number1": 1, "neg_number2": 1, "neg_number3": 0})
+def test_merge_flat_processing(
+    process_add1: ProcessAdd1,
+    process_keep: ProcessKeep,
+) -> None:
+    """Test merge_flat_processing."""
+
+    class _ProcessingTest(Processing):
+        def __init__(self) -> None:
+            super().__init__()
+            self.attr = 0
+
+    proc1 = _ProcessingTest()
+    proc2 = _ProcessingTest()
+    proc2.attr = 1
+    proc3 = _ProcessingTest()
+
+    config1 = Config({"a": {"b": 1, "c": 2, "d@keep": 3}}, [proc1, proc2, process_add1])
+    config2 = Config({"a": {"b": 2, "c@add1": 3, "d": 4}}, [proc3, process_keep])
+    config = merge_flat_processing(
+        config1,
+        config2,
+        allow_new_keys=False,
+    )
+    check.equal(
+        config.dict,
+        {"a.b": 2, "a.c": 4, "a.d": 3},
+    )
+    check.equal(config.process_list, [proc1, proc2, process_add1, process_keep])
+    check.equal(process_keep.keep_vals, {})
 
-    # Failing cases
-    with pytest.raises(
-        ValueError, match="You must provide a tag or a regex but not both."
-    ):
-        create_processing_value(lambda x: x + 1, tag_name="add1", regex="neg_number.*")
-    with pytest.raises(
-        ValueError,
-        match=re.escape(
-            "You must provide a tag or a regex (to trigger the value update)."
+
+def test_merge_flat_paths_processing(
+    process_add1: ProcessAdd1,
+    process_keep: ProcessKeep,
+) -> None:
+    """Test merge_flat_paths_processing."""
+    config1 = Config(
+        {"param1@add1": 0, "param2.param3@keep": 1}, [process_add1, process_keep]
+    )
+    config2 = Config({"param2.param3": 3}, [])
+    expected_dict = {"param1": 1, "param2.param3": 1}
+    check.equal(
+        merge_flat_paths_processing(
+            "tests/configs/configtag1.yaml",
+            "tests/configs/configtag2.yaml",
+            allow_new_keys=False,
+            additional_process=[process_add1, process_keep],
         ),
-    ):
-        create_processing_value(lambda x: x + 1, order=0.0)
+        Config(expected_dict, [process_add1, process_keep]),
+    )
+    check.equal(
+        merge_flat_paths_processing(
+            config1,
+            config2,
+            allow_new_keys=False,
+        ),
+        Config(expected_dict, [process_add1, process_keep]),
+    )
+    check.equal(process_keep.keep_vals, {})
 
+    # Case with dict in input
 
-def test_create_processing_keep_property() -> None:
-    """Test create_processing_keep_property."""
-    proc1 = create_processing_keep_property(type, regex=".*")
-    proc2 = create_processing_keep_property(lambda x: x, tag_name="protect")
-    in_dict = {"str": "foo", "int": 2, "list@protect": [1, 2, 3]}
-    config = Config(in_dict, [proc1, proc2])
-    config = config.process_list[0].premerge(config)
-    config = config.process_list[1].premerge(config)
-    check.equal(config.dict, {"str": "foo", "int": 2, "list": [1, 2, 3]})
-    config = config.process_list[0].postmerge(config)
-    config = config.process_list[1].postmerge(config)
+
+def test_save_processing(
+    process_add1: ProcessAdd1,
+    process_keep: ProcessKeep,
+) -> None:
+    """Test save_processing."""
+    config = Config(
+        {"param1@add1": 0, "param2.param3@add1": 1}, [process_add1, process_keep]
+    )
+    save_processing(config, "tests/tmp/config.yaml")
+    with open("tests/tmp/config.yaml", "r", encoding="utf-8") as yaml_file:
+        loaded_dict = yaml.safe_load(yaml_file)
+    check.equal(loaded_dict, {"param1": 1, "param2": {"param3": 2}})
+    check.equal(process_keep.keep_vals, {})
+    shutil.rmtree("tests/tmp")
+
+
+def test_load_processing(
+    process_add1: ProcessAdd1,
+    process_keep: ProcessKeep,
+) -> None:
+    """Test load_processing."""
+    process_keep.keep_vals = {"param2.param3": 0}
+    config = load_processing(
+        "tests/configs/configtag2.yaml",
+        [process_add1, process_keep],
+    )
+    check.equal(config.dict, {"param2.param3": 0})
     with pytest.raises(
         ValueError,
         match=re.escape(
-            "Property of key str has changed from <class 'str'> to <class 'int'> "
-            "while it is protected by a keep-property processing (problem found on "
-            "post-merge)."
+            "config_or_path must be a Config instance or a path to a yaml file "
+            "but you passed a dict. If you want to use it as a valid input, "
+            "you should use Config(<input dict>, []) instead."
         ),
     ):
-        config.process_list[0].postmerge(Config({"str": 0}, []))
+        merge_flat_paths_processing(
+            {"a": 2},  # type: ignore
+            Config({"a": 1}, []),
+        )
     with pytest.raises(
         ValueError,
-        match=re.escape(
-            "Property of key list has changed from [1, 2, 3] to [1, 2] while "
-            "it is protected by a keep-property processing (problem found on "
-            "post-merge)."
-        ),
+        match=("config_or_path must be a Config instance or a path to a yaml file."),
     ):
-        config.process_list[1].postmerge(Config({"list": [1, 2]}, []))
-    config.process_list[0].premerge(Config({"str": 0}, []))  # should not raise
-    config.process_list[1].premerge(Config({"list": [1, 2]}, []))  # should not raise
+        merge_flat_paths_processing(
+            Config({"a": 1}, []),
+            ("not a path",),  # type: ignore
+        )
 
-    # Failing cases
-    with pytest.raises(
-        ValueError, match="You must provide a tag or a regex but not both."
-    ):
-        create_processing_keep_property(lambda x: x, tag_name="protect", regex=".*")
-    with pytest.raises(
-        ValueError,
-        match=re.escape(
-            "You must provide a tag or a regex (to trigger the value update)."
-        ),
-    ):
-        create_processing_keep_property(lambda x: x, premerge_order=0.0)
+
+def test_end_build_processing(process_add1: ProcessAdd1) -> None:
+    """Test end_build_processing."""
+    config = Config({"param1@add1": 0}, [process_add1])
+    config = end_build_processing(config)
+    check.equal(config.dict, {"param1@add1": 0, "processing name": "ProcessAdd1"})
```

### Comparing `cliconfig-1.0.0b4/tests/unit/processing/test_type_parser.py` & `cliconfig-1.0.0rc1/tests/unit/processing/test_type_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b4/tests/unit/test_base_config.py` & `cliconfig-1.0.0rc1/tests/unit/test_base_config.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b4/tests/unit/test_cli_parser.py` & `cliconfig-1.0.0rc1/tests/unit/test_cli_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b4/tests/unit/test_config_routines.py` & `cliconfig-1.0.0rc1/tests/unit/test_config_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b4/tests/unit/test_dict_routines.py` & `cliconfig-1.0.0rc1/tests/unit/test_dict_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b4/tests/unit/test_ex_docs.py` & `cliconfig-1.0.0rc1/tests/integration/test_ex_docs.py`

 * *Files identical despite different names*

### Comparing `cliconfig-1.0.0b4/tests/unit/test_tag_routines.py` & `cliconfig-1.0.0rc1/tests/unit/test_tag_routines.py`

 * *Files identical despite different names*

